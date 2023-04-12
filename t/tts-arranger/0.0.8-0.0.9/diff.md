# Comparing `tmp/tts_arranger-0.0.8.tar.gz` & `tmp/tts_arranger-0.0.9.tar.gz`

## Comparing `tts_arranger-0.0.8.tar` & `tts_arranger-0.0.9.tar`

### file list

```diff
@@ -1,681 +1,22 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/requirements.txt
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/.vscode/launch.json
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0    25944 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/tts_processor_example.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    14809 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_csv.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_csv.meta.json
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_thread.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_thread.meta.json
--rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_warnings.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_warnings.meta.json
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/ast.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/ast.meta.json
--rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/copy.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/copy.meta.json
--rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/csv.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/csv.meta.json
--rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/math.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/math.meta.json
--rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/textwrap.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/textwrap.meta.json
--rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/threading.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/threading.meta.json
--rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/warnings.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/warnings.meta.json
--rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/zipfile.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/zipfile.meta.json
--rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/logging/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/logging/__init__.meta.json
--rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.data.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/__init__.meta.json
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/_version.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/_version.meta.json
--rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/version.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/version.meta.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/records.meta.json
--rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
--rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_callable.meta.json
--rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
--rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_shape.meta.json
--rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
--rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/__init__.meta.json
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/example.meta.json
--rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/__init__.meta.json
--rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/_log.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/_log.meta.json
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/async_case.meta.json
--rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/case.data.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/case.meta.json
--rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/loader.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/loader.meta.json
--rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/main.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/main.meta.json
--rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/result.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/result.meta.json
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/runner.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/runner.meta.json
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/signals.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/signals.meta.json
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/suite.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/.mypy_cache/3.10/unittest/suite.meta.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/data/replace
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/data/replace_de
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/data/replace_en
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   193633 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57253 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19726 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_csv.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_csv.meta.json
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0    25923 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_thread.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_thread.meta.json
--rw-r--r--   0        0        0    14269 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_warnings.meta.json
--rw-r--r--   0        0        0    22321 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66338 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0   149406 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/ast.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/ast.meta.json
--rw-r--r--   0        0        0  1141170 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134174 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/copy.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/copy.meta.json
--rw-r--r--   0        0        0    32408 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/csv.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/csv.meta.json
--rw-r--r--   0        0        0    63212 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0   154518 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0    66801 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    24361 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93220 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    56135 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/math.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/math.meta.json
--rw-r--r--   0        0        0    31467 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    96535 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48501 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82069 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   182882 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    15164 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30218 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53668 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0    28866 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0   173134 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152111 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0    21126 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/textwrap.meta.json
--rw-r--r--   0        0        0    70489 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/threading.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/threading.meta.json
--rw-r--r--   0        0        0    47421 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0   248468 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444913 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73916 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    24120 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/warnings.data.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/warnings.meta.json
--rw-r--r--   0        0        0    75623 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/zipfile.meta.json
--rw-r--r--   0        0        0    96936 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446227 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140900 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13239 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26952 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9953 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86455 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33538 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75492 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69893 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97859 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12897 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0    16822 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0   154229 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/logging/__init__.meta.json
--rw-r--r--   0        0        0  2343815 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.data.json
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/__init__.meta.json
--rw-r--r--   0        0        0     5481 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_pytesttester.meta.json
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/_version.meta.json
--rw-r--r--   0        0        0   125407 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ctypeslib.meta.json
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/version.meta.json
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.data.json
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/__init__.meta.json
--rw-r--r--   0        0        0    15070 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_asarray.meta.json
--rw-r--r--   0        0        0    24061 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_internal.meta.json
--rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.data.json
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_type_aliases.meta.json
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/_ufunc_config.meta.json
--rw-r--r--   0        0        0    31557 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.data.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/arrayprint.meta.json
--rw-r--r--   0        0        0   183715 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/defchararray.meta.json
--rw-r--r--   0        0        0    52664 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/einsumfunc.meta.json
--rw-r--r--   0        0        0    87731 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.data.json
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/fromnumeric.meta.json
--rw-r--r--   0        0        0    15771 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/function_base.meta.json
--rw-r--r--   0        0        0   333938 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/multiarray.meta.json
--rw-r--r--   0        0        0   205927 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numeric.meta.json
--rw-r--r--   0        0        0    51620 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.data.json
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/numerictypes.meta.json
--rw-r--r--   0        0        0    57610 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/records.meta.json
--rw-r--r--   0        0        0    46542 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/shape_base.meta.json
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/core/umath.meta.json
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/__init__.meta.json
--rw-r--r--   0        0        0    20546 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/_pocketfft.meta.json
--rw-r--r--   0        0        0    24877 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/fft/helper.meta.json
--rw-r--r--   0        0        0    25931 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.data.json
--rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/__init__.meta.json
--rw-r--r--   0        0        0     9945 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/_version.meta.json
--rw-r--r--   0        0        0    21327 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraypad.meta.json
--rw-r--r--   0        0        0   168274 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arraysetops.meta.json
--rw-r--r--   0        0        0    28404 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/arrayterator.meta.json
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/format.meta.json
--rw-r--r--   0        0        0   252203 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.data.json
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/function_base.meta.json
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/histograms.meta.json
--rw-r--r--   0        0        0    69410 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/index_tricks.meta.json
--rw-r--r--   0        0        0    20190 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/mixins.meta.json
--rw-r--r--   0        0        0    42834 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.data.json
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/nanfunctions.meta.json
--rw-r--r--   0        0        0    90145 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.data.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/npyio.meta.json
--rw-r--r--   0        0        0   105059 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/polynomial.meta.json
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.data.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/scimath.meta.json
--rw-r--r--   0        0        0    96442 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.data.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/shape_base.meta.json
--rw-r--r--   0        0        0    26993 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.data.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/stride_tricks.meta.json
--rw-r--r--   0        0        0    87684 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/twodim_base.meta.json
--rw-r--r--   0        0        0   107191 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/type_check.meta.json
--rw-r--r--   0        0        0    27309 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/ufunclike.meta.json
--rw-r--r--   0        0        0    28399 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/lib/utils.meta.json
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/__init__.meta.json
--rw-r--r--   0        0        0   117180 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/linalg/linalg.meta.json
--rw-r--r--   0        0        0    29971 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/__init__.meta.json
--rw-r--r--   0        0        0   148374 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/core.meta.json
--rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/extras.meta.json
--rw-r--r--   0        0        0    15670 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.data.json
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/ma/mrecords.meta.json
--rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/__init__.meta.json
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.data.json
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/matrixlib/defmatrix.meta.json
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.data.json
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/__init__.meta.json
--rw-r--r--   0        0        0    27373 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/_polybase.meta.json
--rw-r--r--   0        0        0    18091 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/chebyshev.meta.json
--rw-r--r--   0        0        0    15600 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite.meta.json
--rw-r--r--   0        0        0    15653 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.data.json
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/hermite_e.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/laguerre.meta.json
--rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.data.json
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/legendre.meta.json
--rw-r--r--   0        0        0    14407 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polynomial.meta.json
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/polynomial/polyutils.meta.json
--rw-r--r--   0        0        0    10371 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/__init__.meta.json
--rw-r--r--   0        0        0   309096 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_generator.meta.json
--rw-r--r--   0        0        0    11554 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.data.json
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_mt19937.meta.json
--rw-r--r--   0        0        0    16856 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_pcg64.meta.json
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.data.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_philox.meta.json
--rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/_sfc64.meta.json
--rw-r--r--   0        0        0    74193 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.data.json
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/bit_generator.meta.json
--rw-r--r--   0        0        0   406457 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/random/mtrand.meta.json
--rw-r--r--   0        0        0     9435 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/__init__.meta.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/__init__.meta.json
--rw-r--r--   0        0        0   113220 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.data.json
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/testing/_private/utils.meta.json
--rw-r--r--   0        0        0    25769 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.data.json
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/__init__.meta.json
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.data.json
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_add_docstring.meta.json
--rw-r--r--   0        0        0    21381 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_array_like.meta.json
--rw-r--r--   0        0        0   274388 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.data.json
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_callable.meta.json
--rw-r--r--   0        0        0    45266 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_char_codes.meta.json
--rw-r--r--   0        0        0    31136 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_dtype_like.meta.json
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_extended_precision.meta.json
--rw-r--r--   0        0        0    32419 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_generic_alias.meta.json
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nbit.meta.json
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.data.json
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_nested_sequence.meta.json
--rw-r--r--   0        0        0     6331 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.data.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_scalars.meta.json
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_shape.meta.json
--rw-r--r--   0        0        0   266807 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/numpy/typing/_ufunc.meta.json
--rw-r--r--   0        0        0   382550 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/__init__.meta.json
--rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.data.json
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/tts_arranger.meta.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/__init__.meta.json
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.data.json
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/audio.meta.json
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/tts_arranger/utils/log.meta.json
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.data.json
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/__init__.meta.json
--rw-r--r--   0        0        0    26106 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.data.json
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/_log.meta.json
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/async_case.meta.json
--rw-r--r--   0        0        0   225848 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.data.json
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/case.meta.json
--rw-r--r--   0        0        0    15841 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/loader.meta.json
--rw-r--r--   0        0        0    12714 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/main.meta.json
--rw-r--r--   0        0        0    22369 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/result.meta.json
--rw-r--r--   0        0        0    11630 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/runner.meta.json
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/signals.meta.json
--rw-r--r--   0        0        0    12185 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/src/tts_arranger/utils/.mypy_cache/3.10/unittest/suite.meta.json
--rw-r--r--   0        0        0    16954 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/LICENSE
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/README.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 tts_arranger-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/requirements.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0    25944 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/tts_processor_example.py
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    14625 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/data/replace
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/data/replace_de
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/data/replace_en
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    16954 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 tts_arranger-0.0.9/PKG-INFO
```

