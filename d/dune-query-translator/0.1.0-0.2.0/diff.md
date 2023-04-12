# Comparing `tmp/dune_query_translator-0.1.0.tar.gz` & `tmp/dune_query_translator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_query_translator-0.1.0.tar", max compression
+gzip compressed data, was "dune_query_translator-0.2.0.tar", max compression
```

## Comparing `dune_query_translator-0.1.0.tar` & `dune_query_translator-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1061 2023-04-11 13:36:16.153977 dune_query_translator-0.1.0/LICENSE
--rw-r--r--   0        0        0     1155 2023-04-11 13:36:16.153977 dune_query_translator-0.1.0/README.md
--rw-r--r--   0        0        0      643 2023-04-11 13:36:36.834942 dune_query_translator-0.1.0/dune/translate/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0    22452 2023-04-11 13:36:36.838942 dune_query_translator-0.1.0/dune/translate/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0        0        0     2492 2023-04-11 13:36:36.614935 dune_query_translator-0.1.0/dune/translate/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0       54 2023-04-11 13:36:16.153977 dune_query_translator-0.1.0/dune/translate/constants.py
--rw-r--r--   0        0        0      101 2023-04-11 13:36:16.153977 dune_query_translator-0.1.0/dune/translate/errors.py
--rw-r--r--   0        0        0    19878 2023-04-11 13:36:16.153977 dune_query_translator-0.1.0/dune/translate/helpers.py
--rw-r--r--   0        0        0     2203 2023-04-11 13:36:16.153977 dune_query_translator-0.1.0/dune/translate/translate.py
--rw-r--r--   0        0        0      504 2023-04-11 13:36:16.153977 dune_query_translator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 dune_query_translator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-12 11:19:43.090427 dune_query_translator-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1155 2023-04-12 11:19:43.090427 dune_query_translator-0.2.0/README.md
+-rw-r--r--   0        0        0      643 2023-04-12 11:20:01.414722 dune_query_translator-0.2.0/dune/translate/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0    22956 2023-04-12 11:20:01.414722 dune_query_translator-0.2.0/dune/translate/__pycache__/helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     2580 2023-04-12 11:20:01.234719 dune_query_translator-0.2.0/dune/translate/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0       54 2023-04-12 11:19:43.090427 dune_query_translator-0.2.0/dune/translate/constants.py
+-rw-r--r--   0        0        0      101 2023-04-12 11:19:43.090427 dune_query_translator-0.2.0/dune/translate/errors.py
+-rw-r--r--   0        0        0    20268 2023-04-12 11:19:43.090427 dune_query_translator-0.2.0/dune/translate/helpers.py
+-rw-r--r--   0        0        0     2271 2023-04-12 11:19:43.090427 dune_query_translator-0.2.0/dune/translate/translate.py
+-rw-r--r--   0        0        0      504 2023-04-12 11:19:43.090427 dune_query_translator-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1497 1970-01-01 00:00:00.000000 dune_query_translator-0.2.0/PKG-INFO
```

### Comparing `dune_query_translator-0.1.0/LICENSE` & `dune_query_translator-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_query_translator-0.1.0/README.md` & `dune_query_translator-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dune_query_translator-0.1.0/dune/translate/__pycache__/errors.cpython-311.pyc` & `dune_query_translator-0.2.0/dune/translate/__pycache__/errors.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x50623564 (Tue Apr 11 13:36:16 2023 UTC)
+moddate:  0xcf933664 (Wed Apr 12 11:19:43 2023 UTC)
 files sz: 101
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `dune_query_translator-0.1.0/dune/translate/__pycache__/helpers.cpython-311.pyc` & `dune_query_translator-0.2.0/dune/translate/__pycache__/helpers.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x50623564 (Tue Apr 11 13:36:16 2023 UTC)
-files sz: 19878
+moddate:  0xcf933664 (Wed Apr 12 11:19:43 2023 UTC)
+files sz: 20268
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064016c035a
@@ -12,16 +12,16 @@
       020000ab0200000000000000005a070200650265066408ac07a6020000ab
       0200000000000000005a080200650265066409ac07a6020000ab02000000
       00000000005a09020065026506640aac07a6020000ab0200000000000000
       005a0a020065026506640bac07a6020000ab0200000000000000005a0b64
       0c84005a0c640d5a0d640e5a0e640f650d9b009d025a0f650e9b00640f9d
       025a10641084005a11641184005a12641284005a13641384005a14641484
       005a15641584005a16641684005a17641784005a18641884005a19641984
-      005a1a641a84005a1b641b84005a1c641c84005a1d641d84005a1e640153
-      00
+      005a1a641a84005a1b641b84005a1c641c84005a1d641d84005a1e641e84
+      005a1f64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (re)
                  8 STORE_NAME               0 (re)
    
@@ -160,23 +160,27 @@
                274 MAKE_FUNCTION            0
                276 STORE_NAME              27 (bytea2numeric)
    
    406         278 LOAD_CONST              27 (<code object fix_bytearray_param, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 406>)
                280 MAKE_FUNCTION            0
                282 STORE_NAME              28 (fix_bytearray_param)
    
-   412         284 LOAD_CONST              28 (<code object transforms, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 412>)
+   412         284 LOAD_CONST              28 (<code object fix_bytearray_lower, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 412>)
                286 MAKE_FUNCTION            0
-               288 STORE_NAME              29 (transforms)
+               288 STORE_NAME              29 (fix_bytearray_lower)
    
-   452         290 LOAD_CONST              29 (<code object add_warnings_and_banner, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 452>)
+   421         290 LOAD_CONST              29 (<code object transforms, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 421>)
                292 MAKE_FUNCTION            0
-               294 STORE_NAME              30 (add_warnings_and_banner)
-               296 LOAD_CONST               1 (None)
-               298 RETURN_VALUE
+               294 STORE_NAME              30 (transforms)
+   
+   461         296 LOAD_CONST              30 (<code object add_warnings_and_banner, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 461>)
+               298 MAKE_FUNCTION            0
+               300 STORE_NAME              31 (add_warnings_and_banner)
+               302 LOAD_CONST               1 (None)
+               304 RETURN_VALUE
    consts
       0
       None
       ('partial',)
       code
          argcount  : 1
          nlocals   : 7
@@ -2683,14 +2687,55 @@
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
          name       'fix_bytearray_param'
          firstlineno 406
          lnotab 0x02020401
       code
+         argcount  : 1
+         nlocals   : 3
+         stacksize : 6
+         flags     : 3
+         code
+            0x970064017d017401000000000000000000006a0100000000000000007c
+            0164027c007400000000000000000000006a020000000000000000ac03a6
+            040000ab0400000000000000007d027c025300
+         412           0 RESUME                   0
+         
+         416           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)')
+                       4 STORE_FAST               1 (pattern)
+         
+         417           6 LOAD_GLOBAL              1 (NULL + re)
+                      18 LOAD_ATTR                1 (sub)
+                      28 LOAD_FAST                1 (pattern)
+                      30 LOAD_CONST               2 ('0x\\1')
+                      32 LOAD_FAST                0 (query)
+                      34 LOAD_GLOBAL              0 (re)
+                      46 LOAD_ATTR                2 (IGNORECASE)
+                      56 KW_NAMES                 3
+                      58 PRECALL                  4
+                      62 CALL                     4
+                      72 STORE_FAST               2 (substituted)
+         
+         418          74 LOAD_FAST                2 (substituted)
+                      76 RETURN_VALUE
+         consts
+            "Remove lower function call around '0x...' string literals, and remove the string since we have native hex types.\n\n    This has to happen after SQLGlot, since it will parse a bare 0x as a string literal"
+            'lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)'
+            '0x\\1'
+            ('flags',)
+         names      ('re', 'sub', 'IGNORECASE')
+         varnames   ('query', 'pattern', 'substituted')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         name       'fix_bytearray_lower'
+         firstlineno 412
+         lnotab 0x020404014401
+      code
          argcount  : 3
          nlocals   : 6
          stacksize : 12
          flags     : 3
          code
             0x97007c0164016b0200000000727a740000000000000000000000740200
             000000000000000000740400000000000000000000740600000000000000
@@ -2702,111 +2747,111 @@
             00000000007c03741c00000000000000000000741e000000000000000000
             00742000000000000000000000670c7d046e2c740e000000000000000000
             007410000000000000000000007412000000000000000000007414000000
             000000000000007416000000000000000000007418000000000000000000
             0074200000000000000000000067077d047c0444005d177d057c00a01100
             000000000000000000000000000000000000007c05a6010000ab01000000
             00000000007d008c187c005300
-         412           0 RESUME                   0
+         421           0 RESUME                   0
          
-         414           2 LOAD_FAST                1 (dialect)
+         423           2 LOAD_FAST                1 (dialect)
                        4 LOAD_CONST               1 ('postgres')
                        6 COMPARE_OP               2 (==)
                       12 POP_JUMP_FORWARD_IF_FALSE   122 (to 258)
          
-         417          14 LOAD_GLOBAL              0 (chain_where_gnosis)
+         426          14 LOAD_GLOBAL              0 (chain_where_gnosis)
          
-         418          26 LOAD_GLOBAL              2 (chain_where_optimism)
+         427          26 LOAD_GLOBAL              2 (chain_where_optimism)
          
-         419          38 LOAD_GLOBAL              4 (chain_where_bnb)
+         428          38 LOAD_GLOBAL              4 (chain_where_bnb)
          
-         420          50 LOAD_GLOBAL              6 (chain_where_polygon)
+         429          50 LOAD_GLOBAL              6 (chain_where_polygon)
          
-         416          62 LOAD_CONST               2 (('gnosis', 'optimism', 'bnb', 'polygon'))
+         425          62 LOAD_CONST               2 (('gnosis', 'optimism', 'bnb', 'polygon'))
                       64 BUILD_CONST_KEY_MAP      4
          
-         421          66 LOAD_METHOD              4 (get)
+         430          66 LOAD_METHOD              4 (get)
                       88 LOAD_FAST                2 (dataset)
                       90 LOAD_GLOBAL             10 (chain_where_ethereum)
                      102 PRECALL                  2
                      106 CALL                     2
          
-         416         116 STORE_FAST               3 (chain_where)
+         425         116 STORE_FAST               3 (chain_where)
          
-         423         118 LOAD_GLOBAL             12 (table_replacement)
+         432         118 LOAD_GLOBAL             12 (table_replacement)
          
-         424         130 LOAD_GLOBAL             14 (interval_fix)
+         433         130 LOAD_GLOBAL             14 (interval_fix)
          
-         425         142 LOAD_GLOBAL             16 (fix_boolean)
+         434         142 LOAD_GLOBAL             16 (fix_boolean)
          
-         426         154 LOAD_GLOBAL             18 (cast_numeric)
+         435         154 LOAD_GLOBAL             18 (cast_numeric)
          
-         427         166 LOAD_GLOBAL             20 (cast_timestamp)
+         436         166 LOAD_GLOBAL             20 (cast_timestamp)
          
-         428         178 LOAD_GLOBAL             22 (warn_unnest)
+         437         178 LOAD_GLOBAL             22 (warn_unnest)
          
-         429         190 LOAD_GLOBAL             24 (warn_sequence)
+         438         190 LOAD_GLOBAL             24 (warn_sequence)
          
-         430         202 LOAD_GLOBAL             26 (dex_trades_fixes)
+         439         202 LOAD_GLOBAL             26 (dex_trades_fixes)
          
-         431         214 LOAD_FAST                3 (chain_where)
+         440         214 LOAD_FAST                3 (chain_where)
          
-         432         216 LOAD_GLOBAL             28 (bytearray_parameter_fix)
+         441         216 LOAD_GLOBAL             28 (bytearray_parameter_fix)
          
-         433         228 LOAD_GLOBAL             30 (spell_rename)
+         442         228 LOAD_GLOBAL             30 (spell_rename)
          
-         434         240 LOAD_GLOBAL             32 (bytea2numeric)
+         443         240 LOAD_GLOBAL             32 (bytea2numeric)
          
-         422         252 BUILD_LIST              12
+         431         252 BUILD_LIST              12
                      254 STORE_FAST               4 (transform_order)
                      256 JUMP_FORWARD            44 (to 346)
          
-         438     >>  258 LOAD_GLOBAL             14 (interval_fix)
+         447     >>  258 LOAD_GLOBAL             14 (interval_fix)
          
-         439         270 LOAD_GLOBAL             16 (fix_boolean)
+         448         270 LOAD_GLOBAL             16 (fix_boolean)
          
-         440         282 LOAD_GLOBAL             18 (cast_numeric)
+         449         282 LOAD_GLOBAL             18 (cast_numeric)
          
-         441         294 LOAD_GLOBAL             20 (cast_timestamp)
+         450         294 LOAD_GLOBAL             20 (cast_timestamp)
          
-         442         306 LOAD_GLOBAL             22 (warn_unnest)
+         451         306 LOAD_GLOBAL             22 (warn_unnest)
          
-         443         318 LOAD_GLOBAL             24 (warn_sequence)
+         452         318 LOAD_GLOBAL             24 (warn_sequence)
          
-         444         330 LOAD_GLOBAL             32 (bytea2numeric)
+         453         330 LOAD_GLOBAL             32 (bytea2numeric)
          
-         437         342 BUILD_LIST               7
+         446         342 BUILD_LIST               7
                      344 STORE_FAST               4 (transform_order)
          
-         447     >>  346 LOAD_FAST                4 (transform_order)
+         456     >>  346 LOAD_FAST                4 (transform_order)
                      348 GET_ITER
                  >>  350 FOR_ITER                23 (to 398)
                      352 STORE_FAST               5 (f)
          
-         448         354 LOAD_FAST                0 (query_tree)
+         457         354 LOAD_FAST                0 (query_tree)
                      356 LOAD_METHOD             17 (transform)
                      378 LOAD_FAST                5 (f)
                      380 PRECALL                  1
                      384 CALL                     1
                      394 STORE_FAST               0 (query_tree)
                      396 JUMP_BACKWARD           24 (to 350)
          
-         449     >>  398 LOAD_FAST                0 (query_tree)
+         458     >>  398 LOAD_FAST                0 (query_tree)
                      400 RETURN_VALUE
          consts
             'Apply several transforms to the query in order. Each transform takes and returns a sqlglot.Expression'
             'postgres'
             ('gnosis', 'optimism', 'bnb', 'polygon')
          names      ('chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'get', 'chain_where_ethereum', 'table_replacement', 'interval_fix', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'dex_trades_fixes', 'bytearray_parameter_fix', 'spell_rename', 'bytea2numeric', 'transform')
          varnames   ('query_tree', 'dialect', 'dataset', 'chain_where', 'transform_order', 'f')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
          name       'transforms'
-         firstlineno 412
+         firstlineno 421
          lnotab
             0x02020c030c010c010c010cfc040532fb02070c010c010c010c010c010c
             010c010c0102010c010c010cf406100c010c010c010c010c010c010cf904
             0a08012c01
       code
          argcount  : 1
          nlocals   : 1
@@ -2815,66 +2860,66 @@
          code
             0x970064017c00a0000000000000000000000000000000000000000000a6
             000000ab0000000000000000007600720564027c007a0000007d00740300
             0000000000000000006a02000000000000000064037c00a6020000ab0200
             00000000000000720564047c007a0000007d0064057c00a0000000000000
             000000000000000000000000000000a6000000ab00000000000000000076
             00720564067c007a0000007d0064077c007a0000005300
-         452           0 RESUME                   0
+         461           0 RESUME                   0
          
-         454           2 LOAD_CONST               1 ("lower('{{")
+         463           2 LOAD_CONST               1 ("lower('{{")
                        4 LOAD_FAST                0 (query)
                        6 LOAD_METHOD              0 (lower)
                       28 PRECALL                  0
                       32 CALL                     0
                       42 CONTAINS_OP              0
                       44 POP_JUMP_FORWARD_IF_FALSE     5 (to 56)
          
-         456          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
+         465          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
          
-         459          48 LOAD_FAST                0 (query)
+         468          48 LOAD_FAST                0 (query)
          
-         455          50 BINARY_OP                0 (+)
+         464          50 BINARY_OP                0 (+)
                       54 STORE_FAST               0 (query)
          
-         462     >>   56 LOAD_GLOBAL              3 (NULL + re)
+         471     >>   56 LOAD_GLOBAL              3 (NULL + re)
                       68 LOAD_ATTR                2 (search)
                       78 LOAD_CONST               3 ('\\[.*\\]')
                       80 LOAD_FAST                0 (query)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 POP_JUMP_FORWARD_IF_FALSE     5 (to 108)
          
-         464          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
+         473          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
          
-         467         100 LOAD_FAST                0 (query)
+         476         100 LOAD_FAST                0 (query)
          
-         463         102 BINARY_OP                0 (+)
+         472         102 BINARY_OP                0 (+)
                      106 STORE_FAST               0 (query)
          
-         469     >>  108 LOAD_CONST               5 ('dune_user_generated')
+         478     >>  108 LOAD_CONST               5 ('dune_user_generated')
                      110 LOAD_FAST                0 (query)
                      112 LOAD_METHOD              0 (lower)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 CONTAINS_OP              0
                      150 POP_JUMP_FORWARD_IF_FALSE     5 (to 162)
          
-         471         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
+         480         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
          
-         474         154 LOAD_FAST                0 (query)
+         483         154 LOAD_FAST                0 (query)
          
-         470         156 BINARY_OP                0 (+)
+         479         156 BINARY_OP                0 (+)
                      160 STORE_FAST               0 (query)
          
-         478     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
+         487     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
          
-         481         164 LOAD_FAST                0 (query)
+         490         164 LOAD_FAST                0 (query)
          
-         477         166 BINARY_OP                0 (+)
+         486         166 BINARY_OP                0 (+)
                      170 RETURN_VALUE
          consts
             "Add a success banner at the top, and look for a few cases of things we don't fix and add a warning if present"
             "lower('{{"
             "/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n"
             '\\[.*\\]'
             '/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n'
@@ -2883,22 +2928,22 @@
             "/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n"
          names      ('lower', 're', 'search')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
          name       'add_warnings_and_banner'
-         firstlineno 452
+         firstlineno 461
          lnotab
             0x02022c02020302fc06072a02020302fc06062c02020302fc0608020302
             fc
-   names      ('re', 'functools', 'partial', 'sqlglot', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'quoted_param_left_placeholder', 'quoted_param_right_placeholder', 'interval_fix', 'bytearray_parameter_fix', 'table_replacement', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'prep_query', 'spell_rename', 'bytea2numeric', 'fix_bytearray_param', 'transforms', 'add_warnings_and_banner')
+   names      ('re', 'functools', 'partial', 'sqlglot', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'quoted_param_left_placeholder', 'quoted_param_right_placeholder', 'interval_fix', 'bytearray_parameter_fix', 'table_replacement', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'prep_query', 'spell_rename', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'transforms', 'add_warnings_and_banner')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108010c0208030612065c06121a011a011a011a011a03062b04
       0104010a010a03062c061b06290609060e060a060e060e06170605060e06
-      060628
+      0606090628
```

