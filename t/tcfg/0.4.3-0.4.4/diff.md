# Comparing `tmp/tcfg-0.4.3.tar.gz` & `tmp/tcfg-0.4.4.tar.gz`

## Comparing `tcfg-0.4.3.tar` & `tcfg-0.4.4.tar`

### file list

```diff
@@ -1,395 +1,13 @@
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tcfg-0.4.3/TODO.md
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/missing_stubs
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   187161 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    61725 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19511 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   179195 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0   118903 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_operator.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_operator.meta.json
--rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_random.data.json
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_random.meta.json
--rw-r--r--   0        0        0    87573 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_socket.data.json
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_socket.meta.json
--rw-r--r--   0        0        0    26727 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_stat.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_stat.meta.json
--rw-r--r--   0        0        0    25287 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_thread.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_thread.meta.json
--rw-r--r--   0        0        0    14185 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_warnings.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_warnings.meta.json
--rw-r--r--   0        0        0    28375 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_weakref.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_weakref.meta.json
--rw-r--r--   0        0        0    47187 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_weakrefset.data.json
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_weakrefset.meta.json
--rw-r--r--   0        0        0    67152 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_winapi.data.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_winapi.meta.json
--rw-r--r--   0        0        0    21728 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    62984 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0   143804 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/ast.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/ast.meta.json
--rw-r--r--   0        0        0    52056 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/bdb.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/bdb.meta.json
--rw-r--r--   0        0        0  1078275 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0    21511 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/cmd.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/cmd.meta.json
--rw-r--r--   0        0        0   127554 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   110480 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/contextvars.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/contextvars.meta.json
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/copy.data.json
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/copy.meta.json
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/copyreg.data.json
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/copyreg.meta.json
--rw-r--r--   0        0        0   147319 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/datetime.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/datetime.meta.json
--rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    43182 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/dis.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/dis.meta.json
--rw-r--r--   0        0        0    64264 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    27329 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/errno.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/errno.meta.json
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/fnmatch.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/fnmatch.meta.json
--rw-r--r--   0        0        0    92888 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/fractions.data.json
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/fractions.meta.json
--rw-r--r--   0        0        0   136195 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/functools.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/functools.meta.json
--rw-r--r--   0        0        0    23903 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    54839 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/gettext.data.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/gettext.meta.json
--rw-r--r--   0        0        0    28906 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/hashlib.data.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/hashlib.meta.json
--rw-r--r--   0        0        0   364882 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/inspect.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/inspect.meta.json
--rw-r--r--   0        0        0    88683 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0   267210 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/itertools.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/itertools.meta.json
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/keyword.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/keyword.meta.json
--rw-r--r--   0        0        0     6993 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/marshal.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/marshal.meta.json
--rw-r--r--   0        0        0    54016 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/math.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/math.meta.json
--rw-r--r--   0        0        0    24378 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    15221 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/ntpath.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/ntpath.meta.json
--rw-r--r--   0        0        0    84030 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0     6641 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/opcode.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/opcode.meta.json
--rw-r--r--   0        0        0    51051 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/operator.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/operator.meta.json
--rw-r--r--   0        0        0    91198 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    99178 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pdb.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pdb.meta.json
--rw-r--r--   0        0        0    47620 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    80931 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0    12696 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pprint.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pprint.meta.json
--rw-r--r--   0        0        0    32182 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/queue.data.json
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/queue.meta.json
--rw-r--r--   0        0        0    44150 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/random.data.json
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/random.meta.json
--rw-r--r--   0        0        0   151234 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    54128 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/selectors.data.json
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/selectors.meta.json
--rw-r--r--   0        0        0    15945 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/signal.data.json
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/signal.meta.json
--rw-r--r--   0        0        0    81032 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/socket.data.json
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/socket.meta.json
--rw-r--r--   0        0        0    15114 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    29779 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    52548 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   198718 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/ssl.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/ssl.meta.json
--rw-r--r--   0        0        0     9568 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/stat.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/stat.meta.json
--rw-r--r--   0        0        0    28298 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/string.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/string.meta.json
--rw-r--r--   0        0        0   176375 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   166055 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0   112095 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/tempfile.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/tempfile.meta.json
--rw-r--r--   0        0        0    20647 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/textwrap.data.json
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/textwrap.meta.json
--rw-r--r--   0        0        0    67650 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/threading.data.json
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/threading.meta.json
--rw-r--r--   0        0        0    40240 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/time.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/time.meta.json
--rw-r--r--   0        0        0    54470 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/traceback.data.json
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/traceback.meta.json
--rw-r--r--   0        0        0   242432 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   430633 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    71560 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    23633 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/warnings.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/warnings.meta.json
--rw-r--r--   0        0        0   129790 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/weakref.data.json
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/weakref.meta.json
--rw-r--r--   0        0        0    72904 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/zipfile.data.json
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/zipfile.meta.json
--rw-r--r--   0        0        0    13862 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/zipimport.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/zipimport.meta.json
--rw-r--r--   0        0        0    92917 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0    11143 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/__init__.data.json
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/__init__.meta.json
--rw-r--r--   0        0        0   106356 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/base_events.data.json
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/base_events.meta.json
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/constants.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/constants.meta.json
--rw-r--r--   0        0        0    27438 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/coroutines.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/coroutines.meta.json
--rw-r--r--   0        0        0   205994 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/events.data.json
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/events.meta.json
--rw-r--r--   0        0        0     9381 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/exceptions.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/exceptions.meta.json
--rw-r--r--   0        0        0    35897 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/futures.data.json
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/futures.meta.json
--rw-r--r--   0        0        0    28369 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/locks.data.json
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/locks.meta.json
--rw-r--r--   0        0        0    21971 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/proactor_events.data.json
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/proactor_events.meta.json
--rw-r--r--   0        0        0    17930 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/protocols.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/protocols.meta.json
--rw-r--r--   0        0        0    24501 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/queues.data.json
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/queues.meta.json
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/runners.data.json
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/runners.meta.json
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/selector_events.data.json
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/selector_events.meta.json
--rw-r--r--   0        0        0    33599 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/streams.data.json
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/streams.meta.json
--rw-r--r--   0        0        0    25602 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/subprocess.data.json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/subprocess.meta.json
--rw-r--r--   0        0        0   107952 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/tasks.data.json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/tasks.meta.json
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/threads.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/threads.meta.json
--rw-r--r--   0        0        0    28507 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/transports.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/transports.meta.json
--rw-r--r--   0        0        0    16842 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/unix_events.data.json
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/unix_events.meta.json
--rw-r--r--   0        0        0    35739 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/windows_events.data.json
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/windows_events.meta.json
--rw-r--r--   0        0        0    19652 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/windows_utils.data.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/asyncio/windows_utils.meta.json
--rw-r--r--   0        0        0   390760 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/concurrent/__init__.data.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/concurrent/__init__.meta.json
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/concurrent/futures/__init__.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/concurrent/futures/__init__.meta.json
--rw-r--r--   0        0        0    63682 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/concurrent/futures/_base.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/concurrent/futures/_base.meta.json
--rw-r--r--   0        0        0    63541 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/concurrent/futures/process.data.json
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/concurrent/futures/process.meta.json
--rw-r--r--   0        0        0    23385 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/concurrent/futures/thread.data.json
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/concurrent/futures/thread.meta.json
--rw-r--r--   0        0        0   144037 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8136 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    12863 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25507 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9713 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    62371 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    32712 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     4509 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/html/__init__.data.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/html/__init__.meta.json
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/html/entities.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/html/entities.meta.json
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    73185 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    68159 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    23013 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/util.data.json
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/util.meta.json
--rw-r--r--   0        0        0    94701 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/__init__.data.json
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/__init__.meta.json
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/_identifier.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/_identifier.meta.json
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/async_utils.data.json
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/async_utils.meta.json
--rw-r--r--   0        0        0    27378 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/bccache.data.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/bccache.meta.json
--rw-r--r--   0        0        0   164971 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/compiler.data.json
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/compiler.meta.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/constants.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/constants.meta.json
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/debug.data.json
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/debug.meta.json
--rw-r--r--   0        0        0     6340 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/defaults.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/defaults.meta.json
--rw-r--r--   0        0        0   123456 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/environment.data.json
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/environment.meta.json
--rw-r--r--   0        0        0    18385 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/exceptions.data.json
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/exceptions.meta.json
--rw-r--r--   0        0        0    52571 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/ext.data.json
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/ext.meta.json
--rw-r--r--   0        0        0   161267 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/filters.data.json
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/filters.meta.json
--rw-r--r--   0        0        0    44527 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/idtracking.data.json
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/idtracking.meta.json
--rw-r--r--   0        0        0    95344 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/lexer.data.json
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/lexer.meta.json
--rw-r--r--   0        0        0    50462 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/loaders.data.json
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/loaders.meta.json
--rw-r--r--   0        0        0   154100 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/nodes.data.json
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/nodes.meta.json
--rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/optimizer.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/optimizer.meta.json
--rw-r--r--   0        0        0    49607 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/parser.data.json
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/parser.meta.json
--rw-r--r--   0        0        0   157859 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/runtime.data.json
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/runtime.meta.json
--rw-r--r--   0        0        0    34285 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/sandbox.data.json
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/sandbox.meta.json
--rw-r--r--   0        0        0    19321 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/tests.data.json
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/tests.meta.json
--rw-r--r--   0        0        0    65245 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/utils.data.json
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/utils.meta.json
--rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/visitor.data.json
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/jinja2/visitor.meta.json
--rw-r--r--   0        0        0    16705 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    15596 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0   149663 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/logging/__init__.data.json
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/logging/__init__.meta.json
--rw-r--r--   0        0        0    36341 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/markupsafe/__init__.data.json
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/markupsafe/__init__.meta.json
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/markupsafe/_native.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/markupsafe/_native.meta.json
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/markupsafe/_speedups.data.json
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/markupsafe/_speedups.meta.json
--rw-r--r--   0        0        0    33085 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/__init__.data.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/__init__.meta.json
--rw-r--r--   0        0        0    32446 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/connection.data.json
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/connection.meta.json
--rw-r--r--   0        0        0    90285 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/context.data.json
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/context.meta.json
--rw-r--r--   0        0        0   154782 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/managers.data.json
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/managers.meta.json
--rw-r--r--   0        0        0    53358 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/pool.data.json
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/pool.meta.json
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/popen_fork.data.json
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/popen_fork.meta.json
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/popen_forkserver.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/popen_forkserver.meta.json
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.data.json
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/popen_spawn_posix.meta.json
--rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/popen_spawn_win32.meta.json
--rw-r--r--   0        0        0    18655 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/process.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/process.meta.json
--rw-r--r--   0        0        0    20825 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/queues.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/queues.meta.json
--rw-r--r--   0        0        0    32328 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/reduction.data.json
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/reduction.meta.json
--rw-r--r--   0        0        0    29259 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/shared_memory.data.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/shared_memory.meta.json
--rw-r--r--   0        0        0    72022 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/sharedctypes.data.json
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/sharedctypes.meta.json
--rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/spawn.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/spawn.meta.json
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/synchronize.data.json
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/synchronize.meta.json
--rw-r--r--   0        0        0    24742 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/util.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/multiprocessing/util.meta.json
--rw-r--r--   0        0        0   248793 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5321 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0    46118 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/__init__.data.json
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/__init__.meta.json
--rw-r--r--   0        0        0     9079 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/actions.data.json
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/actions.meta.json
--rw-r--r--   0        0        0    41814 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/common.data.json
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/common.meta.json
--rw-r--r--   0        0        0   335378 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/core.data.json
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/core.meta.json
--rw-r--r--   0        0        0    23184 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/exceptions.data.json
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/exceptions.meta.json
--rw-r--r--   0        0        0    50766 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/helpers.data.json
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/helpers.meta.json
--rw-r--r--   0        0        0    31583 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/results.data.json
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/results.meta.json
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/testing.data.json
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/testing.meta.json
--rw-r--r--   0        0        0    30270 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/unicode.data.json
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/unicode.meta.json
--rw-r--r--   0        0        0    20242 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/util.data.json
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/util.meta.json
--rw-r--r--   0        0        0    60747 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/diagram/__init__.data.json
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/pyparsing/diagram/__init__.meta.json
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/tcfg/__init__.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/tcfg/__init__.meta.json
--rw-r--r--   0        0        0    81929 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/tcfg/config.data.json
--rw-r--r--   0        0        0    81929 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/tcfg/config.data.json.7756597b892bddbc
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/tcfg/config.meta.json
--rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/tcfg/reserved.data.json
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/tcfg/reserved.meta.json
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/urllib/__init__.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/urllib/__init__.meta.json
--rw-r--r--   0        0        0   152260 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/urllib/parse.data.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 tcfg-0.4.3/.mypy_cache/3.10/urllib/parse.meta.json
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tcfg-0.4.3/examples/cfg.yml
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 tcfg-0.4.3/examples/decorator.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tcfg-0.4.3/examples/inherit.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tcfg-0.4.3/examples/nested.json
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tcfg-0.4.3/tcfg/__init__.py
--rw-r--r--   0        0        0    24520 2020-02-02 00:00:00.000000 tcfg-0.4.3/tcfg/config.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 tcfg-0.4.3/tcfg/reserved.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tcfg-0.4.3/LICENSE
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 tcfg-0.4.3/README.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 tcfg-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 tcfg-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 tcfg-0.4.4/Makefile
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 tcfg-0.4.4/TODO.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 tcfg-0.4.4/examples/cfg.yml
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 tcfg-0.4.4/examples/decorator.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 tcfg-0.4.4/examples/inherit.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tcfg-0.4.4/examples/nested.json
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 tcfg-0.4.4/tcfg/__init__.py
+-rw-r--r--   0        0        0    24618 2020-02-02 00:00:00.000000 tcfg-0.4.4/tcfg/config.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 tcfg-0.4.4/tcfg/reserved.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 tcfg-0.4.4/LICENSE
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 tcfg-0.4.4/README.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 tcfg-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 tcfg-0.4.4/PKG-INFO
```