### Comparing `tts_arranger-0.0.8/src/tts_arranger/tts_processor.py` & `tts_arranger-0.0.9/src/tts_arranger/tts_processor.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.8/src/tts_arranger/tts_processor_example.py` & `tts_arranger-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+# TTS Arranger
+
+A set of classes that simplify arranging text fragments with multiple speakers and processing it using coqui.ai TTS.
+
+# Examples
+
+```python
 #!/usr/bin/python3
 from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
                           TTS_Simple_Writer, TTS_Writer)
 
-# Simple example using Simple Writer
+# Simple example using Simple Writer (using a simple list of TTS items)
 
 tts_items = []
 
 tts_items.append(TTS_Item('This is a test', 'p330'))
 tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 'ED\n', length=10000))
 tts_items.append(TTS_Item(length=2000))  # Insert pause
 
@@ -23,30 +30,12 @@
 items2.append(TTS_Item('Another test',  speaker_idx=0))
 items2.append(TTS_Item('This is getting boring!',  speaker_idx=1))
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Chapter 1'))
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
-project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
+project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor', lang_code='de')
 
 writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/')
 writer.synthesize_and_write(project.author + ' - ' + project.title)
-
-# German example using Thorsten voice (no multispeaker support)
-
-items1 = []
-items1.append(TTS_Item('Dies ist ein Test:', speaker_idx=0))
-items1.append(TTS_Item('Noch ein Test:',  speaker_idx=1))
-
-items2 = []
-items2.append(TTS_Item('Ein weiterer Test',  speaker_idx=0))
-items2.append(TTS_Item('Langsam wird es langweilig!',  speaker_idx=1))
-
-chapter = []
-chapter.append(TTS_Chapter(items1, 'Kapitel 1'))
-chapter.append(TTS_Chapter(items2, 'Kapitel 2'))
-
-project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor')
-
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1')
-writer.synthesize_and_write(project.author + ' - ' + project.title)
+```
```

### Comparing `tts_arranger-0.0.8/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.0.9/src/tts_arranger/tts_simple_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.8/src/tts_arranger/tts_writer.py` & `tts_arranger-0.0.9/src/tts_arranger/tts_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,65 +100,42 @@
             total_items += len(chapter.tts_items)
 
         current_total_items = 0
 
         cumulative_time = 0
 
         for i, chapter in enumerate(chapters):
