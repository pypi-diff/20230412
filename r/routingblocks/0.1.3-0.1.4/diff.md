# Comparing `tmp/routingblocks-0.1.3.tar.gz` & `tmp/routingblocks-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routingblocks-0.1.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "routingblocks-0.1.4.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `routingblocks-0.1.3.tar` & `routingblocks-0.1.4.tar`

### file list

```diff
@@ -1,265 +1,269 @@
--rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 routingblocks-0.1.3/.clang-format
--rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 routingblocks-0.1.3/.cmake-format
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.3/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     2109 2022-11-09 12:37:21.000000 routingblocks-0.1.3/.gitignore
--rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 routingblocks-0.1.3/.readthedocs.yaml
--rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 routingblocks-0.1.3/CMakeLists.txt
--rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 routingblocks-0.1.3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1866 2022-11-09 12:37:21.000000 routingblocks-0.1.3/README.md
--rw-r--r--   0        0        0     2753 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/CMakeLists.txt
--rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/include/routingblocks_bindings/Evaluation.h
--rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/include/routingblocks_bindings/Instance.hpp
--rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/include/routingblocks_bindings/Labeling.h
--rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/include/routingblocks_bindings/LocalSearch.h
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/include/routingblocks_bindings/Operators.h
--rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/include/routingblocks_bindings/Solution.h
--rw-r--r--   0        0        0     3697 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/include/routingblocks_bindings/binding_helpers.hpp
--rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/include/routingblocks_bindings/large_neighborhood.h
--rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/include/routingblocks_bindings/utility.h
--rw-r--r--   0        0        0    15340 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/src/Evaluation.cpp
--rw-r--r--   0        0        0     5514 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/src/Instance.cpp
--rw-r--r--   0        0        0     6141 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/src/Labeling.cpp
--rw-r--r--   0        0        0     3492 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/src/LocalSearch.cpp
--rw-r--r--   0        0        0    10602 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/src/Operators.cpp
--rw-r--r--   0        0        0    23365 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/src/Solution.cpp
--rw-r--r--   0        0        0     1175 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/src/bindings.cpp
--rw-r--r--   0        0        0    10923 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/src/large_neighborhood.cpp
--rw-r--r--   0        0        0     6155 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/src/utility.cpp
--rwxr-xr-x   0        0        0      192 2022-11-09 12:37:21.000000 routingblocks-0.1.3/bindings/stubgen.py
--rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/make.bat
--rw-r--r--   0        0        0       10 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/alns.rst
--rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/auxilliary.rst
--rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/concepts.rst
--rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/conf.py
--rw-r--r--   0        0        0      726 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/development.rst
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/evaluation.rst
--rw-r--r--   0        0        0       29 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/examples.rst
--rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/extension.rst
--rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/frvcp.rst
--rw-r--r--   0        0        0    14649 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/getting_started.rst
--rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/index.rst
--rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/instance.rst
--rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/localsearch.rst
--rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/routingblocks.rst
--rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/solution.rst
--rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 routingblocks-0.1.3/docs/source/usage.rst
--rw-r--r--   0        0        0      427 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/README.md
--rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/README.md
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/__init__.py
--rw-r--r--   0        0        0     3260 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/__main__.py
--rw-r--r--   0        0        0    17856 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/alns.py
--rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/config.json
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instance/__init__.py
--rw-r--r--   0        0        0     2061 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instance/interface.py
--rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instance/models.py
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instance/parsing.py
--rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/c101C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/c104C10.txt
--rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/c202C10.txt
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/c205C10.txt
--rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/r102C10.txt
--rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/r103C10.txt
--rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/r201C10.txt
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/r203C10.txt
--rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/rc102C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/rc108C10.txt
--rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/rc201C10.txt
--rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/rc205C10.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c105_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c108_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c109_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c201_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c202_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c203_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c204_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c205_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c206_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c207_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c208_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r105_21.txt
--rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r108_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r109_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r110_21.txt
--rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r111_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r112_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r201_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r202_21.txt
--rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r203_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r204_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r205_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r206_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r207_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r208_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r209_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r210_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r211_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc102_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc103_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc104_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc105_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc106_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc107_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc108_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc201_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc202_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc203_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc204_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc205_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc206_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc207_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc208_21.txt
--rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/c103C15.txt
--rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/c106C15.txt
--rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/c202C15.txt
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/c208C15.txt
--rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/r102C15.txt
--rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/r105C15.txt
--rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/r202C15.txt
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/r209C15.txt
--rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/rc103C15.txt
--rw-r--r--   0        0        0     2119 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/rc108C15.txt
--rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/rc202C15.txt
--rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/rc204C15.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/c101C5.txt
--rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/c103C5.txt
--rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/c206C5.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/c208C5.txt
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/r104C5.txt
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/r105C5.txt
--rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/r202C5.txt
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/r203C5.txt
--rw-r--r--   0        0        0     1139 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/rc105C5.txt
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/rc108C5.txt
--rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/rc204C5.txt
--rw-r--r--   0        0        0     1053 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/rc208C5.txt
--rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/instances/evrptw/README.txt
--rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/operators/ShawMoveSelector.py
--rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/operators/ShawRelatedness.py
--rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/operators/SpatioTemporalRelatedness.py
--rw-r--r--   0        0        0     2069 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/operators/__init__.py
--rw-r--r--   0        0        0     1269 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/parameters.py
--rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/requirements.txt
--rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/utility/__init__.py
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/evrptw/utility/algorithms.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/ils/__init__.py
--rw-r--r--   0        0        0      864 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/ils/__main__.py
--rw-r--r--   0        0        0     3643 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/ils/ils.py
--rw-r--r--   0        0        0     2949 2022-11-09 12:37:21.000000 routingblocks-0.1.3/examples/ils/parsing.py
--rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/CMakeLists.txt
--rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/cmake/CPM.cmake
--rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/cmake/tools.cmake
--rw-r--r--   0        0        0    23647 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/ADPTWEvaluation.h
--rw-r--r--   0        0        0    14819 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/FRVCP.h
--rw-r--r--   0        0        0     2827 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/Instance.h
--rw-r--r--   0        0        0    11828 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/LocalSearch.h
--rw-r--r--   0        0        0     6234 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/NIFTWEvaluation.h
--rw-r--r--   0        0        0    28881 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/Solution.h
--rw-r--r--   0        0        0     5120 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/adaptive_large_neighborhood.hpp
--rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/arc.h
--rw-r--r--   0        0        0     8674 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/evaluation.h
--rw-r--r--   0        0        0    11760 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/insertion_cache.h
--rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/lns_operators.h
--rw-r--r--   0        0        0     3008 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/node.h
--rw-r--r--   0        0        0     4085 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/operators/InsertStationOperator.h
--rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/operators/InterRouteTwoOptOperator.h
--rw-r--r--   0        0        0     3158 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/operators/RemoveStationOperator.h
--rw-r--r--   0        0        0    15813 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/operators/SwapOperator.h
--rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/operators.h
--rw-r--r--   0        0        0     5054 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/removal_cache.h
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/types.h
--rw-r--r--   0        0        0     8032 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/utility/adaptive_priority_list.h
--rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/utility/algorithms.h
--rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/utility/arc_set.h
--rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/utility/heap.h
--rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/utility/iterator_pair.h
--rw-r--r--   0        0        0     3727 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/utility/random.h
--rw-r--r--   0        0        0     1357 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/include/routingblocks/vertex.h
--rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/CMakeLists.txt
--rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/dynamic_bitset/CMakeLists.txt
--rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/dynamic_bitset/LICENSE.txt
--rw-r--r--   0        0        0   117337 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp
--rw-r--r--   0        0        0    20974 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h
--rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/small_vector/CMakeLists.txt
--rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/small_vector/LICENSE.txt
--rw-r--r--   0        0        0   241472 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/small_vector/small_vector/small_vector.hpp
--rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/xoshiro/CMakeLists.txt
--rw-r--r--   0        0        0     1090 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/xoshiro/LICENSE.txt
--rw-r--r--   0        0        0    49824 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/lib/xoshiro/xoshiro/xoshiro.h
--rw-r--r--   0        0        0     3302 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/ADPTWEvaluation.cpp
--rw-r--r--   0        0        0        1 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/FRVCP.cpp
--rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/Instance.cpp
--rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/LocalSearch.cpp
--rw-r--r--   0        0        0     8324 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/NIFTWEvaluation.cpp
--rw-r--r--   0        0        0     3773 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/Solution.cpp
--rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/adaptive_large_neighborbood.cpp
--rw-r--r--   0        0        0     4504 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/lns_operators.cpp
--rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/node.cpp
--rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/operators/InsertStationOperator.cpp
--rw-r--r--   0        0        0     2051 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/src/operators/InterRouteTwoOptOperator.cpp
--rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/test/CMakeLists.txt
--rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 routingblocks-0.1.3/native/test/src/dummy.cpp
--rw-r--r--   0        0        0     1330 2022-11-09 12:37:21.000000 routingblocks-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/__init__.py
--rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/operators/__init__.py
--rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/operators/best_insert.py
--rw-r--r--   0        0        0     4390 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/operators/cluster_removal.py
--rw-r--r--   0        0        0     1928 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/operators/move_selectors.py
--rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/operators/related_removal.py
--rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/operators/route_removal.py
--rw-r--r--   0        0        0     3835 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/operators/station_vicinity_removal.py
--rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/operators/worst_removal.py
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/utility/__init__.py
--rw-r--r--   0        0        0     2909 2022-11-09 12:37:21.000000 routingblocks-0.1.3/routingblocks/utility/instance_builder.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/benchmarks/__init__.py
--rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/benchmarks/reference/insertion_cache.py
--rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/benchmarks/reference/removal_cache.py
--rw-r--r--   0        0        0     1191 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/benchmarks/test_benchmark_frvcp.py
--rw-r--r--   0        0        0     2006 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/benchmarks/test_benchmark_local_search.py
--rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/benchmarks/test_benchmark_removal_cache.py
--rw-r--r--   0        0        0     9867 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/benchmarks/test_benchmark_route_update.py
--rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/conftest.py
--rw-r--r--   0        0        0     5570 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/fixtures/data/c101C5.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/fixtures/data/c101_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/fixtures/data/r101_21.txt
--rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/fixtures/data/r201_21.txt
--rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/fixtures/data/rc101_21.txt
--rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/fixtures/mock_evaluation.py
--rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/helpers/__init__.py
--rw-r--r--   0        0        0     2061 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/helpers/interface.py
--rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/helpers/models.py
--rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/helpers/parsing.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/operators/__init__.py
--rw-r--r--   0        0        0     7708 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/operators/test_cluster_removal.py
--rw-r--r--   0        0        0     1635 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/operators/test_random_insertion.py
--rw-r--r--   0        0        0     1815 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/operators/test_random_removal.py
--rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/operators/test_related_removal.py
--rw-r--r--   0        0        0     1904 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/operators/test_station_insertion.py
--rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/operators/test_station_removal.py
--rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/operators/test_station_vicinity_removal.py
--rw-r--r--   0        0        0    20342 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/operators/test_swap.py
--rw-r--r--   0        0        0     3851 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/test_evaluation.py
--rw-r--r--   0        0        0     4538 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/test_frvcp.py
--rw-r--r--   0        0        0     6394 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/test_insertion_cache.py
--rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/test_large_neighborhood.py
--rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/test_lns_helpers.py
--rw-r--r--   0        0        0     2622 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/test_local_search.py
--rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/test_node.py
--rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/test_removal_cache.py
--rw-r--r--   0        0        0    13948 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/test_route.py
--rw-r--r--   0        0        0    19901 2022-11-09 12:37:21.000000 routingblocks-0.1.3/test/tests/test_solution.py
--rw-r--r--   0        0        0     2905 2022-11-09 12:37:21.000000 routingblocks-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      467 2022-11-09 12:37:21.000000 routingblocks-0.1.4/.clang-format
+-rw-r--r--   0        0        0     1221 2022-11-09 12:37:21.000000 routingblocks-0.1.4/.cmake-format
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 routingblocks-0.1.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.4/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     2109 2022-11-09 12:37:21.000000 routingblocks-0.1.4/.gitignore
+-rw-r--r--   0        0        0      195 2022-11-09 12:37:21.000000 routingblocks-0.1.4/.readthedocs.yaml
+-rw-r--r--   0        0        0      436 2022-11-09 12:37:21.000000 routingblocks-0.1.4/CMakeLists.txt
+-rw-r--r--   0        0        0      675 2022-11-09 12:37:21.000000 routingblocks-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1866 2022-11-09 12:37:21.000000 routingblocks-0.1.4/README.md
+-rw-r--r--   0        0        0     2753 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/CMakeLists.txt
+-rw-r--r--   0        0        0      229 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/include/routingblocks_bindings/Evaluation.h
+-rw-r--r--   0        0        0      280 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/include/routingblocks_bindings/Instance.hpp
+-rw-r--r--   0        0        0      248 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/include/routingblocks_bindings/Labeling.h
+-rw-r--r--   0        0        0      359 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/include/routingblocks_bindings/LocalSearch.h
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/include/routingblocks_bindings/Operators.h
+-rw-r--r--   0        0        0      424 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/include/routingblocks_bindings/Solution.h
+-rw-r--r--   0        0        0     3697 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/include/routingblocks_bindings/binding_helpers.hpp
+-rw-r--r--   0        0        0      288 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/include/routingblocks_bindings/large_neighborhood.h
+-rw-r--r--   0        0        0      281 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/include/routingblocks_bindings/utility.h
+-rw-r--r--   0        0        0    15437 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/src/Evaluation.cpp
+-rw-r--r--   0        0        0     6117 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/src/Instance.cpp
+-rw-r--r--   0        0        0     6141 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/src/Labeling.cpp
+-rw-r--r--   0        0        0     3492 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/src/LocalSearch.cpp
+-rw-r--r--   0        0        0    10873 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/src/Operators.cpp
+-rw-r--r--   0        0        0    23365 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/src/Solution.cpp
+-rw-r--r--   0        0        0     1175 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/src/bindings.cpp
+-rw-r--r--   0        0        0    11013 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/src/large_neighborhood.cpp
+-rw-r--r--   0        0        0     6155 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/src/utility.cpp
+-rwxr-xr-x   0        0        0      192 2022-11-09 12:37:21.000000 routingblocks-0.1.4/bindings/stubgen.py
+-rw-r--r--   0        0        0      769 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/make.bat
+-rw-r--r--   0        0        0      596 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/alns.rst
+-rw-r--r--   0        0        0       83 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/auxilliary.rst
+-rw-r--r--   0        0        0       19 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/concepts.rst
+-rw-r--r--   0        0        0     1661 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/conf.py
+-rw-r--r--   0        0        0      734 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/development.rst
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/evaluation.rst
+-rw-r--r--   0        0        0       29 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/examples.rst
+-rw-r--r--   0        0        0       43 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/extension.rst
+-rw-r--r--   0        0        0       60 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/frvcp.rst
+-rw-r--r--   0        0        0    28078 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/getting_started.rst
+-rw-r--r--   0        0        0      534 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/index.rst
+-rw-r--r--   0        0        0       34 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/instance.rst
+-rw-r--r--   0        0        0       80 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/localsearch.rst
+-rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/routingblocks.rst
+-rw-r--r--   0        0        0      161 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/solution.rst
+-rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 routingblocks-0.1.4/docs/source/usage.rst
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/alns/__init__.py
+-rw-r--r--   0        0        0     1372 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/alns/__main__.py
+-rw-r--r--   0        0        0     4791 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/alns/alns.py
+-rw-r--r--   0        0        0     2949 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/alns/parsing.py
+-rw-r--r--   0        0        0      508 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/README.md
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/__init__.py
+-rw-r--r--   0        0        0     3260 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/__main__.py
+-rw-r--r--   0        0        0    18132 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/alns.py
+-rw-r--r--   0        0        0      838 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/config.json
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instance/__init__.py
+-rw-r--r--   0        0        0     2061 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instance/interface.py
+-rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instance/models.py
+-rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instance/parsing.py
+-rw-r--r--   0        0        0     1677 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/c101C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/c104C10.txt
+-rw-r--r--   0        0        0     1675 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/c202C10.txt
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/c205C10.txt
+-rw-r--r--   0        0        0     1577 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/r102C10.txt
+-rw-r--r--   0        0        0     1493 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/r103C10.txt
+-rw-r--r--   0        0        0     1585 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/r201C10.txt
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/r203C10.txt
+-rw-r--r--   0        0        0     1587 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/rc102C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/rc108C10.txt
+-rw-r--r--   0        0        0     1586 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/rc201C10.txt
+-rw-r--r--   0        0        0     1584 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/rc205C10.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c105_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c108_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c109_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c201_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c202_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c203_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c204_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c205_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c206_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c207_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c208_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r105_21.txt
+-rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r108_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r109_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r110_21.txt
+-rw-r--r--   0        0        0    11104 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r111_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r112_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r201_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r202_21.txt
+-rw-r--r--   0        0        0    11106 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r203_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r204_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r205_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r206_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r207_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r208_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r209_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r210_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r211_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc102_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc103_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc104_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc105_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc106_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc107_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc108_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc201_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc202_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc203_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc204_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc205_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc206_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc207_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc208_21.txt
+-rw-r--r--   0        0        0     2127 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/c103C15.txt
+-rw-r--r--   0        0        0     1938 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/c106C15.txt
+-rw-r--r--   0        0        0     2123 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/c202C15.txt
+-rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/c208C15.txt
+-rw-r--r--   0        0        0     2401 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/r102C15.txt
+-rw-r--r--   0        0        0     2205 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/r105C15.txt
+-rw-r--r--   0        0        0     2209 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/r202C15.txt
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/r209C15.txt
+-rw-r--r--   0        0        0     2129 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/rc103C15.txt
+-rw-r--r--   0        0        0     2119 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/rc108C15.txt
+-rw-r--r--   0        0        0     2124 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/rc202C15.txt
+-rw-r--r--   0        0        0     2300 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/rc204C15.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/c101C5.txt
+-rw-r--r--   0        0        0      959 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/c103C5.txt
+-rw-r--r--   0        0        0     1149 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/c206C5.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/c208C5.txt
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/r104C5.txt
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/r105C5.txt
+-rw-r--r--   0        0        0     1049 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/r202C5.txt
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/r203C5.txt
+-rw-r--r--   0        0        0     1139 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/rc105C5.txt
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/rc108C5.txt
+-rw-r--r--   0        0        0     1144 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/rc204C5.txt
+-rw-r--r--   0        0        0     1053 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/rc208C5.txt
+-rw-r--r--   0        0        0      995 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/instances/evrptw/README.txt
+-rw-r--r--   0        0        0      913 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/operators/ShawMoveSelector.py
+-rw-r--r--   0        0        0     1733 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/operators/ShawRelatedness.py
+-rw-r--r--   0        0        0     1189 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/operators/SpatioTemporalRelatedness.py
+-rw-r--r--   0        0        0     2069 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/operators/__init__.py
+-rw-r--r--   0        0        0     1269 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/parameters.py
+-rw-r--r--   0        0        0       21 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/requirements.txt
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/utility/__init__.py
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/evrptw/utility/algorithms.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/ils/__init__.py
+-rw-r--r--   0        0        0     1454 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/ils/__main__.py
+-rw-r--r--   0        0        0     4162 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/ils/ils.py
+-rw-r--r--   0        0        0     2949 2022-11-09 12:37:21.000000 routingblocks-0.1.4/examples/ils/parsing.py
+-rw-r--r--   0        0        0     2693 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/CMakeLists.txt
+-rw-r--r--   0        0        0    35623 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/cmake/CPM.cmake
+-rw-r--r--   0        0        0     1739 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/cmake/tools.cmake
+-rw-r--r--   0        0        0    23647 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/ADPTWEvaluation.h
+-rw-r--r--   0        0        0    14819 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/FRVCP.h
+-rw-r--r--   0        0        0     2827 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/Instance.h
+-rw-r--r--   0        0        0    11828 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/LocalSearch.h
+-rw-r--r--   0        0        0     6234 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/NIFTWEvaluation.h
+-rw-r--r--   0        0        0    28881 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/Solution.h
+-rw-r--r--   0        0        0     5120 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/adaptive_large_neighborhood.hpp
+-rw-r--r--   0        0        0      528 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/arc.h
+-rw-r--r--   0        0        0     8674 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/evaluation.h
+-rw-r--r--   0        0        0    11760 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/insertion_cache.h
+-rw-r--r--   0        0        0     2101 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/lns_operators.h
+-rw-r--r--   0        0        0     3008 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/node.h
+-rw-r--r--   0        0        0     4085 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/operators/InsertStationOperator.h
+-rw-r--r--   0        0        0      936 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/operators/InterRouteTwoOptOperator.h
+-rw-r--r--   0        0        0     3158 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/operators/RemoveStationOperator.h
+-rw-r--r--   0        0        0    15813 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/operators/SwapOperator.h
+-rw-r--r--   0        0        0     1972 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/operators.h
+-rw-r--r--   0        0        0     5054 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/removal_cache.h
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/types.h
+-rw-r--r--   0        0        0     8032 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/utility/adaptive_priority_list.h
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/utility/algorithms.h
+-rw-r--r--   0        0        0      992 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/utility/arc_set.h
+-rw-r--r--   0        0        0     1140 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/utility/heap.h
+-rw-r--r--   0        0        0      826 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/utility/iterator_pair.h
+-rw-r--r--   0        0        0     3727 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/utility/random.h
+-rw-r--r--   0        0        0     1357 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/include/routingblocks/vertex.h
+-rw-r--r--   0        0        0      139 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/CMakeLists.txt
+-rw-r--r--   0        0        0      317 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/dynamic_bitset/CMakeLists.txt
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/dynamic_bitset/LICENSE.txt
+-rw-r--r--   0        0        0   117337 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp
+-rw-r--r--   0        0        0    20974 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h
+-rw-r--r--   0        0        0      310 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/small_vector/CMakeLists.txt
+-rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/small_vector/LICENSE.txt
+-rw-r--r--   0        0        0   241472 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/small_vector/small_vector/small_vector.hpp
+-rw-r--r--   0        0        0      290 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/xoshiro/CMakeLists.txt
+-rw-r--r--   0        0        0     1090 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/xoshiro/LICENSE.txt
+-rw-r--r--   0        0        0    49824 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/lib/xoshiro/xoshiro/xoshiro.h
+-rw-r--r--   0        0        0     3302 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/ADPTWEvaluation.cpp
+-rw-r--r--   0        0        0        1 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/FRVCP.cpp
+-rw-r--r--   0        0        0     3393 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/Instance.cpp
+-rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/LocalSearch.cpp
+-rw-r--r--   0        0        0     8324 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/NIFTWEvaluation.cpp
+-rw-r--r--   0        0        0     3773 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/Solution.cpp
+-rw-r--r--   0        0        0      123 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/adaptive_large_neighborbood.cpp
+-rw-r--r--   0        0        0     4504 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/lns_operators.cpp
+-rw-r--r--   0        0        0     1059 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/node.cpp
+-rw-r--r--   0        0        0     3420 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/operators/InsertStationOperator.cpp
+-rw-r--r--   0        0        0     2051 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/src/operators/InterRouteTwoOptOperator.cpp
+-rw-r--r--   0        0        0     1629 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/test/CMakeLists.txt
+-rw-r--r--   0        0        0      154 2022-11-09 12:37:21.000000 routingblocks-0.1.4/native/test/src/dummy.cpp
+-rw-r--r--   0        0        0     1330 2022-11-09 12:37:21.000000 routingblocks-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      264 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/__init__.py
+-rw-r--r--   0        0        0      630 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/operators/__init__.py
+-rw-r--r--   0        0        0     1525 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/operators/best_insert.py
+-rw-r--r--   0        0        0     4390 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/operators/cluster_removal.py
+-rw-r--r--   0        0        0     1928 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/operators/move_selectors.py
+-rw-r--r--   0        0        0     5530 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/operators/related_removal.py
+-rw-r--r--   0        0        0     1022 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/operators/route_removal.py
+-rw-r--r--   0        0        0     3835 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/operators/station_vicinity_removal.py
+-rw-r--r--   0        0        0     1496 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/operators/worst_removal.py
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/utility/__init__.py
+-rw-r--r--   0        0        0     2909 2022-11-09 12:37:21.000000 routingblocks-0.1.4/routingblocks/utility/instance_builder.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/benchmarks/reference/insertion_cache.py
+-rw-r--r--   0        0        0     1986 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/benchmarks/reference/removal_cache.py
+-rw-r--r--   0        0        0     1191 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/benchmarks/test_benchmark_frvcp.py
+-rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/benchmarks/test_benchmark_local_search.py
+-rw-r--r--   0        0        0     3118 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/benchmarks/test_benchmark_removal_cache.py
+-rw-r--r--   0        0        0     9867 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/benchmarks/test_benchmark_route_update.py
+-rw-r--r--   0        0        0       53 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/conftest.py
+-rw-r--r--   0        0        0     5570 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     1048 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/fixtures/data/c101C5.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/fixtures/data/c101_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/fixtures/data/r101_21.txt
+-rw-r--r--   0        0        0    11107 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/fixtures/data/r201_21.txt
+-rw-r--r--   0        0        0    11105 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/fixtures/data/rc101_21.txt
+-rw-r--r--   0        0        0     4553 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/fixtures/mock_evaluation.py
+-rw-r--r--   0        0        0      143 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     2061 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/helpers/interface.py
+-rw-r--r--   0        0        0     4214 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/helpers/models.py
+-rw-r--r--   0        0        0     3060 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/helpers/parsing.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/operators/__init__.py
+-rw-r--r--   0        0        0     7708 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/operators/test_cluster_removal.py
+-rw-r--r--   0        0        0     1645 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/operators/test_random_insertion.py
+-rw-r--r--   0        0        0     1826 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/operators/test_random_removal.py
+-rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/operators/test_related_removal.py
+-rw-r--r--   0        0        0     1914 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/operators/test_station_insertion.py
+-rw-r--r--   0        0        0      295 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/operators/test_station_removal.py
+-rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/operators/test_station_vicinity_removal.py
+-rw-r--r--   0        0        0    20600 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/operators/test_swap.py
+-rw-r--r--   0        0        0     3851 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/test_evaluation.py
+-rw-r--r--   0        0        0     4569 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/test_frvcp.py
+-rw-r--r--   0        0        0     6394 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/test_insertion_cache.py
+-rw-r--r--   0        0        0     5154 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/test_large_neighborhood.py
+-rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/test_lns_helpers.py
+-rw-r--r--   0        0        0     2622 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/test_local_search.py
+-rw-r--r--   0        0        0     1969 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/test_node.py
+-rw-r--r--   0        0        0     3190 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/test_removal_cache.py
+-rw-r--r--   0        0        0    13948 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/test_route.py
+-rw-r--r--   0        0        0    19901 2022-11-09 12:37:21.000000 routingblocks-0.1.4/test/tests/test_solution.py
+-rw-r--r--   0        0        0     2905 2022-11-09 12:37:21.000000 routingblocks-0.1.4/PKG-INFO
```