### Comparing `tcfg-0.4.3/examples/decorator.py` & `tcfg-0.4.4/examples/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tcfg import Path, tcfg
+from tcfg import TypePath, tcfg
 from typing import Literal
 
 
 @tcfg
 class SuperNested:
     extra: str
 
@@ -31,15 +31,15 @@
 
     extensions: list[str | dict[str, dict]]
     """List of extensions to use for the server."""
 
     path: Literal['/home/', '/home/documents']
     """Path to root of server. ONLY two paths supported."""
 
-    random: str = Path('/random/dir')
+    random: str = TypePath('/random/dir')
     """Random path. Is normalized and has `/` stripped from ends. Stored as a
     string."""
 
 
 print(dict(Config()))
 config = Config()
 print(config.nested.port)
```

### Comparing `tcfg-0.4.3/examples/inherit.py` & `tcfg-0.4.4/examples/inherit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tcfg import Path, config
+from tcfg import TypePath, config
 from typing import Literal
 
 
 class Nested(config):
     """Nested config"""
 
     _path_ = "nested.json"
@@ -23,14 +23,14 @@
     """Nested server configurations."""
 
     extensions: list[str | dict[str, dict]]
     """List of extensions to use for the server."""
 
     path: Literal['/home/', '/home/documents']
 