-            # print(f'for {i}, {chapter.title} in enumerate(chapters):')
             audio = AudioSegment.empty()
 
-            # temp_format = 'mp4'
-
-            # if self.output_format != 'm4b':
             temp_format = 'wav'
 
             filename = temp_dir + '/' + f'tts_part_{i}.{temp_format}'
 
             log(LOG_TYPE.INFO, f'Synthesizing chapter {i + 1} of {len(chapters)}')
 
             for j, tts_item in enumerate(chapter.tts_items):
-                # print(f'for {j}, tts_item in enumerate(chapter.tts_items):')
                 if tts_item.text:
                     log(LOG_TYPE.INFO, f'Synthesizing item {j + 1} of {len(chapter.tts_items)} ("{tts_item.speaker}", {tts_item.speaker_idx}, {tts_item.length}ms):{bcolors.ENDC} {tts_item.text}')
                 else:
                     log(LOG_TYPE.INFO, f'Adding pause: {tts_item.length}ms:{bcolors.ENDC} {tts_item.text}')
 
                 audio += tts_processor.synthesize_tts_item(tts_item)
 
                 if callback is not None:
-                    # callback(i + 1, len(chapters), j + 1, len(chapter.tts_items), chapter.title, current_total_items, total_items)
-                    # callback((i * len(chapter.tts_items) + j + 1) / (len(chapters) * len(chapter.tts_items)) * 100)
-                    # print(f'callback(100/({len(chapters)} * {len(chapter.tts_items)} * ({i} + {j}), tts_item)')
                     callback(100/(len(chapters) * len(chapter.tts_items)) * (i + j), tts_item)
 
             current_total_items += len(chapter.tts_items)
 
             self._write_temp_audio(audio, filename)
 
             num_zeros = len(str(len(self.temp_files)))
             chapter_title = f'{i + 1:0{num_zeros}} - {chapter.title}'
 
             filename_out = temp_dir + '/' + f'tts_part_{i}.{temp_format}'
 