### Comparing `routingblocks-0.1.3/.cmake-format` & `routingblocks-0.1.4/.cmake-format`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/.github/workflows/wheels.yml` & `routingblocks-0.1.4/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/.gitignore` & `routingblocks-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/CONTRIBUTING.md` & `routingblocks-0.1.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/README.md` & `routingblocks-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/bindings/CMakeLists.txt` & `routingblocks-0.1.4/bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/bindings/include/routingblocks_bindings/binding_helpers.hpp` & `routingblocks-0.1.4/bindings/include/routingblocks_bindings/binding_helpers.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/bindings/src/Evaluation.cpp` & `routingblocks-0.1.4/bindings/src/Evaluation.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,15 @@
                          std::shared_ptr<PyConcatenationBasedEvaluation>>(
             m, "PyConcatenationBasedEvaluation", evaluation_interface)
             .def(pybind11::init<>())
             .def("propagate_forward", &PyConcatenationBasedEvaluation::py_propagate_forward)
             .def("propagate_backward", &PyConcatenationBasedEvaluation::py_propagate_backward)
             .def("concatenate", &PyConcatenationBasedEvaluation::py_concatenate)
             .def("compute_cost", &PyConcatenationBasedEvaluation::py_compute_cost)
+            .def("get_cost_components", &PyConcatenationBasedEvaluation::py_get_cost_components)
             .def("is_feasible", &PyConcatenationBasedEvaluation::py_is_feasible)
             .def("create_forward_label", &PyConcatenationBasedEvaluation::py_create_forward_label)
             .def("create_backward_label",
                  &PyConcatenationBasedEvaluation::py_create_backward_label);
     }
 
     template <class T, class Binding> auto bind_evaluation(Binding& evaluation) {
```

### Comparing `routingblocks-0.1.3/bindings/src/Instance.cpp` & `routingblocks-0.1.4/bindings/src/Instance.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,30 @@
             .def_readonly("id", &routingblocks::Vertex::id)
             .def_readonly("vertex_id", &routingblocks::Vertex::id)
             .def_readonly("str_id", &routingblocks::Vertex::str_id)
             .def_readonly("is_station", &routingblocks::Vertex::is_station)
             .def_readonly("is_depot", &routingblocks::Vertex::is_depot)
             .def_property_readonly("is_customer",
                                    [](const Vertex& v) { return !v.is_station && !v.is_depot; })
+            .def_property_readonly(
+                "data",
+                [](const Vertex& v) -> pybind11::object { return v.get_data<pybind11::object>(); },
+                "Get the vertex data. Note that this function is well-defined only for VertexData "
+                "classes defined in Python.")
             .def("__str__", &::bindings::helpers::ostream_to_string<routingblocks::Vertex>);
     }
 
     template <class ArcData> auto bind_arc(pybind11::module& m, std::string_view name) {
         return pybind11::class_<routingblocks::Arc>(m, name.data())
-            .def(pybind11::init<>(&::bindings::helpers::arc_constructor<ArcData>));
+            .def(pybind11::init<>(&::bindings::helpers::arc_constructor<ArcData>))
+            .def_property_readonly(
+                "data",
+                [](const Arc& a) -> pybind11::object { return a.get_data<pybind11::object>(); },
+                "Get the arc data. Note that this function is well-defined only for ArcData "
+                "classes defined in Python.");
     }
 
     void bind_routingblocks_instance(pybind11::module& m) {
         bind_vertex<pybind11::object>(m, "Vertex");
         bind_arc<pybind11::object>(m, "Arc");
 
         auto adptw = m.def_submodule("adptw");
```

### Comparing `routingblocks-0.1.3/bindings/src/Labeling.cpp` & `routingblocks-0.1.4/bindings/src/Labeling.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/bindings/src/LocalSearch.cpp` & `routingblocks-0.1.4/bindings/src/LocalSearch.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/bindings/src/Operators.cpp` & `routingblocks-0.1.4/bindings/src/Operators.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -172,26 +172,27 @@
 
     void bind_operators(pybind11::module_& m) {
         auto operator_interface = bind_operator_interface(m);
         auto move_interface = bind_move_interface(m);
 
         bind_arc_set(m);
 
-        bind_inter_route_two_opt(m, operator_interface, move_interface);
-        bind_station_in_operator(m, operator_interface, move_interface);
-        bind_station_out_operator(m, operator_interface, move_interface);
+        auto operator_module = m.def_submodule("operators");
+        bind_inter_route_two_opt(operator_module, operator_interface, move_interface);
+        bind_station_in_operator(operator_module, operator_interface, move_interface);
+        bind_station_out_operator(operator_module, operator_interface, move_interface);
 
-        bind_swap_operator<0, 1>(m, operator_interface, move_interface);
-        bind_swap_operator<0, 2>(m, operator_interface, move_interface);
-        bind_swap_operator<0, 3>(m, operator_interface, move_interface);
-        bind_swap_operator<1, 1>(m, operator_interface, move_interface);
-        bind_swap_operator<1, 2>(m, operator_interface, move_interface);
-        bind_swap_operator<1, 3>(m, operator_interface, move_interface);
-        bind_swap_operator<2, 1>(m, operator_interface, move_interface);
-        bind_swap_operator<2, 2>(m, operator_interface, move_interface);
-        bind_swap_operator<2, 3>(m, operator_interface, move_interface);
-        bind_swap_operator<3, 1>(m, operator_interface, move_interface);
-        bind_swap_operator<3, 2>(m, operator_interface, move_interface);
-        bind_swap_operator<3, 3>(m, operator_interface, move_interface);
+        bind_swap_operator<0, 1>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<0, 2>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<0, 3>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<1, 1>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<1, 2>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<1, 3>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<2, 1>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<2, 2>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<2, 3>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<3, 1>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<3, 2>(operator_module, operator_interface, move_interface);
+        bind_swap_operator<3, 3>(operator_module, operator_interface, move_interface);
     }
 
 }  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.3/bindings/src/Solution.cpp` & `routingblocks-0.1.4/bindings/src/Solution.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/bindings/src/bindings.cpp` & `routingblocks-0.1.4/bindings/src/bindings.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/bindings/src/large_neighborhood.cpp` & `routingblocks-0.1.4/bindings/src/large_neighborhood.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         m.def("sample_positions", &routingblocks::lns::operators::sample_positions,
               "Samples k positions with replacement from the solution. Can optionally include the "
               "start depot.");
     }
 
     auto bind_random_destory_operator(pybind11::module_& m, auto& interface) {
         using _operator = routingblocks::lns::operators::RandomRemoval;
-        return pybind11::class_<_operator, std::shared_ptr<_operator>>(m, "RandomRemoveOperator",
+        return pybind11::class_<_operator, std::shared_ptr<_operator>>(m, "RandomRemovalOperator",
                                                                        interface)
             .def(pybind11::init<routingblocks::utility::random&>())
             .def("apply", &_operator::apply, "Remove random vertices from the solution.")
             .def("name", &_operator::name)
             .def("can_apply_to", &_operator::can_apply_to,
                  "Returns true. Random remove is always possible.");
     }
@@ -193,12 +193,13 @@
                         score);
                 },
                 "Collects the score archived by the selected operators.");
 
         auto destroy_operator_interface = bind_destroy_operator_interface(m);
         auto repair_operator_interface = bind_repair_operator_interface(m);
 