-    random: str = Path('/random/dir')
+    random: str = TypePath('/random/dir')
 
 
 if __name__ == "__main__":
     cfg = Config()
     print(cfg.as_dict())
     print(cfg.nested.port)
```

### Comparing `tcfg-0.4.3/tcfg/config.py` & `tcfg-0.4.4/tcfg/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,40 +24,40 @@
 
 from inspect import getmembers, ismethod
 
 import pathlib
 import re
 
 from types import GenericAlias, UnionType
-from typing import get_type_hints, Any, Literal
+from typing import TypeAlias, get_type_hints, Any, Literal
 
 from json import loads as json_load, dumps as json_dump
 from pyparsing import Iterator
 from toml import loads as toml_load, dumps as toml_dump
 from yaml import safe_load as yml_load, dump as yml_dump
 
-from .reserved import Path, MISSING
+from .reserved import TypePath, MISSING
 
 from saimll import ppath, SAIML, p_value
 
-LiteralGenericAlias = type(Literal[''])
+LiteralGenericAlias: TypeAlias = type(Literal[''])
 
 
 def ptype(_type: str, quotes: bool = True) -> str:
     markup = SAIML.parse(f"[@F #f5a97f $]{_type}[@F]")
 
     if quotes:
         return f"'{markup}'"
     return markup
 
 
 def new_type(
     _type: UnionType | type | GenericAlias | LiteralGenericAlias,
     parents: list[str]
-) -> CFGGenericAlias | CFGUnionType | CFGType:
+) -> CFGGenericAlias | CFGUnionType | CFGType | CFGLiteral:
     """Generate a config validation type from a new_type."""
 
     if isinstance(_type, UnionType):
         return CFGUnionType(_type, parents)
     if isinstance(_type, GenericAlias):
         return CFGGenericAlias.new(_type, parents)
     if isinstance(_type, LiteralGenericAlias):