-            # If the target format is not m4b, write individual files for chapters
-            if self.output_format != 'm4b':
-                title = self.project.title
-
-                if self.project.subtitle:
-                    title += ' - ' + self.project.subtitle
-
-                # Convert to target format, adding metadata
-                (
-                    ffmpeg
-                    .input(filename)
-                    .output(filename_out, **{'metadata': f'title={chapter_title}', 'metadata:': f'album={title}', 'metadata:g': f'artist={self.project.author}'}, loglevel='error')
-                    .run(overwrite_output=True)
-                )
-
             # Add temp files for concatenating later
             self.temp_files.append((chapter_title, filename_out))
 
             chapter.start_time = cumulative_time
             chapter.end_time = cumulative_time + self._get_nanoseconds_for_file(filename)
             cumulative_time = chapter.end_time
 
@@ -245,118 +222,142 @@
 
         # Apply dynamic compression
         params = ['-filter', f'speechnorm=e={comp_expansion}:r={comp_raise}:l=1']
         bitrate = '320k'
         format = 'wav'
         segment.export(output_filename, format, parameters=params, bitrate=bitrate)
 
-    def synthesize_and_write(self, project_filename: str, temp_dir_prefix: str = '', callback: Callable[[float, TTS_Item], None] | None = None) -> None:
+    def synthesize_and_write(self, project_filename: str, temp_dir_prefix: str = '', concat=True, callback: Callable[[float, TTS_Item], None] | None = None) -> None:
         """
         Synthesize and write the output audio files for the given project.
 
         :param project_filename: The project name.
         :type project_filename: str
 
         :param temp_dir_prefix: An optional prefix for the temporary directory name used during synthesis.
         :type temp_dir_prefix: str
 
+        :param concat: A boolean value indicating whether to concatenate the audio files into a single file or not. Defaults to True.
+        :type concat: bool
+
         :param callback: An optional callback function that will be called periodically during synthesis with progress information.
         :type callback: Callable[[float, TTS_Item], None] | None
+
         :return: None
 
         :raises: ValueError if `project_filename` is not a valid file path.
         """
 
-        if self.project.tts_chapters:
-            with tempfile.TemporaryDirectory(prefix=temp_dir_prefix) as temp_dir:
-                try:
-                    log(LOG_TYPE.INFO, f'Synthesizing {self.project.title}')
+        if not self.project.tts_chapters:
+            log(LOG_TYPE.ERROR, f'No chapters to synthesize, exiting')
+            return
 