-        bind_random_insertion_operator(m, repair_operator_interface);
-        bind_random_destory_operator(m, destroy_operator_interface);
+        auto operator_module = m.def_submodule("operators");
+        bind_random_insertion_operator(operator_module, repair_operator_interface);
+        bind_random_destory_operator(operator_module, destroy_operator_interface);
     }
 
 }  // namespace routingblocks::bindings
```

### Comparing `routingblocks-0.1.3/bindings/src/utility.cpp` & `routingblocks-0.1.4/bindings/src/utility.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/docs/make.bat` & `routingblocks-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/docs/source/conf.py` & `routingblocks-0.1.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/docs/source/development.rst` & `routingblocks-0.1.4/docs/source/development.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,36 +2,36 @@
 ====================
 
 Setting up a development environment
 ------------------------------------
 
 Make sure to install the development dependencies. This includes testing and (optionally) documentation dependencies.
 
-.. code-block::bash
+.. code-block:: bash
 
     pip install .[test]
     pip install .[docs]
 
 Running the tests
 -----------------
 
 Then run the tests:
 
-.. code-block::bash
+.. code-block:: bash
 
     cd test
     pytest tests
 
 Building documentation
 ----------------------
 
-.. code-block::bash
+.. code-block:: bash
 
     cd docs
     make html
 