### Comparing `dune_query_translator-0.1.0/dune/translate/helpers.py` & `dune_query_translator-0.2.0/dune/translate/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,14 +405,23 @@
 
 def fix_bytearray_param(query):
     """Remove lower function call from bytearray parameters"""
     pattern = r"lower\(\s*['\"]\{\{(.*?)\}\}['\"]\s*\)"
     return re.sub(pattern, r"{{\1}}", query, flags=re.IGNORECASE)
 
 
+def fix_bytearray_lower(query):
+    """Remove lower function call around '0x...' string literals, and remove the string since we have native hex types.
+
+    This has to happen after SQLGlot, since it will parse a bare 0x as a string literal"""
+    pattern = r"lower\(\s*['\"]0x(.*?)['\"]\s*\)"
+    substituted = re.sub(pattern, r"0x\1", query, flags=re.IGNORECASE)
+    return substituted
+
+
 def transforms(query_tree, dialect, dataset):
     """Apply several transforms to the query in order. Each transform takes and returns a sqlglot.Expression"""
     if dialect == "postgres":
         # Add an appropriate blockchain = '<chain>' filter for trades, tokens, and prices tables.
         chain_where = {
             "gnosis": chain_where_gnosis,
             "optimism": chain_where_optimism,
```

### Comparing `dune_query_translator-0.1.0/dune/translate/translate.py` & `dune_query_translator-0.2.0/dune/translate/translate.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from dune.translate.helpers import (
     prep_query,
     quoted_param_left_placeholder,
     quoted_param_right_placeholder,
     add_warnings_and_banner,
     transforms,
     fix_bytearray_param,
+    fix_bytearray_lower,
 )
 
 
 def translate(query, dialect, dataset):
     """Translate a query into DuneSQL"""
     if dialect not in ("spark", "postgres"):
         raise ValueError(f"Unknown dialect: {dialect}")
@@ -30,14 +31,15 @@
         query_tree = prep_query(query, sqlglot_dialect)
         query_tree = transforms(query_tree, sqlglot_dialect, dataset)
         query = query_tree.sql(dialect="trino", pretty=True)
 
         # Replace placeholders with Dune params again
         query = query.replace(quoted_param_left_placeholder, "{{").replace(quoted_param_right_placeholder, "}}")
         query = fix_bytearray_param(query)
+        query = fix_bytearray_lower(query)
 
         return add_warnings_and_banner(query)
     except ParseError as e:
         # SQLGlot inserts terminal style colors to emphasize error location.
         # We remove these, as they mess up the formatting.
         # Also, don't leak intermediate param syntax in error message
         error_message = (
```

### Comparing `dune_query_translator-0.1.0/PKG-INFO` & `dune_query_translator-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-query-translator
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Vegard Stikbakke
 Author-email: vegard@dune.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlglot (>=11.4.4,<12.0.0)
```