-                    if self.model and self.vocoder:
-                        t = TTS_Processor(self.model, self.vocoder)
-                    else:
-                        match self.project.lang_code:
-                            case 'en':
-                                self.model = 'tts_models/en/vctk/vits'
-                                self.vocoder = ''
-                            case 'de':
-                                self.model = 'tts_models/de/thorsten/tacotron2-DDC'
-                                self.vocoder = 'vocoder_models/de/thorsten/hifigan_v1'
+        with tempfile.TemporaryDirectory(prefix=temp_dir_prefix) as temp_dir:
+            try:
+                log(LOG_TYPE.INFO, f'Synthesizing {self.project.title}')
 
-                        t = TTS_Processor(self.model, self.vocoder)
+                if self.model and self.vocoder:
+                    t = TTS_Processor(self.model, self.vocoder)
+                else:
+                    match self.project.lang_code:
+                        case 'en':
+                            self.model = 'tts_models/en/vctk/vits'
+                            self.vocoder = ''
+                        case 'de':
+                            self.model = 'tts_models/de/thorsten/tacotron2-DDC'
+                            self.vocoder = 'vocoder_models/de/thorsten/hifigan_v1'
+                        case _:
+                            raise ValueError(f'Language code {self.project.lang_code} not supported')
 
-                    self._synthesize_chapters(self.project.tts_chapters, temp_dir, t, callback)
+                    t = TTS_Processor(self.model, self.vocoder)
 
-                except Exception as e:
-                    log(LOG_TYPE.ERROR, f'Synthesizing {self.project.title} failed: {e}')
-                    sys.exit(1)
+                self._synthesize_chapters(self.project.tts_chapters, temp_dir, t, callback)
 
-                finally:
-                    # Prepare chapter metadata
-                    metadata_lines = [';FFMETADATA1\n']
+            except Exception as e:
+                log(LOG_TYPE.ERROR, f'Synthesizing {self.project.title} failed: {e}')
+                sys.exit(1)
 
-                    for chapter in self.project.tts_chapters:
-                        metadata_lines.append(f'[CHAPTER]\nSTART={chapter.start_time}\nEND={chapter.end_time}\ntitle={chapter.title}\n')
+            finally:
+                # Prepare chapter metadata
+                metadata_lines = [';FFMETADATA1\n']
 
-                    metadata = ''.join(metadata_lines)
-                    metadata_filename = f'{temp_dir}/metadata'
+                for chapter in self.project.tts_chapters:
+                    metadata_lines.append(f'[CHAPTER]\nSTART={chapter.start_time}\nEND={chapter.end_time}\ntitle={chapter.title}\n')
 
-                    # Write all the custom metadata to the new metadata file
-                    with open(metadata_filename, 'w') as metadata_file:
-                        metadata_file.write(metadata)
+                metadata = ''.join(metadata_lines)
+                metadata_filename = os.path.join(temp_dir, 'metadata')
 
-                    output_filename = os.path.join(self.project_path, '') + str(sanitize_filename(project_filename))
-                    output_extension = '.' + self.output_format
+                # Write all the custom metadata to the new metadata file
+                with open(metadata_filename, 'w') as metadata_file:
+                    metadata_file.write(metadata)
 
-                    # Shorten path if needed
-                    output_filename = output_filename[:255 - len(output_extension)]
-                    output_path = output_filename + output_extension
+                output_filename = os.path.join(self.project_path, sanitize_filename(project_filename))
+                output_extension = f'.{self.output_format}'
 
-                    # Create directory if needed
-                    os.makedirs(self.project_path, exist_ok=True)
+                # Shorten path if needed
+                output_filename = output_filename[:255 - len(output_extension)]
+                output_path = output_filename + output_extension
 
-                    # Concatenate all files, adding metadata and cover image (if set)
-                    if self.output_format == 'm4b':
-                        infiles = []
+                output_files: list[str] = []
 
-                        for _, file in self.temp_files:
-                            infiles.append(ffmpeg.input(file))
+                # Create directory if needed
+                os.makedirs(self.project_path, exist_ok=True)
 
-                        metadata_input = ffmpeg.input(f'{metadata_filename}')
+                # Concatenate all files, adding metadata and cover image (if set)
+                if concat:
+                    infiles = [ffmpeg.input(file) for _, file in self.temp_files]
 
-                        cmd = (
-                            ffmpeg
-                            .concat(*infiles, v=0, a=1)
-                            .output(metadata_input, output_path, map_metadata=1, **{'metadata': f'title={self.project.title}', 'metadata:': f'album={self.project.subtitle}', 'metadata:g': f'artist={self.project.author}'}, loglevel='error')
-                            .compile(overwrite_output=True)
-                        )
+                    metadata_input = ffmpeg.input(metadata_filename)
 