-I recommend sphinx-autobuild <https://github.com/executablebooks/sphinx-autobuild> for live-reloading the documentation:
+We recommend `sphinx-autobuild <https://github.com/executablebooks/sphinx-autobuild>`_ for live-reloading the documentation:
 
-.. code-block::bash
+.. code-block:: bash
 
     pip install sphinx-autobuild
     sphinx-autobuild docs/source docs/build/html
```

### Comparing `routingblocks-0.1.3/docs/source/index.rst` & `routingblocks-0.1.4/docs/source/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-.. ALNS Framework documentation master file, created by
-sphinx-quickstart on Wed Mar 15 21:56:13 2023.
-You can adapt this file completely to your liking, but it should at least
-contain the root `toctree` directive.
-
 Welcome to RoutingBlock's documentation!
 ==========================================
 
 .. toctree::
     :maxdepth: 1
     :caption: Basics
 
@@ -25,15 +20,15 @@
     alns
     auxilliary
 
 .. toctree::
     :maxdepth: 1
     :caption: Further Reading
 
-    extensions
+    extension
     examples
     development
     routingblocks
 
 
 Indices and tables
 ==================
```

### Comparing `routingblocks-0.1.3/examples/evrptw/__main__.py` & `routingblocks-0.1.4/examples/evrptw/__main__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/alns.py` & `routingblocks-0.1.4/examples/evrptw/alns.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from .instance import Instance as ADPTWInstance
 from .utility import distribute_randomly
 from .parameters import ALNSParams
 
 import routingblocks
 
 
