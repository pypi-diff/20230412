# Comparing `tmp/pydantic-2.0a1.tar.gz` & `tmp/pydantic-2.0a2.tar.gz`

## Comparing `pydantic-2.0a1.tar` & `pydantic-2.0a2.tar`

### file list

```diff
@@ -1,156 +1,165 @@
--rw-r--r--   0        0        0    79101 2020-02-02 00:00:00.000000 pydantic-2.0a1/HISTORY.md
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pydantic-2.0a1/Makefile
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pydantic-2.0a1/README.md
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/__init__.py
--rw-r--r--   0        0        0    14399 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_hypothesis_plugin.py
--rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/analyzed_type.py
--rw-r--r--   0        0        0    17735 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/color.py
--rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/config.py
--rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/dataclasses.py
--rw-r--r--   0        0        0    10288 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/decorator.py
--rw-r--r--   0        0        0    17882 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/decorators.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/errors.py
--rw-r--r--   0        0        0    19522 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/fields.py
--rw-r--r--   0        0        0    55802 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/json_schema.py
--rw-r--r--   0        0        0    40735 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/main.py
--rw-r--r--   0        0        0    38215 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/mypy.py
--rw-r--r--   0        0        0    10019 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/networks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/py.typed
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/tools.py
--rw-r--r--   0        0        0    27024 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/types.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/__init__.py
--rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_core_metadata.py
--rw-r--r--   0        0        0    14440 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_core_utils.py
--rw-r--r--   0        0        0     5482 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_dataclasses.py
--rw-r--r--   0        0        0    27180 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_decorators.py
--rw-r--r--   0        0        0    20993 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_discriminated_union.py
--rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_fields.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_forward_ref.py
--rw-r--r--   0        0        0    52319 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_generate_schema.py
--rw-r--r--   0        0        0    18546 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_generics.py
--rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_model_construction.py
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_repr.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_serializers.py
--rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_std_types_schema.py
--rw-r--r--   0        0        0    16040 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_typing_extra.py
--rw-r--r--   0        0        0    12890 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_utils.py
--rw-r--r--   0        0        0    16337 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/_internal/_validators.py
--rw-r--r--   0        0        0     7234 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/deprecated/copy_internals.py
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/deprecated/json.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pydantic-2.0a1/pydantic/deprecated/parse.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/README.md
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/all.in
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/all.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/docs-constrained.in
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/docs.in
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/docs.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/linting-constrained.in
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/linting.in
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/linting.txt
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/pyproject-all.txt
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/pyproject-min.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/pyproject.toml-constrained.in
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/pyproject.toml-extras-constrained.in
--rwxr-xr-x   0        0        0      354 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/rebuild.sh
--rwxr-xr-x   0        0        0     1193 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/refresh.sh
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/testing-constrained.in
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/testing-extra-constrained.in
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/testing-extra.in
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/testing-extra.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/testing.in
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pydantic-2.0a1/requirements/testing.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/conftest.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_abc.py
--rw-r--r--   0        0        0     8250 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_aliases.py
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_annotated.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_assert_in_validators.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_callable.py
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_color.py
--rw-r--r--   0        0        0    16922 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_config.py
--rw-r--r--   0        0        0    12768 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_construction.py
--rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_create_model.py
--rw-r--r--   0        0        0    44695 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_dataclasses.py
--rw-r--r--   0        0        0    17722 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_datetime.py
--rw-r--r--   0        0        0    14418 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_decorator.py
--rw-r--r--   0        0        0    10550 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_deprecated.py
--rw-r--r--   0        0        0    40402 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_discriminated_union.py
--rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_docs.py
--rw-r--r--   0        0        0    71861 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_edge_cases.py
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_fastapi.sh
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_fastapi_json_schema.py
--rw-r--r--   0        0        0    27889 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_forward_ref.py
--rw-r--r--   0        0        0    61906 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_generics.py
--rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_hypothesis_plugin.py
--rw-r--r--   0        0        0    11516 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_json.py
--rw-r--r--   0        0        0   107660 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_json_schema.py
--rw-r--r--   0        0        0    57933 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_main.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_model_signature.py
--rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_networks.py
--rw-r--r--   0        0        0    15516 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_networks_ipaddress.py
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_parse.py
--rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_private_attributes.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_rich_repr.py
--rw-r--r--   0        0        0    12760 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_serialize.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_strict.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_structural_pattern_matching.py
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_tools.py
--rw-r--r--   0        0        0   112615 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_types.py
--rw-r--r--   0        0        0     4255 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_types_namedtuple.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_types_payment_card_number.py
--rw-r--r--   0        0        0    19116 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_types_typeddict.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_typing.py
--rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_utils.py
--rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_validator.py
--rw-r--r--   0        0        0    55729 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_validators.py
--rwxr-xr-x   0        0        0     4675 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_validators_dataclass.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/__init__.py
--rw-r--r--   0        0        0    10178 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/test_mypy.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/configs/mypy-plugin-strict-no-any.ini
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/configs/mypy-plugin-strict.ini
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/configs/mypy-plugin.ini
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/configs/pyproject-default.toml
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/configs/pyproject-plugin-bad-param.toml
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/configs/pyproject-plugin-strict.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/configs/pyproject-plugin.toml
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/custom_constructor.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/dataclass_no_any.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/fail1.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/fail2.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/fail3.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/fail4.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/fail_defaults.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/plugin_default_factory.py
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/plugin_fail.py
--rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/plugin_fail_baseConfig.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/plugin_success.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/plugin_success_baseConfig.py
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/modules/success.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/custom_constructor.txt
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/fail1.txt
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/fail2.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/fail3.txt
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/fail4.txt
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/fail_defaults.txt
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/plugin-fail-strict.txt
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/plugin-fail.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/plugin-success-strict-baseConfig.txt
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/plugin-success-strict.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/plugin_default_factory.txt
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/plugin_success.txt
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/latest/plugin_success_baseConfig.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/v1.0.1/fail1.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/v1.0.1/fail2.txt
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/v1.0.1/plugin_success.txt
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/mypy/outputs/v1.0.1/plugin_success_baseConfig.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/pyright/pyproject.toml
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pydantic-2.0a1/tests/pyright/pyright_example.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 pydantic-2.0a1/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.0a1/LICENSE
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 pydantic-2.0a1/pyproject.toml
--rw-r--r--   0        0        0   114402 2020-02-02 00:00:00.000000 pydantic-2.0a1/PKG-INFO
+-rw-r--r--   0        0        0    79249 2020-02-02 00:00:00.000000 pydantic-2.0a2/HISTORY.md
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 pydantic-2.0a2/Makefile
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 pydantic-2.0a2/README.md
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/__init__.py
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_hypothesis_plugin.py
+-rw-r--r--   0        0        0    12585 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/analyzed_type.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/annotated_arguments.py
+-rw-r--r--   0        0        0    21194 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/color.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/config.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/dataclasses.py
+-rw-r--r--   0        0        0    10239 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/decorator.py
+-rw-r--r--   0        0        0    21874 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/decorators.py
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/errors.py
+-rw-r--r--   0        0        0    22697 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/fields.py
+-rw-r--r--   0        0        0    56158 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/json_schema.py
+-rw-r--r--   0        0        0    43761 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/main.py
+-rw-r--r--   0        0        0    38032 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/mypy.py
+-rw-r--r--   0        0        0    10041 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/networks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/py.typed
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/tools.py
+-rw-r--r--   0        0        0    27028 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/types.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/__init__.py
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_config.py
+-rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_core_metadata.py
+-rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_core_utils.py
+-rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_dataclasses.py
+-rw-r--r--   0        0        0    23749 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_decorators.py
+-rw-r--r--   0        0        0    21314 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_discriminated_union.py
+-rw-r--r--   0        0        0    10660 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_fields.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_forward_ref.py
+-rw-r--r--   0        0        0    54529 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_generate_schema.py
+-rw-r--r--   0        0        0    19390 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_generics.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_internal_dataclass.py
+-rw-r--r--   0        0        0    12704 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_model_construction.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_repr.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_serializers.py
+-rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_std_types_schema.py
+-rw-r--r--   0        0        0    16243 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_typing_extra.py
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_utils.py
+-rw-r--r--   0        0        0    16778 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/_internal/_validators.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/deprecated/config.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/deprecated/copy_internals.py
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/deprecated/json.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 pydantic-2.0a2/pydantic/deprecated/parse.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/README.md
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/all.in
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/all.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/docs-constrained.in
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/docs.in
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/docs.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/linting-constrained.in
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/linting.in
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/linting.txt
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/pyproject-all.txt
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/pyproject-min.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/pyproject.toml-constrained.in
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/pyproject.toml-extras-constrained.in
+-rwxr-xr-x   0        0        0      374 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/rebuild.sh
+-rwxr-xr-x   0        0        0     1327 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/refresh.sh
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-constrained.in
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-extra-constrained.in
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-extra.in
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-extra.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-mypy-constrained.in
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-mypy.in
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing-mypy.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing.in
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 pydantic-2.0a2/requirements/testing.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/conftest.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_abc.py
+-rw-r--r--   0        0        0    12622 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_aliases.py
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_annotated.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_assert_in_validators.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_callable.py
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_color.py
+-rw-r--r--   0        0        0    18778 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_config.py
+-rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_construction.py
+-rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_create_model.py
+-rw-r--r--   0        0        0    43910 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_dataclasses.py
+-rw-r--r--   0        0        0    17722 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_datetime.py
+-rw-r--r--   0        0        0    14403 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_decorator.py
+-rw-r--r--   0        0        0    15412 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_deprecated.py
+-rw-r--r--   0        0        0    40131 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_discriminated_union.py
+-rw-r--r--   0        0        0     6223 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_docs.py
+-rw-r--r--   0        0        0    70040 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_edge_cases.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_errors.py
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_fastapi.sh
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_fastapi_json_schema.py
+-rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_forward_ref.py
+-rw-r--r--   0        0        0    62435 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_generics.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_hypothesis_plugin.py
+-rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_json.py
+-rw-r--r--   0        0        0   107645 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_json_schema.py
+-rw-r--r--   0        0        0    61586 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_main.py
+-rw-r--r--   0        0        0     5631 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_model_signature.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_model_validator.py
+-rw-r--r--   0        0        0    27311 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_networks.py
+-rw-r--r--   0        0        0    15512 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_networks_ipaddress.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_parse.py
+-rw-r--r--   0        0        0     8552 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_private_attributes.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_rich_repr.py
+-rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_serialize.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_strict.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_structural_pattern_matching.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_tools.py
+-rw-r--r--   0        0        0   122508 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_types.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_types_namedtuple.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_types_payment_card_number.py
+-rw-r--r--   0        0        0    19655 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_types_typeddict.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_typing.py
+-rw-r--r--   0        0        0    14575 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_utils.py
+-rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_validator.py
+-rw-r--r--   0        0        0    66969 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_validators.py
+-rwxr-xr-x   0        0        0     4663 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_validators_dataclass.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/__init__.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/test_mypy.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/mypy-plugin-strict-no-any.ini
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/mypy-plugin-strict.ini
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/mypy-plugin.ini
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/pyproject-default.toml
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/pyproject-plugin-bad-param.toml
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/pyproject-plugin-strict.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/configs/pyproject-plugin.toml
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/custom_constructor.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/dataclass_no_any.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/fail1.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/fail2.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/fail3.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/fail4.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/fail_defaults.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/plugin_default_factory.py
+-rw-r--r--   0        0        0     5822 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/plugin_fail.py
+-rw-r--r--   0        0        0     5840 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/plugin_fail_baseConfig.py
+-rw-r--r--   0        0        0     5611 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/plugin_success.py
+-rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/plugin_success_baseConfig.py
+-rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/modules/success.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/custom_constructor.txt
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/fail1.txt
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/fail2.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/fail3.txt
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/fail4.txt
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/fail_defaults.txt
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-strict.txt
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-success-strict-baseConfig.txt
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin-success-strict.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin_default_factory.txt
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin_success.txt
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/latest/plugin_success_baseConfig.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/v1.0.1/fail1.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/v1.0.1/fail2.txt
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/v1.0.1/plugin_success.txt
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/mypy/outputs/v1.0.1/plugin_success_baseConfig.txt
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/pyright/pyproject.toml
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 pydantic-2.0a2/tests/pyright/pyright_example.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pydantic-2.0a2/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pydantic-2.0a2/LICENSE
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 pydantic-2.0a2/pyproject.toml
+-rw-r--r--   0        0        0   114550 2020-02-02 00:00:00.000000 pydantic-2.0a2/PKG-INFO
```

### Comparing `pydantic-2.0a1/HISTORY.md` & `pydantic-2.0a2/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v2.0a2 (2023-04-12)
+
+Second pre-release of Pydantic V2
+
+See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0a2)
+
 ## v2.0a1 (2023-04-03)
 
 First pre-release of Pydantic V2!
 
 See [this post](https://docs.pydantic.dev/blog/pydantic-v2-alpha/) for more details.
 
 ## v1.10.7 (2023-03-22)
```

### Comparing `pydantic-2.0a1/Makefile` & `pydantic-2.0a2/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .DEFAULT_GOAL := all
 sources = pydantic tests docs/plugins
 
 .PHONY: install
 install:
 	python -m pip install -U pip
 	pip install -r requirements/all.txt
+	pip install -r requirements/pyproject-all.txt
 	pip install -e .
 
 .PHONY: refresh-lockfiles
 refresh-lockfiles:       ## Sync lockfiles with requirements files.
 	bash requirements/refresh.sh
 
 
@@ -24,19 +25,15 @@
 .PHONY: lint
 lint:
 	ruff $(sources)
 	black $(sources) --check --diff
 
 .PHONY: typecheck
 typecheck:
-	mypy pydantic --disable-recursive-aliases --config-file .mypy-configs/full.toml
-
-.PHONY: typecheck-fast
-typecheck-fast:
-	mypy pydantic --disable-recursive-aliases --config-file .mypy-configs/fast.toml
+	pre-commit run typecheck --all-files
 
 .PHONY: test-mypy
 test-mypy:
 	coverage run -m pytest tests/mypy --test-mypy
 
 .PHONY: test-pyright
 test-pyright:
@@ -63,25 +60,24 @@
 
 .PHONY: test-fastapi
 test-fastapi:
 	git clone https://github.com/tiangolo/fastapi.git --single-branch
 	./tests/test_fastapi.sh
 
 .PHONY: all
-all: lint typecheck-fast testcov
+all: lint typecheck testcov
 
 .PHONY: clean
 clean:
 	rm -rf `find . -name __pycache__`
 	rm -f `find . -type f -name '*.py[co]'`
 	rm -f `find . -type f -name '*~'`
 	rm -f `find . -type f -name '.*~'`
 	rm -rf .cache
 	rm -rf .pytest_cache
-	rm -rf .mypy_cache
 	rm -rf .ruff_cache
 	rm -rf htmlcov
 	rm -rf *.egg-info
 	rm -f .coverage
 	rm -f .coverage.*
 	rm -rf build
 	rm -rf dist
```

### Comparing `pydantic-2.0a1/README.md` & `pydantic-2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/pydantic/__init__.py` & `pydantic-2.0a2/pydantic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     SerializerFunctionWrapHandler,
     ValidationInfo,
     ValidatorFunctionWrapHandler,
 )
 
 from . import dataclasses
 from .analyzed_type import AnalyzedType
-from .config import BaseConfig, ConfigDict, Extra
+from .config import ConfigDict, Extra
 from .decorator import validate_arguments
 from .decorators import field_serializer, field_validator, model_serializer, root_validator, validator
+from .deprecated.config import BaseConfig
 from .errors import *
 from .fields import Field, PrivateAttr
 from .main import *
 from .networks import *
 from .tools import *
 from .types import *
 from .version import VERSION
@@ -105,14 +106,15 @@
     'condate',
     'UUID1',
     'UUID3',
     'UUID4',
     'UUID5',
     'FilePath',
     'DirectoryPath',
+    'NewPath',
     'Json',
     'SecretField',
     'SecretStr',
     'SecretBytes',
     'StrictBool',
     'StrictBytes',
     'StrictInt',
```

### Comparing `pydantic-2.0a1/pydantic/_hypothesis_plugin.py` & `pydantic-2.0a2/pydantic/_hypothesis_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 """
 THIS IS A MESS AND NEEDS TO BE REWRITTEN, SORRY ZAC.
 
 Register Hypothesis strategies for Pydantic custom types.
 
 This enables fully-automatic generation of test data for most Pydantic classes.
```

### Comparing `pydantic-2.0a1/pydantic/color.py` & `pydantic-2.0a2/pydantic/color.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
-Color definitions are  used as per CSS3 specification:
-http://www.w3.org/TR/css3-color/#svg-color
+Color definitions are used as per the CSS3
+[CSS Color Module Level 3](http://www.w3.org/TR/css3-color/#svg-color) specification.
 
 A few colors have multiple names referring to the sames colors, eg. `grey` and `gray` or `aqua` and `cyan`.
 
-In these cases the LAST color when sorted alphabetically takes preferences,
-eg. Color((0, 255, 255)).as_named() == 'cyan' because "cyan" comes after "aqua".
+In these cases the _last_ color when sorted alphabetically takes preferences,
+eg. `Color((0, 255, 255)).as_named() == 'cyan'` because "cyan" comes after "aqua".
 """
 import math
 import re
 from colorsys import hls_to_rgb, rgb_to_hls
 from typing import Any, Dict, Optional, Tuple, Union, cast
 
 from pydantic_core import PydanticCustomError, core_schema
@@ -59,14 +59,18 @@
 
 # colors where the two hex characters are the same, if all colors match this the short version of hex colors can be used
 repeat_colors = {int(c * 2, 16) for c in '0123456789abcdef'}
 rads = 2 * math.pi
 
 
 class Color(_repr.Representation):
+    """
+    Represents a color.
+    """
+
     __slots__ = '_original', '_rgba'
 
     def __init__(self, value: ColorType) -> None:
         self._rgba: RGBA
         self._original: ColorType
         if isinstance(value, (tuple, list)):
             self._rgba = parse_tuple(value)
@@ -86,66 +90,88 @@
     @classmethod
     def __pydantic_modify_json_schema__(cls, field_schema: Dict[str, Any]) -> Dict[str, Any]:
         field_schema.update(type='string', format='color')
         return field_schema
 
     def original(self) -> ColorType:
         """
-        Original value passed to Color
+        Original value passed to `Color`.
         """
         return self._original
 
     def as_named(self, *, fallback: bool = False) -> str:
+        """
+        Returns the name of the color if it can be found in `COLORS_BY_VALUE` dictionary,
+        otherwise returns the hexadecimal representation of the color or raises `ValueError`.
+
+        Args:
+            fallback (bool): If True, falls back to returning the hexadecimal representation of
+                the color instead of raising a ValueError when no named color is found.
+
+        Returns:
+            str: The name of the color, or the hexadecimal representation of the color.
+
+        Raises:
+            ValueError: When no named color is found and fallback is `False`.
+        """
         if self._rgba.alpha is None:
             rgb = cast(Tuple[int, int, int], self.as_rgb_tuple())
             try:
                 return COLORS_BY_VALUE[rgb]
             except KeyError as e:
                 if fallback:
                     return self.as_hex()
                 else:
                     raise ValueError('no named color found, use fallback=True, as_hex() or as_rgb()') from e
         else:
             return self.as_hex()
 
     def as_hex(self) -> str:
-        """
-        Hex string representing the color can be 3, 4, 6 or 8 characters depending on whether the string
+        """Returns the hexadecimal representation of the color.
+
+        Hex string representing the color can be 3, 4, 6, or 8 characters depending on whether the string
         a "short" representation of the color is possible and whether there's an alpha channel.
+
+        Returns:
+            str: The hexadecimal representation of the color.
         """
         values = [float_to_255(c) for c in self._rgba[:3]]
         if self._rgba.alpha is not None:
             values.append(float_to_255(self._rgba.alpha))
 
         as_hex = ''.join(f'{v:02x}' for v in values)
         if all(c in repeat_colors for c in values):
             as_hex = ''.join(as_hex[c] for c in range(0, len(as_hex), 2))
         return '#' + as_hex
 
     def as_rgb(self) -> str:
         """
-        Color as an rgb(<r>, <g>, <b>) or rgba(<r>, <g>, <b>, <a>) string.
+        Color as an `rgb(<r>, <g>, <b>)` or `rgba(<r>, <g>, <b>, <a>)` string.
         """
         if self._rgba.alpha is None:
             return f'rgb({float_to_255(self._rgba.r)}, {float_to_255(self._rgba.g)}, {float_to_255(self._rgba.b)})'
         else:
             return (
                 f'rgba({float_to_255(self._rgba.r)}, {float_to_255(self._rgba.g)}, {float_to_255(self._rgba.b)}, '
                 f'{round(self._alpha_float(), 2)})'
             )
 
     def as_rgb_tuple(self, *, alpha: Optional[bool] = None) -> ColorTuple:
         """
-        Color as an RGB or RGBA tuple; red, green and blue are in the range 0 to 255, alpha if included is
-        in the range 0 to 1.
+        Returns the color as an RGB or RGBA tuple.
 
-        :param alpha: whether to include the alpha channel, options are
-          None - (default) include alpha only if it's set (e.g. not None)
-          True - always include alpha,
-          False - always omit alpha,
+        Args:
+            alpha (Optional[bool]): Whether to include the alpha channel. There are three options for this input:
+                `None` (default): Include alpha only if it's set. (e.g. not `None`)
+                `True`: Always include alpha.
+                `False`: Always omit alpha.
+
+        Returns:
+            ColorTuple: A tuple that contains the values of the red, green, and blue channels in the range 0 to 255.
+            If alpha is included, it is in the range 0 to 1.
         """
         r, g, b = (float_to_255(c) for c in self._rgba[:3])
         if alpha is None:
             if self._rgba.alpha is None:
                 return r, g, b
             else:
                 return r, g, b, self._alpha_float()
@@ -153,34 +179,39 @@
             return r, g, b, self._alpha_float()
         else:
             # alpha is False
             return r, g, b
 
     def as_hsl(self) -> str:
         """
-        Color as an hsl(<h>, <s>, <l>) or hsl(<h>, <s>, <l>, <a>) string.
+        Color as an `hsl(<h>, <s>, <l>)` or `hsl(<h>, <s>, <l>, <a>)` string.
         """
         if self._rgba.alpha is None:
             h, s, li = self.as_hsl_tuple(alpha=False)  # type: ignore
             return f'hsl({h * 360:0.0f}, {s:0.0%}, {li:0.0%})'
         else:
             h, s, li, a = self.as_hsl_tuple(alpha=True)  # type: ignore
             return f'hsl({h * 360:0.0f}, {s:0.0%}, {li:0.0%}, {round(a, 2)})'
 
     def as_hsl_tuple(self, *, alpha: Optional[bool] = None) -> HslColorTuple:
         """
-        Color as an HSL or HSLA tuple, e.g. hue, saturation, lightness and optionally alpha; all elements are in
-        the range 0 to 1.
+        Returns the color as an HSL or HSLA tuple.
 
-        NOTE: this is HSL as used in HTML and most other places, not HLS as used in python's colorsys.
+        Args:
+            alpha (Optional[bool]): Whether to include the alpha channel.
+                `None` (default): Include the alpha channel only if it's set (e.g. not `None`).
+                `True`: Always include alpha.
+                `False`: Always omit alpha.
+
+        Returns:
+            HslColorTuple: The color as a tuple of hue, saturation, lightness, and alpha (if included).
+                All elements are in the range 0 to 1.
 
-        :param alpha: whether to include the alpha channel, options are
-          None - (default) include alpha only if it's set (e.g. not None)
-          True - always include alpha,
-          False - always omit alpha,
+        Note:
+            This is HSL as used in HTML and most other places, not HLS as used in Python's `colorsys`.
         """
         h, l, s = rgb_to_hls(self._rgba.r, self._rgba.g, self._rgba.b)  # noqa: E741
         if alpha is None:
             if self._rgba.alpha is None:
                 return h, s, l
             else:
                 return h, s, l, self._alpha_float()
@@ -213,35 +244,55 @@
         return isinstance(other, Color) and self.as_rgb_tuple() == other.as_rgb_tuple()
 
     def __hash__(self) -> int:
         return hash(self.as_rgb_tuple())
 
 
 def parse_tuple(value: Tuple[Any, ...]) -> RGBA:
-    """
-    Parse a tuple or list as a color.
+    """Parse a tuple or list to get RGBA values.
+
+    Args:
+        value (Tuple[Any, ...]): A tuple or list.
+
+    Returns:
+        RGBA: An RGBA tuple parsed from the input tuple.
+
+    Raises:
+        PydanticCustomError: If tuple is not valid.
     """
     if len(value) == 3:
         r, g, b = (parse_color_value(v) for v in value)
         return RGBA(r, g, b, None)
     elif len(value) == 4:
         r, g, b = (parse_color_value(v) for v in value[:3])
         return RGBA(r, g, b, parse_float_alpha(value[3]))
     else:
         raise PydanticCustomError('color_error', 'value is not a valid color: tuples must have length 3 or 4')
 
 
 def parse_str(value: str) -> RGBA:
     """
-    Parse a string to an RGBA tuple, trying the following formats (in this order):
-    * named color, see COLORS_BY_NAME below
+    Parse a string representing a color to an RGBA tuple.
+
+    Possible formats for the input string include:
+
+    * named color, see `COLORS_BY_NAME`
     * hex short eg. `<prefix>fff` (prefix can be `#`, `0x` or nothing)
     * hex long eg. `<prefix>ffffff` (prefix can be `#`, `0x` or nothing)
-    * `rgb(<r>, <g>, <b>) `
+    * `rgb(<r>, <g>, <b>)`
     * `rgba(<r>, <g>, <b>, <a>)`
+
+    Args:
+        value (str): A string representing a color.
+
+    Returns:
+        RGBA: An RGBA tuple parsed from the input string.
+
+    Raises:
+        ValueError: If the input string cannot be parsed to an RGBA tuple.
     """
     value_lower = value.lower()
     try:
         r, g, b = COLORS_BY_NAME[value_lower]
     except KeyError:
         pass
     else:
@@ -275,21 +326,42 @@
     if m:
         return parse_hsl(*m.groups())  # type: ignore
 
     raise PydanticCustomError('color_error', 'value is not a valid color: string not recognised as a valid color')
 
 
 def ints_to_rgba(r: Union[int, str], g: Union[int, str], b: Union[int, str], alpha: Optional[float] = None) -> RGBA:
+    """
+    Converts integer or string values for RGB color and an optional alpha value to an `RGBA` object.
+
+    Args:
+        r (Union[int, str]): An integer or string representing the red color value.
+        g (Union[int, str]): An integer or string representing the green color value.
+        b (Union[int, str]): An integer or string representing the blue color value.
+        alpha (float, optional): A float representing the alpha value. Defaults to None.
+
+    Returns:
+        RGBA: An instance of the `RGBA` class with the corresponding color and alpha values.
+    """
     return RGBA(parse_color_value(r), parse_color_value(g), parse_color_value(b), parse_float_alpha(alpha))
 
 
 def parse_color_value(value: Union[int, str], max_val: int = 255) -> float:
     """
-    Parse a value checking it's a valid int in the range 0 to max_val and divide by max_val to give a number
-    in the range 0 to 1
+    Parse the color value provided and return a number between 0 and 1.
+
+    Args:
+        value (Union[int, str]): An integer or string color value.
+        max_val (int, optional): Maximum range value. Defaults to 255.
+
+    Raises:
+        PydanticCustomError: If the value is not a valid color.
+
+    Returns:
+        float: A number between 0 and 1.
     """
     try:
         color = float(value)
     except ValueError:
         raise PydanticCustomError('color_error', 'value is not a valid color: color values must be a valid number')
     if 0 <= color <= max_val:
         return color / max_val
@@ -299,15 +371,24 @@
             'value is not a valid color: color values must be in the range 0 to {max_val}',
             {'max_val': max_val},
         )
 
 
 def parse_float_alpha(value: Union[None, str, float, int]) -> Optional[float]:
     """
-    Parse a value checking it's a valid float in the range 0 to 1
+    Parse an alpha value checking it's a valid float in the range 0 to 1.
+
+    Args:
+        value (Union[None, str, float, int]): The input value to parse.
+
+    Returns:
+        Optional[float]: The parsed value as a float, or `None` if the value was None or equal 1.
+
+    Raises:
+        PydanticCustomError: If the input value cannot be successfully parsed as a float in the expected range.
     """
     if value is None:
         return None
     try:
         if isinstance(value, str) and value.endswith('%'):
             alpha = float(value[:-1]) / 100
         else:
@@ -321,15 +402,25 @@
         return alpha
     else:
         raise PydanticCustomError('color_error', 'value is not a valid color: alpha values must be in the range 0 to 1')
 
 
 def parse_hsl(h: str, h_units: str, sat: str, light: str, alpha: Optional[float] = None) -> RGBA:
     """
-    Parse raw hue, saturation, lightness and alpha values and convert to RGBA.
+    Parse raw hue, saturation, lightness, and alpha values and convert to RGBA.
+
+    Args:
+        h (str): The hue value.
+        h_units (str): The unit for hue value.
+        sat (str): The saturation value.
+        light (str): The lightness value.
+        alpha (Optional[float]): Alpha value.
+
+    Returns:
+        RGBA: An instance of `RGBA`.
     """
     s_value, l_value = parse_color_value(sat, 100), parse_color_value(light, 100)
 
     h_value = float(h)
     if h_units in {None, 'deg'}:
         h_value = h_value % 360 / 360
     elif h_units == 'rad':
@@ -339,14 +430,26 @@
         h_value = h_value % 1
 
     r, g, b = hls_to_rgb(h_value, l_value, s_value)
     return RGBA(r, g, b, parse_float_alpha(alpha))
 
 
 def float_to_255(c: float) -> int:
+    """
+    Converts a float value between 0 and 1 (inclusive) to an integer between 0 and 255 (inclusive).
+
+    Args:
+        c (float): The float value to be converted. Must be between 0 and 1 (inclusive).
+
+    Returns:
+        int: The integer equivalent of the given float value rounded to the nearest whole number.
+
+    Raises:
+        ValueError: If the given float value is outside the acceptable range of 0 to 1 (inclusive).
+    """
     return int(round(c * 255))
 
 
 COLORS_BY_NAME = {
     'aliceblue': (240, 248, 255),
     'antiquewhite': (250, 235, 215),
     'aqua': (0, 255, 255),
```

### Comparing `pydantic-2.0a1/pydantic/config.py` & `pydantic-2.0a2/pydantic/_internal/_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,46 @@
 from __future__ import annotations as _annotations
 
 import warnings
-from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable
+from typing import TYPE_CHECKING, Any, Callable, cast
 
-from typing_extensions import Literal, Protocol, TypedDict
+from pydantic_core import core_schema
+from typing_extensions import Literal, Self
 
 from pydantic.errors import PydanticUserError
 
-if TYPE_CHECKING:
-    from typing import overload
+from ..config import ConfigDict, ExtraValues
 
-    from .main import BaseModel
+DEPRECATION_MESSAGE = 'Support for class-based `config` is deprecated, use ConfigDict instead.'
 
-    class SchemaExtraCallable(Protocol):
-        # TODO: This has been replaced with __pydantic_modify_json_schema__ in v2; need to make sure we
-        #   document the migration, in particular changing `model_class` to `cls` from the classmethod
-        # TODO: Note that the argument to Field(...) that served a similar purpose received the FieldInfo as well.
-        #   Should we accept that argument here too? Will that add a ton of boilerplate?
-        # Tentative suggestion to previous TODO: I think we let the json_schema_extra argument
-        #   to FieldInfo be a callable that accepts schema, model_class, and field_info. And use
-        #   similar machinery to `_apply_modify_schema` to call the function properly for different signatures.
-        #   (And use this Protocol-based approach to get good type-checking.)
-        @overload
-        def __call__(self, schema: dict[str, Any]) -> None:
-            pass
-
-        @overload
-        def __call__(self, schema: dict[str, Any], model_class: type[BaseModel]) -> None:
-            pass
-
-else:
-    SchemaExtraCallable = Callable[..., None]
-
-__all__ = 'BaseConfig', 'ConfigDict', 'Extra', 'build_config', 'prepare_config'
 
+class ConfigWrapper:
+    """
+    Internal wrapper for Config which exposes ConfigDict items as attributes.
+    """
 
-class Extra(str, Enum):
-    allow = 'allow'
-    ignore = 'ignore'
-    forbid = 'forbid'
+    __slots__ = ('config_dict',)
 
+    config_dict: ConfigDict
 
-class _ConfigDict(TypedDict, total=False):
+    # all annotations are copied directly from ConfigDict, and should be kept up to date, a test will fail if they
+    # stop matching
     title: str | None
     str_to_lower: bool
     str_to_upper: bool
     str_strip_whitespace: bool
     str_min_length: int
     str_max_length: int | None
-    extra: Extra | None
+    extra: ExtraValues | None
     frozen: bool
     populate_by_name: bool
     use_enum_values: bool
     validate_assignment: bool
-    arbitrary_types_allowed: bool  # TODO default True, or remove
-    undefined_types_warning: bool  # TODO review docs
+    arbitrary_types_allowed: bool
+    undefined_types_warning: bool
     from_attributes: bool
     # whether to use the used alias (or first alias for "field required" errors) instead of field_names
     # to construct error `loc`s, default True
     loc_by_alias: bool
     alias_generator: Callable[[str], str] | None
     ignored_types: tuple[type, ...]
     allow_inf_nan: bool
@@ -69,197 +50,181 @@
     # whether instances of models and dataclasses (including subclass instances) should re-validate, default 'never'
     revalidate_instances: Literal['always', 'never', 'subclass-instances']
     ser_json_timedelta: Literal['iso8601', 'float']
     ser_json_bytes: Literal['utf8', 'base64']
     # whether to validate default values during validation, default False
     validate_default: bool
 
+    def __init__(self, config: ConfigDict | dict[str, Any] | type[Any] | None, *, check: bool = True):
+        if check:
+            self.config_dict = prepare_config(config)
+        else:
+            self.config_dict = cast(ConfigDict, config)
+
+    @classmethod
+    def for_model(cls, bases: tuple[type[Any], ...], namespace: dict[str, Any], kwargs: dict[str, Any]) -> Self:
+        """
+        Build a new `ConfigDict` instance for a `BaseModel` based on (from lowest to highest)
+        - options defined in base
+        - options defined in namespace
+        - options defined via kwargs
+
+        :param bases: tuple of base classes
+        :param namespace: namespace of the class being created
+        :param kwargs: kwargs passed to the class being created
+        """
+
+        config_new = ConfigDict()
+        for base in bases:
+            config = getattr(base, 'model_config', None)
+            if config:
+                config_new.update(config.copy())
+
+        config_class_from_namespace = namespace.get('Config')
+        config_dict_from_namespace = namespace.get('model_config')
+
+        if config_class_from_namespace and config_dict_from_namespace:
+            raise PydanticUserError('"Config" and "model_config" cannot be used together', code='config-both')
+
+        config_from_namespace = config_dict_from_namespace or prepare_config(config_class_from_namespace)
+
+        if config_from_namespace is not None:
+            config_new.update(config_from_namespace)
+
+        for k in list(kwargs.keys()):
+            if k in config_keys:
+                config_new[k] = kwargs.pop(k)
 
-config_keys = set(_ConfigDict.__annotations__.keys())
-
-if TYPE_CHECKING:
+        return cls(config_new)
 
-    class ConfigDict(_ConfigDict):
-        ...
+    # we don't show `__getattr__` to type checkers so missing attributes cause errors
+    if not TYPE_CHECKING:
 
-else:
+        def __getattr__(self, name: str) -> Any:
+            try:
+                return self.config_dict[name]
+            except KeyError:
+                try:
+                    return config_defaults[name]
+                except KeyError:
+                    raise AttributeError(f'Config has no attribute {name!r}') from None
+
+    def core_config(self, obj: Any = None) -> core_schema.CoreConfig:
+        """
+        Create a pydantic-core config, `obj` is just used to populate `title` if not set in config.
+
+        We don't use getattr here since we don't want to populate with defaults.
+        """
+        extra = self.config_dict.get('extra')
+        core_config = core_schema.CoreConfig(
+            **core_schema.dict_not_none(
+                title=self.config_dict.get('title') or (obj and obj.__name__),
+                extra_fields_behavior=extra,
+                allow_inf_nan=self.config_dict.get('allow_inf_nan'),
+                populate_by_name=self.config_dict.get('populate_by_name'),
+                str_strip_whitespace=self.config_dict.get('str_strip_whitespace'),
+                str_to_lower=self.config_dict.get('str_to_lower'),
+                str_to_upper=self.config_dict.get('str_to_upper'),
+                strict=self.config_dict.get('strict'),
+                ser_json_timedelta=self.config_dict.get('ser_json_timedelta'),
+                ser_json_bytes=self.config_dict.get('ser_json_bytes'),
+                from_attributes=self.config_dict.get('from_attributes'),
+                loc_by_alias=self.config_dict.get('loc_by_alias'),
+                revalidate_instances=self.config_dict.get('revalidate_instances'),
+                validate_default=self.config_dict.get('validate_default'),
+                str_max_length=self.config_dict.get('str_max_length'),
+                str_min_length=self.config_dict.get('str_min_length'),
+            )
+        )
+        return core_config
 
-    class ConfigDict(dict):
-        _V2_REMOVED_KEYS = {
-            'allow_mutation',
-            'error_msg_templates',
-            'fields',
-            'getter_dict',
-            'schema_extra',
-            'smart_union',
-            'underscore_attrs_are_private',
-            'json_loads',
-            'json_dumps',
-            'json_encoders',
-            'copy_on_model_validation',
-            'post_init_call',
-        }
-        _V2_RENAMED_KEYS = {
-            'allow_population_by_field_name': 'populate_by_name',
-            'anystr_lower': 'str_to_lower',
-            'anystr_strip_whitespace': 'str_strip_whitespace',
-            'anystr_upper': 'str_to_upper',
-            'keep_untouched': 'ignored_types',
-            'max_anystr_length': 'str_max_length',
-            'min_anystr_length': 'str_min_length',
-            'orm_mode': 'from_attributes',
-            'validate_all': 'validate_default',
-        }
-
-        def __init__(self, *args, **kwargs):
-            super().__init__(*args, **kwargs)
-
-            deprecated_removed_keys = ConfigDict._V2_REMOVED_KEYS & self.keys()
-            deprecated_renamed_keys = ConfigDict._V2_RENAMED_KEYS.keys() & self.keys()
-            if deprecated_removed_keys or deprecated_renamed_keys:
-                renamings = {k: self._V2_RENAMED_KEYS[k] for k in sorted(deprecated_renamed_keys)}
-                renamed_bullets = [f'* {k!r} has been renamed to {v!r}' for k, v in renamings.items()]
-                removed_bullets = [f'* {k!r} has been removed' for k in sorted(deprecated_removed_keys)]
-                message = '\n'.join(['Valid config keys have changed in V2:'] + renamed_bullets + removed_bullets)
-                warnings.warn(message, UserWarning)
-
-        def __missing__(self, key: str) -> Any:
-            if key in _default_config:  # need this check to prevent a recursion error
-                return _default_config[key]
-            raise KeyError(key)
+    def __repr__(self):
+        c = ', '.join(f'{k}={v!r}' for k, v in self.config_dict.items())
+        return f'ConfigWrapper({c})'
 
 
-_default_config = ConfigDict(
+config_defaults = ConfigDict(
     title=None,
     str_to_lower=False,
     str_to_upper=False,
     str_strip_whitespace=False,
     str_min_length=0,
     str_max_length=None,
     # let the model / dataclass decide how to handle it
     extra=None,
     frozen=False,
-    revalidate_instances='never',
     populate_by_name=False,
     use_enum_values=False,
     validate_assignment=False,
     arbitrary_types_allowed=False,
     undefined_types_warning=True,
     from_attributes=False,
     loc_by_alias=True,
     alias_generator=None,
     ignored_types=(),
     allow_inf_nan=True,
     strict=False,
+    revalidate_instances='never',
     ser_json_timedelta='iso8601',
     ser_json_bytes='utf8',
     validate_default=False,
 )
 
 
-class ConfigMetaclass(type):
-    def __getattr__(self, item: str) -> Any:
-        warnings.warn(
-            f'Support for "config" as "{self.__name__}" is deprecated and will be removed in a future version"',
-            DeprecationWarning,
-        )
-
-        try:
-            return _default_config[item]  # type: ignore[literal-required]
-        except KeyError as exc:
-            raise AttributeError(f"type object '{self.__name__}' has no attribute {exc}") from exc
-
-
-class BaseConfig(metaclass=ConfigMetaclass):
+def prepare_config(config: ConfigDict | dict[str, Any] | type[Any] | None) -> ConfigDict:
     """
-    This class is only retained for backwards compatibility.
-
-    The preferred approach going forward is to assign a ConfigDict to the `model_config` attribute of the Model class.
+    Create a `ConfigDict` instance from an existing dict, a class (e.g. old class-based config) or None.
     """
-
-    def __getattr__(self, item: str) -> Any:
-        warnings.warn(
-            f'Support for "config" as "{type(self).__name__}" is deprecated and will be removed in a future version',
-            DeprecationWarning,
-        )
-        try:
-            return super().__getattribute__(item)
-        except AttributeError as exc:
-            try:
-                return getattr(type(self), item)
-            except AttributeError:
-                # reraising changes the displayed text to reflect that `self` is not a type
-                raise AttributeError(str(exc)) from exc
-
-    def __init_subclass__(cls, **kwargs: Any) -> None:
-        warnings.warn(
-            '`BaseConfig` is deprecated and will be removed in a future version',
-            DeprecationWarning,
-        )
-        return super().__init_subclass__(**kwargs)
-
-
-def get_config(config: ConfigDict | dict[str, Any] | type[Any] | None, error_label: str | None = None) -> ConfigDict:
     if config is None:
         return ConfigDict()
 
-    if isinstance(config, dict):
-        config_dict = config
-    else:
-        warnings.warn(
-            f'Support for "config" as "{type(config).__name__}" is deprecated and will be removed in a future version',
-            DeprecationWarning,
-        )
-        config_dict = {k: getattr(config, k) for k in dir(config) if not k.startswith('__')}
-
-    prepare_config(config_dict, error_label or 'ConfigDict')
-    return ConfigDict(config_dict)  # type: ignore
+    if not isinstance(config, dict):
+        warnings.warn(DEPRECATION_MESSAGE, DeprecationWarning)
+        config = {k: getattr(config, k) for k in dir(config) if not k.startswith('__')}
+
+    config_dict = cast(ConfigDict, config)
+    check_deprecated(config_dict)
+    return config_dict
+
+
+config_keys = set(ConfigDict.__annotations__.keys())
+
+
+V2_REMOVED_KEYS = {
+    'allow_mutation',
+    'error_msg_templates',
+    'fields',
+    'getter_dict',
+    'schema_extra',
+    'smart_union',
+    'underscore_attrs_are_private',
+    'json_loads',
+    'json_dumps',
+    'json_encoders',
+    'copy_on_model_validation',
+    'post_init_call',
+}
+V2_RENAMED_KEYS = {
+    'allow_population_by_field_name': 'populate_by_name',
+    'anystr_lower': 'str_to_lower',
+    'anystr_strip_whitespace': 'str_strip_whitespace',
+    'anystr_upper': 'str_to_upper',
+    'keep_untouched': 'ignored_types',
+    'max_anystr_length': 'str_max_length',
+    'min_anystr_length': 'str_min_length',
+    'orm_mode': 'from_attributes',
+    'validate_all': 'validate_default',
+}
 
 
-def build_config(
-    cls_name: str, bases: tuple[type[Any], ...], namespace: dict[str, Any], kwargs: dict[str, Any]
-) -> ConfigDict:
+def check_deprecated(config_dict: ConfigDict) -> None:
     """
-    Build a new ConfigDict instance based on (from lowest to highest)
-    - options defined in base
-    - options defined in namespace
-    - options defined via kwargs
+    Check for depreciated config keys and warn the user.
     """
-    config_kwargs = {k: kwargs.pop(k) for k in list(kwargs.keys()) if k in config_keys}
-
-    config_bases = {}
-    configs_ordered = []
-    # collect all config options from bases
-    for base in bases:
-        config = getattr(base, 'model_config', None)
-        if config:
-            configs_ordered.append(config)
-            config_bases.update({key: value for key, value in config.items()})
-    config_new = dict(config_bases.items())
-
-    config_class_from_namespace = namespace.get('Config')
-    config_dict_from_namespace = namespace.get('model_config')
-
-    if config_class_from_namespace and config_dict_from_namespace:
-        raise PydanticUserError('"Config" and "model_config" cannot be used together')
-
-    config_from_namespace = config_dict_from_namespace or get_config(config_class_from_namespace)
-
-    if config_from_namespace:
-        configs_ordered.append(config_from_namespace)
-        config_new.update(config_from_namespace)
-    configs_ordered.append(config_kwargs)
-
-    config_new.update(config_kwargs)
-    new_model_config = ConfigDict(config_new)  # type: ignore
-
-    prepare_config(new_model_config, cls_name)
-    return new_model_config
-
-
-def prepare_config(config: ConfigDict | dict[str, Any], error_label: str) -> None:
-    extra = config.get('extra')
-    if extra is not None and not isinstance(extra, Extra):
-        try:
-            config['extra'] = Extra(extra)
-        except ValueError as e:
-            raise ValueError(f'{error_label!r}: {extra!r} is not a valid value for config[{"extra"!r}]') from e
+    deprecated_removed_keys = V2_REMOVED_KEYS & config_dict.keys()
+    deprecated_renamed_keys = V2_RENAMED_KEYS.keys() & config_dict.keys()
+    if deprecated_removed_keys or deprecated_renamed_keys:
+        renamings = {k: V2_RENAMED_KEYS[k] for k in sorted(deprecated_renamed_keys)}
+        renamed_bullets = [f'* {k!r} has been renamed to {v!r}' for k, v in renamings.items()]
+        removed_bullets = [f'* {k!r} has been removed' for k in sorted(deprecated_removed_keys)]
+        message = '\n'.join(['Valid config keys have changed in V2:'] + renamed_bullets + removed_bullets)
+        warnings.warn(message, UserWarning)
```

### Comparing `pydantic-2.0a1/pydantic/dataclasses.py` & `pydantic-2.0a2/pydantic/dataclasses.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 import dataclasses
 import sys
 from typing import TYPE_CHECKING, Any, Callable, TypeVar, overload
 
 from typing_extensions import Literal, dataclass_transform
 
+from ._internal import _config, _decorators
 from ._internal import _dataclasses as _pydantic_dataclasses
-from ._internal import _decorators
-from .config import ConfigDict, get_config
+from .config import ConfigDict
 from .fields import Field, FieldInfo
 
 if TYPE_CHECKING:
     from ._internal._dataclasses import PydanticDataclass
 
 
 __all__ = ('dataclass',)
@@ -33,21 +33,21 @@
         eq: bool = True,
         order: bool = False,
         unsafe_hash: bool = False,
         frozen: bool = False,
         config: ConfigDict | type[object] | None = None,
         validate_on_init: bool | None = None,
         kw_only: bool = ...,
-    ) -> Callable[[type[_T]], type[PydanticDataclass]]:
+    ) -> Callable[[type[_T]], type[PydanticDataclass]]:  # type: ignore
         ...
 
     @dataclass_transform(field_specifiers=(dataclasses.field, Field))
     @overload
     def dataclass(
-        _cls: type[_T],
+        _cls: type[_T],  # type: ignore
         *,
         init: Literal[False] = False,
         repr: bool = True,
         eq: bool = True,
         order: bool = False,
         unsafe_hash: bool = False,
         frozen: bool = False,
@@ -67,21 +67,21 @@
         repr: bool = True,
         eq: bool = True,
         order: bool = False,
         unsafe_hash: bool = False,
         frozen: bool = False,
         config: ConfigDict | type[object] | None = None,
         validate_on_init: bool | None = None,
-    ) -> Callable[[type[_T]], type[PydanticDataclass]]:
+    ) -> Callable[[type[_T]], type[PydanticDataclass]]:  # type: ignore
         ...
 
     @dataclass_transform(field_specifiers=(dataclasses.field, Field))
     @overload
     def dataclass(
-        _cls: type[_T],
+        _cls: type[_T],  # type: ignore
         *,
         init: Literal[False] = False,
         repr: bool = True,
         eq: bool = True,
         order: bool = False,
         unsafe_hash: bool = False,
         frozen: bool = False,
@@ -142,16 +142,17 @@
                     '__pydantic_omitted_fields__': omitted_fields or None,
                     '__pydantic_decorators__': decorators,
                 },
             )
         else:
             setattr(cls, '__pydantic_decorators__', decorators)
 
-        config_dict = get_config(config, cls.__name__)
-        _pydantic_dataclasses.prepare_dataclass(cls, config_dict, kw_only)
+        config_wrapper = _config.ConfigWrapper(config)
+        # TODO set title
+        _pydantic_dataclasses.prepare_dataclass(cls, config_wrapper, kw_only)
 
         if sys.version_info >= (3, 10):
             kwargs = dict(kw_only=kw_only)
         else:
             kwargs = {}
 
         cls = dataclasses.dataclass(  # type: ignore[call-overload]
```

### Comparing `pydantic-2.0a1/pydantic/decorator.py` & `pydantic-2.0a2/pydantic/decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 TODO this should be removed when we implement `validate` #4669
 """
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Mapping, Optional, Tuple, Type, TypeVar, Union, overload
 
-from ._internal import _typing_extra, _utils
-from .config import Extra, get_config
+from ._internal import _config, _typing_extra, _utils
 from .decorators import field_validator
 from .errors import PydanticUserError
 from .main import BaseModel, create_model
 
 __all__ = ('validate_arguments',)
 
 if TYPE_CHECKING:
@@ -56,28 +55,29 @@
 ALT_V_ARGS = 'v__args'
 ALT_V_KWARGS = 'v__kwargs'
 V_POSITIONAL_ONLY_NAME = 'v__positional_only'
 V_DUPLICATE_KWARGS = 'v__duplicate_kwargs'
 
 
 class ValidatedFunction:
-    def __init__(self, function: 'AnyCallableT', config: 'ConfigType'):
+    def __init__(self, function: 'AnyCallable', config: 'ConfigType'):
         from inspect import Parameter, signature
 
         parameters: Mapping[str, Parameter] = signature(function).parameters
 
         if parameters.keys() & {ALT_V_ARGS, ALT_V_KWARGS, V_POSITIONAL_ONLY_NAME, V_DUPLICATE_KWARGS}:
             raise PydanticUserError(
                 f'"{ALT_V_ARGS}", "{ALT_V_KWARGS}", "{V_POSITIONAL_ONLY_NAME}" and "{V_DUPLICATE_KWARGS}" '
-                f'are not permitted as argument names when using the "{validate_arguments.__name__}" decorator'
+                f'are not permitted as argument names when using the "{validate_arguments.__name__}" decorator',
+                code=None,
             )
 
         self.raw_function = function
         self.arg_mapping: Dict[int, str] = {}
-        self.positional_only_args = set()
+        self.positional_only_args: set[str] = set()
         self.v_args_name = 'args'
         self.v_kwargs_name = 'kwargs'
 
         type_hints = _typing_extra.get_type_hints(function, include_extras=True)
         takes_args = False
         takes_kwargs = False
         fields: Dict[str, Tuple[Any, Any]] = {}
@@ -175,15 +175,15 @@
         if wrong_positional_args:
             values[V_POSITIONAL_ONLY_NAME] = wrong_positional_args
         if duplicate_kwargs:
             values[V_DUPLICATE_KWARGS] = duplicate_kwargs
         return values
 
     def execute(self, m: BaseModel) -> Any:
-        d = {k: v for k, v in m.__dict__.items() if k in m.__fields_set__ or m.model_fields[k].default_factory}
+        d = {k: v for k, v in m.__dict__.items() if k in m.__pydantic_fields_set__ or m.model_fields[k].default_factory}
         var_kwargs = d.pop(self.v_kwargs_name, {})
 
         if self.v_args_name in d:
             args_: List[Any] = []
             in_kwargs = False
             kwargs = {}
             for name, value in d.items():
@@ -206,59 +206,60 @@
             return self.raw_function(*args_, **kwargs, **var_kwargs)
         else:
             return self.raw_function(**d, **var_kwargs)
 
     def create_model(self, fields: Dict[str, Any], takes_args: bool, takes_kwargs: bool, config: 'ConfigType') -> None:
         pos_args = len(self.arg_mapping)
 
-        config_dict = get_config(config, getattr(self.raw_function, '__name__', 'validate_arguments'))
+        config_wrapper = _config.ConfigWrapper(config)
 
-        if 'alias_generator' in config_dict:
+        if config_wrapper.alias_generator:
             raise PydanticUserError(
                 'Setting the "alias_generator" property on custom Config for '
-                '@validate_arguments is not yet supported, please remove.'
+                '@validate_arguments is not yet supported, please remove.',
+                code=None,
             )
-        if 'extra' not in config_dict:
-            config_dict['extra'] = Extra.forbid
+        if config_wrapper.extra is None:
+            config_wrapper.config_dict['extra'] = 'forbid'
 
         class DecoratorBaseModel(BaseModel):
-            @field_validator(self.v_args_name, check_fields=False, allow_reuse=True)
+            @field_validator(self.v_args_name, check_fields=False)
             @classmethod
             def check_args(cls, v: Optional[List[Any]]) -> Optional[List[Any]]:
                 if takes_args or v is None:
                     return v
 
                 raise TypeError(f'{pos_args} positional arguments expected but {pos_args + len(v)} given')
 
-            @field_validator(self.v_kwargs_name, check_fields=False, allow_reuse=True)
+            @field_validator(self.v_kwargs_name, check_fields=False)
             @classmethod
             def check_kwargs(cls, v: Optional[Dict[str, Any]]) -> Optional[Dict[str, Any]]:
                 if takes_kwargs or v is None:
                     return v
 
                 plural = '' if len(v) == 1 else 's'
                 keys = ', '.join(map(repr, v.keys()))
                 raise TypeError(f'unexpected keyword argument{plural}: {keys}')
 
-            @field_validator(V_POSITIONAL_ONLY_NAME, check_fields=False, allow_reuse=True)
+            @field_validator(V_POSITIONAL_ONLY_NAME, check_fields=False)
             @classmethod
             def check_positional_only(cls, v: Optional[List[str]]) -> None:
                 if v is None:
                     return
 
                 plural = '' if len(v) == 1 else 's'
                 keys = ', '.join(map(repr, v))
                 raise TypeError(f'positional-only argument{plural} passed as keyword argument{plural}: {keys}')
 
-            @field_validator(V_DUPLICATE_KWARGS, check_fields=False, allow_reuse=True)
+            @field_validator(V_DUPLICATE_KWARGS, check_fields=False)
             @classmethod
             def check_duplicate_kwargs(cls, v: Optional[List[str]]) -> None:
                 if v is None:
                     return
 
                 plural = '' if len(v) == 1 else 's'
                 keys = ', '.join(map(repr, v))
                 raise TypeError(f'multiple values for argument{plural}: {keys}')
 
-            model_config = config_dict
+            model_config = config_wrapper.config_dict
 
         self.model = create_model(_utils.to_camel(self.raw_function.__name__), __base__=DecoratorBaseModel, **fields)
```

### Comparing `pydantic-2.0a1/pydantic/decorators.py` & `pydantic-2.0a2/pydantic/decorators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 Public methods related to:
+
 * `validator` - a decorator to add validation to a field on a model
 * `root_validator` - a decorator to add validation to a model as a whole
 * `serializer` - a decorator to add serialization to a field on a model
 """
 
 from __future__ import annotations as _annotations
 
-from functools import partial
+from functools import partial, partialmethod
 from types import FunctionType
 from typing import Any, Callable, TypeVar, Union, overload
 from warnings import warn
 
 from pydantic_core import core_schema as _core_schema
-from typing_extensions import Literal, Protocol
+from typing_extensions import Literal, Protocol, TypeAlias
 
 from ._internal import _decorators
+from .errors import PydanticUserError
+
+_ALLOW_REUSE_WARNING_MESSAGE = '`allow_reuse` is deprecated and will be ignored; it should no longer be necessary'
 
 
 class _OnlyValueValidatorClsMethod(Protocol):
     def __call__(self, __cls: Any, __value: Any) -> Any:
         ...
 
 
@@ -90,84 +94,94 @@
 ]
 
 V1RootValidator = Union[
     _V1RootValidatorClsMethod,
     _decorators.V1RootValidatorFunction,
 ]
 
+_PartialClsOrStaticMethod: TypeAlias = 'Union[classmethod[Any, Any, Any], staticmethod[Any, Any], partialmethod[Any]]'
+
 
 # Allow both a V1 (assumed pre=False) or V2 (assumed mode='after') validator
 # We lie to type checkers and say we return the same thing we get
 # but in reality we return a proxy object that _mostly_ behaves like the wrapped thing
-_V1ValidatorType = TypeVar('_V1ValidatorType', bound=Union[V1Validator, 'classmethod[Any]', 'staticmethod[Any]'])
+_V1ValidatorType = TypeVar('_V1ValidatorType', bound=Union[V1Validator, _PartialClsOrStaticMethod])
 _V2BeforeAfterOrPlainValidatorType = TypeVar(
     '_V2BeforeAfterOrPlainValidatorType',
-    bound=Union[V2Validator, 'classmethod[Any]', 'staticmethod[Any]'],
-)
-_V2WrapValidatorType = TypeVar(
-    '_V2WrapValidatorType', bound=Union[V2WrapValidator, 'classmethod[Any]', 'staticmethod[Any]']
+    bound=Union[V2Validator, _PartialClsOrStaticMethod],
 )
+_V2WrapValidatorType = TypeVar('_V2WrapValidatorType', bound=Union[V2WrapValidator, _PartialClsOrStaticMethod])
 _V1RootValidatorFunctionType = TypeVar(
     '_V1RootValidatorFunctionType',
-    bound=Union[
-        _decorators.V1RootValidatorFunction,
-        _V1RootValidatorClsMethod,
-        'classmethod[Any]',
-        'staticmethod[Any]',
-    ],
+    bound=Union[_decorators.V1RootValidatorFunction, _V1RootValidatorClsMethod, _PartialClsOrStaticMethod],
 )
 
 
 def validator(
     __field: str,
     *fields: str,
     pre: bool = False,
     each_item: bool = False,
     always: bool = False,
     check_fields: bool | None = None,
     allow_reuse: bool = False,
 ) -> Callable[[_V1ValidatorType], _V1ValidatorType]:
     """
-    Decorate methods on the class indicating that they should be used to validate fields
-    :param __field: the first field the validator should be called on;
-        this is separate from `fields` to ensure an error is raised if you don't pass at least one
-    :param fields: additional field(s) the validator should be called on
-    :param pre: whether or not this validator should be called before the standard validators (else after)
-    :param each_item: for complex objects (sets, lists etc.) whether to validate individual elements rather than the
-      whole object
-    :param always: whether this method and other validators should be called even if the value is missing
-    :param check_fields: whether to check that the fields actually exist on the model
-    :param allow_reuse: whether to track and raise an error if another validator refers to the decorated function
+    Decorate methods on the class indicating that they should be used to validate fields.
+
+    Args:
+        __field (str): The first field the validator should be called on; this is separate
+            from `fields` to ensure an error is raised if you don't pass at least one.
+        *fields (str): Additional field(s) the validator should be called on.
+        pre (bool, optional): Whether or not this validator should be called before the standard
+            validators (else after). Defaults to False.
+        each_item (bool, optional): For complex objects (sets, lists etc.) whether to validate
+            individual elements rather than the whole object. Defaults to False.
+        always (bool, optional): Whether this method and other validators should be called even if
+            the value is missing. Defaults to False.
+        check_fields (bool | None, optional): Whether to check that the fields actually exist on the model.
+            Defaults to None.
+        allow_reuse (bool, optional): Whether to track and raise an error if another validator refers to
+            the decorated function. Defaults to False.
+
+    Returns:
+        Callable[[_V1ValidatorType], _V1ValidatorType]: A decorator that can be used to decorate a
+            function to be used as a validator.
     """
+    if allow_reuse is True:  # pragma: no cover
+        warn(_ALLOW_REUSE_WARNING_MESSAGE, DeprecationWarning)
     fields = tuple((__field, *fields))
     if isinstance(fields[0], FunctionType):
-        raise TypeError(
-            'field_validators should be used with fields and keyword arguments, not bare. '
-            "E.g. usage should be `@validator('<field_name>', ...)`"
+        raise PydanticUserError(
+            "validators should be used with fields and keyword arguments, not bare. "
+            "E.g. usage should be `@validator('<field_name>', ...)`",
+            code='validator-no-fields',
         )
     elif not all(isinstance(field, str) for field in fields):
-        raise TypeError(
-            'validator fields should be passed as separate string args. '
-            "E.g. usage should be `@validator('<field_name_1>', '<field_name_2>', ...)`"
+        raise PydanticUserError(
+            "validator fields should be passed as separate string args. "
+            "E.g. usage should be `@validator('<field_name_1>', '<field_name_2>', ...)`",
+            code='validator-invalid-fields',
         )
 
     warn(
         'Pydantic V1 style `@validator` validators are deprecated.'
         ' You should migrate to Pydantic V2 style `@field_validator` validators,'
         ' see the migration guide for more details',
         DeprecationWarning,
         stacklevel=2,
     )
 
     mode: Literal['before', 'after'] = 'before' if pre is True else 'after'
 
     def dec(f: Any) -> _decorators.PydanticDecoratorMarker[Any]:
         if _decorators.is_instance_method_from_sig(f):
-            raise TypeError('`@validator` cannot be applied to instance methods')
-        _decorators.check_for_duplicate_validator(f, allow_reuse=allow_reuse)
+            raise PydanticUserError(
+                '`@validator` cannot be applied to instance methods', code='validator-instance-method'
+            )
         # auto apply the @classmethod decorator
         f = _decorators.ensure_classmethod_based_on_signature(f)
         wrap = _decorators.make_generic_v1_field_validator
         validator_wrapper_info = _decorators.ValidatorDecoratorInfo(
             fields=fields,
             mode=mode,
             each_item=each_item,
@@ -181,73 +195,76 @@
 
 @overload
 def field_validator(
     __field: str,
     *fields: str,
     mode: Literal['before', 'after', 'plain'] = ...,
     check_fields: bool | None = ...,
-    sub_path: tuple[str | int, ...] | None = ...,
-    allow_reuse: bool = False,
 ) -> Callable[[_V2BeforeAfterOrPlainValidatorType], _V2BeforeAfterOrPlainValidatorType]:
     ...
 
 
 @overload
 def field_validator(
     __field: str,
     *fields: str,
     mode: Literal['wrap'],
     check_fields: bool | None = ...,
-    sub_path: tuple[str | int, ...] | None = ...,
-    allow_reuse: bool = False,
 ) -> Callable[[_V2WrapValidatorType], _V2WrapValidatorType]:
     ...
 
 
 def field_validator(
     __field: str,
     *fields: str,
     mode: Literal['before', 'after', 'wrap', 'plain'] = 'after',
     check_fields: bool | None = None,
-    sub_path: tuple[str | int, ...] | None = None,
-    allow_reuse: bool = False,
 ) -> Callable[[Any], Any]:
     """
-    Decorate methods on the class indicating that they should be used to validate fields
-    :param __field: the first field the field_validator should be called on;
-        this is separate from `fields` to ensure an error is raised if you don't pass at least one
-    :param fields: additional field(s) the field_validator should be called on
-    :param mode: TODO
-    :param check_fields: whether to check that the fields actually exist on the model
-    :param sub_path: TODO
-    :param allow_reuse: whether to track and raise an error if another validator refers to the decorated function
+    Decorate methods on the class indicating that they should be used to validate fields.
+
+    Args:
+        __field (str): The first field the field_validator should be called on; this is separate
+            from `fields` to ensure an error is raised if you don't pass at least one.
+        *fields (str): Additional field(s) the field_validator should be called on.
+        mode (Literal['before', 'after', 'wrap', 'plain'], optional): TODO. Defaults to 'after'.
+        check_fields (bool | None, optional): Whether to check that the fields actually exist on
+            the model. Defaults to None.
+
+    Returns:
+        Callable[[Any], Any]: A decorator that can be used to decorate a function to be used as a field_validator.
     """
     fields = tuple((__field, *fields))
     if isinstance(fields[0], FunctionType):
-        raise TypeError(
+        raise PydanticUserError(
             'field_validators should be used with fields and keyword arguments, not bare. '
-            "E.g. usage should be `@validator('<field_name>', ...)`"
+            "E.g. usage should be `@validator('<field_name>', ...)`",
+            code='validator-no-fields',
         )
     elif not all(isinstance(field, str) for field in fields):
-        raise TypeError(
+        raise PydanticUserError(
             'field_validator fields should be passed as separate string args. '
-            "E.g. usage should be `@validator('<field_name_1>', '<field_name_2>', ...)`"
+            "E.g. usage should be `@validator('<field_name_1>', '<field_name_2>', ...)`",
+            code='validator-invalid-fields',
         )
 
-    def dec(f: Callable[..., Any] | staticmethod[Any] | classmethod[Any]) -> _decorators.PydanticDecoratorMarker[Any]:
+    def dec(
+        f: Callable[..., Any] | staticmethod[Any, Any] | classmethod[Any, Any, Any]
+    ) -> _decorators.PydanticDecoratorMarker[Any]:
         if _decorators.is_instance_method_from_sig(f):
-            raise TypeError('`@field_validator` cannot be applied to instance methods')
-        _decorators.check_for_duplicate_validator(f, allow_reuse=allow_reuse)
+            raise PydanticUserError(
+                '`@field_validator` cannot be applied to instance methods', code='validator-instance-method'
+            )
         # auto apply the @classmethod decorator and warn users if we had to do so
         f = _decorators.ensure_classmethod_based_on_signature(f)
 
-        wrap = partial(_decorators.make_generic_v2_field_validator, mode=mode)
+        wrap = partial(_decorators.make_generic_validator, mode=mode)
 
         validator_wrapper_info = _decorators.FieldValidatorDecoratorInfo(
-            fields=fields, mode=mode, sub_path=sub_path, check_fields=check_fields
+            fields=fields, mode=mode, check_fields=check_fields
         )
         return _decorators.PydanticDecoratorMarker(f, validator_wrapper_info, shim=wrap)
 
     return dec
 
 
 @overload
@@ -285,182 +302,319 @@
 
 
 def root_validator(
     *,
     pre: bool = False,
     skip_on_failure: bool = False,
     allow_reuse: bool = False,
-) -> Callable[[Any], _decorators.PydanticDecoratorMarker[Any]]:
+) -> Any:
     """
-    Decorate methods on a model indicating that they should be used to validate (and perhaps modify) data either
-    before or after standard model parsing/validation is performed.
+    Decorate methods on a model indicating that they should be used to validate (and perhaps
+    modify) data either before or after standard model parsing/validation is performed.
+
+    Args:
+        pre (bool, optional): Whether or not this validator should be called before the standard
+            validators (else after). Defaults to False.
+        skip_on_failure (bool, optional): Whether to stop validation and return as soon as a
+            failure is encountered. Defaults to False.
+        allow_reuse (bool, optional): Whether to track and raise an error if another validator
+            refers to the decorated function. Defaults to False.
+
+    Returns:
+        Any: A decorator that can be used to decorate a function to be used as a root_validator.
     """
+    if allow_reuse is True:  # pragma: no cover
+        warn(_ALLOW_REUSE_WARNING_MESSAGE, DeprecationWarning)
     mode: Literal['before', 'after'] = 'before' if pre is True else 'after'
     if pre is False and skip_on_failure is not True:
-        raise TypeError(
-            'If you use `@root_validator` with pre=False (the default)'
-            ' you MUST specify `skip_on_failure=True`.'
-            ' The `skip_on_failure=False` option is no longer available.'
-            ' If you were not trying to set `skip_on_failure=False` you'
-            ' can safely set `skip_on_failure=True`.'
-            ' If you do, this root validator will no longer be called'
-            ' if validation fails for any of the fields.'
-            ' Please see the migration guide for more details.'
+        raise PydanticUserError(
+            'If you use `@root_validator` with pre=False (the default) you MUST specify `skip_on_failure=True`.',
+            code='root-validator-pre-skip',
         )
+
     wrap = partial(_decorators.make_v1_generic_root_validator, pre=pre)
 
-    def dec(f: Callable[..., Any] | classmethod[Any] | staticmethod[Any]) -> Any:
+    def dec(f: Callable[..., Any] | classmethod[Any, Any, Any] | staticmethod[Any, Any]) -> Any:
         if _decorators.is_instance_method_from_sig(f):
             raise TypeError('`@root_validator` cannot be applied to instance methods')
-        _decorators.check_for_duplicate_validator(f, allow_reuse=allow_reuse)
         # auto apply the @classmethod decorator and warn users if we had to do so
         res = _decorators.ensure_classmethod_based_on_signature(f)
         validator_wrapper_info = _decorators.RootValidatorDecoratorInfo(mode=mode)
         return _decorators.PydanticDecoratorMarker(res, validator_wrapper_info, shim=wrap)
 
     return dec
 
 
 _PlainSerializationFunction = Union[
     _core_schema.GeneralPlainSerializerFunction,
     _core_schema.FieldPlainSerializerFunction,
     _decorators.GenericPlainSerializerFunctionWithoutInfo,
     _decorators.FieldPlainSerializerFunctionWithoutInfo,
+    _PartialClsOrStaticMethod,
 ]
 
 
 _WrapSerializationFunction = Union[
     _core_schema.GeneralWrapSerializerFunction,
     _core_schema.FieldWrapSerializerFunction,
     _decorators.GeneralWrapSerializerFunctionWithoutInfo,
     _decorators.FieldWrapSerializerFunctionWithoutInfo,
+    _PartialClsOrStaticMethod,
 ]
 
 
 _PlainSerializeMethodType = TypeVar('_PlainSerializeMethodType', bound=_PlainSerializationFunction)
 _WrapSerializeMethodType = TypeVar('_WrapSerializeMethodType', bound=_WrapSerializationFunction)
 
 
 @overload
 def field_serializer(
     __field: str,
     *fields: str,
     json_return_type: _core_schema.JsonReturnTypes | None = ...,
     when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = ...,
-    sub_path: tuple[str | int, ...] | None = ...,
     check_fields: bool | None = ...,
-    allow_reuse: bool = ...,
 ) -> Callable[[_PlainSerializeMethodType], _PlainSerializeMethodType]:
     ...
 
 
 @overload
 def field_serializer(
     __field: str,
     *fields: str,
     mode: Literal['plain'],
     json_return_type: _core_schema.JsonReturnTypes | None = ...,
     when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = ...,
-    sub_path: tuple[str | int, ...] | None = ...,
     check_fields: bool | None = ...,
-    allow_reuse: bool = ...,
 ) -> Callable[[_PlainSerializeMethodType], _PlainSerializeMethodType]:
     ...
 
 
 @overload
 def field_serializer(
     __field: str,
     *fields: str,
     mode: Literal['wrap'],
     json_return_type: _core_schema.JsonReturnTypes | None = ...,
     when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = ...,
-    sub_path: tuple[str | int, ...] | None = ...,
     check_fields: bool | None = ...,
-    allow_reuse: bool = ...,
 ) -> Callable[[_WrapSerializeMethodType], _WrapSerializeMethodType]:
     ...
 
 
 def field_serializer(
     *fields: str,
     mode: Literal['plain', 'wrap'] = 'plain',
     json_return_type: _core_schema.JsonReturnTypes | None = None,
     when_used: Literal['always', 'unless-none', 'json', 'json-unless-none'] = 'always',
-    sub_path: tuple[str | int, ...] | None = None,
     check_fields: bool | None = None,
-    allow_reuse: bool = False,
 ) -> Callable[[Any], Any]:
     """
     Decorate methods on the class indicating that they should be used to serialize fields.
+
     Four signatures are supported:
-    - (self, value: Any, info: FieldSerializationInfo)
-    - (self, value: Any, nxt: SerializerFunctionWrapHandler, info: FieldSerializationInfo)
-    - (value: Any, info: SerializationInfo)
-    - (value: Any, nxt: SerializerFunctionWrapHandler, info: SerializationInfo)
-
-    :param fields: which field(s) the method should be called on
-    :param mode: `'plain'` means the function will be called instead of the default serialization logic,
-        `'wrap'` means the function will be called with an argument to optionally call the default serialization logic.
-    :param json_return_type: The type that the function returns if the serialization mode is JSON.
-    :param when_used: When the function should be called
-    :param sub_path: TODO
-    :param check_fields: whether to check that the fields actually exist on the model
-    :param allow_reuse: whether to track and raise an error if another validator refers to the decorated function
+
+    - `(self, value: Any, info: FieldSerializationInfo)`
+    - `(self, value: Any, nxt: SerializerFunctionWrapHandler, info: FieldSerializationInfo)`
+    - `(value: Any, info: SerializationInfo)`
+    - `(value: Any, nxt: SerializerFunctionWrapHandler, info: SerializationInfo)`
+
+    Args:
+        fields (str): Which field(s) the method should be called on.
+        mode (str):
+            - `'plain'` means the function will be called instead of the default serialization logic,
+            - `'wrap'` means the function will be called with an argument to optionally call the
+                default serialization logic.
+        json_return_type (str): The type that the function returns if the serialization mode is JSON.
+        when_used (str): When the function should be called.
+        check_fields (bool): Whether to check that the fields actually exist on the model.
     """
 
-    def dec(f: Callable[..., Any] | staticmethod[Any] | classmethod[Any]) -> _decorators.PydanticDecoratorMarker[Any]:
-        res = _decorators.prepare_serializer_decorator(f, allow_reuse)
+    def dec(
+        f: Callable[..., Any] | staticmethod[Any, Any] | classmethod[Any, Any, Any]
+    ) -> _decorators.PydanticDecoratorMarker[Any]:
         type_: Literal['field', 'general'] = 'field' if _decorators.is_instance_method_from_sig(f) else 'general'
 
         dec_info = _decorators.FieldSerializerDecoratorInfo(
             fields=fields,
             mode=mode,
             type=type_,
             json_return_type=json_return_type,
             when_used=when_used,
-            sub_path=sub_path,
             check_fields=check_fields,
         )
         return _decorators.PydanticDecoratorMarker(
-            res, dec_info, shim=partial(_decorators.make_generic_field_serializer, mode=mode, type=type_)
+            f, dec_info, shim=partial(_decorators.make_generic_serializer, mode=mode, type=type_)
         )
 
     return dec
 
 
 def model_serializer(
-    __f: Callable[..., Any] = None,
+    __f: Callable[..., Any] | None = None,
     *,
     mode: Literal['plain', 'wrap'] = 'plain',
     json_return_type: _core_schema.JsonReturnTypes | None = None,
-    allow_reuse: bool = False,
 ) -> Callable[[Any], _decorators.PydanticDecoratorMarker[Any]] | _decorators.PydanticDecoratorMarker[Any]:
     """
-    Function decorate to add a function which will be called to serialize the model.
+    Decorator to add a function which will be called to serialize the model.
 
-    (`when_used` is not permitted here since it make no sense)
+    (`when_used` is not permitted here since it makes no sense.)
 
-    :param mode: `'plain'` means the function will be called instead of the default serialization logic,
-        `'wrap'` means the function will be called with an argument to optionally call the default serialization logic.
-    :param json_return_type: The type that the function returns if the serialization mode is JSON.
-    :param allow_reuse: whether to track and raise an error if another validator refers to the decorated function
+    Args:
+        __f (Callable[..., Any] | None): The function to be decorated.
+        mode (Literal['plain', 'wrap']): The serialization mode. `'plain'` means the function will be called
+            instead of the default serialization logic, `'wrap'` means the function will be called with an argument
+            to optionally call the default serialization logic.
+        json_return_type (_core_schema.JsonReturnTypes | None): The type that the function returns if the
+            serialization mode is JSON.
+
+    Returns:
+        Callable[[Any], _decorators.PydanticDecoratorMarker[Any]] | _decorators.PydanticDecoratorMarker[Any]:
+            The decorated function.
     """
 
     def dec(f: Callable[..., Any]) -> _decorators.PydanticDecoratorMarker[Any]:
         if isinstance(f, (staticmethod, classmethod)) or not _decorators.is_instance_method_from_sig(f):
-            raise TypeError('`@model_serializer` must be applied to instance methods')
-
-        res = _decorators.prepare_serializer_decorator(f, allow_reuse)
+            raise PydanticUserError(
+                '`@model_serializer` must be applied to instance methods', code='model-serializer-instance-method'
+            )
 
         dec_info = _decorators.ModelSerializerDecoratorInfo(
             mode=mode,
             json_return_type=json_return_type,
         )
         return _decorators.PydanticDecoratorMarker(
-            res, dec_info, shim=partial(_decorators.make_generic_model_serializer, mode=mode)
+            f, dec_info, shim=partial(_decorators.make_generic_model_serializer, mode=mode)
         )
 
     if __f is None:
         return dec
     else:
         return dec(__f)
+
+
+ModelType = TypeVar('ModelType')
+ModelWrapValidatorHandler = Callable[[Any], ModelType]
+
+
+class ModelWrapValidatorWithoutInfo(Protocol):
+    def __call__(
+        self,
+        cls: type[ModelType],
+        # this can be a dict, a model instance
+        # or anything else that gets passed to validate_python
+        # thus validators _must_ handle all cases
+        __value: Any,
+        __handler: Callable[[Any], ModelType],
+    ) -> ModelType:
+        ...
+
+
+class ModelWrapValidator(Protocol):
+    def __call__(
+        self,
+        cls: type[ModelType],
+        # this can be a dict, a model instance
+        # or anything else that gets passed to validate_python
+        # thus validators _must_ handle all cases
+        __value: Any,
+        __handler: Callable[[Any], ModelType],
+        __info: _core_schema.ValidationInfo,
+    ) -> ModelType:
+        ...
+
+
+class ModelBeforeValidatorWithoutInfo(Protocol):
+    def __call__(
+        self,
+        cls: Any,
+        # this can be a dict, a model instance
+        # or anything else that gets passed to validate_python
+        # thus validators _must_ handle all cases
+        __value: Any,
+    ) -> Any:
+        ...
+
+
+class ModelBeforeValidator(Protocol):
+    def __call__(
+        self,
+        cls: Any,
+        # this can be a dict, a model instance
+        # or anything else that gets passed to validate_python
+        # thus validators _must_ handle all cases
+        __value: Any,
+        __info: _core_schema.ValidationInfo,
+    ) -> Any:
+        ...
+
+
+class ModelAfterValidatorWithoutInfo(Protocol):
+    @staticmethod
+    def __call__(
+        self: ModelType,  # type: ignore
+    ) -> ModelType:
+        ...
+
+
+class ModelAfterValidator(Protocol):
+    @staticmethod
+    def __call__(
+        self: ModelType,  # type: ignore
+        __info: _core_schema.ValidationInfo,
+    ) -> ModelType:
+        ...
+
+
+AnyModelWrapValidator = Union[
+    ModelWrapValidator,
+    ModelWrapValidatorWithoutInfo,
+]
+
+AnyModeBeforeValidator = Union[
+    ModelBeforeValidator,
+    ModelBeforeValidatorWithoutInfo,
+]
+
+AnyModeAfterValidator = Union[
+    ModelAfterValidator,
+    ModelAfterValidatorWithoutInfo,
+]
+
+
+@overload
+def model_validator(
+    *,
+    mode: Literal['wrap'],
+) -> Callable[[AnyModelWrapValidator], _decorators.PydanticDecoratorMarker[_decorators.ModelValidatorDecoratorInfo]]:
+    ...
+
+
+@overload
+def model_validator(
+    *,
+    mode: Literal['before'],
+) -> Callable[[AnyModeBeforeValidator], _decorators.PydanticDecoratorMarker[_decorators.ModelValidatorDecoratorInfo]]:
+    ...
+
+
+@overload
+def model_validator(
+    *,
+    mode: Literal['after'],
+) -> Callable[[AnyModeAfterValidator], _decorators.PydanticDecoratorMarker[_decorators.ModelValidatorDecoratorInfo]]:
+    ...
+
+
+def model_validator(
+    *,
+    mode: Literal['wrap', 'before', 'after'],
+) -> Any:
+    def dec(f: Any) -> _decorators.PydanticDecoratorMarker[Any]:
+        dec_info = _decorators.ModelValidatorDecoratorInfo(
+            mode=mode,
+        )
+        shim = partial(_decorators.make_generic_validator, mode=mode)
+        return _decorators.PydanticDecoratorMarker(f, dec_info, shim=shim)
+
+    return dec
```

### Comparing `pydantic-2.0a1/pydantic/json_schema.py` & `pydantic-2.0a2/pydantic/json_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,38 +126,41 @@
     def generate_definitions(self, schemas: list[CoreSchema]) -> dict[DefsRef, JsonSchemaValue]:
         """
         Given a list of core_schema, generate all JSON schema definitions, and return the generated definitions.
         """
         if self._used:
             raise PydanticUserError(
                 'This JSON schema generator has already been used to generate a JSON schema. '
-                f'You must create a new instance of {type(self).__name__} to generate a new JSON schema.'
+                f'You must create a new instance of {type(self).__name__} to generate a new JSON schema.',
+                code='json-schema-already-used',
             )
         for schema in schemas:
             self.generate_inner(schema)
 
         self.resolve_collisions({})
 
         self._used = True
         return self.definitions
 
     def generate(self, schema: CoreSchema) -> JsonSchemaValue:
         if self._used:
             raise PydanticUserError(
                 'This JSON schema generator has already been used to generate a JSON schema. '
-                f'You must create a new instance of {type(self).__name__} to generate a new JSON schema.'
+                f'You must create a new instance of {type(self).__name__} to generate a new JSON schema.',
+                code='json-schema-already-used',
             )
 
         json_schema = self.generate_inner(schema)
         json_ref_counts = self.get_json_ref_counts(json_schema)
 
         # Remove the top-level $ref if present; note that the _generate method already ensures there are no sibling keys
         ref = json_schema.get('$ref')
         while ref is not None:  # may need to unpack multiple levels
-            ref_json_schema = self.get_schema_from_definitions(JsonRef(ref))
+            ref = JsonRef(ref)
+            ref_json_schema = self.get_schema_from_definitions(ref)
             if json_ref_counts[ref] > 1 or ref_json_schema is None:
                 # Keep the ref, but use an allOf to remove the top level $ref
                 json_schema = {'allOf': [{'$ref': ref}]}
             else:
                 # "Unpack" the ref since this is the only reference
                 json_schema = ref_json_schema.copy()  # copy to prevent recursive dict reference
                 json_ref_counts[ref] -= 1
@@ -248,21 +251,21 @@
     def none_schema(self, schema: core_schema.NoneSchema) -> JsonSchemaValue:
         return {'type': 'null'}
 
     def bool_schema(self, schema: core_schema.BoolSchema) -> JsonSchemaValue:
         return {'type': 'boolean'}
 
     def int_schema(self, schema: core_schema.IntSchema) -> JsonSchemaValue:
-        json_schema = {'type': 'integer'}
+        json_schema: dict[str, Any] = {'type': 'integer'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.numeric)
         json_schema = {k: v for k, v in json_schema.items() if v not in {math.inf, -math.inf}}
         return json_schema
 
     def float_schema(self, schema: core_schema.FloatSchema) -> JsonSchemaValue:
-        json_schema = {'type': 'number'}
+        json_schema: dict[str, Any] = {'type': 'number'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.numeric)
         json_schema = {k: v for k, v in json_schema.items() if v not in {math.inf, -math.inf}}
         return json_schema
 
     def str_schema(self, schema: core_schema.StringSchema) -> JsonSchemaValue:
         json_schema = {'type': 'string'}
         self.update_with_validations(json_schema, schema, self.ValidationsMapping.string)
@@ -434,35 +437,36 @@
         generated: list[JsonSchemaValue] = []
 
         choices = schema['choices']
         for s in choices:
             try:
                 generated.append(self.generate_inner(s))
             except PydanticInvalidForJsonSchema as exc:
-                self.emit_warning('skipped-choice', str(exc))
+                self.emit_warning('skipped-choice', exc.message)
         if len(generated) == 1:
             return generated[0]
         return self.get_flattened_anyof(generated)
 
     def tagged_union_schema(self, schema: core_schema.TaggedUnionSchema) -> JsonSchemaValue:
         generated: dict[str, JsonSchemaValue] = {}
         for k, v in schema['choices'].items():
             if not isinstance(v, (str, int)):
                 try:
                     # Use str(k) since keys must be strings for json; while not technically correct,
                     # it's the closest that can be represented in valid JSON
                     generated[str(k)] = self.generate_inner(v).copy()
                 except PydanticInvalidForJsonSchema as exc:
-                    self.emit_warning('skipped-choice', str(exc))
+                    self.emit_warning('skipped-choice', exc.message)
 
         # Populate the schema with any "indirect" references
         for k, v in schema['choices'].items():
             if isinstance(v, (str, int)):
                 while isinstance(schema['choices'][v], (str, int)):
                     v = schema['choices'][v]
+                    assert isinstance(v, (int, str))
                 if str(v) in generated:
                     # while it might seem unnecessary to check `if str(v) in generated`, a PydanticInvalidForJsonSchema
                     # may have been raised above, which would mean that the schema we want to reference won't be present
                     generated[str(k)] = generated[str(v)]
 
         one_of_choices = _deduplicate_schemas(generated.values())
         json_schema: JsonSchemaValue = {'oneOf': one_of_choices}
@@ -538,28 +542,31 @@
         # because one of the following two branches failed.
         if use_strict:
             return self.generate_inner(schema['strict_schema'])
         else:
             return self.generate_inner(schema['lax_schema'])
 
     def typed_dict_schema(self, schema: core_schema.TypedDictSchema) -> JsonSchemaValue:
-        named_required_fields = [(k, v['required'], v) for k, v in schema['fields'].items()]
+        named_required_fields = [
+            (k, v['required'], v) for k, v in schema['fields'].items()  # type: ignore  # required is always populated
+        ]
         return self._named_required_fields_schema(named_required_fields)
 
     def _named_required_fields_schema(
         self, named_required_fields: Sequence[tuple[str, bool, core_schema.TypedDictField | core_schema.DataclassField]]
     ) -> JsonSchemaValue:
         properties: dict[str, JsonSchemaValue] = {}
         required_fields: list[str] = []
         for name, required, field in named_required_fields:
             if self.by_alias:
-                alias = field.get('validation_alias', name)
+                alias: Any = field.get('validation_alias', name)
                 if isinstance(alias, str):
                     name = alias
                 elif isinstance(alias, list):
+                    alias = cast('list[str] | str', alias)
                     for path in alias:
                         if isinstance(path, list) and len(path) == 1 and isinstance(path[0], str):
                             # Use the first valid single-item string path; the code that constructs the alias array
                             # should ensure the first such item is what belongs in the JSON schema
                             name = path[0]
                             break
             field_json_schema = self.generate_inner(field).copy()
@@ -569,15 +576,15 @@
             field_json_schema = self.handle_ref_overrides(field_json_schema)
             properties[name] = field_json_schema
             if required:
                 required_fields.append(name)
 
         json_schema = {'type': 'object', 'properties': properties}
         if required_fields:
-            json_schema['required'] = required_fields
+            json_schema['required'] = required_fields  # type: ignore
         return json_schema
 
     def typed_dict_field_schema(self, schema: core_schema.TypedDictField) -> JsonSchemaValue:
         json_schema = self.generate_inner(schema['schema'])
 
         return json_schema
 
@@ -777,15 +784,15 @@
     def definitions_schema(self, schema: core_schema.DefinitionsSchema) -> JsonSchemaValue:
         for definition in schema['definitions']:
             self.generate_inner(definition)
         return self.generate_inner(schema['schema'])
 
     def definition_ref_schema(self, schema: core_schema.DefinitionReferenceSchema) -> JsonSchemaValue:
         core_ref = CoreRef(schema['schema_ref'])
-        defs_ref, ref_json_schema = self.get_cache_defs_ref_schema(core_ref)
+        _, ref_json_schema = self.get_cache_defs_ref_schema(core_ref)
         return ref_json_schema
 
     # ### Utility methods
 
     def get_title_from_name(self, name: str) -> str:
         return name.title().replace('_', ' ')
```

### Comparing `pydantic-2.0a1/pydantic/main.py` & `pydantic-2.0a2/pydantic/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,134 +6,151 @@
 import typing
 import warnings
 from abc import ABCMeta
 from copy import copy, deepcopy
 from inspect import getdoc
 from pathlib import Path
 from types import prepare_class, resolve_bases
-from typing import Any, Generic
+from typing import Any, Generic, Mapping, Tuple, cast
 
 import pydantic_core
 import typing_extensions
 
 from ._internal import (
+    _config,
     _decorators,
     _forward_ref,
     _generics,
     _model_construction,
     _repr,
     _typing_extra,
     _utils,
 )
 from ._internal._fields import Undefined
-from .config import BaseConfig, ConfigDict, Extra, build_config, get_config
+from .config import ConfigDict
 from .deprecated import copy_internals as _deprecated_copy_internals
 from .deprecated import parse as _deprecated_parse
 from .errors import PydanticUndefinedAnnotation, PydanticUserError
 from .fields import Field, FieldInfo, ModelPrivateAttr
 from .json_schema import DEFAULT_REF_TEMPLATE, GenerateJsonSchema, JsonSchemaValue, model_json_schema
 
 if typing.TYPE_CHECKING:
     from inspect import Signature
 
     from pydantic_core import CoreSchema, SchemaSerializer, SchemaValidator
 
     from ._internal._generate_schema import GenerateSchema
     from ._internal._utils import AbstractSetIntStr, MappingIntStrAny
 
-    AnyClassMethod = classmethod[Any]
-    TupleGenerator = typing.Generator[tuple[str, Any], None, None]
+    AnyClassMethod = classmethod[Any, Any, Any]
+    TupleGenerator = typing.Generator[Tuple[str, Any], None, None]
     Model = typing.TypeVar('Model', bound='BaseModel')
     # should be `set[int] | set[str] | dict[int, IncEx] | dict[str, IncEx] | None`, but mypy can't cope
-    IncEx = set[int] | set[str] | dict[int, Any] | dict[str, Any] | None
+    IncEx: typing_extensions.TypeAlias = 'set[int] | set[str] | dict[int, Any] | dict[str, Any] | None'
 
 __all__ = 'BaseModel', 'create_model'
 
 _object_setattr = _model_construction.object_setattr
 # Note `ModelMetaclass` refers to `BaseModel`, but is also used to *create* `BaseModel`, so we need to add this extra
 # (somewhat hacky) boolean to keep track of whether we've created the `BaseModel` class yet, and therefore whether it's
 # safe to refer to it. If it *hasn't* been created, we assume that the `__new__` call we're in the middle of is for
 # the `BaseModel` class, since that's defined immediately after the metaclass.
 _base_class_defined = False
 
 
+class _ModelNamespaceDict(dict):  # type: ignore[type-arg]
+    """
+    Intercept attributes being set on model classes and warn about overriding of decorators (`@field_validator`, etc.)
+    """
+
+    def __setitem__(self, k: str, v: object) -> None:
+        existing: Any = self.get(k, None)
+        if existing and v is not existing and isinstance(existing, _decorators.PydanticDecoratorMarker):
+            warnings.warn(f'`{k}` overrides an existing Pydantic `{existing.decorator_info.decorator_repr}` decorator')
+
+        return super().__setitem__(k, v)
+
+
 @typing_extensions.dataclass_transform(kw_only_default=True, field_specifiers=(Field,))
 class ModelMetaclass(ABCMeta):
     def __new__(
         mcs,
         cls_name: str,
         bases: tuple[type[Any], ...],
         namespace: dict[str, Any],
-        __pydantic_generic_origin__: type[BaseModel] | None = None,
-        __pydantic_generic_args__: tuple[Any, ...] | None = None,
-        __pydantic_generic_parameters__: tuple[Any, ...] | None = None,
+        __pydantic_generic_metadata__: _generics.PydanticGenericMetadata | None = None,
         __pydantic_reset_parent_namespace__: bool = True,
         **kwargs: Any,
     ) -> type:
         if _base_class_defined:
             base_field_names, class_vars, base_private_attributes = _collect_bases_data(bases)
 
-            config_new = build_config(cls_name, bases, namespace, kwargs)
-            namespace['model_config'] = config_new
+            config_wrapper = _config.ConfigWrapper.for_model(bases, namespace, kwargs)
+            namespace['model_config'] = config_wrapper.config_dict
             private_attributes = _model_construction.inspect_namespace(
-                namespace, config_new.get('ignored_types', ()), class_vars, base_field_names
+                namespace, config_wrapper.ignored_types, class_vars, base_field_names
             )
             if private_attributes:
                 slots: set[str] = set(namespace.get('__slots__', ()))
                 namespace['__slots__'] = slots | private_attributes.keys()
 
                 if 'model_post_init' in namespace:
-                    # if there are private_attributes and a model_post_init function, we wrap them both
-                    # in a single function
-                    namespace['_init_private_attributes'] = _model_construction.init_private_attributes
-
-                    def __pydantic_post_init__(self_: Any, context: Any) -> None:
-                        self_._init_private_attributes(context)
-                        self_.model_post_init(context)
+                    # if there are private_attributes and a model_post_init function, we handle both
+                    original_model_post_init = namespace['model_post_init']
 
-                    namespace['__pydantic_post_init__'] = __pydantic_post_init__
+                    def wrapped_model_post_init(self: BaseModel, __context: Any) -> None:
+                        """
+                        We need to both initialize private attributes and call the user-defined model_post_init method
+                        """
+                        _model_construction.init_private_attributes(self, __context)
+                        original_model_post_init(self, __context)
+
+                    namespace['model_post_init'] = wrapped_model_post_init
                 else:
-                    namespace['__pydantic_post_init__'] = _model_construction.init_private_attributes
-            elif 'model_post_init' in namespace:
-                namespace['__pydantic_post_init__'] = namespace['model_post_init']
+                    namespace['model_post_init'] = _model_construction.init_private_attributes
 
             namespace['__class_vars__'] = class_vars
             namespace['__private_attributes__'] = {**base_private_attributes, **private_attributes}
 
-            if '__hash__' not in namespace and config_new['frozen']:
+            if '__hash__' not in namespace and config_wrapper.frozen:
 
-                def hash_func(self_: Any) -> int:
-                    return hash(self_.__class__) + hash(tuple(self_.__dict__.values()))
+                def hash_func(self: Any) -> int:
+                    return hash(self.__class__) + hash(tuple(self.__dict__.values()))
 
                 namespace['__hash__'] = hash_func
 
             cls: type[BaseModel] = super().__new__(mcs, cls_name, bases, namespace, **kwargs)  # type: ignore
 
             cls.__pydantic_decorators__ = _decorators.gather_decorator_functions(cls)
 
-            # FIXME all generics related attributes should be moved into a dict, like `__pydantic_decorators__`
-            parent_typevars_map = {}
-            for base in bases:
-                base_typevars_map = getattr(base, '__pydantic_generic_typevars_map__', None)
-                if base_typevars_map:
-                    parent_typevars_map.update(base_typevars_map)
-
-            cls.__pydantic_generic_args__ = __pydantic_generic_args__
-            cls.__pydantic_generic_origin__ = __pydantic_generic_origin__
-            cls.__pydantic_generic_parameters__ = __pydantic_generic_parameters__ or getattr(
-                cls, '__parameters__', None
-            )
-            cls.__pydantic_generic_defaults__ = None if not cls.__pydantic_generic_parameters__ else {}
-            if __pydantic_generic_origin__ is None:
-                cls.__pydantic_generic_typevars_map__ = None
+            # Use the getattr below to grab the __parameters__ from the `typing.Generic` parent class
+            if __pydantic_generic_metadata__:
+                cls.__pydantic_generic_metadata__ = __pydantic_generic_metadata__
             else:
-                new_typevars_map = dict(
-                    zip(_generics.iter_contained_typevars(__pydantic_generic_origin__), __pydantic_generic_args__ or ())
-                )
-                cls.__pydantic_generic_typevars_map__ = {**parent_typevars_map, **new_typevars_map}
+                parameters = getattr(cls, '__parameters__', ())
+                parent_parameters = getattr(cls, '__pydantic_generic_metadata__', {}).get('parameters', ())
+                if parameters and parent_parameters and not all(x in parameters for x in parent_parameters):
+                    combined_parameters = parent_parameters + tuple(x for x in parameters if x not in parent_parameters)
+                    parameters_str = ', '.join([str(x) for x in combined_parameters])
+                    error_message = (
+                        f'All parameters must be present on typing.Generic;'
+                        f' you should inherit from typing.Generic[{parameters_str}]'
+                    )
+                    if Generic not in bases:  # pragma: no cover
+                        # This branch will only be hit if I have misunderstood how `__parameters__` works.
+                        # If that is the case, and a user hits this, I could imagine it being very helpful
+                        # to have this extra detail in the reported traceback.
+                        error_message += f' (bases={bases})'
+                    raise TypeError(error_message)
+
+                cls.__pydantic_generic_metadata__ = {
+                    'origin': None,
+                    'args': (),
+                    'parameters': parameters,
+                }
 
             cls.__pydantic_model_complete__ = False  # Ensure this specific class gets completed
 
             # preserve `__set_name__` protocol defined in https://peps.python.org/pep-0487
             # for attributes not in `new_namespace` (e.g. private attributes)
             for name, obj in private_attributes.items():
                 set_name = getattr(obj, '__set_name__', None)
@@ -145,22 +162,31 @@
             parent_namespace = getattr(cls, '__pydantic_parent_namespace__', None)
 
             types_namespace = _model_construction.get_model_types_namespace(cls, parent_namespace)
             _model_construction.set_model_fields(cls, bases, types_namespace)
             _model_construction.complete_model_class(
                 cls,
                 cls_name,
+                config_wrapper,
                 types_namespace,
                 raise_errors=False,
             )
+            # using super(cls, cls) on the next line ensures we only call the parent class's __pydantic_init_subclass__
+            # I believe the `type: ignore` is only necessary because mypy doesn't realize that this code branch is
+            # only hit for _proper_ subclasses of BaseModel
+            super(cls, cls).__pydantic_init_subclass__(**kwargs)  # type: ignore[misc]
             return cls
         else:
             # this is the BaseModel class itself being created, no logic required
             return super().__new__(mcs, cls_name, bases, namespace, **kwargs)
 
+    @classmethod
+    def __prepare__(cls, *args: Any, **kwargs: Any) -> Mapping[str, object]:
+        return _ModelNamespaceDict()
+
     def __instancecheck__(self, instance: Any) -> bool:
         """
         Avoid calling ABC _abc_subclasscheck unless we're pretty sure.
 
         See #3829 and python/cpython#92810
         """
         return hasattr(instance, '__pydantic_validator__') and super().__instancecheck__(instance)
@@ -174,32 +200,29 @@
         __pydantic_serializer__: typing.ClassVar[SchemaSerializer]
         __pydantic_decorators__: typing.ClassVar[_decorators.DecoratorInfos]
         """metadata for `@validator`, `@root_validator` and `@serializer` decorators"""
         model_fields: typing.ClassVar[dict[str, FieldInfo]] = {}
         __signature__: typing.ClassVar[Signature]
         __private_attributes__: typing.ClassVar[dict[str, ModelPrivateAttr]]
         __class_vars__: typing.ClassVar[set[str]]
-        __fields_set__: set[str] = set()
-        __pydantic_generic_args__: typing.ClassVar[tuple[Any, ...] | None]
-        __pydantic_generic_defaults__: typing.ClassVar[dict[str, Any] | None]
-        __pydantic_generic_origin__: typing.ClassVar[type[BaseModel] | None]
-        __pydantic_generic_parameters__: typing.ClassVar[tuple[_typing_extra.TypeVarType, ...] | None]
-        __pydantic_generic_typevars_map__: typing.ClassVar[dict[_typing_extra.TypeVarType, Any] | None]
+        __pydantic_fields_set__: set[str] = set()
+        __pydantic_generic_metadata__: typing.ClassVar[_generics.PydanticGenericMetadata]
         __pydantic_parent_namespace__: typing.ClassVar[dict[str, Any] | None]
     else:
         __pydantic_validator__ = _model_construction.MockValidator(
-            'Pydantic models should inherit from BaseModel, BaseModel cannot be instantiated directly'
+            'Pydantic models should inherit from BaseModel, BaseModel cannot be instantiated directly',
+            code='base-model-instantiated',
         )
 
     model_config = ConfigDict()
-    __slots__ = '__dict__', '__fields_set__'
+    __slots__ = '__dict__', '__pydantic_fields_set__'
     __doc__ = ''  # Null out the Representation docstring
     __pydantic_model_complete__ = False
 
-    def __init__(__pydantic_self__, **data: Any) -> None:
+    def __init__(__pydantic_self__, **data: Any) -> None:  # type: ignore
         """
         Create a new model by parsing and validating input data from keyword arguments.
 
         Raises ValidationError if the input data cannot be parsed to form a valid model.
 
         Uses something other than `self` for the first arg to allow "self" as a field name.
         """
@@ -208,68 +231,92 @@
         __pydantic_self__.__pydantic_validator__.validate_python(data, self_instance=__pydantic_self__)
 
     @classmethod
     def __get_pydantic_core_schema__(cls, source: type[BaseModel], gen_schema: GenerateSchema) -> CoreSchema:
         return gen_schema.model_schema(cls)
 
     @classmethod
+    def __pydantic_init_subclass__(cls, **kwargs: Any) -> None:
+        """
+        This is intended to behave just like `__init_subclass__`, but is called by ModelMetaclass
+        only after the class is actually fully initialized. In particular, attributes like `model_fields` will
+        be present when this is called.
+
+        This is necessary because `__init_subclass__` will always be called by `type.__new__`,
+        and it would require a prohibitively large refactor to the `ModelMetaclass` to ensure that
+        `type.__new__` was called in such a manner that the class would already be sufficiently initialized.
+
+        This will receive the same `kwargs` that would be passed to the standard `__init_subclass__`, namely,
+        any kwargs passed to the class definition that aren't used internally by pydantic.
+        """
+        pass
+
+    @classmethod
     def model_validate(
         cls: type[Model], obj: Any, *, strict: bool | None = None, context: dict[str, Any] | None = None
     ) -> Model:
         # `__tracebackhide__` tells pytest and some other tools to omit this function from tracebacks
         __tracebackhide__ = True
         return cls.__pydantic_validator__.validate_python(obj, strict=strict, context=context)
 
+    @property
+    def model_fields_set(self) -> set[str]:
+        """
+        The set of fields that have been set on this model instance, i.e. that were not filled from defaults.
+        """
+        return self.__pydantic_fields_set__
+
     @classmethod
     def model_validate_json(
         cls: type[Model],
         json_data: str | bytes | bytearray,
         *,
         strict: bool | None = None,
         context: dict[str, Any] | None = None,
     ) -> Model:
         # `__tracebackhide__` tells pytest and some other tools to omit this function from tracebacks
         __tracebackhide__ = True
         return cls.__pydantic_validator__.validate_json(json_data, strict=strict, context=context)
 
-    if typing.TYPE_CHECKING:
-        # model_after_init is called after at the end of `__init__` if it's defined
-        def model_post_init(self, _context: Any) -> None:
-            pass
+    def model_post_init(self, __context: Any) -> None:
+        """
+        If you override `model_post_init`, it will be called at the end of `__init__` and `model_construct`
+        """
+        pass
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name in self.__class_vars__:
             raise AttributeError(
                 f'"{name}" is a ClassVar of `{self.__class__.__name__}` and cannot be set on an instance. '
                 f'If you want to set a value on the class, use `{self.__class__.__name__}.{name} = value`.'
             )
         if name.startswith('_'):
             _object_setattr(self, name, value)
-        elif self.model_config['frozen']:
+        elif self.model_config.get('frozen', None):
             raise TypeError(f'"{self.__class__.__name__}" is frozen and does not support item assignment')
-        elif self.model_config['validate_assignment']:
+        elif self.model_config.get('validate_assignment', None):
             self.__pydantic_validator__.validate_assignment(self, name, value)
-        elif self.model_config['extra'] is not Extra.allow and name not in self.model_fields:
+        elif self.model_config.get('extra') != 'allow' and name not in self.model_fields:
             # TODO - matching error
             raise ValueError(f'"{self.__class__.__name__}" object has no field "{name}"')
         else:
             self.__dict__[name] = value
-            self.__fields_set__.add(name)
+            self.__pydantic_fields_set__.add(name)
 
     def __getstate__(self) -> dict[Any, Any]:
         private_attrs = ((k, getattr(self, k, Undefined)) for k in self.__private_attributes__)
         return {
             '__dict__': self.__dict__,
-            '__fields_set__': self.__fields_set__,
+            '__pydantic_fields_set__': self.__pydantic_fields_set__,
             '__private_attribute_values__': {k: v for k, v in private_attrs if v is not Undefined},
         }
 
     def __setstate__(self, state: dict[Any, Any]) -> None:
         _object_setattr(self, '__dict__', state['__dict__'])
-        _object_setattr(self, '__fields_set__', state['__fields_set__'])
+        _object_setattr(self, '__pydantic_fields_set__', state['__pydantic_fields_set__'])
         for name, value in state.get('__private_attribute_values__', {}).items():
             _object_setattr(self, name, value)
 
     def model_dump(
         self,
         *,
         mode: typing_extensions.Literal['json', 'python'] | str = 'python',
@@ -326,15 +373,15 @@
             round_trip=round_trip,
             warnings=warnings,
         ).decode()
 
     @classmethod
     def model_construct(cls: type[Model], _fields_set: set[str] | None = None, **values: Any) -> Model:
         """
-        Creates a new model setting __dict__ and __fields_set__ from trusted or pre-validated data.
+        Creates a new model setting __dict__ and __pydantic_fields_set__ from trusted or pre-validated data.
         Default values are respected, but no other validation is performed.
         Behaves as if `Config.extra = 'allow'` was set since it adds all passed values
         """
         m = cls.__new__(cls)
         fields_values: dict[str, Any] = {}
         for name, field in cls.model_fields.items():
             if field.alias and field.alias in values:
@@ -343,17 +390,17 @@
                 fields_values[name] = values[name]
             elif not field.is_required():
                 fields_values[name] = field.get_default(call_default_factory=True)
         fields_values.update(values)
         _object_setattr(m, '__dict__', fields_values)
         if _fields_set is None:
             _fields_set = set(values.keys())
-        _object_setattr(m, '__fields_set__', _fields_set)
-        if hasattr(m, '__pydantic_post_init__'):
-            m.__pydantic_post_init__(context=None)
+        _object_setattr(m, '__pydantic_fields_set__', _fields_set)
+        if type(m).model_post_init is not BaseModel.model_post_init:
+            m.model_post_init(None)
         return m
 
     @classmethod
     def model_json_schema(
         cls,
         by_alias: bool = True,
         ref_template: str = DEFAULT_REF_TEMPLATE,
@@ -373,43 +420,48 @@
 
         This is a convenience method primarily intended to control how the "generic" properties of the JSON schema
         are populated. See https://json-schema.org/understanding-json-schema/reference/generic.html for more details.
 
         If you want to make more sweeping changes to how the JSON schema is generated, you will probably want to create
         a subclass of `GenerateJsonSchema` and pass it as `schema_generator` in `BaseModel.model_json_schema`.
         """
-        metadata = {'title': cls.model_config['title'] or cls.__name__, 'description': getdoc(cls) or None}
+        metadata = {'title': cls.model_config.get('title', None) or cls.__name__, 'description': getdoc(cls) or None}
         metadata = {k: v for k, v in metadata.items() if v is not None}
         return {**metadata, **json_schema}
 
     @classmethod
     def model_rebuild(
         cls,
         *,
         force: bool = False,
         raise_errors: bool = True,
         _parent_namespace_depth: int = 2,
+        _types_namespace: dict[str, Any] | None = None,
     ) -> bool | None:
         """
         Try to (Re)construct the model schema.
         """
         if not force and cls.__pydantic_model_complete__:
             return None
         else:
-            if _parent_namespace_depth > 0:
-                frame_parent_ns = _typing_extra.parent_frame_namespace(parent_depth=_parent_namespace_depth) or {}
-                cls_parent_ns = cls.__pydantic_parent_namespace__ or {}
-                cls.__pydantic_parent_namespace__ = {**cls_parent_ns, **frame_parent_ns}
+            if _types_namespace is not None:
+                types_namespace: dict[str, Any] | None = _types_namespace.copy()
+            else:
+                if _parent_namespace_depth > 0:
+                    frame_parent_ns = _typing_extra.parent_frame_namespace(parent_depth=_parent_namespace_depth) or {}
+                    cls_parent_ns = cls.__pydantic_parent_namespace__ or {}
+                    cls.__pydantic_parent_namespace__ = {**cls_parent_ns, **frame_parent_ns}
 
-            types_namespace = cls.__pydantic_parent_namespace__
+                types_namespace = cls.__pydantic_parent_namespace__
 
-            types_namespace = _model_construction.get_model_types_namespace(cls, types_namespace)
+                types_namespace = _model_construction.get_model_types_namespace(cls, types_namespace)
             return _model_construction.complete_model_class(
                 cls,
                 cls.__name__,
+                _config.ConfigWrapper(cls.model_config, check=False),
                 types_namespace,
                 raise_errors=raise_errors,
             )
 
     def __iter__(self) -> TupleGenerator:
         """
         so `dict(model)` works
@@ -419,16 +471,16 @@
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, BaseModel):
             return False
 
         # When comparing instances of generic types for equality, as long as all field values are equal,
         # only require their generic origin types to be equal, rather than exact type equality.
         # This prevents headaches like MyGeneric(x=1) != MyGeneric[Any](x=1).
-        self_type = getattr(self, '__pydantic_generic_origin__', None) or self.__class__
-        other_type = getattr(other, '__pydantic_generic_origin__', None) or other.__class__
+        self_type = self.__pydantic_generic_metadata__['origin'] or self.__class__
+        other_type = other.__pydantic_generic_metadata__['origin'] or other.__class__
 
         if self_type != other_type:
             return False
 
         if self.__dict__ != other.__dict__:
             return False
 
@@ -447,41 +499,41 @@
             the new model: you should trust this data
         :param deep: set to `True` to make a deep copy of the model
         :return: new model instance
         """
         copied = self.__deepcopy__() if deep else self.__copy__()
         if update:
             copied.__dict__.update(update)
-            copied.__fields_set__.update(update.keys())
+            copied.__pydantic_fields_set__.update(update.keys())
         return copied
 
     def __copy__(self: Model) -> Model:
         """
         Returns a shallow copy of the model
         """
         cls = type(self)
         m = cls.__new__(cls)
         _object_setattr(m, '__dict__', copy(self.__dict__))
-        _object_setattr(m, '__fields_set__', copy(self.__fields_set__))
+        _object_setattr(m, '__pydantic_fields_set__', copy(self.__pydantic_fields_set__))
         for name in self.__private_attributes__:
             value = getattr(self, name, Undefined)
             if value is not Undefined:
                 _object_setattr(m, name, value)
         return m
 
     def __deepcopy__(self: Model, memo: dict[int, Any] | None = None) -> Model:
         """
         Returns a deep copy of the model
         """
         cls = type(self)
         m = cls.__new__(cls)
         _object_setattr(m, '__dict__', deepcopy(self.__dict__, memo=memo))
-        # This next line doesn't need a deepcopy because __fields_set__ is a set[str],
+        # This next line doesn't need a deepcopy because __pydantic_fields_set__ is a set[str],
         # and attempting a deepcopy would be marginally slower.
-        _object_setattr(m, '__fields_set__', copy(self.__fields_set__))
+        _object_setattr(m, '__pydantic_fields_set__', copy(self.__pydantic_fields_set__))
         for name in self.__private_attributes__:
             value = getattr(self, name, Undefined)
             if value is not Undefined:
                 _object_setattr(m, name, deepcopy(value, memo=memo))
         return m
 
     def __repr_args__(self) -> _repr.ReprArgs:
@@ -498,37 +550,37 @@
         if cached is not None:
             return cached
 
         if cls is BaseModel:
             raise TypeError('Type parameters should be placed on typing.Generic, not BaseModel')
         if not hasattr(cls, '__parameters__'):
             raise TypeError(f'{cls} cannot be parametrized because it does not inherit from typing.Generic')
-        if not cls.__pydantic_generic_parameters__ and Generic not in cls.__bases__:
+        if not cls.__pydantic_generic_metadata__['parameters'] and Generic not in cls.__bases__:
             raise TypeError(f'{cls} is not a generic class')
 
         if not isinstance(typevar_values, tuple):
             typevar_values = (typevar_values,)
         _generics.check_parameters_count(cls, typevar_values)
 
         # Build map from generic typevars to passed params
         typevars_map: dict[_typing_extra.TypeVarType, type[Any]] = dict(
-            zip(cls.__pydantic_generic_parameters__ or (), typevar_values)
+            zip(cls.__pydantic_generic_metadata__['parameters'], typevar_values)
         )
 
         if _utils.all_identical(typevars_map.keys(), typevars_map.values()) and typevars_map:
             submodel = cls  # if arguments are equal to parameters it's the same object
             _generics.set_cached_generic_type(cls, typevar_values, submodel)
         else:
-            parent_args = cls.__pydantic_generic_args__
+            parent_args = cls.__pydantic_generic_metadata__['args']
             if not parent_args:
                 args = typevar_values
             else:
                 args = tuple(_generics.replace_types(arg, typevars_map) for arg in parent_args)
 
-            origin = cls.__pydantic_generic_origin__ or cls
+            origin = cls.__pydantic_generic_metadata__['origin'] or cls
             model_name = origin.model_parametrized_name(args)
             params = tuple(
                 {param: None for param in _generics.iter_contained_typevars(typevars_map.values())}
             )  # use dict as ordered set
 
             with _generics.generic_recursion_self_type(origin, args) as maybe_self_type:
                 if maybe_self_type is not None:
@@ -549,21 +601,14 @@
                     pass
 
                 submodel = _generics.create_generic_submodel(model_name, origin, args, params)
 
                 # Update cache
                 _generics.set_cached_generic_type(cls, typevar_values, submodel, origin, args)
 
-                # Doing the rebuild _after_ populating the cache prevents infinite recursion
-                submodel.model_rebuild(
-                    force=True,
-                    raise_errors=False,
-                    _parent_namespace_depth=0,
-                )
-
         return submodel
 
     @classmethod
     def model_parametrized_name(cls, params: tuple[type[Any], ...]) -> str:
         """
         Compute class name for parametrizations of generic classes.
 
@@ -582,14 +627,21 @@
         # If we eventually move toward wrapping them in a ForwardRef in __class_getitem__ in the future,
         # we may be able to remove this special case.
         param_names = [param if isinstance(param, str) else _repr.display_as_type(param) for param in params]
         params_component = ', '.join(param_names)
         return f'{cls.__name__}[{params_component}]'
 
     # ##### Deprecated methods from v1 #####
+    @property
+    def __fields_set__(self) -> set[str]:
+        warnings.warn(
+            'The `__fields_set__` attribute is deprecated, use `model_fields_set` instead.', DeprecationWarning
+        )
+        return self.__pydantic_fields_set__
+
     def dict(
         self,
         *,
         include: IncEx = None,
         exclude: IncEx = None,
         by_alias: bool = False,
         exclude_unset: bool = False,
@@ -643,17 +695,17 @@
         return cls.model_validate(obj)
 
     @classmethod
     def parse_raw(
         cls: type[Model],
         b: str | bytes,
         *,
-        content_type: str = None,
+        content_type: str | None = None,
         encoding: str = 'utf8',
-        proto: _deprecated_parse.Protocol = None,
+        proto: _deprecated_parse.Protocol | None = None,
         allow_pickle: bool = False,
     ) -> Model:
         warnings.warn(
             'The `parse_raw` method is deprecated; if your data is JSON use `model_json_validate`, '
             'otherwise load the data then use `model_validate` instead.',
             DeprecationWarning,
         )
@@ -688,17 +740,17 @@
         return cls.model_validate(obj)
 
     @classmethod
     def parse_file(
         cls: type[Model],
         path: str | Path,
         *,
-        content_type: str = None,
+        content_type: str | None = None,
         encoding: str = 'utf8',
-        proto: _deprecated_parse.Protocol = None,
+        proto: _deprecated_parse.Protocol | None = None,
         allow_pickle: bool = False,
     ) -> Model:
         warnings.warn(
             'The `parse_file` method is deprecated; load the data from file, then if your data is JSON '
             'use `model_json_validate` otherwise `model_validate` instead.',
             DeprecationWarning,
         )
@@ -710,20 +762,22 @@
             allow_pickle=allow_pickle,
         )
         return cls.parse_obj(obj)
 
     @classmethod
     def from_orm(cls: type[Model], obj: Any) -> Model:
         warnings.warn(
-            'The `from_orm` method is deprecated; set model_config["from_attributes"]=True '
+            'The `from_orm` method is deprecated; set `model_config["from_attributes"]=True` '
             'and use `model_validate` instead.',
             DeprecationWarning,
         )
-        if not cls.model_config['from_attributes']:
-            raise PydanticUserError('You must set the config attribute `from_attributes=True` to use from_orm')
+        if not cls.model_config.get('from_attributes', None):
+            raise PydanticUserError(
+                'You must set the config attribute `from_attributes=True` to use from_orm', code=None
+            )
         return cls.model_validate(obj)
 
     @classmethod
     def construct(cls: type[Model], _fields_set: set[str] | None = None, **values: Any) -> Model:
         warnings.warn('The `construct` method is deprecated; use `model_construct` instead.', DeprecationWarning)
         return cls.model_construct(_fields_set=_fields_set, **values)
 
@@ -745,31 +799,31 @@
         warnings.warn(
             'The `copy` method is deprecated; use `model_copy` instead. '
             'See the docstring of `BaseModel.copy` for details about how to handle `include` and `exclude`.',
             DeprecationWarning,
         )
 
         values = dict(
-            _deprecated_copy_internals._iter(
+            _deprecated_copy_internals._iter(  # type: ignore
                 self, to_dict=False, by_alias=False, include=include, exclude=exclude, exclude_unset=False
             ),
             **(update or {}),
         )
 
-        # new `__fields_set__` can have unset optional fields with a set value in `update` kwarg
+        # new `__pydantic_fields_set__` can have unset optional fields with a set value in `update` kwarg
         if update:
-            fields_set = self.__fields_set__ | update.keys()
+            fields_set = self.__pydantic_fields_set__ | update.keys()
         else:
-            fields_set = set(self.__fields_set__)
+            fields_set = set(self.__pydantic_fields_set__)
 
-        # removing excluded fields from `__fields_set__`
+        # removing excluded fields from `__pydantic_fields_set__`
         if exclude:
             fields_set -= set(exclude)
 
-        return _deprecated_copy_internals._copy_and_set_values(self, values, fields_set, deep=deep)
+        return _deprecated_copy_internals._copy_and_set_values(self, values, fields_set, deep=deep)  # type: ignore
 
     @classmethod
     def schema(
         cls, by_alias: bool = True, ref_template: str = DEFAULT_REF_TEMPLATE
     ) -> typing.Dict[str, Any]:  # noqa UP006
         warnings.warn('The `schema` method is deprecated; use `model_json_schema` instead.', DeprecationWarning)
         return cls.model_json_schema(by_alias=by_alias, ref_template=ref_template)
@@ -804,76 +858,76 @@
         )
         if localns:
             raise TypeError('`localns` arguments are not longer accepted.')
         cls.model_rebuild(force=True)
 
     def _iter(self, *args: Any, **kwargs: Any) -> Any:
         warnings.warn('The private method `_iter` will be removed and should no longer be used.', DeprecationWarning)
-        return _deprecated_copy_internals._iter(self, *args, **kwargs)
+        return _deprecated_copy_internals._iter(self, *args, **kwargs)  # type: ignore
 
     def _copy_and_set_values(self, *args: Any, **kwargs: Any) -> Any:
         warnings.warn(
             'The private method  `_copy_and_set_values` will be removed and should no longer be used.',
             DeprecationWarning,
         )
-        return _deprecated_copy_internals._copy_and_set_values(self, *args, **kwargs)
+        return _deprecated_copy_internals._copy_and_set_values(self, *args, **kwargs)  # type: ignore
 
     @classmethod
     def _get_value(cls, *args: Any, **kwargs: Any) -> Any:
         warnings.warn(
             'The private method  `_get_value` will be removed and should no longer be used.', DeprecationWarning
         )
-        return _deprecated_copy_internals._get_value(cls, *args, **kwargs)
+        return _deprecated_copy_internals._get_value(cls, *args, **kwargs)  # type: ignore
 
     def _calculate_keys(self, *args: Any, **kwargs: Any) -> Any:
         warnings.warn(
             'The private method `_calculate_keys` will be removed and should no longer be used.', DeprecationWarning
         )
-        return _deprecated_copy_internals._calculate_keys(self, *args, **kwargs)
+        return _deprecated_copy_internals._calculate_keys(self, *args, **kwargs)  # type: ignore
 
 
 _base_class_defined = True
 
 
 @typing.overload
 def create_model(
     __model_name: str,
     *,
-    __config__: ConfigDict | type[BaseConfig] | None = None,
+    __config__: ConfigDict | None = None,
     __base__: None = None,
     __module__: str = __name__,
-    __validators__: dict[str, AnyClassMethod] = None,
-    __cls_kwargs__: dict[str, Any] = None,
+    __validators__: dict[str, AnyClassMethod] | None = None,
+    __cls_kwargs__: dict[str, Any] | None = None,
     **field_definitions: Any,
-) -> type[Model]:
+) -> type[BaseModel]:
     ...
 
 
 @typing.overload
 def create_model(
     __model_name: str,
     *,
-    __config__: ConfigDict | type[BaseConfig] | None = None,
+    __config__: ConfigDict | None = None,
     __base__: type[Model] | tuple[type[Model], ...],
     __module__: str = __name__,
-    __validators__: dict[str, AnyClassMethod] = None,
-    __cls_kwargs__: dict[str, Any] = None,
+    __validators__: dict[str, AnyClassMethod] | None = None,
+    __cls_kwargs__: dict[str, Any] | None = None,
     **field_definitions: Any,
 ) -> type[Model]:
     ...
 
 
 def create_model(
     __model_name: str,
     *,
-    __config__: ConfigDict | type[BaseConfig] | None = None,
+    __config__: ConfigDict | None = None,
     __base__: type[Model] | tuple[type[Model], ...] | None = None,
     __module__: str = __name__,
-    __validators__: dict[str, AnyClassMethod] = None,
-    __cls_kwargs__: dict[str, Any] = None,
+    __validators__: dict[str, AnyClassMethod] | None = None,
+    __cls_kwargs__: dict[str, Any] | None = None,
     __slots__: tuple[str, ...] | None = None,
     **field_definitions: Any,
 ) -> type[Model]:
     """
     Dynamically create a model.
     :param __model_name: name of the created model
     :param __config__: config dict/class to use for the new model
@@ -891,50 +945,53 @@
     """
     if __slots__ is not None:
         # __slots__ will be ignored from here on
         warnings.warn('__slots__ should not be passed to create_model', RuntimeWarning)
 
     if __base__ is not None:
         if __config__ is not None:
-            raise PydanticUserError('to avoid confusion __config__ and __base__ cannot be used together')
+            raise PydanticUserError(
+                'to avoid confusion `__config__` and `__base__` cannot be used together',
+                code='create-model-config-base',
+            )
         if not isinstance(__base__, tuple):
             __base__ = (__base__,)
     else:
         __base__ = (typing.cast(typing.Type['Model'], BaseModel),)
 
     __cls_kwargs__ = __cls_kwargs__ or {}
 
     fields = {}
     annotations = {}
 
     for f_name, f_def in field_definitions.items():
         if f_name.startswith('_'):
             warnings.warn(f'fields may not start with an underscore, ignoring "{f_name}"', RuntimeWarning)
         if isinstance(f_def, tuple):
+            f_def = cast('tuple[str, Any]', f_def)
             try:
                 f_annotation, f_value = f_def
             except ValueError as e:
                 raise PydanticUserError(
-                    'field definitions should either be a tuple of (<type>, <default>) or just a '
-                    'default value, unfortunately this means tuples as '
-                    'default values are not allowed'
+                    'Field definitions should either be a `(<type>, <default>)`.',
+                    code='create-model-field-definitions',
                 ) from e
         else:
             f_annotation, f_value = None, f_def
 
         if f_annotation:
             annotations[f_name] = f_annotation
         fields[f_name] = f_value
 
     namespace: dict[str, Any] = {'__annotations__': annotations, '__module__': __module__}
     if __validators__:
         namespace.update(__validators__)
     namespace.update(fields)
     if __config__:
-        namespace['model_config'] = get_config(__config__, __model_name)
+        namespace['model_config'] = _config.ConfigWrapper(__config__).config_dict
     resolved_bases = resolve_bases(__base__)
     meta, ns, kwds = prepare_class(__model_name, resolved_bases, kwds=__cls_kwargs__)
     if resolved_bases is not __base__:
         ns['__orig_bases__'] = __base__
     namespace.update(ns)
     return meta(__model_name, resolved_bases, namespace, __pydantic_reset_parent_namespace__=False, **kwds)
```

### Comparing `pydantic-2.0a1/pydantic/mypy.py` & `pydantic-2.0a2/pydantic/mypy.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,23 +302,19 @@
         In particular:
         * determines the model config and fields,
         * adds a fields-aware signature for the initializer and construct methods
         * freezes the class if frozen = True
         * stores the fields, config, and if the class is settings in the mypy metadata for access by subclasses
         """
         ctx = self._ctx
-        info = self._ctx.cls.info
+        info = ctx.cls.info
 
         self.adjust_validator_signatures()
         config = self.collect_config()
         fields = self.collect_fields(config)
-        for field in fields:
-            if info[field.name].type is None:
-                if not ctx.api.final_iteration:
-                    ctx.api.defer()
         self.add_initializer(fields, config)
         self.add_model_construct_method(fields)
         self.set_frozen(fields, frozen=config.frozen is True)
         info.metadata[METADATA_KEY] = {
             'fields': {field.name: field.serialize() for field in fields},
             'config': config.set_values_dict(),
         }
@@ -459,15 +455,15 @@
             if (
                 isinstance(stmt.rvalue, CallExpr)
                 and isinstance(stmt.rvalue.callee, CallExpr)
                 and isinstance(stmt.rvalue.callee.callee, NameExpr)
                 and stmt.rvalue.callee.callee.fullname in DECORATOR_FULLNAMES
             ):
                 # This is a (possibly-reused) validator or serializer, not a field
-                # In particular, it looks something like: my_validator = validator('my_field', allow_reuse=True)(f)
+                # In particular, it looks something like: my_validator = validator('my_field')(f)
                 # Eventually, we may want to attempt to respect model_config['ignored_types']
                 return None
 
             # The assignment does not have an annotation, and it's not anything else we recognize
             error_untyped_fields(ctx.api, stmt)
             return None
```

### Comparing `pydantic-2.0a1/pydantic/networks.py` & `pydantic-2.0a2/pydantic/networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import dataclasses as _dataclasses
 import re
 from ipaddress import IPv4Address, IPv4Interface, IPv4Network, IPv6Address, IPv6Interface, IPv6Network
 from typing import TYPE_CHECKING, Any
 
 from pydantic_core import MultiHostUrl, PydanticCustomError, Url, core_schema
-from typing_extensions import Annotated
+from typing_extensions import Annotated, TypeAlias
 
 from ._internal import _fields, _repr
 
 if TYPE_CHECKING:
     import email_validator
 
-    NetworkType = str | bytes | int | tuple[str | bytes | int, str | int]
+    NetworkType: TypeAlias = 'str | bytes | int | tuple[str | bytes | int, str | int]'
 
 else:
     email_validator = None
 
 
 __all__ = [
     'AnyUrl',
@@ -244,15 +244,15 @@
         return cls(__input_value)  # type: ignore[return-value]
 
 
 class IPvAnyNetwork:
     __slots__ = ()
 
     def __new__(cls, value: NetworkType) -> IPv4Network | IPv6Network:  # type: ignore[misc]
-        # Assume IP Network is defined with a default value for ``strict`` argument.
+        # Assume IP Network is defined with a default value for `strict` argument.
         # Define your own class if you want to specify network address check strictness.
         try:
             return IPv4Network(value)
         except ValueError:
             pass
 
         try:
```

### Comparing `pydantic-2.0a1/pydantic/tools.py` & `pydantic-2.0a2/pydantic/tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,50 +4,58 @@
 import warnings
 from typing import Any, Callable, Type, TypeVar, Union
 
 from . import AnalyzedType
 
 __all__ = 'parse_obj_as', 'schema_of', 'schema_json_of'
 
-from ._internal import _generate_schema
 from .json_schema import DEFAULT_REF_TEMPLATE, GenerateJsonSchema
 
 NameFactory = Union[str, Callable[[Type[Any]], str]]
 
 
 T = TypeVar('T')
 
 
 def parse_obj_as(type_: type[T], obj: Any, type_name: NameFactory | None = None) -> T:
     # TODO: add deprecation warning of some sort
     if type_name is not None:  # pragma: no cover
         warnings.warn(
-            'The type_name parameter is deprecated. parse_obj_as no longer creates temporary models', stacklevel=2
+            'The type_name parameter is deprecated. parse_obj_as no longer creates temporary models',
+            DeprecationWarning,
+            stacklevel=2,
         )
     return AnalyzedType(type_).validate_python(obj)
 
 
 def schema_of(
     type_: Any,
     *,
     title: NameFactory | None = None,
     by_alias: bool = True,
     ref_template: str = DEFAULT_REF_TEMPLATE,
     schema_generator: type[GenerateJsonSchema] = GenerateJsonSchema,
 ) -> dict[str, Any]:
     """Generate a JSON schema (as dict) for the passed model or dynamically generated one"""
-    json_schema_generator = schema_generator(by_alias=by_alias, ref_template=ref_template)
-    if hasattr(type_, '__pydantic_core_schema__'):
-        core_schema = type_.__pydantic_core_schema__
-    else:
-        core_schema = _generate_schema.GenerateSchema(True, None).generate_schema(type_)
-    json_schema = json_schema_generator.generate(core_schema)
+    res = AnalyzedType(type_).json_schema(
+        by_alias=by_alias,
+        schema_generator=schema_generator,
+        ref_template=ref_template,
+    )
     if title is not None:
-        json_schema['title'] = title
-    return json_schema
+        if isinstance(title, str):
+            res['title'] = title
+        else:
+            warnings.warn(
+                'Passing a callable for the `title` parameter is deprecated and no longer supported',
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            res['title'] = title(type_)
+    return res
 
 
 def schema_json_of(
     type_: Any,
     *,
     title: NameFactory | None = None,
     by_alias: bool = True,
```

### Comparing `pydantic-2.0a1/pydantic/types.py` & `pydantic-2.0a2/pydantic/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     Any,
     ClassVar,
     FrozenSet,
     Generic,
     Hashable,
     List,
     Set,
-    Tuple,
     TypeVar,
     cast,
 )
 from uuid import UUID
 
 import annotated_types
 from pydantic_core import PydanticCustomError, PydanticKnownError, core_schema
@@ -51,14 +50,15 @@
     'condecimal',
     'UUID1',
     'UUID3',
     'UUID4',
     'UUID5',
     'FilePath',
     'DirectoryPath',
+    'NewPath',
     'Json',
     'SecretField',
     'SecretStr',
     'SecretBytes',
     'StrictBool',
     'StrictBytes',
     'StrictInt',
@@ -76,14 +76,17 @@
 from ._internal._utils import update_not_none
 
 
 @_dataclasses.dataclass
 class Strict(_fields.PydanticMetadata):
     strict: bool = True
 
+    def __hash__(self) -> int:
+        return hash(self.strict)
+
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ BOOLEAN TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 StrictBool = Annotated[bool, Strict()]
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ INTEGER TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -114,14 +117,17 @@
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ FLOAT TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 @_dataclasses.dataclass
 class AllowInfNan(_fields.PydanticMetadata):
     allow_inf_nan: bool = True
 
+    def __hash__(self) -> int:
+        return hash(self.allow_inf_nan)
+
 
 def confloat(
     *,
     strict: bool | None = None,
     gt: float | None = None,
     ge: float | None = None,
     lt: float | None = None,
@@ -195,15 +201,15 @@
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~ COLLECTION TYPES ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 HashableItemType = TypeVar('HashableItemType', bound=Hashable)
 
 
 def conset(
-    item_type: type[HashableItemType], *, min_length: int = None, max_length: int = None
+    item_type: type[HashableItemType], *, min_length: int | None = None, max_length: int | None = None
 ) -> type[set[HashableItemType]]:
     return Annotated[  # type: ignore[return-value]
         Set[item_type], annotated_types.Len(min_length or 0, max_length)  # type: ignore[valid-type]
     ]
 
 
 def confrozenset(
@@ -223,23 +229,14 @@
 ) -> type[list[AnyItemType]]:
     return Annotated[  # type: ignore[return-value]
         List[item_type],  # type: ignore[valid-type]
         annotated_types.Len(min_length or 0, max_length),
     ]
 
 
-def contuple(
-    item_type: type[AnyItemType], *, min_length: int | None = None, max_length: int | None = None
-) -> type[tuple[AnyItemType]]:
-    return Annotated[  # type: ignore[return-value]
-        Tuple[item_type],
-        annotated_types.Len(min_length or 0, max_length),
-    ]
-
-
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~ IMPORT STRING TYPE ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 AnyType = TypeVar('AnyType')
 if TYPE_CHECKING:
     ImportString = Annotated[AnyType, ...]
 else:
 
@@ -365,14 +362,17 @@
         if path.exists():
             raise PydanticCustomError('path_exists', 'path already exists')
         elif not path.parent.exists():
             raise PydanticCustomError('parent_does_not_exist', 'Parent directory does not exist')
         else:
             return path
 
+    def __hash__(self) -> int:
+        return hash(type(self.path_type))
+
 
 FilePath = Annotated[Path, PathType('file')]
 DirectoryPath = Annotated[Path, PathType('dir')]
 NewPath = Annotated[Path, PathType('new')]
 
 
 # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ JSON TYPE ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -785,15 +785,22 @@
                 schema['now_op'] = 'future'
                 return schema
 
         def __repr__(self) -> str:
             return 'FutureDate'
 
 
-def condate(*, strict: bool = None, gt: date = None, ge: date = None, lt: date = None, le: date = None) -> type[date]:
+def condate(
+    *,
+    strict: bool | None = None,
+    gt: date | None = None,
+    ge: date | None = None,
+    lt: date | None = None,
+    le: date | None = None,
+) -> type[date]:
     return Annotated[  # type: ignore[return-value]
         date,
         Strict(strict) if strict is not None else None,
         annotated_types.Interval(gt=gt, ge=ge, lt=lt, le=le),
     ]
```

### Comparing `pydantic-2.0a1/pydantic/version.py` & `pydantic-2.0a2/pydantic/_internal/_serializers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-__all__ = 'VERSION', 'version_info'
+from __future__ import annotations as _annotations
 
-VERSION = '2.0a1'
+from collections import deque
+from typing import Any, Pattern
 
+from pydantic_core import PydanticOmit
+from pydantic_core.core_schema import SerializationInfo, SerializerFunctionWrapHandler
 
-def version_info() -> str:
-    import platform
-    import sys
-    from importlib import import_module
-    from pathlib import Path
 
-    optional_deps = []
-    for p in 'devtools', 'email-validator', 'typing-extensions':
+def pattern_serializer(input_value: Pattern[Any], info: SerializationInfo) -> str | Pattern[Any]:
+    if info.mode == 'json':
+        return input_value.pattern
+    else:
+        return input_value
+
+
+def serialize_deque(
+    __value: Any, __serialize: SerializerFunctionWrapHandler, __info: SerializationInfo
+) -> list[Any] | deque[Any]:
+    items = []
+    for index, item in enumerate(__value):
         try:
-            import_module(p.replace('-', '_'))
-        except ImportError:
-            continue
-        optional_deps.append(p)
-
-    info = {
-        'pydantic version': VERSION,
-        'install path': Path(__file__).resolve().parent,
-        'python version': sys.version,
-        'platform': platform.platform(),
-        'optional deps. installed': optional_deps,
-    }
-    return '\n'.join('{:>30} {}'.format(k + ':', str(v).replace('\n', ' ')) for k, v in info.items())
+            v = __serialize(item, index)
+        except PydanticOmit:
+            pass
+        else:
+            items.append(v)
+    if __info.mode_is_json():
+        return items
+    else:
+        return deque(items)
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_core_metadata.py` & `pydantic-2.0a2/pydantic/_internal/_core_metadata.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/pydantic/_internal/_core_utils.py` & `pydantic-2.0a2/pydantic/_internal/_core_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,20 @@
 def get_type_ref(type_: type[Any], args_override: tuple[type[Any], ...] | None = None) -> str:
     """
     Produces the ref to be used for this type by pydantic_core's core schemas.
 
     This `args_override` argument was added for the purpose of creating valid recursive references
     when creating generic models without needing to create a concrete class.
     """
-    origin = getattr(type_, '__pydantic_generic_origin__', None) or type_
-    args = getattr(type_, '__pydantic_generic_args__', None) or args_override or ()
+    origin = type_
+    args = args_override or ()
+    generic_metadata = getattr(type_, '__pydantic_generic_metadata__', None)
+    if generic_metadata:
+        origin = generic_metadata['origin'] or origin
+        args = generic_metadata['args'] or args
 
     module_name = getattr(origin, '__module__', '<No __module__>')
     qualname = getattr(origin, '__qualname__', f'<No __qualname__: {origin}>')
     type_ref = f'{module_name}.{qualname}:{id(origin)}'
 
     arg_refs: list[str] = []
     for arg in args:
@@ -95,15 +99,15 @@
     after the first can safely be replaced.
 
     In most cases, schemas with the same ref should not actually be produced, or should be completely identical.
     However, as an implementation detail, recursive generic models will emit a non-identical schema deeper in the
     tree with a re-used ref, with the intent that that schema gets replaced with a recursive reference once the
     specific generic parametrization to use can be determined.
     """
-    refs = set()
+    refs: set[str] = set()
 
     def _replace_refs(s: core_schema.CoreSchema) -> core_schema.CoreSchema:
         ref: str | None = s.get('ref')  # type: ignore[assignment]
         if ref:
             if ref in refs:
                 return {'type': 'definition-ref', 'schema_ref': ref}
             refs.add(ref)
@@ -137,19 +141,25 @@
 
     def _remove_invalid_defs(s: core_schema.CoreSchema) -> core_schema.CoreSchema:
         if s['type'] != 'definitions':
             return s
 
         new_schema = s.copy()
 
-        new_definitions = []
+        new_definitions: list[CoreSchema] = []
         for definition in s['definitions']:
             metadata = definition.get('metadata')
-            if isinstance(metadata, dict) and 'invalid' in metadata and definition['ref'] in valid_refs:
+            # fmt: off
+            if (
+                isinstance(metadata, dict)
+                and 'invalid' in metadata
+                and definition['ref'] in valid_refs  # type: ignore
+            ):
                 continue
+            # fmt: on
             new_definitions.append(definition)
 
         new_schema['definitions'] = new_definitions
         return new_schema
 
     return WalkAndApply(_remove_invalid_defs).walk(schema)
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_dataclasses.py` & `pydantic-2.0a2/pydantic/_internal/_dataclasses.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,32 @@
 Private logic for creating pydantic dataclasses.
 """
 from __future__ import annotations as _annotations
 
 import typing
 import warnings
 from functools import wraps
-from typing import Any, Callable, ClassVar
+from typing import Any, Callable, ClassVar, cast
 
 from pydantic_core import ArgsKwargs, SchemaSerializer, SchemaValidator, core_schema
 
-from ..config import ConfigDict
 from ..errors import PydanticUndefinedAnnotation
 from ..fields import FieldInfo
 from . import _decorators
 from ._core_utils import get_type_ref
 from ._fields import collect_fields
 from ._forward_ref import PydanticForwardRef
-from ._generate_schema import dataclass_schema, generate_config
+from ._generate_schema import dataclass_schema
 from ._model_construction import MockValidator
 
 __all__ = 'StandardDataclass', 'PydanticDataclass', 'prepare_dataclass'
 
 if typing.TYPE_CHECKING:
+    from ..config import ConfigDict
+    from ._config import ConfigWrapper
 
     class StandardDataclass(typing.Protocol):
         __dataclass_fields__: ClassVar[dict[str, Any]]
         __dataclass_params__: ClassVar[Any]  # in reality `dataclasses._DataclassParams`
         __post_init__: ClassVar[Callable[..., None]]
 
         def __init__(self, *args: object, **kwargs: object) -> None:
@@ -40,15 +41,15 @@
         """metadata for `@validator`, `@root_validator` and `@serializer` decorators"""
         __pydantic_fields__: typing.ClassVar[dict[str, FieldInfo]]
         __pydantic_config__: typing.ClassVar[ConfigDict]
 
 
 def prepare_dataclass(
     cls: type[Any],
-    config: ConfigDict,
+    config_wrapper: ConfigWrapper,
     kw_only: bool,
     *,
     raise_errors: bool = True,
     types_namespace: dict[str, Any] | None = None,
 ) -> bool:
     """
     Prepare a raw class to become a pydantic dataclass.
@@ -58,68 +59,70 @@
     This logic is called on a class which is yet to be wrapped in `dataclasses.dataclass()`.
     """
     if hasattr(cls, '__post_init_post_parse__'):
         warnings.warn(
             'Support for `__post_init_post_parse__` has been dropped, the method will not be called', DeprecationWarning
         )
 
+    cls = cast('type[PydanticDataclass]', cls)
+
     name = cls.__name__
     bases = cls.__bases__
 
     dataclass_ref = get_type_ref(cls)
     self_schema = core_schema.definition_reference_schema(dataclass_ref)
     types_namespace = {**(types_namespace or {}), name: PydanticForwardRef(self_schema, cls)}
     try:
         fields, _ = collect_fields(cls, bases, types_namespace, is_dataclass=True, dc_kw_only=kw_only)
     except PydanticUndefinedAnnotation as e:
         if raise_errors:
             raise
         warning_string = (
             f'`{name}` is not fully defined, you should define `{e}`, then call TODO! `methods.rebuild({name})`'
         )
-        if config['undefined_types_warning']:
+        if config_wrapper.undefined_types_warning:
             raise UserWarning(warning_string)
-        cls.__pydantic_validator__ = MockValidator(warning_string)
+        cls.__pydantic_validator__ = MockValidator(warning_string, code='dataclass-not-fully-defined')  # type: ignore
         return False
 
     decorators = cls.__pydantic_decorators__
 
     cls.__pydantic_core_schema__ = schema = dataclass_schema(
         cls,
         dataclass_ref,
         fields,
         decorators,
-        config['arbitrary_types_allowed'],
+        config_wrapper,
         types_namespace,
     )
 
-    core_config = generate_config(config, cls)
+    core_config = config_wrapper.core_config(cls)
     cls.__pydantic_fields__ = fields
     cls.__pydantic_validator__ = validator = SchemaValidator(schema, core_config)
     # this works because cls has been transformed into a dataclass by the time "cls" is called
     cls.__pydantic_serializer__ = SchemaSerializer(schema, core_config)
-    cls.__pydantic_config__ = config
+    cls.__pydantic_config__ = config_wrapper.config_dict
 
-    if config.get('validate_assignment'):
+    if config_wrapper.validate_assignment:
 
         @wraps(cls.__setattr__)
         def validated_setattr(instance: Any, __field: str, __value: str) -> None:
             validator.validate_assignment(instance, __field, __value)
 
-        cls.__setattr__ = validated_setattr.__get__(None, cls)
+        cls.__setattr__ = validated_setattr.__get__(None, cls)  # type: ignore
 
     # dataclass.__init__ must be defined here so its `__qualname__` can be changed since functions can't copied.
 
     def __init__(__dataclass_self__: PydanticDataclass, *args: Any, **kwargs: Any) -> None:
         __tracebackhide__ = True
         s = __dataclass_self__
         s.__pydantic_validator__.validate_python(ArgsKwargs(args, kwargs), self_instance=s)
 
     __init__.__qualname__ = f'{cls.__qualname__}.__init__'
-    cls.__init__ = __init__
+    cls.__init__ = __init__  # type: ignore
 
     return True
 
 
 def is_builtin_dataclass(_cls: type[Any]) -> bool:
     """
     Whether a class is a stdlib dataclass
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_decorators.py` & `pydantic-2.0a2/pydantic/_internal/_decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Logic related to validators applied to models etc. via the `@validator` and `@root_validator` decorators.
 """
 from __future__ import annotations as _annotations
 
-import warnings
+from dataclasses import field
+from functools import partial, partialmethod
 from inspect import Parameter, Signature, signature
 from typing import (
-    TYPE_CHECKING,
     Any,
     Callable,
+    ClassVar,
     Dict,
     Generic,
     Set,
     Tuple,
     TypeVar,
     Union,
     cast,
@@ -29,269 +30,210 @@
     GeneralWrapSerializerFunction,
     JsonReturnTypes,
     SerializationInfo,
     SerializerFunctionWrapHandler,
     ValidationInfo,
     WhenUsed,
 )
-from typing_extensions import Protocol, TypeAlias
-
-from pydantic._internal._repr import Representation
-
-if TYPE_CHECKING:
-    from typing_extensions import Literal
+from typing_extensions import Literal, Protocol, TypeAlias
 
+from ..errors import PydanticUserError
+from ._core_utils import get_type_ref
+from ._internal_dataclass import slots_dataclass
 
 FIELD_VALIDATOR_TAG = '_field_validator'
 ROOT_VALIDATOR_TAG = '_root_validator'
 
 FIELD_SERIALIZER_TAG = '_field_serializer'
 
 
-class ValidatorDecoratorInfo(Representation):
+@slots_dataclass
+class ValidatorDecoratorInfo:
     """
     A container for data from `@validator` so that we can access it
     while building the pydantic-core schema.
     """
 
-    __slots__ = 'fields', 'mode', 'each_item', 'always', 'check_fields'
+    decorator_repr: ClassVar[str] = '@validator'
 
     fields: tuple[str, ...]
     mode: Literal['before', 'after']
     each_item: bool
     always: bool
     check_fields: bool | None
 
-    def __init__(
-        self,
-        *,
-        fields: tuple[str, ...],
-        # pre=True/False in v1 should be converted to mode='before'/'after' in v2
-        mode: Literal['before', 'after'],
-        each_item: bool,
-        always: bool,
-        check_fields: bool | None,
-    ) -> None:
-        """
-        :param mode: the pydantic-core validator mode.
-        :param check_fields: whether to check that the fields actually exist on the model.
-        :param each_item: if True this validator gets applied to the internal items of
-            lists/sets/dicts instead of the collection itself.
-        """
-        self.fields = fields
-        self.mode = mode
-        self.each_item = each_item
-        self.always = always
-        self.check_fields = check_fields
 
-
-class FieldValidatorDecoratorInfo(Representation):
+@slots_dataclass
+class FieldValidatorDecoratorInfo:
     """
     A container for data from `@field_validator` so that we can access it
     while building the pydantic-core schema.
     """
 
-    __slots__ = 'fields', 'mode', 'sub_path', 'check_fields'
+    decorator_repr: ClassVar[str] = '@field_validator'
 
     fields: tuple[str, ...]
     mode: Literal['before', 'after', 'wrap', 'plain']
-    sub_path: tuple[str | int, ...] | None
     check_fields: bool | None
 
-    def __init__(
-        self,
-        *,
-        fields: tuple[str, ...],
-        mode: Literal['before', 'after', 'wrap', 'plain'],
-        sub_path: tuple[str | int, ...] | None,
-        check_fields: bool | None,
-    ) -> None:
-        """
-        :param fields: the fields this validator applies to.
-        :param mode: the pydantic-core validator mode.
-        :param sub_path: Not yet supported.
-        :param check_fields: whether to check that the fields actually exist on the model.
-        """
-        self.fields = fields
-        self.mode = mode
-        self.sub_path = sub_path
-        self.check_fields = check_fields
-
 
-class RootValidatorDecoratorInfo(Representation):
+@slots_dataclass
+class RootValidatorDecoratorInfo:
     """
     A container for data from `@root_validator` so that we can access it
     while building the pydantic-core schema.
     """
 
-    def __init__(
-        self,
-        *,
-        mode: Literal['before', 'after'],
-    ) -> None:
-        """
-        :param mode: the pydantic-core validator mode
-        """
-        self.mode = mode
+    decorator_repr: ClassVar[str] = '@root_validator'
+    mode: Literal['before', 'after']
 
 
-class FieldSerializerDecoratorInfo(Representation):
+@slots_dataclass
+class FieldSerializerDecoratorInfo:
     """
     A container for data from `@field_serializer` so that we can access it
     while building the pydantic-core schema.
     """
 
-    __slots__ = 'fields', 'sub_path', 'mode', 'json_return_type', 'when_used', 'check_fields', 'type'
-
+    decorator_repr: ClassVar[str] = '@field_serializer'
     fields: tuple[str, ...]
     mode: Literal['plain', 'wrap']
     type: Literal['general', 'field']
     json_return_type: JsonReturnTypes | None
     when_used: WhenUsed
-    sub_path: tuple[str | int, ...] | None
     check_fields: bool | None
 
-    def __init__(
-        self,
-        *,
-        fields: tuple[str, ...],
-        mode: Literal['plain', 'wrap'],
-        type: Literal['general', 'field'],
-        json_return_type: JsonReturnTypes | None = None,
-        when_used: WhenUsed = 'always',
-        sub_path: tuple[str | int, ...] | None = None,
-        check_fields: bool | None = None,
-    ) -> None:
-        self.fields = fields
-        self.sub_path = sub_path
-        self.mode = mode
-        self.json_return_type = json_return_type
-        self.when_used = when_used
-        self.check_fields = check_fields
-        self.type = type
-
 
-class ModelSerializerDecoratorInfo(Representation):
+@slots_dataclass
+class ModelSerializerDecoratorInfo:
     """
     A container for data from `@model_serializer` so that we can access it
     while building the pydantic-core schema.
     """
 
-    __slots__ = 'mode', 'json_return_type', 'when_used'
-
+    decorator_repr: ClassVar[str] = '@model_serializer'
     mode: Literal['plain', 'wrap']
     json_return_type: JsonReturnTypes | None
 
-    def __init__(
-        self,
-        *,
-        mode: Literal['plain', 'wrap'],
-        json_return_type: JsonReturnTypes | None = None,
-    ) -> None:
-        self.mode = mode
-        self.json_return_type = json_return_type
+
+@slots_dataclass
+class ModelValidatorDecoratorInfo:
+    """
+    A container for data from `@model_validator` so that we can access it
+    while building the pydantic-core schema.
+    """
+
+    decorator_repr: ClassVar[str] = '@model_validator'
+    mode: Literal['wrap', 'before', 'after']
 
 
 DecoratorInfo = Union[
     ValidatorDecoratorInfo,
     FieldValidatorDecoratorInfo,
     RootValidatorDecoratorInfo,
     FieldSerializerDecoratorInfo,
     ModelSerializerDecoratorInfo,
+    ModelValidatorDecoratorInfo,
 ]
 
 ReturnType = TypeVar('ReturnType')
-DecoratedType: TypeAlias = 'Union[classmethod[ReturnType], staticmethod[ReturnType], Callable[..., ReturnType]]'
+DecoratedType: TypeAlias = (
+    'Union[classmethod[Any, Any, ReturnType], staticmethod[Any, ReturnType], Callable[..., ReturnType]]'
+)
 
 
-class PydanticDecoratorMarker(Generic[ReturnType], Representation):
+@slots_dataclass
+class PydanticDecoratorMarker(Generic[ReturnType]):
     """
     Wrap a classmethod, staticmethod or unbound function
     and act as a descriptor that allows us to detect decorated items
     from the class' attributes.
 
     This class' __get__ returns the wrapped item's __get__ result,
     which makes it transparent for classmethods and staticmethods.
     """
 
-    def __init__(
-        self,
-        wrapped: DecoratedType[ReturnType],
-        decorator_info: DecoratorInfo,
-        shim: Callable[[Callable[..., Any]], Callable[..., Any]] | None,
-    ) -> None:
-        self.wrapped = wrapped
-        self.decorator_info = decorator_info
-        self.shim = shim
+    wrapped: DecoratedType[ReturnType]
+    decorator_info: DecoratorInfo
+    shim: Callable[[Callable[..., Any]], Callable[..., Any]] | None
 
     @overload
     def __get__(self, obj: None, objtype: None) -> PydanticDecoratorMarker[ReturnType]:
         ...
 
     @overload
     def __get__(self, obj: object, objtype: type[object]) -> Callable[..., ReturnType]:
         ...
 
     def __get__(
         self, obj: object | None, objtype: type[object] | None = None
     ) -> Callable[..., ReturnType] | PydanticDecoratorMarker[ReturnType]:
-        if obj is None:
-            return self
-        return self.wrapped.__get__(obj, objtype)
+        try:
+            return self.wrapped.__get__(obj, objtype)
+        except AttributeError:
+            # not a descriptor, e.g. a partial object
+            return self.wrapped  # type: ignore[return-value]
 
 
 DecoratorInfoType = TypeVar('DecoratorInfoType', bound=DecoratorInfo)
 
 
-class Decorator(Generic[DecoratorInfoType], Representation):
+@slots_dataclass
+class Decorator(Generic[DecoratorInfoType]):
     """
     A generic container class to join together the decorator metadata
     (metadata from decorator itself, which we have when the
     decorator is called but not when we are building the core-schema)
     and the bound function (which we have after the class itself is created).
     """
 
-    def __init__(
-        self,
+    cls_ref: str
+    cls_var_name: str
+    func: Callable[..., Any]
+    shim: Callable[[Any], Any] | None
+    info: DecoratorInfoType
+
+    @staticmethod
+    def build(
+        cls_: Any,
         cls_var_name: str,
-        func: Callable[..., Any],
-        unwrapped_func: Callable[..., Any],
+        shim: Callable[[Any], Any] | None,
         info: DecoratorInfoType,
-    ) -> None:
-        self.cls_var_name = cls_var_name
-        self.func = func
-        self.unwrapped_func = unwrapped_func
-        self.info = info
-
-
-AnyDecorator = Union[
-    Decorator[ValidatorDecoratorInfo],
-    Decorator[FieldValidatorDecoratorInfo],
-    Decorator[RootValidatorDecoratorInfo],
-    Decorator[FieldSerializerDecoratorInfo],
-    Decorator[ModelSerializerDecoratorInfo],
-]
+    ) -> Decorator[DecoratorInfoType]:
+        func = getattr(cls_, cls_var_name)
+        if shim is not None:
+            func = shim(func)
+        return Decorator(
+            cls_ref=get_type_ref(cls_),
+            cls_var_name=cls_var_name,
+            func=func,
+            shim=shim,
+            info=info,
+        )
+
+    def bind_to_cls(self, cls: Any) -> Decorator[DecoratorInfoType]:
+        return self.build(
+            cls,
+            cls_var_name=self.cls_var_name,
+            shim=self.shim,
+            info=self.info,
+        )
 
 
-class DecoratorInfos(Representation):
+@slots_dataclass
+class DecoratorInfos:
     # mapping of name in the class namespace to decorator info
     # note that the name in the class namespace is the function or attribute name
     # not the field name!
-    validator: dict[str, Decorator[ValidatorDecoratorInfo]]
-    field_validator: dict[str, Decorator[FieldValidatorDecoratorInfo]]
-    root_validator: dict[str, Decorator[RootValidatorDecoratorInfo]]
-    field_serializer: dict[str, Decorator[FieldSerializerDecoratorInfo]]
-    model_serializer: dict[str, Decorator[ModelSerializerDecoratorInfo]]
-
-    def __init__(self) -> None:
-        self.validator = {}
-        self.field_validator = {}
-        self.root_validator = {}
-        self.field_serializer = {}
-        self.model_serializer = {}
+    validator: dict[str, Decorator[ValidatorDecoratorInfo]] = field(default_factory=dict)
+    field_validator: dict[str, Decorator[FieldValidatorDecoratorInfo]] = field(default_factory=dict)
+    root_validator: dict[str, Decorator[RootValidatorDecoratorInfo]] = field(default_factory=dict)
+    field_serializer: dict[str, Decorator[FieldSerializerDecoratorInfo]] = field(default_factory=dict)
+    model_serializer: dict[str, Decorator[ModelSerializerDecoratorInfo]] = field(default_factory=dict)
+    model_validator: dict[str, Decorator[ModelValidatorDecoratorInfo]] = field(default_factory=dict)
 
 
 def gather_decorator_functions(cls: type[Any]) -> DecoratorInfos:
     """
     We want to collect all DecFunc instances that exist as
     attributes in the namespace of the class (a BaseModel or dataclass)
     that called us
@@ -303,125 +245,147 @@
     works with inheritance.
     If we do replace any functions we put the replacement into the position
     the replaced function was in; that is, we maintain the order.
     """
 
     # reminder: dicts are ordered and replacement does not alter the order
     res = DecoratorInfos()
-    for base in cls.__bases__:
+    for base in cls.__bases__[::-1]:
         existing = cast(Union[DecoratorInfos, None], getattr(base, '__pydantic_decorators__', None))
         if existing is not None:
-            res.validator.update(existing.validator)
-            res.field_validator.update(existing.field_validator)
-            res.root_validator.update(existing.root_validator)
-            res.field_serializer.update(existing.field_serializer)
-            res.model_serializer.update(existing.model_serializer)
+            res.validator.update({k: v.bind_to_cls(cls) for k, v in existing.validator.items()})
+            res.field_validator.update({k: v.bind_to_cls(cls) for k, v in existing.field_validator.items()})
+            res.root_validator.update({k: v.bind_to_cls(cls) for k, v in existing.root_validator.items()})
+            res.field_serializer.update({k: v.bind_to_cls(cls) for k, v in existing.field_serializer.items()})
+            res.model_serializer.update({k: v.bind_to_cls(cls) for k, v in existing.model_serializer.items()})
 
     for var_name, var_value in vars(cls).items():
         if isinstance(var_value, PydanticDecoratorMarker):
-            func = var_value.wrapped.__get__(None, cls)
-            shimmed_func = var_value.shim(func) if var_value.shim is not None else func
             info = var_value.decorator_info
             if isinstance(info, ValidatorDecoratorInfo):
-                res.validator[var_name] = Decorator(var_name, shimmed_func, func, info)
+                res.validator[var_name] = Decorator.build(cls, cls_var_name=var_name, shim=var_value.shim, info=info)
             elif isinstance(info, FieldValidatorDecoratorInfo):
-                res.field_validator[var_name] = Decorator(var_name, shimmed_func, func, info)
+                res.field_validator[var_name] = Decorator.build(
+                    cls, cls_var_name=var_name, shim=var_value.shim, info=info
+                )
             elif isinstance(info, RootValidatorDecoratorInfo):
-                res.root_validator[var_name] = Decorator(var_name, shimmed_func, func, info)
+                res.root_validator[var_name] = Decorator.build(
+                    cls, cls_var_name=var_name, shim=var_value.shim, info=info
+                )
             elif isinstance(info, FieldSerializerDecoratorInfo):
-                res.field_serializer[var_name] = Decorator(var_name, shimmed_func, func, info)
+                # check whether a serializer function is already registered for fields
+                for field_serializer_decorator in res.field_serializer.values():
+                    # check that each field has at most one serializer function.
+                    # serializer functions for the same field in subclasses are allowed,
+                    # and are treated as overrides
+                    if field_serializer_decorator.cls_var_name == var_name:
+                        continue
+                    for f in info.fields:
+                        if f in field_serializer_decorator.info.fields:
+                            raise PydanticUserError(
+                                'Multiple field serializer functions were defined '
+                                f'for field {f!r}, this is not allowed.',
+                                code='multiple-field-serializers',
+                            )
+                res.field_serializer[var_name] = Decorator.build(
+                    cls, cls_var_name=var_name, shim=var_value.shim, info=info
+                )
+            elif isinstance(info, ModelValidatorDecoratorInfo):
+                res.model_validator[var_name] = Decorator.build(
+                    cls, cls_var_name=var_name, shim=var_value.shim, info=info
+                )
             else:
                 assert isinstance(info, ModelSerializerDecoratorInfo)
-                res.model_serializer[var_name] = Decorator(var_name, shimmed_func, func, info)
-            # replace our marker with the bound, concrete function
-            setattr(cls, var_name, func)
-
+                res.model_serializer[var_name] = Decorator.build(
+                    cls, cls_var_name=var_name, shim=var_value.shim, info=info
+                )
+            setattr(cls, var_name, var_value.wrapped)
     return res
 
 
 _FUNCS: set[str] = set()
 
 
-def prepare_serializer_decorator(
-    function: Callable[..., Any] | classmethod[Any] | staticmethod[Any], allow_reuse: bool
-) -> Callable[..., Any] | classmethod[Any]:
-    """
-    Warn about validators/serializers with duplicated names since without this, they can be overwritten silently
-    which generally isn't the intended behaviour, don't run in ipython (see #312) or if `allow_reuse` is True.
-    """
-    if isinstance(function, staticmethod):
-        function = function.__func__
-    if not allow_reuse and not in_ipython():
-        ref = f'{function.__module__}::{function.__qualname__}'
-        if ref in _FUNCS:
-            warnings.warn(f'duplicate validator function "{ref}"; if this is intended, set `allow_reuse=True`')
-        _FUNCS.add(ref)
-    return function
+AnyDecoratorCallable: TypeAlias = (
+    'Union[classmethod[Any, Any, Any], staticmethod[Any, Any], partialmethod[Any], Callable[..., Any]]'
+)
 
 
-def unwrap_unbound_methods(function: Callable[..., Any] | classmethod[Any] | staticmethod[Any]) -> Callable[..., Any]:
-    """
-    Unwrap unbound classmethods and staticmethods
-    """
-    if isinstance(function, (classmethod, staticmethod)):
-        return function.__func__
-    return function
+def unwrap_wrapped_function(
+    func: Any,
+    *,
+    unwrap_class_static_method: bool = True,
+) -> Any:
+    """
+    Recursively unwraps a wrapped function until the underlying function is reached.
+    This handles functools.partial, functools.partialmethod, staticmethod and classmethod.
+
+    Args:
+        func: The function to unwrap.
+        unwrap_class_static_method: If True (default), also unwrap classmethod and staticmethod
+            decorators. If False, only unwrap partial and partialmethod decorators.
+
+    Returns:
+        The underlying function of the wrapped function.
+    """
+    all: tuple[Any, ...]
+    if unwrap_class_static_method:
+        all = (
+            staticmethod,
+            classmethod,
+            partial,
+            partialmethod,
+        )
+    else:
+        all = partial, partialmethod
+
+    while isinstance(func, all):
+        if unwrap_class_static_method and isinstance(func, (classmethod, staticmethod)):
+            func = func.__func__
+        elif isinstance(func, (partial, partialmethod)):
+            func = func.func
+
+    return func
+
+
+def get_function_ref(func: Any) -> str:
+    func = unwrap_wrapped_function(func)
+    return (
+        getattr(func, '__module__', '<No __module__>')
+        + '.'
+        + getattr(func, '__qualname__', f'<No __qualname__: id:{id(func)}>')
+    )
 
 
-def is_classmethod_from_sig(function: Callable[..., Any] | classmethod[Any] | staticmethod[Any]) -> bool:
-    sig = signature(unwrap_unbound_methods(function))
+def is_classmethod_from_sig(function: AnyDecoratorCallable) -> bool:
+    sig = signature(unwrap_wrapped_function(function))
     first = next(iter(sig.parameters.values()), None)
     if first and first.name == 'cls':
         return True
     return False
 
 
-def is_instance_method_from_sig(function: Callable[..., Any] | classmethod[Any] | staticmethod[Any]) -> bool:
-    sig = signature(unwrap_unbound_methods(function))
+def is_instance_method_from_sig(function: AnyDecoratorCallable) -> bool:
+    sig = signature(unwrap_wrapped_function(function))
     first = next(iter(sig.parameters.values()), None)
     if first and first.name == 'self':
         return True
     return False
 
 
 def ensure_classmethod_based_on_signature(
-    function: Callable[..., Any] | classmethod[Any] | staticmethod[Any],
-) -> classmethod[Any] | staticmethod[Any] | Callable[..., Any]:
-    if not isinstance(function, classmethod) and is_classmethod_from_sig(function):
-        return classmethod(function)
+    function: AnyDecoratorCallable,
+) -> Any:
+    if not isinstance(
+        unwrap_wrapped_function(function, unwrap_class_static_method=False), classmethod
+    ) and is_classmethod_from_sig(function):
+        return classmethod(function)  # type: ignore[arg-type]
     return function
 
 
-def check_for_duplicate_validator(
-    function: Callable[..., Any] | classmethod[Any] | staticmethod[Any], allow_reuse: bool
-) -> None:
-    """
-    Warn about validators with duplicated names since without this, they can be overwritten silently
-    which generally isn't the intended behaviour, don't run in ipython (see #312) or if `allow_reuse` is True.
-    """
-    if not allow_reuse and not in_ipython():
-        function = unwrap_unbound_methods(function)
-        ref = f'{function.__module__}::{function.__qualname__}'
-        if ref in _FUNCS:
-            warnings.warn(f'duplicate validator function "{ref}"; if this is intended, set `allow_reuse=True`')
-        _FUNCS.add(ref)
-
-
-def in_ipython() -> bool:
-    """
-    Check whether we're in an ipython environment, including jupyter notebooks.
-    """
-    try:
-        eval('__IPYTHON__')
-    except NameError:
-        return False
-    else:  # pragma: no cover
-        return True
-
-
 class OnlyValueValidator(Protocol):
     """
     A simple validator, supported for V1 validators and V2 validators
     """
 
     def __call__(self, __value: Any) -> Any:
         ...
@@ -448,121 +412,78 @@
 
 
 V1Validator = Union[
     V1ValidatorWithValues, V1ValidatorWithValuesKwOnly, V1ValidatorWithKwargs, V1ValidatorWithValuesAndKwargs
 ]
 
 
-V1_VALIDATOR_VALID_SIGNATURES = """\
-def f1(value: Any) -> Any: ...
-def f2(value: Any, values: Dict[str, Any]) -> Any: ...
-
-class Model(BaseModel):
-    x: int
-
-    @validator('x')
-    @classmethod  # optional
-    def val_x1(cls, value: Any) -> Any: ...
-
-    @validator('x')
-    @classmethod  # optional
-    def val_x2(cls, value: Any, values: Dict[str, Any]) -> Any: ...
-
-    @validator('x')
-    @staticmethod  # required
-    def val_x3(value: Any) -> Any: ...
-
-    @validator('x')
-    @staticmethod  # required
-    def val_x4(value: Any, values: Dict[str, Any]) -> Any: ...
+def can_be_positional(param: Parameter) -> bool:
+    return param.kind in (Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD)
 
-    val_x5 = validator('x')(f1)
-    val_x6 = validator('x')(f2)
-"""
+
+def can_be_keyword(param: Parameter) -> bool:
+    return param.kind in (Parameter.POSITIONAL_OR_KEYWORD, Parameter.KEYWORD_ONLY)
 
 
 def make_generic_v1_field_validator(validator: V1Validator) -> FieldValidatorFunction:
-    sig = signature(unwrap_unbound_methods(validator))
-    positional_params: list[str] = []
-    keyword_only_params: list[str] = []
-    accepts_kwargs = False
-    for param_name, parameter in sig.parameters.items():
-        if param_name in ('field', 'config'):
-            raise TypeError(
-                'The `field` and `config` parameters are not available in Pydantic V2.'
-                ' Please use the `info` parameter instead.'
-                ' You can access the configuration via `info.config`,'
-                ' but it is a dictionary instead of an object like it was in Pydantic V1.'
-                ' The `field` argument is no longer available.'
-            )
-        if parameter.kind in (Parameter.POSITIONAL_ONLY, Parameter.POSITIONAL_OR_KEYWORD):
-            positional_params.append(param_name)
-        elif parameter.kind is Parameter.KEYWORD_ONLY:
-            keyword_only_params.append(param_name)
-        else:
-            assert parameter.kind is Parameter.VAR_KEYWORD
-            accepts_kwargs = True
+    sig = signature(validator)
 
-    accepts_values_kw = (keyword_only_params == ['values'] and len(positional_params) == 1) or (
-        len(positional_params) == 2 and positional_params[1] == 'values'
-    )
+    needs_values_kw = False
 
-    if accepts_kwargs and len(positional_params) == 1:
-        # has (v, **kwargs) or (v, values, **kwargs)
-        val1 = cast(Union[V1ValidatorWithKwargs, V1ValidatorWithValuesAndKwargs], validator)
+    for param_num, (param_name, parameter) in enumerate(sig.parameters.items()):
+        if can_be_keyword(parameter) and param_name in ('field', 'config'):
+            raise PydanticUserError(
+                'The `field` and `config` parameters are not available in Pydantic V2, '
+                'please use the `info` parameter instead.',
+                code='validator-field-config-info',
+            )
+        if parameter.kind is Parameter.VAR_KEYWORD:
+            needs_values_kw = True
+        elif can_be_keyword(parameter) and param_name == 'values':
+            needs_values_kw = True
+        elif can_be_positional(parameter) and param_num == 0:
+            # value
+            continue
+        elif parameter.default is Parameter.empty:  # ignore params with defaults e.g. bound by functools.partial
+            raise PydanticUserError(
+                f'Unsupported signature for V1 style validator {validator}: {sig} is not supported.',
+                code='validator-v1-signature',
+            )
+
+    if needs_values_kw:
+        # (v, **kwargs), (v, values, **kwargs), (v, *, values, **kwargs) or (v, *, values)
+        val1 = cast(V1ValidatorWithValues, validator)
 
         def wrapper1(value: Any, info: FieldValidationInfo) -> Any:
             return val1(value, values=info.data)
 
         return wrapper1
-    if len(positional_params) == 1 and keyword_only_params == []:
-        # (v) -> Any
+    else:
         val2 = cast(OnlyValueValidator, validator)
 
-        def wrapper2(value: Any, _: ValidationInfo) -> Any:
+        def wrapper2(value: Any, _: FieldValidationInfo) -> Any:
             return val2(value)
 
         return wrapper2
-    elif len(positional_params) in (1, 2) and accepts_values_kw:
-        # (v, values) -> Any or (v, *, values) -> Any
-        val3 = cast(V1ValidatorWithValues, validator)
-
-        def wrapper3(value: Any, info: FieldValidationInfo) -> Any:
-            return val3(value, values=info.data)
-
-        return wrapper3
-    raise TypeError(
-        f'Unsupported signature for V1 style validator {validator}: {sig} is not supported.'
-        f' Valid signatures are:\n{V1_VALIDATOR_VALID_SIGNATURES}'
-    )
-
 
-@overload
-def make_generic_v2_field_validator(
-    validator: FieldWrapValidatorFunction, mode: Literal['wrap']
-) -> FieldWrapValidatorFunction:
-    ...
 
+def remove_params_with_defaults(sig: Signature) -> Signature:
+    return Signature([p for p in sig.parameters.values() if p.default is Parameter.empty])
 
-@overload
-def make_generic_v2_field_validator(
-    validator: OnlyValueValidator | FieldValidatorFunction, mode: Literal['before', 'after', 'plain']
-) -> FieldValidatorFunction:
-    ...
 
-
-def make_generic_v2_field_validator(
+def make_generic_validator(
     validator: OnlyValueValidator | FieldValidatorFunction | FieldWrapValidatorFunction, mode: str
-) -> FieldValidatorFunction | FieldWrapValidatorFunction:
+) -> Any:
     """
     In order to support different signatures, including deprecated validator signatures from v1,
     we introspect the function signature and wrap it in a parent function that has a signature
     compatible with pydantic_core
     """
-    if mode in ('before', 'after', 'plain') and len(signature(validator).parameters) == 1:
+    sig = remove_params_with_defaults(signature(validator))
+    if mode in ('before', 'after', 'plain') and len(sig.parameters) == 1:
         val1 = cast(OnlyValueValidator, validator)
 
         # allow the (v) -> Any signature as a convenience
         def wrapper1(value: Any, info: FieldValidationInfo) -> Any:
             return val1(value)
 
         return wrapper1
@@ -632,58 +553,21 @@
 AnySerializerFunction = Union[
     GenericPlainSerializerFunctionWithoutInfo,
     GeneralWrapSerializerFunctionWithoutInfo,
     AnyCoreSerializer,
 ]
 
 
-_VALID_SERIALIZER_SIGNATURES = """\
-Valid serializer signatures are:
-
-# an instance method with the default mode or `mode='plain'`
-@serializer('x')  # or @serialize('x', mode='plain')
-def ser_x(self, value: Any, info: pydantic.FieldSerializationInfo): ...
-
-# a static method or free-standing function with the default mode or `mode='plain'`
-@serializer('x')  # or @serialize('x', mode='plain')
-@staticmethod
-def ser_x(value: Any, info: pydantic.FieldSerializationInfo): ...
-# equivalent to
-def ser_x(value: Any, info: pydantic.FieldSerializationInfo): ...
-serializer('x')(ser_x)
-
-# an instance method with `mode='wrap'`
-@serializer('x', mode='wrap')
-def ser_x(self, value: Any, nxt: pydantic.SerializerFunctionWrapHandler, info: pydantic.FieldSerializationInfo): ...
-
-# a static method or free-standing function with `mode='wrap'`
-@serializer('x', mode='wrap')
-@staticmethod
-def ser_x(value: Any, nxt: pydantic.SerializerFunctionWrapHandler, info: pydantic.FieldSerializationInfo): ...
-# equivalent to
-def ser_x(value: Any, nxt: pydantic.SerializerFunctionWrapHandler, info: pydantic.FieldSerializationInfo): ...
-serializer('x')(ser_x)
-
-For all of these, you can also choose to omit the `info` argument, for example:
-
-@serializer('x')
-def ser_x(self, value: Any): ...
-
-@serializer('x', mode='wrap')
-def ser_x(self, value: Any, handler: pydantic.SerializerFunctionWrapHandler): ...
-"""
-
-
-def make_generic_field_serializer(
+def make_generic_serializer(
     serializer: AnySerializerFunction, mode: Literal['plain', 'wrap'], type: Literal['field', 'general']
-) -> AnyCoreSerializer:
+) -> Any:
     """
     Wrap serializers to allow ignoring the `info` argument as a convenience.
     """
-    sig = signature(serializer)
+    sig = remove_params_with_defaults(signature(serializer))
     if is_instance_method_from_sig(serializer):
         # for the errors below to exclude self
         sig = Signature(parameters=list(sig.parameters.values())[1:])
 
     n_positional = sum(
         1
         for param in sig.parameters.values()
@@ -703,17 +587,17 @@
                 func2 = cast(FieldPlainSerializerFunctionWithoutInfo, serializer)
 
                 def wrap_field_serializer_single_argument(self: Any, value: Any, _: SerializationInfo) -> Any:
                     return func2(self, value)
 
                 return wrap_field_serializer_single_argument
         if n_positional != 2:
-            raise TypeError(
-                f'Unrecognized serializer signature for {serializer} with `mode={mode}`:{sig}\n'
-                f' {_VALID_SERIALIZER_SIGNATURES}'
+            raise PydanticUserError(
+                f'Unrecognized field_serializer signature for {serializer} with `mode={mode}`:{sig}',
+                code='field-serializer-signature',
             )
         func = cast(AnyCoreSerializer, serializer)
         return func
     else:
         assert mode == 'wrap'
         if n_positional == 2:
             if type == 'general':
@@ -733,17 +617,17 @@
                     self: Any, value: Any, handler: SerializerFunctionWrapHandler, _: SerializationInfo
                 ) -> Any:
                     return func4(self, value, handler)
 
                 return wrap_field_serializer_in_wrap_mode
 
         if n_positional != 3:
-            raise TypeError(
-                f'Unrecognized serializer signature for {serializer} with `mode={mode}`:{sig}\n'
-                f' {_VALID_SERIALIZER_SIGNATURES}'
+            raise PydanticUserError(
+                f'Unrecognized field_serializer signature for {serializer} with `mode={mode}`:{sig}',
+                code='field-serializer-signature',
             )
         func = cast(AnyCoreSerializer, serializer)
         return func
 
 
 def make_generic_model_serializer(
     serializer: AnySerializerFunction, mode: Literal['plain', 'wrap']
@@ -763,15 +647,18 @@
             func1 = cast(GenericPlainSerializerFunctionWithoutInfo, serializer)
 
             def wrap_model_serializer_single_argument(value: Any, _: SerializationInfo) -> Any:
                 return func1(value)
 
             return wrap_model_serializer_single_argument
         if n_positional != 2:
-            raise TypeError(f'Unrecognized serializer signature for {serializer} with `mode={mode}`:{sig}')
+            raise PydanticUserError(
+                f'Unrecognized model_serializer signature for {serializer} with `mode={mode}`:{sig}',
+                code='model-serializer-signature',
+            )
         func = cast(AnyCoreSerializer, serializer)
         return func
     else:
         assert mode == 'wrap'
         if n_positional == 2:
             func2 = cast(GeneralWrapSerializerFunctionWithoutInfo, serializer)
 
@@ -779,10 +666,13 @@
                 value: Any, handler: SerializerFunctionWrapHandler, _: SerializationInfo
             ) -> Any:
                 return func2(value, handler)
 
             return wrap_model_serializer_in_wrap_mode
 
         if n_positional != 3:
-            raise TypeError(f'Unrecognized serializer signature for {serializer} with `mode={mode}`:{sig}')
+            raise PydanticUserError(
+                f'Unrecognized serializer signature for {serializer} with `mode={mode}`:{sig}',
+                code='model-serializer-signature',
+            )
         func = cast(AnyCoreSerializer, serializer)
         return func
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_discriminated_union.py` & `pydantic-2.0a2/pydantic/_internal/_discriminated_union.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,40 +291,47 @@
         """
         This method just extracts the _infer_discriminator_values_for_choice logic specific to TypedDictSchema
         for the sake of readability.
         """
         source = 'TypedDict' if source_name is None else f'Model {source_name!r}'
         field = choice['fields'].get(self.discriminator)
         if field is None:
-            raise PydanticUserError(f'{source} needs a discriminator field for key {self.discriminator!r}')
+            raise PydanticUserError(
+                f'{source} needs a discriminator field for key {self.discriminator!r}', code='discriminator-no-field'
+            )
         return self._infer_discriminator_values_for_field(field, source)
 
     def _infer_discriminator_values_for_dataclass_choice(
         self, choice: core_schema.DataclassArgsSchema, source_name: str | None = None
     ) -> list[str | int]:
         source = 'DataclassArgs' if source_name is None else f'Dataclass {source_name!r}'
         for field in choice['fields']:
             if field['name'] == self.discriminator:
                 break
         else:
-            raise PydanticUserError(f'{source} needs a discriminator field for key {self.discriminator!r}')
+            raise PydanticUserError(
+                f'{source} needs a discriminator field for key {self.discriminator!r}', code='discriminator-no-field'
+            )
         return self._infer_discriminator_values_for_field(field, source)
 
     def _infer_discriminator_values_for_field(
         self, field: core_schema.TypedDictField | core_schema.DataclassField, source: str
     ) -> list[str | int]:
         alias = field.get('validation_alias', self.discriminator)
         if not isinstance(alias, str):
-            raise TypeError(f'Alias {alias!r} is not supported in a discriminated union')
+            raise PydanticUserError(
+                f'Alias {alias!r} is not supported in a discriminated union', code='discriminator-alias-type'
+            )
         if self._discriminator_alias is None:
             self._discriminator_alias = alias
         elif self._discriminator_alias != alias:
             raise PydanticUserError(
                 f'Aliases for discriminator {self.discriminator!r} must be the same '
-                f'(got {alias}, {self._discriminator_alias})'
+                f'(got {alias}, {self._discriminator_alias})',
+                code='discriminator-alias',
             )
         return self._infer_discriminator_values_for_inner_schema(field['schema'], source)
 
     def _infer_discriminator_values_for_inner_schema(
         self, schema: core_schema.CoreSchema, source: str
     ) -> list[str | int]:
         """
@@ -352,15 +359,18 @@
             return values
 
         elif schema['type'] == 'default':
             # This will happen if the field has a default value; we ignore it while extracting the discriminator values
             return self._infer_discriminator_values_for_inner_schema(schema['schema'], source)
 
         else:
-            raise PydanticUserError(f'{source} needs field {self.discriminator!r} to be of type `Literal`')
+            raise PydanticUserError(
+                f'{source} needs field {self.discriminator!r} to be of type `Literal`',
+                code='discriminator-needs-literal',
+            )
 
     def _set_unique_choice_for_values(self, choice: core_schema.CoreSchema, values: Sequence[str | int]) -> None:
         """
         This method updates `self.tagged_union_choices` so that all provided (discriminator) `values` map to the
         provided `choice`, validating that none of these values already map to another (different) choice.
         """
         primary_value: str | int | None = None
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_fields.py` & `pydantic-2.0a2/pydantic/_internal/_fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from abc import ABC, abstractmethod
 from copy import copy
 from typing import TYPE_CHECKING, Any
 
 from pydantic_core import core_schema
 
 from ._forward_ref import PydanticForwardRef
-from ._generics import replace_types
+from ._generics import get_typevars_map, replace_types
 from ._repr import Representation
-from ._typing_extra import get_cls_type_hints_lenient, get_type_hints, is_classvar
+from ._typing_extra import get_cls_type_hints_lenient, get_type_hints, is_classvar, is_finalvar
 
 if TYPE_CHECKING:
     from ..fields import FieldInfo
 
 
 def get_type_hints_infer_globalns(
     obj: Any,
@@ -148,14 +148,17 @@
     omitted_fields: set[str] | None = getattr(cls, '__pydantic_omitted_fields__', None)
 
     class_vars: set[str] = set()
     for ann_name, ann_type in type_hints.items():
         if is_classvar(ann_type):
             class_vars.add(ann_name)
             continue
+        if _is_finalvar_with_default_val(ann_type, getattr(cls, ann_name, Undefined)):
+            class_vars.add(ann_name)
+            continue
         if ann_name.startswith('_') or (omitted_fields and ann_name in omitted_fields):
             continue
 
         if DC_KW_ONLY and ann_type is DC_KW_ONLY:
             # all field fields will be kw_only
             dc_kw_only = True
             continue
@@ -170,15 +173,15 @@
             ann_type = Any
         elif isinstance(ann_type, dataclasses.InitVar):
             init_var = True
             ann_type = ann_type.type
 
         # when building a generic model with `MyModel[int]`, the generic_origin check makes sure we don't get
         # "... shadows an attribute" errors
-        generic_origin = getattr(cls, '__pydantic_generic_origin__', None)
+        generic_origin = getattr(cls, '__pydantic_generic_metadata__', {}).get('origin')
         for base in bases:
             if hasattr(base, ann_name):
                 if base is generic_origin:
                     # Don't error when "shadowing" of attributes in parametrized generics
                     continue
                 if is_dataclass and dataclasses.is_dataclass(base):
                     # Don't error when shadowing a field in a parent dataclass
@@ -186,16 +189,14 @@
                 raise NameError(
                     f'Field name "{ann_name}" shadows an attribute in parent "{base.__qualname__}"; '
                     f'you might want to use a different field name with "alias=\'{ann_name}\'".'
                 )
 
         try:
             default = getattr(cls, ann_name, Undefined)
-            if default is Undefined and generic_origin:
-                default = (generic_origin.__pydantic_generic_defaults__ or {}).get(ann_name, Undefined)
             if default is Undefined:
                 raise AttributeError
         except AttributeError:
             if ann_name in annotations or isinstance(ann_type, PydanticForwardRef):
                 field_info = FieldInfo.from_annotation(ann_type)
             else:
                 # if field has no default value and is not in __annotations__ this means that it is
@@ -213,26 +214,23 @@
                     # Nothing stops us from just creating a new FieldInfo for this type hint, so we do this.
                     field_info = FieldInfo.from_annotation(ann_type)
         else:
             if isinstance(default, dataclasses.Field):
                 if not default.init:
                     # dataclasses.Field with init=False are not fields
                     continue
-                if DC_KW_ONLY and default.kw_only is True:
+                if DC_KW_ONLY and default.kw_only is True:  # type: ignore
                     kw_only = True
 
             field_info = FieldInfo.from_annotated_attribute(ann_type, default)
             # attributes which are fields are removed from the class namespace:
             # 1. To match the behaviour of annotation-only fields
             # 2. To avoid false positives in the NameError check above
             try:
                 delattr(cls, ann_name)
-                if cls.__pydantic_generic_parameters__:  # model can be parametrized
-                    assert cls.__pydantic_generic_defaults__ is not None
-                    cls.__pydantic_generic_defaults__[ann_name] = default
             except AttributeError:
                 pass  # indicates the attribute was on a parent class
 
             if is_dataclass:
                 # for dataclasses we preserve the default value if it is set
                 # field, e.g. `a: int = 1` gets kept as is
                 # and `a: int = field(default=1, repr=False)` gets converted to the above
@@ -248,19 +246,34 @@
 
         if init_var:
             field_info.init_var = True
         if kw_only is not None:
             field_info.kw_only = kw_only
         fields[ann_name] = field_info
 
-    typevars_map = getattr(cls, '__pydantic_generic_typevars_map__', None)
-    if typevars_map:
-        for field in fields.values():
-            try:
-                field.annotation = typing._eval_type(  # type: ignore[attr-defined]
-                    field.annotation, types_namespace, None
-                )
-            except NameError:
-                pass
-            field.annotation = replace_types(field.annotation, typevars_map)
+    generic_metadata = getattr(cls, '__pydantic_generic_metadata__', None)
+    if generic_metadata:
+        typevars_map = get_typevars_map(generic_metadata['origin'], generic_metadata['args'])
+        if typevars_map:
+            for field in fields.values():
+                try:
+                    field.annotation = typing._eval_type(  # type: ignore[attr-defined]
+                        field.annotation, types_namespace, None
+                    )
+                except NameError:
+                    pass
+                field.annotation = replace_types(field.annotation, typevars_map)
 
     return fields, class_vars
+
+
+def _is_finalvar_with_default_val(type_: type[Any], val: Any) -> bool:
+    from pydantic.fields import FieldInfo
+
+    if not is_finalvar(type_):
+        return False
+    elif val is Undefined:
+        return False
+    elif isinstance(val, FieldInfo) and (val.default is Undefined and val.default_factory is None):
+        return False
+    else:
+        return True
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_forward_ref.py` & `pydantic-2.0a2/pydantic/_internal/_forward_ref.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pydantic_core import core_schema
 from typing_extensions import Literal, TypedDict
 
 from ._typing_extra import TypeVarType
 
 if TYPE_CHECKING:
     from pydantic import BaseModel
+    from pydantic._internal._dataclasses import PydanticDataclass
 
 
 class DeferredClassGetitem(TypedDict):
     kind: Literal['class_getitem']
     item: Any
 
 
@@ -44,15 +45,15 @@
     """
     No-op marker class for (recursive) type references.
 
     Most of the logic here exists to handle recursive generics.
     """
 
     schema: core_schema.CoreSchema
-    model: type[BaseModel]
+    model: type[BaseModel] | type[PydanticDataclass]
     deferred_actions: tuple[DeferredAction, ...] = ()
 
     __name__ = 'PydanticForwardRef'
     __hash__ = object.__hash__
 
     def __call__(self) -> None:
         """
@@ -64,18 +65,18 @@
         updated_actions = self.deferred_actions + ({'kind': 'class_getitem', 'item': item},)
         return replace(self, deferred_actions=updated_actions)
 
     def replace_types(self, typevars_map: Any) -> PydanticForwardRef:
         updated_actions = self.deferred_actions + ({'kind': 'replace_types', 'typevars_map': typevars_map},)
         return replace(self, deferred_actions=updated_actions)
 
-    def resolve_model(self) -> type[BaseModel] | PydanticForwardRef:
+    def resolve_model(self) -> type[BaseModel] | type[PydanticDataclass] | PydanticForwardRef:
         from ._generics import replace_types
 
-        model: type[BaseModel] | PydanticForwardRef = self.model
+        model: type[BaseModel] | type[PydanticDataclass] | PydanticForwardRef = self.model
         for action in self.deferred_actions:
             if action['kind'] == 'replace_types':
                 model = replace_types(model, action['typevars_map'])
             elif action['kind'] == 'class_getitem':
                 model = model[action['item']]  # type: ignore[index]
             else:
                 raise ValueError(f'Unexpected action: {action}')
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_generate_schema.py` & `pydantic-2.0a2/pydantic/_internal/_generate_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,47 +10,53 @@
 import typing
 import warnings
 from itertools import chain
 from typing import TYPE_CHECKING, Any, Callable, ForwardRef, Iterable, Mapping, TypeVar, Union
 
 from annotated_types import BaseMetadata, GroupedMetadata
 from pydantic_core import SchemaError, SchemaValidator, core_schema
-from typing_extensions import Annotated, Literal, TypedDict, get_args, get_origin, is_typeddict
+from typing_extensions import Annotated, Final, Literal, TypedDict, get_args, get_origin, is_typeddict
+
+from pydantic.annotated_arguments import AfterValidator, BeforeValidator, PlainSerializer, WrapSerializer, WrapValidator
 
 from ..errors import PydanticSchemaGenerationError, PydanticUndefinedAnnotation, PydanticUserError
 from ..fields import FieldInfo
 from ..json_schema import JsonSchemaValue, update_json_schema
 from . import _discriminated_union, _typing_extra
+from ._config import ConfigWrapper
 from ._core_metadata import CoreMetadataHandler, build_metadata_dict
 from ._core_utils import (
     consolidate_refs,
     define_expected_missing_refs,
     get_type_ref,
     is_list_like_schema_with_items_schema,
     remove_unnecessary_invalid_definitions,
 )
 from ._decorators import (
     Decorator,
     DecoratorInfos,
     FieldSerializerDecoratorInfo,
     FieldValidatorDecoratorInfo,
     ModelSerializerDecoratorInfo,
+    ModelValidatorDecoratorInfo,
     RootValidatorDecoratorInfo,
     ValidatorDecoratorInfo,
+    make_generic_serializer,
+    make_generic_validator,
 )
 from ._fields import PydanticGeneralMetadata, PydanticMetadata, Undefined, collect_fields, get_type_hints_infer_globalns
 from ._forward_ref import PydanticForwardRef, PydanticRecursiveRef
 from ._generics import recursively_defined_type_refs, replace_types
+from ._typing_extra import is_finalvar
 
 if TYPE_CHECKING:
-    from ..config import ConfigDict
     from ..main import BaseModel
     from ._dataclasses import StandardDataclass
 
-__all__ = 'dataclass_schema', 'GenerateSchema', 'generate_config'
+__all__ = 'dataclass_schema', 'GenerateSchema'
 
 _SUPPORTS_TYPEDDICT = sys.version_info >= (3, 11)
 
 FieldDecoratorInfo = Union[ValidatorDecoratorInfo, FieldValidatorDecoratorInfo, FieldSerializerDecoratorInfo]
 FieldDecoratorInfoType = TypeVar('FieldDecoratorInfoType', bound=FieldDecoratorInfo)
 AnyFieldDecorator = Union[
     Decorator[ValidatorDecoratorInfo],
@@ -80,16 +86,17 @@
             # V1 compat: accept `'*'` as a wildcard that matches all fields
             continue
         if dec.info.check_fields is False:
             continue
         for field in dec.info.fields:
             if field not in fields:
                 raise PydanticUserError(
-                    f'Validators defined with incorrect fields: {dec.unwrapped_func.__name__}'
-                    " (use check_fields=False if you're inheriting from the model and intended this)"
+                    f'Validators defined with incorrect fields: {dec.cls_ref}.{dec.cls_var_name}'
+                    " (use check_fields=False if you're inheriting from the model and intended this)",
+                    code='decorator-missing-field',
                 )
 
 
 def filter_field_decorator_info_by_field(
     validator_functions: Iterable[Decorator[FieldDecoratorInfoType]], field: str
 ) -> list[Decorator[FieldDecoratorInfoType]]:
     return [dec for dec in validator_functions if check_validator_fields_against_field_name(dec.info, field)]
@@ -125,74 +132,55 @@
 
 
 def dataclass_schema(
     cls: type[Any],
     ref: str,
     fields: dict[str, FieldInfo],
     decorators: DecoratorInfos,
-    arbitrary_types: bool,
+    config_wrapper: ConfigWrapper,
     types_namespace: dict[str, Any] | None,
 ) -> core_schema.CoreSchema:
     """
     Generate schema for a dataclass.
     """
     # TODO add typevars_map argument when we support generic dataclasses
-    schema_generator = GenerateSchema(arbitrary_types, types_namespace)
+    schema_generator = GenerateSchema(config_wrapper, types_namespace)
     args = [schema_generator.generate_dc_field_schema(k, v, decorators) for k, v in fields.items()]
     has_post_init = hasattr(cls, '__post_init__')
     args_schema = core_schema.dataclass_args_schema(cls.__name__, args, collect_init_only=has_post_init)
     inner_schema = apply_validators(args_schema, decorators.root_validator.values())
     dc_schema = core_schema.dataclass_schema(cls, inner_schema, post_init=has_post_init, ref=ref)
-    return apply_model_serializers(dc_schema, decorators.model_serializer.values())
-
-
-def generate_config(config: ConfigDict, cls: type[Any]) -> core_schema.CoreConfig:
-    """
-    Create a pydantic-core config from a pydantic config.
-    """
-    extra = None if config['extra'] is None else config['extra'].value
-    core_config = core_schema.CoreConfig(  # type: ignore[misc]
-        **core_schema.dict_not_none(
-            title=config['title'] or cls.__name__,
-            extra_fields_behavior=extra,
-            allow_inf_nan=config['allow_inf_nan'],
-            populate_by_name=config['populate_by_name'],
-            str_strip_whitespace=config['str_strip_whitespace'],
-            str_to_lower=config['str_to_lower'],
-            str_to_upper=config['str_to_upper'],
-            strict=config['strict'],
-            ser_json_timedelta=config['ser_json_timedelta'],
-            ser_json_bytes=config['ser_json_bytes'],
-            from_attributes=config['from_attributes'],
-            loc_by_alias=config['loc_by_alias'],
-            revalidate_instances=config['revalidate_instances'],
-            validate_default=config['validate_default'],
-            str_max_length=config.get('str_max_length'),
-            str_min_length=config.get('str_min_length'),
-        )
-    )
-    return core_config
+    schema = apply_model_serializers(dc_schema, decorators.model_serializer.values())
+    return apply_model_validators(schema, decorators.model_validator.values())
 
 
 class GenerateSchema:
-    __slots__ = '_arbitrary_types_stack', 'types_namespace', 'typevars_map', 'recursion_cache', 'definitions'
+    __slots__ = '_config_wrapper_stack', 'types_namespace', 'typevars_map', 'recursion_cache', 'definitions'
 
     def __init__(
-        self, arbitrary_types: bool, types_namespace: dict[str, Any] | None, typevars_map: dict[Any, Any] | None = None
+        self,
+        config_wrapper: ConfigWrapper,
+        types_namespace: dict[str, Any] | None,
+        typevars_map: dict[Any, Any] | None = None,
     ):
-        self._arbitrary_types_stack: list[bool] = [arbitrary_types]  # we need a stack for recursing into child models
+        # we need a stack for recursing into child models
+        self._config_wrapper_stack: list[ConfigWrapper] = [config_wrapper]
         self.types_namespace = types_namespace
         self.typevars_map = typevars_map
 
         self.recursion_cache: dict[str, core_schema.DefinitionReferenceSchema] = {}
         self.definitions: dict[str, core_schema.CoreSchema] = {}
 
     @property
+    def config_wrapper(self) -> ConfigWrapper:
+        return self._config_wrapper_stack[-1]
+
+    @property
     def arbitrary_types(self) -> bool:
-        return self._arbitrary_types_stack[-1]
+        return self.config_wrapper.arbitrary_types_allowed
 
     def generate_schema(self, obj: Any) -> core_schema.CoreSchema:
         schema = self._generate_schema(obj)
 
         schema = remove_unnecessary_invalid_definitions(schema)
 
         js_modify_function = _get_pydantic_modify_json_schema(obj)
@@ -210,14 +198,16 @@
 
         return schema
 
     def model_schema(self, cls: type[BaseModel]) -> core_schema.CoreSchema:
         """
         Generate schema for a pydantic model.
         """
+        from pydantic.main import BaseModel
+
         model_ref = get_type_ref(cls)
         cached_def = self.recursion_cache.get(model_ref)
         if cached_def is not None:
             return cached_def
 
         self.recursion_cache[model_ref] = core_schema.definition_reference_schema(model_ref)
         fields = cls.model_fields
@@ -229,39 +219,41 @@
                 decorators.validator.values(),
             ),
             fields.keys(),
         )
         # TODO: we need to do something similar to this for pydantic dataclasses
         #   This should be straight forward once we expose the pydantic config on the dataclass;
         #   I have done this in my PR for dataclasses JSON schema
-        self._arbitrary_types_stack.append(cls.model_config['arbitrary_types_allowed'])
+        config_wrapper = ConfigWrapper(cls.model_config, check=False)
+        self._config_wrapper_stack.append(config_wrapper)
         try:
             fields_schema: core_schema.CoreSchema = core_schema.typed_dict_schema(
                 {k: self.generate_td_field_schema(k, v, decorators) for k, v in fields.items()},
                 return_fields_set=True,
             )
         finally:
-            self._arbitrary_types_stack.pop()
+            self._config_wrapper_stack.pop()
         inner_schema = apply_validators(fields_schema, decorators.root_validator.values())
 
         inner_schema = consolidate_refs(inner_schema)
         inner_schema = define_expected_missing_refs(inner_schema, recursively_defined_type_refs())
 
-        core_config = generate_config(cls.model_config, cls)
-        model_post_init = '__pydantic_post_init__' if hasattr(cls, '__pydantic_post_init__') else None
+        core_config = config_wrapper.core_config()
+        model_post_init = None if cls.model_post_init is BaseModel.model_post_init else 'model_post_init'
 
         model_schema = core_schema.model_schema(
             cls,
             inner_schema,
             ref=model_ref,
             config=core_config,
             post_init=model_post_init,
             metadata=build_metadata_dict(js_modify_function=cls.model_modify_json_schema),
         )
-        return apply_model_serializers(model_schema, decorators.model_serializer.values())
+        schema = apply_model_serializers(model_schema, decorators.model_serializer.values())
+        return apply_model_validators(schema, decorators.model_validator.values())
 
     def _generate_schema_from_property(self, obj: Any, source: Any) -> core_schema.CoreSchema | None:
         """
         Try to generate schema from either the `__get_pydantic_core_schema__` function or
         `__pydantic_core_schema__` property.
 
         Note: `__get_pydantic_core_schema__` takes priority so it can decide whether to use a `__pydantic_core_schema__`
@@ -364,14 +356,18 @@
                 # TODO: We would need to handle generic subclasses of certain typing dict subclasses here
                 #   This includes subclasses of typing.Counter, typing.DefaultDict, and typing.OrderedDict
                 #   Note also that we may do a better job of handling typing.DefaultDict by inspecting its arguments.
                 return self._dict_subclass_schema(obj)
             # probably need to take care of other subclasses here
         elif isinstance(obj, typing.TypeVar):
             return self._unsubstituted_typevar_schema(obj)
+        elif is_finalvar(obj):
+            if obj is Final:
+                return core_schema.AnySchema(type='any')
+            return self.generate_schema(get_args(obj)[0])
 
         # TODO: _std_types_schema iterates over the __mro__ looking for an expected schema.
         #   This will catch subclasses of typing.Deque, preventing us from properly supporting user-defined
         #   generic subclasses. (In principle this would also catch typing.OrderedDict, but that is currently
         #   already getting caught in the `issubclass(obj, dict):` check above.
         std_schema = self._std_types_schema(obj)
         if std_schema is not None:
@@ -461,14 +457,15 @@
         common_field = self._common_field_schema(name, field_info, decorators)
         return core_schema.typed_dict_field(
             common_field['schema'],
             required=False if not field_info.is_required() else required,
             serialization_exclude=common_field['serialization_exclude'],
             validation_alias=common_field['validation_alias'],
             serialization_alias=common_field['serialization_alias'],
+            frozen=common_field['frozen'],
             metadata=common_field['metadata'],
         )
 
     def generate_dc_field_schema(
         self,
         name: str,
         field_info: FieldInfo,
@@ -482,14 +479,15 @@
             name,
             common_field['schema'],
             init_only=field_info.init_var or None,
             kw_only=None if field_info.kw_only else False,
             serialization_exclude=common_field['serialization_exclude'],
             validation_alias=common_field['validation_alias'],
             serialization_alias=common_field['serialization_alias'],
+            frozen=common_field['frozen'],
             metadata=common_field['metadata'],
         )
 
     def _common_field_schema(self, name: str, field_info: FieldInfo, decorators: DecoratorInfos) -> _CommonField:
         assert field_info.annotation is not None, 'field_info.annotation should not be None when generating a schema'
 
         schema = self.generate_schema(field_info.annotation)
@@ -530,16 +528,17 @@
         }
         json_schema_updates = {k: v for k, v in json_schema_updates.items() if v is not None}
         json_schema_updates.update(field_info.json_schema_extra or {})
         metadata = build_metadata_dict(js_modify_function=lambda s: update_json_schema(s, json_schema_updates))
         return _common_field(
             schema,
             serialization_exclude=True if field_info.exclude else None,
-            validation_alias=field_info.alias,
-            serialization_alias=field_info.alias,
+            validation_alias=field_info.validation_alias,
+            serialization_alias=field_info.serialization_alias,
+            frozen=field_info.frozen or field_info.final,
             metadata=metadata,
         )
 
     def _union_schema(self, union_type: Any) -> core_schema.CoreSchema:
         """
         Generate schema for a Union.
         """
@@ -597,15 +596,16 @@
             typeddict_typevars_map = dict(zip(origin.__parameters__, typed_dict_cls.__args__))
             typed_dict_cls = origin
         else:
             typeddict_typevars_map = {}
 
         if not _SUPPORTS_TYPEDDICT and type(typed_dict_cls).__module__ == 'typing':
             raise PydanticUserError(
-                'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.11.'
+                'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.11.',
+                code='typed-dict-version',
             )
 
         required_keys: frozenset[str] = typed_dict_cls.__required_keys__
 
         fields: dict[str, core_schema.TypedDictField] = {}
 
         obj_ref = f'{typed_dict_cls.__module__}.{typed_dict_cls.__qualname__}:{id(typed_dict_cls)}'
@@ -908,15 +908,15 @@
         for base in obj.__mro__[:-1]:
             try:
                 encoder = SCHEMA_LOOKUP[base]
             except KeyError:
                 continue
             return encoder(self, obj)
         if dataclasses.is_dataclass(obj):
-            return self._dataclass_schema(obj)
+            return self._dataclass_schema(obj)  # type: ignore
         return None
 
     def _dataclass_schema(self, dataclass: type[StandardDataclass]) -> core_schema.CoreSchema:
         """
         Generate schema for a dataclass.
         """
         # FIXME we need a way to make sure kw_only info is propagated through to fields
@@ -926,25 +926,25 @@
 
         return dataclass_schema(
             dataclass,
             get_type_ref(dataclass),
             fields,
             # FIXME we need to get validators and serializers from the dataclasses
             DecoratorInfos(),
-            self.arbitrary_types,
+            self.config_wrapper,
             self.types_namespace,
         )
 
     def _unsubstituted_typevar_schema(self, typevar: typing.TypeVar) -> core_schema.CoreSchema:
         assert isinstance(typevar, typing.TypeVar)
 
         if typevar.__bound__:
             return self.generate_schema(typevar.__bound__)
         elif typevar.__constraints__:
-            return self._union_schema(typing.Union[typevar.__constraints__])
+            return self._union_schema(typing.Union[typevar.__constraints__])  # type: ignore
         else:
             return core_schema.AnySchema(type='any')
 
 
 _VALIDATOR_F_MATCH: Mapping[
     tuple[str, bool], Callable[[Callable[..., Any], core_schema.CoreSchema], core_schema.CoreSchema]
 ] = {
@@ -1046,14 +1046,40 @@
                 serializer.func,
                 json_return_type=serializer.info.json_return_type,
             )
         schema['serialization'] = ser_schema
     return schema
 
 
+def apply_model_validators(
+    schema: core_schema.CoreSchema, validators: Iterable[Decorator[ModelValidatorDecoratorInfo]]
+) -> core_schema.CoreSchema:
+    """
+    Apply model validators to a schema.
+    """
+    for validator in validators:
+        if validator.info.mode == 'wrap':
+            schema = core_schema.general_wrap_validator_function(
+                function=validator.func,
+                schema=schema,
+            )
+        elif validator.info.mode == 'before':
+            schema = core_schema.general_before_validator_function(
+                function=validator.func,
+                schema=schema,
+            )
+        else:
+            assert validator.info.mode == 'after'
+            schema = core_schema.general_after_validator_function(
+                function=validator.func,
+                schema=schema,
+            )
+    return schema
+
+
 def apply_annotations(
     schema: core_schema.CoreSchema, annotations: typing.Iterable[Any], definitions: dict[str, core_schema.CoreSchema]
 ) -> core_schema.CoreSchema:
     """
     Apply arguments from `Annotated` or from `FieldInfo` to a schema.
     """
     handler = CoreMetadataHandler(schema)
@@ -1085,14 +1111,43 @@
         return apply_annotations(schema, metadata, definitions)
     elif isinstance(metadata, FieldInfo):
         schema = apply_annotations(schema, metadata.metadata, definitions)
         if metadata.discriminator is not None:
             schema = _discriminated_union.apply_discriminator(schema, metadata.discriminator, definitions)
         # TODO setting a default here needs to be tested
         return wrap_default(metadata, schema)
+    elif isinstance(metadata, AfterValidator):
+        return core_schema.general_after_validator_function(
+            make_generic_validator(metadata.func, mode='after'),
+            schema=schema,
+        )
+    elif isinstance(metadata, BeforeValidator):
+        return core_schema.general_before_validator_function(
+            make_generic_validator(metadata.func, mode='before'),
+            schema=schema,
+        )
+    elif isinstance(metadata, WrapValidator):
+        return core_schema.general_wrap_validator_function(
+            make_generic_validator(metadata.func, mode='wrap'),
+            schema=schema,
+        )
+    elif isinstance(metadata, PlainSerializer):
+        schema['serialization'] = core_schema.general_plain_serializer_function_ser_schema(
+            function=make_generic_serializer(metadata.func, mode='plain', type='general'),
+            json_return_type=metadata.json_return_type,
+            when_used=metadata.when_used,
+        )
+        return schema
+    elif isinstance(metadata, WrapSerializer):
+        schema['serialization'] = core_schema.general_wrap_serializer_function_ser_schema(
+            function=make_generic_serializer(metadata.func, mode='wrap', type='general'),
+            json_return_type=metadata.json_return_type,
+            when_used=metadata.when_used,
+        )
+        return schema
 
     if isinstance(metadata, PydanticGeneralMetadata):
         metadata_dict = metadata.__dict__
     elif isinstance(metadata, (BaseMetadata, PydanticMetadata)):
         metadata_dict = dataclasses.asdict(metadata)  # type: ignore[call-overload]
     elif isinstance(metadata, type) and issubclass(metadata, PydanticMetadata):
         # also support PydanticMetadata classes being used without initialisation,
@@ -1168,25 +1223,28 @@
 
 
 class _CommonField(TypedDict):
     schema: core_schema.CoreSchema
     validation_alias: str | list[str | int] | list[list[str | int]] | None
     serialization_alias: str | None
     serialization_exclude: bool | None
+    frozen: bool | None
     metadata: Any
 
 
 def _common_field(
     schema: core_schema.CoreSchema,
     *,
     validation_alias: str | list[str | int] | list[list[str | int]] | None = None,
     serialization_alias: str | None = None,
     serialization_exclude: bool | None = None,
+    frozen: bool | None = None,
     metadata: Any = None,
 ) -> _CommonField:
     return {
         'schema': schema,
         'validation_alias': validation_alias,
         'serialization_alias': serialization_alias,
         'serialization_exclude': serialization_exclude,
+        'frozen': frozen,
         'metadata': metadata,
     }
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_generics.py` & `pydantic-2.0a2/pydantic/_internal/_generics.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 if sys.version_info >= (3, 9):  # Typing for weak dictionaries available at 3.9
     GenericTypesCache = WeakValueDictionary[GenericTypesCacheKey, 'type[BaseModel]']
 else:
     GenericTypesCache = WeakValueDictionary
 
 if TYPE_CHECKING:
 
-    class DeepChainMap(ChainMap[KT, VT]):
+    class DeepChainMap(ChainMap[KT, VT]):  # type: ignore
         ...
 
 else:
 
     class DeepChainMap(ChainMap):
         """
         Variant of ChainMap that allows direct updates to inner scopes
@@ -109,14 +109,20 @@
 # Despite the fact that LimitedDict _seems_ no longer necessary, I'm very nervous to actually remove it
 # and discover later on that we need to re-add all this infrastructure...
 # _GENERIC_TYPES_CACHE = DeepChainMap(GenericTypesCache(), LimitedDict())
 
 _GENERIC_TYPES_CACHE = GenericTypesCache()
 
 
+class PydanticGenericMetadata(typing_extensions.TypedDict):
+    origin: type[BaseModel] | None  # analogous to typing._GenericAlias.__origin__
+    args: tuple[Any, ...]  # analogous to typing._GenericAlias.__args__
+    parameters: tuple[type[Any], ...]  # analogous to typing.Generic.__parameters__
+
+
 def create_generic_submodel(
     model_name: str, origin: type[BaseModel], args: tuple[Any, ...], params: tuple[Any, ...]
 ) -> type[BaseModel]:
     """
     Dynamically create a submodel of a provided (generic) BaseModel.
 
     This is used when producing concrete parametrizations of generic models. This function
@@ -130,17 +136,19 @@
     bases = (origin,)
     meta, ns, kwds = prepare_class(model_name, bases)
     namespace.update(ns)
     created_model = meta(
         model_name,
         bases,
         namespace,
-        __pydantic_generic_origin__=origin,
-        __pydantic_generic_args__=args,
-        __pydantic_generic_parameters__=params,
+        __pydantic_generic_metadata__={
+            'origin': origin,
+            'args': args,
+            'parameters': params,
+        },
         __pydantic_reset_parent_namespace__=False,
         **kwds,
     )
 
     model_module, called_globally = _get_caller_frame_info(depth=3)
     if called_globally:  # create global reference and therefore allow pickling
         object_by_reference = None
@@ -178,38 +186,46 @@
 
     This is inspired as an alternative to directly accessing the `__parameters__` attribute of a GenericAlias,
     since __parameters__ of (nested) generic BaseModel subclasses won't show up in that list.
     """
     if isinstance(v, TypeVar):
         yield v
     elif is_basemodel(v):
-        yield from v.__pydantic_generic_parameters__ or ()
+        yield from v.__pydantic_generic_metadata__['parameters']
     elif isinstance(v, (DictValues, list)):
         for var in v:
             yield from iter_contained_typevars(var)
     else:
         args = get_args(v)
         for arg in args:
             yield from iter_contained_typevars(arg)
 
 
 def get_args(v: Any) -> Any:
-    pydantic_generic_args = getattr(v, '__pydantic_generic_args__', None)
-    if pydantic_generic_args:
-        return pydantic_generic_args
+    pydantic_generic_metadata: PydanticGenericMetadata | None = getattr(v, '__pydantic_generic_metadata__', None)
+    if pydantic_generic_metadata:
+        return pydantic_generic_metadata.get('args')
     return typing_extensions.get_args(v)
 
 
 def get_origin(v: Any) -> Any:
-    pydantic_generic_origin = getattr(v, '__pydantic_generic_origin__', None)
-    if pydantic_generic_origin:
-        return pydantic_generic_origin
+    pydantic_generic_metadata: PydanticGenericMetadata | None = getattr(v, '__pydantic_generic_metadata__', None)
+    if pydantic_generic_metadata:
+        return pydantic_generic_metadata.get('origin')
     return typing_extensions.get_origin(v)
 
 
+def get_typevars_map(origin: type[Any] | None, args: tuple[type[Any], ...]) -> dict[TypeVarType, type[Any]]:
+    """
+    Builds the mapping of typevars to argument values in a manner consistent with how the `typing` library,
+    but correctly handles the case where the origin is a generic BaseModel subclass.
+    """
+    return dict(zip(iter_contained_typevars(origin), args))
+
+
 def replace_types(type_: Any, type_map: Mapping[Any, Any] | None) -> Any:
     """Return type with all occurrences of `type_map` keys recursively replaced with their values.
 
     :param type_: Any type, class or generic alias
     :param type_map: Mapping from `TypeVar` instance to concrete types.
     :return: New type representing the basic structure of `type_` with all
         `typevar_map` keys recursively replaced.
@@ -256,15 +272,15 @@
             return _UnionGenericAlias(origin_type, resolved_type_args)
         return origin_type[resolved_type_args]
 
     # We handle pydantic generic models separately as they don't have the same
     # semantics as "typing" classes or generic aliases
 
     if not origin_type and is_basemodel(type_):
-        parameters = type_.__pydantic_generic_parameters__
+        parameters = type_.__pydantic_generic_metadata__['parameters']
         if not parameters:
             return type_
         resolved_type_args = tuple(replace_types(t, type_map) for t in parameters)
         if all_identical(parameters, resolved_type_args):
             return type_
         return type_[resolved_type_args]  # type: ignore[index]
 
@@ -283,15 +299,15 @@
     # If all else fails, we try to resolve the type directly and otherwise just
     # return the input with no modifications.
     return type_map.get(type_, type_)
 
 
 def check_parameters_count(cls: type[BaseModel], parameters: tuple[Any, ...]) -> None:
     actual = len(parameters)
-    expected = len(cls.__pydantic_generic_parameters__ or ())
+    expected = len(cls.__pydantic_generic_metadata__['parameters'])
     if actual != expected:
         description = 'many' if actual > expected else 'few'
         raise TypeError(f'Too {description} parameters for {cls}; actual {actual}, expected {expected}')
 
 
 _generic_recursion_cache: ContextVar[set[str] | None] = ContextVar('_generic_recursion_cache', default=None)
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_model_construction.py` & `pydantic-2.0a2/pydantic/_internal/_model_construction.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 
 import typing
 from types import FunctionType
 from typing import Any, Callable
 
 from pydantic_core import SchemaSerializer, SchemaValidator
 
-from ..errors import PydanticUndefinedAnnotation, PydanticUserError
+from ..errors import PydanticErrorCodes, PydanticUndefinedAnnotation, PydanticUserError
 from ..fields import FieldInfo, ModelPrivateAttr, PrivateAttr
+from ._config import ConfigWrapper
 from ._decorators import PydanticDecoratorMarker
 from ._fields import Undefined, collect_fields
-from ._generate_schema import GenerateSchema, generate_config
+from ._generate_schema import GenerateSchema
+from ._generics import get_typevars_map
 from ._typing_extra import add_module_globals, is_classvar
 from ._utils import ClassAttribute, is_valid_identifier
 
 if typing.TYPE_CHECKING:
     from inspect import Signature
 
     from ..config import ConfigDict
@@ -25,24 +27,24 @@
 
 __all__ = 'object_setattr', 'init_private_attributes', 'inspect_namespace', 'MockValidator'
 
 IGNORED_TYPES: tuple[Any, ...] = (FunctionType, property, type, classmethod, staticmethod, PydanticDecoratorMarker)
 object_setattr = object.__setattr__
 
 
-def init_private_attributes(self_: Any, _context: Any) -> None:
+def init_private_attributes(self: BaseModel, __context: Any) -> None:
     """
-    This method is bound to model classes to initialise private attributes.
+    This function is meant to behave like a BaseModel method to initialise private attributes.
 
     It takes context as an argument since that's what pydantic-core passes when calling it.
     """
-    for name, private_attr in self_.__private_attributes__.items():
+    for name, private_attr in self.__private_attributes__.items():
         default = private_attr.get_default()
         if default is not Undefined:
-            object_setattr(self_, name, default)
+            object_setattr(self, name, default)
 
 
 def inspect_namespace(  # noqa C901
     namespace: dict[str, Any],
     ignored_types: tuple[type[Any], ...],
     base_class_vars: set[str],
     base_class_fields: set[str],
@@ -96,22 +98,26 @@
         elif var_name in base_class_vars:
             continue
         elif var_name not in raw_annotations:
             if var_name in base_class_fields:
                 raise PydanticUserError(
                     f'Field {var_name!r} defined on a base class was overridden by a non-annotated attribute. '
                     f'All field definitions, including overrides, require a type annotation.',
+                    code='model-field-overridden',
                 )
             elif isinstance(value, FieldInfo):
-                raise PydanticUserError(f'Field {var_name!r} requires a type annotation')
+                raise PydanticUserError(
+                    f'Field {var_name!r} requires a type annotation', code='model-field-missing-annotation'
+                )
             else:
                 raise PydanticUserError(
-                    f'A non-annotated attribute was detected: `{var_name} = {value!r}`. All model fields require a '
-                    f'type annotation; if {var_name!r} is not meant to be a field, you may be able to resolve this '
-                    f'error by annotating it as a ClassVar or updating model_config["ignored_types"].',
+                    f"A non-annotated attribute was detected: `{var_name} = {value!r}`. All model fields require a "
+                    f"type annotation; if `{var_name}` is not meant to be a field, you may be able to resolve this "
+                    f"error by annotating it as a `ClassVar` or updating `model_config['ignored_types']`.",
+                    code='model-field-missing-annotation',
                 )
 
     for ann_name, ann_type in raw_annotations.items():
         if (
             single_underscore(ann_name)
             and ann_name not in private_attributes
             and ann_name not in ignored_names
@@ -143,73 +149,80 @@
     cls.model_fields = fields
     cls.__class_vars__.update(class_vars)
 
 
 def complete_model_class(
     cls: type[BaseModel],
     cls_name: str,
+    config_wrapper: ConfigWrapper,
     types_namespace: dict[str, Any] | None,
     *,
     raise_errors: bool = True,
 ) -> bool:
     """
     Finish building a model class.
 
     Returns `True` if the model is successfully completed, else `False`.
 
     This logic must be called after class has been created since validation functions must be bound
     and `get_type_hints` requires a class object.
     """
+    generic_metadata = cls.__pydantic_generic_metadata__
+    typevars_map = get_typevars_map(generic_metadata['origin'], generic_metadata['args'])
     gen_schema = GenerateSchema(
-        cls.model_config['arbitrary_types_allowed'], types_namespace, cls.__pydantic_generic_typevars_map__
+        config_wrapper,
+        types_namespace,
+        typevars_map,
     )
     try:
         schema = gen_schema.generate_schema(cls)
     except PydanticUndefinedAnnotation as e:
         if raise_errors:
             raise
-        if cls.model_config['undefined_types_warning']:
+        if config_wrapper.undefined_types_warning:
             config_warning_string = (
                 f'`{cls_name}` has an undefined annotation: `{e.name}`. '
                 f'It may be possible to resolve this by setting '
                 f'undefined_types_warning=False in the config for `{cls_name}`.'
             )
             # FIXME UserWarning should not be raised here, but rather warned!
             raise UserWarning(config_warning_string)
         usage_warning_string = (
             f'`{cls_name}` is not fully defined; you should define `{e.name}`, then call `{cls_name}.model_rebuild()` '
             f'before the first `{cls_name}` instance is created.'
         )
-        cls.__pydantic_validator__ = MockValidator(usage_warning_string)  # type: ignore[assignment]
+        cls.__pydantic_validator__ = MockValidator(  # type: ignore[assignment]
+            usage_warning_string, code='model-not-fully-defined'
+        )
         return False
 
-    core_config = generate_config(cls.model_config, cls)
+    core_config = config_wrapper.core_config(cls)
 
     # debug(schema)
     cls.__pydantic_core_schema__ = schema
     cls.__pydantic_validator__ = SchemaValidator(schema, core_config)
     cls.__pydantic_serializer__ = SchemaSerializer(schema, core_config)
     cls.__pydantic_model_complete__ = True
 
     # set __signature__ attr only for model class, but not for its instances
     cls.__signature__ = ClassAttribute(
-        '__signature__', generate_model_signature(cls.__init__, cls.model_fields, cls.model_config)
+        '__signature__', generate_model_signature(cls.__init__, cls.model_fields, config_wrapper)
     )
     return True
 
 
-def generate_model_signature(init: Callable[..., None], fields: dict[str, FieldInfo], config: ConfigDict) -> Signature:
+def generate_model_signature(
+    init: Callable[..., None], fields: dict[str, FieldInfo], config_wrapper: ConfigWrapper
+) -> Signature:
     """
     Generate signature for model based on its fields
     """
     from inspect import Parameter, Signature, signature
     from itertools import islice
 
-    from ..config import Extra
-
     present_params = signature(init).parameters.values()
     merged_params: dict[str, Parameter] = {}
     var_kw = None
     use_var_kw = False
 
     for param in islice(present_params, 1, None):  # skip self arg
         # inspect does "clever" things to show annotations as strings because we have
@@ -218,17 +231,21 @@
             param = param.replace(annotation=Any)
         if param.kind is param.VAR_KEYWORD:
             var_kw = param
             continue
         merged_params[param.name] = param
 
     if var_kw:  # if custom init has no var_kw, fields which are not declared in it cannot be passed through
-        allow_names = config['populate_by_name']
+        allow_names = config_wrapper.populate_by_name
         for field_name, field in fields.items():
-            param_name = field.alias or field_name
+            # when alias is a str it should be used for signature generation
+            if isinstance(field.alias, str):
+                param_name = field.alias
+            else:
+                param_name = field_name
             if field_name in merged_params or param_name in merged_params:
                 continue
             elif not is_valid_identifier(param_name):
                 if allow_names and is_valid_identifier(field_name):
                     param_name = field_name
                 else:
                     use_var_kw = True
@@ -236,15 +253,15 @@
 
             # TODO: replace annotation with actual expected types once #1055 solved
             kwargs = {} if field.is_required() else {'default': field.get_default(call_default_factory=False)}
             merged_params[param_name] = Parameter(
                 param_name, Parameter.KEYWORD_ONLY, annotation=field.rebuild_annotation(), **kwargs
             )
 
-    if config['extra'] is Extra.allow:
+    if config_wrapper.extra == 'allow':
         use_var_kw = True
 
     if var_kw and use_var_kw:
         # Make sure the parameter for extra kwargs
         # does not have the same name as a field
         default_model_signature = [
             ('__pydantic_self__', Parameter.POSITIONAL_OR_KEYWORD),
@@ -266,31 +283,34 @@
 
 
 class MockValidator:
     """
     Mocker for `pydantic_core.SchemaValidator` which just raises an error when one of its methods is accessed.
     """
 
-    __slots__ = ('_error_message',)
+    __slots__ = '_error_message', '_code'
 
-    def __init__(self, error_message: str) -> None:
+    def __init__(self, error_message: str, *, code: PydanticErrorCodes) -> None:
         self._error_message = error_message
+        self._code: PydanticErrorCodes = code
 
     def __getattr__(self, item: str) -> None:
         __tracebackhide__ = True
         # raise an AttributeError if `item` doesn't exist
         getattr(SchemaValidator, item)
-        raise PydanticUserError(self._error_message)
+        raise PydanticUserError(self._error_message, code=self._code)
 
 
 def apply_alias_generator(config: ConfigDict, fields: dict[str, FieldInfo]) -> None:
-    alias_generator = config['alias_generator']
+    alias_generator = config.get('alias_generator')
     if alias_generator is None:
         return
 
     for name, field_info in fields.items():
         if field_info.alias_priority is None or field_info.alias_priority <= 1:
             alias = alias_generator(name)
             if not isinstance(alias, str):
                 raise TypeError(f'alias_generator {alias_generator} must return str, not {alias.__class__}')
             field_info.alias = alias
+            field_info.validation_alias = alias
+            field_info.serialization_alias = alias
             field_info.alias_priority = 1
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_repr.py` & `pydantic-2.0a2/pydantic/_internal/_repr.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 from typing import Any
 
 import typing_extensions
 
 from . import _typing_extra
 
 if typing.TYPE_CHECKING:
-    ReprArgs = typing.Iterable[tuple[str | None, Any]]
-    RichReprResult = typing.Iterable[Any | tuple[Any] | tuple[str, Any] | tuple[str, Any, Any]]
+    ReprArgs: typing_extensions.TypeAlias = 'typing.Iterable[tuple[str | None, Any]]'
+    RichReprResult: typing_extensions.TypeAlias = (
+        'typing.Iterable[Any | tuple[Any] | tuple[str, Any] | tuple[str, Any, Any]]'
+    )
 
 
 class PlainRepr(str):
     """
     String class where repr doesn't include quotes. Useful with Representation when you want to return a string
     representation of something that is valid (or pseudo-valid) python.
     """
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_std_types_schema.py` & `pydantic-2.0a2/pydantic/_internal/_std_types_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/pydantic/_internal/_typing_extra.py` & `pydantic-2.0a2/pydantic/_internal/_typing_extra.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
 def is_classvar(ann_type: type[Any]) -> bool:
     if _check_classvar(ann_type) or _check_classvar(get_origin(ann_type)):
         return True
 
     # this is an ugly workaround for class vars that contain forward references and are therefore themselves
     # forward references, see #3679
-    if ann_type.__class__ == typing.ForwardRef and ann_type.__forward_arg__.startswith('ClassVar['):
+    if ann_type.__class__ == typing.ForwardRef and ann_type.__forward_arg__.startswith('ClassVar['):  # type: ignore
         return True
 
     return False
 
 
 def _check_finalvar(v: type[Any] | None) -> bool:
     """
@@ -196,15 +196,15 @@
     """
     if v is None:
         return False
 
     return v.__class__ == Final.__class__ and (sys.version_info < (3, 8) or getattr(v, '_name', None) == 'Final')
 
 
-def is_finalvar(ann_type: type[Any]) -> bool:
+def is_finalvar(ann_type: Any) -> bool:
     return _check_finalvar(ann_type) or _check_finalvar(get_origin(ann_type))
 
 
 def parent_frame_namespace(*, parent_depth: int = 2) -> dict[str, Any] | None:
     """
     We allow use of items in parent namespace to get around the issue with `get_type_hints` only looking in the
     global module namespace. See https://github.com/pydantic/pydantic/issues/2678#issuecomment-1008139014 -> Scope
@@ -256,70 +256,73 @@
         ann = base.__dict__.get('__annotations__')
         localns = dict(vars(base))
         if ann is not None and ann is not GetSetDescriptorType:
             for name, value in ann.items():
                 if value is None:
                     value = NoneType
                 elif isinstance(value, str):
-                    value = ForwardRef(value, is_argument=False, is_class=True)
+                    value = _make_forward_ref(value, is_argument=False, is_class=True)  # type: ignore
 
                 try:
                     hints[name] = typing._eval_type(value, globalns, localns)  # type: ignore[attr-defined]
                 except NameError:
                     # the point of this function is to be tolerant to this case
                     hints[name] = value
     return hints
 
 
 if sys.version_info < (3, 9):
 
-    def ForwardRefWrapper(arg: Any, is_argument: bool = True, *, is_class: bool = False) -> typing.ForwardRef:
+    def _make_forward_ref(
+        arg: Any,
+        is_argument: bool = True,
+        *,
+        is_class: bool = False,
+    ) -> typing.ForwardRef:
         """
         Wrapper for ForwardRef that accounts for the `is_class` argument missing in older versions.
         The `module` argument is omitted as it breaks <3.9 and isn't used in the calls below.
 
         See https://github.com/python/cpython/pull/28560 for some background
 
         Implemented as EAFP with memory.
         """
-        global fr_has_is_class
-
-        if not fr_has_is_class:
-            return typing.ForwardRef(arg, is_argument)
-
+        global _make_forward_ref
         try:
-            return typing.ForwardRef(arg, is_argument, is_class=is_class)
+            res = typing.ForwardRef(arg, is_argument, is_class=is_class)  # type: ignore
+            _make_forward_ref = typing.ForwardRef  # type: ignore
+            return res
         except TypeError:
-            fr_has_is_class = False
             return typing.ForwardRef(arg, is_argument)
 
-    ForwardRef = ForwardRefWrapper  # noqa F811
+else:
+    _make_forward_ref = typing.ForwardRef
+
 
 if sys.version_info >= (3, 10):
     get_type_hints = typing.get_type_hints
 
 else:
     """
     For older versions of python, we have a custom implementation of `get_type_hints` which is a close as possible to
     the implementation in CPython 3.10.8.
     """
-    fr_has_is_class = True
 
     @typing.no_type_check
     def get_type_hints(  # noqa: C901
         obj: Any,
         globalns: dict[str, Any] | None = None,
         localns: dict[str, Any] | None = None,
         include_extras: bool = False,
     ) -> dict[str, Any]:  # pragma: no cover
         """
         Taken verbatim from python 3.10.8 unchanged, except:
         * type annotations of the function definition above.
         * prefixing `typing.` where appropriate
-        * Use `ForwardRefWrapper` instead of `typing.ForwardRef`
+        * Use `_make_forward_ref` instead of `typing.ForwardRef` to handle the `is_class` argument
 
         https://github.com/python/cpython/blob/aaaf5174241496afca7ce4d4584570190ff972fe/Lib/typing.py#L1773-L1875
 
         DO NOT CHANGE THIS METHOD UNLESS ABSOLUTELY NECESSARY.
         ======================================================
 
         Return type hints for an object.
@@ -376,19 +379,21 @@
                     # *base_globals* first rather than *base_locals*.
                     # This only affects ForwardRefs.
                     base_globals, base_locals = base_locals, base_globals
                 for name, value in ann.items():
                     if value is None:
                         value = type(None)
                     if isinstance(value, str):
-                        value = ForwardRef(value, is_argument=False, is_class=True)
+                        value = _make_forward_ref(value, is_argument=False, is_class=True)
 
-                    value = typing._eval_type(value, base_globals, base_locals)
+                    value = typing._eval_type(value, base_globals, base_locals)  # type: ignore
                     hints[name] = value
-            return hints if include_extras else {k: typing._strip_annotations(t) for k, t in hints.items()}
+            return (
+                hints if include_extras else {k: typing._strip_annotations(t) for k, t in hints.items()}  # type: ignore
+            )
 
         if globalns is None:
             if isinstance(obj, types.ModuleType):
                 globalns = obj.__dict__
             else:
                 nsobj = obj
                 # Find globalns for the unwrapped object.
@@ -398,37 +403,37 @@
             if localns is None:
                 localns = globalns
         elif localns is None:
             localns = globalns
         hints = getattr(obj, '__annotations__', None)
         if hints is None:
             # Return empty annotations for something that _could_ have them.
-            if isinstance(obj, typing._allowed_types):
+            if isinstance(obj, typing._allowed_types):  # type: ignore
                 return {}
             else:
                 raise TypeError('{!r} is not a module, class, method, ' 'or function.'.format(obj))
-        defaults = typing._get_defaults(obj)
+        defaults = typing._get_defaults(obj)  # type: ignore
         hints = dict(hints)
         for name, value in hints.items():
             if value is None:
                 value = type(None)
             if isinstance(value, str):
                 # class-level forward refs were handled above, this must be either
                 # a module-level annotation or a function argument annotation
 
-                value = ForwardRef(
+                value = _make_forward_ref(
                     value,
                     is_argument=not isinstance(obj, types.ModuleType),
                     is_class=False,
                 )
-            value = typing._eval_type(value, globalns, localns)
+            value = typing._eval_type(value, globalns, localns)  # type: ignore
             if name in defaults and defaults[name] is None:
                 value = typing.Optional[value]
             hints[name] = value
-        return hints if include_extras else {k: typing._strip_annotations(t) for k, t in hints.items()}
+        return hints if include_extras else {k: typing._strip_annotations(t) for k, t in hints.items()}  # type: ignore
 
 
 if sys.version_info < (3, 9):
 
     def evaluate_fwd_ref(
         ref: ForwardRef, globalns: dict[str, Any] | None = None, localns: dict[str, Any] | None = None
     ) -> Any:
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_utils.py` & `pydantic-2.0a2/pydantic/_internal/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 import weakref
 from collections import OrderedDict, defaultdict, deque
 from copy import deepcopy
 from itertools import zip_longest
 from types import BuiltinFunctionType, CodeType, FunctionType, GeneratorType, LambdaType, ModuleType
 from typing import Any, TypeVar
 
-from typing_extensions import TypeGuard
+from typing_extensions import TypeAlias, TypeGuard
 
 from . import _repr, _typing_extra
 
 if typing.TYPE_CHECKING:
-    MappingIntStrAny = typing.Mapping[int | str, Any]
-    AbstractSetIntStr = typing.AbstractSet[int | str]
+    MappingIntStrAny: TypeAlias = 'typing.Mapping[int, Any] | typing.Mapping[str, Any]'
+    AbstractSetIntStr: TypeAlias = 'typing.AbstractSet[int] | typing.AbstractSet[str]'
     from ..main import BaseModel
 
 __all__ = (
     'sequence_like',
     'lenient_isinstance',
     'lenient_issubclass',
     'is_valid_identifier',
@@ -130,15 +130,15 @@
             if k in updated_mapping and isinstance(updated_mapping[k], dict) and isinstance(v, dict):
                 updated_mapping[k] = deep_update(updated_mapping[k], v)
             else:
                 updated_mapping[k] = v
     return updated_mapping
 
 
-def dict_not_none(__pos: dict[str, Any] = None, **kwargs: Any) -> dict[str, Any]:
+def dict_not_none(__pos: dict[str, Any] | None = None, **kwargs: Any) -> dict[str, Any]:
     return {k: v for k, v in (__pos or kwargs).items() if v is not None}
 
 
 def update_not_none(mapping: dict[Any, Any], **update: Any) -> None:
     mapping.update({k: v for k, v in update.items() if v is not None})
 
 
@@ -193,17 +193,17 @@
 
     __slots__ = ('_items', '_type')
 
     def __init__(self, value: Any, items: AbstractSetIntStr | MappingIntStrAny) -> None:
         items = self._coerce_items(items)
 
         if isinstance(value, (list, tuple)):
-            items = self._normalize_indexes(items, len(value))
+            items = self._normalize_indexes(items, len(value))  # type: ignore
 
-        self._items: MappingIntStrAny = items
+        self._items: MappingIntStrAny = items  # type: ignore
 
     def is_excluded(self, item: Any) -> bool:
         """
         Check if item is fully excluded.
 
         :param item: key or index of a value
         """
@@ -219,15 +219,15 @@
 
     def for_element(self, e: int | str) -> AbstractSetIntStr | MappingIntStrAny | None:
         """
         :param e: key or index of element on value
         :return: raw values for element if self._items is dict and contain needed element
         """
 
-        item = self._items.get(e)
+        item = self._items.get(e)  # type: ignore
         return item if not self.is_true(item) else None
 
     def _normalize_indexes(self, items: MappingIntStrAny, v_length: int) -> dict[int | str, Any]:
         """
         :param items: dict or set of indexes which will be normalized
         :param v_length: length of sequence indexes of which will be
 
@@ -264,26 +264,26 @@
             if not self.is_true(normalized_item):
                 normalized_items[i] = self.merge(all_items, normalized_item)
         return normalized_items
 
     @classmethod
     def merge(cls, base: Any, override: Any, intersect: bool = False) -> Any:
         """
-        Merge a ``base`` item with an ``override`` item.
+        Merge a `base` item with an `override` item.
 
-        Both ``base`` and ``override`` are converted to dictionaries if possible.
+        Both `base` and `override` are converted to dictionaries if possible.
         Sets are converted to dictionaries with the sets entries as keys and
         Ellipsis as values.
 
-        Each key-value pair existing in ``base`` is merged with ``override``,
+        Each key-value pair existing in `base` is merged with `override`,
         while the rest of the key-value pairs are updated recursively with this function.
 
-        Merging takes place based on the "union" of keys if ``intersect`` is
-        set to ``False`` (default) and on the intersection of keys if
-        ``intersect`` is set to ``True``.
+        Merging takes place based on the "union" of keys if `intersect` is
+        set to `False` (default) and on the intersection of keys if
+        `intersect` is set to `True`.
         """
         override = cls._coerce_value(override)
         base = cls._coerce_value(base)
         if override is None:
             return base
         if cls.is_true(base) or base is None:
             return override
@@ -304,20 +304,20 @@
 
         return merged
 
     @staticmethod
     def _coerce_items(items: AbstractSetIntStr | MappingIntStrAny) -> MappingIntStrAny:
         if isinstance(items, typing.Mapping):
             pass
-        elif isinstance(items, typing.AbstractSet):
-            items = dict.fromkeys(items, ...)
+        elif isinstance(items, typing.AbstractSet):  # type: ignore
+            items = dict.fromkeys(items, ...)  # type: ignore
         else:
             class_name = getattr(items, '__class__', '???')
             raise TypeError(f'Unexpected type of exclude value {class_name}')
-        return items
+        return items  # type: ignore
 
     @classmethod
     def _coerce_value(cls, value: Any) -> Any:
         if value is None or cls.is_true(value):
             return value
         return cls._coerce_items(value)
```

### Comparing `pydantic-2.0a1/pydantic/_internal/_validators.py` & `pydantic-2.0a2/pydantic/_internal/_validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -227,22 +227,30 @@
             if mod != 0:
                 raise PydanticCustomError(
                     'decimal_multiple_of',
                     'Input should be a multiple of {multiple_of}',
                     {'multiple_of': self.multiple_of},
                 )
 
-        if self.gt is not None and not value > self.gt:
+        # these type checks are here to handle the following error:
+        # Operator ">" not supported for types "(
+        #   <subclass of int and Decimal>
+        #   | <subclass of float and Decimal>
+        #   | <subclass of str and Decimal>
+        #   | Decimal" and "int
+        #   | Decimal"
+        # )
+        if self.gt is not None and not value > self.gt:  # type: ignore
             raise PydanticKnownError('greater_than', {'gt': self.gt})
-        elif self.ge is not None and not value >= self.ge:
+        elif self.ge is not None and not value >= self.ge:  # type: ignore
             raise PydanticKnownError('greater_than_equal', {'ge': self.ge})
 
-        if self.lt is not None and not value < self.lt:
+        if self.lt is not None and not value < self.lt:  # type: ignore
             raise PydanticKnownError('less_than', {'lt': self.lt})
-        if self.le is not None and not value <= self.le:
+        if self.le is not None and not value <= self.le:  # type: ignore
             raise PydanticKnownError('less_than_equal', {'le': self.le})
 
         return value
 
     def __repr__(self) -> str:
         slots = [(k, getattr(self, k)) for k in self.__slots__]
         s = ', '.join(f'{k}={v!r}' for k, v in slots if v is not None)
@@ -269,26 +277,26 @@
         return Path(__input_value)
     except TypeError:
         raise PydanticCustomError('path_type', 'Input is not a valid path')
 
 
 def pattern_either_validator(__input_value: Any, _: core_schema.ValidationInfo) -> typing.Pattern[Any]:
     if isinstance(__input_value, typing.Pattern):
-        return __input_value
+        return __input_value  # type: ignore
     elif isinstance(__input_value, (str, bytes)):
         # todo strict mode
-        return compile_pattern(__input_value)
+        return compile_pattern(__input_value)  # type: ignore
     else:
         raise PydanticCustomError('pattern_type', 'Input should be a valid pattern')
 
 
 def pattern_str_validator(__input_value: Any, _: core_schema.ValidationInfo) -> typing.Pattern[str]:
     if isinstance(__input_value, typing.Pattern):
-        if isinstance(__input_value.pattern, str):
-            return __input_value
+        if isinstance(__input_value.pattern, str):  # type: ignore
+            return __input_value  # type: ignore
         else:
             raise PydanticCustomError('pattern_str_type', 'Input should be a string pattern')
     elif isinstance(__input_value, str):
         return compile_pattern(__input_value)
     elif isinstance(__input_value, bytes):
         raise PydanticCustomError('pattern_str_type', 'Input should be a string pattern')
     else:
@@ -363,15 +371,15 @@
         return IPv6Address(__input_value)
     except ValueError:
         raise PydanticCustomError('ip_v6_address', 'Input is not a valid IPv6 address')
 
 
 def ip_v4_network_validator(__input_value: Any, _: core_schema.ValidationInfo) -> IPv4Network:
     """
-    Assume IPv4Network initialised with a default ``strict`` argument
+    Assume IPv4Network initialised with a default `strict` argument
 
     See more:
     https://docs.python.org/library/ipaddress.html#ipaddress.IPv4Network
     """
     if isinstance(__input_value, IPv4Network):
         return __input_value
 
@@ -379,15 +387,15 @@
         return IPv4Network(__input_value)
     except ValueError:
         raise PydanticCustomError('ip_v4_network', 'Input is not a valid IPv4 network')
 
 
 def ip_v6_network_validator(__input_value: Any, _: core_schema.ValidationInfo) -> IPv6Network:
     """
-    Assume IPv6Network initialised with a default ``strict`` argument
+    Assume IPv6Network initialised with a default `strict` argument
 
     See more:
     https://docs.python.org/library/ipaddress.html#ipaddress.IPv6Network
     """
     if isinstance(__input_value, IPv6Network):
         return __input_value
```

### Comparing `pydantic-2.0a1/pydantic/deprecated/copy_internals.py` & `pydantic-2.0a2/pydantic/deprecated/copy_internals.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations as _annotations
 
 import typing
 from copy import deepcopy
 from enum import Enum
-from typing import Any
+from typing import Any, Tuple
+
+import typing_extensions
 
 from .._internal import (
     _model_construction,
     _typing_extra,
     _utils,
 )
 from .._internal._fields import Undefined
 
 if typing.TYPE_CHECKING:
     from pydantic import BaseModel
     from pydantic._internal._utils import AbstractSetIntStr, MappingIntStrAny
 
-    AnyClassMethod = classmethod[Any]
-    TupleGenerator = typing.Generator[tuple[str, Any], None, None]
+    AnyClassMethod = classmethod[Any, Any, Any]
+    TupleGenerator = typing.Generator[Tuple[str, Any], None, None]
     Model = typing.TypeVar('Model', bound='BaseModel')
     # should be `set[int] | set[str] | dict[int, IncEx] | dict[str, IncEx] | None`, but mypy can't cope
-    IncEx = set[int] | set[str] | dict[int, Any] | dict[str, Any] | None
+    IncEx: typing_extensions.TypeAlias = 'set[int] | set[str] | dict[int, Any] | dict[str, Any] | None'
 
 _object_setattr = _model_construction.object_setattr
 
 
 def _iter(
     self: BaseModel,
     to_dict: bool = False,
@@ -93,15 +95,15 @@
     if deep:
         # chances of having empty dict here are quite low for using smart_deepcopy
         values = deepcopy(values)
 
     cls = self.__class__
     m = cls.__new__(cls)
     _object_setattr(m, '__dict__', values)
-    _object_setattr(m, '__fields_set__', fields_set)
+    _object_setattr(m, '__pydantic_fields_set__', fields_set)
     for name in self.__private_attributes__:
         value = getattr(self, name, Undefined)
         if value is not Undefined:
             if deep:
                 value = deepcopy(value)
             _object_setattr(m, name, value)
 
@@ -124,16 +126,16 @@
 
     if isinstance(v, BaseModel):
         if to_dict:
             return v.model_dump(
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
-                include=include,
-                exclude=exclude,
+                include=include,  # type: ignore
+                exclude=exclude,  # type: ignore
                 exclude_none=exclude_none,
             )
         else:
             return v.copy(include=include, exclude=exclude)
 
     value_exclude = _utils.ValueItems(v, exclude) if exclude else None
     value_include = _utils.ValueItems(v, include) if include else None
@@ -191,15 +193,15 @@
     update: typing.Dict[str, Any] | None = None,  # noqa UP006
 ) -> typing.AbstractSet[str] | None:
     if include is None and exclude is None and exclude_unset is False:
         return None
 
     keys: typing.AbstractSet[str]
     if exclude_unset:
-        keys = self.__fields_set__.copy()
+        keys = self.__pydantic_fields_set__.copy()
     else:
         keys = self.__dict__.keys()
 
     if include is not None:
         keys &= include.keys()
 
     if update:
```

### Comparing `pydantic-2.0a1/pydantic/deprecated/json.py` & `pydantic-2.0a2/pydantic/deprecated/json.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/pydantic/deprecated/parse.py` & `pydantic-2.0a2/pydantic/deprecated/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     json = 'json'
     pickle = 'pickle'
 
 
 def load_str_bytes(
     b: str | bytes,
     *,
-    content_type: str = None,
+    content_type: str | None = None,
     encoding: str = 'utf8',
-    proto: Protocol = None,
+    proto: Protocol | None = None,
     allow_pickle: bool = False,
     json_loads: Callable[[str], Any] = json.loads,
 ) -> Any:
     if proto is None and content_type:
         if content_type.endswith(('json', 'javascript')):
             pass
         elif allow_pickle and content_type.endswith('pickle'):
@@ -43,17 +43,17 @@
     else:
         raise TypeError(f'Unknown protocol: {proto}')
 
 
 def load_file(
     path: str | Path,
     *,
-    content_type: str = None,
+    content_type: str | None = None,
     encoding: str = 'utf8',
-    proto: Protocol = None,
+    proto: Protocol | None = None,
     allow_pickle: bool = False,
     json_loads: Callable[[str], Any] = json.loads,
 ) -> Any:
     path = Path(path)
     b = path.read_bytes()
     if content_type is None:
         if path.suffix in ('.js', '.json'):
```

### Comparing `pydantic-2.0a1/requirements/README.md` & `pydantic-2.0a2/requirements/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/requirements/all.txt` & `pydantic-2.0a2/requirements/all.txt`

 * *Files 4% similar despite different names*

```diff
@@ -92,20 +92,16 @@
     # via -r requirements/docs.in
 mkdocs-material-extensions==1.1.1
     # via mkdocs-material
 mkdocs-redirects==1.2.0
     # via -r requirements/docs.in
 mkdocs-simple-hooks==0.1.5
     # via -r requirements/docs.in
-mypy==1.1.1
-    # via -r requirements/linting.in
 mypy-extensions==1.0.0
-    # via
-    #   black
-    #   mypy
+    # via black
 nodeenv==1.7.0
     # via pre-commit
 packaging==23.0
     # via
     #   black
     #   mkdocs
     #   pytest
@@ -115,16 +111,18 @@
     # via
     #   black
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==2.21.0
     # via -r requirements/linting.in
-pydantic-core==0.22.0
-    # via -r requirements/linting.in
+pydantic-core==0.23.1
+    # via
+    #   -r requirements/docs.in
+    #   -r requirements/linting.in
 pyflakes==3.0.1
     # via autoflake
 pygments==2.14.0
     # via
     #   mkdocs-material
     #   rich
 pymdown-extensions==9.10
@@ -179,20 +177,18 @@
     # via pyupgrade
 tomli==2.0.1
     # via
     #   -r requirements/docs.in
     #   autoflake
     #   black
     #   coverage
-    #   mypy
     #   pytest
 typing-extensions==4.5.0
     # via
     #   dirty-equals
-    #   mypy
     #   pydantic-core
 urllib3==1.26.15
     # via requests
 virtualenv==20.21.0
     # via pre-commit
 watchdog==3.0.0
     # via mkdocs
```

### Comparing `pydantic-2.0a1/requirements/docs.txt` & `pydantic-2.0a2/requirements/docs.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,50 +19,61 @@
 click==8.1.3
     # via
     #   -c requirements/all.txt
     #   mkdocs
 colorama==0.4.6
     # via
     #   -c requirements/all.txt
+    #   griffe
     #   mkdocs-material
 ghp-import==2.1.0
     # via
     #   -c requirements/all.txt
     #   mkdocs
+griffe==0.26.0
+    # via mkdocstrings-python
 idna==3.4
     # via
     #   -c requirements/all.txt
     #   requests
 jinja2==3.1.2
     # via
     #   -c requirements/all.txt
     #   mkdocs
     #   mkdocs-material
+    #   mkdocstrings
 markdown==3.3.7
     # via
     #   -c requirements/all.txt
     #   mkdocs
+    #   mkdocs-autorefs
     #   mkdocs-material
+    #   mkdocstrings
     #   pymdown-extensions
 markupsafe==2.1.2
     # via
     #   -c requirements/all.txt
     #   jinja2
+    #   mkdocstrings
 mergedeep==1.3.4
     # via
     #   -c requirements/all.txt
     #   mkdocs
 mkdocs==1.4.2
     # via
     #   -c requirements/all.txt
     #   -r requirements/docs.in
+    #   mkdocs-autorefs
     #   mkdocs-exclude
     #   mkdocs-material
     #   mkdocs-redirects
     #   mkdocs-simple-hooks
+    #   mkdocstrings
+mkdocs-autorefs==0.4.1
+    # via mkdocstrings
 mkdocs-exclude==1.0.2
     # via
     #   -c requirements/all.txt
     #   -r requirements/docs.in
 mkdocs-material==9.1.4
     # via
     #   -c requirements/all.txt
@@ -75,30 +86,39 @@
     # via
     #   -c requirements/all.txt
     #   -r requirements/docs.in
 mkdocs-simple-hooks==0.1.5
     # via
     #   -c requirements/all.txt
     #   -r requirements/docs.in
+mkdocstrings==0.21.2
+    # via mkdocstrings-python
+mkdocstrings-python==0.9.0
+    # via -r requirements/docs.in
 packaging==23.0
     # via
     #   -c requirements/all.txt
     #   mkdocs
+pydantic-core==0.23.1
+    # via
+    #   -c requirements/all.txt
+    #   -r requirements/docs.in
 pyflakes==3.0.1
     # via
     #   -c requirements/all.txt
     #   autoflake
 pygments==2.14.0
     # via
     #   -c requirements/all.txt
     #   mkdocs-material
 pymdown-extensions==9.10
     # via
     #   -c requirements/all.txt
     #   mkdocs-material
+    #   mkdocstrings
 python-dateutil==2.8.2
     # via
     #   -c requirements/all.txt
     #   ghp-import
 pyupgrade==3.3.1
     # via
     #   -c requirements/all.txt
@@ -130,14 +150,18 @@
     #   -c requirements/all.txt
     #   pyupgrade
 tomli==2.0.1
     # via
     #   -c requirements/all.txt
     #   -r requirements/docs.in
     #   autoflake
+typing-extensions==4.5.0
+    # via
+    #   -c requirements/all.txt
+    #   pydantic-core
 urllib3==1.26.15
     # via
     #   -c requirements/all.txt
     #   requests
 watchdog==3.0.0
     # via
     #   -c requirements/all.txt
```

### Comparing `pydantic-2.0a1/requirements/linting.txt` & `pydantic-2.0a2/requirements/linting.txt`

 * *Files 8% similar despite different names*

```diff
@@ -40,23 +40,18 @@
     # via
     #   -c requirements/all.txt
     #   -r requirements/linting.in
 identify==2.5.21
     # via
     #   -c requirements/all.txt
     #   pre-commit
-mypy==1.1.1
-    # via
-    #   -c requirements/all.txt
-    #   -r requirements/linting.in
 mypy-extensions==1.0.0
     # via
     #   -c requirements/all.txt
     #   black
-    #   mypy
 nodeenv==1.7.0
     # via
     #   -c requirements/all.txt
     #   pre-commit
 packaging==23.0
     # via
     #   -c requirements/all.txt
@@ -70,15 +65,15 @@
     #   -c requirements/all.txt
     #   black
     #   virtualenv
 pre-commit==2.21.0
     # via
     #   -c requirements/all.txt
     #   -r requirements/linting.in
-pydantic-core==0.22.0
+pydantic-core==0.23.1
     # via
     #   -c requirements/all.txt
     #   -r requirements/linting.in
 pyupgrade==3.3.1
     # via
     #   -c requirements/all.txt
     #   -r requirements/linting.in
@@ -98,19 +93,17 @@
     # via
     #   -c requirements/all.txt
     #   pyupgrade
 tomli==2.0.1
     # via
     #   -c requirements/all.txt
     #   black
-    #   mypy
 typing-extensions==4.5.0
     # via
     #   -c requirements/all.txt
-    #   mypy
     #   pydantic-core
 virtualenv==20.21.0
     # via
     #   -c requirements/all.txt
     #   pre-commit
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `pydantic-2.0a1/requirements/pyproject-all.txt` & `pydantic-2.0a2/requirements/pyproject-all.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,13 +8,13 @@
     # via pydantic (pyproject.toml)
 dnspython==2.3.0
     # via email-validator
 email-validator==1.3.1
     # via pydantic (pyproject.toml)
 idna==3.4
     # via email-validator
-pydantic-core==0.22.0
+pydantic-core==0.23.1
     # via pydantic (pyproject.toml)
 typing-extensions==4.5.0
     # via
     #   pydantic (pyproject.toml)
     #   pydantic-core
```

### Comparing `pydantic-2.0a1/requirements/refresh.sh` & `pydantic-2.0a2/requirements/refresh.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/bin/bash
+set -e
+
 # Rebuild lockfiles from scratch, updating all dependencies
 
 command -v pip-compile >/dev/null 2>&1 || {
   echo >&2 "pip-compile is not installed. Install with 'pip install pip-tools'."
   exit 1
 }
 
@@ -9,13 +12,14 @@
 # refresh the constraints / all lockfile
 pip-compile -q --resolver backtracking -o requirements/all.txt --strip-extras requirements/all.in
 
 # update all of the other lockfiles
 pip-compile -q --resolver backtracking -o requirements/docs.txt requirements/docs-constrained.in
 pip-compile -q --resolver backtracking -o requirements/linting.txt requirements/linting-constrained.in
 pip-compile -q --resolver backtracking -o requirements/testing.txt  requirements/testing-constrained.in
+pip-compile -q --resolver backtracking -o requirements/testing-mypy.txt  requirements/testing-mypy-constrained.in
 pip-compile -q --resolver backtracking -o requirements/testing-extra.txt requirements/testing-extra-constrained.in
 pip-compile -q --resolver backtracking -o requirements/pyproject-min.txt --pip-args '-c requirements/all.txt' pyproject.toml
 pip-compile -q --resolver backtracking -o requirements/pyproject-all.txt --pip-args '-c requirements/all.txt' --all-extras pyproject.toml
 
 # confirm we can do an install
 pip install --dry-run -r requirements/all.txt
```

### Comparing `pydantic-2.0a1/requirements/testing-extra.txt` & `pydantic-2.0a2/requirements/testing-extra.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/requirements/testing.txt` & `pydantic-2.0a2/requirements/testing.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/conftest.py` & `pydantic-2.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_abc.py` & `pydantic-2.0a2/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_aliases.py` & `pydantic-2.0a2/tests/test_create_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,268 +1,298 @@
-from contextlib import nullcontext as does_not_raise
-from typing import Any, ContextManager, List, Optional
+from typing import Optional, Tuple
 
 import pytest
-from dirty_equals import IsStr
 
-from pydantic import BaseModel, ConfigDict, Extra, ValidationError
-from pydantic.fields import Field
+from pydantic import BaseModel, ConfigDict, Field, PydanticUserError, ValidationError, create_model, errors
+from pydantic.decorators import field_validator, validator
+from pydantic.fields import ModelPrivateAttr
 
 
-def test_alias_generator():
-    def to_camel(string: str):
-        return ''.join(x.capitalize() for x in string.split('_'))
+def test_create_model():
+    model = create_model('FooModel', foo=(str, ...), bar=(int, 123))
+    assert issubclass(model, BaseModel)
+    assert model.model_config == BaseModel.model_config
+    assert model.__name__ == 'FooModel'
+    assert model.model_fields.keys() == {'foo', 'bar'}
 
-    class MyModel(BaseModel):
-        model_config = ConfigDict(alias_generator=to_camel)
-        a: List[str] = None
-        foo_bar: str
+    assert not model.__pydantic_decorators__.validator
+    assert not model.__pydantic_decorators__.root_validator
+    assert not model.__pydantic_decorators__.field_validator
+    assert not model.__pydantic_decorators__.field_serializer
 
-    data = {'A': ['foo', 'bar'], 'FooBar': 'foobar'}
-    v = MyModel(**data)
-    assert v.a == ['foo', 'bar']
-    assert v.foo_bar == 'foobar'
-    assert v.model_dump(by_alias=True) == data
+    assert model.__module__ == 'pydantic.main'
 
 
-def test_alias_generator_wrong_type_error():
-    def return_bytes(string):
-        return b'not a string'
+def test_create_model_usage():
+    model = create_model('FooModel', foo=(str, ...), bar=(int, 123))
+    m = model(foo='hello')
+    assert m.foo == 'hello'
+    assert m.bar == 123
+    with pytest.raises(ValidationError):
+        model()
+    with pytest.raises(ValidationError):
+        model(foo='hello', bar='xxx')
 
-    with pytest.raises(TypeError) as e:
 
-        class MyModel(BaseModel):
-            model_config = ConfigDict(alias_generator=return_bytes)
-            bar: Any
+def test_create_model_pickle(create_module):
+    """
+    Pickle will work for dynamically created model only if it was defined globally with its class name
+    and module where it's defined was specified
+    """
 
-    assert str(e.value) == IsStr(regex="alias_generator <function .*> must return str, not <class 'bytes'>")
+    @create_module
+    def module():
+        import pickle
 
+        from pydantic import create_model
 
-def test_basic_alias():
-    class Model(BaseModel):
-        a: str = Field('foobar', alias='_a')
+        FooModel = create_model('FooModel', foo=(str, ...), bar=(int, 123), __module__=__name__)
 
-    assert Model().a == 'foobar'
-    assert Model(_a='different').a == 'different'
-    assert repr(Model.model_fields['a']) == (
-        "FieldInfo(annotation=str, required=False, default='foobar', alias='_a', alias_priority=2)"
-    )
+        m = FooModel(foo='hello')
+        d = pickle.dumps(m)
+        m2 = pickle.loads(d)
+        assert m2.foo == m.foo == 'hello'
+        assert m2.bar == m.bar == 123
+        assert m2 == m
+        assert m2 is not m
 
 
-def test_alias_error():
-    class Model(BaseModel):
-        a: int = Field(123, alias='_a')
+def test_invalid_name():
+    with pytest.warns(RuntimeWarning):
+        model = create_model('FooModel', _foo=(str, ...))
+    assert len(model.model_fields) == 0
 
-    assert Model(_a='123').a == 123
 
-    with pytest.raises(ValidationError) as exc_info:
-        Model(_a='foo')
-    assert exc_info.value.errors() == [
-        {
-            'input': 'foo',
-            'loc': ('_a',),
-            'msg': 'Input should be a valid integer, unable to parse string as an integer',
-            'type': 'int_parsing',
-        }
-    ]
+def test_field_wrong_tuple():
+    with pytest.raises(errors.PydanticUserError):
+        create_model('FooModel', foo=(1, 2, 3))
 
 
-def test_alias_error_loc_by_alias():
-    class Model(BaseModel):
-        model_config = dict(loc_by_alias=False)
-        a: int = Field(123, alias='_a')
+def test_config_and_base():
+    with pytest.raises(errors.PydanticUserError):
+        create_model('FooModel', __config__=BaseModel.model_config, __base__=BaseModel)
 
-    assert Model(_a='123').a == 123
 
-    with pytest.raises(ValidationError) as exc_info:
-        Model(_a='foo')
-    assert exc_info.value.errors() == [
-        {
-            'input': 'foo',
-            'loc': ('a',),
-            'msg': 'Input should be a valid integer, unable to parse string as an integer',
-            'type': 'int_parsing',
-        }
-    ]
+def test_inheritance():
+    class BarModel(BaseModel):
+        x: int = 1
+        y: int = 2
 
+    model = create_model('FooModel', foo=(str, ...), bar=(int, 123), __base__=BarModel)
+    assert model.model_fields.keys() == {'foo', 'bar', 'x', 'y'}
+    m = model(foo='a', x=4)
+    assert m.model_dump() == {'bar': 123, 'foo': 'a', 'x': 4, 'y': 2}
 
-def test_annotation_config():
-    class Model(BaseModel):
-        b: float = Field(alias='foobar')
-        a: int = 10
-        _c: str
 
-    assert list(Model.model_fields.keys()) == ['b', 'a']
-    assert [f.alias for f in Model.model_fields.values()] == ['foobar', None]
-    assert Model(foobar='123').b == 123.0
+def test_custom_config():
+    config = ConfigDict(frozen=True)
+    expected_config = BaseModel.model_config.copy()
+    expected_config['frozen'] = True
 
+    model = create_model('FooModel', foo=(int, ...), __config__=config)
+    m = model(**{'foo': '987'})
+    assert m.foo == 987
+    assert model.model_config == expected_config
+    with pytest.raises(TypeError):
+        m.foo = 654
 
-def test_pop_by_field_name():
-    class Model(BaseModel):
-        model_config = ConfigDict(extra=Extra.forbid, populate_by_name=True)
-        last_updated_by: Optional[str] = Field(None, alias='lastUpdatedBy')
 
-    assert Model(lastUpdatedBy='foo').model_dump() == {'last_updated_by': 'foo'}
-    assert Model(last_updated_by='foo').model_dump() == {'last_updated_by': 'foo'}
-    with pytest.raises(ValidationError) as exc_info:
-        Model(lastUpdatedBy='foo', last_updated_by='bar')
-    assert exc_info.value.errors() == [
-        {
-            'input': 'bar',
-            'loc': ('last_updated_by',),
-            'msg': 'Extra inputs are not permitted',
-            'type': 'extra_forbidden',
-        }
-    ]
+def test_custom_config_inherits():
+    class Config(ConfigDict):
+        custom_config: bool
 
+    config = Config(custom_config=True, validate_assignment=True)
+    expected_config = Config(BaseModel.model_config)
+    expected_config.update(config)
 
-def test_alias_override_behavior():
-    class Parent(BaseModel):
-        # Use `gt` to demonstrate that using `Field` to override an alias does not preserve other attributes
-        x: int = Field(alias='x1', gt=0)
-
-    class Child(Parent):
-        x: int = Field(..., alias='x2')
-        y: int = Field(..., alias='y2')
-
-    assert Parent.model_fields['x'].alias == 'x1'
-    assert Child.model_fields['x'].alias == 'x2'
-    assert Child.model_fields['y'].alias == 'y2'
+    model = create_model('FooModel', foo=(int, ...), __config__=config)
+    m = model(**{'foo': '987'})
+    assert m.foo == 987
+    assert model.model_config == expected_config
+    with pytest.raises(ValidationError):
+        m.foo = ['123']
 
-    Parent(x1=1)
-    with pytest.raises(ValidationError) as exc_info:
-        Parent(x1=-1)
-    assert exc_info.value.errors() == [
-        {'ctx': {'gt': 0}, 'input': -1, 'loc': ('x1',), 'msg': 'Input should be greater than 0', 'type': 'greater_than'}
-    ]
 
-    Child(x2=1, y2=2)
+def test_custom_config_extras():
+    config = ConfigDict(extra='forbid')
 
-    # Check the gt=0 is not preserved from Parent
-    Child(x2=-1, y2=2)
+    model = create_model('FooModel', foo=(int, ...), __config__=config)
+    assert model(foo=654)
+    with pytest.raises(ValidationError):
+        model(bar=654)
 
-    # Check the alias from Parent cannot be used
-    with pytest.raises(ValidationError) as exc_info:
-        Child(x1=1, y2=2)
-    assert exc_info.value.errors() == [
-        {'input': {'x1': 1, 'y2': 2}, 'loc': ('x2',), 'msg': 'Field required', 'type': 'missing'}
-    ]
 
-    # Check the type hint from Parent _is_ preserved
+def test_inheritance_validators():
+    class BarModel(BaseModel):
+        @field_validator('a', check_fields=False)
+        @classmethod
+        def check_a(cls, v):
+            if 'foobar' not in v:
+                raise ValueError('"foobar" not found in a')
+            return v
+
+    model = create_model('FooModel', a=(str, 'cake'), __base__=BarModel)
+    assert model().a == 'cake'
+    assert model(a='this is foobar good').a == 'this is foobar good'
+    with pytest.raises(ValidationError):
+        model(a='something else')
+
+
+def test_inheritance_validators_always():
+    class BarModel(BaseModel):
+        @field_validator('a', check_fields=False)
+        @classmethod
+        def check_a(cls, v):
+            if 'foobar' not in v:
+                raise ValueError('"foobar" not found in a')
+            return v
+
+    model = create_model('FooModel', a=(str, Field('cake', validate_default=True)), __base__=BarModel)
+    with pytest.raises(ValidationError):
+        model()
+    assert model(a='this is foobar good').a == 'this is foobar good'
+    with pytest.raises(ValidationError):
+        model(a='something else')
+
+
+def test_inheritance_validators_all():
+    with pytest.warns(DeprecationWarning, match='Pydantic V1 style `@validator` validators are deprecated'):
+
+        class BarModel(BaseModel):
+            @validator('*')
+            @classmethod
+            def check_all(cls, v):
+                return v * 2
+
+    model = create_model('FooModel', a=(int, ...), b=(int, ...), __base__=BarModel)
+    assert model(a=2, b=6).model_dump() == {'a': 4, 'b': 12}
+
+
+def test_funky_name():
+    model = create_model('FooModel', **{'this-is-funky': (int, ...)})
+    m = model(**{'this-is-funky': '123'})
+    assert m.model_dump() == {'this-is-funky': 123}
     with pytest.raises(ValidationError) as exc_info:
-        Child(x2='a', y2=2)
+        model()
     assert exc_info.value.errors() == [
-        {
-            'input': 'a',
-            'loc': ('x2',),
-            'msg': 'Input should be a valid integer, unable to parse string as an ' 'integer',
-            'type': 'int_parsing',
-        }
+        {'input': {}, 'loc': ('this-is-funky',), 'msg': 'Field required', 'type': 'missing'}
     ]
 
 
-def test_alias_generator_parent():
-    class Parent(BaseModel):
-        model_config = ConfigDict(populate_by_name=True, alias_generator=lambda f_name: f_name + '1')
-        x: int
+def test_repeat_base_usage():
+    class Model(BaseModel):
+        a: str
 
-    class Child(Parent):
-        model_config = ConfigDict(alias_generator=lambda f_name: f_name + '2')
-        y: int
-
-    assert Child.model_fields['y'].alias == 'y2'
-    assert Child.model_fields['x'].alias == 'x2'
-
-
-def test_alias_generator_on_parent():
-    class Parent(BaseModel):
-        model_config = ConfigDict(alias_generator=lambda x: x.upper())
-        x: bool = Field(..., alias='a_b_c')
-        y: str
+    assert Model.model_fields.keys() == {'a'}
 
-    class Child(Parent):
-        y: str
-        z: str
+    model = create_model('FooModel', b=(int, 1), __base__=Model)
+
+    assert Model.model_fields.keys() == {'a'}
+    assert model.model_fields.keys() == {'a', 'b'}
+
+    model2 = create_model('Foo2Model', c=(int, 1), __base__=Model)
 
-    assert Parent.model_fields['x'].alias == 'a_b_c'
-    assert Parent.model_fields['y'].alias == 'Y'
-    assert Child.model_fields['x'].alias == 'a_b_c'
-    assert Child.model_fields['y'].alias == 'Y'
-    assert Child.model_fields['z'].alias == 'Z'
-
-
-def test_alias_generator_on_child():
-    class Parent(BaseModel):
-        x: bool = Field(..., alias='abc')
-        y: str
+    assert Model.model_fields.keys() == {'a'}
+    assert model.model_fields.keys() == {'a', 'b'}
+    assert model2.model_fields.keys() == {'a', 'c'}
 
-    class Child(Parent):
-        model_config = ConfigDict(alias_generator=lambda x: x.upper())
+    model3 = create_model('Foo2Model', d=(int, 1), __base__=model)
 
-        y: str
+    assert Model.model_fields.keys() == {'a'}
+    assert model.model_fields.keys() == {'a', 'b'}
+    assert model2.model_fields.keys() == {'a', 'c'}
+    assert model3.model_fields.keys() == {'a', 'b', 'd'}
+
+
+def test_dynamic_and_static():
+    class A(BaseModel):
+        x: int
+        y: float
         z: str
 
-    assert [f.alias for f in Parent.model_fields.values()] == ['abc', None]
-    assert [f.alias for f in Child.model_fields.values()] == ['abc', 'Y', 'Z']
+    DynamicA = create_model('A', x=(int, ...), y=(float, ...), z=(str, ...))
 
+    for field_name in ('x', 'y', 'z'):
+        assert A.model_fields[field_name].default == DynamicA.model_fields[field_name].default
 
-def test_low_priority_alias():
-    # TODO:
-    #  Alternative 1: we could drop alias_priority and tell people to manually override aliases in child classes
-    #  Alternative 2: we could add a new argument `override_with_alias_generator=True` equivalent to `alias_priority=1`
-    class Parent(BaseModel):
-        w: bool = Field(..., alias='w_')
-        x: bool = Field(..., alias='abc', alias_priority=1)
-        y: str
 
-    class Child(Parent):
-        model_config = ConfigDict(alias_generator=lambda x: x.upper())
+def test_config_field_info_create_model():
+    # TODO fields doesn't exist anymore, remove test?
+    # class Config:
+    #     fields = {'a': {'description': 'descr'}}
+    ConfigDict()
+
+    m1 = create_model('M1', __config__={'title': 'abc'}, a=(str, ...))
+    assert m1.model_json_schema() == {
+        'properties': {'a': {'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+        'title': 'abc',
+        'type': 'object',
+    }
+
+    m2 = create_model('M2', __config__={}, a=(str, Field(description='descr')))
+    assert m2.model_json_schema() == {
+        'properties': {'a': {'description': 'descr', 'title': 'A', 'type': 'string'}},
+        'required': ['a'],
+        'title': 'M2',
+        'type': 'object',
+    }
+
+
+@pytest.mark.parametrize('base', [ModelPrivateAttr, object])
+def test_set_name(base):
+    calls = []
+
+    class class_deco(base):
+        def __init__(self, fn):
+            super().__init__()
+            self.fn = fn
 
-        y: str
-        z: str
+        def __set_name__(self, owner, name):
+            calls.append((owner, name))
 
-    assert [f.alias for f in Parent.model_fields.values()] == ['w_', 'abc', None]
-    assert [f.alias for f in Child.model_fields.values()] == ['w_', 'X', 'Y', 'Z']
+        def __get__(self, obj, type=None):
+            return self.fn(obj) if obj else self
 
+    class A(BaseModel):
+        x: int
 
-def test_empty_string_alias():
-    class Model(BaseModel):
-        empty_string_key: int = Field(alias='')
+        @class_deco
+        def _some_func(self):
+            return self.x
+
+    assert calls == [(A, '_some_func')]
+    a = A(x=2)
+
+    # we don't test whether calling the method on a PrivateAttr works:
+    # attribute access on privateAttributes is more complicated, it doesn't
+    # get added to the class namespace (and will also get set on the instance
+    # with _init_private_attributes), so the descriptor protocol won't work.
+    if base is object:
+        assert a._some_func == 2
+
+
+def test_create_model_with_slots():
+    field_definitions = {'__slots__': (Optional[Tuple[str, ...]], None), 'foobar': (Optional[int], None)}
+    with pytest.warns(RuntimeWarning, match='__slots__ should not be passed to create_model'):
+        model = create_model('PartialPet', **field_definitions)
+
+    assert model.model_fields.keys() == {'foobar'}
+
+
+def test_create_model_non_annotated():
+    with pytest.raises(
+        TypeError,
+        match='A non-annotated attribute was detected: `bar = 123`. All model fields require a type annotation',
+    ):
+        create_model('FooModel', foo=(str, ...), bar=123)
+
+
+def test_create_model_tuple():
+    model = create_model('FooModel', foo=(Tuple[int, int], (1, 2)))
+    assert model().foo == (1, 2)
+    assert model(foo=(3, 4)).foo == (3, 4)
 
-    data = {'': 123}
-    m = Model(**data)
-    assert m.empty_string_key == 123
-    assert m.model_dump(by_alias=True) == data
-
-
-@pytest.mark.parametrize(
-    'use_construct, populate_by_name_config, arg_name, expectation',
-    [
-        [False, True, 'bar', does_not_raise()],
-        [False, True, 'bar_', does_not_raise()],
-        [False, False, 'bar', does_not_raise()],
-        [False, False, 'bar_', pytest.raises(ValueError)],
-        [True, True, 'bar', does_not_raise()],
-        [True, True, 'bar_', does_not_raise()],
-        [True, False, 'bar', does_not_raise()],
-        [True, False, 'bar_', does_not_raise()],
-    ],
-)
-def test_populate_by_name_config(
-    use_construct: bool,
-    populate_by_name_config: bool,
-    arg_name: str,
-    expectation: ContextManager,
-):
-    expected_value: int = 7
-
-    class Foo(BaseModel):
-        model_config = ConfigDict(populate_by_name=populate_by_name_config)
-        bar_: int = Field(..., alias='bar')
-
-    with expectation:
-        if use_construct:
-            f = Foo.model_construct(**{arg_name: expected_value})
-        else:
-            f = Foo(**{arg_name: expected_value})
 
-        assert f.bar_ == expected_value
+def test_create_model_tuple_3():
+    with pytest.raises(PydanticUserError, match=r'^Field definitions should either be a `\(<type>, <default>\)`\.\n'):
+        create_model('FooModel', foo=(Tuple[int, int], (1, 2), 'more'))
```

### Comparing `pydantic-2.0a1/tests/test_annotated.py` & `pydantic-2.0a2/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_assert_in_validators.py` & `pydantic-2.0a2/tests/test_assert_in_validators.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_callable.py` & `pydantic-2.0a2/tests/test_callable.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_color.py` & `pydantic-2.0a2/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_config.py` & `pydantic-2.0a2/tests/test_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import re
 import sys
 from contextlib import nullcontext as does_not_raise
 from functools import partial
 from inspect import signature
-from typing import Any, ContextManager, Iterable, NamedTuple, Type, Union
+from typing import Any, ContextManager, Iterable, NamedTuple, Type, Union, get_type_hints
 
 from dirty_equals import HasRepr
+from pydantic_core import SchemaError
 
 from pydantic import (
     BaseConfig,
     BaseModel,
-    Extra,
     Field,
     PrivateAttr,
     PydanticSchemaGenerationError,
     ValidationError,
     create_model,
     validate_arguments,
 )
-from pydantic.config import ConfigDict, _default_config, get_config
+from pydantic._internal._config import ConfigWrapper, config_defaults
+from pydantic.config import ConfigDict
 from pydantic.dataclasses import dataclass as pydantic_dataclass
 from pydantic.errors import PydanticUserError
 
 if sys.version_info < (3, 9):
     from typing_extensions import Annotated
 else:
     from typing import Annotated
@@ -65,15 +66,15 @@
     with pytest.raises(KeyError, match="'missing_property'"):
         ConfigDict()['missing_property']
 
 
 @pytest.mark.filterwarnings('ignore:.* is deprecated.*:DeprecationWarning')
 class TestsBaseConfig:
     def test_base_config_equality_defaults_of_config_dict_class(self):
-        for key, value in _default_config.items():
+        for key, value in config_defaults.items():
             assert getattr(BaseConfig, key) == value
 
     def test_config_and_module_config_cannot_be_used_together(self):
         with pytest.raises(PydanticUserError):
 
             class MyModel(BaseModel):
                 model_config = ConfigDict(title='MyTitle')
@@ -89,28 +90,26 @@
         class MyBaseModel(BaseModel):
             class Config(MyConfig):
                 ...
 
         class MyModel(MyBaseModel):
             ...
 
-        expected = _default_config.copy()
-        expected['title'] = 'MyTitle'
-        expected['frozen'] = True
-        for k, v in expected.items():
-            assert MyModel.model_config[k] == v
+        MyModel.model_config['title'] = 'MyTitle'
+        MyModel.model_config['frozen'] = True
+        assert 'str_to_lower' not in MyModel.model_config
 
     def test_base_config_custom_init_signature(self):
         class MyModel(BaseModel):
             id: int
             name: str = 'John Doe'
             f__: str = Field(..., alias='foo')
 
             class Config:
-                extra = Extra.allow
+                extra = 'allow'
 
             def __init__(self, id: int = 1, bar=2, *, baz: Any, **data):
                 super().__init__(id=id, **data)
                 self.bar = bar
                 self.baz = baz
 
         sig = signature(MyModel)
@@ -126,15 +125,15 @@
             b: int = 2
             c: int
 
             def __init__(self, a: float, b: int):
                 super().__init__(a=a, b=b, c=1)
 
             class Config:
-                extra = Extra.allow
+                extra = 'allow'
 
         assert _equals(str(signature(Model)), '(a: float, b: int) -> None')
 
     def test_base_config_use_field_name(self):
         class Foo(BaseModel):
             foo: str = Field(..., alias='this is invalid')
 
@@ -153,46 +152,46 @@
         assert _equals(str(signature(Foo)), '(*, from_: str) -> None')
 
     def test_base_config_extra_allow_no_conflict(self):
         class Model(BaseModel):
             spam: str
 
             class Config:
-                extra = Extra.allow
+                extra = 'allow'
 
         assert _equals(str(signature(Model)), '(*, spam: str, **extra_data: Any) -> None')
 
     def test_base_config_extra_allow_conflict_twice(self):
         class Model(BaseModel):
             extra_data: str
             extra_data_: str
 
             class Config:
-                extra = Extra.allow
+                extra = 'allow'
 
         assert _equals(str(signature(Model)), '(*, extra_data: str, extra_data_: str, **extra_data__: Any) -> None')
 
     def test_base_config_extra_allow_conflict_custom_signature(self):
         class Model(BaseModel):
             extra_data: int
 
             def __init__(self, extra_data: int = 1, **foobar: Any):
                 super().__init__(extra_data=extra_data, **foobar)
 
             class Config:
-                extra = Extra.allow
+                extra = 'allow'
 
         assert _equals(str(signature(Model)), '(extra_data: int = 1, **foobar: Any) -> None')
 
     def test_base_config_private_attribute_intersection_with_extra_field(self):
         class Model(BaseModel):
             _foo = PrivateAttr('private_attribute')
 
             class Config:
-                extra = Extra.allow
+                extra = 'allow'
 
         assert Model.__slots__ == {'_foo'}
         m = Model(_foo='field')
         assert m._foo == 'private_attribute'
         assert m.__dict__ == m.model_dump() == {'_foo': 'field'}
         m._foo = 'still_private'
         assert m._foo == 'still_private'
@@ -347,45 +346,45 @@
                 frozen = True
 
         m = Model(a=40, b=10)
         assert m == m.model_copy()
 
     def test_config_class_is_deprecated(self):
         with pytest.warns(
-            DeprecationWarning, match='`BaseConfig` is deprecated and will be removed in a future version'
+            DeprecationWarning, match='Support for class-based `config` is deprecated, use ConfigDict instead.'
         ):
 
             class Config(BaseConfig):
                 pass
 
     def test_config_class_attributes_are_deprecated(self):
         with pytest.warns(
             DeprecationWarning,
-            match='Support for "config" as "BaseConfig" is deprecated and will be removed in a future version"',
+            match='Support for class-based `config` is deprecated, use ConfigDict instead.',
         ):
             assert BaseConfig.validate_assignment is False
 
         with pytest.warns(
             DeprecationWarning,
-            match='Support for "config" as "BaseConfig" is deprecated and will be removed in a future version"',
+            match='Support for class-based `config` is deprecated, use ConfigDict instead.',
         ):
             assert BaseConfig().validate_assignment is False
 
         class Config(BaseConfig):
             pass
 
         with pytest.warns(
             DeprecationWarning,
-            match='Support for "config" as "Config" is deprecated and will be removed in a future version"',
+            match='Support for class-based `config` is deprecated, use ConfigDict instead.',
         ):
             assert Config.validate_assignment is False
 
         with pytest.warns(
             DeprecationWarning,
-            match='Support for "config" as "Config" is deprecated and will be removed in a future version"',
+            match='Support for class-based `config` is deprecated, use ConfigDict instead.',
         ):
             assert Config().validate_assignment is False
 
     def test_config_class_missing_attributes(self):
         with pytest.raises(AttributeError, match="type object 'BaseConfig' has no attribute 'missing_attribute'"):
             BaseConfig.missing_attribute
 
@@ -460,56 +459,106 @@
 
         @validate_arguments(config=config_dict)
         def my_function():
             pass
 
 
 def test_invalid_extra():
-    error_message = "'{label}': 'invalid-value' is not a valid value for config['extra']"
+    extra_error = re.escape(
+        "Input should be 'allow', 'forbid' or 'ignore'"
+        " [type=literal_error, input_value='invalid-value', input_type=str]"
+    )
     config_dict = {'extra': 'invalid-value'}
 
-    with pytest.raises(ValueError, match=re.escape(error_message.format(label='MyModel'))):
+    with pytest.raises(SchemaError, match=extra_error):
 
         class MyModel(BaseModel):
             model_config = config_dict
 
-    with pytest.raises(ValueError, match=re.escape(error_message.format(label='MyCreatedModel'))):
+    with pytest.raises(SchemaError, match=extra_error):
         create_model('MyCreatedModel', __config__=config_dict)
 
-    with pytest.raises(ValueError, match=re.escape(error_message.format(label='MyDataclass'))):
+    with pytest.raises(SchemaError, match='Invalid extra_behavior: `invalid-value`'):
 
         @pydantic_dataclass(config=config_dict)
         class MyDataclass:
             pass
 
-    with pytest.raises(ValueError, match=re.escape(error_message.format(label='my_function'))):
+    with pytest.raises(SchemaError, match=extra_error):
 
         @validate_arguments(config=config_dict)
         def my_function():
             pass
 
-    with pytest.raises(ValueError, match=re.escape(error_message.format(label='validate_arguments'))):
+    with pytest.raises(SchemaError, match=extra_error):
         # This case happens when the function passed to `validate_arguments` has no `__name__`.
         # This is a pretty exotic case, but it has caused issues in the past, so I wanted to add a test.
         def my_wrapped_function():
             pass
 
         my_partial_function = partial(my_wrapped_function)
         my_partial_function.__annotations__ = my_wrapped_function.__annotations__
         validate_arguments(config=config_dict)(my_partial_function)
 
-    with pytest.raises(ValueError, match=re.escape(error_message.format(label='ConfigDict'))):
-        get_config(config_dict)
-
 
 def test_invalid_config_keys():
     with pytest.raises(
         PydanticUserError,
         match=re.escape(
             'Setting the "alias_generator" property on custom Config for'
             ' @validate_arguments is not yet supported, please remove.'
         ),
     ):
 
-        @validate_arguments(config={'alias_generator': None})
+        @validate_arguments(config={'alias_generator': lambda x: x})
         def my_function():
             pass
+
+
+def test_multiple_inheritance_config():
+    class Parent(BaseModel):
+        model_config = ConfigDict(frozen=True, extra='forbid')
+
+    class Mixin(BaseModel):
+        model_config = ConfigDict(use_enum_values=True)
+
+    class Child(Mixin, Parent):
+        model_config = ConfigDict(populate_by_name=True)
+
+    assert BaseModel.model_config.get('frozen') is None
+    assert BaseModel.model_config.get('populate_by_name') is None
+    assert BaseModel.model_config.get('extra') is None
+    assert BaseModel.model_config.get('use_enum_values') is None
+
+    assert Parent.model_config.get('frozen') is True
+    assert Parent.model_config.get('populate_by_name') is None
+    assert Parent.model_config.get('extra') == 'forbid'
+    assert Parent.model_config.get('use_enum_values') is None
+
+    assert Mixin.model_config.get('frozen') is None
+    assert Mixin.model_config.get('populate_by_name') is None
+    assert Mixin.model_config.get('extra') is None
+    assert Mixin.model_config.get('use_enum_values') is True
+
+    assert Child.model_config.get('frozen') is True
+    assert Child.model_config.get('populate_by_name') is True
+    assert Child.model_config.get('extra') == 'forbid'
+    assert Child.model_config.get('use_enum_values') is True
+
+
+@pytest.mark.skipif(sys.version_info < (3, 10), reason='different on older versions')
+def test_config_wrapper_match():
+    config_dict_annotations = [(k, str(v)) for k, v in get_type_hints(ConfigDict).items()]
+    # remove config
+    config_wrapper_annotations = [(k, str(v)) for k, v in get_type_hints(ConfigWrapper).items() if k != 'config_dict']
+
+    assert (
+        config_dict_annotations == config_wrapper_annotations
+    ), 'ConfigDict and ConfigWrapper must have the same annotations (except ConfigWrapper.config_dict)'
+
+
+@pytest.mark.skipif(sys.version_info < (3, 10), reason='different on older versions')
+def test_config_defaults_match():
+    config_dict_keys = list(get_type_hints(ConfigDict).keys())
+    config_defaults_keys = list(config_defaults.keys())
+
+    assert config_dict_keys == config_defaults_keys, 'ConfigDict and config_defaults must have the same keys'
```

### Comparing `pydantic-2.0a1/tests/test_construction.py` & `pydantic-2.0a2/tests/test_construction.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     b: int = 10
 
 
 def test_simple_construct():
     m = Model.model_construct(a=3.14)
     assert m.a == 3.14
     assert m.b == 10
-    assert m.__fields_set__ == {'a'}
+    assert m.model_fields_set == {'a'}
     assert m.model_dump() == {'a': 3.14, 'b': 10}
 
 
 def test_construct_misuse():
     m = Model.model_construct(b='foobar')
     assert m.b == 'foobar'
     with pytest.warns(UserWarning, match='Expected `int` but got `str`'):
@@ -29,15 +29,15 @@
         print(m.a)
 
 
 def test_construct_fields_set():
     m = Model.model_construct(a=3.0, b=-1, _fields_set={'a'})
     assert m.a == 3
     assert m.b == -1
-    assert m.__fields_set__ == {'a'}
+    assert m.model_fields_set == {'a'}
     assert m.model_dump() == {'a': 3, 'b': -1}
 
 
 def test_construct_allow_extra():
     """model_construct() should allow extra fields"""
 
     class Foo(BaseModel, extra='allow'):
@@ -426,16 +426,16 @@
         name: str
         age: int
         dob: str
 
     user = User(name='test_user', age=23, dob='01/01/2000')
     user_copy = deprecated_copy(user, exclude={'dob': ...})
 
-    assert 'dob' in user.__fields_set__
-    assert 'dob' not in user_copy.__fields_set__
+    assert 'dob' in user.model_fields_set
+    assert 'dob' not in user_copy.model_fields_set
 
 
 def test_dunder_copy(ModelTwo):
     m = ModelTwo(a=24, d=Model(a='12'))
     m2 = m.__copy__()
     assert m is not m2
```

### Comparing `pydantic-2.0a1/tests/test_dataclasses.py` & `pydantic-2.0a2/tests/test_dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from typing import Any, Callable, ClassVar, Dict, FrozenSet, List, Optional, Set, Union
 
 import pytest
 from typing_extensions import Literal
 
 import pydantic
-from pydantic import BaseModel, ConfigDict, Extra, FieldValidationInfo, ValidationError
+from pydantic import BaseModel, ConfigDict, FieldValidationInfo, ValidationError
 from pydantic.decorators import field_validator
 from pydantic.fields import Field, FieldInfo
 from pydantic.json_schema import model_json_schema
 
 
 def test_simple():
     @pydantic.dataclasses.dataclass
@@ -135,21 +135,21 @@
 
 
 @pytest.mark.parametrize(
     'config',
     [
         ConfigDict(validate_assignment=False),
         ConfigDict(extra=None),
-        ConfigDict(extra=Extra.forbid),
-        ConfigDict(extra=Extra.ignore),
+        ConfigDict(extra='forbid'),
+        ConfigDict(extra='ignore'),
         ConfigDict(validate_assignment=False, extra=None),
-        ConfigDict(validate_assignment=False, extra=Extra.forbid),
-        ConfigDict(validate_assignment=False, extra=Extra.ignore),
-        ConfigDict(validate_assignment=False, extra=Extra.allow),
-        ConfigDict(validate_assignment=True, extra=Extra.allow),
+        ConfigDict(validate_assignment=False, extra='forbid'),
+        ConfigDict(validate_assignment=False, extra='ignore'),
+        ConfigDict(validate_assignment=False, extra='allow'),
+        ConfigDict(validate_assignment=True, extra='allow'),
     ],
 )
 def test_validate_assignment_extra_unknown_field_assigned_allowed(config: ConfigDict):
     @pydantic.dataclasses.dataclass(config=config)
     class MyDataclass:
         a: int
 
@@ -161,16 +161,16 @@
 
 
 @pytest.mark.parametrize(
     'config',
     [
         ConfigDict(validate_assignment=True),
         ConfigDict(validate_assignment=True, extra=None),
-        ConfigDict(validate_assignment=True, extra=Extra.forbid),
-        ConfigDict(validate_assignment=True, extra=Extra.ignore),
+        ConfigDict(validate_assignment=True, extra='forbid'),
+        ConfigDict(validate_assignment=True, extra='ignore'),
     ],
 )
 def test_validate_assignment_extra_unknown_field_assigned_errors(config: ConfigDict):
     @pydantic.dataclasses.dataclass(config=config)
     class MyDataclass:
         a: int
 
@@ -865,34 +865,14 @@
 
     pika = X(x='2', y='4', z='3')
     assert pika.x == 2
     assert pika.y == 4
     assert pika.z == 3
 
 
-@pytest.mark.xfail(reason='cannot parse a tuple into a dataclass')
-def test_dataclass_arbitrary():
-    class ArbitraryType:
-        def __init__(self):
-            ...
-
-    @dataclasses.dataclass
-    class Test:
-        foo: ArbitraryType
-        bar: List[ArbitraryType]
-
-    class TestModel(BaseModel):
-        a: ArbitraryType
-        b: Test
-
-        model_config = ConfigDict(arbitrary_types_allowed=True)
-
-    TestModel(a=ArbitraryType(), b=(ArbitraryType(), [ArbitraryType()]))
-
-
 def test_forward_stdlib_dataclass_params():
     @dataclasses.dataclass(frozen=True)
     class Item:
         name: str
 
     class Example(BaseModel):
         item: Item
@@ -964,17 +944,15 @@
     module = create_module(
         # language=Python
         """\
 import dataclasses
 import pydantic
 
 
-@pydantic.dataclasses.dataclass(
-    config=pydantic.config.ConfigDict(validate_assignment=True)
-)
+@pydantic.dataclasses.dataclass(config=pydantic.config.ConfigDict(validate_assignment=True))
 class BuiltInDataclassForPickle:
     value: int
         """
     )
     obj = module.BuiltInDataclassForPickle(value=5)
 
     pickled_obj = pickle.dumps(obj)
@@ -1332,61 +1310,60 @@
     test_string = 'string'
     for cls in clases_to_test:
         instance = cls(a=test_string)
         assert instance._special_property == 1
         assert instance.a == test_string
 
 
-@pytest.mark.xfail(reason='model_config["extra"] is not respected')
 def test_ignore_extra():
-    @pydantic.dataclasses.dataclass(config=dict(extra=Extra.ignore))
+    @pydantic.dataclasses.dataclass(config=ConfigDict(extra='ignore'))
     class Foo:
         x: int
 
     foo = Foo(**{'x': '1', 'y': '2'})
-    assert foo.__dict__ == {'x': 1, '__pydantic_initialised__': True}
+    assert foo.__dict__ == {'x': 1}
 
 
 def test_ignore_extra_subclass():
-    @pydantic.dataclasses.dataclass(config=ConfigDict(extra=Extra.ignore))
+    @pydantic.dataclasses.dataclass(config=ConfigDict(extra='ignore'))
     class Foo:
         x: int
 
-    @pydantic.dataclasses.dataclass(config=ConfigDict(extra=Extra.ignore))
+    @pydantic.dataclasses.dataclass(config=ConfigDict(extra='ignore'))
     class Bar(Foo):
         y: int
 
     bar = Bar(**{'x': '1', 'y': '2', 'z': '3'})
     assert bar.__dict__ == {'x': 1, 'y': 2}
 
 
 def test_allow_extra():
-    @pydantic.dataclasses.dataclass(config=ConfigDict(extra=Extra.allow))
+    @pydantic.dataclasses.dataclass(config=ConfigDict(extra='allow'))
     class Foo:
         x: int
 
     foo = Foo(**{'x': '1', 'y': '2'})
     assert foo.__dict__ == {'x': 1, 'y': '2'}
 
 
 def test_allow_extra_subclass():
-    @pydantic.dataclasses.dataclass(config=ConfigDict(extra=Extra.allow))
+    @pydantic.dataclasses.dataclass(config=ConfigDict(extra='allow'))
     class Foo:
         x: int
 
-    @pydantic.dataclasses.dataclass(config=ConfigDict(extra=Extra.allow))
+    @pydantic.dataclasses.dataclass(config=ConfigDict(extra='allow'))
     class Bar(Foo):
         y: int
 
     bar = Bar(**{'x': '1', 'y': '2', 'z': '3'})
     assert bar.__dict__ == {'x': 1, 'y': 2, 'z': '3'}
 
 
 def test_forbid_extra():
-    @pydantic.dataclasses.dataclass(config=ConfigDict(extra=Extra.forbid))
+    @pydantic.dataclasses.dataclass(config=ConfigDict(extra='forbid'))
     class Foo:
         x: int
 
     msg = re.escape("Unexpected keyword argument [type=unexpected_keyword_argument, input_value='2', input_type=str]")
 
     with pytest.raises(ValidationError, match=msg):
         Foo(**{'x': '1', 'y': '2'})
@@ -1415,27 +1392,27 @@
     with pytest.raises(ValidationError):
         A(1, '')
 
     assert A(b='hi').b == 'hi'
 
 
 def test_extra_forbid_list_no_error():
-    @pydantic.dataclasses.dataclass(config=dict(extra=Extra.forbid))
+    @pydantic.dataclasses.dataclass(config=dict(extra='forbid'))
     class Bar:
         ...
 
     @pydantic.dataclasses.dataclass
     class Foo:
         a: List[Bar]
 
     assert isinstance(Foo(a=[Bar()]).a[0], Bar)
 
 
 def test_extra_forbid_list_error():
-    @pydantic.dataclasses.dataclass(config=ConfigDict(extra=Extra.forbid))
+    @pydantic.dataclasses.dataclass(config=ConfigDict(extra='forbid'))
     class Bar:
         ...
 
     with pytest.raises(ValidationError, match=r'a\s+Unexpected keyword argument'):
         Bar(a=1)
 
 
@@ -1527,15 +1504,15 @@
 
 
 def test_config_as_type_deprecated():
     class Config:
         validate_assignment = True
 
     with pytest.warns(
-        DeprecationWarning, match='Support for "config" as "type" is deprecated and will be removed in a future version'
+        DeprecationWarning, match='Support for class-based `config` is deprecated, use ConfigDict instead.'
     ):
 
         @pydantic.dataclasses.dataclass(config=Config)
         class MyDataclass:
             a: int
 
     assert MyDataclass.__pydantic_config__ == ConfigDict(validate_assignment=True)
@@ -1582,47 +1559,47 @@
     it replaces the existing validator and is run instead of it.
     """
 
     @decorator1
     class Parent:
         a: List[str]
 
-        @field_validator('a', allow_reuse=True)
+        @field_validator('a')
         @classmethod
         def parent_val_before(cls, v: List[str]):
             v.append('parent before')
             return v
 
-        @field_validator('a', allow_reuse=True)
+        @field_validator('a')
         @classmethod
         def val(cls, v: List[str]):
             v.append('parent')
             return v
 
-        @field_validator('a', allow_reuse=True)
+        @field_validator('a')
         @classmethod
         def parent_val_after(cls, v: List[str]):
             v.append('parent after')
             return v
 
     @pydantic.dataclasses.dataclass
     class Child(Parent):
-        @field_validator('a', allow_reuse=True)
+        @field_validator('a')
         @classmethod
         def child_val_before(cls, v: List[str]):
             v.append('child before')
             return v
 
-        @field_validator('a', allow_reuse=True)
+        @field_validator('a')
         @classmethod
         def val(cls, v: List[str]):
             v.append('child')
             return v
 
-        @field_validator('a', allow_reuse=True)
+        @field_validator('a')
         @classmethod
         def child_val_after(cls, v: List[str]):
             v.append('child after')
             return v
 
     assert Parent(a=[]).a == expected_parent
     assert Child(a=[]).a == expected_child
```

### Comparing `pydantic-2.0a1/tests/test_datetime.py` & `pydantic-2.0a2/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_decorator.py` & `pydantic-2.0a2/tests/test_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import List
 
 import pytest
 from dirty_equals import IsInstance
 from typing_extensions import Annotated, TypedDict
 
-from pydantic import BaseModel, Extra, Field, ValidationError, validate_arguments
+from pydantic import BaseModel, Field, ValidationError, validate_arguments
 from pydantic.decorator import ValidatedFunction
 from pydantic.errors import PydanticUserError
 
 skip_pre_38 = pytest.mark.skipif(sys.version_info < (3, 8), reason='testing >= 3.8 behaviour only')
 
 
 def test_args():
@@ -443,18 +443,18 @@
 
 
 @pytest.mark.xfail(reason='config["extra"] does not seem to be respected')
 def test_validate_extra():
     class TypedTest(TypedDict):
         y: str
 
-    @validate_arguments(config={'extra': Extra.allow})
+    @validate_arguments(config={'extra': 'allow'})
     def test(other: TypedTest):
         return other
 
     assert test(other={'y': 'b', 'z': 'a'}) == {'y': 'b', 'z': 'a'}
 
-    @validate_arguments(config={'extra': Extra.ignore})
+    @validate_arguments(config={'extra': 'ignore'})
     def test(other: TypedTest):
         return other
 
     assert test(other={'y': 'b', 'z': 'a'}) == {'y': 'b'}
```

### Comparing `pydantic-2.0a1/tests/test_discriminated_union.py` & `pydantic-2.0a2/tests/test_discriminated_union.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,20 +465,15 @@
         ValidationError,
         match=re.escape(
             "Input tag 'Other' found using 'type' does not match any of the expected tags: 'Success', 'Failure'"
         ),
     ):
         Container[str].model_validate({'result': {'type': 'Other'}})
 
-    # See https://github.com/pydantic/pydantic-core/issues/425 for why this is set weirdly; this is an unrelated issue
-    # If/when the issue is fixed, the following line should replace the current title = 'Failure' line
-    # title = 'Container[str]'
-    title = 'Failure'
-
-    with pytest.raises(ValidationError, match=f'{title}\nresult -> Success -> data') as exc_info:
+    with pytest.raises(ValidationError, match=r'Container\[str\]\nresult\.Success\.data') as exc_info:
         Container[str].model_validate({'result': {'type': 'Success'}})
     assert exc_info.value.errors() == [
         {'input': {'type': 'Success'}, 'loc': ('result', 'Success', 'data'), 'msg': 'Field required', 'type': 'missing'}
     ]
 
     # invalid types error
     with pytest.raises(ValidationError) as exc_info:
```

### Comparing `pydantic-2.0a1/tests/test_docs.py` & `pydantic-2.0a2/tests/test_docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from datetime import datetime
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 import pytest
 from pytest_examples import CodeExample, EvalExample, find_examples
 
+from pydantic.errors import PydanticErrorCodes
+
 INDEX_MAIN = None
 DOCS_ROOT = Path(__file__).parent.parent / 'docs'
 
 
 def skip_docs_tests():
     if sys.platform not in {'linux', 'darwin'}:
         return 'not in linux or macos'
@@ -176,7 +178,17 @@
 
     if eval_example.update_examples:
         output_file.write_text(output_html)
     elif not output_file.exists():
         pytest.fail(f'output file {output_file} does not exist')
     else:
         assert output_html == output_file.read_text()
+
+
+def test_error_codes():
+    error_text = (DOCS_ROOT / 'usage/errors.md').read_text()
+
+    code_error_codes = PydanticErrorCodes.__args__
+
+    documented_error_codes = tuple(re.findall(r'^## .+ \{#(.+?)}$', error_text, flags=re.MULTILINE))
+
+    assert code_error_codes == documented_error_codes, 'Error codes in code and docs do not match'
```

### Comparing `pydantic-2.0a1/tests/test_edge_cases.py` & `pydantic-2.0a2/tests/test_edge_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,25 @@
 from decimal import Decimal
 from enum import Enum
 from typing import Any, Dict, FrozenSet, Generic, List, Optional, Sequence, Set, Tuple, Type, TypeVar, Union
 
 import pytest
 from dirty_equals import HasRepr, IsStr
 from pydantic_core import core_schema
-from typing_extensions import get_args
+from typing_extensions import Annotated, get_args
 
 from pydantic import (
     AnalyzedType,
     BaseModel,
     ConfigDict,
-    Extra,
     PydanticSchemaGenerationError,
     ValidationError,
     constr,
     errors,
 )
-from pydantic._internal._fields import PydanticGeneralMetadata
-from pydantic.config import get_config
 from pydantic.decorators import field_validator
 from pydantic.fields import Field
 
 
 def test_str_bytes():
     class Model(BaseModel):
         v: Union[str, bytes] = ...
@@ -526,15 +523,15 @@
         c: int = 3
         d: int = 4
         e: int = 5
         f: int = 6
 
     m = Model(a=1, b=2, e=5, f=7)
     assert m.model_dump() == {'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5, 'f': 7}
-    assert m.__fields_set__ == {'a', 'b', 'e', 'f'}
+    assert m.model_fields_set == {'a', 'b', 'e', 'f'}
     assert m.model_dump(exclude_unset=True) == {'a': 1, 'b': 2, 'e': 5, 'f': 7}
 
     assert m.model_dump(include={'a'}, exclude_unset=True) == {'a': 1}
     assert m.model_dump(include={'c'}, exclude_unset=True) == {}
 
     assert m.model_dump(exclude={'a'}, exclude_unset=True) == {'b': 2, 'e': 5, 'f': 7}
     assert m.model_dump(exclude={'c'}, exclude_unset=True) == {'a': 1, 'b': 2, 'e': 5, 'f': 7}
@@ -550,15 +547,15 @@
         c: int = 3
         d: int = 4
         e: int = 5
         f: int = 6
 
     m = Model(a=1, b=2, e=5, f=7)
     assert m.model_dump() == {'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5, 'f': 7}
-    assert m.__fields_set__ == {'a', 'b', 'e', 'f'}
+    assert m.model_fields_set == {'a', 'b', 'e', 'f'}
     assert m.model_dump(exclude_defaults=True) == {'a': 1, 'b': 2, 'f': 7}
 
     assert m.model_dump(include={'a'}, exclude_defaults=True) == {'a': 1}
     assert m.model_dump(include={'c'}, exclude_defaults=True) == {}
 
     assert m.model_dump(exclude={'a'}, exclude_defaults=True) == {'b': 2, 'f': 7}
     assert m.model_dump(exclude={'c'}, exclude_defaults=True) == {'a': 1, 'b': 2, 'f': 7}
@@ -863,45 +860,45 @@
     m = Model(subs=[dict(k=1, subsubs=[dict(i=1, j=1), dict(i=2, j=2)]), dict(k=2, subsubs=[dict(i=3, j=3)])])
 
     assert m.model_dump(include=include) == expected
 
 
 def test_field_set_ignore_extra():
     class Model(BaseModel):
-        model_config = ConfigDict(extra=Extra.ignore)
+        model_config = ConfigDict(extra='ignore')
         a: int
         b: int
         c: int = 3
 
     m = Model(a=1, b=2)
     assert m.model_dump() == {'a': 1, 'b': 2, 'c': 3}
-    assert m.__fields_set__ == {'a', 'b'}
+    assert m.model_fields_set == {'a', 'b'}
     assert m.model_dump(exclude_unset=True) == {'a': 1, 'b': 2}
 
     m2 = Model(a=1, b=2, d=4)
     assert m2.model_dump() == {'a': 1, 'b': 2, 'c': 3}
-    assert m2.__fields_set__ == {'a', 'b'}
+    assert m2.model_fields_set == {'a', 'b'}
     assert m2.model_dump(exclude_unset=True) == {'a': 1, 'b': 2}
 
 
 def test_field_set_allow_extra():
     class Model(BaseModel):
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
         a: int
         b: int
         c: int = 3
 
     m = Model(a=1, b=2)
     assert m.model_dump() == {'a': 1, 'b': 2, 'c': 3}
-    assert m.__fields_set__ == {'a', 'b'}
+    assert m.model_fields_set == {'a', 'b'}
     assert m.model_dump(exclude_unset=True) == {'a': 1, 'b': 2}
 
     m2 = Model(a=1, b=2, d=4)
     assert m2.model_dump() == {'a': 1, 'b': 2, 'c': 3, 'd': 4}
-    assert m2.__fields_set__ == {'a', 'b', 'd'}
+    assert m2.model_fields_set == {'a', 'b', 'd'}
     assert m2.model_dump(exclude_unset=True) == {'a': 1, 'b': 2, 'd': 4}
 
 
 def test_field_set_field_name():
     class Model(BaseModel):
         a: int
         field_set: int
@@ -1101,15 +1098,15 @@
 
         class D(A):
             integer = 'G'
 
 
 def test_string_none():
     class Model(BaseModel):
-        model_config = ConfigDict(extra=Extra.ignore)
+        model_config = ConfigDict(extra='ignore')
         a: constr(min_length=20, max_length=1000) = ...
 
     with pytest.raises(ValidationError) as exc_info:
         Model(a=None)
     assert exc_info.value.errors() == [
         {'input': None, 'loc': ('a',), 'msg': 'Input should be a valid string', 'type': 'string_type'}
     ]
@@ -1178,16 +1175,16 @@
 
 
 def test_unable_to_infer():
     with pytest.raises(
         errors.PydanticUserError,
         match=re.escape(
             "A non-annotated attribute was detected: `x = None`. All model fields require a type annotation; "
-            "if 'x' is not meant to be a field, you may be able to resolve this error by annotating it as a "
-            "ClassVar or updating model_config[\"ignored_types\"]"
+            "if `x` is not meant to be a field, you may be able to resolve this error by annotating it as a "
+            "`ClassVar` or updating `model_config['ignored_types']`"
         ),
     ):
 
         class InvalidDefinitionModel(BaseModel):
             x = None
 
 
@@ -1241,54 +1238,15 @@
 
 
 def test_force_extra():
     class Model(BaseModel):
         model_config = ConfigDict(extra='ignore')
         foo: int
 
-    assert Model.model_config['extra'] is Extra.ignore
-
-
-def test_illegal_extra_value():
-    with pytest.raises(ValueError, match=re.escape("is not a valid value for config['extra']")):
-
-        class Model(BaseModel):
-            model_config = ConfigDict(extra='foo')
-            foo: int
-
-
-def test_multiple_inheritance_config():
-    class Parent(BaseModel):
-        model_config = ConfigDict(frozen=True, extra=Extra.forbid)
-
-    class Mixin(BaseModel):
-        model_config = ConfigDict(use_enum_values=True)
-
-    class Child(Mixin, Parent):
-        model_config = ConfigDict(populate_by_name=True)
-
-    assert BaseModel.model_config['frozen'] is False
-    assert BaseModel.model_config['populate_by_name'] is False
-    assert BaseModel.model_config['extra'] is None
-    assert BaseModel.model_config['use_enum_values'] is False
-
-    assert Parent.model_config['frozen'] is True
-    assert Parent.model_config['populate_by_name'] is False
-    assert Parent.model_config['extra'] is Extra.forbid
-    assert Parent.model_config['use_enum_values'] is False
-
-    assert Mixin.model_config['frozen'] is False
-    assert Mixin.model_config['populate_by_name'] is False
-    assert Mixin.model_config['extra'] is None
-    assert Mixin.model_config['use_enum_values'] is True
-
-    assert Child.model_config['frozen'] is True
-    assert Child.model_config['populate_by_name'] is True
-    assert Child.model_config['extra'] is Extra.forbid
-    assert Child.model_config['use_enum_values'] is True
+    assert Model.model_config['extra'] == 'ignore'
 
 
 def test_submodel_different_type():
     class Foo(BaseModel):
         a: int
 
     class Bar(BaseModel):
@@ -2136,36 +2094,42 @@
 
     with pytest.warns(
         DeprecationWarning, match='The private method `_iter` will be removed and should no longer be used.'
     ):
         assert list(MyModel()._iter(by_alias=True)) == [('x', 1), ('y', 'a')]
 
 
-@pytest.mark.xfail(reason='field frozen')
 def test_frozen_config_and_field():
     class Foo(BaseModel):
         model_config = ConfigDict(frozen=False, validate_assignment=True)
         a: str = Field(...)
 
     assert Foo.model_fields['a'].metadata == []
 
     f = Foo(a='x')
     f.a = 'y'
     assert f.model_dump() == {'a': 'y'}
 
     class Bar(BaseModel):
         model_config = ConfigDict(validate_assignment=True)
         a: str = Field(..., frozen=True)
+        c: Annotated[str, Field(frozen=True)]
 
-    assert PydanticGeneralMetadata(frozen=True) in Bar.model_fields['a'].metadata
+    assert Bar.model_fields['a'].frozen
 
-    b = Bar(a='x')
-    with pytest.raises(TypeError):
+    b = Bar(a='x', c='z')
+    with pytest.raises(ValidationError) as exc_info:
         b.a = 'y'
-    assert b.model_dump() == {'a': 'x'}
+    assert exc_info.value.errors() == [{'input': 'y', 'loc': ('a',), 'msg': 'Field is frozen', 'type': 'frozen_field'}]
+
+    with pytest.raises(ValidationError) as exc_info:
+        b.c = 'y'
+    assert exc_info.value.errors() == [{'input': 'y', 'loc': ('c',), 'msg': 'Field is frozen', 'type': 'frozen_field'}]
+
+    assert b.model_dump() == {'a': 'x', 'c': 'z'}
 
 
 def test_arbitrary_types_allowed_custom_eq():
     class Foo:
         def __eq__(self, other):
             if other.__class__ is not Foo:
                 raise TypeError(f'Cannot interpret {other.__class__.__name__!r} as a valid type')
@@ -2280,27 +2244,7 @@
     class Child(Parent):
         c: int = 3
 
     c = Child()
     assert c.a == 1
     assert c.b == 2
     assert c.c == 3
-
-
-def test_get_config():
-    ret = get_config(None)
-    assert ret == {}
-    assert isinstance(ret, ConfigDict)
-
-    ret = get_config(ConfigDict(title='1234', extra=Extra.allow))
-    assert ret == {'title': '1234', 'extra': Extra.allow}
-    assert isinstance(ret, ConfigDict)
-
-    class Config:
-        title = '1234'
-        random_option = True
-        strict = True
-
-    with pytest.warns(DeprecationWarning, match='is deprecated'):
-        ret = get_config(Config)
-        assert ret == {'title': '1234', 'random_option': True, 'strict': True}
-        assert isinstance(ret, ConfigDict)
```

### Comparing `pydantic-2.0a1/tests/test_fastapi_json_schema.py` & `pydantic-2.0a2/tests/test_fastapi_json_schema.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_forward_ref.py` & `pydantic-2.0a2/tests/test_forward_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -733,16 +733,16 @@
 class Foobar(BaseModel):
     x: int
     y: Optional[Foobar] = None
 """
     )
     f = module.Foobar(x=1, y={'x': 2})
     assert f.model_dump() == {'x': 1, 'y': {'x': 2, 'y': None}}
-    assert f.__fields_set__ == {'x', 'y'}
-    assert f.y.__fields_set__ == {'x'}
+    assert f.model_fields_set == {'x', 'y'}
+    assert f.y.model_fields_set == {'x'}
 
 
 def test_force_rebuild():
     class Foobar(BaseModel):
         b: int
 
     assert Foobar.__pydantic_model_complete__ is True
```

### Comparing `pydantic-2.0a1/tests/test_generics.py` & `pydantic-2.0a2/tests/test_generics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import gc
 import itertools
 import json
 import platform
+import re
 import sys
 from collections import deque
 from enum import Enum, IntEnum
-from pprint import pprint
 from typing import (
     Any,
     Callable,
     ClassVar,
     Counter,
     DefaultDict,
     Deque,
@@ -52,15 +52,15 @@
     iter_contained_typevars,
     recursively_defined_type_refs,
     replace_types,
 )
 from pydantic.decorators import field_validator
 
 
-@pytest.fixture(autouse=True)
+@pytest.fixture()
 def clean_cache():
     # cleans up _GENERIC_TYPES_CACHE for checking item counts in the cache
     _GENERIC_TYPES_CACHE.clear()
     gc.collect(0)
     gc.collect(1)
     gc.collect(2)
 
@@ -296,15 +296,15 @@
     error_message = str(exc_info.value)
     assert error_message.startswith('Too many parameters') or error_message.startswith('Too many arguments')
     assert error_message.endswith(
         " for <class 'tests.test_generics.test_parameter_count.<locals>.Model'>; actual 3, expected 2"
     )
 
 
-def test_cover_cache():
+def test_cover_cache(clean_cache):
     cache_size = len(_GENERIC_TYPES_CACHE)
     T = TypeVar('T')
 
     class Model(BaseModel, Generic[T]):
         x: T
 
     models = []  # keep references to models to get cache size
@@ -312,15 +312,15 @@
     models.append(Model[int])  # adds both with-tuple and without-tuple version to cache
     assert len(_GENERIC_TYPES_CACHE) == cache_size + 3
     models.append(Model[int])  # uses the cache
     assert len(_GENERIC_TYPES_CACHE) == cache_size + 3
     del models
 
 
-def test_cache_keys_are_hashable():
+def test_cache_keys_are_hashable(clean_cache):
     cache_size = len(_GENERIC_TYPES_CACHE)
     T = TypeVar('T')
     C = Callable[[str, Dict[str, Any]], Iterable[str]]
 
     class MyGenericModel(BaseModel, Generic[T]):
         t: T
 
@@ -344,15 +344,15 @@
 
     models.append(Model)
     assert len(_GENERIC_TYPES_CACHE) == cache_size + 15
     del models
 
 
 @pytest.mark.skipif(platform.python_implementation() == 'PyPy', reason='PyPy does not play nice with PyO3 gc')
-def test_caches_get_cleaned_up():
+def test_caches_get_cleaned_up(clean_cache):
     initial_types_cache_size = len(_GENERIC_TYPES_CACHE)
     T = TypeVar('T')
 
     class MyGenericModel(BaseModel, Generic[T]):
         x: T
 
         model_config = dict(arbitrary_types_allowed=True)
@@ -371,15 +371,15 @@
     gc.collect(0)
     gc.collect(1)
     gc.collect(2)
     assert len(_GENERIC_TYPES_CACHE) < initial_types_cache_size + _LIMITED_DICT_SIZE
 
 
 @pytest.mark.skipif(platform.python_implementation() == 'PyPy', reason='PyPy does not play nice with PyO3 gc')
-def test_caches_get_cleaned_up_with_aliased_parametrized_bases():
+def test_caches_get_cleaned_up_with_aliased_parametrized_bases(clean_cache):
     types_cache_size = len(_GENERIC_TYPES_CACHE)
 
     def run() -> None:  # Run inside nested function to get classes in local vars cleaned also
         T1 = TypeVar('T1')
         T2 = TypeVar('T2')
 
         class A(BaseModel, Generic[T1, T2]):
@@ -397,15 +397,15 @@
 
     gc.collect(0)
     gc.collect(1)
     gc.collect(2)
     assert len(_GENERIC_TYPES_CACHE) < types_cache_size + _LIMITED_DICT_SIZE
 
 
-def test_generics_work_with_many_parametrized_base_models():
+def test_generics_work_with_many_parametrized_base_models(clean_cache):
     cache_size = len(_GENERIC_TYPES_CACHE)
     count_create_models = 1000
     T = TypeVar('T')
     C = TypeVar('C')
 
     class A(BaseModel, Generic[T, C]):
         x: T
@@ -633,15 +633,15 @@
     class OuterT_SameType(BaseModel, Generic[AT]):
         i: InnerT[AT]
 
     OuterT_SameType[int](i={'a': 8})
     OuterT_SameType[int](i=inner_int)
     OuterT_SameType[str](i=inner_str)
     # TODO: The next line is failing, but passes in v1.
-    #   Might need to do something smart for Any, or re-parse-from-dict if the __pydantic_generic_origin__ is the same..
+    #   Might need to do something smart for Any, or re-parse-from-dict if the pydantic_generic_origin is the same..
     # OuterT_SameType[str](i=inner_int_any)
     OuterT_SameType[int](i=inner_int_any.model_dump())
 
     with pytest.raises(ValidationError) as exc_info:
         OuterT_SameType[int](i=inner_str.model_dump())
     assert exc_info.value.errors() == [
         {
@@ -700,18 +700,18 @@
     BT = TypeVar('BT')
 
     class Model(BaseModel, Generic[AT, BT]):
         a: List[AT]
         b: List[BT]
 
     partial_model = Model[int, BT]
-    assert partial_model.__pydantic_generic_parameters__
+    assert partial_model.__pydantic_generic_metadata__['parameters']
     concrete_model = partial_model[int]
 
-    assert not concrete_model.__pydantic_generic_parameters__
+    assert not concrete_model.__pydantic_generic_metadata__['parameters']
 
     # nested resolution of partial models should work as expected
     nested_resolved = concrete_model(a=['123'], b=['456'])
     assert nested_resolved.a == [123]
     assert nested_resolved.b == [456]
 
 
@@ -1237,29 +1237,29 @@
     generic_model = OuterModel[inner_model, NormalModel, int]
 
     inner_models = [inner_model(c=1, d='a')]
     generic_model(a={1: inner_models, 2: None}, b=None, c=1, d=1.5)
     generic_model(a={}, b=NormalModel(e=1, f='a'), c=1, d=1.5)
     generic_model(a={}, b=1, c=1, d=1.5)
 
-    assert InnerModel.__pydantic_generic_parameters__  # i.e., InnerModel is not concrete
-    assert not inner_model.__pydantic_generic_parameters__  # i.e., inner_model is concrete
+    assert InnerModel.__pydantic_generic_metadata__['parameters']  # i.e., InnerModel is not concrete
+    assert not inner_model.__pydantic_generic_metadata__['parameters']  # i.e., inner_model is concrete
 
 
 def test_deep_generic_with_inner_typevar():
     T = TypeVar('T')
 
     class OuterModel(BaseModel, Generic[T]):
         a: List[T]
 
     class InnerModel(OuterModel[T], Generic[T]):
         pass
 
-    assert not InnerModel[int].__pydantic_generic_parameters__  # i.e., InnerModel[int] is concrete
-    assert InnerModel.__pydantic_generic_parameters__  # i.e., InnerModel is not concrete
+    assert not InnerModel[int].__pydantic_generic_metadata__['parameters']  # i.e., InnerModel[int] is concrete
+    assert InnerModel.__pydantic_generic_metadata__['parameters']  # i.e., InnerModel is not concrete
 
     with pytest.raises(ValidationError):
         InnerModel[int](a=['wrong'])
     assert InnerModel[int](a=['1']).a == [1]
 
 
 def test_deep_generic_with_referenced_generic():
@@ -1271,16 +1271,16 @@
 
     class OuterModel(BaseModel, Generic[T]):
         a: ReferencedModel[T]
 
     class InnerModel(OuterModel[T], Generic[T]):
         pass
 
-    assert not InnerModel[int].__pydantic_generic_parameters__
-    assert InnerModel.__pydantic_generic_parameters__
+    assert not InnerModel[int].__pydantic_generic_metadata__['parameters']
+    assert InnerModel.__pydantic_generic_metadata__['parameters']
 
     with pytest.raises(ValidationError):
         InnerModel[int](a={'a': 'wrong'})
     assert InnerModel[int](a={'a': 1}).a.a == 1
 
 
 def test_deep_generic_with_referenced_inner_generic():
@@ -1291,16 +1291,16 @@
 
     class OuterModel(BaseModel, Generic[T]):
         a: Optional[List[Union[ReferencedModel[T], str]]]
 
     class InnerModel(OuterModel[T], Generic[T]):
         pass
 
-    assert not InnerModel[int].__pydantic_generic_parameters__
-    assert InnerModel.__pydantic_generic_parameters__
+    assert not InnerModel[int].__pydantic_generic_metadata__['parameters']
+    assert InnerModel.__pydantic_generic_metadata__['parameters']
 
     with pytest.raises(ValidationError):
         InnerModel[int](a=['s', {'a': 'wrong'}])
     assert InnerModel[int](a=['s', {'a': 1}]).a[1].a == 1
 
     assert InnerModel[int].model_fields['a'].annotation == Optional[List[Union[ReferencedModel[int], str]]]
 
@@ -1394,30 +1394,30 @@
 def test_generic_with_callable():
     T = TypeVar('T')
 
     class Model(BaseModel, Generic[T]):
         # Callable is a test for any type that accepts a list as an argument
         some_callable: Callable[[Optional[int], T], None]
 
-    assert not Model[str].__pydantic_generic_parameters__
-    assert Model.__pydantic_generic_parameters__
+    assert not Model[str].__pydantic_generic_metadata__['parameters']
+    assert Model.__pydantic_generic_metadata__['parameters']
 
 
 def test_generic_with_partial_callable():
     T = TypeVar('T')
     U = TypeVar('U')
 
     class Model(BaseModel, Generic[T, U]):
         t: T
         u: U
         # Callable is a test for any type that accepts a list as an argument
         some_callable: Callable[[Optional[int], str], None]
 
-    assert Model[str, U].__pydantic_generic_parameters__ == (U,)
-    assert not Model[str, int].__pydantic_generic_parameters__
+    assert Model[str, U].__pydantic_generic_metadata__['parameters'] == (U,)
+    assert not Model[str, int].__pydantic_generic_metadata__['parameters']
 
 
 def test_generic_recursive_models(create_module):
     @create_module
     def module():
         from typing import Generic, TypeVar, Union
 
@@ -1893,14 +1893,32 @@
         ...
 
     assert B[int, str].__name__ == 'B[int, str]', B[int, str].__name__
     assert issubclass(B[str, int], B)
     assert issubclass(B[str, int], A)
 
 
+def test_generic_subclass_with_extra_type_requires_all_params():
+    T = TypeVar('T')
+    S = TypeVar('S')
+
+    class A(BaseModel, Generic[T]):
+        ...
+
+    with pytest.raises(
+        TypeError,
+        match=re.escape(
+            'All parameters must be present on typing.Generic; you should inherit from typing.Generic[~T, ~S]'
+        ),
+    ):
+
+        class B(A[T], Generic[S]):
+            ...
+
+
 def test_multi_inheritance_generic_binding():
     T = TypeVar('T')
 
     class A(BaseModel, Generic[T]):
         ...
 
     class B(A[int], Generic[T]):
@@ -1926,15 +1944,15 @@
 
     with pytest.raises(ValidationError) as exc_info:
         B[int](a='a', b=1)
     assert exc_info.value.errors() == [
         {
             'input': 'a',
             'loc': ('a',),
-            'msg': 'Input should be a valid integer, unable to parse string as an ' 'integer',
+            'msg': 'Input should be a valid integer, unable to parse string as an integer',
             'type': 'int_parsing',
         }
     ]
 
 
 def test_multi_inheritance_generic_defaults():
     T = TypeVar('T')
@@ -2047,15 +2065,14 @@
 
 def test_double_typevar_substitution() -> None:
     T = TypeVar('T')
 
     class GenericPydanticModel(BaseModel, Generic[T]):
         x: T = []
 
-    pprint(GenericPydanticModel[List[T]].__pydantic_core_schema__)
     assert GenericPydanticModel[List[T]](x=[1, 2, 3]).model_dump() == {'x': [1, 2, 3]}
 
 
 @pytest.fixture(autouse=True)
 def ensure_contextvar_gets_reset():
     # Ensure that the generic recursion contextvar is empty at the start of every test
     assert not recursively_defined_type_refs()
```

### Comparing `pydantic-2.0a1/tests/test_hypothesis_plugin.py` & `pydantic-2.0a2/tests/test_hypothesis_plugin.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_json.py` & `pydantic-2.0a2/tests/test_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -229,30 +229,14 @@
         @field_serializer('timedt')
         def serialize_timedt(self, _v: timedelta, _info):
             return 'child_encoder'
 
     assert Child().model_dump_json() == '{"dt":"parent_encoder","timedt":"child_encoder"}'
 
 
-def test_json_encoder_inheritance_override():
-    class Parent(BaseModel):
-        dt: datetime = datetime.now()
-
-        @field_serializer('dt')
-        def serialize_dt(self, _v: datetime, _info):
-            return 'parent_encoder'
-
-    class Child(Parent):
-        @field_serializer('dt')
-        def serialize_dt(self, _v: datetime, _info):
-            return 'child_encoder'
-
-    assert Child().model_dump_json() == '{"dt":"child_encoder"}'
-
-
 def test_encode_dataclass():
     @vanilla_dataclass
     class Foo:
         bar: int
         spam: str
 
     f = Foo(bar=123, spam='apple pie')
```

### Comparing `pydantic-2.0a1/tests/test_json_schema.py` & `pydantic-2.0a2/tests/test_json_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 import pytest
 from pydantic_core import core_schema
 from typing_extensions import Annotated, Literal
 
 from pydantic import (
     BaseModel,
-    Extra,
     Field,
     ImportString,
     ValidationError,
     field_validator,
 )
 from pydantic._internal._core_metadata import build_metadata_dict
 from pydantic._internal._generate_schema import GenerateSchema
@@ -1923,15 +1922,15 @@
         'properties': {'color': {'title': 'Color', 'type': 'string', 'format': 'color'}},
         'required': ['color'],
     }
 
 
 def test_model_with_extra_forbidden():
     class Model(BaseModel):
-        model_config = ConfigDict(extra=Extra.forbid)
+        model_config = ConfigDict(extra='forbid')
         a: str
 
     assert Model.model_json_schema() == {
         'title': 'Model',
         'type': 'object',
         'properties': {'a': {'title': 'A', 'type': 'string'}},
         'required': ['a'],
```

### Comparing `pydantic-2.0a1/tests/test_main.py` & `pydantic-2.0a2/tests/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,22 +20,22 @@
     Type,
     TypeVar,
     get_type_hints,
 )
 from uuid import UUID, uuid4
 
 import pytest
-from typing_extensions import Final, Literal
+from typing_extensions import Annotated, Final, Literal
 
 from pydantic import (
     BaseModel,
     ConfigDict,
-    Extra,
     Field,
     PrivateAttr,
+    PydanticUndefinedAnnotation,
     PydanticUserError,
     SecretStr,
     ValidationError,
     ValidationInfo,
     constr,
 )
 from pydantic.decorators import field_validator
@@ -213,40 +213,56 @@
             'input': None,
         },
     ]
 
 
 def test_allow_extra():
     class Model(BaseModel):
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
         a: float = ...
 
-    assert Model(a='10.2', b=12).model_dump() == {'a': 10.2, 'b': 12}
+    assert Model(a='10.2', b=12).b == 12
+
+
+@pytest.mark.parametrize('extra', ['ignore', 'forbid', 'allow'])
+def test_allow_extra_from_attributes(extra: Literal['ignore', 'forbid', 'allow']):
+    class Model(BaseModel):
+        a: float
+
+        model_config = ConfigDict(extra=extra, from_attributes=True)
+
+    class TestClass:
+        a = 1.0
+        b = 12
+
+    m = Model.model_validate(TestClass())
+    assert m.a == 1.0
+    assert not hasattr(m, 'b')
 
 
 def test_allow_extra_repr():
     class Model(BaseModel):
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
         a: float = ...
 
     assert str(Model(a='10.2', b=12)) == 'a=10.2 b=12'
 
 
 def test_forbidden_extra_success():
     class ForbiddenExtra(BaseModel):
-        model_config = ConfigDict(extra=Extra.forbid)
+        model_config = ConfigDict(extra='forbid')
         foo: str = 'whatever'
 
     m = ForbiddenExtra()
     assert m.foo == 'whatever'
 
 
 def test_forbidden_extra_fails():
     class ForbiddenExtra(BaseModel):
-        model_config = ConfigDict(extra=Extra.forbid)
+        model_config = ConfigDict(extra='forbid')
         foo: str = 'whatever'
 
     with pytest.raises(ValidationError) as exc_info:
         ForbiddenExtra(foo='ok', bar='wrong', spam='xx')
     assert exc_info.value.errors() == [
         {
             'type': 'extra_forbidden',
@@ -281,29 +297,29 @@
     model = Model(a=0.2)
     with pytest.raises(ValidationError, match=r"b\s+Object has no attribute 'b'"):
         model.b = 2
 
 
 def test_extra_allowed():
     class Model(BaseModel):
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
         a: float
 
     model = Model(a=0.2, b=0.1)
     assert model.b == 0.1
 
     assert not hasattr(model, 'c')
     model.c = 1
     assert hasattr(model, 'c')
     assert model.c == 1
 
 
 def test_extra_ignored():
     class Model(BaseModel):
-        model_config = ConfigDict(extra=Extra.ignore)
+        model_config = ConfigDict(extra='ignore')
         a: float
 
     model = Model(a=0.2, b=0.1)
     assert not hasattr(model, 'b')
 
     with pytest.raises(ValueError, match='"Model" object has no field "c"'):
         model.c = 1
@@ -378,26 +394,26 @@
     assert exc_info.value.errors() == [{'type': 'missing', 'loc': ('a',), 'msg': 'Field required', 'input': {}}]
 
 
 def test_mutability():
     class TestModel(BaseModel):
         a: int = 10
 
-        model_config = ConfigDict(extra=Extra.forbid, frozen=False)
+        model_config = ConfigDict(extra='forbid', frozen=False)
 
     m = TestModel()
 
     assert m.a == 10
     m.a = 11
     assert m.a == 11
 
 
 def test_frozen_model():
     class FrozenModel(BaseModel):
-        model_config = ConfigDict(extra=Extra.forbid, frozen=True)
+        model_config = ConfigDict(extra='forbid', frozen=True)
 
         a: int = 10
 
     m = FrozenModel()
 
     assert m.a == 10
     with pytest.raises(TypeError) as exc_info:
@@ -745,21 +761,21 @@
 
 def test_fields_set():
     class MyModel(BaseModel):
         a: int
         b: int = 2
 
     m = MyModel(a=5)
-    assert m.__fields_set__ == {'a'}
+    assert m.model_fields_set == {'a'}
 
     m.b = 2
-    assert m.__fields_set__ == {'a', 'b'}
+    assert m.model_fields_set == {'a', 'b'}
 
     m = MyModel(a=5, b=2)
-    assert m.__fields_set__ == {'a', 'b'}
+    assert m.model_fields_set == {'a', 'b'}
 
 
 def test_exclude_unset_dict():
     class MyModel(BaseModel):
         a: int
         b: int = 2
 
@@ -850,15 +866,15 @@
     assert 'model_dump_json' in dir(m)
     assert 'attribute_a' in dir(m)
     assert 'attribute_b' in dir(m)
 
 
 def test_dict_with_extra_keys():
     class MyModel(BaseModel):
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
         a: str = Field(None, alias='alias_a')
 
     m = MyModel(extra_key='extra')
     assert m.model_dump() == {'a': None, 'extra_key': 'extra'}
     assert m.model_dump(by_alias=True) == {'alias_a': None, 'extra_key': 'extra'}
 
 
@@ -1311,16 +1327,16 @@
 
 
 def test_untyped_fields_warning():
     with pytest.raises(
         PydanticUserError,
         match=re.escape(
             "A non-annotated attribute was detected: `x = 1`. All model fields require a type annotation; "
-            "if 'x' is not meant to be a field, you may be able to resolve this error by annotating it "
-            "as a ClassVar or updating model_config[\"ignored_types\"]."
+            "if `x` is not meant to be a field, you may be able to resolve this error by annotating it "
+            "as a `ClassVar` or updating `model_config['ignored_types']`."
         ),
     ):
 
         class WarningModel(BaseModel):
             x = 1
 
     # Prove that annotating with ClassVar prevents the warning
@@ -1492,30 +1508,30 @@
 def test_base_config_type_hinting():
     class M(BaseModel):
         a: int
 
     get_type_hints(type(M.model_config))
 
 
-@pytest.mark.xfail(reason='frozen field; https://github.com/pydantic/pydantic-core/pull/237')
 def test_frozen_field():
     """assigning a frozen=True field should raise a TypeError"""
 
     class Entry(BaseModel):
         model_config = ConfigDict(validate_assignment=True)
         id: float = Field(frozen=True)
         val: float
 
     r = Entry(id=1, val=100)
     assert r.val == 100
     r.val = 101
     assert r.val == 101
     assert r.id == 1
-    with pytest.raises(TypeError, match='"id" has frozen set to True and cannot be assigned'):
+    with pytest.raises(ValidationError) as exc_info:
         r.id = 2
+    assert exc_info.value.errors() == [{'input': 2, 'loc': ('id',), 'msg': 'Field is frozen', 'type': 'frozen_field'}]
 
 
 def test_repr_field():
     class Model(BaseModel):
         a: int = Field()
         b: float = Field(repr=True)
         c: bool = Field(repr=False)
@@ -1664,32 +1680,32 @@
     ]
 
 
 def test_class_kwargs_config():
     class Base(BaseModel, extra='forbid', alias_generator=str.upper):
         a: int
 
-    assert Base.model_config['extra'] is Extra.forbid
+    assert Base.model_config['extra'] == 'forbid'
     assert Base.model_config['alias_generator'] is str.upper
     # assert Base.model_fields['a'].alias == 'A'
 
     class Model(Base, extra='allow'):
         b: int
 
-    assert Model.model_config['extra'] is Extra.allow  # overwritten as intended
+    assert Model.model_config['extra'] == 'allow'  # overwritten as intended
     assert Model.model_config['alias_generator'] is str.upper  # inherited as intended
     # assert Model.model_fields['b'].alias == 'B'  # alias_generator still works
 
 
 def test_class_kwargs_config_and_attr_conflict():
     class Model(BaseModel, extra='allow', alias_generator=str.upper):
         model_config = ConfigDict(extra='forbid', title='Foobar')
         b: int
 
-    assert Model.model_config['extra'] is Extra.allow
+    assert Model.model_config['extra'] == 'allow'
     assert Model.model_config['alias_generator'] is str.upper
     assert Model.model_config['title'] == 'Foobar'
 
 
 def test_class_kwargs_custom_config():
     if platform.python_implementation() == 'PyPy':
         msg = r"__init_subclass__\(\) got an unexpected keyword argument 'some_config'"
@@ -1715,15 +1731,14 @@
     #     'title': 'Model',
     #     'type': 'object',
     #     'properties': {'x': {'title': 'X', 'anyOf': [{'type': 'integer'}, {'type': 'string'}]}},
     #     'required': ['x'],
     # }
 
 
-@pytest.mark.xfail(reason='implement final')
 @pytest.mark.parametrize(
     'ann',
     [Final, Final[int]],
     ids=['no-arg', 'with-arg'],
 )
 @pytest.mark.parametrize(
     'value',
@@ -1733,90 +1748,151 @@
 def test_final_field_decl_without_default_val(ann, value):
     class Model(BaseModel):
         a: ann
 
         if value is not None:
             a = value
 
-    Model.model_rebuild(ann=ann)
-
     assert 'a' not in Model.__class_vars__
     assert 'a' in Model.model_fields
 
     assert Model.model_fields['a'].final
 
 
-@pytest.mark.xfail(reason='waiting for https://github.com/pydantic/pydantic-core/pull/237')
 @pytest.mark.parametrize(
     'ann',
     [Final, Final[int]],
     ids=['no-arg', 'with-arg'],
 )
 def test_final_field_decl_with_default_val(ann):
     class Model(BaseModel):
         a: ann = 10
 
-    Model.model_rebuild(ann=ann)
-
     assert 'a' in Model.__class_vars__
     assert 'a' not in Model.model_fields
 
 
-@pytest.mark.xfail(reason='waiting for https://github.com/pydantic/pydantic-core/pull/237')
 def test_final_field_reassignment():
     class Model(BaseModel):
+        model_config = ConfigDict(validate_assignment=True)
+
         a: Final[int]
 
     obj = Model(a=10)
 
-    with pytest.raises(
-        TypeError,
-        match=r'^"Model" object "a" field is final and does not support reassignment$',
-    ):
+    with pytest.raises(ValidationError) as exc_info:
         obj.a = 20
+    assert exc_info.value.errors() == [{'input': 20, 'loc': ('a',), 'msg': 'Field is frozen', 'type': 'frozen_field'}]
 
 
-@pytest.mark.xfail(reason='waiting for https://github.com/pydantic/pydantic-core/pull/237')
 def test_field_by_default_is_not_final():
     class Model(BaseModel):
         a: int
 
     assert not Model.model_fields['a'].final
 
 
+def test_annotated_final():
+    class Model(BaseModel):
+        a: Annotated[Final[int], Field(title='abc')]
+
+    assert Model.model_fields['a'].final
+    assert Model.model_fields['a'].title == 'abc'
+
+    class Model2(BaseModel):
+        a: Final[Annotated[int, Field(title='def')]]
+
+    assert Model2.model_fields['a'].final
+    assert Model2.model_fields['a'].title == 'def'
+
+
 def test_post_init():
     calls = []
 
-    class SubModel(BaseModel):
+    class InnerModel(BaseModel):
         a: int
         b: int
 
-        def model_post_init(self, _context) -> None:
+        def model_post_init(self, __context) -> None:
+            super().model_post_init(__context)  # this is included just to show it doesn't error
             assert self.model_dump() == {'a': 3, 'b': 4}
-            calls.append('submodel_post_init')
+            calls.append('inner_model_post_init')
 
     class Model(BaseModel):
         c: int
         d: int
-        sub: SubModel
+        sub: InnerModel
 
-        def model_post_init(self, _context) -> None:
+        def model_post_init(self, __context) -> None:
             assert self.model_dump() == {'c': 1, 'd': 2, 'sub': {'a': 3, 'b': 4}}
             calls.append('model_post_init')
 
     m = Model(c=1, d='2', sub={'a': 3, 'b': '4'})
+    assert calls == ['inner_model_post_init', 'model_post_init']
     assert m.model_dump() == {'c': 1, 'd': 2, 'sub': {'a': 3, 'b': 4}}
-    assert calls == ['submodel_post_init', 'model_post_init']
 
+    class SubModel(Model):
+        def model_post_init(self, __context) -> None:
+            assert self.model_dump() == {'c': 1, 'd': 2, 'sub': {'a': 3, 'b': 4}}
+            super().model_post_init(__context)
+            calls.append('submodel_post_init')
 
-def test_extra_args_to_field_type_error():
-    with pytest.raises(TypeError, match='unexpected keyword argument'):
+    calls.clear()
+    m = SubModel(c=1, d='2', sub={'a': 3, 'b': '4'})
+    assert calls == ['inner_model_post_init', 'model_post_init', 'submodel_post_init']
+    assert m.model_dump() == {'c': 1, 'd': 2, 'sub': {'a': 3, 'b': 4}}
 
-        class Model(BaseModel):
-            a: int = Field(thing=1)
+
+@pytest.mark.parametrize('include_private_attribute', [True, False])
+def test_post_init_call_signatures(include_private_attribute):
+    calls = []
+
+    class Model(BaseModel):
+        a: int
+        b: int
+        if include_private_attribute:
+            _x: int = PrivateAttr(1)
+
+        def model_post_init(self, *args, **kwargs) -> None:
+            calls.append((args, kwargs))
+
+    Model(a=1, b=2)
+    assert calls == [((None,), {})]
+    Model.model_construct(a=3, b=4)
+    assert calls == [((None,), {}), ((None,), {})]
+
+
+def test_post_init_not_called_without_override():
+    calls = []
+
+    def monkey_patched_model_post_init(cls, __context):
+        calls.append('BaseModel.model_post_init')
+
+    original_base_model_post_init = BaseModel.model_post_init
+    try:
+        BaseModel.model_post_init = monkey_patched_model_post_init
+
+        class WithoutOverrideModel(BaseModel):
+            pass
+
+        WithoutOverrideModel()
+        WithoutOverrideModel.model_construct()
+        assert calls == []
+
+        class WithOverrideModel(BaseModel):
+            def model_post_init(self, __context: Any) -> None:
+                calls.append('WithOverrideModel.model_post_init')
+
+        WithOverrideModel()
+        assert calls == ['WithOverrideModel.model_post_init']
+        WithOverrideModel.model_construct()
+        assert calls == ['WithOverrideModel.model_post_init', 'WithOverrideModel.model_post_init']
+
+    finally:
+        BaseModel.model_post_init = original_base_model_post_init
 
 
 def test_deeper_recursive_model():
     class A(BaseModel, undefined_types_warning=False):
         b: 'B'
 
     class B(BaseModel, undefined_types_warning=False):
@@ -1829,14 +1905,34 @@
     B.model_rebuild()
     C.model_rebuild()
 
     m = A(b=B(c=C(a=None)))
     assert m.model_dump() == {'b': {'c': {'a': None}}}
 
 
+def test_model_rebuild_localns():
+    class A(BaseModel, undefined_types_warning=False):
+        x: int
+
+    class B(BaseModel, undefined_types_warning=False):
+        a: 'Model'  # noqa F821
+
+    B.model_rebuild(_types_namespace={'Model': A})
+
+    m = B(a={'x': 1})
+    assert m.model_dump() == {'a': {'x': 1}}
+    assert isinstance(m.a, A)
+
+    class C(BaseModel, undefined_types_warning=False):
+        a: 'Model'  # noqa F821
+
+    with pytest.raises(PydanticUndefinedAnnotation, match="name 'Model' is not defined"):
+        C.model_rebuild(_types_namespace={'A': A})
+
+
 @pytest.fixture(scope='session', name='InnerEqualityModel')
 def inner_equality_fixture():
     class InnerEqualityModel(BaseModel):
         iw: int
         ix: int = 0
         _iy: int = PrivateAttr()
         _iz: int = PrivateAttr(0)
@@ -1885,15 +1981,15 @@
     assert model != dict(model)
     assert dict(model) != model.model_dump()  # Due to presence of inner model
 
 
 def test_model_equality_fields_set(InnerEqualityModel):
     m1 = InnerEqualityModel(iw=0)
     m2 = InnerEqualityModel(iw=0, ix=0)
-    assert m1.__fields_set__ != m2.__fields_set__
+    assert m1.model_fields_set != m2.model_fields_set
     assert m1 == m2
 
 
 def test_model_equality_private_attrs(InnerEqualityModel):
     m = InnerEqualityModel(iw=0, ix=0)
 
     m1 = m.model_copy()
@@ -2056,7 +2152,29 @@
             assert info.context == contexts.pop(0)
             return v
 
     Model.model_validate_json(json.dumps({'x': 1}))
     Model.model_validate_json(json.dumps({'x': 1}), context=None)
     Model.model_validate_json(json.dumps({'x': 1}), context={'foo': 'bar'})
     assert contexts == []
+
+
+def test_pydantic_init_subclass() -> None:
+    calls = []
+
+    class MyModel(BaseModel):
+        def __init_subclass__(cls, **kwargs):
+            super().__init_subclass__()  # can't pass kwargs to object.__init_subclass__, weirdly
+            calls.append((cls.__name__, '__init_subclass__', kwargs))
+
+        @classmethod
+        def __pydantic_init_subclass__(cls, **kwargs):
+            super().__pydantic_init_subclass__(**kwargs)
+            calls.append((cls.__name__, '__pydantic_init_subclass__', kwargs))
+
+    class MySubModel(MyModel, a=1):
+        pass
+
+    assert calls == [
+        ('MySubModel', '__init_subclass__', {'a': 1}),
+        ('MySubModel', '__pydantic_init_subclass__', {'a': 1}),
+    ]
```

### Comparing `pydantic-2.0a1/tests/test_model_signature.py` & `pydantic-2.0a2/tests/test_model_signature.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from inspect import Parameter, Signature, signature
 from typing import Any, Iterable, Optional, Union
 
 import pytest
 from typing_extensions import Annotated
 
-from pydantic import BaseModel, ConfigDict, Extra, Field, create_model
+from pydantic import BaseModel, ConfigDict, Field, create_model
 from pydantic._internal._typing_extra import is_annotated
 
 
 def _equals(a: Union[str, Iterable[str]], b: Union[str, Iterable[str]]) -> bool:
     """
     compare strings with spaces removed
     """
@@ -34,15 +34,15 @@
 
 def test_custom_init_signature():
     class MyModel(BaseModel):
         id: int
         name: str = 'John Doe'
         f__: str = Field(..., alias='foo')
 
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
 
         def __init__(self, id: int = 1, bar=2, *, baz: Any, **data):
             super().__init__(id=id, **data)
             self.bar = bar
             self.baz = baz
 
     sig = signature(MyModel)
@@ -59,15 +59,15 @@
         a: float
         b: int = 2
         c: int
 
         def __init__(self, a: float, b: int):
             super().__init__(a=a, b=b, c=1)
 
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
 
     assert _equals(str(signature(Model)), '(a: float, b: int) -> None')
 
 
 def test_invalid_identifiers_signature():
     model = create_model(
         'Model',
@@ -96,46 +96,46 @@
     assert _equals(str(signature(Foo)), '(*, from_: str) -> None')
 
 
 def test_extra_allow_no_conflict():
     class Model(BaseModel):
         spam: str
 
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
 
     assert _equals(str(signature(Model)), '(*, spam: str, **extra_data: Any) -> None')
 
 
 def test_extra_allow_conflict():
     class Model(BaseModel):
         extra_data: str
 
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
 
     assert _equals(str(signature(Model)), '(*, extra_data: str, **extra_data_: Any) -> None')
 
 
 def test_extra_allow_conflict_twice():
     class Model(BaseModel):
         extra_data: str
         extra_data_: str
 
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
 
     assert _equals(str(signature(Model)), '(*, extra_data: str, extra_data_: str, **extra_data__: Any) -> None')
 
 
 def test_extra_allow_conflict_custom_signature():
     class Model(BaseModel):
         extra_data: int
 
         def __init__(self, extra_data: int = 1, **foobar: Any):
             super().__init__(extra_data=extra_data, **foobar)
 
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
 
     assert _equals(str(signature(Model)), '(extra_data: int = 1, **foobar: Any) -> None')
 
 
 def test_signature_is_class_only():
     class Model(BaseModel):
         foo: int = 123
```

### Comparing `pydantic-2.0a1/tests/test_networks.py` & `pydantic-2.0a2/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_networks_ipaddress.py` & `pydantic-2.0a2/tests/test_networks_ipaddress.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
         ('192.168.0.0/24', IPv4Interface),
         ('192.168.0.1/24', IPv4Interface),
         ('192.168.128.0/30', IPv4Interface),
         ('192.168.128.1/30', IPv4Interface),
         ('2001:db00::0/120', IPv6Interface),
         ('2001:db00::1/120', IPv6Interface),
         (2**32 - 1, IPv4Interface),  # no mask equals to mask /32
-        (2**32 - 1, IPv4Interface),  # so ``strict`` has no effect
+        (2**32 - 1, IPv4Interface),  # so `strict` has no effect
         (20_282_409_603_651_670_423_947_251_286_015, IPv6Interface),  # /128
         (20_282_409_603_651_670_423_947_251_286_014, IPv6Interface),
         (b'\xff\xff\xff\xff', IPv4Interface),  # /32
         (b'\xff\xff\xff\xff', IPv4Interface),
         (b'\x00\x00\x00\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff', IPv6Interface),
         (b'\x00\x00\x00\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff\xff', IPv6Interface),
         (('192.168.0.0', 24), IPv4Interface),
@@ -386,15 +386,15 @@
     'value,cls',
     [
         ('192.168.0.0/24', IPv4Interface),
         ('192.168.0.1/24', IPv4Interface),
         ('192.168.128.0/30', IPv4Interface),
         ('192.168.128.1/30', IPv4Interface),
         (2**32 - 1, IPv4Interface),  # no mask equals to mask /32
-        (2**32 - 1, IPv4Interface),  # so ``strict`` has no effect
+        (2**32 - 1, IPv4Interface),  # so `strict` has no effect
         (b'\xff\xff\xff\xff', IPv4Interface),  # /32
         (b'\xff\xff\xff\xff', IPv4Interface),
         (('192.168.0.0', 24), IPv4Interface),
         (('192.168.0.1', 24), IPv4Interface),
         (IPv4Interface('192.168.0.0/24'), IPv4Interface),
         (IPv4Interface('192.168.0.1/24'), IPv4Interface),
     ],
```

### Comparing `pydantic-2.0a1/tests/test_parse.py` & `pydantic-2.0a2/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_private_attributes.py` & `pydantic-2.0a2/tests/test_private_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import platform
 from typing import ClassVar, Generic, TypeVar
 
 import pytest
 
-from pydantic import BaseModel, ConfigDict, Extra, PrivateAttr
+from pydantic import BaseModel, ConfigDict, PrivateAttr
 from pydantic.fields import Undefined
 
 
 def test_private_attribute():
     default = {'a': {}}
 
     class Model(BaseModel):
@@ -137,15 +137,15 @@
         m._bar = 1
 
 
 def test_private_attribute_intersection_with_extra_field():
     class Model(BaseModel):
         _foo = PrivateAttr('private_attribute')
 
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
 
     assert Model.__slots__ == {'_foo'}
     m = Model(_foo='field')
     assert m._foo == 'private_attribute'
     assert m.__dict__ == m.model_dump() == {'_foo': 'field'}
 
     m._foo = 'still_private'
```

### Comparing `pydantic-2.0a1/tests/test_rich_repr.py` & `pydantic-2.0a2/tests/test_rich_repr.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_serialize.py` & `pydantic-2.0a2/tests/test_serialize.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 New tests for v2 of serialization logic.
 """
+import json
+from functools import partial, partialmethod
 from typing import Any, Optional
 
 import pytest
 from pydantic_core import PydanticSerializationError, core_schema
 from typing_extensions import Annotated
 
 from pydantic import (
@@ -12,14 +14,110 @@
     Field,
     FieldSerializationInfo,
     SerializationInfo,
     SerializerFunctionWrapHandler,
     field_serializer,
     model_serializer,
 )
+from pydantic.annotated_arguments import PlainSerializer, WrapSerializer
+from pydantic.config import ConfigDict
+
+
+def test_serialize_extra_allow() -> None:
+    class Model(BaseModel):
+        x: int
+        model_config = ConfigDict(extra='allow')
+
+    m = Model(x=1, y=2)
+    assert m.y == 2
+    assert m.model_dump() == {'x': 1, 'y': 2}
+    assert json.loads(m.model_dump_json()) == {'x': 1, 'y': 2}
+
+
+def test_serialize_extra_allow_subclass_1() -> None:
+    class Parent(BaseModel):
+        x: int
+
+    class Child(Parent):
+        model_config = ConfigDict(extra='allow')
+
+    class Model(BaseModel):
+        inner: Parent
+
+    m = Model(inner=Child(x=1, y=2))
+    assert m.inner.y == 2
+    assert m.model_dump() == {'inner': {'x': 1}}
+    assert json.loads(m.model_dump_json()) == {'inner': {'x': 1}}
+
+
+def test_serialize_extra_allow_subclass_2() -> None:
+    class Parent(BaseModel):
+        x: int
+        model_config = ConfigDict(extra='allow')
+
+    class Child(Parent):
+        y: int
+
+    class Model(BaseModel):
+        inner: Parent
+
+    m = Model(inner=Child(x=1, y=2))
+    assert m.inner.y == 2
+    assert m.model_dump() == {'inner': {'x': 1, 'y': 2}}
+    assert json.loads(m.model_dump_json()) == {'inner': {'x': 1, 'y': 2}}
+
+
+def test_serializer_annotated_plain_always():
+    FancyInt = Annotated[int, PlainSerializer(lambda x: f'{x:,}', json_return_type='str')]
+
+    class MyModel(BaseModel):
+        x: FancyInt
+
+    assert MyModel(x=1234).model_dump() == {'x': '1,234'}
+    assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
+    assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
+
+
+def test_serializer_annotated_plain_json():
+    FancyInt = Annotated[int, PlainSerializer(lambda x: f'{x:,}', json_return_type='str', when_used='json')]
+
+    class MyModel(BaseModel):
+        x: FancyInt
+
+    assert MyModel(x=1234).model_dump() == {'x': 1234}
+    assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
+    assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
+
+
+def test_serializer_annotated_wrap_always():
+    def ser_wrap(v: Any, nxt: SerializerFunctionWrapHandler) -> Any:
+        return f'{nxt(v + 1):,}'
+
+    FancyInt = Annotated[int, WrapSerializer(ser_wrap, json_return_type='str')]
+
+    class MyModel(BaseModel):
+        x: FancyInt
+
+    assert MyModel(x=1234).model_dump() == {'x': '1,235'}
+    assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,235'}
+    assert MyModel(x=1234).model_dump_json() == '{"x":"1,235"}'
+
+
+def test_serializer_annotated_wrap_json():
+    def ser_wrap(v: Any, nxt: SerializerFunctionWrapHandler) -> Any:
+        return f'{nxt(v + 1):,}'
+
+    FancyInt = Annotated[int, WrapSerializer(ser_wrap, json_return_type='str', when_used='json')]
+
+    class MyModel(BaseModel):
+        x: FancyInt
+
+    assert MyModel(x=1234).model_dump() == {'x': 1234}
+    assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,235'}
+    assert MyModel(x=1234).model_dump_json() == '{"x":"1,235"}'
 
 
 def test_serialize_decorator_always():
     class MyModel(BaseModel):
         x: Optional[int]
 
         @field_serializer('x', json_return_type='str')
@@ -42,28 +140,28 @@
 
 
 def test_serialize_decorator_json():
     class MyModel(BaseModel):
         x: int
 
         @field_serializer('x', json_return_type='str', when_used='json')
-        def customise_x_serialisation(v, _info):
+        def customise_x_serialisation(v):
             return f'{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': 1234}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
 
 
 def test_serialize_decorator_unless_none():
     class MyModel(BaseModel):
         x: Optional[int]
 
         @field_serializer('x', when_used='unless-none')
-        def customise_x_serialisation(v, _info):
+        def customise_x_serialisation(v):
             return f'{v:,}'
 
     assert MyModel(x=1234).model_dump() == {'x': '1,234'}
     assert MyModel(x=None).model_dump() == {'x': None}
     assert MyModel(x=1234).model_dump(mode='json') == {'x': '1,234'}
     assert MyModel(x=None).model_dump(mode='json') == {'x': None}
     assert MyModel(x=1234).model_dump_json() == '{"x":"1,234"}'
@@ -133,64 +231,64 @@
         'f3': '3,000',
         'f4': '4,000',
     }
     assert m.model_dump_json() == '{"f1":"1,000","f2":"2,000","f3":"3,000","f4":"4,000"}'
 
 
 def test_invalid_signature_no_params() -> None:
-    with pytest.raises(TypeError, match='Unrecognized serializer signature'):
+    with pytest.raises(TypeError, match='Unrecognized field_serializer signature'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x')
             def no_args() -> Any:  # pragma: no cover
                 ...
 
 
 def test_invalid_signature_single_params() -> None:
-    with pytest.raises(TypeError, match='Unrecognized serializer signature'):
+    with pytest.raises(TypeError, match='Unrecognized field_serializer signature'):
 
         class _(BaseModel):
             x: int
 
             # not caught by type checkers
             @field_serializer('x')
             def no_args(self) -> Any:  # pragma: no cover
                 ...
 
 
 def test_invalid_signature_too_many_params_1() -> None:
-    with pytest.raises(TypeError, match='Unrecognized serializer signature'):
+    with pytest.raises(TypeError, match='Unrecognized field_serializer signature'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x')
             def no_args(self, value: Any, nxt: Any, info: Any, extra_param: Any) -> Any:  # pragma: no cover
                 ...
 
 
 def test_invalid_signature_too_many_params_2() -> None:
-    with pytest.raises(TypeError, match='Unrecognized serializer signature'):
+    with pytest.raises(TypeError, match='Unrecognized field_serializer signature'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x')
             @staticmethod
             def no_args(not_self: Any, value: Any, nxt: Any, info: Any) -> Any:  # pragma: no cover
                 ...
 
 
 def test_invalid_signature_bad_plain_signature() -> None:
-    with pytest.raises(TypeError, match='Unrecognized serializer signature for'):
+    with pytest.raises(TypeError, match='Unrecognized field_serializer signature for'):
 
         class _(BaseModel):
             x: int
 
             # caught by type checkers
             @field_serializer('x', mode='plain')
             def no_args(self, value: Any, nxt: Any, info: Any) -> Any:  # pragma: no cover
@@ -358,15 +456,18 @@
 
     msg = "^Error serializing to JSON: 'int' object cannot be converted to 'PyString'$"
     with pytest.raises(PydanticSerializationError, match=msg):
         m.model_dump_json()
 
 
 def test_model_serializer_wrong_args():
-    m = r'Unrecognized serializer signature for ' r'<.+MyModel._serialize at 0x\w+> with `mode=plain`:\(self, x, y, z\)'
+    m = (
+        r'Unrecognized model_serializer signature for '
+        r'<.+MyModel._serialize at 0x\w+> with `mode=plain`:\(self, x, y, z\)'
+    )
     with pytest.raises(TypeError, match=m):
 
         class MyModel(BaseModel):
             a: int
 
             @model_serializer
             def _serialize(self, x, y, z):
@@ -390,7 +491,259 @@
         class MyModel(BaseModel):
             a: int
 
             @model_serializer
             @classmethod
             def _serialize(self, x, y, z):
                 return self
+
+
+def test_field_multiple_serializer():
+    m = "Multiple field serializer functions were defined for field 'x', this is not allowed."
+    with pytest.raises(TypeError, match=m):
+
+        class MyModel(BaseModel):
+            x: int
+            y: int
+
+            @field_serializer('x', 'y', json_return_type='str')
+            def serializer1(v):
+                return f'{v:,}'
+
+            @field_serializer('x', json_return_type='str')
+            def serializer2(v):
+                return v
+
+
+def test_field_multiple_serializer_subclass():
+    class MyModel(BaseModel):
+        x: int
+
+        @field_serializer('x', json_return_type='str')
+        def serializer1(v):
+            return f'{v:,}'
+
+    class MySubModel(MyModel):
+        @field_serializer('x', json_return_type='str')
+        def serializer1(v):
+            return f'{v}'
+
+    assert MyModel(x=1234).model_dump() == {'x': '1,234'}
+    assert MySubModel(x=1234).model_dump() == {'x': '1234'}
+
+
+def int_ser_func_without_info1(v: int, expected: int) -> str:
+    return f'{v:,}'
+
+
+def int_ser_func_without_info2(v: int, *, expected: int) -> str:
+    return f'{v:,}'
+
+
+def int_ser_func_with_info1(v: int, info: FieldSerializationInfo, expected: int) -> str:
+    return f'{v:,}'
+
+
+def int_ser_func_with_info2(v: int, info: FieldSerializationInfo, *, expected: int) -> str:
+    return f'{v:,}'
+
+
+def int_ser_instance_method_without_info1(self: Any, v: int, *, expected: int) -> str:
+    assert self.x == v
+    return f'{v:,}'
+
+
+def int_ser_instance_method_without_info2(self: Any, v: int, expected: int) -> str:
+    assert self.x == v
+    return f'{v:,}'
+
+
+def int_ser_instance_method_with_info1(self: Any, v: int, info: FieldSerializationInfo, expected: int) -> str:
+    assert self.x == v
+    return f'{v:,}'
+
+
+def int_ser_instance_method_with_info2(self: Any, v: int, info: FieldSerializationInfo, *, expected: int) -> str:
+    assert self.x == v
+    return f'{v:,}'
+
+
+@pytest.mark.parametrize(
+    'func',
+    [
+        int_ser_func_with_info1,
+        int_ser_func_with_info2,
+        int_ser_func_without_info1,
+        int_ser_func_without_info2,
+        int_ser_instance_method_with_info1,
+        int_ser_instance_method_with_info2,
+        int_ser_instance_method_without_info1,
+        int_ser_instance_method_without_info2,
+    ],
+)
+def test_serialize_partial(
+    func: Any,
+):
+    class MyModel(BaseModel):
+        x: int
+
+        ser = field_serializer('x', json_return_type='str')(partial(func, expected=1234))
+
+    assert MyModel(x=1234).model_dump() == {'x': '1,234'}
+
+
+@pytest.mark.parametrize(
+    'func',
+    [
+        int_ser_func_with_info1,
+        int_ser_func_with_info2,
+        int_ser_func_without_info1,
+        int_ser_func_without_info2,
+        int_ser_instance_method_with_info1,
+        int_ser_instance_method_with_info2,
+        int_ser_instance_method_without_info1,
+        int_ser_instance_method_without_info2,
+    ],
+)
+def test_serialize_partialmethod(
+    func: Any,
+):
+    class MyModel(BaseModel):
+        x: int
+
+        ser = field_serializer('x', json_return_type='str')(partialmethod(func, expected=1234))
+
+    assert MyModel(x=1234).model_dump() == {'x': '1,234'}
+
+
+def test_serializer_allow_reuse_inheritance_override():
+    class Parent(BaseModel):
+        x: int
+
+        @field_serializer('x')
+        def ser_x(self, _v: int, _info: SerializationInfo) -> str:
+            return 'parent_encoder'
+
+    # overriding a serializer with a function / class var
+    # of the same name is allowed
+    # to mimick how inheritance works
+    # the serializer in the child class replaces the parent
+    # (without modifying the parent class itself)
+    class Child1(Parent):
+        @field_serializer('x')
+        def ser_x(self, _v: int, _info: SerializationInfo) -> str:
+            return 'child1_encoder' + ' ' + super().ser_x(_v, _info)
+
+    assert Parent(x=1).model_dump_json() == '{"x":"parent_encoder"}'
+    assert Child1(x=1).model_dump_json() == '{"x":"child1_encoder parent_encoder"}'
+
+    # defining an _different_ serializer on the other hand is not allowed
+    # because they would both "exist" thus causing confusion
+    # since it's not clear if both or just one will run
+    msg = 'Multiple field serializer functions were defined ' "for field 'x', this is not allowed."
+    with pytest.raises(TypeError, match=msg):
+
+        class _(Parent):
+            @field_serializer('x')
+            def ser_x_other(self, _v: int) -> str:
+                return 'err'
+
+    # the same thing applies if defined on the same class
+    with pytest.raises(TypeError, match=msg):
+
+        class _(BaseModel):
+            x: int
+
+            @field_serializer('x')
+            def ser_x(self, _v: int) -> str:
+                return 'parent_encoder'
+
+            @field_serializer('x')
+            def other_func_name(self, _v: int) -> str:
+                return 'parent_encoder'
+
+
+def test_serializer_allow_reuse_same_field():
+    with pytest.warns(UserWarning, match='`ser_x` overrides an existing Pydantic `@field_serializer` decorator'):
+
+        class Model(BaseModel):
+            x: int
+
+            @field_serializer('x')
+            def ser_x(self, _v: int) -> str:
+                return 'ser_1'
+
+            @field_serializer('x')
+            def ser_x(self, _v: int) -> str:  # noqa: F811
+                return 'ser_2'
+
+        assert Model(x=1).model_dump() == {'x': 'ser_2'}
+
+
+def test_serializer_allow_reuse_different_field_1():
+    with pytest.warns(UserWarning, match='`ser` overrides an existing Pydantic `@field_serializer` decorator'):
+
+        class Model(BaseModel):
+            x: int
+            y: int
+
+            @field_serializer('x')
+            def ser(self, _v: int) -> str:
+                return 'x'
+
+            @field_serializer('y')
+            def ser(self, _v: int) -> str:  # noqa: F811
+                return 'y'
+
+    assert Model(x=1, y=2).model_dump() == {'x': 1, 'y': 'y'}
+
+
+def test_serializer_allow_reuse_different_field_2():
+    with pytest.warns(UserWarning, match='`ser_x` overrides an existing Pydantic `@field_serializer` decorator'):
+
+        def ser(self: Any, _v: int, _info: Any) -> str:
+            return 'ser'
+
+        class Model(BaseModel):
+            x: int
+            y: int
+
+            @field_serializer('x')
+            def ser_x(self, _v: int) -> str:
+                return 'ser_x'
+
+            ser_x = field_serializer('y')(ser)  # noqa: F811
+
+    assert Model(x=1, y=2).model_dump() == {'x': 1, 'y': 'ser'}
+
+
+def test_serializer_allow_reuse_different_field_3():
+    with pytest.warns(UserWarning, match='`ser_x` overrides an existing Pydantic `@field_serializer` decorator'):
+
+        def ser1(self: Any, _v: int, _info: Any) -> str:
+            return 'ser1'
+
+        def ser2(self: Any, _v: int, _info: Any) -> str:
+            return 'ser2'
+
+        class Model(BaseModel):
+            x: int
+            y: int
+
+            ser_x = field_serializer('x')(ser1)
+            ser_x = field_serializer('y')(ser2)
+
+    assert Model(x=1, y=2).model_dump() == {'x': 1, 'y': 'ser2'}
+
+
+def test_serializer_allow_reuse_different_field_4():
+    def ser(self: Any, _v: int, _info: Any) -> str:
+        return f'{_v:,}'
+
+    class Model(BaseModel):
+        x: int
+        y: int
+
+        ser_x = field_serializer('x')(ser)
+        not_ser_x = field_serializer('y')(ser)
+
+    assert Model(x=1_000, y=2_000).model_dump() == {'x': '1,000', 'y': '2,000'}
```

### Comparing `pydantic-2.0a1/tests/test_strict.py` & `pydantic-2.0a2/tests/test_strict.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_structural_pattern_matching.py` & `pydantic-2.0a2/tests/test_structural_pattern_matching.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_tools.py` & `pydantic-2.0a2/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_types.py` & `pydantic-2.0a2/tests/test_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import itertools
 import math
 import os
 import re
 import sys
 import uuid
 from collections import OrderedDict, deque
-from datetime import date, datetime, time, timedelta
+from datetime import date, datetime, time, timedelta, timezone
 from decimal import Decimal
 from enum import Enum, IntEnum
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Deque,
@@ -36,41 +36,47 @@
 from typing_extensions import Annotated, Literal, TypedDict
 
 from pydantic import (
     UUID1,
     UUID3,
     UUID4,
     UUID5,
+    AwareDatetime,
     BaseModel,
     ByteSize,
     ConfigDict,
     DirectoryPath,
     EmailStr,
     Field,
     FilePath,
     FiniteFloat,
+    FutureDate,
     Json,
+    NaiveDatetime,
     NameEmail,
     NegativeFloat,
     NegativeInt,
+    NewPath,
     NonNegativeFloat,
     NonNegativeInt,
     NonPositiveFloat,
     NonPositiveInt,
+    PastDate,
     PositiveFloat,
     PositiveInt,
     SecretBytes,
     SecretStr,
     StrictBool,
     StrictBytes,
     StrictFloat,
     StrictInt,
     StrictStr,
     ValidationError,
     conbytes,
+    condate,
     condecimal,
     confloat,
     confrozenset,
     conint,
     conlist,
     conset,
     constr,
@@ -873,24 +879,126 @@
     ]
 
     v = Decimal(1.23)
     assert Model(v=v).v == v
     assert Model(v=v).model_dump() == {'v': v}
 
 
+def test_strict_date():
+    class Model(BaseModel):
+        v: Annotated[date, Field(strict=True)]
+
+    assert Model(v=date(2017, 5, 5)).v == date(2017, 5, 5)
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(v=datetime(2017, 5, 5))
+    assert exc_info.value.errors() == [
+        {
+            'type': 'date_type',
+            'loc': ('v',),
+            'msg': 'Input should be a valid date',
+            'input': datetime(2017, 5, 5),
+        }
+    ]
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(v='2017-05-05')
+    assert exc_info.value.errors() == [
+        {
+            'type': 'date_type',
+            'loc': ('v',),
+            'msg': 'Input should be a valid date',
+            'input': '2017-05-05',
+        }
+    ]
+
+
+def test_strict_datetime():
+    class Model(BaseModel):
+        v: Annotated[datetime, Field(strict=True)]
+
+    assert Model(v=datetime(2017, 5, 5, 10, 10, 10)).v == datetime(2017, 5, 5, 10, 10, 10)
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(v=date(2017, 5, 5))
+    assert exc_info.value.errors() == [
+        {
+            'type': 'datetime_type',
+            'loc': ('v',),
+            'msg': 'Input should be a valid datetime',
+            'input': date(2017, 5, 5),
+        }
+    ]
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(v='2017-05-05T10:10:10')
+    assert exc_info.value.errors() == [
+        {
+            'type': 'datetime_type',
+            'loc': ('v',),
+            'msg': 'Input should be a valid datetime',
+            'input': '2017-05-05T10:10:10',
+        }
+    ]
+
+
+def test_strict_time():
+    class Model(BaseModel):
+        v: Annotated[time, Field(strict=True)]
+
+    assert Model(v=time(10, 10, 10)).v == time(10, 10, 10)
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(v='10:10:10')
+    assert exc_info.value.errors() == [
+        {
+            'type': 'time_type',
+            'loc': ('v',),
+            'msg': 'Input should be a valid time',
+            'input': '10:10:10',
+        }
+    ]
+
+
+def test_strict_timedelta():
+    class Model(BaseModel):
+        v: Annotated[timedelta, Field(strict=True)]
+
+    assert Model(v=timedelta(days=1)).v == timedelta(days=1)
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(v='1 days')
+    assert exc_info.value.errors() == [
+        {
+            'type': 'time_delta_type',
+            'loc': ('v',),
+            'msg': 'Input should be a valid timedelta',
+            'input': '1 days',
+        }
+    ]
+
+
 @pytest.fixture(scope='session', name='CheckModel')
 def check_model_fixture():
     class CheckModel(BaseModel):
         bool_check: bool = True
         str_check: constr(strip_whitespace=True, max_length=10) = 's'
         bytes_check: bytes = b's'
         int_check: int = 1
         float_check: float = 1.0
         uuid_check: UUID = UUID('7bd00d58-6485-4ca6-b889-3da6d8df3ee4')
         decimal_check: condecimal(allow_inf_nan=False) = Decimal('42.24')
+        date_check: date = date(2017, 5, 5)
+        datetime_check: datetime = datetime(2017, 5, 5, 10, 10, 10)
+        time_check: time = time(10, 10, 10)
+        timedelta_check: timedelta = timedelta(days=1)
+        list_check: List[str] = ['1', '2']
+        tuple_check: Tuple[str, ...] = ('1', '2')
+        set_check: Set[str] = {'1', '2'}
+        frozenset_check: FrozenSet[str] = frozenset(['1', '2'])
 
     return CheckModel
 
 
 class BoolCastable:
     def __bool__(self) -> bool:
         return True
@@ -898,14 +1006,16 @@
 
 @pytest.mark.xfail(sys.platform.startswith('win'), reason='https://github.com/PyO3/pyo3/issues/2913', strict=False)
 @pytest.mark.parametrize(
     'field,value,result',
     [
         ('bool_check', True, True),
         ('bool_check', 1, True),
+        ('bool_check', 1.0, True),
+        ('bool_check', Decimal(1), True),
         ('bool_check', 'y', True),
         ('bool_check', 'Y', True),
         ('bool_check', 'yes', True),
         ('bool_check', 'Yes', True),
         ('bool_check', 'YES', True),
         ('bool_check', 'true', True),
         ('bool_check', 'True', True),
@@ -915,14 +1025,16 @@
         ('bool_check', 'ON', True),
         ('bool_check', '1', True),
         ('bool_check', 't', True),
         ('bool_check', 'T', True),
         ('bool_check', b'TRUE', True),
         ('bool_check', False, False),
         ('bool_check', 0, False),
+        ('bool_check', 0.0, False),
+        ('bool_check', Decimal(0), False),
         ('bool_check', 'n', False),
         ('bool_check', 'N', False),
         ('bool_check', 'no', False),
         ('bool_check', 'No', False),
         ('bool_check', 'NO', False),
         ('bool_check', 'false', False),
         ('bool_check', 'False', False),
@@ -939,61 +1051,148 @@
         ('bool_check', [], ValidationError),
         ('bool_check', {}, ValidationError),
         ('bool_check', [1, 2, 3, 4], ValidationError),
         ('bool_check', {1: 2, 3: 4}, ValidationError),
         ('bool_check', b'2', ValidationError),
         ('bool_check', '2', ValidationError),
         ('bool_check', 2, ValidationError),
+        ('bool_check', 2.0, ValidationError),
+        ('bool_check', Decimal(2), ValidationError),
         ('bool_check', b'\x81', ValidationError),
         ('bool_check', BoolCastable(), ValidationError),
         ('str_check', 's', 's'),
         ('str_check', '  s  ', 's'),
         ('str_check', b's', 's'),
         ('str_check', b'  s  ', 's'),
+        ('str_check', bytearray(b's' * 5), 'sssss'),
         ('str_check', 1, ValidationError),
         ('str_check', 'x' * 11, ValidationError),
         ('str_check', b'x' * 11, ValidationError),
+        ('str_check', b'\x81', ValidationError),
+        ('str_check', bytearray(b'\x81' * 5), ValidationError),
         ('bytes_check', 's', b's'),
         ('bytes_check', '  s  ', b'  s  '),
         ('bytes_check', b's', b's'),
         ('bytes_check', 1, ValidationError),
         ('bytes_check', bytearray('xx', encoding='utf8'), b'xx'),
         ('bytes_check', True, ValidationError),
         ('bytes_check', False, ValidationError),
         ('bytes_check', {}, ValidationError),
         ('bytes_check', 'x' * 11, b'x' * 11),
         ('bytes_check', b'x' * 11, b'x' * 11),
         ('int_check', 1, 1),
         ('int_check', 1.0, 1),
         ('int_check', 1.9, ValidationError),
+        ('int_check', Decimal(1), 1),
+        ('int_check', Decimal(1.9), ValidationError),
         ('int_check', '1', 1),
         ('int_check', '1.9', ValidationError),
         ('int_check', b'1', 1),
         ('int_check', 12, 12),
         ('int_check', '12', 12),
         ('int_check', b'12', 12),
         ('float_check', 1, 1.0),
         ('float_check', 1.0, 1.0),
+        ('float_check', Decimal(1.0), 1.0),
         ('float_check', '1.0', 1.0),
         ('float_check', '1', 1.0),
         ('float_check', b'1.0', 1.0),
         ('float_check', b'1', 1.0),
+        ('float_check', True, 1.0),
+        ('float_check', False, 0.0),
+        ('float_check', 't', ValidationError),
+        ('float_check', b't', ValidationError),
         ('uuid_check', 'ebcdab58-6eb8-46fb-a190-d07a33e9eac8', UUID('ebcdab58-6eb8-46fb-a190-d07a33e9eac8')),
         ('uuid_check', UUID('ebcdab58-6eb8-46fb-a190-d07a33e9eac8'), UUID('ebcdab58-6eb8-46fb-a190-d07a33e9eac8')),
         ('uuid_check', b'ebcdab58-6eb8-46fb-a190-d07a33e9eac8', UUID('ebcdab58-6eb8-46fb-a190-d07a33e9eac8')),
         ('uuid_check', b'\x12\x34\x56\x78' * 4, UUID('12345678-1234-5678-1234-567812345678')),
         ('uuid_check', 'ebcdab58-6eb8-46fb-a190-', ValidationError),
         ('uuid_check', 123, ValidationError),
         ('decimal_check', 42.24, Decimal('42.24')),
         ('decimal_check', '42.24', Decimal('42.24')),
         ('decimal_check', b'42.24', ValidationError),
         ('decimal_check', '  42.24  ', Decimal('42.24')),
         ('decimal_check', Decimal('42.24'), Decimal('42.24')),
         ('decimal_check', 'not a valid decimal', ValidationError),
         ('decimal_check', 'NaN', ValidationError),
+        ('date_check', date(2017, 5, 5), date(2017, 5, 5)),
+        ('date_check', datetime(2017, 5, 5), date(2017, 5, 5)),
+        ('date_check', '2017-05-05', date(2017, 5, 5)),
+        ('date_check', b'2017-05-05', date(2017, 5, 5)),
+        ('date_check', 1493942400000, date(2017, 5, 5)),
+        ('date_check', 1493942400, date(2017, 5, 5)),
+        ('date_check', 1493942400000.0, date(2017, 5, 5)),
+        ('date_check', Decimal(1493942400000), date(2017, 5, 5)),
+        ('date_check', datetime(2017, 5, 5, 10), ValidationError),
+        ('date_check', '2017-5-5', ValidationError),
+        ('date_check', b'2017-5-5', ValidationError),
+        ('date_check', 1493942401000, ValidationError),
+        ('date_check', 1493942401000.0, ValidationError),
+        ('date_check', Decimal(1493942401000), ValidationError),
+        ('datetime_check', datetime(2017, 5, 5, 10, 10, 10), datetime(2017, 5, 5, 10, 10, 10)),
+        ('datetime_check', date(2017, 5, 5), datetime(2017, 5, 5, 0, 0, 0)),
+        ('datetime_check', '2017-05-05T10:10:10.0002', datetime(2017, 5, 5, 10, 10, 10, microsecond=200)),
+        ('datetime_check', '2017-05-05 10:10:10', datetime(2017, 5, 5, 10, 10, 10)),
+        ('datetime_check', '2017-05-05 10:10:10+00:00', datetime(2017, 5, 5, 10, 10, 10, tzinfo=timezone.utc)),
+        ('datetime_check', b'2017-05-05T10:10:10.0002', datetime(2017, 5, 5, 10, 10, 10, microsecond=200)),
+        ('datetime_check', 1493979010000, datetime(2017, 5, 5, 10, 10, 10)),
+        ('datetime_check', 1493979010, datetime(2017, 5, 5, 10, 10, 10)),
+        ('datetime_check', 1493979010000.0, datetime(2017, 5, 5, 10, 10, 10)),
+        ('datetime_check', Decimal(1493979010), datetime(2017, 5, 5, 10, 10, 10)),
+        ('datetime_check', '2017-5-5T10:10:10', ValidationError),
+        ('datetime_check', b'2017-5-5T10:10:10', ValidationError),
+        ('time_check', time(10, 10, 10), time(10, 10, 10)),
+        ('time_check', '10:10:10.0002', time(10, 10, 10, microsecond=200)),
+        ('time_check', b'10:10:10.0002', time(10, 10, 10, microsecond=200)),
+        ('time_check', 3720, time(1, 2)),
+        ('time_check', 3720.0002, time(1, 2, microsecond=200)),
+        ('time_check', Decimal(3720.0002), time(1, 2, microsecond=200)),
+        ('time_check', '1:1:1', ValidationError),
+        ('time_check', b'1:1:1', ValidationError),
+        ('time_check', -1, ValidationError),
+        ('time_check', 86400, ValidationError),
+        ('time_check', 86400.0, ValidationError),
+        ('time_check', Decimal(86400), ValidationError),
+        ('timedelta_check', timedelta(days=1), timedelta(days=1)),
+        ('timedelta_check', '1 days 10:10', timedelta(days=1, seconds=36600)),
+        ('timedelta_check', '1 d 10:10', timedelta(days=1, seconds=36600)),
+        ('timedelta_check', b'1 days 10:10', timedelta(days=1, seconds=36600)),
+        ('timedelta_check', 123_000, timedelta(days=1, seconds=36600)),
+        ('timedelta_check', 123_000.0002, timedelta(days=1, seconds=36600, microseconds=200)),
+        ('timedelta_check', Decimal(123_000.0002), timedelta(days=1, seconds=36600, microseconds=200)),
+        ('timedelta_check', '1 10:10', ValidationError),
+        ('timedelta_check', b'1 10:10', ValidationError),
+        ('list_check', ['1', '2'], ['1', '2']),
+        ('list_check', ('1', '2'), ['1', '2']),
+        ('list_check', {'1': 1, '2': 2}.keys(), ['1', '2']),
+        ('list_check', {'1': '1', '2': '2'}.values(), ['1', '2']),
+        ('list_check', {'1', '2'}, ValidationError),
+        ('list_check', frozenset(['1', '2']), ValidationError),
+        ('list_check', {'1': 1, '2': 2}, ValidationError),
+        ('tuple_check', ('1', '2'), ('1', '2')),
+        ('tuple_check', ['1', '2'], ('1', '2')),
+        ('tuple_check', {'1': 1, '2': 2}.keys(), ('1', '2')),
+        ('tuple_check', {'1': '1', '2': '2'}.values(), ('1', '2')),
+        ('tuple_check', {'1', '2'}, ValidationError),
+        ('tuple_check', frozenset(['1', '2']), ValidationError),
+        ('tuple_check', {'1': 1, '2': 2}, ValidationError),
+        ('set_check', {'1', '2'}, {'1', '2'}),
+        ('set_check', ['1', '2', '1', '2'], {'1', '2'}),
+        ('set_check', ('1', '2', '1', '2'), {'1', '2'}),
+        ('set_check', frozenset(['1', '2']), {'1', '2'}),
+        ('set_check', {'1': 1, '2': 2}.keys(), {'1', '2'}),
+        ('set_check', {'1': '1', '2': '2'}.values(), {'1', '2'}),
+        ('set_check', {'1': 1, '2': 2}, ValidationError),
+        ('frozenset_check', frozenset(['1', '2']), frozenset(['1', '2'])),
+        ('frozenset_check', ['1', '2', '1', '2'], frozenset(['1', '2'])),
+        ('frozenset_check', ('1', '2', '1', '2'), frozenset(['1', '2'])),
+        ('frozenset_check', {'1', '2'}, frozenset(['1', '2'])),
+        ('frozenset_check', {'1': 1, '2': 2}.keys(), frozenset(['1', '2'])),
+        ('frozenset_check', {'1': '1', '2': '2'}.values(), frozenset(['1', '2'])),
+        ('frozenset_check', {'1': 1, '2': 2}, ValidationError),
     ],
 )
 def test_default_validators(field, value, result, CheckModel):
     kwargs = {field: value}
     if result == ValidationError:
         with pytest.raises(ValidationError):
             CheckModel(**kwargs)
@@ -1157,15 +1356,14 @@
 
 
 @pytest.mark.parametrize(
     'kwargs,type_',
     [
         ({'max_length': 5}, int),
         ({'min_length': 2}, float),
-        ({'frozen': True}, bool),
         ({'pattern': '^foo$'}, int),
         ({'gt': 2}, str),
         ({'lt': 5}, bytes),
         ({'ge': 2}, str),
         ({'le': 5}, bool),
         ({'gt': 0}, Callable),
         ({'gt': 0}, Callable[[int], int]),
@@ -2072,33 +2270,41 @@
 
     with pytest.raises(ValidationError, match=r'Input should be a valid integer \[type=int_type,'):
         Model(v='123456')
 
     with pytest.raises(ValidationError, match=r'Input should be a valid integer \[type=int_type,'):
         Model(v=3.14159)
 
+    with pytest.raises(ValidationError, match=r'Input should be a valid integer \[type=int_type,'):
+        Model(v=2**64)
+
+    with pytest.raises(ValidationError, match=r'Input should be a valid integer \[type=int_type,'):
+        Model(v=True)
+
 
 def test_strict_float():
     class Model(BaseModel):
         v: StrictFloat
 
     assert Model(v=3.14159).v == 3.14159
     assert Model(v=123456).v == 123456
 
     with pytest.raises(ValidationError, match=r'Input should be a valid number \[type=float_type,'):
         Model(v='3.14159')
 
+    with pytest.raises(ValidationError, match=r'Input should be a valid number \[type=float_type,'):
+        Model(v=True)
+
 
 def test_bool_unhashable_fails():
     class Model(BaseModel):
         v: bool
 
     with pytest.raises(ValidationError) as exc_info:
         Model(v={})
-    # insert_assert(exc_info.value.errors())
     assert exc_info.value.errors() == [
         {'type': 'bool_type', 'loc': ('v',), 'msg': 'Input should be a valid boolean', 'input': {}}
     ]
 
 
 def test_uuid_error():
     class Model(BaseModel):
@@ -3107,16 +3313,67 @@
         password: SecretStr
 
     # Should not raise an exception
     m = Foobar(password=SecretStr('1234'))
     assert m.password.get_secret_value() == '1234'
 
 
-def test_secretstr_is_hashable():
-    assert type(hash(SecretStr('secret'))) is int
+@pytest.mark.parametrize(
+    'pydantic_type',
+    [
+        Strict,
+        StrictBool,
+        conint,
+        PositiveInt,
+        NegativeInt,
+        NonPositiveInt,
+        NonNegativeInt,
+        StrictInt,
+        confloat,
+        PositiveFloat,
+        NegativeFloat,
+        NonPositiveFloat,
+        NonNegativeFloat,
+        StrictFloat,
+        FiniteFloat,
+        conbytes,
+        SecretBytes,
+        constr,
+        StrictStr,
+        SecretStr,
+        ImportString,
+        conset,
+        confrozenset,
+        conlist,
+        condecimal,
+        UUID1,
+        UUID3,
+        UUID4,
+        UUID5,
+        FilePath,
+        DirectoryPath,
+        NewPath,
+        Json,
+        ByteSize,
+        condate,
+        PastDate,
+        FutureDate,
+        AwareDatetime,
+        NaiveDatetime,
+    ],
+)
+def test_is_hashable(pydantic_type):
+    assert type(hash(pydantic_type)) is int
+
+
+def test_model_contain_hashable_type():
+    class MyModel(BaseModel):
+        v: Union[str, StrictStr]
+
+    assert MyModel(v='test').v == 'test'
 
 
 def test_secretstr_error():
     class Foobar(BaseModel):
         password: SecretStr
 
     with pytest.raises(ValidationError) as exc_info:
@@ -3212,18 +3469,14 @@
     class Foobar(BaseModel):
         password: SecretBytes
 
     # Should not raise an exception.
     _ = Foobar(password=SecretBytes(b'1234'))
 
 
-def test_secretbytes_is_hashable():
-    assert type(hash(SecretBytes(b'secret'))) is int
-
-
 def test_secretbytes_error():
     class Foobar(BaseModel):
         password: SecretBytes
 
     with pytest.raises(ValidationError) as exc_info:
         Foobar(password=[6, 23, 'abc'])
     # insert_assert(exc_info.value.errors())
```

### Comparing `pydantic-2.0a1/tests/test_types_namedtuple.py` & `pydantic-2.0a2/tests/test_types_namedtuple.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     with pytest.raises(ValidationError) as exc_info:
         Model(pos=('1', 2), event=['qwe', '2', 3, 'qwe'])
     # insert_assert(exc_info.value.errors())
     assert exc_info.value.errors() == [
         {
             'type': 'int_parsing',
-            'loc': ('event', 'arguments', 0),
+            'loc': ('event', 0),
             'msg': 'Input should be a valid integer, unable to parse string as an integer',
             'input': 'qwe',
         }
     ]
 
 
 def test_namedtuple_schema():
@@ -114,15 +114,15 @@
 
     with pytest.raises(ValidationError) as exc_info:
         Model(p=(1, 2, 3))
     # insert_assert(exc_info.value.errors())
     assert exc_info.value.errors() == [
         {
             'type': 'unexpected_positional_argument',
-            'loc': ('p', 'arguments', 2),
+            'loc': ('p', 2),
             'msg': 'Unexpected positional argument',
             'input': 3,
         }
     ]
 
 
 def test_namedtuple_postponed_annotation():
```

### Comparing `pydantic-2.0a1/tests/test_types_payment_card_number.py` & `pydantic-2.0a2/tests/test_types_payment_card_number.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_types_typeddict.py` & `pydantic-2.0a2/tests/test_types_typeddict.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         foo: str
 
     try:
 
         class M(BaseModel):
             d: MyDict
 
-    except TypeError as e:
-        assert str(e) == 'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.11.'
+    except PydanticUserError as e:
+        assert e.message == 'Please use `typing_extensions.TypedDict` instead of `typing.TypedDict` on Python < 3.11.'
     else:
         assert M(d=dict(foo='baz')).d == {'foo': 'baz'}
 
 
 def test_typeddict_annotated_simple(TypedDict, req_no_req):
     Required, NotRequired = req_no_req
 
@@ -82,18 +82,18 @@
         spam: NotRequired[float]
 
     class M(BaseModel):
         d: MyDict
 
     assert M(d=dict(foo='baz', bar='8')).d == {'foo': 'baz', 'bar': 8}
     assert M(d=dict(foo='baz', bar='8', spam='44.4')).d == {'foo': 'baz', 'bar': 8, 'spam': 44.4}
-    with pytest.raises(ValidationError, match=r'd -> bar\s+Field required \[type=missing,'):
+    with pytest.raises(ValidationError, match=r'd\.bar\s+Field required \[type=missing,'):
         M(d=dict(foo='baz'))
 
-    with pytest.raises(ValidationError, match=r'd -> bar\s+Input should be less than 10 \[type=less_than,'):
+    with pytest.raises(ValidationError, match=r'd\.bar\s+Input should be less than 10 \[type=less_than,'):
         M(d=dict(foo='baz', bar='11'))
 
 
 def test_typeddict_total_false(TypedDict, req_no_req):
     Required, NotRequired = req_no_req
 
     class MyDict(TypedDict, total=False):
@@ -101,15 +101,15 @@
         bar: int
 
     class M(BaseModel):
         d: MyDict
 
     assert M(d=dict(foo='baz', bar='8')).d == {'foo': 'baz', 'bar': 8}
     assert M(d=dict(foo='baz')).d == {'foo': 'baz'}
-    with pytest.raises(ValidationError, match=r'd -> foo\s+Field required \[type=missing,'):
+    with pytest.raises(ValidationError, match=r'd\.foo\s+Field required \[type=missing,'):
         M(d={})
 
 
 def test_typeddict(TypedDict):
     class TD(TypedDict):
         a: int
         b: int
@@ -120,15 +120,14 @@
         td: TD
 
     m = Model(td={'a': '3', 'b': b'1', 'c': 4, 'd': 'qwe'})
     assert m.td == {'a': 3, 'b': 1, 'c': 4, 'd': 'qwe'}
 
     with pytest.raises(ValidationError) as exc_info:
         Model(td={'a': [1], 'b': 2, 'c': 3, 'd': 'qwe'})
-    # insert_assert(exc_info.value.errors())
     assert exc_info.value.errors() == [
         {'type': 'int_type', 'loc': ('td', 'a'), 'msg': 'Input should be a valid integer', 'input': [1]}
     ]
 
 
 def test_typeddict_non_total(TypedDict):
     class FullMovie(TypedDict, total=True):
@@ -136,15 +135,14 @@
         year: int
 
     class Model(BaseModel):
         movie: FullMovie
 
     with pytest.raises(ValidationError) as exc_info:
         Model(movie={'year': '2002'})
-    # insert_assert(exc_info.value.errors())
     assert exc_info.value.errors() == [
         {'type': 'missing', 'loc': ('movie', 'name'), 'msg': 'Field required', 'input': {'year': '2002'}}
     ]
 
     class PartialMovie(TypedDict, total=False):
         name: str
         year: int
@@ -256,14 +254,35 @@
                 },
                 'required': ['b'],
             }
         },
     }
 
 
+def test_typeddict_from_attributes():
+    class UserCls:
+        def __init__(self, name: str, age: int):
+            self.name = name
+            self.age = age
+
+    class User(TypedDict):
+        name: str
+        age: int
+
+    class FromAttributesModel(BaseModel, from_attributes=True):
+        u: Annotated[User, Field(strict=False)]
+
+    class Model(BaseModel):
+        u: Annotated[User, Field(strict=False)]
+
+    assert FromAttributesModel(u=UserCls('foo', 15)).u == {'name': 'foo', 'age': 15}
+    with pytest.raises(ValidationError, match='Input should be a valid dictionary'):
+        Model(u=UserCls('foo', 15))
+
+
 def test_typeddict_not_required_schema(TypedDict, req_no_req):
     Required, NotRequired = req_no_req
 
     class DataTD(TypedDict, total=True):
         a: NotRequired[int]
         b: str
```

### Comparing `pydantic-2.0a1/tests/test_typing.py` & `pydantic-2.0a2/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_utils.py` & `pydantic-2.0a2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_validator.py` & `pydantic-2.0a2/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/test_validators.py` & `pydantic-2.0a2/tests/test_validators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,130 @@
 import re
 from collections import deque
-from datetime import datetime
+from datetime import date, datetime
 from enum import Enum
+from functools import partial, partialmethod
 from itertools import product
-from typing import Any, Deque, Dict, FrozenSet, List, Optional, Tuple, Type, Union
+from typing import Any, Callable, Deque, Dict, FrozenSet, List, Optional, Tuple, Type, Union
 from unittest.mock import MagicMock
 
 import pytest
-from typing_extensions import Literal
+from typing_extensions import Annotated, Literal
 
 from pydantic import (
     BaseModel,
     ConfigDict,
-    Extra,
     Field,
     FieldValidationInfo,
     ValidationError,
+    ValidationInfo,
+    ValidatorFunctionWrapHandler,
     errors,
     validator,
 )
+from pydantic.annotated_arguments import AfterValidator, BeforeValidator, WrapValidator
 from pydantic.decorators import field_validator, root_validator
 
 
+def test_annotated_validator_after() -> None:
+    MyInt = Annotated[int, AfterValidator(lambda x: x if x != -1 else 0)]
+
+    class Model(BaseModel):
+        x: MyInt
+
+    assert Model(x=0).x == 0
+    assert Model(x=-1).x == 0
+    assert Model(x=-2).x == -2
+    assert Model(x=1).x == 1
+    assert Model(x='-1').x == 0
+
+
+def test_annotated_validator_before() -> None:
+    FloatMaybeInf = Annotated[float, BeforeValidator(lambda x: x if x != 'zero' else 0.0)]
+
+    class Model(BaseModel):
+        x: FloatMaybeInf
+
+    assert Model(x='zero').x == 0.0
+    assert Model(x=1.0).x == 1.0
+    assert Model(x='1.0').x == 1.0
+
+
+def test_annotated_validator_wrap() -> None:
+    def sixties_validator(val: Any, handler: ValidatorFunctionWrapHandler, info: ValidationInfo) -> date:
+        if val == 'epoch':
+            return date.fromtimestamp(0)
+        newval = handler(val)
+        if not date.fromisoformat('1960-01-01') <= newval < date.fromisoformat('1970-01-01'):
+            raise ValueError(f'{val} is not in the sixties!')
+        return newval
+
+    SixtiesDateTime = Annotated[date, WrapValidator(sixties_validator)]
+
+    class Model(BaseModel):
+        x: SixtiesDateTime
+
+    assert Model(x='epoch').x == date.fromtimestamp(0)
+    assert Model(x='1962-01-13').x == date(year=1962, month=1, day=13)
+    assert Model(x=datetime(year=1962, month=1, day=13)).x == date(year=1962, month=1, day=13)
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(x=date(year=1970, month=4, day=17))
+    assert exc_info.value.errors() == [
+        {
+            'type': 'value_error',
+            'loc': ('x',),
+            'msg': 'Value error, 1970-04-17 is not in the sixties!',
+            'input': date(1970, 4, 17),
+            'ctx': {'error': '1970-04-17 is not in the sixties!'},
+        }
+    ]
+
+
+def test_annotated_validator_nested() -> None:
+    MyInt = Annotated[int, AfterValidator(lambda x: x if x != -1 else 0)]
+
+    def non_decreasing_list(data: List[int]) -> List[int]:
+        for prev, cur in zip(data, data[1:]):
+            assert cur >= prev
+        return data
+
+    class Model(BaseModel):
+        x: Annotated[List[MyInt], AfterValidator(non_decreasing_list)]
+
+    assert Model(x=[0, -1, 2]).x == [0, 0, 2]
+
+    with pytest.raises(ValidationError) as exc_info:
+        Model(x=[0, -1, -2])
+
+    assert exc_info.value.errors() == [
+        {
+            'type': 'assertion_error',
+            'loc': ('x',),
+            'msg': 'Assertion failed, assert -2 >= 0',
+            'input': [0, -1, -2],
+            'ctx': {'error': 'assert -2 >= 0'},
+        }
+    ]
+
+
+def test_annotated_validator_runs_before_field_validators() -> None:
+    MyInt = Annotated[int, AfterValidator(lambda x: x if x != -1 else 0)]
+
+    class Model(BaseModel):
+        x: MyInt
+
+        @field_validator('x')
+        def val_x(cls, v: int) -> int:
+            assert v != -1
+            return v
+
+    assert Model(x=-1).x == 0
+
+
 def test_simple():
     class Model(BaseModel):
         a: str
 
         @field_validator('a')
         @classmethod
         def check_a(cls, v: Any):
@@ -72,14 +171,17 @@
             'type': 'int_from_float',
             'loc': ('a',),
             'msg': 'Input should be a valid integer, got a number with a fractional part',
             'input': 4.5,
         }
     ]
 
+    # Doesn't raise ValidationError for number > (2 ^ 63) - 1 and limits them to (2 ^ 63) - 1
+    assert Model(a=(2**63) + 100).a == (2**63) - 1
+
 
 @pytest.mark.parametrize('value', [2.2250738585072011e308, float('nan'), float('inf')])
 def test_int_overflow_validation(value):
     class Model(BaseModel):
         a: int
 
     with pytest.raises(ValidationError) as exc_info:
@@ -233,15 +335,15 @@
             return v
 
         @field_validator('c')
         @classmethod
         def double_c(cls, v: Any):
             return v * 2
 
-        model_config = ConfigDict(validate_assignment=True, extra=Extra.allow)
+        model_config = ConfigDict(validate_assignment=True, extra='allow')
 
     return ValidateAssignmentModel
 
 
 def test_validating_assignment_ok(ValidateAssignmentModel):
     p = ValidateAssignmentModel(b='hello')
     assert p.b == 'hello'
@@ -360,31 +462,14 @@
             return v
 
     m = Model(a='this is foobar good')
     assert m.a == 'this is foobar good'
     m.check_a('x')
 
 
-def test_duplicates():
-    msg = r'duplicate validator function \"tests.test_validators::test_duplicates.<locals>.Model.duplicate_name\";'
-    with pytest.warns(UserWarning, match=msg):
-
-        class Model(BaseModel):
-            a: str
-            b: str
-
-            @field_validator('a')
-            def duplicate_name(cls, v: Any):
-                return v
-
-            @field_validator('b')
-            def duplicate_name(cls, v: Any):  # noqa
-                return v
-
-
 def test_use_bare():
     with pytest.raises(TypeError, match='validators should be used with fields'):
 
         class Model(BaseModel):
             a: str
 
             with pytest.warns(DeprecationWarning, match=V1_VALIDATOR_DEPRECATION_MATCH):
@@ -616,28 +701,28 @@
             'ctx': {'error': '"foobar" not found in a'},
         },
         {'type': 'missing', 'loc': ('b',), 'msg': 'Field required', 'input': {'a': 'snap'}},
     ]
 
 
 def test_invalid_field():
-    with pytest.raises(errors.PydanticUserError) as exc_info:
+    msg = (
+        r'Validators defined with incorrect fields:'
+        r' tests.test_validators.test_invalid_field.<locals>.Model:\d+.check_b'
+        r" \(use check_fields=False if you're inheriting from the model and intended this\)"
+    )
+    with pytest.raises(errors.PydanticUserError, match=msg):
 
         class Model(BaseModel):
             a: str
 
             @field_validator('b')
             def check_b(cls, v: Any):
                 return v
 
-    assert str(exc_info.value) == (
-        "Validators defined with incorrect fields: check_b "
-        "(use check_fields=False if you're inheriting from the model and intended this)"
-    )
-
 
 def test_validate_child():
     class Parent(BaseModel):
         a: str
 
     class Child(Parent):
         @field_validator('a')
@@ -1187,14 +1272,53 @@
     assert root_val_values == [
         {'a': 123, 'b': 'barbar', 'c': 'baz'},
         {'a': 123, 'b': 'changed', 'c': 'baz'},
         {'a': 1, 'b': 'snap dragonsnap dragon', 'c': 'snap dragon2'},
     ]
 
 
+def test_root_validator_subclass():
+    """
+    https://github.com/pydantic/pydantic/issues/5388
+    """
+
+    class Parent(BaseModel):
+        x: int
+        expected: Any
+
+        @root_validator(skip_on_failure=True)
+        @classmethod
+        def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+            assert cls is values['expected']
+            return values
+
+    class Child1(Parent):
+        pass
+
+    class Child2(Parent):
+        @root_validator(skip_on_failure=True)
+        @classmethod
+        def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+            assert cls is Child2
+            values['x'] = values['x'] * 2
+            return values
+
+    class Child3(Parent):
+        @classmethod
+        def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+            assert cls is Child3
+            values['x'] = values['x'] * 3
+            return values
+
+    assert Parent(x=1, expected=Parent).x == 1
+    assert Child1(x=1, expected=Child1).x == 1
+    assert Child2(x=1, expected=Child2).x == 2
+    assert Child3(x=1, expected=Child3).x == 3
+
+
 def test_root_validator_pre():
     root_val_values: List[Dict[str, Any]] = []
 
     class Model(BaseModel):
         a: int = 1
         b: str
 
@@ -1223,58 +1347,28 @@
             'msg': 'Value error, foobar',
             'input': {'b': 'snap dragon'},
             'ctx': {'error': 'foobar'},
         }
     ]
 
 
-def test_root_validator_repeat():
-    with pytest.warns(UserWarning, match='duplicate validator function'):
-
-        class Model(BaseModel):
-            a: int = 1
-
-            @root_validator(skip_on_failure=True)
-            def root_validator_repeated(cls, values: Dict[str, Any]) -> Dict[str, Any]:  # type: ignore
-                return values
-
-            @root_validator(skip_on_failure=True)
-            def root_validator_repeated(cls, values: Dict[str, Any]) -> Dict[str, Any]:  # noqa: F811
-                return values
-
-
-def test_root_validator_repeat2():
-    with pytest.warns(UserWarning, match='duplicate validator function'):
-
-        class Model(BaseModel):
-            a: int = 1
-
-            @field_validator('a')
-            def repeat_validator(cls, v: Any) -> Any:  # type: ignore
-                return v
-
-            @root_validator(skip_on_failure=True)
-            def repeat_validator(cls, values: Any) -> Any:  # noqa: F811
-                return values
-
-
 def test_root_validator_types():
     root_val_values: Optional[Tuple[Type[BaseModel], Dict[str, Any]]] = None
 
     class Model(BaseModel):
         a: int = 1
         b: str
 
         @root_validator(skip_on_failure=True)
         def root_validator(cls, values: Dict[str, Any]) -> Dict[str, Any]:
             nonlocal root_val_values
             root_val_values = cls, values
             return values
 
-        model_config = ConfigDict(extra=Extra.allow)
+        model_config = ConfigDict(extra='allow')
 
     assert Model(b='bar', c='wobble').model_dump() == {'a': 1, 'b': 'bar', 'c': 'wobble'}
 
     assert root_val_values == (Model, {'a': 1, 'b': 'bar', 'c': 'wobble'})
 
 
 def test_root_validator_returns_none_exception():
@@ -1297,64 +1391,22 @@
 
 
 def test_reuse_global_validators():
     class Model(BaseModel):
         x: int
         y: int
 
-        double_x = field_validator('x', allow_reuse=True)(reusable_validator)
-        double_y = field_validator('y', allow_reuse=True)(reusable_validator)
+        double_x = field_validator('x')(reusable_validator)
+        double_y = field_validator('y')(reusable_validator)
 
     assert dict(Model(x=1, y=1)) == {'x': 2, 'y': 2}
 
 
-def declare_with_reused_validators(include_root, allow_1, allow_2, allow_3):
-    class Model(BaseModel):
-        a: str
-        b: str
-
-        @field_validator('a', allow_reuse=allow_1)
-        @classmethod
-        def duplicate_name(cls, v: Any):
-            return v
-
-        @field_validator('b', allow_reuse=allow_2)
-        @classmethod
-        def duplicate_name(cls, v: Any):  # noqa F811
-            return v
-
-        if include_root:
-
-            @root_validator(allow_reuse=allow_3, skip_on_failure=True)
-            def duplicate_name(cls, values):  # noqa F811
-                return values
-
-
-@pytest.fixture
-def reset_tracked_validators():
-    from pydantic._internal._decorators import _FUNCS
-
-    original_tracked_validators = set(_FUNCS)
-    yield
-    _FUNCS.clear()
-    _FUNCS.update(original_tracked_validators)
-
-
-@pytest.mark.parametrize('include_root,allow_1,allow_2,allow_3', product(*[[True, False]] * 4))
-def test_allow_reuse(include_root, allow_1, allow_2, allow_3, reset_tracked_validators):
-    duplication_count = int(not allow_1) + int(not allow_2) + int(include_root and not allow_3)
-    if duplication_count > 1:
-        with pytest.warns(UserWarning, match='duplicate validator function'):
-            declare_with_reused_validators(include_root, allow_1, allow_2, allow_3)
-    else:
-        declare_with_reused_validators(include_root, allow_1, allow_2, allow_3)
-
-
 @pytest.mark.parametrize('validator_classmethod,root_validator_classmethod', product(*[[True, False]] * 2))
-def test_root_validator_classmethod(validator_classmethod, root_validator_classmethod, reset_tracked_validators):
+def test_root_validator_classmethod(validator_classmethod, root_validator_classmethod):
     root_val_values = []
 
     class Model(BaseModel):
         a: int = 1
         b: str
 
         def repeat_b(cls, v: Any):
@@ -1484,25 +1536,22 @@
             'msg': "Input should be 'foo' or 'bar'",
             'input': 'nope',
             'ctx': {'expected': "'foo' or 'bar'"},
         }
     ]
 
 
-# TODO: this test fails because our union schema
-# doesn't accept `frozen` as an argument
-# Do we need to add `frozen` to every schema?
-@pytest.mark.xfail(reason='frozen field')
 def test_union_literal_with_constraints():
     class Model(BaseModel, validate_assignment=True):
         x: Union[Literal[42], Literal['pika']] = Field(frozen=True)
 
     m = Model(x=42)
-    with pytest.raises(TypeError):
+    with pytest.raises(ValidationError) as exc_info:
         m.x += 1
+    assert exc_info.value.errors() == [{'input': 43, 'loc': ('x',), 'msg': 'Field is frozen', 'type': 'frozen_field'}]
 
 
 def test_field_that_is_being_validated_is_excluded_from_validator_values():
     check_values = MagicMock()
 
     class Model(BaseModel):
         foo: str
@@ -1645,30 +1694,30 @@
         {'skip_on_failure': True, 'pre': False},
         {'skip_on_failure': False, 'pre': True},
         {'pre': True},
     ],
 )
 def test_root_validator_skip_on_failure_valid(kwargs: Dict[str, Any]):
     class Model(BaseModel):
-        @root_validator(**kwargs, allow_reuse=True)
+        @root_validator(**kwargs)
         def root_val(cls, values: Dict[str, Any]) -> Dict[str, Any]:
             return values
 
 
 def test_root_validator_many_values_change():
     """It should run root_validator on assignment and update ALL concerned fields"""
 
     class Rectangle(BaseModel):
         width: float
         height: float
         area: Optional[float] = None
 
         model_config = ConfigDict(validate_assignment=True)
 
-        @root_validator(skip_on_failure=True, allow_reuse=True)
+        @root_validator(skip_on_failure=True)
         def set_area(cls, values: Dict[str, Any]) -> Dict[str, Any]:
             values['area'] = values['width'] * values['height']
             return values
 
     r = Rectangle(width=1, height=1)
     assert r.area == 1
     r.height = 5
@@ -1922,7 +1971,431 @@
             'ctx': {'error': 'assert -1 > 0'},
             'input': -1,
             'loc': ('x',),
             'msg': 'Assertion failed, assert -1 > 0',
             'type': 'assertion_error',
         }
     ]
+
+
+def partial_val_func1(
+    value: int,
+    allowed: int,
+) -> int:
+    assert value == allowed
+    return value
+
+
+def partial_val_func2(
+    value: int,
+    *,
+    allowed: int,
+) -> int:
+    assert value == allowed
+    return value
+
+
+def partial_values_val_func1(
+    value: int,
+    values: Dict[str, Any],
+    *,
+    allowed: int,
+) -> int:
+    assert isinstance(values, dict)
+    assert value == allowed
+    return value
+
+
+def partial_values_val_func2(
+    value: int,
+    *,
+    values: Dict[str, Any],
+    allowed: int,
+) -> int:
+    assert isinstance(values, dict)
+    assert value == allowed
+    return value
+
+
+def partial_info_val_func(
+    value: int,
+    info: FieldValidationInfo,
+    *,
+    allowed: int,
+) -> int:
+    assert isinstance(info.data, dict)
+    assert value == allowed
+    return value
+
+
+def partial_cls_val_func1(
+    cls: Any,
+    value: int,
+    allowed: int,
+    expected_cls: Any,
+) -> int:
+    assert cls.__name__ == expected_cls
+    assert value == allowed
+    return value
+
+
+def partial_cls_val_func2(
+    cls: Any,
+    value: int,
+    *,
+    allowed: int,
+    expected_cls: Any,
+) -> int:
+    assert cls.__name__ == expected_cls
+    assert value == allowed
+    return value
+
+
+def partial_cls_values_val_func1(
+    cls: Any,
+    value: int,
+    values: Dict[str, Any],
+    *,
+    allowed: int,
+    expected_cls: Any,
+) -> int:
+    assert cls.__name__ == expected_cls
+    assert isinstance(values, dict)
+    assert value == allowed
+    return value
+
+
+def partial_cls_values_val_func2(
+    cls: Any,
+    value: int,
+    *,
+    values: Dict[str, Any],
+    allowed: int,
+    expected_cls: Any,
+) -> int:
+    assert cls.__name__ == expected_cls
+    assert isinstance(values, dict)
+    assert value == allowed
+    return value
+
+
+def partial_cls_info_val_func(
+    cls: Any,
+    value: int,
+    info: FieldValidationInfo,
+    *,
+    allowed: int,
+    expected_cls: Any,
+) -> int:
+    assert cls.__name__ == expected_cls
+    assert isinstance(info.data, dict)
+    assert value == allowed
+    return value
+
+
+@pytest.mark.parametrize(
+    'func',
+    [
+        partial_val_func1,
+        partial_val_func2,
+        partial_info_val_func,
+    ],
+)
+def test_functools_partial_validator_v2(
+    func: Callable[..., Any],
+) -> None:
+    class Model(BaseModel):
+        x: int
+
+        val = field_validator('x')(partial(func, allowed=42))
+
+    Model(x=42)
+
+    with pytest.raises(ValidationError):
+        Model(x=123)
+
+
+@pytest.mark.parametrize(
+    'func',
+    [
+        partial_val_func1,
+        partial_val_func2,
+        partial_info_val_func,
+    ],
+)
+def test_functools_partialmethod_validator_v2(
+    func: Callable[..., Any],
+) -> None:
+    class Model(BaseModel):
+        x: int
+
+        val = field_validator('x')(partialmethod(func, allowed=42))
+
+    Model(x=42)
+
+    with pytest.raises(ValidationError):
+        Model(x=123)
+
+
+@pytest.mark.parametrize(
+    'func',
+    [
+        partial_cls_val_func1,
+        partial_cls_val_func2,
+        partial_cls_info_val_func,
+    ],
+)
+def test_functools_partialmethod_validator_v2_cls_method(
+    func: Callable[..., Any],
+) -> None:
+    class Model(BaseModel):
+        x: int
+
+        # note that you _have_ to wrap your function with classmethod
+        # it's partialmethod not us that requires it
+        # otherwise it creates a bound instance method
+        val = field_validator('x')(partialmethod(classmethod(func), allowed=42, expected_cls='Model'))
+
+    Model(x=42)
+
+    with pytest.raises(ValidationError):
+        Model(x=123)
+
+
+@pytest.mark.parametrize(
+    'func',
+    [
+        partial_val_func1,
+        partial_val_func2,
+        partial_values_val_func1,
+        partial_values_val_func2,
+    ],
+)
+def test_functools_partial_validator_v1(
+    func: Callable[..., Any],
+) -> None:
+    with pytest.warns(DeprecationWarning, match=V1_VALIDATOR_DEPRECATION_MATCH):
+
+        class Model(BaseModel):
+            x: int
+
+            val = validator('x')(partial(func, allowed=42))
+
+    Model(x=42)
+
+    with pytest.raises(ValidationError):
+        Model(x=123)
+
+
+@pytest.mark.parametrize(
+    'func',
+    [
+        partial_val_func1,
+        partial_val_func2,
+        partial_values_val_func1,
+        partial_values_val_func2,
+    ],
+)
+def test_functools_partialmethod_validator_v1(
+    func: Callable[..., Any],
+) -> None:
+    with pytest.warns(DeprecationWarning, match=V1_VALIDATOR_DEPRECATION_MATCH):
+
+        class Model(BaseModel):
+            x: int
+
+            val = validator('x')(partialmethod(func, allowed=42))
+
+        Model(x=42)
+
+        with pytest.raises(ValidationError):
+            Model(x=123)
+
+
+@pytest.mark.parametrize(
+    'func',
+    [
+        partial_cls_val_func1,
+        partial_cls_val_func2,
+        partial_cls_values_val_func1,
+        partial_cls_values_val_func2,
+    ],
+)
+def test_functools_partialmethod_validator_v1_cls_method(
+    func: Callable[..., Any],
+) -> None:
+    with pytest.warns(DeprecationWarning, match=V1_VALIDATOR_DEPRECATION_MATCH):
+
+        class Model(BaseModel):
+            x: int
+
+            # note that you _have_ to wrap your function with classmethod
+            # it's partialmethod not us that requires it
+            # otherwise it creates a bound instance method
+            val = validator('x')(partialmethod(classmethod(func), allowed=42, expected_cls='Model'))
+
+    Model(x=42)
+
+    with pytest.raises(ValidationError):
+        Model(x=123)
+
+
+def test_validator_allow_reuse_inheritance():
+    class Parent(BaseModel):
+        x: int
+
+        @field_validator('x')
+        def val(cls, v: int) -> int:
+            return v + 1
+
+    class Child(Parent):
+        @field_validator('x')
+        def val(cls, v: int) -> int:
+            assert v == 1
+            v = super().val(v)
+            assert v == 2
+            return 4
+
+    assert Parent(x=1).model_dump() == {'x': 2}
+    assert Child(x=1).model_dump() == {'x': 4}
+
+
+def test_validator_allow_reuse_same_field():
+    with pytest.warns(UserWarning, match='`val_x` overrides an existing Pydantic `@field_validator` decorator'):
+
+        class Model(BaseModel):
+            x: int
+
+            @field_validator('x')
+            def val_x(cls, v: int) -> int:
+                return v + 1
+
+            @field_validator('x')
+            def val_x(cls, v: int) -> int:  # noqa: F811
+                return v + 2
+
+        assert Model(x=1).model_dump() == {'x': 3}
+
+
+def test_validator_allow_reuse_different_field_1():
+    with pytest.warns(UserWarning, match='`val` overrides an existing Pydantic `@field_validator` decorator'):
+
+        class Model(BaseModel):
+            x: int
+            y: int
+
+            @field_validator('x')
+            def val(cls, v: int) -> int:
+                return v + 1
+
+            @field_validator('y')
+            def val(cls, v: int) -> int:  # noqa: F811
+                return v + 2
+
+    assert Model(x=1, y=2).model_dump() == {'x': 1, 'y': 4}
+
+
+def test_validator_allow_reuse_different_field_2():
+    with pytest.warns(UserWarning, match='`val_x` overrides an existing Pydantic `@field_validator` decorator'):
+
+        def val(cls: Any, v: int) -> int:
+            return v + 2
+
+        class Model(BaseModel):
+            x: int
+            y: int
+
+            @field_validator('x')
+            def val_x(cls, v: int) -> int:
+                return v + 1
+
+            val_x = field_validator('y')(val)  # noqa: F811
+
+    assert Model(x=1, y=2).model_dump() == {'x': 1, 'y': 4}
+
+
+def test_validator_allow_reuse_different_field_3():
+    with pytest.warns(UserWarning, match='`val_x` overrides an existing Pydantic `@field_validator` decorator'):
+
+        def val1(v: int) -> int:
+            return v + 1
+
+        def val2(v: int) -> int:
+            return v + 2
+
+        class Model(BaseModel):
+            x: int
+            y: int
+
+            val_x = field_validator('x')(val1)
+            val_x = field_validator('y')(val2)
+
+    assert Model(x=1, y=2).model_dump() == {'x': 1, 'y': 4}
+
+
+def test_validator_allow_reuse_different_field_4():
+    def val(v: int) -> int:
+        return v + 1
+
+    class Model(BaseModel):
+        x: int
+        y: int
+
+        val_x = field_validator('x')(val)
+        not_val_x = field_validator('y')(val)
+
+    assert Model(x=1, y=2).model_dump() == {'x': 2, 'y': 3}
+
+
+def test_root_validator_allow_reuse_same_field():
+    with pytest.warns(UserWarning, match='`root_val` overrides an existing Pydantic `@root_validator` decorator'):
+
+        class Model(BaseModel):
+            x: int
+
+            @root_validator(skip_on_failure=True)
+            def root_val(cls, v: Dict[str, Any]) -> Dict[str, Any]:
+                v['x'] += 1
+                return v
+
+            @root_validator(skip_on_failure=True)
+            def root_val(cls, v: Dict[str, Any]) -> Dict[str, Any]:  # noqa: F811
+                v['x'] += 2
+                return v
+
+        assert Model(x=1).model_dump() == {'x': 3}
+
+
+def test_root_validator_allow_reuse_inheritance():
+    class Parent(BaseModel):
+        x: int
+
+        @root_validator(skip_on_failure=True)
+        def root_val(cls, v: Dict[str, Any]) -> Dict[str, Any]:
+            v['x'] += 1
+            return v
+
+    class Child(Parent):
+        @root_validator(skip_on_failure=True)
+        def root_val(cls, v: Dict[str, Any]) -> Dict[str, Any]:
+            assert v == {'x': 1}
+            v = super().root_val(v)
+            assert v == {'x': 2}
+            return {'x': 4}
+
+    assert Parent(x=1).model_dump() == {'x': 2}
+    assert Child(x=1).model_dump() == {'x': 4}
+
+
+def test_validator_with_underscore_name() -> None:
+    """
+    https://github.com/pydantic/pydantic/issues/5252
+    """
+
+    def f(name: str) -> str:
+        return name.lower()
+
+    class Model(BaseModel):
+        name: str
+        _normalize_name = field_validator('name')(f)
+
+    assert Model(name='Adrian').name == 'adrian'
```

### Comparing `pydantic-2.0a1/tests/test_validators_dataclass.py` & `pydantic-2.0a2/tests/test_validators_dataclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,13 +176,13 @@
     with pytest.raises(ValidationError) as exc_info:
         MyDataclass(1, b='snap dragon')
     assert root_val_values == [{'a': 123, 'b': 'barbar'}, {'a': 1, 'b': 'snap dragonsnap dragon'}]
 
     assert exc_info.value.errors() == [
         {
             'ctx': {'error': 'foobar'},
-            'input': HasRepr(IsStr(regex=re.escape("ArgsKwargs(args=(1,), kwargs={'b': 'snap dragon'})"))),
+            'input': HasRepr(IsStr(regex=re.escape("ArgsKwargs((1,), {'b': 'snap dragon'})"))),
             'loc': (),
             'msg': 'Value error, foobar',
             'type': 'value_error',
         }
     ]
```

### Comparing `pydantic-2.0a1/tests/test_version.py` & `pydantic-2.0a2/tests/test_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pydantic
 from pydantic.version import version_info
 
 
 def test_version_info():
     s = version_info()
     assert re.match(' *pydantic version: ', s)
-    assert s.count('\n') == 4
+    assert s.count('\n') == 5
 
 
 def test_standard_version():
     v = parse_version(pydantic.VERSION)
     assert str(v) == pydantic.VERSION
```

### Comparing `pydantic-2.0a1/tests/mypy/test_mypy.py` & `pydantic-2.0a2/tests/mypy/test_mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 except ImportError:
     mypy_api = None
     mypy_version = None
     parse_mypy_version = lambda _: (0,)  # noqa: E731
 
 MYPY_VERSION_TUPLE = parse_mypy_version(mypy_version)
 
-pytestmark = pytest.mark.skipif('--test-mypy' not in sys.argv, reason='Test only with "--test-mypy" flag')
+pytestmark = pytest.mark.skipif(
+    '--test-mypy' not in sys.argv
+    and os.environ.get('PYCHARM_HOSTED') != '1',  # never skip when running via the PyCharm runner
+    reason='Test only with "--test-mypy" flag',
+)
 
 # This ensures mypy can find the test files, no matter where tests are run from:
 os.chdir(Path(__file__).parent.parent.parent)
 
 cases = [
     ('mypy-plugin.ini', 'plugin_success.py', None),
     ('mypy-plugin.ini', 'plugin_fail.py', 'plugin-fail.txt'),
@@ -133,15 +137,23 @@
                 break
         else:
             raise FileNotFoundError(f'Could not find expected output file {output_filename} in any of {output_roots}')
 
     # Specifying a different cache dir for each configuration dramatically speeds up subsequent execution
     # It also prevents cache-invalidation-related bugs in the tests
     cache_dir = f'.mypy_cache/test-{os.path.splitext(config_filename)[0]}'
-    command = [full_filename, '--config-file', full_config_filename, '--cache-dir', cache_dir, '--show-error-codes']
+    command = [
+        full_filename,
+        '--config-file',
+        full_config_filename,
+        '--cache-dir',
+        cache_dir,
+        '--show-error-codes',
+        '--show-traceback',
+    ]
     if MYPY_VERSION_TUPLE >= (0, 990):
         command.append('--disable-recursive-aliases')
     print(f"\nExecuting: mypy {' '.join(command)}")  # makes it easier to debug as necessary
     actual_result = mypy_api.run(command)
     actual_out, actual_err, actual_returncode = actual_result
     # Need to strip filenames due to differences in formatting by OS
     actual_out = '\n'.join(['.py:'.join(line.split('.py:')[1:]) for line in actual_out.split('\n') if line]).strip()
```

### Comparing `pydantic-2.0a1/tests/mypy/configs/mypy-plugin-strict-no-any.ini` & `pydantic-2.0a2/tests/mypy/configs/mypy-plugin-strict-no-any.ini`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/configs/pyproject-default.toml` & `pydantic-2.0a2/tests/mypy/configs/pyproject-default.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/configs/pyproject-plugin-bad-param.toml` & `pydantic-2.0a2/tests/mypy/configs/pyproject-plugin-bad-param.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/configs/pyproject-plugin-strict.toml` & `pydantic-2.0a2/tests/mypy/configs/pyproject-plugin-strict.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/configs/pyproject-plugin.toml` & `pydantic-2.0a2/tests/mypy/configs/pyproject-plugin.toml`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/modules/fail4.py` & `pydantic-2.0a2/tests/mypy/modules/fail4.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/modules/plugin_default_factory.py` & `pydantic-2.0a2/tests/mypy/modules/plugin_default_factory.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/modules/plugin_fail.py` & `pydantic-2.0a2/tests/mypy/modules/plugin_fail.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 kwargs_model = KwargsModel(x=1)
 kwargs_model.y = 'a'
 KwargsModel.from_orm({})
 KwargsModel.from_orm({})  # type: ignore[pydantic-orm]
 
 
 class ForbidExtraModel(BaseModel):
-    model_config = ConfigDict(extra='forbid')  # type: ignore[typeddict-item]
+    model_config = ConfigDict(extra=Extra.forbid)
 
 
 ForbidExtraModel(x=1)
 
 
 class KwargsForbidExtraModel(BaseModel, extra='forbid'):
     pass
```

### Comparing `pydantic-2.0a1/tests/mypy/modules/plugin_fail_baseConfig.py` & `pydantic-2.0a2/tests/mypy/modules/plugin_fail_baseConfig.py`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/modules/plugin_success.py` & `pydantic-2.0a2/tests/mypy/modules/plugin_success.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import ClassVar, Generic, List, Optional, TypeVar, Union
+from typing import Any, ClassVar, Generic, List, Optional, TypeVar, Union
 
-from pydantic import BaseModel, ConfigDict, Field, create_model, field_validator
+from pydantic import BaseModel, ConfigDict, Field, create_model, field_validator, validator
 from pydantic.dataclasses import dataclass
 
 
 # placeholder for removed line
 class Model(BaseModel):
     x: float
     y: str
@@ -190,15 +190,15 @@
 
 def f(name: str) -> str:
     return name
 
 
 class ModelWithAllowReuseValidator(BaseModel):
     name: str
-    normalize_name = field_validator('name', allow_reuse=True)(f)
+    normalize_name = field_validator('name')(f)
 
 
 model_with_allow_reuse_validator = ModelWithAllowReuseValidator(name='xyz')
 
 
 T = TypeVar('T')
 
@@ -272,7 +272,23 @@
 @dataclass
 class MyDataClass:
     foo: InitVarStr
     bar: str
 
 
 MyDataClass(foo='foo', bar='bar')
+
+
+def get_my_custom_validator(field_name: str) -> Any:
+    @validator(field_name, allow_reuse=True)
+    def my_custom_validator(cls: Any, v: int) -> int:
+        return v
+
+    return my_custom_validator
+
+
+def foo() -> None:
+    class MyModel(BaseModel):
+        number: int
+        custom_validator = get_my_custom_validator('number')  # type: ignore[pydantic-field]
+
+    MyModel(number=2)
```

### Comparing `pydantic-2.0a1/tests/mypy/modules/plugin_success_baseConfig.py` & `pydantic-2.0a2/tests/mypy/modules/plugin_success_baseConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
 def f(name: str) -> str:
     return name
 
 
 class ModelWithAllowReuseValidator(BaseModel):
     name: str
-    normalize_name = field_validator('name', allow_reuse=True)(f)
+    normalize_name = field_validator('name')(f)
 
 
 model_with_allow_reuse_validator = ModelWithAllowReuseValidator(name='xyz')
 
 
 T = TypeVar('T')
```

### Comparing `pydantic-2.0a1/tests/mypy/modules/success.py` & `pydantic-2.0a2/tests/mypy/modules/success.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 from pydantic import (
     UUID1,
     AwareDatetime,
     BaseModel,
     ConfigDict,
     DirectoryPath,
-    Extra,
     FilePath,
     FutureDate,
     ImportString,
     Json,
     NaiveDatetime,
     NegativeFloat,
     NegativeInt,
@@ -270,15 +269,15 @@
 
 obj: SomeDict = {
     'val': 12,
     'name': 'John',
 }
 
 
-config = ConfigDict(title='Record', extra=Extra.ignore, str_max_length=1234)
+config = ConfigDict(title='Record', extra='ignore', str_max_length=1234)
 
 
 class CustomPath(PurePath):
     def __init__(self, *args: str):
         self.path = os.path.join(*args)
 
     def __fspath__(self) -> str:
```

### Comparing `pydantic-2.0a1/tests/mypy/outputs/latest/fail4.txt` & `pydantic-2.0a2/tests/mypy/outputs/latest/fail4.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt` & `pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-baseConfig.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt` & `pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-strict-baseConfig.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/outputs/latest/plugin-fail-strict.txt` & `pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail-strict.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/tests/mypy/outputs/latest/plugin-fail.txt` & `pydantic-2.0a2/tests/mypy/outputs/latest/plugin-fail.txt`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/LICENSE` & `pydantic-2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic-2.0a1/pyproject.toml` & `pydantic-2.0a2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     'Framework :: Pydantic',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
 requires-python = '>=3.7'
 dependencies = [
     'typing-extensions>=4.2.0',
-    'pydantic-core>=0.22.0',
+    'pydantic-core==0.23.1',
     'annotated-types>=0.4.0',
 ]
 optional-dependencies = { email = ['email-validator>=1.3.0'] }
 dynamic = ['version', 'readme']
 
 entry-points.hypothesis = {_ = 'pydantic._hypothesis_plugin'}
 
@@ -94,15 +94,15 @@
 filterwarnings = [
     'error',
     'ignore:path is deprecated.*:DeprecationWarning:',
 ]
 
 # configuring https://github.com/pydantic/hooky
 [tool.hooky]
-reviewers = ['samuelcolvin', 'adriangb', 'dmontagu']
+reviewers = ['samuelcolvin', 'adriangb', 'dmontagu', 'hramezani', 'kludex']
 require_change_file = false
 
 [tool.ruff]
 line-length = 120
 extend-select = ['Q', 'RUF100', 'C90', 'UP', 'I']
 flake8-quotes = {inline-quotes = 'single', multiline-quotes = 'double'}
 mccabe = { max-complexity = 14 }
@@ -140,7 +140,8 @@
 color = true
 line-length = 120
 target-version = ['py310']
 skip-string-normalization = true
 
 [tool.pyright]
 include = ['pydantic']
+exclude = ['pydantic/_hypothesis_plugin.py', 'pydantic/mypy.py']
```

### Comparing `pydantic-2.0a1/PKG-INFO` & `pydantic-2.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic
-Version: 2.0a1
+Version: 2.0a2
 Summary: Data validation using Python type hints
 Project-URL: Homepage, https://github.com/pydantic/pydantic
 Project-URL: Documentation, https://docs.pydantic.dev
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic
 Project-URL: Changelog, https://docs.pydantic.dev/changelog
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>, Adrian Garcia Badaracco <1755071+adriangb@users.noreply.github.com>, Terrence Dorsey <terry@pydantic.dev>, David Montague <david@pydantic.dev>
@@ -31,15 +31,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: annotated-types>=0.4.0
-Requires-Dist: pydantic-core>=0.22.0
+Requires-Dist: pydantic-core==0.23.1
 Requires-Dist: typing-extensions>=4.2.0
 Provides-Extra: email
 Requires-Dist: email-validator>=1.3.0; extra == 'email'
 Description-Content-Type: text/markdown
 
 # Pydantic
 
@@ -108,14 +108,20 @@
 
 ## Reporting a Security Vulnerability
 
 See our [security policy](https://github.com/pydantic/pydantic/security/policy).
 
 ## Changelog
 
+## v2.0a2 (2023-04-12)
+
+Second pre-release of Pydantic V2
+
+See the full changelog [here](https://github.com/pydantic/pydantic/releases/tag/v2.0a2)
+
 ## v2.0a1 (2023-04-03)
 
 First pre-release of Pydantic V2!
 
 See [this post](https://docs.pydantic.dev/blog/pydantic-v2-alpha/) for more details.
 
 ## v1.10.7 (2023-03-22)
```