@@ -99,41 +99,41 @@
 def parse_valid_value(
         _type: CFGType | CFGUnionType | CFGGenericAlias | type,
         value: Any
 ):
     """Parse the config value, if it is one of the special config types then
     return the transformed value.
     """
-    if isinstance(_type, CFGType) and _type.type == Path or _type == Path:
-        return Path.normalize(value)
+    if isinstance(_type, CFGType) and _type.type == TypePath or _type == TypePath:
+        return TypePath.normalize(value)
     return value
 
 
 def is_reserved(_type):
-    return _type in [Path]
+    return _type in [TypePath]
 
 
 def validate_reserved(value, _type, parents):
-    if _type == Path:
+    if _type == TypePath:
         if not isinstance(value, str):
             raise TypeError(
                 f"{ppath(*parents, spr='.')}; invalid type \
 {ptype(type(value).__name__)}, expected {ptype('str')}"
             )
-        return Path.normalize(value)
+        return TypePath.normalize(value)
 
 
-valid_type = (int, float, bool, str, list, dict, Path)
+valid_type = (int, float, bool, str, list, dict, TypePath)
 
 
 class CFGGenericAlias:
     """Base type that can validate a value."""
 
     @staticmethod
-    def new(_type: GenericAlias, parents: list[str]) -> GenericAlias:
+    def new(_type: GenericAlias, parents: list[str]) -> CFGGenericAlias:
         """Create a specific generic alias config validation type from a
         GenericAlias type hint.
         """
 
         name = re.match(
             r"(?:typing.*)?(?P<name>set|dict|list|tuple)\[.+\]",
             str(_type),
@@ -392,30 +392,30 @@
 
 class CFGLiteral:
     """Represents a literal option for the configuration type.
     Coniguration value must match one of the literal values in this literal
     type.
     """
 
-    def __init__(self, literal: Literal, parents: list[str]):
+    def __init__(self, literal: LiteralGenericAlias, parents: list[str]):
         self.literals = literal.__args__
 
     def default(self) -> Any:
         """Default value of the literal type. Will
         be the first value of the typing.Literal type.
         """
         return self.literals[0]
 
     def validate(self, value: Any, parents: list[str]) -> bool:
         """Validate that a given value is one of the literal values.
         """
 
         for option in self.literals:
             if is_reserved(get_type(option)):
-                return validate_reserved(value, Path, parents)
+                return validate_reserved(value, TypePath, parents)
             if value == option:
                 return value
 
         raise TypeError(f"{ppath(*parents, spr='.')}; invalid value \
 {p_value(value)}, expected one of: \
 {p_value(self.literals)}")
 
@@ -568,27 +568,27 @@
             if data["default"] == MISSING:
                 if (
                     not isinstance(data["type"], CFGType)
                     or cfg not in data["type"].type.__bases__
                 ):
                     data["default"] = data["type"].default()
 
-            if isinstance(data["default"], Path):
-                data["type"] = parse_type(Path, [*parents, attr])
+            if isinstance(data["default"], TypePath):
+                data["type"] = parse_type(TypePath, [*parents, attr])
                 data["default"] = str(data["default"])
 
             setattr(self, attr, data["default"])
 
         setattr(self, "__tcfg_values__", __tcfg_values__)
 
     def __tcfg_attributes__(self):
         """Parse and normalize tcfg class attributes for a given object."""
 
         # Normalize the seperators in the _path_ and strip `/` from the ends
-        _path_ = Path.normalize(getattr(self, "_path_") or "")
+        _path_ = TypePath.normalize(getattr(self, "_path_") or "")
         setattr(self, "_path_", _path_ if _path_ != "" else MISSING)
 
     def __validate__(self, data: dict, parents: list[str] = None):
         """Validate the values from the configuration dict and set the values
         accordingly.
         """
```

### Comparing `tcfg-0.4.3/tcfg/reserved.py` & `tcfg-0.4.4/tcfg/reserved.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
 
 __all__ = [
     "MISSING",
-    "Path",
+    "TypePath",
 ]
 
 
 class Missing:
     """Placeholding for missing values. Allows for null values to be
     represented as literals.
     """
 
 
 MISSING = Missing()
 
 
-class Path:
+class TypePath(str):
     """Allows for eazy path generation."""
 
     def __init__(self, *paths: str, strip: bool = True) -> None:
-        self.path = Path.normalize(
+        self.path = TypePath.normalize(
             *paths, strip=strip) if len(paths) > 0 else ""
 
     @staticmethod
     def normalize(*paths: str, strip: bool = True) -> str:
         """Normalize a path or segments of a path into a consistant path with
         `\\` replaced with `/` and either leading and trailing `/` stripped or
         left alone.
@@ -43,17 +43,17 @@
                     path.replace("\\", "/").strip("/")
                     for path in paths[1:-1]
                 ],
                 paths[-1].lstrip("/")
             ]
         )
 
-    def __truediv__(self, scalar: Path):
-        if isinstance(scalar, Path):
-            return Path(self.path.rstrip("/") + "/" + scalar.path.lstrip("/"))
+    def __truediv__(self, scalar: TypePath):
+        if isinstance(scalar, TypePath):
+            return TypePath(self.path.rstrip("/") + "/" + scalar.path.lstrip("/"))
         raise TypeError("Can't divide with values other that 'Path'")
 
     def __repr__(self) -> str:
         return f"Path({self.path!r})"
 
     def __str__(self) -> str:
         return self.path
```

### Comparing `tcfg-0.4.3/LICENSE` & `tcfg-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tcfg-0.4.3/README.md` & `tcfg-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `tcfg-0.4.3/pyproject.toml` & `tcfg-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tcfg"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
     { name="Tired Fox", email="zboehm104@gmail.com"}
 ]
 description="Typed dataclass like configuration objects"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.7"
```

### Comparing `tcfg-0.4.3/PKG-INFO` & `tcfg-0.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcfg
-Version: 0.4.3
+Version: 0.4.4
 Summary: Typed dataclass like configuration objects
 Project-URL: Homepage, https://github.com/Tired-Fox/tcfg
 Project-URL: Documentation, https://tired-fox.github.io/tcfg
 Author-email: Tired Fox <zboehm104@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