-def create_reduced_arc_set(instance: routingblocks.Instance, py_instance: ADPTWInstance, n_neighbours: int) -> routingblocks.ArcSet:
+def create_reduced_arc_set(instance: routingblocks.Instance, py_instance: ADPTWInstance,
+                           n_neighbours: int) -> routingblocks.ArcSet:
     arc_set = routingblocks.ArcSet(instance.number_of_vertices)
     for i in range(1, instance.number_of_vertices):
         sorted_arcs = sorted(
             ((j, py_instance.arcs[instance.get_vertex(i).str_id, instance.get_vertex(j).str_id]) for j in
              range(1, instance.number_of_vertices)), key=lambda arc: arc[1].cost)
         for j, _ in sorted_arcs[n_neighbours:]:
             arc_set.forbid_arc(i, j)
@@ -46,27 +47,28 @@
     def register(self, solution: routingblocks.Solution):
         self._last_penalites.append(self._get_cost_components(solution))
         if len(self._last_penalites) > self._window_length:
             self._last_penalites.pop(0)
 
 
 class ALNS:
-    def __init__(self, evaluation: routingblocks.Evaluation, py_instance: ADPTWInstance, cpp_instance: routingblocks.Instance,
+    def __init__(self, evaluation: routingblocks.Evaluation, py_instance: ADPTWInstance,
+                 cpp_instance: routingblocks.Instance,
                  params: ALNSParams, seed: int):
         self._evaluation = evaluation
         self._py_instance = py_instance
         self._cpp_instance = cpp_instance
         self._params = params
         # Initialize random engines
         self._random = routingblocks.Random(seed)
         self._py_random = random.Random(seed)
 
         # Create and configure algorithmic components
         self._adaptive_large_neighborhood = routingblocks.AdaptiveLargeNeighborhood(self._random,
-                                                                            self._params.adaptive_smoothing_factor)
+                                                                                    self._params.adaptive_smoothing_factor)
         self._local_search = routingblocks.LocalSearch(self._cpp_instance, evaluation, None)
         self._local_search.set_use_best_improvement(self._params.use_best_improvement)
 
         # Compute the granular neighborhood
         self._reduced_arc_set = create_reduced_arc_set(self._cpp_instance, self._py_instance, self._params.granularity)
 
         # Create specialized FRVCP solver
@@ -99,62 +101,66 @@
         # Create/Register operators
         self._configure_local_search_operators()
         self._configure_repair_operators()
         self._configure_destroy_operators()
 
     def _configure_local_search_operators(self):
         self._operators = [
-            routingblocks.SwapOperator_0_1(self._cpp_instance, self._reduced_arc_set),
-            routingblocks.SwapOperator_0_2(self._cpp_instance, self._reduced_arc_set),
-            routingblocks.SwapOperator_0_3(self._cpp_instance, self._reduced_arc_set),
-            routingblocks.SwapOperator_1_1(self._cpp_instance, self._reduced_arc_set),
-            routingblocks.InterRouteTwoOptOperator(self._cpp_instance, self._reduced_arc_set),
-            routingblocks.InsertStationOperator(self._cpp_instance),
-            routingblocks.RemoveStationOperator(self._cpp_instance)
+            routingblocks.operators.SwapOperator_0_1(self._cpp_instance, self._reduced_arc_set),
+            routingblocks.operators.SwapOperator_0_2(self._cpp_instance, self._reduced_arc_set),
+            routingblocks.operators.SwapOperator_0_3(self._cpp_instance, self._reduced_arc_set),
+            routingblocks.operators.SwapOperator_1_1(self._cpp_instance, self._reduced_arc_set),
+            routingblocks.operators.InterRouteTwoOptOperator(self._cpp_instance, self._reduced_arc_set),
+            routingblocks.operators.InsertStationOperator(self._cpp_instance),
+            routingblocks.operators.RemoveStationOperator(self._cpp_instance)
         ]
 
     def _configure_destroy_operators(self):
-        self._adaptive_large_neighborhood.add_destroy_operator(routingblocks.RandomRemoveOperator(self._random))
+        self._adaptive_large_neighborhood.add_destroy_operator(
+            routingblocks.operators.RandomRemovalOperator(self._random))
         self._adaptive_large_neighborhood.add_destroy_operator(RouteRemoveOperator(self._random))
         self._adaptive_large_neighborhood.add_destroy_operator(
             create_related_remove_operator(self._py_instance, self._cpp_instance, self._random,
                                            self._params.tw_shift_weight, self._params.slack_weight))
         self._adaptive_large_neighborhood.add_destroy_operator(create_shaw_remove_operator(
             self._py_instance, self._cpp_instance, self._random,
             distance_weight=self._params.distance_weight, demand_weight=self._params.demand_weight,
             time_weight=self._params.time_weight, shaw_exponent=self._params.shaw_exponent))
         self._adaptive_large_neighborhood.add_destroy_operator(
             WorstRemovalOperator(self._cpp_instance,
                                  blink_selector_factory(self._params.worst_removal_blink_probability,
                                                         self._random)))
 
     def _configure_repair_operators(self):
-        self._adaptive_large_neighborhood.add_repair_operator(routingblocks.RandomInsertionOperator(self._random))
+        self._adaptive_large_neighborhood.add_repair_operator(
+            routingblocks.operators.RandomInsertionOperator(self._random))
         self._adaptive_large_neighborhood.add_repair_operator(
             best_insert.BestInsertionOperator(self._cpp_instance, first_move_selector))
         self._adaptive_large_neighborhood.add_repair_operator(
             best_insert.BestInsertionOperator(self._cpp_instance,
                                               blink_selector_factory(self._params.best_insertion_blink_probability,
                                                                      self._random)))
 
     def _apply_dp(self, _solution: routingblocks.Solution) -> routingblocks.Solution:
         optimized_routes = [routingblocks.create_route(self._evaluation, self._cpp_instance,
-                                               self._frvcp.optimize([x.vertex_id for x in route])[1:-1]) for route
+                                                       self._frvcp.optimize([x.vertex_id for x in route])[1:-1]) for
+                            route
                             in
                             _solution]
         return routingblocks.Solution(self._evaluation, self._cpp_instance,
-                              [route for route in optimized_routes if not route.empty or not _solution.feasible])
+                                      [route for route in optimized_routes if
+                                       not route.empty or not _solution.feasible])
 
     def _generate_random_solution(self):
         customers = [x.vertex_id for x in self._cpp_instance.customers]
         while True:
             sol = routingblocks.Solution(self._evaluation, self._cpp_instance,
-                                 [routingblocks.create_route(self._evaluation, self._cpp_instance, r) for r in
-                                  distribute_randomly(customers, self._cpp_instance.fleet_size,
-                                                      self._random)])
+                                         [routingblocks.create_route(self._evaluation, self._cpp_instance, r) for r in
+                                          distribute_randomly(customers, self._cpp_instance.fleet_size,
+                                                              self._random)])
             self._local_search.optimize(sol, self._operators)
             yield self._apply_dp(sol)
 
     @property
     def _current_obj(self):
         return self._current_solution.cost if self._current_solution else sys.float_info.max