-                        # Remove last map parameter (workaround for ffmpeg-python bug)
-                        cmd = self._remove_last_arg(cmd, '-map')
+                    if self.output_format not in ['m4b', 'm4a']:
+                        log(LOG_TYPE.WARNING, f'Chapters are only possible for m4b/m4a at the moment.')
 
-                        subprocess.call(cmd)
+                    cmd = (
+                        ffmpeg
+                        .concat(*infiles, v=0, a=1)
+                        .output(metadata_input, output_path, map_metadata=1, **{'metadata': f'title={self.project.title}', 'metadata:': f'album={self.project.subtitle}', 'metadata:g': f'artist={self.project.author}'}, loglevel='error')
+                        .compile(overwrite_output=True)
+                    )
 
-                        # Add image
-                        output_path_with_image = output_filename + '_tmp' + output_extension
+                    # Remove last map parameter (workaround for ffmpeg-python bug)
+                    cmd = self._remove_last_arg(cmd, '-map')
 
-                        if self.project.image_bytes:
-                            image_bytes = base64.b64decode(self.project.image_bytes)
-                            image_file = io.BytesIO(image_bytes)
-                            image = Image.open(image_file)
-
-                            if image.format:
-                                log(LOG_TYPE.INFO, f'Adding first found image as cover')
-                                self._add_image(image, output_path, output_path_with_image)
-                                os.remove(output_path)
-                                os.rename(output_path_with_image, output_path)
-
-                    else:
-                        # For all other formats, don’t concatenate, just reuse the tempfiles
-                        os.makedirs(output_filename, exist_ok=True)
-
-                        for name, file in self.temp_files:
-                            destination = output_filename + '/' + f'{name}.{self.output_format}'
-                            os.rename(file, destination)
+                    subprocess.call(cmd)
 
-            log(LOG_TYPE.SUCCESS, f'Synthesizing {self.project.title} finished, file saved under {output_path}.')
-        else:
-            log(LOG_TYPE.ERROR, f'No chapters to synthesize, exiting')
+                    output_files.append(output_path)
+                    log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, file saved as {output_path}.')
+                else:
+                    # Don’t concatenate, convert the chapter temp files to the target format
+                    os.makedirs(output_filename, exist_ok=True)
+
+                    for name, file in self.temp_files:
+                        output_chapter_filename = os.path.join(output_filename, name + output_extension)
+
+                        # Convert to target format, adding metadata
+                        (
+                            ffmpeg
+                            .input(file)
+                            .output(output_chapter_filename, **{'metadata': f'title={self.project.title} - {name}', 'metadata:': f'album={self.project.subtitle}', 'metadata:g': f'artist={self.project.author}'}, loglevel='error')
+                            .run(overwrite_output=True)
+                        )
+
+                        output_files.append(output_chapter_filename)
+                    log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, chapter files saved under {output_filename}.')
+
+                image_added = False
+                for output_file in output_files:
+                    # Add image
+                    output_path_with_image = output_file + '_tmp' + output_extension
+
+                    if self.project.image_bytes:
+                        image_bytes = base64.b64decode(self.project.image_bytes)
+                        image_file = io.BytesIO(image_bytes)
+                        image = Image.open(image_file)
+
+                        if image.format:
+                            self._add_image(image, output_file, output_path_with_image)
+                            os.remove(output_file)
+                            os.rename(output_path_with_image, output_file)
+                            image_added = True
+
+                if image_added:
+                    log(LOG_TYPE.SUCCESS, 'Project image added to final output for all files.')
```

### Comparing `tts_arranger-0.0.8/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.0.9/src/tts_arranger/items/tts_chapter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.8/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.0.9/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.8/src/tts_arranger/utils/audio.py` & `tts_arranger-0.0.9/src/tts_arranger/utils/audio.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.8/src/tts_arranger/utils/log.py` & `tts_arranger-0.0.9/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.8/tests/tts_arranger_test.py` & `tts_arranger-0.0.9/tests/tts_arranger_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.0.8/LICENSE` & `tts_arranger-0.0.9/LICENSE`

 * *Files identical despite different names*