```

### Comparing `routingblocks-0.1.3/examples/evrptw/config.json` & `routingblocks-0.1.4/examples/evrptw/config.json`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instance/interface.py` & `routingblocks-0.1.4/examples/evrptw/instance/interface.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instance/models.py` & `routingblocks-0.1.4/examples/evrptw/instance/models.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instance/parsing.py` & `routingblocks-0.1.4/examples/evrptw/instance/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/c101C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/c101C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/c104C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/c104C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/c202C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/c202C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/c205C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/c205C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/r102C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/r102C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/r103C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/r103C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/r201C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/r201C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/r203C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/r203C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/rc102C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/rc102C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/rc108C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/rc108C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/rc201C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/rc201C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/10/rc205C10.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/10/rc205C10.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c101_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c102_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c103_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c104_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c105_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c106_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c107_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c108_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c109_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c109_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c201_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c202_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c203_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c204_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c205_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c206_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c207_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/c208_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/c208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r101_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r102_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r103_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r104_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r105_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r106_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r107_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r108_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r109_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r109_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r110_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r110_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r111_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r111_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r112_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r112_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r201_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r202_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r203_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r204_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r205_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r206_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r207_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r208_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r209_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r209_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r210_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r210_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/r211_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/r211_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc101_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc102_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc102_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc103_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc103_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc104_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc104_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc105_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc105_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc106_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc106_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc107_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc107_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc108_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc108_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc201_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc202_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc202_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc203_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc203_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc204_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc204_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc205_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc205_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc206_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc206_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc207_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc207_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/100/rc208_21.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/100/rc208_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/c103C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/c103C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/c106C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/c106C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/c202C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/c202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/c208C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/c208C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/r102C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/r102C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/r105C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/r105C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/r202C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/r202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/r209C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/r209C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/rc103C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/rc103C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/rc108C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/rc108C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/rc202C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/rc202C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/15/rc204C15.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/15/rc204C15.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/c101C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/c101C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/c103C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/c103C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/c206C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/c206C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/c208C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/c208C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/r104C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/r104C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/r105C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/r105C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/r202C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/r202C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/r203C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/r203C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/rc105C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/rc105C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/rc108C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/rc108C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/rc204C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/rc204C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/5/rc208C5.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/5/rc208C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/instances/evrptw/README.txt` & `routingblocks-0.1.4/examples/evrptw/instances/evrptw/README.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/operators/ShawMoveSelector.py` & `routingblocks-0.1.4/examples/evrptw/operators/ShawMoveSelector.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/operators/ShawRelatedness.py` & `routingblocks-0.1.4/examples/evrptw/operators/ShawRelatedness.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/operators/SpatioTemporalRelatedness.py` & `routingblocks-0.1.4/examples/evrptw/operators/SpatioTemporalRelatedness.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/operators/__init__.py` & `routingblocks-0.1.4/examples/evrptw/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/evrptw/parameters.py` & `routingblocks-0.1.4/examples/evrptw/parameters.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/examples/ils/ils.py` & `routingblocks-0.1.4/examples/ils/ils.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,25 +18,27 @@
     # Create RoutingBlocks Route objects
     routes = [rb.create_route(evaluation, instance, route) for route in routes]
     # Create RoutingBlocks Solution object
     return rb.Solution(evaluation, instance, routes)
 
 
 def perturb(solution: rb.Solution, max_exchanges: int) -> rb.Solution:
+    assert sum(1 for r in solution if not r.empty) > 1, "Cannot perturb a solution with only one route."
     # Create a new solution by copying the current solution
     new_solution = copy.copy(solution)
 
     # Exchange random sequences between routes
     num_exchanges = random.randint(0, max_exchanges)
     for _ in range(num_exchanges):
         # Select two random routes
-        route_1 = random.choice(new_solution)
-        route_2 = random.choice(new_solution)
-        if route_1 is route_2:
-            continue
+        while True:
+            route_1 = random.choice(new_solution)
+            route_2 = random.choice(new_solution)
+            if route_1 is not route_2 and not route_1.empty and not route_2.empty:
+                break
         # Select a random sequence of customers in route 1 that does not include the depot
         start_index_1 = random.randint(1, len(route_1) - 2)
         # end_index is exclusive
         end_index_1 = random.randint(start_index_1, len(route_1) - 1)
         # Do the same for the second route
         # Select a random sequence of customers in route 1 that does not include the depot
         start_index_2 = random.randint(1, len(route_2) - 2)
@@ -44,37 +46,41 @@
         end_index_2 = random.randint(start_index_2, len(route_2) - 1)
         # Exchange the sequences
         new_solution.exchange_segment(route_1, start_index_1, end_index_1,
                                       route_2, start_index_2, end_index_2)
     return new_solution
 
 
-def iterated_local_search(instance: rb.Instance, vehicle_storage_capacity: float, vehicle_battery_capacity_time: float):
+def iterated_local_search(instance: rb.Instance, vehicle_storage_capacity: float, vehicle_battery_capacity_time: float,
+                          number_of_iterations: int = 100):
     evaluation = rb.adptw.Evaluation(vehicle_battery_capacity_time, vehicle_storage_capacity)
+    # Set the penalty factors used to penalize violations of the time window, the
+    # vehicle capacity, and the charge constraints
+    evaluation.penalty_factors = [1., 100., 100., 100.]
 
     local_search = rb.LocalSearch(instance, evaluation, None)
     # Configure the local search to use a best-improvement pivoting rule
     local_search.set_use_best_improvement(True)
     # Create a set of allowed arcs
     arc_set = rb.ArcSet(instance.number_of_vertices)
 
     # Create a set of operators that will be used later when calling the local search
     operators = [
-        rb.SwapOperator_0_1(instance, arc_set),
-        rb.SwapOperator_1_1(instance, arc_set),
-        rb.InsertStationOperator(instance),
-        rb.RemoveStationOperator(instance),
+        rb.operators.SwapOperator_0_1(instance, arc_set),
+        rb.operators.SwapOperator_1_1(instance, arc_set),
+        rb.operators.InsertStationOperator(instance),
+        rb.operators.RemoveStationOperator(instance),
     ]
 
     best_solution = create_random_solution(evaluation, instance)
     current_solution = copy.copy(best_solution)
-    for i in range(10):
+    for i in range(number_of_iterations):
         # Search the neighborhood of the current solution. This modifies the solution in-place.
         local_search.optimize(current_solution, operators)
         if current_solution.cost < best_solution.cost:
             best_solution = current_solution
-            print(f"New best solution found: {best_solution.cost}")
+            print(f"New best solution found: {best_solution.cost} ({best_solution.feasible})")
 
         # Perturb the current solution
         current_solution = perturb(current_solution, len(current_solution) // 2)
 
     return best_solution
```

### Comparing `routingblocks-0.1.3/examples/ils/parsing.py` & `routingblocks-0.1.4/examples/alns/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/CMakeLists.txt` & `routingblocks-0.1.4/native/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/cmake/CPM.cmake` & `routingblocks-0.1.4/native/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/cmake/tools.cmake` & `routingblocks-0.1.4/native/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/ADPTWEvaluation.h` & `routingblocks-0.1.4/native/include/routingblocks/ADPTWEvaluation.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/FRVCP.h` & `routingblocks-0.1.4/native/include/routingblocks/FRVCP.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/Instance.h` & `routingblocks-0.1.4/native/include/routingblocks/Instance.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/LocalSearch.h` & `routingblocks-0.1.4/native/include/routingblocks/LocalSearch.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/NIFTWEvaluation.h` & `routingblocks-0.1.4/native/include/routingblocks/NIFTWEvaluation.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/Solution.h` & `routingblocks-0.1.4/native/include/routingblocks/Solution.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/adaptive_large_neighborhood.hpp` & `routingblocks-0.1.4/native/include/routingblocks/adaptive_large_neighborhood.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/arc.h` & `routingblocks-0.1.4/native/include/routingblocks/arc.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/evaluation.h` & `routingblocks-0.1.4/native/include/routingblocks/evaluation.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/insertion_cache.h` & `routingblocks-0.1.4/native/include/routingblocks/insertion_cache.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/lns_operators.h` & `routingblocks-0.1.4/native/include/routingblocks/lns_operators.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/node.h` & `routingblocks-0.1.4/native/include/routingblocks/node.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/operators/InsertStationOperator.h` & `routingblocks-0.1.4/native/include/routingblocks/operators/InsertStationOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/operators/InterRouteTwoOptOperator.h` & `routingblocks-0.1.4/native/include/routingblocks/operators/InterRouteTwoOptOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/operators/RemoveStationOperator.h` & `routingblocks-0.1.4/native/include/routingblocks/operators/RemoveStationOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/operators/SwapOperator.h` & `routingblocks-0.1.4/native/include/routingblocks/operators/SwapOperator.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/operators.h` & `routingblocks-0.1.4/native/include/routingblocks/operators.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/removal_cache.h` & `routingblocks-0.1.4/native/include/routingblocks/removal_cache.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/utility/adaptive_priority_list.h` & `routingblocks-0.1.4/native/include/routingblocks/utility/adaptive_priority_list.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/utility/algorithms.h` & `routingblocks-0.1.4/native/include/routingblocks/utility/algorithms.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/utility/arc_set.h` & `routingblocks-0.1.4/native/include/routingblocks/utility/arc_set.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/utility/heap.h` & `routingblocks-0.1.4/native/include/routingblocks/utility/heap.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/utility/iterator_pair.h` & `routingblocks-0.1.4/native/include/routingblocks/utility/iterator_pair.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/utility/random.h` & `routingblocks-0.1.4/native/include/routingblocks/utility/random.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/include/routingblocks/vertex.h` & `routingblocks-0.1.4/native/include/routingblocks/vertex.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/lib/dynamic_bitset/LICENSE.txt` & `routingblocks-0.1.4/native/lib/dynamic_bitset/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp` & `routingblocks-0.1.4/native/lib/dynamic_bitset/dynamic_bitset/dynamic_bitset.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h` & `routingblocks-0.1.4/native/lib/dynamic_bitset/dynamic_bitset/libpopcnt.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/lib/small_vector/LICENSE.txt` & `routingblocks-0.1.4/native/lib/small_vector/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/lib/small_vector/small_vector/small_vector.hpp` & `routingblocks-0.1.4/native/lib/small_vector/small_vector/small_vector.hpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/lib/xoshiro/LICENSE.txt` & `routingblocks-0.1.4/native/lib/xoshiro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/lib/xoshiro/xoshiro/xoshiro.h` & `routingblocks-0.1.4/native/lib/xoshiro/xoshiro/xoshiro.h`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/src/ADPTWEvaluation.cpp` & `routingblocks-0.1.4/native/src/ADPTWEvaluation.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/src/Instance.cpp` & `routingblocks-0.1.4/native/src/Instance.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/src/LocalSearch.cpp` & `routingblocks-0.1.4/native/src/LocalSearch.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/src/NIFTWEvaluation.cpp` & `routingblocks-0.1.4/native/src/NIFTWEvaluation.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/src/Solution.cpp` & `routingblocks-0.1.4/native/src/Solution.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/src/lns_operators.cpp` & `routingblocks-0.1.4/native/src/lns_operators.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/src/node.cpp` & `routingblocks-0.1.4/native/src/node.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/src/operators/InsertStationOperator.cpp` & `routingblocks-0.1.4/native/src/operators/InsertStationOperator.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/src/operators/InterRouteTwoOptOperator.cpp` & `routingblocks-0.1.4/native/src/operators/InterRouteTwoOptOperator.cpp`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/native/test/CMakeLists.txt` & `routingblocks-0.1.4/native/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/pyproject.toml` & `routingblocks-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core>=0.2.1", "pybind11", "mypy"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "RoutingBlocks"
-version = "0.1.3"
+version = "0.1.4"
 description = "A package for the implementation of vehicle routing problems with intermediate stops"
 readme = "README.md"
 authors = [
     { name = "Patrick Sean Klein", email = "patrick.sean.klein@tum.de" },
 ]
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `routingblocks-0.1.3/routingblocks/operators/__init__.py` & `routingblocks-0.1.4/routingblocks/operators/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,7 +3,8 @@
 from .worst_removal import WorstRemovalOperator
 from .best_insert import BestInsertionOperator
 from .route_removal import RouteRemoveOperator
 from .cluster_removal import ClusterRemovalOperator, DistanceBasedClusterMemberSelector, ClusterMemberSelector, \
     SeedSelector
 from .station_vicinity_removal import StationVicinityRemovalOperator, StationSeedSelector
 from .related_removal import RelatedRemovalOperator, RelatednessComputer, MoveSelector
+from .._routingblocks.operators import *
```

### Comparing `routingblocks-0.1.3/routingblocks/operators/best_insert.py` & `routingblocks-0.1.4/routingblocks/operators/best_insert.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/routingblocks/operators/cluster_removal.py` & `routingblocks-0.1.4/routingblocks/operators/cluster_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/routingblocks/operators/move_selectors.py` & `routingblocks-0.1.4/routingblocks/operators/move_selectors.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/routingblocks/operators/related_removal.py` & `routingblocks-0.1.4/routingblocks/operators/related_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/routingblocks/operators/route_removal.py` & `routingblocks-0.1.4/routingblocks/operators/route_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/routingblocks/operators/station_vicinity_removal.py` & `routingblocks-0.1.4/routingblocks/operators/station_vicinity_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/routingblocks/operators/worst_removal.py` & `routingblocks-0.1.4/routingblocks/operators/worst_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/routingblocks/utility/instance_builder.py` & `routingblocks-0.1.4/routingblocks/utility/instance_builder.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/benchmarks/reference/insertion_cache.py` & `routingblocks-0.1.4/test/tests/benchmarks/reference/insertion_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/benchmarks/reference/removal_cache.py` & `routingblocks-0.1.4/test/tests/benchmarks/reference/removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/benchmarks/test_benchmark_frvcp.py` & `routingblocks-0.1.4/test/tests/benchmarks/test_benchmark_frvcp.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/benchmarks/test_benchmark_local_search.py` & `routingblocks-0.1.4/test/tests/benchmarks/test_benchmark_local_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
 def run_local_search(local_search: alns.LocalSearch, solution: alns.Solution, operators):
     local_search.optimize(solution, operators)
 
 
 def create_operators(instance):
     return [
-        alns.SwapOperator_0_1(instance, None),
-        alns.SwapOperator_0_2(instance, None),
-        alns.SwapOperator_1_1(instance, None),
-        alns.SwapOperator_1_2(instance, None),
-        alns.InterRouteTwoOptOperator(instance, None)
+        alns.operators.SwapOperator_0_1(instance, None),
+        alns.operators.SwapOperator_0_2(instance, None),
+        alns.operators.SwapOperator_1_1(instance, None),
+        alns.operators.SwapOperator_1_2(instance, None),
+        alns.operators.InterRouteTwoOptOperator(instance, None)
     ]
 
 
 @pytest.mark.benchmark(group="local-search")
 @pytest.mark.parametrize("instance_name", ['c101_21.txt', 'r101_21.txt'])
 @pytest.mark.parametrize("evaluation", ['adptw_native', 'niftw_native'])
 def test_local_search_benchmark(instance_parser, instance_name,
```

### Comparing `routingblocks-0.1.3/test/tests/benchmarks/test_benchmark_removal_cache.py` & `routingblocks-0.1.4/test/tests/benchmarks/test_benchmark_removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/benchmarks/test_benchmark_route_update.py` & `routingblocks-0.1.4/test/tests/benchmarks/test_benchmark_route_update.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/fixtures/__init__.py` & `routingblocks-0.1.4/test/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/fixtures/data/c101C5.txt` & `routingblocks-0.1.4/test/tests/fixtures/data/c101C5.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/fixtures/data/c101_21.txt` & `routingblocks-0.1.4/test/tests/fixtures/data/c101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/fixtures/data/r101_21.txt` & `routingblocks-0.1.4/test/tests/fixtures/data/r101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/fixtures/data/r201_21.txt` & `routingblocks-0.1.4/test/tests/fixtures/data/r201_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/fixtures/data/rc101_21.txt` & `routingblocks-0.1.4/test/tests/fixtures/data/rc101_21.txt`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/fixtures/mock_evaluation.py` & `routingblocks-0.1.4/test/tests/fixtures/mock_evaluation.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/helpers/interface.py` & `routingblocks-0.1.4/test/tests/helpers/interface.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/helpers/models.py` & `routingblocks-0.1.4/test/tests/helpers/models.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/helpers/parsing.py` & `routingblocks-0.1.4/test/tests/helpers/parsing.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/operators/test_cluster_removal.py` & `routingblocks-0.1.4/test/tests/operators/test_cluster_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/operators/test_random_insertion.py` & `routingblocks-0.1.4/test/tests/operators/test_random_insertion.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 except ModuleNotFoundError:
     pass
 
 
 def test_random_insertion_apply(adptw_instance, mock_evaluation, randgen):
     instance: evrptw.Instance = adptw_instance
     evaluation = mock_evaluation
-    operator = alns.RandomInsertionOperator(randgen)
+    operator = alns.operators.RandomInsertionOperator(randgen)
     # Inserts customers at random positions
     customers = list(instance.customers)
     missing_customers = customers[1:]
     solutions = []
     for _ in range(10):
         sol = alns.Solution(evaluation, instance, [alns.create_route(evaluation, instance, [customers[0].vertex_id]),
                                                    alns.Route(evaluation, instance)])
```

### Comparing `routingblocks-0.1.3/test/tests/operators/test_random_removal.py` & `routingblocks-0.1.4/test/tests/operators/test_random_removal.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     import routingblocks as alns
 except ModuleNotFoundError:
     pass
 
 
 def test_random_removal_apply(adptw_instance, mock_evaluation, random_solution_factory, randgen):
     instance: evrptw.Instance = adptw_instance
-    operator = alns.RandomRemoveOperator(randgen)
+    operator = alns.operators.RandomRemovalOperator(randgen)
     evaluation = mock_evaluation
     # Throws if removing more customers than are in the solution
     solution = random_solution_factory(instance, evaluation, [next(instance.customers)], n_routes=1)
     with pytest.raises(RuntimeError):
         operator.apply(evaluation, solution, 2)
     # Single customer in solution
     solution = random_solution_factory(instance, evaluation, [next(instance.customers)], n_routes=1)
```

### Comparing `routingblocks-0.1.3/test/tests/operators/test_related_removal.py` & `routingblocks-0.1.4/test/tests/operators/test_related_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/operators/test_station_insertion.py` & `routingblocks-0.1.4/test/tests/operators/test_station_insertion.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,12 +33,12 @@
     penalties[evrptw.niftw.OverchargeCostComponent] = 1000.
     evaluation.penalty_factors = penalties
 
     solution = recreate_solution(evaluation=evaluation, instance=instance)
     route = solution[0]
     assert not route.feasible
     assert route.cost_components[evrptw.niftw.OverchargeCostComponent] > 0
-    station_insertion_operator = evrptw.InsertStationOperator(instance)
+    station_insertion_operator = evrptw.operators.InsertStationOperator(instance)
     ls = evrptw.LocalSearch(instance, evaluation, None)
     ls.optimize(solution, [station_insertion_operator])
     # Charge penalty should be 0.
     assert route.cost_components[evrptw.niftw.OverchargeCostComponent] == 0.
```

### Comparing `routingblocks-0.1.3/test/tests/operators/test_station_vicinity_removal.py` & `routingblocks-0.1.4/test/tests/operators/test_station_vicinity_removal.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/operators/test_swap.py` & `routingblocks-0.1.4/test/tests/operators/test_swap.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                                   [customers[2].id, customers[3].id, customers[4].id])
     return create_solution(evaluation=evaluation, instance=instance,
                            routes=[route_a, route_b])
 
 
 def build_solution(evaluation: routingblocks.Evaluation, instance: routingblocks.Instance, raw_routes: List[List[int]]):
     return routingblocks.Solution(evaluation, instance,
-                          [routingblocks.create_route(evaluation, instance, route) for route in raw_routes])
+                                  [routingblocks.create_route(evaluation, instance, route) for route in raw_routes])
 
 
 def to_propagated_arcs(forward_propagation_sequence: List[routingblocks.Node]) -> List[Tuple[int, int]]:
     return [(i.vertex_id, j.vertex_id) for i, j in zip(forward_propagation_sequence,
                                                        forward_propagation_sequence[1:])]
 
 
@@ -67,19 +67,19 @@
 
 
 @pytest.mark.parametrize("raw_routes", [
     [[1, 7, 2, 6, 6, 3, 8], [6, 4, 7, 8, 5, 8]],
     [[], [1, 7, 2, 6, 6, 3, 8]]
 ])
 @pytest.mark.parametrize("move_type,origin_segment_length,target_segment_length", [
-    (routingblocks.SwapOperatorMove_0_1, 0, 1),
-    (routingblocks.SwapOperatorMove_0_2, 0, 2),
-    (routingblocks.SwapOperatorMove_1_1, 1, 1),
-    (routingblocks.SwapOperatorMove_1_2, 1, 2),
-    (routingblocks.SwapOperatorMove_2_1, 2, 1),
+    (routingblocks.operators.SwapOperatorMove_0_1, 0, 1),
+    (routingblocks.operators.SwapOperatorMove_0_2, 0, 2),
+    (routingblocks.operators.SwapOperatorMove_1_1, 1, 1),
+    (routingblocks.operators.SwapOperatorMove_1_2, 1, 2),
+    (routingblocks.operators.SwapOperatorMove_2_1, 2, 1),
 ])
 def test_swap_interroute_apply(adptw_instance: evrptw.Instance, mock_evaluation, move_type, origin_segment_length,
                                target_segment_length, raw_routes):
     instance: evrptw.Instance = adptw_instance
 
     def _recreate_solution():
         return build_solution(mock_evaluation, instance, raw_routes)
@@ -124,19 +124,19 @@
 
 @pytest.mark.parametrize("raw_routes", [
     [[1, 5, 2, 6, 6, 3, 8, 6, 4, 7, 6, 5, 7]],
     [[]],
     [[1]]
 ])
 @pytest.mark.parametrize("move_type,origin_segment_length,target_segment_length", [
-    (routingblocks.SwapOperatorMove_0_1, 0, 1),
-    (routingblocks.SwapOperatorMove_0_2, 0, 2),
-    (routingblocks.SwapOperatorMove_1_1, 1, 1),
-    (routingblocks.SwapOperatorMove_1_2, 1, 2),
-    (routingblocks.SwapOperatorMove_2_1, 2, 1),
+    (routingblocks.operators.SwapOperatorMove_0_1, 0, 1),
+    (routingblocks.operators.SwapOperatorMove_0_2, 0, 2),
+    (routingblocks.operators.SwapOperatorMove_1_1, 1, 1),
+    (routingblocks.operators.SwapOperatorMove_1_2, 1, 2),
+    (routingblocks.operators.SwapOperatorMove_2_1, 2, 1),
 ])
 def test_swap_intraroute_apply(mock_evaluation, adptw_instance: evrptw.Instance, move_type, origin_segment_length,
                                target_segment_length, raw_routes):
     instance: evrptw.Instance = adptw_instance
 
     def _recreate_solution():
         return build_solution(mock_evaluation, instance, raw_routes)
@@ -186,19 +186,19 @@
 
 
 @pytest.mark.parametrize("raw_routes", [
     [[1, 7, 2, 6, 6, 3, 8], [6, 4, 7, 8, 5, 8]],
     [[], [1, 7, 2, 6, 6, 3, 8]]
 ])
 @pytest.mark.parametrize("move_type,origin_segment_length,target_segment_length", [
-    (routingblocks.SwapOperatorMove_0_1, 0, 1),
-    (routingblocks.SwapOperatorMove_0_2, 0, 2),
-    (routingblocks.SwapOperatorMove_1_1, 1, 1),
-    (routingblocks.SwapOperatorMove_1_2, 1, 2),
-    (routingblocks.SwapOperatorMove_2_1, 2, 1),
+    (routingblocks.operators.SwapOperatorMove_0_1, 0, 1),
+    (routingblocks.operators.SwapOperatorMove_0_2, 0, 2),
+    (routingblocks.operators.SwapOperatorMove_1_1, 1, 1),
+    (routingblocks.operators.SwapOperatorMove_1_2, 1, 2),
+    (routingblocks.operators.SwapOperatorMove_2_1, 2, 1),
 ])
 def test_swap_interroute_evaluation(mock_evaluation, adptw_instance, move_type, origin_segment_length,
                                     target_segment_length, raw_routes):
     instance: evrptw.Instance = adptw_instance
 
     def _recreate_solution():
         return build_solution(mock_evaluation, instance, raw_routes)
@@ -258,19 +258,19 @@
 
 @pytest.mark.parametrize("raw_routes", [
     [[1, 2, 3, 4, 5, 6, 7, 8]],
     [[]],
     [[1]]
 ])
 @pytest.mark.parametrize("move_type,origin_segment_length,target_segment_length", [
-    (routingblocks.SwapOperatorMove_0_1, 0, 1),
-    (routingblocks.SwapOperatorMove_0_2, 0, 2),
-    (routingblocks.SwapOperatorMove_1_1, 1, 1),
-    (routingblocks.SwapOperatorMove_1_2, 1, 2),
-    (routingblocks.SwapOperatorMove_2_1, 2, 1),
+    (routingblocks.operators.SwapOperatorMove_0_1, 0, 1),
+    (routingblocks.operators.SwapOperatorMove_0_2, 0, 2),
+    (routingblocks.operators.SwapOperatorMove_1_1, 1, 1),
+    (routingblocks.operators.SwapOperatorMove_1_2, 1, 2),
+    (routingblocks.operators.SwapOperatorMove_2_1, 2, 1),
 ])
 def test_swap_intraroute_evaluation(mock_evaluation, adptw_instance: evrptw.Instance, move_type, origin_segment_length,
                                     target_segment_length, raw_routes):
     instance: evrptw.Instance = adptw_instance
 
     assert all(len(set(route)) == len(route) for route in raw_routes), "Test does not work with duplicate vertex ids"
 
@@ -334,19 +334,19 @@
 
 @pytest.mark.parametrize("raw_routes", [
     [[1, 2, 3, 4, 5, 6, 7, 8]],
     [[1, 2, 3, 4, 5, 6, 7, 8], [9, 10, 11, 12, 13, 14]],
     [[], [1, 7, 2, 6, 3, 8]]
 ])
 @pytest.mark.parametrize("move_type,origin_segment_length,target_segment_length", [
-    (routingblocks.SwapOperatorMove_0_1, 0, 1),
-    (routingblocks.SwapOperatorMove_0_2, 0, 2),
-    (routingblocks.SwapOperatorMove_1_1, 1, 1),
-    (routingblocks.SwapOperatorMove_1_2, 1, 2),
-    (routingblocks.SwapOperatorMove_2_1, 2, 1),
+    (routingblocks.operators.SwapOperatorMove_0_1, 0, 1),
+    (routingblocks.operators.SwapOperatorMove_0_2, 0, 2),
+    (routingblocks.operators.SwapOperatorMove_1_1, 1, 1),
+    (routingblocks.operators.SwapOperatorMove_1_2, 1, 2),
+    (routingblocks.operators.SwapOperatorMove_2_1, 2, 1),
 ])
 def test_swap_symmetry(mock_evaluation, large_adptw_instance: evrptw.Instance, move_type, origin_segment_length,
                        target_segment_length, raw_routes):
     instance: evrptw.Instance = large_adptw_instance
 
     assert len([x for route in raw_routes for x in route]) == len(
         set([x for route in raw_routes for x in route])), "Test does not work with duplicate vertex ids"
```

### Comparing `routingblocks-0.1.3/test/tests/test_evaluation.py` & `routingblocks-0.1.4/test/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/test_frvcp.py` & `routingblocks-0.1.4/test/tests/test_frvcp.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import time
 from typing import Tuple, Callable, Dict, List, Iterable, Optional
 
 import pytest
 
 import helpers
+import routingblocks
 
 from fixtures import *
 
 import sys
 
 try:
     import routingblocks as evrptw
@@ -109,15 +110,15 @@
     while True:
         picked_customers = random.choices([x.id for x in customers], k=random.randint(1, 10))
 
         local_search = evrptw.LocalSearch(instance, evaluation, None)
         sol = evrptw.Solution(evaluation, instance,
                               [evrptw.create_route(evaluation, instance, picked_customers),
                                *(evrptw.Route(evaluation, instance) for _ in range(instance.fleet_size - 1))])
-        local_search.optimize(sol, [routingblocks.SwapOperator_0_1(instance, None)])
+        local_search.optimize(sol, [routingblocks.operators.SwapOperator_0_1(instance, None)])
         for r in sol:
             if r.empty:
                 continue
             frvcp = adptw.FRVCP(instance, py_instance.parameters.battery_capacity_time)
             labelled_route = frvcp.optimize([x.vertex_id for x in r])
             labelled_route = evrptw.create_route(evaluation, instance, labelled_route[1:-1])
             assert labelled_route.cost <= r.cost
```

### Comparing `routingblocks-0.1.3/test/tests/test_insertion_cache.py` & `routingblocks-0.1.4/test/tests/test_insertion_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/test_large_neighborhood.py` & `routingblocks-0.1.4/test/tests/test_large_neighborhood.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/test_lns_helpers.py` & `routingblocks-0.1.4/test/tests/test_lns_helpers.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/test_local_search.py` & `routingblocks-0.1.4/test/tests/test_local_search.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/test_node.py` & `routingblocks-0.1.4/test/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/test_removal_cache.py` & `routingblocks-0.1.4/test/tests/test_removal_cache.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/test_route.py` & `routingblocks-0.1.4/test/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/test/tests/test_solution.py` & `routingblocks-0.1.4/test/tests/test_solution.py`

 * *Files identical despite different names*

### Comparing `routingblocks-0.1.3/PKG-INFO` & `routingblocks-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routingblocks
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for the implementation of vehicle routing problems with intermediate stops
 Author-Email: Patrick Sean Klein <patrick.sean.klein@tum.de>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

