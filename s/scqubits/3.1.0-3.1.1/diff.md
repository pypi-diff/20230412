# Comparing `tmp/scqubits-3.1.0.tar.gz` & `tmp/scqubits-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scqubits-3.1.0.tar", last modified: Mon Sep  5 13:31:43 2022, max compression
+gzip compressed data, was "scqubits-3.1.1.tar", last modified: Wed Apr 12 05:38:35 2023, max compression
```

## Comparing `scqubits-3.1.0.tar` & `scqubits-3.1.1.tar`

### file list

```diff
@@ -1,133 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.174502 scqubits-3.1.0/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1549 2022-09-05 13:31:33.000000 scqubits-3.1.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (121)      237 2022-09-05 13:31:33.000000 scqubits-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-09-05 13:31:43.174502 scqubits-3.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     3439 2022-09-05 13:31:33.000000 scqubits-3.1.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)       54 2022-09-05 13:31:33.000000 scqubits-3.1.0/optional-requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      100 2022-09-05 13:31:33.000000 scqubits-3.1.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.138503 scqubits-3.1.0/scqubits/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3091 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.146502 scqubits-3.1.0/scqubits/core/
--rwxr-xr-x   0 runner    (1001) docker     (121)      482 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6940 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/central_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (121)   139774 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/circuit.py
--rw-r--r--   0 runner    (1001) docker     (121)    11422 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/circuit_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1107 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    37994 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/cos2phi_qubit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3538 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/descriptors.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9105 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/discretization.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23190 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/flux_qubit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9814 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/fluxonium.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3739 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/generic_qubit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    41509 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/hilbert_space.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    24841 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/namedslots_array.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    59862 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/noise.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6580 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/operators.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9247 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/oscillator.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    56724 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/param_sweep.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    39598 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/qubit_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.150502 scqubits-3.1.0/scqubits/core/qubit_img/
--rwxr-xr-x   0 runner    (1001) docker     (121)    87518 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/qubit_img/cos2phi-qubit.jpg
--rwxr-xr-x   0 runner    (1001) docker     (121)    97089 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/qubit_img/fixed-transmon.jpg
--rwxr-xr-x   0 runner    (1001) docker     (121)   106916 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/qubit_img/flux-qubit.jpg
--rwxr-xr-x   0 runner    (1001) docker     (121)   113985 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/qubit_img/fluxonium.jpg
--rwxr-xr-x   0 runner    (1001) docker     (121)   328242 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/qubit_img/fullzeropi.jpg
--rwxr-xr-x   0 runner    (1001) docker     (121)   255948 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/qubit_img/kerr-oscillator.jpg
--rwxr-xr-x   0 runner    (1001) docker     (121)   412869 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/qubit_img/oscillator.jpg
--rwxr-xr-x   0 runner    (1001) docker     (121)   133117 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/qubit_img/tunable-transmon.jpg
--rwxr-xr-x   0 runner    (1001) docker     (121)   295606 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/qubit_img/zeropi.jpg
--rwxr-xr-x   0 runner    (1001) docker     (121)    20181 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/spec_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9047 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/storage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3071 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/sweeps.py
--rw-r--r--   0 runner    (1001) docker     (121)    70530 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/symbolic_circuit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    21007 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/transmon.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4034 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/units.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23823 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/zeropi.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18316 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/core/zeropi_full.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.150502 scqubits-3.1.0/scqubits/explorer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9668 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/explorer/explorer_panels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.150502 scqubits-3.1.0/scqubits/io_utils/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/io_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5884 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/io_utils/fileio.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13961 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/io_utils/fileio_backends.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2395 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/io_utils/fileio_qutip.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10969 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/io_utils/fileio_serializers.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4783 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      689 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.158501 scqubits-3.1.0/scqubits/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9645 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.170502 scqubits-3.1.0/scqubits/tests/data/
--rwxr-xr-x   0 runner    (1001) docker     (121)    16576 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/.fullzeropi_1.hdf5
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/circuit_DFC.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/circuit_fluxonium.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/circuit_zeropi.yaml
--rwxr-xr-x   0 runner    (1001) docker     (121)    14128 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/cos2phiqubit_1.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)   213036 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/cos2phiqubit_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)  1014811 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/cos2phiqubit_4.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    14680 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/cos2phiqubit_5.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    15048 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/fluxonium_1.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    21667 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/fluxonium_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)   367163 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/fluxonium_4.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    14512 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/fluxonium_5.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    14136 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/fluxqubit_1.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    39269 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/fluxqubit_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)  1205265 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/fluxqubit_4.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    14960 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/fluxqubit_5.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    16576 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/fullzeropi_1.hdf5
--rw-r--r--   0 runner    (1001) docker     (121)    33692 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/fullzeropi_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    13624 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/transmon_1.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    18560 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/transmon_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)   120906 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/transmon_4.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    14416 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/transmon_5.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)     9024 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/zeropi-test.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    16320 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/zeropi_1.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)   784344 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/zeropi_2.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)  1755013 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/zeropi_4.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)    16976 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/zeropi_5.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)     9264 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/data/zpifull-test.hdf5
--rwxr-xr-x   0 runner    (1001) docker     (121)     2659 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_centraldispatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     7666 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_circuit_plot.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1020 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_cos2phiqubit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2501 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_explorer.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      951 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_fluxonium.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      953 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_fluxqubit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2110 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_fullzeropi.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      595 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_gui.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12965 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_hilbertspace.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1509 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_namedslotsndarray.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4731 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_noise.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1545 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     4191 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_parametersweep.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16340 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_spectrumlookup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1172 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_transmon.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1349 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_units.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1006 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/tests/test_zeropi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.174502 scqubits-3.1.0/scqubits/ui/
--rwxr-xr-x   0 runner    (1001) docker     (121)      619 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34823 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/ui/explorer_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)    86237 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/ui/gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     7240 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/ui/gui_defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15818 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/ui/hspace_widget.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2888 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/ui/qubit_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.174502 scqubits-3.1.0/scqubits/utils/
--rwxr-xr-x   0 runner    (1001) docker     (121)      619 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1856 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/utils/cpu_switch.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    10582 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/utils/misc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6821 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/utils/plot_defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)     6516 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/utils/plot_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18113 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/utils/plotting.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15623 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/utils/spectrum_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-09-05 13:31:33.000000 scqubits-3.1.0/scqubits/utils/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-05 13:31:42.000000 scqubits-3.1.0/scqubits/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-05 13:31:43.146502 scqubits-3.1.0/scqubits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1916 2022-09-05 13:31:43.000000 scqubits-3.1.0/scqubits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-09-05 13:31:43.000000 scqubits-3.1.0/scqubits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 13:31:43.000000 scqubits-3.1.0/scqubits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-05 13:31:43.000000 scqubits-3.1.0/scqubits.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-05 13:31:43.000000 scqubits-3.1.0/scqubits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-09-05 13:31:43.000000 scqubits-3.1.0/scqubits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-05 13:31:43.174502 scqubits-3.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     4759 2022-09-05 13:31:33.000000 scqubits-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.828381 scqubits-3.1.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-04-12 05:38:24.000000 scqubits-3.1.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      237 2023-04-12 05:38:24.000000 scqubits-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-12 05:38:35.828381 scqubits-3.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3439 2023-04-12 05:38:24.000000 scqubits-3.1.1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-12 05:38:24.000000 scqubits-3.1.1/optional-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      100 2023-04-12 05:38:24.000000 scqubits-3.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.796381 scqubits-3.1.1/scqubits/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.804381 scqubits-3.1.1/scqubits/core/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6939 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/central_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139627 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/circuit_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54530 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/cos2phi_qubit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3538 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/descriptors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9106 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/discretization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36737 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/flux_qubit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18938 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/fluxonium.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3645 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/generic_qubit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43780 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/hilbert_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24921 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/namedslots_array.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60033 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/noise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6580 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/operators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8974 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/oscillator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56815 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/param_sweep.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42979 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.808381 scqubits-3.1.1/scqubits/core/qubit_img/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    87518 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/cos2phi-qubit.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    97089 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/fixed-transmon.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   106916 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/flux-qubit.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113985 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/fluxonium.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   328242 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/fullzeropi.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   255948 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/kerr-oscillator.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   412869 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/oscillator.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   133117 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/tunable-transmon.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   295606 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/qubit_img/zeropi.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14843 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/spec_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8507 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3071 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/sweeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70527 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/symbolic_circuit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31094 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/transmon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4034 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/units.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32843 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/zeropi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29519 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/core/zeropi_full.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.808381 scqubits-3.1.1/scqubits/explorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/explorer/explorer_panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.812381 scqubits-3.1.1/scqubits/io_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/io_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5884 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/io_utils/fileio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13961 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/io_utils/fileio_backends.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/io_utils/fileio_qutip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10969 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/io_utils/fileio_serializers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5030 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      689 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.812381 scqubits-3.1.1/scqubits/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9645 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.824381 scqubits-3.1.1/scqubits/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/circuit_DFC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/circuit_fluxonium.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/circuit_zeropi.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15496 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_1.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   214632 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   472471 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_4.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16032 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15048 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxonium_1.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21667 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxonium_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   367163 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxonium_4.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14512 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxonium_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14136 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxqubit_1.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39269 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxqubit_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1205265 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxqubit_4.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14960 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fluxqubit_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17920 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fullzeropi_1.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    33599 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/fullzeropi_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13624 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/transmon_1.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18560 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/transmon_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   120906 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/transmon_4.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14416 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/transmon_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9024 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zeropi-test.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17664 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zeropi_1.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)   788882 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zeropi_2.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1761598 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zeropi_4.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18200 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zeropi_5.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9264 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/data/zpifull-test.hdf5
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2659 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_centraldispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_circuit_plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1020 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_cos2phiqubit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2501 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_explorer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      951 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_fluxonium.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      953 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_fluxqubit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_fullzeropi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16570 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_hilbertspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1509 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_namedslotsndarray.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4731 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_noise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_parametersweep.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16340 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_spectrumlookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_transmon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1349 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_units.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/tests/test_zeropi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.828381 scqubits-3.1.1/scqubits/ui/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35028 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/explorer_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86193 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/gui_defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15818 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/hspace_widget.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2860 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/ui/qubit_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.828381 scqubits-3.1.1/scqubits/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1856 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/cpu_switch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11110 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6892 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/plot_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/plot_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18701 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/plotting.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15622 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/spectrum_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-12 05:38:24.000000 scqubits-3.1.1/scqubits/utils/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 05:38:35.800381 scqubits-3.1.1/scqubits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-12 05:38:35.000000 scqubits-3.1.1/scqubits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 05:38:35.828381 scqubits-3.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4759 2023-04-12 05:38:24.000000 scqubits-3.1.1/setup.py
```

### Comparing `scqubits-3.1.0/LICENSE` & `scqubits-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/PKG-INFO` & `scqubits-3.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scqubits
-Version: 3.1.0
+Version: 3.1.1
 Summary: scqubits: superconducting qubits in Python
 Home-page: https://scqubits.readthedocs.io
 Author: Jens Koch, Peter Groszkowski
 Author-email: jens-koch@northwestern.edu, piotrekg@gmail.com
 License: BSD
 Keywords: superconducting qubits
 Platform: Linux
```

### Comparing `scqubits-3.1.0/README.md` & `scqubits-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/__init__.py` & `scqubits-3.1.1/scqubits/__init__.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/central_dispatch.py` & `scqubits-3.1.1/scqubits/core/central_dispatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 
 import logging
 import warnings
 import weakref
-
 from types import MethodType
 from weakref import WeakKeyDictionary
 
 import scqubits.settings as settings
 
 LOGGER = logging.getLogger(__name__)
```

### Comparing `scqubits-3.1.0/scqubits/core/circuit.py` & `scqubits-3.1.1/scqubits/core/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,86 +5,82 @@
 #
 #    Copyright (c) 2019 and later, Jens Koch and Peter Groszkowski
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
+
 import copy
 import functools
 import itertools
 import operator as builtin_op
 import re
 import warnings
-
 from types import MethodType
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import qutip as qt
 import scipy as sp
 import sympy as sm
 
 from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from numpy import ndarray
-from scipy import sparse, stats
+from scipy import sparse
 from scipy.sparse import csc_matrix
 from sympy import latex
 
 try:
-    from IPython.display import display, Latex
+    from IPython.display import Latex, display
 except ImportError:
     _HAS_IPYTHON = False
 else:
     _HAS_IPYTHON = True
 
 import scqubits as scq
 import scqubits.core.discretization as discretization
 import scqubits.core.oscillator as osc
 import scqubits.core.qubit_base as base
-import scqubits.core.spec_lookup as spec_lookup
 import scqubits.core.storage as storage
 import scqubits.io_utils.fileio_serializers as serializers
 import scqubits.utils.plot_defaults as defaults
 import scqubits.utils.plotting as plot
 import scqubits.utils.spectrum_utils as utils
-
 from scqubits import HilbertSpace, settings
 from scqubits.core import operators as op
 from scqubits.core.circuit_utils import (
     _cos_dia,
     _cos_dia_dense,
     _cos_phi,
     _cos_theta,
     _exp_i_theta_operator,
     _exp_i_theta_operator_conjugate,
     _generate_symbols_list,
     _i_d2_dphi2_operator,
     _i_d_dphi_operator,
-    _identity_theta,
     _n_theta_operator,
     _phi_operator,
     _sin_dia,
     _sin_dia_dense,
     _sin_phi,
     _sin_theta,
     compose,
     get_operator_number,
     get_trailing_number,
     grid_operator_func_factory,
     is_potential_term,
     matrix_power_sparse,
     operator_func_factory,
 )
-from scqubits.core.namedslots_array import NamedSlotsNdarray
 from scqubits.core.symbolic_circuit import Branch, SymbolicCircuit
 from scqubits.io_utils.fileio import IOData
-from scqubits.io_utils.fileio_serializers import dict_deserialize, dict_serialize
+from scqubits.io_utils.fileio_serializers import dict_serialize
 from scqubits.utils.misc import (
     flatten_list,
     flatten_list_recursive,
     list_intersection,
     number_of_lists_in_list,
 )
 from scqubits.utils.plot_utils import _process_options
@@ -110,15 +106,15 @@
         Defines the hierarchy of the new subsystem, is set to None when hierarchical
         diagonalization is not required. by default None
     subsystem_trunc_dims: Optional[List], optional
         Defines the truncated dimensions for the subsystems inside the current
         subsystem, is set to None when hierarchical diagonalization is not required,
         by default `None`
     truncated_dim: Optional[int], optional
-        sets the truncated dimension for the current subsystem, by default 10
+        sets the truncated dimension for the current subsystem, set to 10 by default.
     """
 
     # switch used in protecting the class from erroneous addition of new attributes
     _frozen = False
 
     def __init__(
         self,
@@ -190,15 +186,15 @@
         self.discretized_phi_range: Dict[int, Tuple[float]] = {
             idx: self.parent.discretized_phi_range[idx]
             for idx in self.parent.discretized_phi_range
             if idx in self.var_categories_list
         }
 
         # storing the potential terms separately
-        # also bringing the potential to the same form as in the class Circuit
+        # and bringing the potential into the same form as for the class Circuit
         potential_symbolic = 0 * sm.symbols("x")
         for term in self.hamiltonian_symbolic.as_ordered_terms():
             if is_potential_term(term):
                 potential_symbolic += term
         for i in self.var_categories_list:
             potential_symbolic = (
                 potential_symbolic.replace(
@@ -680,15 +676,15 @@
         )
 
     def get_eigenstates(self) -> ndarray:
         """
         Returns the eigenstates for the SubSystem instance
         """
         if self.is_child:
-            subsys_index = self.parent.hilbert_space.subsys_list.index(self)
+            subsys_index = self.parent.hilbert_space.subsystem_list.index(self)
             return self.parent.hilbert_space["bare_evecs"][subsys_index][0]
         else:
             return self.eigensys()[1]
 
     def get_subsystem_index(self, var_index: int) -> int:
         """
         Returns the subsystem index for the subsystem to which the given var_index
@@ -866,27 +862,25 @@
         )
 
         # Defining the list of discretized_ext variables
         y_symbols = _generate_symbols_list("θ", self.var_categories["extended"])
         p_symbols = _generate_symbols_list("Q", self.var_categories["extended"])
 
         if self.ext_basis == "discretized":
-
             ps_symbols = [
                 sm.symbols("Qs" + str(i)) for i in self.var_categories["extended"]
             ]
             sin_symbols = [
                 sm.symbols(f"sinθ{i}") for i in self.var_categories["extended"]
             ]
             cos_symbols = [
                 sm.symbols(f"cosθ{i}") for i in self.var_categories["extended"]
             ]
 
         elif self.ext_basis == "harmonic":
-
             a_symbols = [sm.symbols(f"a{i}") for i in self.var_categories["extended"]]
             ad_symbols = [sm.symbols(f"ad{i}") for i in self.var_categories["extended"]]
             Nh_symbols = [sm.symbols(f"Nh{i}") for i in self.var_categories["extended"]]
             pos_symbols = [sm.symbols(f"θ{i}") for i in self.var_categories["extended"]]
             sin_symbols = [
                 sm.symbols(f"sinθ{i}") for i in self.var_categories["extended"]
             ]
@@ -991,15 +985,14 @@
         )  # applying expand is critical; otherwise the replacement of p^2 with ps2
         # would not succeed
 
         # shifting the potential to the point of external fluxes
         hamiltonian = self._shift_harmonic_oscillator_potential(hamiltonian)
 
         if self.ext_basis == "discretized":
-
             # marking the squared momentum operators with a separate symbol
             for i in self.var_categories["extended"]:
                 hamiltonian = hamiltonian.replace(
                     sm.symbols(f"Q{i}") ** 2, sm.symbols("Qs" + str(i))
                 )
 
         # removing the constants from the Hamiltonian
@@ -1233,15 +1226,14 @@
                     + op.annihilation(self.cutoffs_dict()[var_index])
                 )
                 exp_i_theta = sp.linalg.expm(pos_operator * prefactor * 1j)
 
         return self._sparsity_adaptive(exp_i_theta)
 
     def _evaluate_matrix_cosine_terms(self, junction_potential: sm.Expr) -> qt.Qobj:
-
         if self.hierarchical_diagonalization:
             subsystem_list = list(self.subsystems.values())
             identity = qt.tensor(
                 [qt.identity(subsystem.truncated_dim) for subsystem in subsystem_list]
             )
         else:
             identity = qt.identity(self.hilbertdim())
@@ -1360,15 +1352,15 @@
                     sp.linalg.cosm,
                     functools.partial(
                         op.a_plus_adag, prefactor=osc_lengths[var_index] / (2**0.5)
                     ),
                 )
                 nonwrapped_ops["momentum"] = functools.partial(
                     op.ia_minus_iadag_sparse,
-                    prefactor=1 / (osc_lengths[var_index] * 2**0.5),
+                    prefactor=-1 / (osc_lengths[var_index] * 2**0.5),
                 )
 
                 for short_op_name in nonwrapped_ops.keys():
                     op_func = nonwrapped_ops[short_op_name]
                     sym_variable = extended_vars[short_op_name][list_idx]
                     op_name = sym_variable.name + "_operator"
                     extended_operators[op_name] = operator_func_factory(
@@ -1530,15 +1522,14 @@
     def _is_mat_mul_replacement_necessary(self, term):
         return (
             set(self.var_categories["extended"])
             & set([get_trailing_number(str(i)) for i in term.free_symbols])
         ) and "*" in str(term)
 
     def _replace_mat_mul_operator(self, term: sm.Expr):
-
         if not self._is_mat_mul_replacement_necessary(term):
             return str(term)
 
         if self.ext_basis == "discretized":
             term_string = str(term)
             term_var_categories = [
                 get_trailing_number(str(i)) for i in term.free_symbols
@@ -1803,15 +1794,15 @@
             self.updated_subsystem_indices = []
 
             bare_esys = {
                 sys_index: (
                     self.hilbert_space["bare_evals"][sys_index][0],
                     self.hilbert_space["bare_evecs"][sys_index][0],
                 )
-                for sys_index, sys in enumerate(self.hilbert_space.subsys_list)
+                for sys_index, sys in enumerate(self.hilbert_space.subsystem_list)
             }
             hamiltonian = self.hilbert_space.hamiltonian(bare_esys=bare_esys)
             if self.type_of_matrices == "dense":
                 return hamiltonian.full()
             if self.type_of_matrices == "sparse":
                 return hamiltonian.data.tocsc()
 
@@ -1837,15 +1828,14 @@
         elif self.type_of_matrices == "dense":
             evals = sp.linalg.eigvalsh(
                 hamiltonian_mat, subset_by_index=[0, evals_count - 1]
             )
         return np.sort(evals)
 
     def _esys_calc(self, evals_count: int) -> Tuple[ndarray, ndarray]:
-
         if (
             isinstance(self, Circuit)
             and self.is_purely_harmonic
             and not self.hierarchical_diagonalization
         ):
             return self._eigensys_for_purely_harmonic(evals_count=evals_count)
 
@@ -2467,15 +2457,14 @@
                     wf_dim += subsys.var_categories_list.index(var_index)
                 break
             else:
                 wf_dim += 1
         return wf_dim
 
     def _dims_to_be_summed(self, var_indices: Tuple[int], num_wf_dims) -> List[int]:
-
         all_var_indices = self.var_categories_list
         non_summed_dims = []
         for var_index in all_var_indices:
             if var_index in var_indices:
                 non_summed_dims.append(
                     self._get_var_dim_for_reshaped_wf(var_indices, var_index)
                 )
@@ -2802,15 +2791,14 @@
         self,
         wf_plot: ndarray,
         var_indices,
         grids_per_varindex_dict,
         change_discrete_charge_to_phi: bool,
         kwargs,
     ) -> Tuple[Figure, Axes]:
-
         var_index = var_indices[0]
         wavefunc = storage.WaveFunction(
             basis_labels=grids_per_varindex_dict[var_indices[0]].make_linspace(),
             amplitudes=wf_plot,
         )
 
         if not change_discrete_charge_to_phi and (
```

### Comparing `scqubits-3.1.0/scqubits/core/circuit_utils.py` & `scqubits-3.1.1/scqubits/core/circuit_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import re
 
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Union
+from typing import TYPE_CHECKING, Any, Callable, List, Union
 
 import numpy as np
 import sympy as sm
 
 from numpy import ndarray
 from scipy import sparse
 from scipy.sparse import csc_matrix
@@ -237,27 +237,27 @@
 
 def _exp_i_theta_operator(ncut) -> csc_matrix:
     r"""
     Operator :math:`\cos(\theta)`, acting only on the `\theta` Hilbert subspace.
     """
     dim_theta = 2 * ncut + 1
     matrix = sparse.dia_matrix(
-        (np.ones(dim_theta), [1]),
+        (np.ones(dim_theta), [-1]),
         shape=(dim_theta, dim_theta),
     ).tocsc()
     return matrix
 
 
 def _exp_i_theta_operator_conjugate(ncut) -> csc_matrix:
     r"""
     Operator :math:`\cos(\theta)`, acting only on the `\theta` Hilbert subspace.
     """
     dim_theta = 2 * ncut + 1
     matrix = sparse.dia_matrix(
-        (np.ones(dim_theta), [-1]),
+        (np.ones(dim_theta), [1]),
         shape=(dim_theta, dim_theta),
     ).tocsc()
     return matrix
 
 
 def _cos_theta(ncut: int) -> csc_matrix:
     """Returns operator :math:`\\cos \\varphi` in the charge basis"""
```

### Comparing `scqubits-3.1.0/scqubits/core/constants.py` & `scqubits-3.1.1/scqubits/core/constants.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/cos2phi_qubit.py` & `scqubits-3.1.1/scqubits/core/cos2phi_qubit.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,53 +19,62 @@
 import numpy as np
 import scipy as sp
 
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from numpy import ndarray
 from scipy import sparse
-from scipy.sparse import csc_matrix, dia_matrix
+from scipy.sparse import coo_matrix, csc_matrix, dia_matrix
 
 import scqubits.core.constants as constants
 import scqubits.core.descriptors as descriptors
 import scqubits.core.discretization as discretization
 import scqubits.core.operators as op
 import scqubits.core.oscillator as osc
 import scqubits.core.qubit_base as base
 import scqubits.core.storage as storage
 import scqubits.core.units as units
 import scqubits.io_utils.fileio_serializers as serializers
-import scqubits.settings as settings
 import scqubits.utils.plotting as plot
 import scqubits.utils.spectrum_utils as utils
 
 from scqubits.core.noise import NOISE_PARAMS, NoisySystem, calc_therm_ratio
 from scqubits.core.storage import WaveFunctionOnGrid
 
 
-# -Cosine two phi qubit noise class
+# - Cosine-2-phi qubit noise class ------------------------------------------------------------------------------------
 class NoisyCos2PhiQubit(NoisySystem, ABC):
     @abstractmethod
-    def phi_1_operator(self) -> csc_matrix:
+    def phi_1_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
         pass
 
     @abstractmethod
-    def phi_2_operator(self) -> csc_matrix:
+    def phi_2_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
         pass
 
     @abstractmethod
-    def n_1_operator(self) -> csc_matrix:
+    def n_1_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
         pass
 
     @abstractmethod
-    def n_2_operator(self) -> csc_matrix:
+    def n_2_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
         pass
 
     @abstractmethod
-    def n_zeta_operator(self) -> csc_matrix:
+    def n_zeta_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
         pass
 
     def t1_inductive(
         self,
         i: int = 1,
         j: int = 0,
         Q_ind: Union[float, Callable] = None,
@@ -597,73 +606,158 @@
         dimension = self._dim_phi()
         return (
             (op.creation_sparse(dimension) + op.annihilation_sparse(dimension))
             * self.phi_osc()
             / math.sqrt(2)
         )
 
-    def phi_operator(self) -> csc_matrix:
-        r"""Returns :math:`\phi` operator"""
-        return self._kron3(
+    def phi_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        r"""
+        Returns the :math:`\phi` operator in the native or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns :math:`\phi` operator in the native basis.
+            If `True`, the energy eigenspectrum is computed, returns :math:`\phi` operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns :math:`\phi` operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            :math:`\phi` operator in chosen basis. If native basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless energy_esys is specified, :math:`\phi` operator has dimensions of truncated_dim
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen, :math:`\phi`
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
+        native = self._kron3(
             self._phi_operator(), self._identity_zeta(), self._identity_theta()
         )
+        return self.process_op(native_op=native, energy_esys=energy_esys)
 
     def _n_phi_operator(self) -> csc_matrix:
         r"""
         Returns
         -------
             `n_\phi` operator in the harmonic oscillator basis"""
         dimension = self._dim_phi()
         return (
             1j
             * (op.creation_sparse(dimension) - op.annihilation_sparse(dimension))
             / (self.phi_osc() * math.sqrt(2))
         )
 
-    def n_phi_operator(self) -> csc_matrix:
-        r"""Returns :math:`n_\phi` operator"""
-        return self._kron3(
+    # changed expected from csc_matrix to Union[ndarray, coo_matrix]
+    def n_phi_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, coo_matrix]:
+        r"""
+        Returns the :math:`n_\phi` operator in the harmonic oscillator or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns :math:`n_\phi` operator in the native basis.
+            If `True`, the energy eigenspectrum is computed, returns :math:`n_\phi` operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns :math:`n_\phi` operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            :math:`n_\phi` operator in chosen basis. If native basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless energy_esys is specified, :math:`n_\phi` operator has dimensions of truncated_dim
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen, :math:`n_\phi`
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray :math:`\zeta`.
+        """
+        native = self._kron3(
             self._n_phi_operator(), self._identity_zeta(), self._identity_theta()
         )
+        return self.process_op(native_op=native, energy_esys=energy_esys)
 
     def _zeta_operator(self) -> csc_matrix:
         """
         Returns
         -------
             `zeta` operator in the harmonic oscillator basis"""
         dimension = self._dim_zeta()
         return (
             (op.creation_sparse(dimension) + op.annihilation_sparse(dimension))
             * self.zeta_osc()
             / math.sqrt(2)
         )
 
-    def zeta_operator(self) -> csc_matrix:
-        r"""Returns :math:`\zeta` operator"""
-        return self._kron3(
+    def zeta_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        r"""
+        Returns the :math:`\zeta`  operator in the harmonic oscillator or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns :math:`\zeta` operator in the native basis.
+            If `True`, the energy eigenspectrum is computed, returns :math:`\zeta`  operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns :math:`\zeta`  operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            :math:`\zeta`  operator in chosen basis. If native basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless energy_esys is specified, :math:`\zeta`  operator has dimensions of truncated_dim
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen, :math:`\zeta`
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
+        native = self._kron3(
             self._identity_phi(), self._zeta_operator(), self._identity_theta()
         )
+        return self.process_op(native_op=native, energy_esys=energy_esys)
 
     def _n_zeta_operator(self) -> csc_matrix:
         r"""
         Returns
         -------
             `n_\zeta` operator in the harmonic oscillator basis"""
         dimension = self._dim_zeta()
         return (
             1j
             * (op.creation_sparse(dimension) - op.annihilation_sparse(dimension))
             / (self.zeta_osc() * math.sqrt(2))
         )
 
-    def n_zeta_operator(self) -> csc_matrix:
-        r"""Returns :math:`n_\zeta` operator"""
-        return self._kron3(
+    def n_zeta_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        r"""
+        Returns the :math:`n_\zeta`  operator in the harmonic oscillator or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns :math:`n_\zeta` operator in the native basis.
+            If `True`, the energy eigenspectrum is computed, returns :math:`n_\zeta`  operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns :math:`n_\zeta`  operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            :math:`n_\zeta`  operator in chosen basis. If native basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless energy_esys is specified, :math:`n_\zeta`  operator has dimensions of truncated_dim
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen, :math:`n_\zeta`
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
+        native = self._kron3(
             self._identity_phi(), self._n_zeta_operator(), self._identity_theta()
         )
+        return self.process_op(native_op=native, energy_esys=energy_esys)
 
     def _exp_i_phi_operator(self) -> csc_matrix:
         """
         Returns
         -------
             `e^{i*phi}` operator in the  harmonic oscillator basis"""
         exponent = 1j * self._phi_operator()
@@ -693,19 +787,40 @@
         -------
             `n_theta` operator in the charge basis"""
         diag_elements = np.arange(-self.ncut, self.ncut + 1)
         return dia_matrix(
             (diag_elements, [0]), shape=(self._dim_theta(), self._dim_theta())
         ).tocsc()
 
-    def n_theta_operator(self) -> csc_matrix:
-        r"""Returns :math:`n_\theta` operator"""
-        return self._kron3(
+    def n_theta_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        r"""
+        Returns the :math:`n_\theta`  operator in the charge or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns :math:`n_\theta` operator in the charge basis.
+            If `True`, the energy eigenspectrum is computed, returns :math:`n_\theta`  operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns :math:`n_\theta`  operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            :math:`n_\theta`  operator in chosen basis. If charge basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless energy_esys is specified, :math:`n_\theta`  operator has dimensions of truncated_dim
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen, :math:`n_\theta`
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
+        native = self._kron3(
             self._identity_phi(), self._identity_zeta(), self._n_theta_operator()
         )
+        return self.process_op(native_op=native, energy_esys=energy_esys)
 
     def _cos_theta_operator(self) -> csc_matrix:
         r"""Returns operator :math:`\cos \theta` in the charge basis"""
         cos_op = (
             0.5
             * sparse.dia_matrix(
                 (np.ones(self._dim_theta()), [1]),
@@ -722,22 +837,22 @@
         return cos_op
 
     def _sin_theta_operator(self) -> csc_matrix:
         r"""Returns operator :math:`\sin \theta` in the charge basis"""
         sin_op = (
             0.5
             * sparse.dia_matrix(
-                (np.ones(self._dim_theta()), [1]),
+                (np.ones(self._dim_theta()), [-1]),
                 shape=(self._dim_theta(), self._dim_theta()),
             ).tocsc()
         )
         sin_op -= (
             0.5
             * sparse.dia_matrix(
-                (np.ones(self._dim_theta()), [-1]),
+                (np.ones(self._dim_theta()), [1]),
                 shape=(self._dim_theta(), self._dim_theta()),
             ).tocsc()
         )
         return sin_op * (-1j)
 
     def _kron3(self, mat1, mat2, mat3) -> csc_matrix:
         """
@@ -768,18 +883,35 @@
 
     def total_identity(self) -> csc_matrix:
         """Returns Identity operator acting on the total Hilbert space."""
         return self._kron3(
             self._identity_phi(), self._identity_zeta(), self._identity_theta()
         )
 
-    def hamiltonian(self) -> csc_matrix:
-        """
-        Returns Hamiltonian in basis obtained by employing harmonic basis for
-        :math:`\\phi, \\zeta` and charge basis for :math:`\\theta`.
+    def hamiltonian(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> csc_matrix:
+        """Returns Hamiltonian in basis obtained by employing harmonic basis for
+        :math:`\\phi, \\zeta` and charge basis for :math:`\\theta` or in the eigenenerg basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns Hamiltonian in basis obtained by employing harmonic basis for
+            :math:`\\phi, \\zeta` and charge basis for :math:`\\theta`.
+            If `True`, the energy eigenspectrum is computed, returns Hamiltonian in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns Hamiltonian in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            Hamiltonian in chosen basis as csc_matrix. If the eigenenergy basis is chosen,
+            unless `energy_esys` is specified, the Hamiltonian has dimensions of `truncated_dim`
+            x `truncated_dim`. Otherwise, if eigenenergy basis is chosen, Hamiltonian has dimensions of m x m,
+            for m given eigenvectors.
         """
         phi_osc_mat = self._kron3(
             op.number_sparse(self._dim_phi(), self.phi_plasma()),
             self._identity_zeta(),
             self._identity_theta(),
         )
 
@@ -840,23 +972,27 @@
             - self.n_phi_operator() * self.ng
             - self._kron3(
                 self._n_phi_operator(), self._n_zeta_operator(), self._identity_theta()
             )
         )
         disorder_c = -4 * self._disordered_ecj() * self.dCJ * dis_c_opt
 
-        return (
+        hamiltonian_mat = (
             phi_osc_mat
             + zeta_osc_mat
             + cross_kinetic_mat
             + junction_mat
             + disorder_l
             + disorder_j
             + disorder_c
         )
+        native = hamiltonian_mat.tocsc()
+        return self.process_hamiltonian(
+            native_hamiltonian=native, energy_esys=energy_esys
+        )
 
     def _evals_calc(self, evals_count) -> ndarray:
         hamiltonian_mat = self.hamiltonian()
         evals = utils.eigsh_safe(
             hamiltonian_mat,
             k=evals_count,
             return_eigenvectors=False,
@@ -1073,35 +1209,141 @@
             wavefunc,
             zero_calibrate=zero_calibrate,
             ylabel=r"$\theta$",
             xlabel=r"$\phi$",
             **kwargs
         )
 
-    def phi_1_operator(self) -> csc_matrix:
-        """Returns operator representing the phase across inductor 1"""
-        return self.zeta_operator() - self.phi_operator()
-
-    def phi_2_operator(self) -> csc_matrix:
-        """Returns operator representing the phase across inductor 2"""
-        return -self.zeta_operator() - self.phi_operator()
-
-    def n_1_operator(self) -> csc_matrix:
-        """Returns operator representing the charge difference across junction 1"""
-        return 0.5 * self.n_phi_operator() + 0.5 * (
+    def phi_1_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        """
+        Returns operator representing the phase across inductor 1 in harmonic oscillator or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns operator in the harmonic oscillator basis.
+            If `True`, the energy eigenspectrum is computed, returns operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            Operator in chosen basis. If harmonic oscillator basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless `energy_esys` is specified, operator has dimensions of `truncated_dim`
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen,
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
+        native = self.zeta_operator() - self.phi_operator()
+        return self.process_op(native_op=native, energy_esys=energy_esys)
+
+    def phi_2_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        """
+        Returns operator representing the phase across inductor 2 in harmonic oscillator or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns operator in the harmonic oscillator basis.
+            If `True`, the energy eigenspectrum is computed, returns operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            Operator in chosen basis. If harmonic oscillator basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless `energy_esys` is specified, operator has dimensions of `truncated_dim`
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen,
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
+        native = -self.zeta_operator() - self.phi_operator()
+        return self.process_op(native_op=native, energy_esys=energy_esys)
+
+    def n_1_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        """
+        Returns operator representing the charge difference across junction 1 in native or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns operator in the harmonic oscillator basis.
+            If `True`, the energy eigenspectrum is computed, returns operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            Operator in chosen basis. If native basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless `energy_esys` is specified, operator has dimensions of `truncated_dim`
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen,
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
+        native = 0.5 * self.n_phi_operator() + 0.5 * (
             self.n_theta_operator() - self.n_zeta_operator()
         )
+        return self.process_op(native_op=native, energy_esys=energy_esys)
+
+    def n_2_operator(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        """
+        Returns operator representing the charge difference across junction 2 in native or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns operator in the harmonic oscillator basis.
+            If `True`, the energy eigenspectrum is computed, returns operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
 
-    def n_2_operator(self) -> csc_matrix:
-        """Returns operator representing the charge difference across junction 2"""
-        return 0.5 * self.n_phi_operator() - 0.5 * (
+        Returns
+        -------
+            Operator in chosen basis. If native basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless `energy_esys` is specified, operator has dimensions of `truncated_dim`
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen,
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
+        native = 0.5 * self.n_phi_operator() - 0.5 * (
             self.n_theta_operator() - self.n_zeta_operator()
         )
+        return self.process_op(native_op=native, energy_esys=energy_esys)
+
+    def d_hamiltonian_d_flux(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        """
+        Returns operator representing a derivative of the Hamiltonian with respect to
+        flux in the native or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns operator in the native basis.
+            If `True`, the energy eigenspectrum is computed, returns operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
 
-    def d_hamiltonian_d_flux(self) -> csc_matrix:
+        Returns
+        -------
+            Operator in chosen basis. If native basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless `energy_esys` is specified, operator has dimensions of `truncated_dim`
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen,
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
         phi_flux_term = self._sin_phi_operator() * np.cos(
             self.flux * np.pi
         ) + self._cos_phi_operator() * np.sin(self.flux * np.pi)
         junction_mat = (
             2
             * self.EJ
             * self._kron3(
@@ -1118,17 +1360,40 @@
             * self.dEJ
             * self.EJ
             * self._kron3(
                 dis_phi_flux_term, self._identity_zeta(), self._sin_theta_operator()
             )
             * np.pi
         )
-        return junction_mat + dis_junction_mat
+        native = junction_mat + dis_junction_mat
+        return self.process_op(native_op=native, energy_esys=energy_esys)
+
+    def d_hamiltonian_d_EJ(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        """
+        Returns operator representing a derivative of the Hamiltonian with respect to
+        EJ in the native or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns operator in the native basis.
+            If `True`, the energy eigenspectrum is computed, returns operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
 
-    def d_hamiltonian_d_EJ(self) -> csc_matrix:
+        Returns
+        -------
+            Operator in chosen basis. If native basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless `energy_esys` is specified, operator has dimensions of `truncated_dim`
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen,
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
         phi_flux_term = self._cos_phi_operator() * np.cos(
             self.flux * np.pi
         ) - self._sin_phi_operator() * np.sin(self.flux * np.pi)
         junction_mat = -2 * self._kron3(
             phi_flux_term, self._identity_zeta(), self._cos_theta_operator()
         )
 
@@ -1138,16 +1403,40 @@
         dis_junction_mat = (
             2
             * self.dEJ
             * self._kron3(
                 dis_phi_flux_term, self._identity_zeta(), self._sin_theta_operator()
             )
         )
-        return junction_mat + dis_junction_mat
+        native = junction_mat + dis_junction_mat
+        return self.process_op(native_op=native, energy_esys=energy_esys)
 
-    def d_hamiltonian_d_ng(self) -> csc_matrix:
-        return (
+    def d_hamiltonian_d_ng(
+        self, energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False
+    ) -> Union[ndarray, csc_matrix]:
+        """
+        Returns operator representing a derivative of the Hamiltonian with respect to
+        ng in the native or eigenenergy basis.
+
+        Parameters
+        ----------
+        energy_esys:
+            If `False` (default), returns operator in the native basis.
+            If `True`, the energy eigenspectrum is computed, returns operator in the energy eigenbasis.
+            If `energy_esys = esys`, where esys is a tuple containing two ndarrays (eigenvalues and energy eigenvectors),
+            returns operator in the energy eigenbasis, and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            Operator in chosen basis. If native basis chosen, operator
+            returned as a csc_matrix. If the eigenenergy basis is chosen,
+            unless `energy_esys` is specified, operator has dimensions of `truncated_dim`
+            x truncated_dim, and is returned as an ndarray. Otherwise, if eigenenergy basis is chosen,
+            operator has dimensions of m x m, for m given eigenvectors, and is returned as an ndarray.
+        """
+        native = (
             4 * self.dCJ * self._disordered_ecj() * self.n_phi_operator()
             - 4
             * self._disordered_ecj()
             * (self.n_theta_operator() - self.ng - self.n_zeta_operator())
         )
+        return self.process_op(native_op=native, energy_esys=energy_esys)
```

### Comparing `scqubits-3.1.0/scqubits/core/descriptors.py` & `scqubits-3.1.1/scqubits/core/descriptors.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/discretization.py` & `scqubits-3.1.1/scqubits/core/discretization.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 import scqubits.core.central_dispatch as dispatch
 import scqubits.core.descriptors as descriptors
 import scqubits.io_utils.fileio_serializers as serializers
 import scqubits.settings as settings
 import scqubits.utils.misc as utils
 
+
 FIRST_STENCIL_COEFFS: Dict[int, List[float]] = {
     3: [-1 / 2, 0.0, 1 / 2],
     5: [1 / 12, -2 / 3, 0.0, 2 / 3, -1 / 12],
     7: [-1 / 60, 3 / 20, -3 / 4, 0.0, 3 / 4, -3 / 20, 1 / 60],
     9: [1 / 280, -4 / 105, 1 / 5, -4 / 5, 0.0, 4 / 5, -1 / 5, 4 / 105, -1 / 280],
 }
```

### Comparing `scqubits-3.1.0/scqubits/core/fluxonium.py` & `scqubits-3.1.1/scqubits/core/oscillator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,290 +1,254 @@
-# fluxonium.py
+# oscillator.py
 #
 # This file is part of scqubits: a Python package for superconducting qubits,
 # Quantum 5, 583 (2021). https://quantum-journal.org/papers/q-2021-11-17-583/
 #
 #    Copyright (c) 2019 and later, Jens Koch and Peter Groszkowski
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
-import cmath
-import math
 import os
 
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
 import scipy as sp
 
 from numpy import ndarray
+from scipy.special import factorial, pbdv
 
 import scqubits.core.descriptors as descriptors
-import scqubits.core.discretization as discretization
 import scqubits.core.operators as op
-import scqubits.core.oscillator as osc
 import scqubits.core.qubit_base as base
-import scqubits.core.storage as storage
 import scqubits.io_utils.fileio_serializers as serializers
 
-from scqubits.core.noise import NoisySystem
+_default_evals_count = 6
 
-if TYPE_CHECKING:
-    from scqubits.core.discretization import Grid1d
 
+def harm_osc_wavefunction(
+    n: int, x: Union[float, ndarray], l_osc: float
+) -> Union[float, ndarray]:
+    r"""For given quantum number n=0,1,2,... return the value of the harmonic
+    oscillator wave function :math:`\psi_n(x) = N H_n(x/l_{osc}) \exp(-x^2/2l_\text{
+    osc})`, N being the proper normalization factor.
+
+    Directly uses `scipy.special.pbdv` (implementation of the parabolic cylinder
+    function) to mitigate numerical stability issues with the more commonly used
+    expression in terms of a Gaussian and a Hermite polynomial factor.
+
+    Parameters
+    ----------
+    n:
+        index of wave function, n=0 is ground state
+    x:
+        coordinate(s) where wave function is evaluated
+    l_osc:
+        oscillator length, defined via <0|x^2|0> = l_osc^2/2
+
+    Returns
+    -------
+        value of harmonic oscillator wave function
+    """
+    result = pbdv(n, np.sqrt(2.0) * x / l_osc) / np.sqrt(
+        l_osc * np.sqrt(np.pi) * factorial(n)
+    )
+    return result[0]
+
+
+def convert_to_E_osc(E_kin: float, E_pot: float) -> float:
+    r"""Returns the oscillator energy given a harmonic Hamiltonian of the form
+    :math:`H=\frac{1}{2}E_{\text{kin}}p^2 + \frac{1}{2}E_{\text{pot}}x^2`"""
+    return np.sqrt(E_kin * E_pot)
+
+
+def convert_to_l_osc(E_kin: float, E_pot: float) -> float:
+    r"""Returns the oscillator length given a harmonic Hamiltonian of the form
+    :math:`H=\frac{1}{2}E_{\text{kin}}p^2 + \frac{1}{2}E_{\text{pot}}x^2`"""
+    return (E_kin / E_pot) ** (1 / 4)
 
-class Fluxonium(base.QubitBaseClass1d, serializers.Serializable, NoisySystem):
-    r"""Class for the fluxonium qubit. Hamiltonian :math:`H_\text{fl}=-4E_\text{
-    C}\partial_\phi^2-E_\text{J}\cos(\phi+\varphi_\text{ext}) +\frac{1}{2}E_L\phi^2`
-    is represented in dense form. The employed basis is the EC-EL harmonic oscillator
-    basis. The cosine term in the potential is handled via matrix exponentiation.
-    Initialize with, for example::
 
-        qubit = Fluxonium(EJ=1.0, EC=2.0, EL=0.3, flux=0.2, cutoff=120)
+# -Oscillator class-------------------------------------------------------------------
+
+
+class Oscillator(base.QuantumSystem, serializers.Serializable):
+    r"""Class representing a harmonic oscillator/resonator governed by a Hamiltonian
+    :math:`H=E_\text{osc} a^{\dagger} a`, with :math:`a` being the annihilation
+    operator.
 
     Parameters
     ----------
-    EJ: float
-        Josephson energy
-    EC: float
-        charging energy
-    EL: float
-        inductive energy
-    flux: float
-        external magnetic flux in units of one flux quantum
-    cutoff: int
-        number of harm. osc. basis states used in diagonalization
-    truncated_dim: int
+    E_osc:
+        energy of the oscillator
+    l_osc:
+        oscillator length (required to define phi_operator and n_operator)
+    truncated_dim:
         desired dimension of the truncated quantum system; expected: truncated_dim > 1
-    id_str: str
+    id_str:
         optional string by which this instance can be referred to in `HilbertSpace`
         and `ParameterSweep`. If not provided, an id is auto-generated.
     """
-    EJ = descriptors.WatchedProperty(float, "QUANTUMSYSTEM_UPDATE")
-    EC = descriptors.WatchedProperty(float, "QUANTUMSYSTEM_UPDATE")
-    EL = descriptors.WatchedProperty(float, "QUANTUMSYSTEM_UPDATE")
-    flux = descriptors.WatchedProperty(float, "QUANTUMSYSTEM_UPDATE")
-    cutoff = descriptors.WatchedProperty(int, "QUANTUMSYSTEM_UPDATE")
+    E_osc = descriptors.WatchedProperty(float, "QUANTUMSYSTEM_UPDATE")
+    l_osc = descriptors.WatchedProperty(float, "QUANTUMSYSTEM_UPDATE")
 
     def __init__(
         self,
-        EJ: float,
-        EC: float,
-        EL: float,
-        flux: float,
-        cutoff: int,
-        truncated_dim: int = 6,
+        E_osc: float,
+        l_osc: Union[float, None] = None,
+        truncated_dim: int = _default_evals_count,
         id_str: Optional[str] = None,
     ) -> None:
         base.QuantumSystem.__init__(self, id_str=id_str)
-        self.EJ = EJ
-        self.EC = EC
-        self.EL = EL
-        self.flux = flux
-        self.cutoff = cutoff
-        self.truncated_dim = truncated_dim
-        self._default_grid = discretization.Grid1d(-4.5 * np.pi, 4.5 * np.pi, 151)
+        self.truncated_dim: int = truncated_dim  # type:ignore
+        self.l_osc: Union[None, float] = l_osc  # type:ignore
+        self.E_osc = E_osc
         self._image_filename = os.path.join(
-            os.path.dirname(os.path.abspath(__file__)), "qubit_img/fluxonium.jpg"
+            os.path.dirname(os.path.abspath(__file__)), "qubit_img/oscillator.jpg"
         )
 
     @staticmethod
     def default_params() -> Dict[str, Any]:
-        return {
-            "EJ": 8.9,
-            "EC": 2.5,
-            "EL": 0.5,
-            "flux": 0.0,
-            "cutoff": 110,
-            "truncated_dim": 10,
-        }
+        return {"E_osc": 5.0, "l_osc": 1, "truncated_dim": _default_evals_count}
 
-    @classmethod
-    def supported_noise_channels(cls) -> List[str]:
-        """Return a list of supported noise channels"""
-        return [
-            "tphi_1_over_f_cc",
-            "tphi_1_over_f_flux",
-            "t1_capacitive",
-            "t1_charge_impedance",
-            "t1_flux_bias_line",
-            "t1_inductive",
-            "t1_quasiparticle_tunneling",
-        ]
-
-    @classmethod
-    def effective_noise_channels(cls) -> List[str]:
-        """Return a default list of channels used when calculating effective t1 and t2
-        noise."""
-        noise_channels = cls.supported_noise_channels()
-        noise_channels.remove("t1_charge_impedance")
-        return noise_channels
+    def eigenvals(self, evals_count: int = _default_evals_count) -> ndarray:
+        """Returns array of eigenvalues.
 
-    def phi_osc(self) -> float:
-        """
-        Returns
-        -------
-            Returns oscillator length for the LC oscillator composed of the fluxonium
-             inductance and capacitance.
+        Parameters
+        ----------
+        evals_count:
+            number of desired eigenvalues (default value = 6)
         """
-        return (8.0 * self.EC / self.EL) ** 0.25  # LC oscillator length
+        evals = [self.E_osc * n for n in range(evals_count)]
+        return np.asarray(evals)
 
-    def plasma_energy(self) -> float:
-        """
-        Returns
-        -------
-            Returns the plasma oscillation frequency, sqrt(8*EL*EC).
-        """
-        return math.sqrt(8.0 * self.EL * self.EC)  # LC plasma oscillation energy
+    def eigensys(
+        self, evals_count: int = _default_evals_count
+    ) -> Tuple[ndarray, ndarray]:
+        """Returns array of eigenvalues and eigenvectors
 
-    def phi_operator(self) -> ndarray:
-        """
-        Returns
-        -------
-            Returns the phi operator in the LC harmonic oscillator basis
+        Parameters
+        ----------
+        evals_count:
+            number of desired eigenvalues (default value = 6)
         """
-        dimension = self.hilbertdim()
-        return (
-            (op.creation(dimension) + op.annihilation(dimension))
-            * self.phi_osc()
-            / math.sqrt(2)
-        )
+        evals_count = evals_count or _default_evals_count
+        evecs = np.zeros(shape=(self.truncated_dim, evals_count), dtype=np.float_)
+        np.fill_diagonal(evecs, 1.0)
 
-    def n_operator(self) -> ndarray:
-        """
-        Returns
-        -------
-            Returns the :math:`n = - i d/d\\phi` operator in the LC harmonic
-            oscillator basis
-        """
-        dimension = self.hilbertdim()
-        return (
-            1j
-            * (op.creation(dimension) - op.annihilation(dimension))
-            / (self.phi_osc() * math.sqrt(2))
+        return self.eigenvals(evals_count=evals_count), evecs
+
+    def hilbertdim(self) -> int:
+        """Returns Hilbert space dimension"""
+        return self.truncated_dim
+
+    def creation_operator(self) -> ndarray:
+        """Returns the creation operator"""
+        return op.creation(self.truncated_dim)
+
+    def annihilation_operator(self) -> ndarray:
+        """Returns the creation operator"""
+        return op.annihilation(self.truncated_dim)
+
+    def matrixelement_table(self, *args, **kwargs) -> ndarray:
+        raise NotImplementedError(
+            "The Oscillator class does not implement the matrixelement_table method."
         )
 
-    def exp_i_phi_operator(self, alpha: float = 1.0, beta: float = 0.0) -> ndarray:
-        """
-        Returns
-        -------
-            Returns the :math:`e^{i (\\alpha \\phi + \\beta) }` operator in the
-            LC harmonic oscillator basis,
-            with :math:`\\alpha` and :math:`\\beta` being numbers
-        """
-        exponent = 1j * (alpha * self.phi_operator())
-        return sp.linalg.expm(exponent) * cmath.exp(1j * beta)
+    def phi_operator(self) -> ndarray:
+        r"""Returns the phase operator defined as
+        :math:`l_\text{osc} (a + a^{\dagger})/\sqrt{2}`, with :math:`a` representing
+        an annihilation operator, and :math:`l_\text{osc}` the oscillator length.
+        """
+        if self.l_osc is None:
+            raise ValueError(
+                "Variable l_osc has to be set to something other than None\n"
+                + "in order to use the phi_operator() method. This can be done by either\n"
+                + "passing it to the class constructor, or by setting it afterwords."
+            )
+        a = op.annihilation(self.truncated_dim)
+        return self.l_osc / np.sqrt(2) * (a + a.T)
 
-    def cos_phi_operator(self, alpha: float = 1.0, beta: float = 0.0) -> ndarray:
-        """
-        Returns
-        -------
-            Returns the :math:`\\cos (\\alpha \\phi + \\beta)` operator in the LC
-            harmonic oscillator basis,
-            with :math:`\\alpha` and :math:`\\beta` being numbers
+    def n_operator(self) -> ndarray:
+        r"""Returns the charge-number n operator defined as
+        :math:`i (a^{\dagger} - a)/ ( \sqrt{2} l_\text{osc})`, with :math:`a` representing
+        an annihilation operator, and :math:`l_\text{osc}` the oscillator length.
         """
-        argument = alpha * self.phi_operator() + beta * np.eye(self.hilbertdim())
-        return sp.linalg.cosm(argument)
 
-    def sin_phi_operator(self, alpha: float = 1.0, beta: float = 0.0) -> ndarray:
-        """
-        Returns
-        -------
-            Returns the :math:`\\sin (\\alpha \\phi + \\beta)` operator in the
-            LC harmonic oscillator basis
-            with :math:`\\alpha` and :math:`\\beta` being numbers
-        """
-        argument = alpha * self.phi_operator() + beta * np.eye(self.hilbertdim())
-        return sp.linalg.sinm(argument)
+        if self.l_osc is None:
+            raise ValueError(
+                "Variable l_osc has to be set to something other than None\n"
+                + "in order to use the n_operator() method. This can be done by either\n"
+                + "passing it to the class constructor, or by setting it afterwords."
+            )
+        a = op.annihilation(self.truncated_dim)
+        return 1.0j / (self.l_osc * np.sqrt(2)) * (a.T - a)
 
-    def hamiltonian(self) -> ndarray:  # follow Zhu et al., PRB 87, 024510 (2013)
-        """Construct Hamiltonian matrix in harmonic-oscillator basis, following Zhu
-        et al., PRB 87, 024510 (2013)"""
-        dimension = self.hilbertdim()
-        diag_elements = [(i + 0.5) * self.plasma_energy() for i in range(dimension)]
-        lc_osc_matrix = np.diag(diag_elements)
-
-        cos_matrix = self.cos_phi_operator(beta=2 * np.pi * self.flux)
-
-        hamiltonian_mat = lc_osc_matrix - self.EJ * cos_matrix
-        return hamiltonian_mat
-
-    def d_hamiltonian_d_EJ(self) -> ndarray:
-        """Returns operator representing a derivative of the Hamiltonian with respect
-        to `EJ`.
 
-        The flux is grouped as in the Hamiltonian.
-        """
-        return -self.cos_phi_operator(1, 2 * np.pi * self.flux)
+# -KerrOscillator class-------------------------------------------------------------------
 
-    def d_hamiltonian_d_flux(self) -> ndarray:
-        """Returns operator representing a derivative of the Hamiltonian with respect
-        to `flux`.
 
-        Flux is grouped as in the Hamiltonian.
-        """
-        return -2 * np.pi * self.EJ * self.sin_phi_operator(1, 2 * np.pi * self.flux)
+class KerrOscillator(Oscillator, serializers.Serializable):
+    r"""Class representing a nonlinear Kerr oscillator/resonator governed by a Hamiltonian
+    :math:`H_\text{Kerr}=E_\text{osc} a^{\dagger} a - K a^{\dagger} a^{\dagger} a a`, with :math:`a`
+    being the annihilation operator.
 
-    def hilbertdim(self) -> int:
-        """
-        Returns
-        -------
-            Returns the Hilbert space dimension."""
-        return self.cutoff
+    Parameters
+    ----------
+    E_osc:
+        energy of harmonic term
+    K:
+        energy of the Kerr term
+    l_osc:
+        oscillator length (used to define phi_operator and n_operator)
+    truncated_dim:
+        desired dimension of the truncated quantum system; expected: truncated_dim > 1
+    id_str:
+        optional string by which this instance can be referred to in `HilbertSpace`
+        and `ParameterSweep`. If not provided, an id is auto-generated.
+    """
+    K = descriptors.WatchedProperty(float, "QUANTUMSYSTEM_UPDATE")
 
-    def potential(self, phi: Union[float, ndarray]) -> ndarray:
-        """Fluxonium potential evaluated at `phi`.
+    def __init__(
+        self,
+        E_osc: float,
+        K: float,
+        l_osc: Union[float, None] = None,
+        truncated_dim: int = _default_evals_count,
+        id_str: Optional[str] = None,
+    ) -> None:
+        self.K: float = K  # type:ignore
 
-        Parameters
-        ----------
-            float value of the phase variable `phi`
+        super().__init__(
+            E_osc=E_osc,
+            l_osc=l_osc,
+            truncated_dim=truncated_dim,
+            id_str=id_str,
+        )
 
-        Returns
-        -------
-        float or ndarray
-        """
-        return 0.5 * self.EL * phi * phi - self.EJ * np.cos(
-            phi + 2.0 * np.pi * self.flux
+        self._image_filename = os.path.join(
+            os.path.dirname(os.path.abspath(__file__)), "qubit_img/kerr-oscillator.jpg"
         )
 
-    def wavefunction(
-        self,
-        esys: Optional[Tuple[ndarray, ndarray]],
-        which: int = 0,
-        phi_grid: "Grid1d" = None,
-    ) -> storage.WaveFunction:
-        """Returns a fluxonium wave function in `phi` basis
+    @staticmethod
+    def default_params() -> Dict[str, Any]:
+        return {
+            "E_osc": 5.0,
+            "K": 0.05,
+            "l_osc": 1,
+            "truncated_dim": _default_evals_count,
+        }
+
+    def eigenvals(self, evals_count: int = _default_evals_count) -> ndarray:
+        """Returns array of eigenvalues.
 
         Parameters
         ----------
-        esys:
-            eigenvalues, eigenvectors
-        which:
-             index of desired wave function (default value = 0)
-        phi_grid:
-            used for setting a custom grid for phi; if None use self._default_grid
+        evals_count:
+            number of desired eigenvalues (default value = 6)
         """
-        if esys is None:
-            evals_count = max(which + 1, 3)
-            evals, evecs = self.eigensys(evals_count=evals_count)
-        else:
-            evals, evecs = esys
-        dim = self.hilbertdim()
-
-        phi_grid = phi_grid or self._default_grid
-
-        phi_basis_labels = phi_grid.make_linspace()
-        wavefunc_osc_basis_amplitudes = evecs[:, which]
-        phi_wavefunc_amplitudes = np.zeros(phi_grid.pt_count, dtype=np.complex_)
-        phi_osc = self.phi_osc()
-        for n in range(dim):
-            phi_wavefunc_amplitudes += wavefunc_osc_basis_amplitudes[
-                n
-            ] * osc.harm_osc_wavefunction(n, phi_basis_labels, phi_osc)
-        return storage.WaveFunction(
-            basis_labels=phi_basis_labels,
-            amplitudes=phi_wavefunc_amplitudes,
-            energy=evals[which],
-        )
+        evals = [
+            (self.E_osc + self.K) * n - self.K * n**2 for n in range(evals_count)
+        ]
+        return np.asarray(evals)
```

### Comparing `scqubits-3.1.0/scqubits/core/generic_qubit.py` & `scqubits-3.1.1/scqubits/core/generic_qubit.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import scqubits.core.descriptors as descriptors
 import scqubits.core.operators as operators
 import scqubits.core.qubit_base as base
 import scqubits.io_utils.fileio_serializers as serializers
 
 from scqubits.utils.spectrum_utils import get_matrixelement_table, order_eigensystem
 
-# —generic qubit (two-level system)——————————————————————————————————————————————
+# -generic qubit (two-level system)----------------------------------------------
 
 
 class GenericQubit(base.QuantumSystem, serializers.Serializable):
     """Class for a generic qubit (genuine two-level system). Create a class instance
     via::
 
         GenericQubit(E=4.3)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scqubits-3.1.0/scqubits/core/hilbert_space.py` & `scqubits-3.1.1/scqubits/core/hilbert_space.py`

 * *Files 3% similar despite different names*

```diff
@@ -311,15 +311,15 @@
             return hamiltonian + hamiltonian.dag()
 
 
 class HilbertSpace(
     spec_lookup.SpectrumLookupMixin, dispatch.DispatchClient, serializers.Serializable
 ):
     """Class holding information about the full Hilbert space, usually composed of
-    multiple subsys_list. The class provides methods to turn subsystem operators into
+    multiple subsystems. The class provides methods to turn subsystem operators into
     operators acting on the full Hilbert space, and establishes the interface to
     qutip. Returned operators are of the `qutip.Qobj` type. The class also provides
     methods for obtaining eigenvalues, absorption and emission spectra as a function
     of an external parameter.
 
     Parameters
     ----------
@@ -327,14 +327,15 @@
         List of all quantum systems comprising the composite Hilbert space
     interaction_list:
         (optional) typically, interaction terms are added one by one by means of the
         `add_interaction` method. Alternatively, a list of interaction term objects
         can be supplied here upon initialization of a `HilbertSpace` instance.
     """
 
+    _lookup_exists = False
     osc_subsys_list = descriptors.ReadOnlyProperty(OscillatorList)
     qbt_subsys_list = descriptors.ReadOnlyProperty(QubitList)
     interaction_list = descriptors.WatchedProperty(
         Tuple[Union[InteractionTerm, InteractionTermStr], ...], "INTERACTIONLIST_UPDATE"
     )
 
     def __init__(
@@ -344,28 +345,27 @@
         ignore_low_overlap: bool = False,
     ) -> None:
         if has_duplicate_id_str(subsystem_list):
             raise ValueError(
                 "Subsystem list must not contain multiple objects with "
                 "the same `id_str` name."
             )
-        self._subsystems: Tuple[QuantumSys, ...] = tuple(subsystem_list)
+        self._subsystems: List[QuantumSys] = subsystem_list
         self._subsys_by_id_str = {
             obj._id_str: self[index] for index, obj in enumerate(self)
         }
         if interaction_list:
             self.interaction_list = interaction_list
         else:
             self.interaction_list: List[InteractionTerm] = []
         self._interaction_term_by_id_str = {
             "InteractionTerm_{}".format(index): interaction_term
             for index, interaction_term in enumerate(self.interaction_list)
         }
 
-        self._lookup: Optional[spec_lookup.SpectrumLookupAdapter] = None
         self._osc_subsys_list = [
             subsys for subsys in self if isinstance(subsys, osc.Oscillator)
         ]
         self._qbt_subsys_list = [
             subsys for subsys in self if not isinstance(subsys, osc.Oscillator)
         ]
 
@@ -436,47 +436,44 @@
                 output += term_output
         return output
 
     def __len__(self):
         return len(self._subsystems)
 
     @property
-    def lookup(self):
-        """[Legacy] supporting old lookup interface."""
-        return self._lookup
-
-    @property
-    def hilbertspace(self) -> "HilbertSpace":
+    def hilbertspace(self) -> HilbertSpace:
         """[Legacy] Auxiliary reference to self for compatibility with
         SpectrumLookupMixin
         class."""
         return self
 
     @property
+    @utils.DeprecationMessage(
+        "`subsys_list` is deprecated. Use `subsystem_list` instead."
+    )
     def subsys_list(self) -> List[QuantumSys]:
         return list(self._subsystems)
 
     def subsys_by_id_str(self, id_str: str) -> QuantumSys:
         return self._subsys_by_id_str[id_str]
 
     ###################################################################################
     # HilbertSpace: file IO methods
     ###################################################################################
     @classmethod
-    def deserialize(cls, io_data: "IOData") -> "HilbertSpace":
+    def deserialize(cls, io_data: "IOData") -> HilbertSpace:
         """
         Take the given IOData and return an instance of the described class,
         initialized with the data stored in io_data.
         """
         alldata_dict = io_data.as_kwargs()
         alldata_dict["ignore_low_overlap"] = alldata_dict.pop("_ignore_low_overlap")
         data = alldata_dict.pop("_data", {})
-        new_hilbertspace: "HilbertSpace" = cls(**alldata_dict)
+        new_hilbertspace: HilbertSpace = cls(**alldata_dict)
         new_hilbertspace._data = data
-        new_hilbertspace._lookup = spec_lookup.SpectrumLookupAdapter(new_hilbertspace)
         return new_hilbertspace
 
     def serialize(self) -> "IOData":
         """
         Convert the content of the current class instance into IOData format.
         """
         init_parameters = self._init_params
@@ -497,69 +494,69 @@
             "interaction_list": self.interaction_list,
         }
 
     ###################################################################################
     # HilbertSpace: creation via GUI
     ###################################################################################
     @classmethod
-    def create(cls) -> "HilbertSpace":
+    def create(cls) -> HilbertSpace:
         hilbertspace = cls([])
         scqubits.ui.hspace_widget.create_hilbertspace_widget(hilbertspace.__init__)
         return hilbertspace
 
     ###################################################################################
     # HilbertSpace: methods for CentralDispatch
     ###################################################################################
     def receive(self, event: str, sender: Any, **kwargs) -> None:
         if event == "QUANTUMSYSTEM_UPDATE" and sender in self:
             self.broadcast("HILBERTSPACE_UPDATE")
-            if self._lookup:
-                self._lookup._out_of_sync = True
+            if self.lookup_exists():
+                self._out_of_sync = True
         elif event == "INTERACTIONTERM_UPDATE" and sender in self.interaction_list:
             self.broadcast("HILBERTSPACE_UPDATE")
-            if self._lookup:
-                self._lookup._out_of_sync = True
+            if self.lookup_exists():
+                self._out_of_sync = True
         elif event == "INTERACTIONLIST_UPDATE" and sender is self:
             self.broadcast("HILBERTSPACE_UPDATE")
-            if self._lookup:
-                self._lookup._out_of_sync = True
+            if self.lookup_exists():
+                self._out_of_sync = True
 
     ###################################################################################
     # HilbertSpace: subsystems, dimensions, etc.
     ###################################################################################
     def get_subsys_index(self, subsys: QuantumSys) -> int:
         """
         Return the index of the given subsystem in the HilbertSpace.
         """
         return self._subsystems.index(subsys)
 
     @property
-    def subsystem_list(self) -> Tuple[QuantumSys, ...]:
+    def subsystem_list(self) -> List[QuantumSys]:
         return self._subsystems
 
     @property
     def subsystem_dims(self) -> List[int]:
         """Returns list of the Hilbert space dimensions of each subsystem"""
         return [subsystem.truncated_dim for subsystem in self]
 
     @property
     def dimension(self) -> int:
         """Returns total dimension of joint Hilbert space"""
         return np.prod(np.asarray(self.subsystem_dims))  # type:ignore
 
     @property
     def subsystem_count(self) -> int:
-        """Returns number of subsys_list composing the joint Hilbert space"""
+        """Returns number of subsystems composing the joint Hilbert space"""
         return len(self._subsystems)
 
     ###################################################################################
     # HilbertSpace: generate SpectrumLookup
     ###################################################################################
     def generate_lookup(self, update_subsystem_indices: List[int] = None) -> None:
-
+        self._lookup_exists = True
         bare_esys_dict = self.generate_bare_esys(
             update_subsystem_indices=update_subsystem_indices
         )
         dummy_params = self._parameters.paramvals_by_name
 
         evals, evecs = self.eigensys(
             evals_count=self.dimension, bare_esys=bare_esys_dict
@@ -570,17 +567,19 @@
         evecs_wrapped[0] = evecs
 
         self._data["evals"] = NamedSlotsNdarray(np.array([evals]), dummy_params)
         self._data["evecs"] = NamedSlotsNdarray(evecs_wrapped, dummy_params)
         self._data["dressed_indices"] = spec_lookup.SpectrumLookupMixin.generate_lookup(
             self
         )
-        self._lookup = spec_lookup.SpectrumLookupAdapter(self)
 
-    def generate_bare_esys(self, update_subsystem_indices: List[int] = None) -> None:
+    def lookup_exists(self) -> bool:
+        return self._lookup_exists
+
+    def generate_bare_esys(self, update_subsystem_indices: List[int] = None) -> dict:
         # update all the subsystems when update_subsystem_indices is set to None
         if update_subsystem_indices is None:
             update_subsystem_indices = list(range(self.subsystem_count))
 
         bare_evals = np.empty((self.subsystem_count,), dtype=object)
         bare_evecs = np.empty((self.subsystem_count,), dtype=object)
         bare_esys_dict = {}
@@ -617,15 +616,15 @@
     ##################################################################################
     def eigenvals(
         self,
         evals_count: int = 6,
         bare_esys: Optional[Dict[int, Union[ndarray, List[ndarray]]]] = None,
     ) -> ndarray:
         """Calculates eigenvalues of the full Hamiltonian using
-        `qutip.Qob.eigenenergies()`.
+        `qutip.Qobj.eigenenergies()`.
 
         Parameters
         ----------
         evals_count:
             number of desired eigenvalues/eigenstates
         bare_esys:
             optionally, the bare eigensystems for each subsystem can be provided to
@@ -636,15 +635,15 @@
 
     def eigensys(
         self,
         evals_count: int = 6,
         bare_esys: Optional[Dict[int, Union[ndarray, List[ndarray]]]] = None,
     ) -> Tuple[ndarray, QutipEigenstates]:
         """Calculates eigenvalues and eigenvectors of the full Hamiltonian using
-        `qutip.Qob.eigenstates()`.
+        `qutip.Qobj.eigenstates()`.
 
         Parameters
         ----------
         evals_count:
             number of desired eigenvalues/eigenstates
         bare_esys:
             optionally, the bare eigensystems for each subsystem can be provided to
@@ -709,15 +708,15 @@
         ----------
         bare_esys:
             optionally, the bare eigensystems for each subsystem can be provided to
             speed up computation; these are provided in dict form via <subsys>: esys
 
         Returns
         -------
-            composite Hamiltonian composed of bare Hamiltonians of subsys_list
+            composite Hamiltonian composed of bare Hamiltonians of subsystems
             independent of the external parameter
         """
         bare_hamiltonian = Qobj(0)
         for subsys_index, subsys in enumerate(self):
             if bare_esys is not None and subsys_index in bare_esys:
                 evals = bare_esys[subsys_index][0]
             else:
@@ -747,15 +746,15 @@
 
         operator_list = []
         for term in self.interaction_list:
             if isinstance(term, Qobj):
                 operator_list.append(term)
             elif isinstance(term, (InteractionTerm, InteractionTermStr)):
                 operator_list.append(
-                    term.hamiltonian(self.subsys_list, bare_esys=bare_esys)
+                    term.hamiltonian(self.subsystem_list, bare_esys=bare_esys)
                 )
             else:
                 raise TypeError(
                     "Expected an instance of InteractionTerm, InteractionTermStr, "
                     "or Qobj; got {} instead.".format(type(term))
                 )
         hamiltonian = sum(operator_list)
@@ -773,63 +772,63 @@
             Eigenenergies can be provided as `evals`; otherwise, they are calculated.
         """
         evals_count = subsystem.truncated_dim
 
         if evals is None:
             evals = subsystem.eigenvals(evals_count=evals_count)
         diag_qt_op = qt.Qobj(inpt=np.diagflat(evals[0:evals_count]))  # type:ignore
-        return spec_utils.identity_wrap(diag_qt_op, subsystem, self.subsys_list)
+        return spec_utils.identity_wrap(diag_qt_op, subsystem, self.subsystem_list)
 
     ###################################################################################
     # HilbertSpace: identity wrapping, operators
     ###################################################################################
 
     def diag_operator(self, diag_elements: ndarray, subsystem: QuantumSys) -> Qobj:
         """For given diagonal elements of a diagonal operator in `subsystem`, return
         the `Qobj` operator for the full Hilbert space (perform wrapping in
-        identities for other subsys_list).
+        identities for other subsystems).
 
         Parameters
         ----------
         diag_elements:
             diagonal elements of subsystem diagonal operator
         subsystem:
             subsystem where diagonal operator is defined
         """
         dim = subsystem.truncated_dim
         index = range(dim)
         diag_matrix = np.zeros((dim, dim), dtype=np.float_)
         diag_matrix[index, index] = diag_elements
-        return spec_utils.identity_wrap(diag_matrix, subsystem, self.subsys_list)
+        return spec_utils.identity_wrap(diag_matrix, subsystem, self.subsystem_list)
 
     def hubbard_operator(self, j: int, k: int, subsystem: QuantumSys) -> Qobj:
         """Hubbard operator :math:`|j\\rangle\\langle k|` for system `subsystem`
 
         Parameters
         ----------
         j,k:
             eigenstate indices for Hubbard operator
         subsystem:
             subsystem in which Hubbard operator acts
         """
         dim = subsystem.truncated_dim
         operator = qt.states.basis(dim, j) * qt.states.basis(dim, k).dag()
-        return spec_utils.identity_wrap(operator, subsystem, self.subsys_list)
+        return spec_utils.identity_wrap(operator, subsystem, self.subsystem_list)
 
     def annihilate(self, subsystem: QuantumSys) -> Qobj:
         """Annihilation operator a for `subsystem`
 
         Parameters
         ----------
         subsystem:
             specifies subsystem in which annihilation operator acts
         """
         dim = subsystem.truncated_dim
         operator = qt.destroy(dim)
-        return spec_utils.identity_wrap(operator, subsystem, self.subsys_list)
+        return spec_utils.identity_wrap(operator, subsystem, self.subsystem_list)
 
     ###################################################################################
     # HilbertSpace: spectrum sweep
     ###################################################################################
     def get_spectrum_vs_paramvals(
         self,
         param_vals: ndarray,
@@ -920,14 +919,71 @@
             eigenvalue_table,
             self.get_initdata(),
             param_name,
             param_vals,
             state_table=eigenstate_table,
         )
 
+    def standardize_eigenvector_phases(self) -> None:
+        """
+        Standardize the phases of the (dressed) eigenvectors.
+        """
+        for idx, evec in enumerate(self._data["evecs"][0]):
+            phase = spec_utils.extract_phase(evec.data.toarray())
+            self._data["evecs"][0][idx] = evec * np.exp(-1j * phase)
+
+    def op_in_dressed_eigenbasis(self, **kwargs) -> Qobj:
+        """
+        Express a subsystem operator in the dressed eigenbasis of the full system
+        (as opposed to both the "native basis" or "bare eigenbasis" of the subsystem).
+        `op_in_dressed_eigenbasis(...)` offers two different interfaces:
+
+        1. subsystem operators may be expressed as Callables
+
+            signature::
+
+                .op_in_dressed_eigenbasis(op=<Callable>)
+
+        2. subsystem operators may be passed as arrays, along with the
+           corresponding subsystem. In this case the user must additionally
+           specify if the operator is in the native, subsystem-internal
+           basis or the subsystem bare eigenbasis::
+
+                .op_in_dressed_eigenbasis(op=(<ndarray>, <subsys>),
+                                          op_in_bare_eigenbasis=<Bool>)
+        """
+        op_callable_or_tuple = kwargs.pop("op")
+        if isinstance(op_callable_or_tuple, Callable):
+            subsys_index, op = self._parse_op(op_callable_or_tuple)
+            return self._op_in_dressed_eigenbasis(
+                op, subsys_index, op_in_bare_eigenbasis=False
+            )
+        else:
+            op, subsys = op_callable_or_tuple
+            op_in_bare_eigenbasis = kwargs.pop("op_in_bare_eigenbasis", False)
+            subsys_index = self.get_subsys_index(subsys)
+            return self._op_in_dressed_eigenbasis(
+                op, subsys_index, op_in_bare_eigenbasis
+            )
+
+    def _op_in_dressed_eigenbasis(
+        self, op: ndarray, subsys_index: int, op_in_bare_eigenbasis: bool = False
+    ) -> Qobj:
+        bare_evecs = self._data["bare_evecs"][subsys_index][0]
+        id_wrapped_op = spec_utils.identity_wrap(
+            op,
+            self.subsystem_list[subsys_index],
+            self.subsystem_list,
+            op_in_eigenbasis=op_in_bare_eigenbasis,
+            evecs=bare_evecs,
+        )
+        dressed_evecs = self._data["evecs"][0]
+        dressed_op = id_wrapped_op.transform(dressed_evecs)
+        return dressed_op
+
     ###################################################################################
     # HilbertSpace: add interaction and parsing arguments to .add_interaction
     ###################################################################################
     def add_interaction(
         self, check_validity=True, id_str: Optional[str] = None, **kwargs
     ) -> None:
         """
@@ -984,16 +1040,16 @@
             interaction = self._parse_qobj(**kwargs)
         elif "op1" in kwargs:
             interaction = self._parse_interactionterm(**kwargs)
         else:
             raise TypeError(
                 "Invalid combination and/or types of arguments for `add_interaction`"
             )
-        if self._lookup is not None:
-            self._lookup._out_of_sync = True
+        if self.lookup_exists():
+            self._out_of_sync = True
 
         self.interaction_list.append(interaction)
 
         id_str = id_str or "Interaction_{}".format(len(self.interaction_list))
         self._interaction_term_by_id_str[id_str] = interaction
 
         if not check_validity:
```

### Comparing `scqubits-3.1.0/scqubits/core/namedslots_array.py` & `scqubits-3.1.1/scqubits/core/namedslots_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import warnings
 
 from collections import OrderedDict
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
 
+from matplotlib import rc_context
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from numpy import ndarray
 
 import scqubits.settings as settings
 import scqubits.utils.misc as utils
 import scqubits.utils.plotting as plot
@@ -602,14 +603,15 @@
             }
         return io.IOData(typename, io_attributes, io_ndarrays, objects=objects)
 
     @property
     def slot_count(self) -> int:
         return len(self._parameters.paramvals_by_name)
 
+    @rc_context(settings.matplotlib_settings)
     def plot(self, **kwargs) -> Tuple[Figure, Axes]:
         if len(self._parameters) != 1:
             raise ValueError(
                 "Plotting of NamedSlotNdarray only supported for a "
                 "one-dimensional parameter sweep. (Consider slicing.)"
             )
         return plot.data_vs_paramvals(
```

### Comparing `scqubits-3.1.0/scqubits/core/noise.py` & `scqubits-3.1.1/scqubits/core/noise.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 import math
 import warnings
 
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 
 import matplotlib.pyplot as plt
+import matplotlib as mpl
 import numpy as np
 import scipy as sp
-import scipy.constants
 
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from matplotlib.offsetbox import AnchoredText
 from numpy import ndarray
 from scipy.sparse import csc_matrix
 
 import scqubits.core.units as units
 import scqubits.settings as settings
 import scqubits.utils.plotting as plotting
 
 from scqubits.core.storage import SpectrumData
+from scqubits.settings import matplotlib_settings
+
 
 # flag that lets us show a warning about the default t1 behavior
 # (i.e., total=True setting) only once. Using the standard warnings
 # filtering does not seem to work in jupyter.
 _t1_default_warning_given_flag = False
 
 
@@ -114,14 +116,15 @@
     @classmethod
     def effective_noise_channels(cls) -> List[str]:
         """Return a list of noise channels that are used when calculating the
         effective noise (i.e. via `t1_effective` and `t2_effective`.
         """
         return cls.supported_noise_channels()
 
+    @mpl.rc_context(matplotlib_settings)
     def plot_coherence_vs_paramvals(
         self,
         param_name: str,
         param_vals: ndarray,
         noise_channels: Union[str, List[str], List[Tuple[str, Dict]]] = None,
         common_noise_options: Dict = None,
         spectrum_data: SpectrumData = None,
@@ -243,15 +246,14 @@
             }
         )
 
         # remember current value of param_name
         current_val = getattr(self, param_name)
 
         for channel_idx, noise_channel in enumerate(noise_channels):  # type:ignore
-
             # case 1: noise_channel is a string representing the noise method
             if isinstance(noise_channel, str):
                 noise_channel_method = noise_channel
 
                 # calculate the noise over the full param span in param_vals
                 noise_vals = np.asarray(
                     [
@@ -327,14 +329,15 @@
 
         # Set the parameter we varied to its initial value
         setattr(self, param_name, current_val)
 
         fig.tight_layout()
         return fig, axes
 
+    @mpl.rc_context(matplotlib_settings)
     def plot_t1_effective_vs_paramvals(
         self,
         param_name: str,
         param_vals: ndarray,
         noise_channels: Union[str, List[str], List[Tuple[str, Dict]]] = None,
         common_noise_options: Dict = None,
         spectrum_data: SpectrumData = None,
@@ -481,14 +484,15 @@
             param_vals, noise_vals, **plotting_options
         )
 
         fig.tight_layout()
 
         return fig, axes
 
+    @mpl.rc_context(matplotlib_settings)
     def plot_t2_effective_vs_paramvals(
         self,
         param_name: str,
         param_vals: ndarray,
         noise_channels: Union[str, List[str], List[Tuple[str, Dict]]] = None,
         common_noise_options: Dict = None,
         spectrum_data: SpectrumData = None,
@@ -562,15 +566,14 @@
         # if we only have a single noise channel to consider (and hence are given a
         # str), put it into a one element list
         noise_channels = (
             [noise_channels] if isinstance(noise_channels, str) else noise_channels
         )
 
         if spectrum_data is None:
-
             # We have to figure out the largest energy level involved in the
             # calculations, to know how many levels we need from the diagonalization.
             # This may be hidden in noise-channel-specific options, so have to search
             # through those, if any were given.
             max_level = max(
                 common_noise_options.get("i", 1), common_noise_options.get("j", 1)
             )
@@ -660,18 +663,16 @@
         Returns
         -------
             coherence rate
         """
         rate = 0.0
 
         for n, noise_channel in enumerate(noise_channels):
-
             # noise_channel is a string representing the noise method
             if isinstance(noise_channel, str):
-
                 noise_channel_method = noise_channel
 
                 # If dealing with a tphi noise type, the contribution of a t1 process
                 # to the dephasing rate its halved.
                 scale_factor = (
                     0.5
                     if noise_type == "tphi" and noise_channel_method.startswith("t1")
@@ -685,15 +686,14 @@
                 # calculate the noise over the full param span in param_vals
                 rate += scale_factor * getattr(self, noise_channel_method)(
                     esys=esys, **options
                 )
 
             # noise_channel is a tuple representing the noise method and default options
             elif isinstance(noise_channel, tuple):
-
                 noise_channel_method = noise_channel[0]
 
                 # If dealing with a tphi noise type, the contribution of a t1 process
                 # to the dephasing rate its halved.
                 scale_factor = (
                     0.5
                     if noise_type == "tphi" and noise_channel_method.startswith("t1")
```

### Comparing `scqubits-3.1.0/scqubits/core/operators.py` & `scqubits-3.1.1/scqubits/core/operators.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/param_sweep.py` & `scqubits-3.1.1/scqubits/core/param_sweep.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 
 class ParameterSweepBase(ABC, SpectrumLookupMixin):
     """
     The_ParameterSweepBase class is an abstract base class for ParameterSweep and
     StoredSweep
     """
 
+    _lookup_exists = False
     _parameters = descriptors.WatchedProperty(Parameters, "PARAMETERSWEEP_UPDATE")
     _evals_count = descriptors.WatchedProperty(int, "PARAMETERSWEEP_UPDATE")
     _data = descriptors.WatchedProperty(Dict[str, ndarray], "PARAMETERSWEEP_UPDATE")
     _hilbertspace: HilbertSpace
 
     _out_of_sync = False
     _current_param_indices: NpIndices
@@ -600,15 +601,15 @@
             diff_energies /= photon_number
             if make_positive:
                 diff_energies = np.abs(diff_energies)
             if not np.isnan(diff_energies).all():  # omit transitions with all nans
                 transitions.append((initial_state, final_state))
                 transition_energies.append(diff_energies)
 
-        self._preslicing_reset()
+        self.reset_preslicing()
 
         if not as_specdata:
             return transitions, transition_energies
 
         label_list = self._generate_transition_labels(
             initial_dressed, final_dressed, transitions
         )
@@ -724,15 +725,15 @@
 
         specdata_all = copy.deepcopy(self[param_indices].dressed_specdata)
         specdata_all.energy_table -= specdata_for_highlighting.subtract  # type:ignore
         specdata_all.energy_table /= photon_number
         if make_positive:
             specdata_all.energy_table = np.abs(specdata_all.energy_table)
 
-        self._preslicing_reset()
+        self.reset_preslicing()
 
         if coloring == "plain":
             return specdata_all.plot_evals_vs_paramvals()
 
         if "fig_ax" in kwargs:
             fig_ax = kwargs.pop("fig_ax")
         else:
@@ -882,15 +883,15 @@
         `<subsystem a>` while leaving other subsystems unchanged. Similarly, sweeping
         `<parameter name 2>` affects `<subsystem b>`, `<subsystem c>` etc.
     bare_only:
         if set to True, only bare eigendata is calculated; useful when performing a
         sweep for a single quantum system, no interaction (default: False)
     ignore_low_overlap:
         if set to False (default), bare product states and dressed eigenstates are
-        identified if `\|<psi_bare\|psi_dressed>\|^2 > 0.5`; if True,
+        identified if `|<psi_bare|psi_dressed>|^2 > 0.5`; if True,
         then identification will always take place based on which bare product state
         has the maximum overlap
     autorun:
         Determines whether to directly run the sweep or delay it until `.run()` is
         called manually. (Default: `settings.AUTORUN_SWEEP=True`)
     deepcopy:
         if set to True, the parameter sweep is run with an exact copy of the Hilbert
@@ -951,15 +952,15 @@
         self._bare_only = bare_only
         self._ignore_low_overlap = ignore_low_overlap
         self._deepcopy = deepcopy
         self._num_cpus = num_cpus
         self.tqdm_disabled = settings.PROGRESSBAR_DISABLED or (num_cpus > 1)
 
         self._out_of_sync = False
-        self._preslicing_reset()
+        self.reset_preslicing()
 
         dispatch.CENTRAL_DISPATCH.register("PARAMETERSWEEP_UPDATE", self)
         dispatch.CENTRAL_DISPATCH.register("HILBERTSPACE_UPDATE", self)
 
         if autorun:
             self.run()
 
@@ -990,14 +991,15 @@
         return iodata
 
     def run(self) -> None:
         """Create all sweep data: bare spectral data, dressed spectral data, lookup
         data and custom sweep data."""
         # generate one dispatch before temporarily disabling CENTRAL_DISPATCH
 
+        self._lookup_exists = True
         if self._deepcopy:
             stored_hilbertspace = copy.deepcopy(self.hilbertspace)
             self._hilbertspace = copy.deepcopy(self.hilbertspace)
         else:
             self.cause_dispatch()
         settings.DISPATCH_ENABLED = False
 
@@ -1321,14 +1323,15 @@
     def __init__(
         self,
         paramvals_by_name: Dict[str, ndarray],
         hilbertspace: HilbertSpace,
         evals_count: int,
         _data,
     ) -> None:
+        self._lookup_exists = True
         self._parameters = Parameters(paramvals_by_name)
         self._hilbertspace = hilbertspace
         self._evals_count = evals_count
         self._data = _data
 
         self._out_of_sync = False
         self._current_param_indices: NpIndices = slice(None, None, None)
```

### Comparing `scqubits-3.1.0/scqubits/core/qubit_base.py` & `scqubits-3.1.1/scqubits/core/qubit_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,32 +26,34 @@
     Optional,
     Tuple,
     Union,
     overload,
 )
 
 import matplotlib.pyplot as plt
+import matplotlib as mpl
 import numpy as np
 import scipy as sp
 
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from numpy import ndarray
+from scipy.sparse import csc_matrix, dia_matrix
 
 import scqubits.core.constants as constants
 import scqubits.core.descriptors as descriptors
 import scqubits.core.units as units
 import scqubits.settings as settings
 import scqubits.ui.qubit_widget as ui
 import scqubits.utils.plotting as plot
 
 from scqubits.core.central_dispatch import DispatchClient
 from scqubits.core.discretization import Grid1d
 from scqubits.core.storage import DataStore, SpectrumData
-from scqubits.settings import IN_IPYTHON
+from scqubits.settings import IN_IPYTHON, matplotlib_settings
 from scqubits.utils.cpu_switch import get_map_method
 from scqubits.utils.misc import InfoBar, process_which
 from scqubits.utils.spectrum_utils import (
     get_matrixelement_table,
     order_eigensystem,
     recast_esys_mapdata,
     standardize_sign,
@@ -68,15 +70,15 @@
     from scqubits.core.storage import WaveFunction
 
 
 LevelsTuple = Tuple[int, ...]
 Transition = Tuple[int, int]
 TransitionsTuple = Tuple[Transition, ...]
 
-# —Generic quantum system container and Qubit base class——————————————————————————————
+# -Generic quantum system container and Qubit base class------------------------------
 
 
 class QuantumSystem(DispatchClient, ABC):
     """Generic quantum system class"""
 
     truncated_dim = descriptors.WatchedProperty(int, "QUANTUMSYSTEM_UPDATE")
     _init_params: List[str]
@@ -225,15 +227,15 @@
         """
         Returns a list of noise channels this QuantumSystem supports. If none,
         return an empty list.
         """
         return []
 
 
-# —QubitBaseClass———————————————————————————————————————————————————————————————————————————————————————————————————————
+# -QubitBaseClass-------------------------------------------------------------------------------------------------------
 
 
 class QubitBaseClass(QuantumSystem, ABC):
     """Base class for superconducting qubit objects. Provide general mechanisms and
     routines for plotting spectra, matrix elements, and writing data to files
     """
 
@@ -246,22 +248,22 @@
     @abstractmethod
     def hamiltonian(self):
         """Returns the Hamiltonian"""
 
     def _evals_calc(self, evals_count: int) -> ndarray:
         hamiltonian_mat = self.hamiltonian()
         evals = sp.linalg.eigh(
-            hamiltonian_mat, eigvals_only=True, eigvals=(0, evals_count - 1)
+            hamiltonian_mat, eigvals_only=True, subset_by_index=(0, evals_count - 1)
         )
         return np.sort(evals)
 
     def _esys_calc(self, evals_count: int) -> Tuple[ndarray, ndarray]:
         hamiltonian_mat = self.hamiltonian()
         evals, evecs = sp.linalg.eigh(
-            hamiltonian_mat, eigvals_only=False, eigvals=(0, evals_count - 1)
+            hamiltonian_mat, eigvals_only=False, subset_by_index=(0, evals_count - 1)
         )
         evals, evecs = order_eigensystem(evals, evecs)
         return evals, evecs
 
     @overload
     def eigenvals(
         self,
@@ -361,14 +363,91 @@
             specdata = SpectrumData(
                 energy_table=evals, system_params=self.get_initdata(), state_table=evecs
             )
         if filename:
             specdata.filewrite(filename)
         return specdata if return_spectrumdata else (evals, evecs)
 
+    def process_op(
+        self,
+        native_op: Union[ndarray, csc_matrix],
+        energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False,
+    ) -> Union[ndarray, csc_matrix]:
+        """Processes the operator `native_op`: either hand back `native_op` unchanged, or transform it into the
+        energy eigenbasis. (Native basis refers to the basis used internally by each qubit, e.g., charge basis in the
+        case of `Transmon`.
+
+        Parameters
+        ----------
+        native_op:
+            operator in native basis
+        energy_esys:
+            If `False` (default), returns operator in the native basis
+            If `True`, the energy eigenspectrum is computed, returns operator in the energy eigenbasis
+            if energy_esys is the energy eigenspectrum, in the form of a tuple containing two ndarrays
+            (eigenvalues and energy eigenvectors), returns operator in the energy eigenbasis,
+            and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            `native_op` either unchanged or transformed into eigenenergy basis
+        """
+        if isinstance(energy_esys, bool):
+            if not energy_esys:
+                return native_op
+            esys = self.eigensys(evals_count=self.truncated_dim)
+        else:
+            esys = energy_esys
+        evectors = esys[1][:, : self.truncated_dim]
+        return get_matrixelement_table(native_op, evectors)
+
+    def process_hamiltonian(
+        self,
+        native_hamiltonian: Union[ndarray, csc_matrix],
+        energy_esys: Union[bool, Tuple[ndarray, ndarray]] = False,
+    ) -> Union[ndarray, csc_matrix]:
+        """Return qubit Hamiltonian in chosen basis: either return unchanged (i.e., in native basis) or transform
+        into eigenenergy basis
+
+        Parameters
+        ----------
+        native_hamiltonian:
+            Hamiltonian in native basis
+        energy_esys:
+            If `False` (default), returns Hamiltonian in the native basis
+            If `True`, the energy eigenspectrum is computed, returns Hamiltonian in the energy eigenbasis
+            if energy_esys is the energy eigenspectrum, in the form of a tuple containing two ndarrays
+            (eigenvalues and energy eigenvectors), returns Hamiltonian in the energy eigenbasis,
+            and does not have to recalculate eigenspectrum.
+
+        Returns
+        -------
+            Hamiltonian, either unchanged in native basis, or transformed into eigenenergy basis
+        """
+        if isinstance(energy_esys, bool):
+            if not energy_esys:
+                return native_hamiltonian
+            esys = self.eigensys(evals_count=self.truncated_dim)
+        else:
+            esys = energy_esys
+        evals = esys[0][: self.truncated_dim]
+        if isinstance(native_hamiltonian, ndarray):
+            return np.diag(evals)
+        return dia_matrix(evals).tocsc()
+
+    def anharmonicity(self) -> float:
+        """Returns the qubit's anharmonicity, (E_2 - E_1) - (E_1 - E_0)."""
+        energies = self.eigenvals(evals_count=3)
+        return energies[2] - 2 * energies[1] + energies[0]
+
+    def E01(self) -> float:
+        """Returns the qubit's fundamental energy splitting, E_1 - E_0."""
+        energies = self.eigenvals(evals_count=2)
+        return energies[1] - energies[0]
+
     @overload
     def matrixelement_table(
         self,
         operator: str,
         evecs: ndarray = None,
         evals_count: int = 6,
         filename: str = None,
@@ -734,24 +813,28 @@
             num_cpus=num_cpus,
         )
         paramvals_count = len(param_vals)
         matelem_table = np.empty(
             shape=(paramvals_count, evals_count, evals_count), dtype=np.complex_
         )
 
+        paramval_before = getattr(self, param_name)
         assert spectrumdata.state_table is not None
         for index, paramval in enumerate(param_vals):
             evecs = spectrumdata.state_table[index]
+            setattr(self, param_name, paramval)
             matelem_table[index] = self.matrixelement_table(
                 operator, evecs=evecs, evals_count=evals_count
             )
+        setattr(self, param_name, paramval_before)
 
         spectrumdata.matrixelem_table = matelem_table
         return spectrumdata
 
+    @mpl.rc_context(matplotlib_settings)
     def plot_evals_vs_paramvals(
         self,
         param_name: str,
         param_vals: ndarray,
         evals_count: int = 6,
         subtract_ground: bool = False,
         num_cpus: Optional[int] = None,
@@ -785,14 +868,15 @@
             param_vals,
             evals_count=evals_count,
             subtract_ground=subtract_ground,
             num_cpus=num_cpus,
         )
         return plot.evals_vs_paramvals(specdata, which=range(evals_count), **kwargs)
 
+    @mpl.rc_context(matplotlib_settings)
     def plot_dispersion_vs_paramvals(
         self,
         dispersion_name: str,
         param_name: str,
         param_vals: ndarray,
         ref_param: Optional[str] = None,
         transitions: Union[Transition, TransitionsTuple] = (0, 1),
@@ -860,14 +944,15 @@
             label_list=label_list,
             xlabel=specdata.param_name,
             ylabel="energy dispersion [{}]".format(units.get_units()),
             yscale="log",
             **kwargs,
         )
 
+    @mpl.rc_context(matplotlib_settings)
     def plot_matrixelements(
         self,
         operator: str,
         evecs: ndarray = None,
         evals_count: int = 6,
         mode: str = "abs",
         show_numbers: bool = False,
@@ -913,14 +998,15 @@
         return plot.matrix(
             matrixelem_array,
             mode=mode,
             show_numbers=show_numbers,
             **kwargs,
         )
 
+    @mpl.rc_context(matplotlib_settings)
     def plot_matelem_vs_paramvals(
         self,
         operator: str,
         param_name: str,
         param_vals: ndarray,
         select_elems: Union[int, List[Tuple[int, int]]] = 4,
         mode: str = "abs",
@@ -989,15 +1075,15 @@
         -------
             self
         """
         setattr(self, attr_name, value)
         return self
 
 
-# —QubitBaseClass1d——————————————————————————————————————————————————————————————————
+# -QubitBaseClass1d------------------------------------------------------------------
 
 
 class QubitBaseClass1d(QubitBaseClass):
     """Base class for superconducting qubit objects with one degree of freedom.
     Provide general mechanisms and routines for plotting spectra, matrix elements,
     and writing data to files.
     """
@@ -1034,14 +1120,15 @@
         """
         ylabel = r"$\psi_j(\varphi)$"
         ylabel = constants.MODE_STR_DICT[mode](ylabel)
         ylabel += ",  energy [{}]".format(units.get_units())
         options = {"xlabel": r"$\varphi$", "ylabel": ylabel}
         return options
 
+    @mpl.rc_context(matplotlib_settings)
     def plot_wavefunction(
         self,
         which: Union[int, Iterable[int]] = 0,
         mode: str = "real",
         esys: Tuple[ndarray, ndarray] = None,
         phi_grid: Grid1d = None,
         scaling: float = None,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scqubits-3.1.0/scqubits/core/qubit_img/cos2phi-qubit.jpg` & `scqubits-3.1.1/scqubits/core/qubit_img/cos2phi-qubit.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/qubit_img/fixed-transmon.jpg` & `scqubits-3.1.1/scqubits/core/qubit_img/fixed-transmon.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/qubit_img/flux-qubit.jpg` & `scqubits-3.1.1/scqubits/core/qubit_img/flux-qubit.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/qubit_img/fluxonium.jpg` & `scqubits-3.1.1/scqubits/core/qubit_img/fluxonium.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/qubit_img/fullzeropi.jpg` & `scqubits-3.1.1/scqubits/core/qubit_img/fullzeropi.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/qubit_img/kerr-oscillator.jpg` & `scqubits-3.1.1/scqubits/core/qubit_img/kerr-oscillator.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/qubit_img/oscillator.jpg` & `scqubits-3.1.1/scqubits/core/qubit_img/oscillator.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/qubit_img/tunable-transmon.jpg` & `scqubits-3.1.1/scqubits/core/qubit_img/tunable-transmon.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/qubit_img/zeropi.jpg` & `scqubits-3.1.1/scqubits/core/qubit_img/zeropi.jpg`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/spec_lookup.py` & `scqubits-3.1.1/scqubits/core/spec_lookup.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #    All rights reserved.
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import itertools
+import numbers
 
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import qutip as qt
 
 from numpy import ndarray
@@ -30,16 +31,14 @@
 
 if TYPE_CHECKING:
     from typing_extensions import Protocol
 
     from scqubits import HilbertSpace
     from scqubits.core.descriptors import WatchedProperty
     from scqubits.core.param_sweep import Parameters
-    from scqubits.core.qubit_base import QuantumSystem
-    from scqubits.io_utils.fileio_qutip import QutipEigenstates
     from scqubits.utils.typedefs import QuantumSys
 
 
 class MixinCompatible(Protocol):
     _parameters: "WatchedProperty[Parameters]"
     _evals_count: "WatchedProperty[int]"
     _current_param_indices: NpIndices
@@ -52,207 +51,36 @@
         ...
 
     @property
     def hilbertspace(self) -> "HilbertSpace":
         ...
 
 
-class SpectrumLookupAdapter:
-    """Bridges earlier functionality provided by the `SpectrumLookup` class to
-    universal use of the `SpectrumLookupMixin` class (originally developed for
-    `ParameterSweep` and then extended to `HilbertSpace`)."""
-
-    def __init__(self, hilbertspace):
-        self.hilbertspace = hilbertspace
-
-    @property
-    def _out_of_sync(self):
-        return self.hilbertspace._out_of_sync
-
-    @_out_of_sync.setter
-    def _out_of_sync(self, value: bool):
-        self.hilbertspace._out_of_sync = value
-
-    @utils.DeprecationMessage(
-        "<HilbertSpace>.lookup.run is deprecated. "
-        "Use <HilbertSpace>.generate_lookup instead."
-    )
-    def run(self) -> None:
-        self.hilbertspace.generate_lookup()
-
-    @utils.check_sync_status
-    @utils.DeprecationMessage(
-        "<HilbertSpace>.lookup.dressed_index is "
-        "deprecated. Use <HilbertSpace>.dressed_index instead."
-    )
-    def dressed_index(self, bare_labels: Tuple[int, ...]) -> Union[int, None]:
-        """
-        For given bare product state return the corresponding dressed-state index.
-
-        Parameters
-        ----------
-        bare_labels:
-            bare_labels = (index, index2, ...)
-
-        Returns
-        -------
-            dressed state index closest to the specified bare state
-        """
-        return self.hilbertspace.dressed_index(bare_labels)
-
-    @utils.check_sync_status
-    @utils.DeprecationMessage(
-        "<HilbertSpace>.lookup.bare_index is "
-        "deprecated. Use <HilbertSpace>.bare_index instead."
-    )
-    def bare_index(self, dressed_index: int) -> Union[Tuple[int, ...], None]:
-        """
-        For given dressed index, look up the corresponding bare index.
-
-        Returns
-        -------
-            Bare state specification in tuple form. Example: (1,0,3) means subsystem 1
-            is in bare state 1, subsystem 2 in bare state 0, and subsystem 3 in bare
-            state 3.
-        """
-        return self.hilbertspace.bare_index(dressed_index)
-
-    @utils.check_sync_status
-    @utils.DeprecationMessage(
-        "<HilbertSpace>.lookup.dressed_eigenstates is "
-        "deprecated. Use <HilbertSpace>['evecs'] instead."
-    )
-    def dressed_eigenstates(self) -> List["QutipEigenstates"]:
-        """
-        Return the list of dressed eigenvectors
-
-        Returns
-        -------
-            dressed eigenvectors for the external parameter fixed to the value
-            indicated by the provided index
-        """
-        return self.hilbertspace["evecs"]
-
-    @utils.check_sync_status
-    @utils.DeprecationMessage(
-        "<HilbertSpace>.lookup.dressed_eigenenergies is "
-        "deprecated. Use <HilbertSpace>['evals'] instead."
-    )
-    def dressed_eigenenergies(self) -> ndarray:
-        """
-        Return the array of dressed eigenenergies
-
-
-        Returns
-        -------
-            dressed eigenenergies for the external parameter fixed to the value
-            indicated by the provided index
-        """
-        return self.hilbertspace["evals"]
-
-    @utils.check_sync_status
-    @utils.DeprecationMessage(
-        "<HilbertSpace>.lookup.energy_bare_index is "
-        "deprecated. Use "
-        "<HilbertSpace>.energy_by_bare_index instead."
-    )
-    def energy_bare_index(self, bare_tuple: Tuple[int, ...]) -> Union[float, None]:
-        """
-        Look up dressed energy most closely corresponding to the given bare-state labels
-
-        Parameters
-        ----------
-        bare_tuple:
-            bare state indices
-
-        Returns
-        -------
-            dressed energy, if lookup successful
-        """
-        return self.hilbertspace.energy_by_bare_index(bare_tuple)
-
-    @utils.check_sync_status
-    @utils.DeprecationMessage(
-        "<HilbertSpace>.lookup.energy_dressed_index is "
-        "deprecated. Use "
-        "<HilbertSpace>.energy_by_dressed_index instead."
-    )
-    def energy_dressed_index(self, dressed_index: int) -> float:
-        """
-        Look up the dressed eigenenergy belonging to the given dressed index.
-
-        Parameters
-        ----------
-        dressed_index:
-            index of dressed state of interest
-
-        Returns
-        -------
-            dressed energy
-        """
-        return self.hilbertspace.energy_by_dressed_index(dressed_index)
-
-    @utils.check_sync_status
-    @utils.DeprecationMessage(
-        "<HilbertSpace>.lookup.bare_eigenstates is deprecated. "
-        "Use <HilbertSpace>.bare_eigenstates instead."
-    )
-    def bare_eigenstates(self, subsys: "QuantumSystem") -> ndarray:
-        """
-        Return ndarray of bare eigenstates for given subsystem.
-        Eigenstates are expressed in the basis internal to the subsystem.
-        """
-        return self.hilbertspace.bare_eigenstates(subsys)
-
-    @utils.check_sync_status
-    @utils.DeprecationMessage(
-        "<HilbertSpace>.lookup.bare_eigenenergies is deprecated. "
-        "Use <HilbertSpace>.bare_eigenvals instead."
-    )
-    def bare_eigenenergies(self, subsys: "QuantumSystem") -> ndarray:
-        """
-        Return list of bare eigenenergies for given subsystem.
-
-        Parameters
-        ----------
-        subsys:
-            Hilbert space subsystem for which bare eigendata is to be looked up
-
-        Returns
-        -------
-            bare eigenenergies for the specified subsystem
-        """
-        return self.hilbertspace.bare_eigenvals(subsys)
-
-    @utils.DeprecationMessage(
-        "<HilbertSpace>.lookup.bare_productstate is deprecated. "
-        "Use <HilbertSpace>.bare_productstate instead."
-    )
-    def bare_productstate(self, bare_index: Tuple[int, ...]) -> Qobj:
-        """
-        Return the bare product state specified by `bare_index`.
-
-        Parameters
-        ----------
-        bare_index:
-
-        Returns
-        -------
-            ket in full Hilbert space
-        """
-        return self.hilbertspace.bare_productstate(bare_index)
-
-
 class SpectrumLookupMixin(MixinCompatible):
     """
     SpectrumLookupMixin is used as a mix-in class by `ParameterSweep`. It makes various
     spectrum and spectrum lookup related methods directly available at the
     `ParameterSweep` level.
     """
 
+    _inside_hilbertspace = False
+
+    def __init_subclass__(cls):
+        super().__init_subclass__()
+        if cls.__name__ == "HilbertSpace":
+            cls._inside_hilbertspace = True
+        else:
+            cls._inside_hilbertspace = False
+
+    def reset_preslicing(self):
+        if self._inside_hilbertspace:
+            self._current_param_indices = 0
+        else:
+            self._current_param_indices = slice(None, None, None)
+
     @property
     def _bare_product_states_labels(self) -> List[Tuple[int, ...]]:
         """
         Generates the list of bare-state labels in canonical order. For example,
          for a Hilbert space composed of two subsystems sys1 and sys2, each label is
          of the type (3,0) meaning sys1 is in bare eigenstate 3, sys2 in bare
          eigenstate 0. The full list then reads
@@ -325,14 +153,15 @@
         self, param_indices: Optional[NpIndices] = None
     ) -> NpIndexTuple:
         param_indices = param_indices or self._current_param_indices
         if not isinstance(param_indices, tuple):
             param_indices = (param_indices,)
         return param_indices
 
+    @utils.check_lookup_exists
     @utils.check_sync_status
     def dressed_index(
         self,
         bare_labels: Tuple[int, ...],
         param_indices: Optional[NpIndices] = None,
     ) -> Union[ndarray, int, None]:
         """
@@ -352,14 +181,15 @@
         param_indices = self.set_npindextuple(param_indices)
         try:
             lookup_position = self._bare_product_states_labels.index(bare_labels)
         except ValueError:
             return None
         return self._data["dressed_indices"][param_indices + (lookup_position,)]
 
+    @utils.check_lookup_exists
     @utils.check_sync_status
     def bare_index(
         self,
         dressed_index: int,
         param_indices: Optional[Tuple[int, ...]] = None,
     ) -> Union[Tuple[int, ...], None]:
         """
@@ -426,21 +256,22 @@
         -------
             dressed eigenenergies for the external parameters fixed to the values
             indicated by the provided indices
         """
         param_indices_tuple = self.set_npindextuple(param_indices)
         return self._data["evals"][param_indices_tuple]
 
+    @utils.check_lookup_exists
     @utils.check_sync_status
     def energy_by_bare_index(
         self,
         bare_tuple: Tuple[int, ...],
         subtract_ground: bool = False,
         param_indices: Optional[NpIndices] = None,
-    ) -> NamedSlotsNdarray:  # the return value may also be np.nan
+    ) -> Union[float, NamedSlotsNdarray]:  # the return value may also be np.nan
         """
         Look up dressed energy most closely corresponding to the given bare-state labels
 
         Parameters
         ----------
         bare_tuple:
             bare state indices
@@ -454,22 +285,22 @@
             dressed energies, if lookup successful, otherwise nan;
         """
         param_indices = self.set_npindextuple(param_indices)
         dressed_index = self.dressed_index(bare_tuple, param_indices)
 
         if dressed_index is None:
             return np.nan  # type:ignore
-        if isinstance(dressed_index, int):
+        if isinstance(dressed_index, numbers.Number):
             energy = self["evals"][param_indices + (dressed_index,)]
             if subtract_ground:
                 energy -= self["evals"][param_indices + (0,)]
             return energy
 
         dressed_index = np.asarray(dressed_index)
-        energies = np.empty_like(dressed_index)
+        energies = np.empty_like(dressed_index, dtype=np.float_)
         it = np.nditer(dressed_index, flags=["multi_index", "refs_ok"])
         sliced_energies = self["evals"][param_indices]
 
         for location in it:
             location = location.tolist()
             if location is None:
                 energies[it.multi_index] = np.nan
@@ -477,21 +308,22 @@
                 energies[it.multi_index] = sliced_energies[it.multi_index][location]
                 if subtract_ground:
                     energies[it.multi_index] -= sliced_energies[it.multi_index][0]
         return NamedSlotsNdarray(
             energies, sliced_energies._parameters.paramvals_by_name
         )
 
+    @utils.check_lookup_exists
     @utils.check_sync_status
     def energy_by_dressed_index(
         self,
         dressed_index: int,
         subtract_ground: bool = False,
         param_indices: Optional[Tuple[int, ...]] = None,
-    ) -> float:
+    ) -> Union[float, NamedSlotsNdarray]:
         """
         Look up the dressed eigenenergy belonging to the given dressed index,
         usually to be used with pre-slicing
 
         Parameters
         ----------
         dressed_index:
@@ -507,30 +339,32 @@
         """
         param_indices_tuple = self.set_npindextuple(param_indices)
         energies = self["evals"][param_indices_tuple + (dressed_index,)]
         if subtract_ground:
             energies -= self["evals"][param_indices_tuple + (0,)]
         return energies
 
+    @utils.check_lookup_exists
     @utils.check_sync_status
     def bare_eigenstates(
         self,
         subsys: "QuantumSys",
         param_indices: Optional[Tuple[int, ...]] = None,
     ) -> NamedSlotsNdarray:
         """
         Return ndarray of bare eigenstates for given subsystems and parameter index.
         Eigenstates are expressed in the basis internal to the subsystems. Usually to be
-        with pre-slicing.
+        used with pre-slicing when part of `ParameterSweep`.
         """
         param_indices_tuple = self.set_npindextuple(param_indices)
         subsys_index = self.hilbertspace.get_subsys_index(subsys)
-        self._current_param_indices = slice(None, None, None)
+        self.reset_preslicing()
         return self["bare_evecs"][subsys_index][param_indices_tuple]
 
+    @utils.check_lookup_exists
     @utils.check_sync_status
     def bare_eigenvals(
         self,
         subsys: "QuantumSys",
         param_indices: Optional[Tuple[int, ...]] = None,
     ) -> NamedSlotsNdarray:
         """
@@ -547,15 +381,15 @@
         Returns
         -------
             bare eigenenergies for the specified subsystem and the external parameter
             fixed to the value indicated by its index
         """
         param_indices_tuple = self.set_npindextuple(param_indices)
         subsys_index = self.hilbertspace.get_subsys_index(subsys)
-        self._current_param_indices = slice(None, None, None)
+        self.reset_preslicing()
         return self["bare_evals"][subsys_index][param_indices_tuple]
 
     def bare_productstate(
         self,
         bare_index: Tuple[int, ...],
     ) -> Qobj:
         """
```

### Comparing `scqubits-3.1.0/scqubits/core/storage.py` & `scqubits-3.1.1/scqubits/core/storage.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from scqubits.io_utils.fileio_qutip import QutipEigenstates
 
 if TYPE_CHECKING:
     from scqubits.core.discretization import GridSpec
 
 
-# —WaveFunction class———————————————————————————————————————————————————————————————————
+# -WaveFunction class-------------------------------------------------------------------
 
 
 class WaveFunction:
     """Container for wave function amplitudes defined for a specific basis.
     Optionally,  a corresponding energy is saved as well.
 
     Parameters
@@ -70,15 +70,15 @@
         energy_range = np.max(potential_vals) - np.min(potential_vals)
         amplitude_range = np.max(self.amplitudes) - np.min(self.amplitudes)
         if amplitude_range < 1.0e-10:
             return 0.0
         self.amplitudes *= FILL_FACTOR * energy_range / amplitude_range
 
 
-# —WaveFunctionOnGrid class—————————————————————————————————————————————————————————————
+# -WaveFunctionOnGrid class-------------------------------------------------------------
 
 
 class WaveFunctionOnGrid:
     """Container for wave function amplitudes defined on a coordinate grid (arbitrary
     dimensions). Optionally, a corresponding eigenenergy is saved as well.
 
     Parameters
@@ -95,15 +95,15 @@
         self, gridspec: "GridSpec", amplitudes: np.ndarray, energy: float = None
     ) -> None:
         self.gridspec = gridspec
         self.amplitudes = amplitudes
         self.energy = energy
 
 
-# —BaseData class———————————————————————————————————————————————————————————————————————
+# -BaseData class-----------------------------------------------------------------------
 
 
 class DataStore(serializers.Serializable):
     """Base class for storing and processing spectral data and custom data from
     parameter sweeps.
 
     Parameters
@@ -156,15 +156,15 @@
             setattr(self, dataname, data)
             self._datanames.append(dataname)
             self._init_params.append(
                 dataname
             )  # register additional dataset for file IO
 
 
-# —SpectrumData class———————————————————————————————————————————————————————————————————
+# -SpectrumData class-------------------------------------------------------------------
 
 
 class SpectrumData(DataStore):
     """Container holding energy and state data as a function of a particular parameter
     that is varied. Also stores all other system parameters used for generating the
     set, and provides method for writing data to file.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scqubits-3.1.0/scqubits/core/sweeps.py` & `scqubits-3.1.1/scqubits/core/sweeps.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/core/symbolic_circuit.py` & `scqubits-3.1.1/scqubits/core/symbolic_circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,14 @@
             orthogonal_evecs[:, degenerate_set] = self._gram_schmidt(
                 evecs[:, degenerate_set].T, metric=cap_matrix
             )
 
         return orthogonal_evecs
 
     def purely_harmonic_transformation(self) -> Tuple[ndarray, ndarray]:
-
         trans_mat, _ = self.variable_transformation_matrix()
         c_mat = (
             trans_mat.T @ self._capacitance_matrix(substitute_params=True) @ trans_mat
         )
         l_mat = (
             trans_mat.T @ self._inductance_matrix(substitute_params=True) @ trans_mat
         )
@@ -575,20 +574,18 @@
             node_index_list.remove(0)
         return ground_node, [Node(idx, 0) for idx in node_index_list]
 
     @staticmethod
     def _parse_branches(
         branches_list, nodes: List[Node], ground_node: Optional[Node]
     ) -> Tuple[List[Branch], Dict[Union[Any, Symbol], Union[Any, float]]]:
-
         branches = []
         branch_var_dict = {}  # dict stores init values of all vars from input string
 
         for branch_list_input in branches_list:
-
             branch_type = branch_list_input[0]
             node_id1, node_id2 = branch_list_input[1], branch_list_input[2]
 
             if (branch_type == "JJ" or branch_type == "JJ2") and len(
                 branch_list_input
             ) != 5:
                 raise Exception(
```

### Comparing `scqubits-3.1.0/scqubits/core/units.py` & `scqubits-3.1.1/scqubits/core/units.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/explorer/explorer_panels.py` & `scqubits-3.1.1/scqubits/explorer/explorer_panels.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,32 +8,36 @@
 #
 #    This source code is licensed under the BSD-style license found in the
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 from typing import TYPE_CHECKING, List, Tuple, Union
 
+# import matplotlib as mlp
 import numpy as np
 
+from matplotlib import rc_context
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 
 import scqubits.core.units as units
 import scqubits.utils.plotting as plot
 
 from scqubits import SpectrumData, settings
 from scqubits.core.namedslots_array import NamedSlotsNdarray
 from scqubits.core.oscillator import Oscillator
+from scqubits.settings import matplotlib_settings
 from scqubits.utils.misc import tuple_to_short_str
 
 if TYPE_CHECKING:
     from scqubits.core.param_sweep import ParameterSlice, ParameterSweep
     from scqubits.core.qubit_base import QuantumSystem, QubitBaseClass, QubitBaseClass1d
 
 
+@rc_context(matplotlib_settings)
 def display_bare_spectrum(
     sweep: "ParameterSweep",
     subsys: Union["QubitBaseClass", "Oscillator"],
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
     evals_count: int = None,
     subtract_ground: bool = False,
@@ -51,14 +55,15 @@
         title=title,
         ylabel="energy [{}]".format(units.get_units()),
         fig_ax=fig_ax,
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
 
 
+@rc_context(matplotlib_settings)
 def display_anharmonicity(
     sweep: "ParameterSweep",
     subsys: "QubitBaseClass",
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
 ) -> None:
     subsys_index = sweep.get_subsys_index(subsys)
@@ -71,14 +76,15 @@
         title=title,
         ylabel="anharmonicity [{}]".format(units.get_units()),
         fig_ax=fig_ax,
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
 
 
+@rc_context(matplotlib_settings)
 def display_matrixelements(
     sweep: "ParameterSweep",
     operator_name: str,
     subsys: "QubitBaseClass",
     param_slice: "ParameterSlice",
     mode_str: str,
     fig_ax: Tuple[Figure, Axes],
@@ -99,14 +105,15 @@
         show_numbers=True,
         show_colorbar=False,
         fig_ax=fig_ax,
         title=title,
     )
 
 
+@rc_context(matplotlib_settings)
 def display_matrixelement_sweep(
     sweep: "ParameterSweep",
     operator_name: str,
     subsys: "QubitBaseClass",
     param_slice: "ParameterSlice",
     mode_str: str,
     fig_ax: Tuple[Figure, Axes],
@@ -145,14 +152,15 @@
     title = "{}: {}".format(subsys.id_str, operator_name)
     fig, axes = plot.matelem_vs_paramvals(
         specdata, mode=mode_str, fig_ax=fig_ax, title=title
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
 
 
+@rc_context(matplotlib_settings)
 def display_bare_wavefunctions(
     sweep: "ParameterSweep",
     subsys: "QubitBaseClass",
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
 ) -> None:
     subsys_index = sweep.get_subsys_index(subsys)
@@ -166,14 +174,15 @@
 
     title = "wavefunctions: {}".format(subsys.id_str)
     __ = subsys.plot_wavefunction(
         which=-1, esys=(evals, evecs), title=title, fig_ax=fig_ax
     )
 
 
+@rc_context(matplotlib_settings)
 def display_transitions(
     sweep: "ParameterSweep",
     photon_number: int,
     subsys_list: List["QuantumSystem"],
     initial: Union[int, Tuple[int, ...]],
     sidebands: bool,
     param_slice: "ParameterSlice",
@@ -191,27 +200,28 @@
         title=title,
         sidebands=sidebands,
         fig_ax=fig_ax,
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
 
 
+@rc_context(matplotlib_settings)
 def display_cross_kerr(
     sweep: "ParameterSweep",
     subsys1: "QuantumSystem",
     subsys2: "QuantumSystem",
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
 ) -> None:
     subsys1_index = sweep.get_subsys_index(subsys1)
     subsys2_index = sweep.get_subsys_index(subsys2)
     type_list = [type(sys) for sys in [subsys1, subsys2]]
     if type_list.count(Oscillator) == 1:
         title = f"ac Stark: {subsys1.id_str} + {subsys2.id_str}"
-        ylabel = f"ac Stark shift $\chi^{{{subsys1_index},{subsys2_index}}}$"
+        ylabel = rf"ac Stark shift $\chi^{{{subsys1_index},{subsys2_index}}}$"
         levels_list = [1]
         kerr_data = sweep["chi"][subsys1_index, subsys2_index]
         if param_slice.fixed != tuple():
             kerr_data = kerr_data[param_slice.fixed]
         label_list = []
         kerr_datasets = [kerr_data[..., level] for level in levels_list]
     elif type_list.count(Oscillator) == 2:
@@ -246,14 +256,15 @@
         label_list=label_list if label_list else None,
         ylabel=ylabel + "[{}]".format(units.get_units()),
         fig_ax=fig_ax,
     )
     axes.axvline(param_slice.param_val, color="gray", linestyle=":")
 
 
+@rc_context(matplotlib_settings)
 def display_self_kerr(
     sweep: "ParameterSweep",
     subsys: "QuantumSystem",
     param_slice: "ParameterSlice",
     fig_ax: Tuple[Figure, Axes],
 ) -> None:
     subsys_index = sweep.get_subsys_index(subsys)
```

### Comparing `scqubits-3.1.0/scqubits/io_utils/fileio.py` & `scqubits-3.1.1/scqubits/io_utils/fileio.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/io_utils/fileio_backends.py` & `scqubits-3.1.1/scqubits/io_utils/fileio_backends.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/io_utils/fileio_qutip.py` & `scqubits-3.1.1/scqubits/io_utils/fileio_qutip.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/io_utils/fileio_serializers.py` & `scqubits-3.1.1/scqubits/io_utils/fileio_serializers.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/settings.py` & `scqubits-3.1.1/scqubits/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -89,40 +89,49 @@
 
 # Select multiprocessing library
 # Options:  'multiprocessing'
 #           'pathos'
 MULTIPROC = "pathos"
 
 # Matplotlib options -------------------------------------------------------------------
-# set custom matplotlib color cycle
-mpl.rcParams["axes.prop_cycle"] = cycler(
-    color=[
-        "#016E82",
-        "#333795",
-        "#2E5EAC",
-        "#4498D3",
-        "#CD85B9",
-        "#45C3D1",
-        "#AA1D3F",
-        "#F47752",
-        "#19B35A",
-        "#EDE83B",
-        "#ABD379",
-        "#F9E6BE",
-    ]
-)
-
-# set matplotlib defaults
-mpl.rcParams["font.family"] = "sans-serif"
-mpl.rcParams["font.sans-serif"] = "Roboto, Arial, Helvetica, DejaVu Sans"
-mpl.rcParams["font.size"] = 11
-mpl.rcParams["axes.labelsize"] = 11
-mpl.rcParams["axes.titlesize"] = 11
-mpl.rcParams["xtick.labelsize"] = 10
-mpl.rcParams["ytick.labelsize"] = 10
+# set matplotlib defaults for use in @mpl.rc_context
+off_black = "0.2"
+matplotlib_settings = {
+    "axes.prop_cycle": cycler(
+        color=[
+            "#016E82",
+            "#333795",
+            "#2E5EAC",
+            "#4498D3",
+            "#CD85B9",
+            "#45C3D1",
+            "#AA1D3F",
+            "#F47752",
+            "#19B35A",
+            "#EDE83B",
+            "#ABD379",
+            "#F9E6BE",
+        ]
+    ),
+    "font.family": "IBM Plex Sans, Roboto, Arial, Helvetica, DejaVu Sans",
+    "font.size": 11,
+    "font.weight": 500,
+    "axes.labelsize": 11,
+    "axes.titlesize": 11,
+    "xtick.labelsize": 10,
+    "ytick.labelsize": 10,
+    "xtick.labelcolor": off_black,
+    "ytick.labelcolor": off_black,
+    "xtick.color": off_black,
+    "ytick.color": off_black,
+    "axes.labelcolor": off_black,
+    "axes.edgecolor": off_black,
+    "axes.titlecolor": off_black
+}
+
 
 # toggle top and right axes on and off
 DESPINE = True
 
 # This is a setting for number of points in stencil to approximate derivatives
 STENCIL = 7
```

### Comparing `scqubits-3.1.0/scqubits/testing.py` & `scqubits-3.1.1/scqubits/testing.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/conftest.py` & `scqubits-3.1.1/scqubits/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/data/.fullzeropi_1.hdf5` & `scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_1.hdf5`

 * *Files 12% similar despite different names*

#### h5dump {}

```diff
@@ -1,177 +1,155 @@
-HDF5 "/tmp/diffoscope_t77nf7_l_/tmp7aiew04k_TarContainer/0/61.hdf5" {
+HDF5 "/tmp/diffoscope_t77nf7_l_/tmp8yvfas64_TarContainer/0/64.hdf5" {
 GROUP "/" {
    ATTRIBUTE "__type" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
       }
       DATASPACE  SCALAR
       DATA {
       (0): "SpectrumData"
       }
    }
+   GROUP "__data" {
+      DATASET "6345245502074420277" {
+         DATATYPE  H5T_IEEE_F64LE
+         DATASPACE  SIMPLE { ( 7 ) / ( 7 ) }
+         DATA {
+         (0): 13.9831, 14.8111, 15.6396, 16.4708, 17.3101, 18.1662, 19.0145
+         }
+      }
+   }
    GROUP "__dicts" {
       GROUP "system_params" {
          ATTRIBUTE "EC" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.001
+            (0): 0.04
             }
          }
          ATTRIBUTE "ECJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.49375
+            (0): 2.2
             }
          }
          ATTRIBUTE "EJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.253165
+            (0): 15
             }
          }
          ATTRIBUTE "EL" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.001
+            (0): 1.2
             }
          }
          ATTRIBUTE "__type" {
             DATATYPE  H5T_STRING {
                STRSIZE H5T_VARIABLE;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_UTF8;
                CTYPE H5T_C_S1;
             }
             DATASPACE  SCALAR
             DATA {
             (0): "dict"
             }
          }
-         ATTRIBUTE "dC" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0.08
-            }
-         }
          ATTRIBUTE "dCJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.05
+            (0): 0.2
             }
          }
          ATTRIBUTE "dEJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.05
+            (0): 0.3
             }
          }
-         ATTRIBUTE "dEL" {
+         ATTRIBUTE "dL" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.05
+            (0): 0.1
             }
          }
          ATTRIBUTE "flux" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
             (0): 0.2
             }
          }
+         ATTRIBUTE "id_str" {
+            DATATYPE  H5T_STRING {
+               STRSIZE H5T_VARIABLE;
+               STRPAD H5T_STR_NULLTERM;
+               CSET H5T_CSET_UTF8;
+               CTYPE H5T_C_S1;
+            }
+            DATASPACE  SCALAR
+            DATA {
+            (0): "Cos2PhiQubit_1"
+            }
+         }
          ATTRIBUTE "ncut" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
-            (0): 30
+            (0): 7
             }
          }
          ATTRIBUTE "ng" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
             (0): 0.3
             }
          }
-         ATTRIBUTE "zeropi_cutoff" {
+         ATTRIBUTE "phi_cut" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
-            (0): 10
+            (0): 7
             }
          }
-         ATTRIBUTE "zeta_cutoff" {
+         ATTRIBUTE "truncated_dim" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
-            (0): 40
+            (0): 6
             }
          }
-         GROUP "__objects" {
-            GROUP "grid" {
-               ATTRIBUTE "__type" {
-                  DATATYPE  H5T_STRING {
-                     STRSIZE H5T_VARIABLE;
-                     STRPAD H5T_STR_NULLTERM;
-                     CSET H5T_CSET_UTF8;
-                     CTYPE H5T_C_S1;
-                  }
-                  DATASPACE  SCALAR
-                  DATA {
-                  (0): "Grid1d"
-                  }
-               }
-               ATTRIBUTE "max_val" {
-                  DATATYPE  H5T_IEEE_F64LE
-                  DATASPACE  SCALAR
-                  DATA {
-                  (0): 25.1327
-                  }
-               }
-               ATTRIBUTE "min_val" {
-                  DATATYPE  H5T_IEEE_F64LE
-                  DATASPACE  SCALAR
-                  DATA {
-                  (0): -25.1327
-                  }
-               }
-               ATTRIBUTE "pt_count" {
-                  DATATYPE  H5T_STD_I32LE
-                  DATASPACE  SCALAR
-                  DATA {
-                  (0): 360
-                  }
-               }
-               GROUP "__objects" {
-               }
+         ATTRIBUTE "zeta_cut" {
+            DATATYPE  H5T_STD_I32LE
+            DATASPACE  SCALAR
+            DATA {
+            (0): 30
             }
          }
+         GROUP "__objects" {
+         }
       }
    }
    GROUP "__objects" {
    }
    DATASET "energy_table" {
-      DATATYPE  H5T_IEEE_F64LE
-      DATASPACE  SIMPLE { ( 40 ) / ( 40 ) }
+      DATATYPE  H5T_STD_I64LE
+      DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
       DATA {
-      (0): 0.427623, 0.428401, 0.430448, 0.431226, 0.433274, 0.434052,
-      (6): 0.436099, 0.436877, 0.438925, 0.439702, 0.44175, 0.442527,
-      (12): 0.444576, 0.445352, 0.447401, 0.448177, 0.450226, 0.451002,
-      (18): 0.453052, 0.453827, 0.455877, 0.456052, 0.456652, 0.456712,
-      (24): 0.458703, 0.458879, 0.459477, 0.459537, 0.461528, 0.461705,
-      (30): 0.462303, 0.462362, 0.464354, 0.464531, 0.465128, 0.465187,
-      (36): 0.467179, 0.467357, 0.467953, 0.468012
+      (0): 6345245502074420277
       }
    }
 }
 }
```

### Comparing `scqubits-3.1.0/scqubits/tests/data/cos2phiqubit_1.hdf5` & `scqubits-3.1.1/scqubits/tests/data/fluxqubit_1.hdf5`

 * *Files 9% similar despite different names*

#### h5dump {}

```diff
@@ -1,8 +1,8 @@
-HDF5 "/tmp/diffoscope_t77nf7_l_/tmp7aiew04k_TarContainer/0/65.hdf5" {
+HDF5 "/tmp/diffoscope_t77nf7_l_/tmp8yvfas64_TarContainer/0/72.hdf5" {
 GROUP "/" {
    ATTRIBUTE "__type" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
@@ -10,119 +10,119 @@
       DATASPACE  SCALAR
       DATA {
       (0): "SpectrumData"
       }
    }
    GROUP "__dicts" {
       GROUP "system_params" {
-         ATTRIBUTE "EC" {
+         ATTRIBUTE "ECJ1" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.04
+            (0): 0.0166667
             }
          }
-         ATTRIBUTE "ECJ" {
+         ATTRIBUTE "ECJ2" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 2.2
+            (0): 0.0166667
             }
          }
-         ATTRIBUTE "EJ" {
+         ATTRIBUTE "ECJ3" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 15
+            (0): 0.0208333
             }
          }
-         ATTRIBUTE "EL" {
+         ATTRIBUTE "ECg1" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 1.2
+            (0): 0.833333
             }
          }
-         ATTRIBUTE "__type" {
-            DATATYPE  H5T_STRING {
-               STRSIZE H5T_VARIABLE;
-               STRPAD H5T_STR_NULLTERM;
-               CSET H5T_CSET_UTF8;
-               CTYPE H5T_C_S1;
-            }
+         ATTRIBUTE "ECg2" {
+            DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): "dict"
+            (0): 0.833333
             }
          }
-         ATTRIBUTE "dCJ" {
+         ATTRIBUTE "EJ1" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.2
+            (0): 1
             }
          }
-         ATTRIBUTE "dEJ" {
+         ATTRIBUTE "EJ2" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.3
+            (0): 1
             }
          }
-         ATTRIBUTE "dL" {
+         ATTRIBUTE "EJ3" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.1
+            (0): 0.8
             }
          }
-         ATTRIBUTE "flux" {
-            DATATYPE  H5T_IEEE_F64LE
+         ATTRIBUTE "__type" {
+            DATATYPE  H5T_STRING {
+               STRSIZE H5T_VARIABLE;
+               STRPAD H5T_STR_NULLTERM;
+               CSET H5T_CSET_UTF8;
+               CTYPE H5T_C_S1;
+            }
             DATASPACE  SCALAR
             DATA {
-            (0): 0.2
+            (0): "dict"
             }
          }
-         ATTRIBUTE "ncut" {
-            DATATYPE  H5T_STD_I64LE
+         ATTRIBUTE "flux" {
+            DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 7
+            (0): 0.1
             }
          }
-         ATTRIBUTE "ng" {
-            DATATYPE  H5T_IEEE_F64LE
+         ATTRIBUTE "ncut" {
+            DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.3
+            (0): 10
             }
          }
-         ATTRIBUTE "phi_cut" {
-            DATATYPE  H5T_STD_I64LE
+         ATTRIBUTE "ng1" {
+            DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 7
+            (0): 0
             }
          }
-         ATTRIBUTE "zeta_cut" {
-            DATATYPE  H5T_STD_I64LE
+         ATTRIBUTE "ng2" {
+            DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 30
+            (0): 0
             }
          }
          GROUP "__objects" {
          }
       }
    }
    GROUP "__objects" {
    }
    DATASET "energy_table" {
       DATATYPE  H5T_IEEE_F64LE
       DATASPACE  SIMPLE { ( 12 ) / ( 12 ) }
       DATA {
-      (0): 14.5259, 15.347, 16.1685, 16.9924, 17.8241, 18.6728, 19.5189,
-      (7): 19.5568, 20.3478, 20.4826, 21.1893, 21.4523
+      (0): -2.38684, -2.04051, -2.0405, -1.70734, -1.70093, -1.69995,
+      (6): -1.38196, -1.38011, -1.36682, -1.3668, -1.06965, -1.06334
       }
    }
 }
 }
```

### Comparing `scqubits-3.1.0/scqubits/tests/data/cos2phiqubit_5.hdf5` & `scqubits-3.1.1/scqubits/tests/data/fluxonium_5.hdf5`

 * *Files 12% similar despite different names*

#### h5dump {}

```diff
@@ -1,529 +1,486 @@
-HDF5 "/tmp/diffoscope_t77nf7_l_/tmp7aiew04k_TarContainer/0/68.hdf5" {
+HDF5 "/tmp/diffoscope_t77nf7_l_/tmp8yvfas64_TarContainer/0/71.hdf5" {
 GROUP "/" {
    ATTRIBUTE "__type" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
       }
       DATASPACE  SCALAR
       DATA {
-      (0): "DataStore"
+      (0): "SpectrumData"
       }
    }
    GROUP "__dicts" {
       GROUP "system_params" {
          ATTRIBUTE "EC" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.04
-            }
-         }
-         ATTRIBUTE "ECJ" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 2.2
+            (0): 2.5
             }
          }
          ATTRIBUTE "EJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 15
+            (0): 8.9
             }
          }
          ATTRIBUTE "EL" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 1.2
+            (0): 0.5
             }
          }
          ATTRIBUTE "__type" {
             DATATYPE  H5T_STRING {
                STRSIZE H5T_VARIABLE;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_UTF8;
                CTYPE H5T_C_S1;
             }
             DATASPACE  SCALAR
             DATA {
             (0): "dict"
             }
          }
-         ATTRIBUTE "dCJ" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0.2
-            }
-         }
-         ATTRIBUTE "dEJ" {
-            DATATYPE  H5T_IEEE_F64LE
+         ATTRIBUTE "cutoff" {
+            DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.3
-            }
-         }
-         ATTRIBUTE "dL" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0.1
+            (0): 110
             }
          }
          ATTRIBUTE "flux" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.2
-            }
-         }
-         ATTRIBUTE "ncut" {
-            DATATYPE  H5T_STD_I64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 7
-            }
-         }
-         ATTRIBUTE "ng" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0.3
-            }
-         }
-         ATTRIBUTE "phi_cut" {
-            DATATYPE  H5T_STD_I64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 7
-            }
-         }
-         ATTRIBUTE "zeta_cut" {
-            DATATYPE  H5T_STD_I64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 30
+            (0): 0.33
             }
          }
          GROUP "__objects" {
          }
       }
    }
    GROUP "__objects" {
    }
+   DATASET "energy_table" {
+      DATATYPE  H5T_IEEE_F64LE
+      DATASPACE  SIMPLE { ( 0 ) / ( 0 ) }
+      DATA {
+      }
+   }
    DATASET "matrixelem_table" {
       DATATYPE  H5T_COMPOUND {
          H5T_IEEE_F64LE "r";
          H5T_IEEE_F64LE "i";
       }
       DATASPACE  SIMPLE { ( 10, 10 ) / ( 10, 10 ) }
       DATA {
       (0,0): {
-            0.299945,
-            -1.75505e-18
+            0,
+            4.16334e-17
          },
       (0,1): {
-            0.495924,
-            1.02393
+            0,
+            -0.0566262
          },
       (0,2): {
-            -0.000270602,
-            0.000632764
+            0,
+            -0.456401
          },
       (0,3): {
-            4.13671e-05,
-            -0.000230681
+            0,
+            -0.183446
          },
       (0,4): {
-            5.80153e-05,
-            -1.09611e-05
+            0,
+            0.110036
          },
       (0,5): {
-            2.39986e-05,
-            1.94382e-05
+            0,
+            -0.0277945
          },
       (0,6): {
-            -2.03071e-06,
-            -5.13124e-06
+            0,
+            0.0580859
          },
       (0,7): {
-            -6.89378e-06,
-            -1.44688e-05
+            0,
+            0.049891
          },
       (0,8): {
-            4.99648e-05,
-            -6.95132e-05
+            0,
+            0.00730155
          },
       (0,9): {
-            2.47793e-05,
-            4.02316e-05
+            0,
+            -0.034428
          },
       (1,0): {
-            0.495924,
-            -1.02393
+            0,
+            0.0566262
          },
       (1,1): {
-            0.299203,
-            2.13452e-19
+            0,
+            -6.93889e-18
          },
       (1,2): {
-            -0.945126,
-            1.30111
+            0,
+            0.26432
          },
       (1,3): {
-            -0.00170171,
-            0.000260477
+            0,
+            -0.365142
          },
       (1,4): {
-            0.000189731,
-            -0.00113287
+            0,
+            0.154441
          },
       (1,5): {
-            0.000280423,
-            -0.000114152
+            0,
+            0.16172
          },
       (1,6): {
-            3.18986e-05,
-            1.70197e-05
+            0,
+            -0.00731812
          },
       (1,7): {
-            0.000149026,
-            1.2608e-05
+            0,
+            -0.0626743
          },
       (1,8): {
-            -5.51986e-05,
-            8.8962e-05
+            0,
+            -0.0212585
          },
       (1,9): {
-            8.73131e-05,
-            1.2158e-05
+            0,
+            0.054007
          },
       (2,0): {
-            -0.000270602,
-            -0.000632764
+            0,
+            0.456401
          },
       (2,1): {
-            -0.945126,
-            -1.30111
+            0,
+            -0.26432
          },
       (2,2): {
-            0.294498,
-            1.09437e-17
+            0,
+            -8.32667e-17
          },
       (2,3): {
-            -0.00909007,
-            1.9658
+            0,
+            0.40328
          },
       (2,4): {
-            -0.00392964,
-            0.00396949
+            0,
+            -0.0425159
          },
       (2,5): {
-            -0.00366588,
-            -0.00202759
+            0,
+            0.232905
          },
       (2,6): {
-            0.000836216,
-            -0.000363173
+            0,
+            0.12391
          },
       (2,7): {
-            -0.000352334,
-            -0.000552635
+            0,
+            0.00776755
          },
       (2,8): {
-            -0.000335046,
-            1.13916e-05
+            0,
+            -0.20436
          },
       (2,9): {
-            0.000218647,
-            0.000386186
+            0,
+            -0.0473006
          },
       (3,0): {
-            4.13671e-05,
-            0.000230681
+            0,
+            0.183446
          },
       (3,1): {
-            -0.00170171,
-            -0.000260477
+            0,
+            0.365142
          },
       (3,2): {
-            -0.00909007,
-            -1.9658
+            0,
+            -0.40328
          },
       (3,3): {
-            0.276825,
-            -6.09864e-19
+            0,
+            5.55112e-17
          },
       (3,4): {
-            1.00344,
-            2.02199
+            0,
+            0.204656
          },
       (3,5): {
-            -0.00503971,
-            0.0144396
+            0,
+            0.485833
          },
       (3,6): {
-            -0.0020984,
-            -0.00628462
+            0,
+            -0.179446
          },
       (3,7): {
-            -0.00760276,
-            0.0060543
+            0,
+            -0.149614
          },
       (3,8): {
-            -0.00272673,
-            -0.00237572
+            0,
+            -0.000828576
          },
       (3,9): {
-            0.000774842,
-            -0.000808991
+            0,
+            -0.121081
          },
       (4,0): {
-            5.80153e-05,
-            1.09611e-05
+            0,
+            -0.110036
          },
       (4,1): {
-            0.000189731,
-            0.00113287
+            0,
+            -0.154441
          },
       (4,2): {
-            -0.00392964,
-            -0.00396949
+            0,
+            0.0425159
          },
       (4,3): {
-            1.00344,
-            -2.02199
+            0,
+            -0.204656
          },
       (4,4): {
-            0.23322,
-            -1.60597e-18
+            0,
+            -1.38778e-17
          },
       (4,5): {
-            1.41193,
-            2.05442
+            0,
+            -0.483264
          },
       (4,6): {
-            0.00588678,
-            0.00324804
+            0,
+            -0.099519
          },
       (4,7): {
-            0.00954281,
-            0.0338403
+            0,
+            -0.11526
          },
       (4,8): {
-            -0.0146649,
-            0.00830058
+            0,
+            -0.248078
          },
       (4,9): {
-            -0.00586877,
-            -0.0192341
+            0,
+            -0.120675
          },
       (5,0): {
-            2.39986e-05,
-            -1.94382e-05
+            0,
+            0.0277945
          },
       (5,1): {
-            0.000280423,
-            0.000114152
+            0,
+            -0.16172
          },
       (5,2): {
-            -0.00366588,
-            0.00202759
+            0,
+            -0.232905
          },
       (5,3): {
-            -0.00503971,
-            -0.0144396
+            0,
+            -0.485833
          },
       (5,4): {
-            1.41193,
-            -2.05442
+            0,
+            0.483264
          },
       (5,5): {
-            0.162764,
-            -6.04443e-18
+            0,
+            2.77556e-16
          },
       (5,6): {
-            -0.673817,
-            0.826174
+            0,
+            0.623424
          },
       (5,7): {
-            2.23888,
-            0.997925
+            0,
+            0.31442
          },
       (5,8): {
-            0.0340398,
-            -0.0503377
+            0,
+            -0.123908
          },
       (5,9): {
-            -0.052469,
-            -0.0214005
+            0,
+            0.014593
          },
       (6,0): {
-            -2.03071e-06,
-            5.13124e-06
+            0,
+            -0.0580859
          },
       (6,1): {
-            3.18986e-05,
-            -1.70197e-05
+            0,
+            0.00731812
          },
       (6,2): {
-            0.000836216,
-            0.000363173
+            0,
+            -0.12391
          },
       (6,3): {
-            -0.0020984,
-            0.00628462
+            0,
+            0.179446
          },
       (6,4): {
-            0.00588678,
-            -0.00324804
+            0,
+            0.099519
          },
       (6,5): {
-            -0.673817,
-            -0.826174
+            0,
+            -0.623424
          },
       (6,6): {
-            0.170686,
-            -2.1684e-19
+            0,
+            2.77556e-16
          },
       (6,7): {
-            0.0697081,
-            0.159338
+            0,
+            0.3849
          },
       (6,8): {
-            -0.670659,
-            0.238881
+            0,
+            0.351903
          },
       (6,9): {
-            0.359905,
-            1.22942
+            0,
+            0.00765457
          },
       (7,0): {
-            -6.89378e-06,
-            1.44688e-05
+            0,
+            -0.049891
          },
       (7,1): {
-            0.000149026,
-            -1.2608e-05
+            0,
+            0.0626743
          },
       (7,2): {
-            -0.000352334,
-            0.000552635
+            0,
+            -0.00776755
          },
       (7,3): {
-            -0.00760276,
-            -0.0060543
+            0,
+            0.149614
          },
       (7,4): {
-            0.00954281,
-            -0.0338403
+            0,
+            0.11526
          },
       (7,5): {
-            2.23888,
-            -0.997925
+            0,
+            -0.31442
          },
       (7,6): {
-            0.0697081,
-            -0.159338
+            0,
+            -0.3849
          },
       (7,7): {
-            0.225715,
-            -1.00289e-18
+            0,
+            -1.38778e-17
          },
       (7,8): {
-            0.400878,
-            1.1102
+            0,
+            0.645336
          },
       (7,9): {
-            -2.35764,
-            0.192433
+            0,
+            -0.080455
          },
       (8,0): {
-            4.99648e-05,
-            6.95132e-05
+            0,
+            -0.00730155
          },
       (8,1): {
-            -5.51986e-05,
-            -8.8962e-05
+            0,
+            0.0212585
          },
       (8,2): {
-            -0.000335046,
-            -1.13916e-05
+            0,
+            0.20436
          },
       (8,3): {
-            -0.00272673,
-            0.00237572
+            0,
+            0.000828576
          },
       (8,4): {
-            -0.0146649,
-            -0.00830058
+            0,
+            0.248078
          },
       (8,5): {
-            0.0340398,
-            0.0503377
+            0,
+            0.123908
          },
       (8,6): {
-            -0.670659,
-            -0.238881
+            0,
+            -0.351903
          },
       (8,7): {
-            0.400878,
-            -1.1102
+            0,
+            -0.645336
          },
       (8,8): {
-            0.155899,
-            1.84314e-18
+            0,
+            -8.32667e-17
          },
       (8,9): {
-            -0.0899714,
-            -0.331466
+            0,
+            0.884105
          },
       (9,0): {
-            2.47793e-05,
-            -4.02316e-05
+            0,
+            0.034428
          },
       (9,1): {
-            8.73131e-05,
-            -1.2158e-05
+            0,
+            -0.054007
          },
       (9,2): {
-            0.000218647,
-            -0.000386186
+            0,
+            0.0473006
          },
       (9,3): {
-            0.000774842,
-            0.000808991
+            0,
+            0.121081
          },
       (9,4): {
-            -0.00586877,
-            0.0192341
+            0,
+            0.120675
          },
       (9,5): {
-            -0.052469,
-            0.0214005
+            0,
+            -0.014593
          },
       (9,6): {
-            0.359905,
-            -1.22942
+            0,
+            -0.00765457
          },
       (9,7): {
-            -2.35764,
-            -0.192433
+            0,
+            0.080455
          },
       (9,8): {
-            -0.0899714,
-            0.331466
+            0,
+            -0.884105
          },
       (9,9): {
-            0.171804,
-            -1.18178e-17
+            0,
+            -5.55112e-17
          }
       }
    }
 }
 }
```

### Comparing `scqubits-3.1.0/scqubits/tests/data/fluxonium_1.hdf5` & `scqubits-3.1.1/scqubits/tests/data/fluxonium_1.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/data/fluxonium_2.hdf5` & `scqubits-3.1.1/scqubits/tests/data/fluxonium_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/data/fluxonium_4.hdf5` & `scqubits-3.1.1/scqubits/tests/data/fluxonium_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/data/fluxonium_5.hdf5` & `scqubits-3.1.1/scqubits/tests/data/transmon_5.hdf5`

 * *Files 20% similar despite different names*

#### h5dump {}

```diff
@@ -1,8 +1,8 @@
-HDF5 "/tmp/diffoscope_t77nf7_l_/tmp7aiew04k_TarContainer/0/72.hdf5" {
+HDF5 "/tmp/diffoscope_t77nf7_l_/tmp8yvfas64_TarContainer/0/81.hdf5" {
 GROUP "/" {
    ATTRIBUTE "__type" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
@@ -14,55 +14,48 @@
    }
    GROUP "__dicts" {
       GROUP "system_params" {
          ATTRIBUTE "EC" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 2.5
+            (0): 1.2
             }
          }
          ATTRIBUTE "EJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 8.9
-            }
-         }
-         ATTRIBUTE "EL" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0.5
+            (0): 30.02
             }
          }
          ATTRIBUTE "__type" {
             DATATYPE  H5T_STRING {
                STRSIZE H5T_VARIABLE;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_UTF8;
                CTYPE H5T_C_S1;
             }
             DATASPACE  SCALAR
             DATA {
             (0): "dict"
             }
          }
-         ATTRIBUTE "cutoff" {
+         ATTRIBUTE "ncut" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
-            (0): 110
+            (0): 31
             }
          }
-         ATTRIBUTE "flux" {
+         ATTRIBUTE "ng" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.33
+            (0): 0.3
             }
          }
          GROUP "__objects" {
          }
       }
    }
    GROUP "__objects" {
@@ -70,417 +63,34 @@
    DATASET "energy_table" {
       DATATYPE  H5T_IEEE_F64LE
       DATASPACE  SIMPLE { ( 0 ) / ( 0 ) }
       DATA {
       }
    }
    DATASET "matrixelem_table" {
-      DATATYPE  H5T_COMPOUND {
-         H5T_IEEE_F64LE "r";
-         H5T_IEEE_F64LE "i";
-      }
+      DATATYPE  H5T_IEEE_F64LE
       DATASPACE  SIMPLE { ( 10, 10 ) / ( 10, 10 ) }
       DATA {
-      (0,0): {
-            0,
-            4.16334e-17
-         },
-      (0,1): {
-            0,
-            -0.0566262
-         },
-      (0,2): {
-            0,
-            -0.456401
-         },
-      (0,3): {
-            0,
-            -0.183446
-         },
-      (0,4): {
-            0,
-            0.110036
-         },
-      (0,5): {
-            0,
-            -0.0277945
-         },
-      (0,6): {
-            0,
-            0.0580859
-         },
-      (0,7): {
-            0,
-            0.049891
-         },
-      (0,8): {
-            0,
-            0.00730155
-         },
-      (0,9): {
-            0,
-            -0.034428
-         },
-      (1,0): {
-            0,
-            0.0566262
-         },
-      (1,1): {
-            0,
-            -6.93889e-18
-         },
-      (1,2): {
-            0,
-            0.26432
-         },
-      (1,3): {
-            0,
-            -0.365142
-         },
-      (1,4): {
-            0,
-            0.154441
-         },
-      (1,5): {
-            0,
-            0.16172
-         },
-      (1,6): {
-            0,
-            -0.00731812
-         },
-      (1,7): {
-            0,
-            -0.0626743
-         },
-      (1,8): {
-            0,
-            -0.0212585
-         },
-      (1,9): {
-            0,
-            0.054007
-         },
-      (2,0): {
-            0,
-            0.456401
-         },
-      (2,1): {
-            0,
-            -0.26432
-         },
-      (2,2): {
-            0,
-            -8.32667e-17
-         },
-      (2,3): {
-            0,
-            0.40328
-         },
-      (2,4): {
-            0,
-            -0.0425159
-         },
-      (2,5): {
-            0,
-            0.232905
-         },
-      (2,6): {
-            0,
-            0.12391
-         },
-      (2,7): {
-            0,
-            0.00776755
-         },
-      (2,8): {
-            0,
-            -0.20436
-         },
-      (2,9): {
-            0,
-            -0.0473006
-         },
-      (3,0): {
-            0,
-            0.183446
-         },
-      (3,1): {
-            0,
-            0.365142
-         },
-      (3,2): {
-            0,
-            -0.40328
-         },
-      (3,3): {
-            0,
-            5.55112e-17
-         },
-      (3,4): {
-            0,
-            0.204656
-         },
-      (3,5): {
-            0,
-            0.485833
-         },
-      (3,6): {
-            0,
-            -0.179446
-         },
-      (3,7): {
-            0,
-            -0.149614
-         },
-      (3,8): {
-            0,
-            -0.000828576
-         },
-      (3,9): {
-            0,
-            -0.121081
-         },
-      (4,0): {
-            0,
-            -0.110036
-         },
-      (4,1): {
-            0,
-            -0.154441
-         },
-      (4,2): {
-            0,
-            0.0425159
-         },
-      (4,3): {
-            0,
-            -0.204656
-         },
-      (4,4): {
-            0,
-            -1.38778e-17
-         },
-      (4,5): {
-            0,
-            -0.483264
-         },
-      (4,6): {
-            0,
-            -0.099519
-         },
-      (4,7): {
-            0,
-            -0.11526
-         },
-      (4,8): {
-            0,
-            -0.248078
-         },
-      (4,9): {
-            0,
-            -0.120675
-         },
-      (5,0): {
-            0,
-            0.0277945
-         },
-      (5,1): {
-            0,
-            -0.16172
-         },
-      (5,2): {
-            0,
-            -0.232905
-         },
-      (5,3): {
-            0,
-            -0.485833
-         },
-      (5,4): {
-            0,
-            0.483264
-         },
-      (5,5): {
-            0,
-            2.77556e-16
-         },
-      (5,6): {
-            0,
-            0.623424
-         },
-      (5,7): {
-            0,
-            0.31442
-         },
-      (5,8): {
-            0,
-            -0.123908
-         },
-      (5,9): {
-            0,
-            0.014593
-         },
-      (6,0): {
-            0,
-            -0.0580859
-         },
-      (6,1): {
-            0,
-            0.00731812
-         },
-      (6,2): {
-            0,
-            -0.12391
-         },
-      (6,3): {
-            0,
-            0.179446
-         },
-      (6,4): {
-            0,
-            0.099519
-         },
-      (6,5): {
-            0,
-            -0.623424
-         },
-      (6,6): {
-            0,
-            2.77556e-16
-         },
-      (6,7): {
-            0,
-            0.3849
-         },
-      (6,8): {
-            0,
-            0.351903
-         },
-      (6,9): {
-            0,
-            0.00765457
-         },
-      (7,0): {
-            0,
-            -0.049891
-         },
-      (7,1): {
-            0,
-            0.0626743
-         },
-      (7,2): {
-            0,
-            -0.00776755
-         },
-      (7,3): {
-            0,
-            0.149614
-         },
-      (7,4): {
-            0,
-            0.11526
-         },
-      (7,5): {
-            0,
-            -0.31442
-         },
-      (7,6): {
-            0,
-            -0.3849
-         },
-      (7,7): {
-            0,
-            -1.38778e-17
-         },
-      (7,8): {
-            0,
-            0.645336
-         },
-      (7,9): {
-            0,
-            -0.080455
-         },
-      (8,0): {
-            0,
-            -0.00730155
-         },
-      (8,1): {
-            0,
-            0.0212585
-         },
-      (8,2): {
-            0,
-            0.20436
-         },
-      (8,3): {
-            0,
-            0.000828576
-         },
-      (8,4): {
-            0,
-            0.248078
-         },
-      (8,5): {
-            0,
-            0.123908
-         },
-      (8,6): {
-            0,
-            -0.351903
-         },
-      (8,7): {
-            0,
-            -0.645336
-         },
-      (8,8): {
-            0,
-            -8.32667e-17
-         },
-      (8,9): {
-            0,
-            0.884105
-         },
-      (9,0): {
-            0,
-            0.034428
-         },
-      (9,1): {
-            0,
-            -0.054007
-         },
-      (9,2): {
-            0,
-            0.0473006
-         },
-      (9,3): {
-            0,
-            0.121081
-         },
-      (9,4): {
-            0,
-            0.120675
-         },
-      (9,5): {
-            0,
-            -0.014593
-         },
-      (9,6): {
-            0,
-            -0.00765457
-         },
-      (9,7): {
-            0,
-            0.080455
-         },
-      (9,8): {
-            0,
-            -0.884105
-         },
-      (9,9): {
-            0,
-            -5.55112e-17
-         }
+      (0,0): 0.299957, -0.902867, -0.00126536, -0.0503118, 0.00705431,
+      (0,5): 0.00708892, -0.00188275, 0.000692384, -0.00012552, 3.61049e-05,
+      (1,0): -0.902867, 0.301952, -1.21191, 0.0252011, 0.109441, -0.0389272,
+      (1,6): -0.0129142, -0.00468152, -0.000849522, -0.000244503,
+      (2,0): -0.00126536, -1.21191, 0.262411, -1.36957, 0.210165, 0.208837,
+      (2,6): -0.0563017, 0.020429, -0.00375389, 0.0010653,
+      (3,0): -0.0503118, 0.0252011, -1.36957, 0.627079, 1.20863, -0.534407,
+      (3,6): -0.155118, -0.0652285, -0.0102135, -0.00340713,
+      (4,0): 0.00705431, 0.109441, 0.210165, 1.20863, -1.14248, -0.763431,
+      (4,6): 0.547221, -0.0798064, 0.0368575, -0.00416354,
+      (5,0): 0.00708892, -0.0389272, 0.208837, -0.534407, -0.763431, 2.56566,
+      (5,6): 0.141344, 0.49012, 0.00935398, 0.0257687,
+      (6,0): -0.00188275, -0.0129142, -0.0563017, -0.155118, 0.547221,
+      (6,5): 0.141344, -2.83977, 0.0153919, -0.414516, 0.000803244,
+      (7,0): 0.000692384, -0.00468152, 0.020429, -0.0652285, -0.0798064,
+      (7,5): 0.49012, 0.0153919, 3.89325, 0.00101933, 0.374251,
+      (8,0): -0.00012552, -0.000849522, -0.00375389, -0.0102135, 0.0368575,
+      (8,5): 0.00935398, -0.414516, 0.00101933, -3.93477, 5.3195e-05,
+      (9,0): 3.61049e-05, -0.000244503, 0.0010653, -0.00340713, -0.00416354,
+      (9,5): 0.0257687, 0.000803244, 0.374251, 5.3195e-05, 4.95078
       }
    }
 }
 }
```

### Comparing `scqubits-3.1.0/scqubits/tests/data/fluxqubit_1.hdf5` & `scqubits-3.1.1/scqubits/tests/data/transmon_1.hdf5`

 * *Files 18% similar despite different names*

#### h5dump {}

```diff
@@ -1,8 +1,8 @@
-HDF5 "/tmp/diffoscope_t77nf7_l_/tmp7aiew04k_TarContainer/0/73.hdf5" {
+HDF5 "/tmp/diffoscope_t77nf7_l_/tmp8yvfas64_TarContainer/0/78.hdf5" {
 GROUP "/" {
    ATTRIBUTE "__type" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
@@ -10,119 +10,63 @@
       DATASPACE  SCALAR
       DATA {
       (0): "SpectrumData"
       }
    }
    GROUP "__dicts" {
       GROUP "system_params" {
-         ATTRIBUTE "ECJ1" {
+         ATTRIBUTE "EC" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.0166667
+            (0): 1.2
             }
          }
-         ATTRIBUTE "ECJ2" {
+         ATTRIBUTE "EJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.0166667
-            }
-         }
-         ATTRIBUTE "ECJ3" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0.0208333
-            }
-         }
-         ATTRIBUTE "ECg1" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0.833333
-            }
-         }
-         ATTRIBUTE "ECg2" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0.833333
-            }
-         }
-         ATTRIBUTE "EJ1" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 1
-            }
-         }
-         ATTRIBUTE "EJ2" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 1
-            }
-         }
-         ATTRIBUTE "EJ3" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0.8
+            (0): 30.02
             }
          }
          ATTRIBUTE "__type" {
             DATATYPE  H5T_STRING {
                STRSIZE H5T_VARIABLE;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_UTF8;
                CTYPE H5T_C_S1;
             }
             DATASPACE  SCALAR
             DATA {
             (0): "dict"
             }
          }
-         ATTRIBUTE "flux" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0.1
-            }
-         }
          ATTRIBUTE "ncut" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
-            (0): 10
-            }
-         }
-         ATTRIBUTE "ng1" {
-            DATATYPE  H5T_IEEE_F64LE
-            DATASPACE  SCALAR
-            DATA {
-            (0): 0
+            (0): 31
             }
          }
-         ATTRIBUTE "ng2" {
+         ATTRIBUTE "ng" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0
+            (0): 0.3
             }
          }
          GROUP "__objects" {
          }
       }
    }
    GROUP "__objects" {
    }
    DATASET "energy_table" {
       DATATYPE  H5T_IEEE_F64LE
       DATASPACE  SIMPLE { ( 12 ) / ( 12 ) }
       DATA {
-      (0): -2.38684, -2.04051, -2.0405, -1.70734, -1.70093, -1.69995,
-      (6): -1.38196, -1.38011, -1.36682, -1.3668, -1.06965, -1.06334
+      (0): -21.8438, -6.17519, 8.01367, 20.049, 30.5431, 38.7072, 54.5548,
+      (7): 67.4932, 90.0518, 107.114, 135.679, 156.682
       }
    }
 }
 }
```

### Comparing `scqubits-3.1.0/scqubits/tests/data/fluxqubit_2.hdf5` & `scqubits-3.1.1/scqubits/tests/data/fluxqubit_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/data/fluxqubit_4.hdf5` & `scqubits-3.1.1/scqubits/tests/data/fluxqubit_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/data/fluxqubit_5.hdf5` & `scqubits-3.1.1/scqubits/tests/data/fluxqubit_5.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/data/fullzeropi_1.hdf5` & `scqubits-3.1.1/scqubits/tests/data/fullzeropi_1.hdf5`

 * *Files 9% similar despite different names*

#### h5dump {}

```diff
@@ -1,21 +1,36 @@
-HDF5 "/tmp/diffoscope_t77nf7_l_/tmp7aiew04k_TarContainer/0/77.hdf5" {
+HDF5 "/tmp/diffoscope_t77nf7_l_/tmp8yvfas64_TarContainer/0/76.hdf5" {
 GROUP "/" {
    ATTRIBUTE "__type" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
       }
       DATASPACE  SCALAR
       DATA {
       (0): "SpectrumData"
       }
    }
+   GROUP "__data" {
+      DATASET "252697575698951622" {
+         DATATYPE  H5T_IEEE_F64LE
+         DATASPACE  SIMPLE { ( 40 ) / ( 40 ) }
+         DATA {
+         (0): 0.427131, 0.427927, 0.429957, 0.430752, 0.432782, 0.433577,
+         (6): 0.435608, 0.436402, 0.438433, 0.439227, 0.441259, 0.442053,
+         (12): 0.444084, 0.444878, 0.446909, 0.447703, 0.449735, 0.450528,
+         (18): 0.45256, 0.453353, 0.455386, 0.455606, 0.456178, 0.45628,
+         (24): 0.458211, 0.458432, 0.459003, 0.459105, 0.461037, 0.461258,
+         (30): 0.461828, 0.46193, 0.463862, 0.464084, 0.464653, 0.464756,
+         (36): 0.466688, 0.46691, 0.467478, 0.467581
+         }
+      }
+   }
    GROUP "__dicts" {
       GROUP "system_params" {
          ATTRIBUTE "EC" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
             (0): 0.001
@@ -85,28 +100,47 @@
          ATTRIBUTE "flux" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
             (0): 0.2
             }
          }
+         ATTRIBUTE "id_str" {
+            DATATYPE  H5T_STRING {
+               STRSIZE H5T_VARIABLE;
+               STRPAD H5T_STR_NULLTERM;
+               CSET H5T_CSET_UTF8;
+               CTYPE H5T_C_S1;
+            }
+            DATASPACE  SCALAR
+            DATA {
+            (0): "FullZeroPi_1"
+            }
+         }
          ATTRIBUTE "ncut" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
             (0): 30
             }
          }
          ATTRIBUTE "ng" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
             (0): 0.3
             }
          }
+         ATTRIBUTE "truncated_dim" {
+            DATATYPE  H5T_STD_I32LE
+            DATASPACE  SCALAR
+            DATA {
+            (0): 6
+            }
+         }
          ATTRIBUTE "zeropi_cutoff" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
             (0): 10
             }
          }
@@ -157,21 +191,15 @@
             }
          }
       }
    }
    GROUP "__objects" {
    }
    DATASET "energy_table" {
-      DATATYPE  H5T_IEEE_F64LE
-      DATASPACE  SIMPLE { ( 40 ) / ( 40 ) }
+      DATATYPE  H5T_STD_I64LE
+      DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
       DATA {
-      (0): 0.42713, 0.427926, 0.429956, 0.430751, 0.432781, 0.433576,
-      (6): 0.435607, 0.436401, 0.438432, 0.439226, 0.441258, 0.442052,
-      (12): 0.444083, 0.444877, 0.446908, 0.447702, 0.449734, 0.450527,
-      (18): 0.452559, 0.453352, 0.455385, 0.455605, 0.456177, 0.456279,
-      (24): 0.45821, 0.458431, 0.459002, 0.459104, 0.461036, 0.461257,
-      (30): 0.461827, 0.461929, 0.463861, 0.464083, 0.464652, 0.464755,
-      (36): 0.466686, 0.466909, 0.467477, 0.46758
+      (0): 252697575698951622
       }
    }
 }
 }
```

### Comparing `scqubits-3.1.0/scqubits/tests/data/fullzeropi_2.hdf5` & `scqubits-3.1.1/scqubits/tests/data/fullzeropi_2.hdf5`

 * *Files 20% similar despite different names*

#### h5dump {}

```diff
@@ -1,3235 +1,3235 @@
-HDF5 "/tmp/diffoscope_t77nf7_l_/tmp7aiew04k_TarContainer/0/78.hdf5" {
+HDF5 "/tmp/diffoscope_t77nf7_l_/tmp8yvfas64_TarContainer/0/77.hdf5" {
 GROUP "/" {
    ATTRIBUTE "__type" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
       }
       DATASPACE  SCALAR
       DATA {
       (0): "SpectrumData"
       }
    }
    GROUP "__data" {
-      DATASET "-6741523309743639754" {
+      DATASET "-5522267930686899526" {
          DATATYPE  H5T_IEEE_F64LE
          DATASPACE  SIMPLE { ( 2 ) / ( 2 ) }
          DATA {
          (0): 0.427131, 0.427927
          }
       }
-      DATASET "7040608736081761962" {
+      DATASET "2543333760430554360" {
          DATATYPE  H5T_COMPOUND {
             H5T_IEEE_F64LE "r";
             H5T_IEEE_F64LE "i";
          }
          DATASPACE  SIMPLE { ( 400, 2 ) / ( 400, 2 ) }
          DATA {
          (0,0): {
-               -0.999912,
-               -0.00556411
+               0.999904,
+               0.00681554
             },
          (0,1): {
-               -6.49191e-08,
-               -7.18029e-08
+               -8.1298e-08,
+               -5.26323e-08
             },
          (1,0): {
-               0.00198458,
-               0.0100937
+               -0.0019719,
+               -0.0100962
             },
          (1,1): {
-               4.89658e-07,
-               -7.40047e-07
+               2.81402e-07,
+               -8.42303e-07
             },
          (2,0): {
-               0.000241921,
-               -2.77531e-05
+               -0.000241955,
+               2.74496e-05
             },
          (2,1): {
-               -1.97345e-08,
-               -1.4109e-08
+               -2.27251e-08,
+               -8.55183e-09
             },
          (3,0): {
-               -9.1993e-07,
-               -3.39052e-06
+               9.1563e-07,
+               3.39166e-06
             },
          (3,1): {
-               -2.47275e-10,
-               3.29621e-10
+               -1.53169e-10,
+               3.8101e-10
             },
          (4,0): {
-               -7.40565e-08,
-               1.51034e-08
+               7.40796e-08,
+               -1.50096e-08
             },
          (4,1): {
-               3.73529e-12,
-               -1.70806e-13
+               3.52508e-12,
+               -1.1419e-12
             },
          (5,0): {
-               3.84522e-10,
-               1.18223e-09
+               -3.83027e-10,
+               -1.18281e-09
             },
          (5,1): {
-               3.58883e-13,
-               -4.24646e-13
+               2.33815e-13,
+               -4.96844e-13
             },
          (6,0): {
-               2.41766e-11,
-               -6.77164e-12
+               -2.41821e-11,
+               6.74132e-12
             },
          (6,1): {
-               -8.34768e-15,
-               -7.80485e-15
+               -1.04876e-14,
+               -6.08391e-15
             },
          (7,0): {
-               -1.52e-13,
-               -4.06545e-13
+               1.5603e-13,
+               4.0679e-13
             },
          (7,1): {
-               -2.70211e-16,
-               1.42531e-15
+               1.01392e-15,
+               3.15697e-16
             },
          (8,0): {
-               -7.84948e-15,
-               2.76677e-15
+               9.02108e-15,
+               -2.77317e-15
             },
          (8,1): {
-               -4.06438e-17,
-               8.3802e-16
+               8.49322e-16,
+               7.36362e-17
             },
          (9,0): {
-               5.12299e-18,
-               1.22851e-16
+               2.05562e-15,
+               -1.39106e-16
             },
          (9,1): {
-               2.65972e-17,
-               1.99849e-16
+               8.37716e-16,
+               -6.07239e-18
             },
          (10,0): {
-               1.05758e-16,
-               7.24131e-18
+               6.62752e-16,
+               -1.91458e-17
             },
          (10,1): {
-               2.94367e-17,
-               -2.48734e-16
+               -5.84981e-16,
+               -6.33161e-17
             },
          (11,0): {
-               1.51716e-16,
-               3.90792e-18
+               1.21595e-16,
+               2.90676e-18
             },
          (11,1): {
-               -6.27163e-18,
-               3.39729e-16
+               -2.98096e-16,
+               -7.69444e-18
             },
          (12,0): {
-               7.15224e-18,
-               1.33565e-17
+               7.79951e-18,
+               5.63382e-19
             },
          (12,1): {
-               -3.29221e-17,
-               7.81708e-16
+               2.93711e-16,
+               2.66446e-17
             },
          (13,0): {
-               -3.11989e-17,
-               1.28918e-17
+               2.17236e-17,
+               1.61829e-20
             },
          (13,1): {
-               4.30428e-17,
-               -1.89777e-16
+               -1.21504e-16,
+               1.31249e-17
             },
          (14,0): {
-               -3.34882e-16,
-               8.04293e-18
+               -1.5389e-16,
+               -2.92763e-18
             },
          (14,1): {
-               -9.6167e-18,
-               -1.59152e-15
+               -1.49178e-15,
+               -1.4702e-17
             },
          (15,0): {
-               -5.52047e-17,
-               7.27587e-18
+               -2.41296e-17,
+               -3.69752e-18
             },
          (15,1): {
-               -2.66988e-17,
-               -5.03302e-17
+               -7.81072e-17,
+               -1.51415e-17
             },
          (16,0): {
-               -2.26535e-16,
-               2.27312e-18
+               -2.09857e-16,
+               -4.91682e-18
             },
          (16,1): {
-               -2.95352e-18,
-               4.99222e-17
+               -1.88794e-16,
+               -5.59575e-17
             },
          (17,0): {
-               -7.38685e-16,
-               -1.54031e-17
+               -3.70565e-16,
+               1.92542e-19
             },
          (17,1): {
-               2.66541e-18,
-               2.4365e-17
+               5.78076e-17,
+               1.31406e-17
             },
          (18,0): {
-               -1.21048e-16,
-               -1.45954e-17
+               -1.27052e-16,
+               -2.63235e-18
             },
          (18,1): {
-               1.94899e-17,
-               -6.42475e-17
+               -1.38678e-17,
+               3.57127e-19
             },
          (19,0): {
-               -9.95847e-18,
-               -1.46613e-18
+               -7.80979e-18,
+               -2.48328e-18
             },
          (19,1): {
-               4.58346e-18,
-               -9.51219e-18
+               -1.165e-17,
+               -5.16959e-18
             },
          (20,0): {
-               -3.62551e-16,
-               -4.72734e-18
+               -3.29486e-16,
+               -3.3727e-18
             },
          (20,1): {
-               1.12942e-17,
-               -1.59859e-16
+               -2.39648e-16,
+               -1.14184e-17
             },
          (21,0): {
-               -2.99598e-16,
-               1.63095e-18
+               -5.52976e-17,
+               2.56932e-18
             },
          (21,1): {
-               -1.32232e-17,
-               5.59817e-17
+               2.35665e-16,
+               1.73168e-17
             },
          (22,0): {
-               -3.1178e-17,
-               3.25634e-18
+               -4.77939e-18,
+               -3.2605e-19
             },
          (22,1): {
-               -8.90879e-18,
-               2.07907e-17
+               4.73678e-17,
+               2.20309e-17
             },
          (23,0): {
-               -2.68721e-17,
-               8.79346e-19
+               -7.23604e-18,
+               8.35583e-20
             },
          (23,1): {
-               3.1191e-18,
-               1.39871e-17
+               6.42081e-17,
+               1.67205e-18
             },
          (24,0): {
-               -1.46584e-17,
-               1.48627e-18
+               -4.4525e-18,
+               1.69898e-18
             },
          (24,1): {
-               6.01276e-18,
-               7.03791e-18
+               1.4759e-17,
+               1.43533e-17
             },
          (25,0): {
-               -1.09603e-16,
-               -2.76817e-18
+               8.44772e-19,
+               -8.05114e-19
             },
          (25,1): {
-               1.11705e-17,
-               -6.8794e-17
+               1.80683e-17,
+               -1.23027e-18
             },
          (26,0): {
-               -3.32307e-18,
-               3.58345e-18
+               -3.25993e-17,
+               -1.61317e-20
             },
          (26,1): {
-               -6.13452e-18,
-               8.7838e-17
+               -1.64361e-17,
+               -1.05259e-17
             },
          (27,0): {
-               3.0822e-17,
-               -3.36219e-19
+               -3.22442e-17,
+               -4.98175e-19
             },
          (27,1): {
-               -4.42175e-18,
-               1.75913e-16
+               2.11007e-17,
+               3.28018e-19
             },
          (28,0): {
-               -2.72103e-17,
-               1.21551e-18
+               -1.21267e-17,
+               -2.61718e-19
             },
          (28,1): {
-               -2.53855e-18,
-               8.10884e-17
+               -9.44703e-18,
+               2.80562e-18
             },
          (29,0): {
-               2.60444e-18,
-               -3.33092e-18
+               -4.84097e-18,
+               2.5324e-19
             },
          (29,1): {
-               1.09051e-17,
-               9.30777e-18
+               1.34841e-17,
+               1.96688e-18
             },
          (30,0): {
-               -5.23553e-17,
-               -1.96628e-18
+               -5.43421e-17,
+               -5.34143e-20
             },
          (30,1): {
-               3.50787e-18,
-               -8.03818e-18
+               -1.7692e-17,
+               1.87991e-19
             },
          (31,0): {
-               -2.06572e-17,
-               -6.40927e-19
+               -5.63037e-17,
+               3.72601e-19
             },
          (31,1): {
-               3.58939e-18,
-               5.24674e-17
+               -5.97505e-17,
+               -9.88298e-19
             },
          (32,0): {
-               3.53178e-17,
-               6.66648e-18
+               -5.11071e-17,
+               -1.26577e-19
             },
          (32,1): {
-               1.07247e-18,
-               1.89794e-16
+               -2.0854e-16,
+               -8.03499e-19
             },
          (33,0): {
-               -5.15348e-18,
-               -1.73796e-18
+               -6.16547e-18,
+               -5.21925e-19
             },
          (33,1): {
-               -6.96447e-18,
-               9.34213e-17
+               -4.26314e-17,
+               2.94289e-18
             },
          (34,0): {
-               -5.56133e-18,
-               -2.49126e-18
+               -5.1796e-17,
+               -5.10526e-19
             },
          (34,1): {
-               -4.18103e-18,
-               1.31985e-17
+               2.26329e-18,
+               -2.4499e-20
             },
          (35,0): {
-               -2.12346e-17,
-               -1.57678e-18
+               -1.35489e-18,
+               2.58831e-19
             },
          (35,1): {
-               4.13805e-18,
-               -4.55006e-17
+               1.51113e-17,
+               1.60019e-18
             },
          (36,0): {
-               2.31989e-17,
-               -4.96355e-18
+               3.04364e-17,
+               -5.3535e-20
             },
          (36,1): {
-               1.23192e-17,
-               -3.42596e-17
+               2.45081e-17,
+               -1.25863e-18
             },
          (37,0): {
-               7.10102e-17,
-               -1.17983e-18
+               1.49189e-17,
+               -2.41584e-19
             },
          (37,1): {
-               2.22783e-18,
-               8.27499e-18
+               3.52097e-17,
+               2.49413e-18
             },
          (38,0): {
-               2.37126e-17,
-               -4.59128e-18
+               2.90813e-17,
+               2.4842e-19
             },
          (38,1): {
-               9.17457e-19,
-               6.87122e-17
+               3.75639e-17,
+               1.08575e-18
             },
          (39,0): {
-               3.32519e-17,
-               7.40745e-18
+               1.77467e-17,
+               -1.53896e-19
             },
          (39,1): {
-               -2.28202e-18,
-               7.69846e-18
+               1.17991e-17,
+               -3.75933e-18
             },
          (40,0): {
-               -7.67267e-09,
-               -8.04218e-08
+               -8.05124e-08,
+               7.16789e-09
             },
          (40,1): {
-               -0.66463,
-               0.747071
+               -0.890987,
+               -0.453861
             },
          (41,0): {
-               -4.93937e-07,
-               7.26321e-08
+               6.89124e-08,
+               4.94056e-07
             },
          (41,1): {
-               0.00602537,
-               0.00839702
+               -0.00659813,
+               0.00795483
             },
          (42,0): {
-               1.50122e-09,
-               1.54466e-08
+               1.54403e-08,
+               -1.40868e-09
             },
          (42,1): {
-               0.00015891,
-               -0.000129951
+               0.000165947,
+               0.000120837
             },
          (43,0): {
-               2.23454e-10,
-               -2.79718e-11
+               -2.65953e-11,
+               -2.24728e-10
             },
          (43,1): {
-               -1.37642e-06,
-               -2.52013e-06
+               2.08962e-06,
+               -1.96956e-06
             },
          (44,0): {
-               -1.74512e-12,
-               -1.00002e-13
+               -1.35838e-13,
+               1.75851e-12
             },
          (44,1): {
-               -4.0141e-08,
-               2.14656e-08
+               -3.09273e-08,
+               -3.33993e-08
             },
          (45,0): {
-               -4.06499e-13,
-               -2.08725e-14
+               -2.02933e-14,
+               4.07659e-13
             },
          (45,1): {
-               2.03739e-10,
-               6.41809e-10
+               -5.69334e-10,
+               3.5955e-10
             },
          (46,0): {
-               1.56011e-15,
-               8.75202e-15
+               1.34166e-14,
+               -6.98526e-16
             },
          (46,1): {
-               9.42777e-12,
-               -1.98949e-12
+               4.31085e-12,
+               8.61689e-12
             },
          (47,0): {
-               2.08489e-16,
-               7.4528e-19
+               2.70044e-15,
+               -3.52473e-16
             },
          (47,1): {
-               -1.25887e-15,
-               -1.42502e-13
+               1.38862e-13,
+               -3.74514e-14
             },
          (48,0): {
-               7.62839e-16,
-               -2.06559e-17
+               3.24083e-15,
+               2.85968e-18
             },
          (48,1): {
-               -1.99169e-15,
-               2.23047e-15
+               2.20721e-15,
+               -1.88276e-15
             },
          (49,0): {
-               3.64627e-16,
-               -3.47988e-18
+               1.8208e-15,
+               -2.34847e-17
             },
          (49,1): {
-               5.38355e-17,
-               7.09335e-17
+               -5.27549e-18,
+               -5.52233e-17
             },
          (50,0): {
-               1.22633e-16,
-               -9.03106e-19
+               4.33638e-16,
+               -3.82545e-18
             },
          (50,1): {
-               4.6206e-17,
-               -3.30886e-16
+               -5.43239e-16,
+               -1.08922e-16
             },
          (51,0): {
-               -2.35268e-17,
-               3.88599e-18
+               4.47069e-16,
+               -4.07774e-18
             },
          (51,1): {
-               -1.58369e-18,
-               1.16878e-15
+               3.47707e-16,
+               3.05577e-18
             },
          (52,0): {
-               3.40565e-18,
-               -5.29424e-18
+               4.64034e-17,
+               -1.03673e-17
             },
          (52,1): {
-               1.84676e-18,
-               1.09492e-16
+               5.68436e-17,
+               1.34389e-17
             },
          (53,0): {
-               -3.1995e-17,
-               4.67061e-18
+               -6.51026e-17,
+               -1.48628e-18
             },
          (53,1): {
-               -1.22938e-17,
-               -1.52965e-16
+               -1.65139e-16,
+               -3.45868e-18
             },
          (54,0): {
-               -1.40429e-17,
-               1.18601e-18
+               -1.87494e-17,
+               -8.25525e-19
             },
          (54,1): {
-               -2.06496e-17,
-               -3.95662e-17
+               -7.25201e-17,
+               -1.08686e-17
             },
          (55,0): {
-               -7.45586e-17,
-               9.68651e-18
+               -1.03707e-16,
+               3.46569e-19
             },
          (55,1): {
-               -3.59157e-18,
-               -9.33732e-17
+               -3.12172e-16,
+               -1.73298e-17
             },
          (56,0): {
-               -1.5972e-16,
-               5.48361e-18
+               -3.36838e-16,
+               1.56126e-19
             },
          (56,1): {
-               -3.94169e-18,
-               -1.49589e-16
+               -2.35347e-16,
+               -2.47699e-18
             },
          (57,0): {
-               -1.59537e-16,
-               3.37694e-18
+               -7.66853e-17,
+               -5.27375e-19
             },
          (57,1): {
-               -1.1351e-18,
-               4.61455e-18
+               4.50379e-17,
+               1.65069e-17
             },
          (58,0): {
-               -5.69121e-16,
-               9.07719e-18
+               -3.66478e-16,
+               -8.80261e-19
             },
          (58,1): {
-               -9.57859e-18,
-               -5.52432e-16
+               -1.85431e-17,
+               1.4702e-17
             },
          (59,0): {
-               -5.19181e-16,
-               4.73264e-18
+               -2.2382e-16,
+               7.93135e-19
             },
          (59,1): {
-               -2.27896e-18,
-               -3.31815e-16
+               -1.55043e-16,
+               -1.38164e-17
             },
          (60,0): {
-               -3.36009e-16,
-               8.6097e-18
+               -1.29654e-16,
+               2.26192e-18
             },
          (60,1): {
-               1.38841e-18,
-               -1.61897e-17
+               -6.45465e-17,
+               -8.3083e-19
             },
          (61,0): {
-               -2.36913e-16,
-               1.29027e-17
+               -1.90499e-17,
+               -8.983e-20
             },
          (61,1): {
-               -6.63644e-19,
-               5.35129e-17
+               1.38717e-16,
+               -5.49969e-18
             },
          (62,0): {
-               -2.7962e-16,
-               1.36092e-18
+               -8.1047e-17,
+               -8.59107e-19
             },
          (62,1): {
-               -6.22079e-18,
-               1.35059e-16
+               5.10132e-16,
+               1.47578e-17
             },
          (63,0): {
-               -2.00995e-16,
-               2.85985e-18
+               -6.7646e-17,
+               3.8339e-19
             },
          (63,1): {
-               -2.42754e-18,
-               1.70254e-16
+               5.46725e-16,
+               1.52784e-17
             },
          (64,0): {
-               -1.55626e-16,
-               3.54387e-18
+               -1.05202e-16,
+               -4.15641e-19
             },
          (64,1): {
-               1.07686e-17,
-               3.14183e-18
+               2.5385e-16,
+               -7.68255e-18
             },
          (65,0): {
-               2.6153e-17,
-               8.01854e-18
+               -5.95366e-17,
+               2.17706e-19
             },
          (65,1): {
-               1.34495e-17,
-               -2.9921e-20
+               2.53368e-17,
+               -8.86335e-18
             },
          (66,0): {
-               -4.85714e-17,
-               1.75942e-17
+               -1.10861e-16,
+               9.15981e-20
             },
          (66,1): {
-               7.57435e-18,
-               1.48195e-16
+               8.26963e-17,
+               -5.3744e-18
             },
          (67,0): {
-               -2.17909e-17,
-               1.91437e-18
+               -1.65948e-17,
+               -7.13683e-19
             },
          (67,1): {
-               -2.25931e-18,
-               1.13013e-16
+               1.04441e-16,
+               2.27581e-18
             },
          (68,0): {
-               -2.96201e-17,
-               1.09828e-17
+               -1.84961e-16,
+               -6.8322e-20
             },
          (68,1): {
-               3.28917e-18,
-               9.51138e-17
+               -1.31686e-17,
+               1.31295e-18
             },
          (69,0): {
-               -7.62797e-17,
-               1.65696e-19
+               -5.23221e-17,
+               -2.80308e-19
             },
          (69,1): {
-               6.08974e-18,
-               1.46767e-17
+               6.89581e-17,
+               3.03068e-18
             },
          (70,0): {
-               -4.51245e-17,
-               1.41967e-18
+               -6.09571e-17,
+               -7.82255e-19
             },
          (70,1): {
-               5.02397e-18,
-               -9.29289e-19
+               -3.90771e-17,
+               -8.5571e-19
             },
          (71,0): {
-               1.45177e-17,
-               5.08285e-18
+               -8.2043e-17,
+               -3.03041e-19
             },
          (71,1): {
-               3.93148e-18,
-               7.57869e-17
+               -1.05439e-16,
+               -1.10545e-18
             },
          (72,0): {
-               8.30951e-18,
-               -1.02938e-18
+               -8.4496e-17,
+               -1.43117e-19
             },
          (72,1): {
-               -2.088e-18,
-               2.19567e-16
+               -1.63789e-16,
+               -3.10152e-18
             },
          (73,0): {
-               -5.50592e-17,
-               1.06805e-19
+               -3.27051e-17,
+               -2.02884e-19
             },
          (73,1): {
-               4.38005e-18,
-               2.22555e-16
+               -5.73563e-17,
+               1.09876e-18
             },
          (74,0): {
-               2.10519e-18,
-               -6.32385e-18
+               -4.62929e-18,
+               -8.19343e-20
             },
          (74,1): {
-               -1.40003e-19,
-               3.08489e-18
+               1.2008e-18,
+               -7.43815e-19
             },
          (75,0): {
-               3.40643e-18,
-               -1.53292e-18
+               4.51796e-17,
+               -2.89845e-19
             },
          (75,1): {
-               7.60054e-19,
-               -5.4519e-17
+               3.4199e-17,
+               -4.01652e-18
             },
          (76,0): {
-               3.05853e-17,
-               -1.27293e-17
+               1.75692e-17,
+               3.40234e-19
             },
          (76,1): {
-               -2.12935e-18,
-               -4.09918e-17
+               -2.05431e-17,
+               1.00997e-18
             },
          (77,0): {
-               1.97112e-17,
-               -5.78908e-18
+               -1.76168e-17,
+               7.4653e-19
             },
          (77,1): {
-               -3.20973e-18,
-               -4.45508e-18
+               8.93648e-17,
+               1.75135e-18
             },
          (78,0): {
-               3.14684e-17,
-               -1.07655e-17
+               3.10902e-17,
+               3.86152e-19
             },
          (78,1): {
-               -1.54408e-18,
-               5.40925e-17
+               3.50346e-17,
+               1.58975e-18
             },
          (79,0): {
-               2.82667e-17,
-               -4.17567e-18
+               6.0765e-17,
+               4.02159e-19
             },
          (79,1): {
-               2.24696e-19,
-               5.44267e-18
+               1.50899e-18,
+               8.10787e-19
             },
          (80,0): {
-               6.98151e-05,
-               -7.57786e-06
+               -1.39342e-05,
+               -6.88323e-05
             },
          (80,1): {
-               -4.82291e-08,
-               -7.08112e-08
+               4.96976e-08,
+               -6.95256e-08
             },
          (81,0): {
-               0.000351263,
-               -0.00571489
+               -0.00572282,
+               0.000172667
             },
          (81,1): {
-               -5.14054e-06,
-               5.14428e-06
+               -6.62014e-06,
+               -3.05388e-06
             },
          (82,0): {
-               -8.25021e-05,
-               1.12868e-05
+               1.87739e-05,
+               8.11214e-05
             },
          (82,1): {
-               5.44378e-08,
-               8.53209e-08
+               -6.13602e-08,
+               8.07819e-08
             },
          (83,0): {
-               1.30566e-07,
-               2.52295e-06
+               2.49875e-06,
+               -3.6048e-07
             },
          (83,1): {
-               1.88642e-09,
-               -1.46544e-09
+               2.03286e-09,
+               1.26728e-09
             },
          (84,0): {
-               4.16277e-08,
-               -8.34073e-09
+               -1.20994e-08,
+               -4.06573e-08
             },
          (84,1): {
-               -2.87202e-11,
-               -4.69213e-11
+               3.40988e-11,
+               -4.32107e-11
             },
          (85,0): {
-               -1.40457e-10,
-               -1.00836e-09
+               -9.90245e-10,
+               2.31795e-10
             },
          (85,1): {
-               -8.68062e-13,
-               4.82552e-13
+               -7.54853e-13,
+               -6.47281e-13
             },
          (86,0): {
-               -1.76921e-11,
-               4.47519e-12
+               6.0655e-12,
+               1.71889e-11
             },
          (86,1): {
-               1.35368e-14,
-               2.39569e-14
+               -1.80251e-14,
+               2.09199e-14
             },
          (87,0): {
-               8.20827e-14,
-               3.84097e-13
+               3.74287e-13,
+               -1.16823e-13
             },
          (87,1): {
-               4.77121e-16,
-               -2.29412e-16
+               4.12624e-16,
+               3.84437e-16
             },
          (88,0): {
-               6.86957e-15,
-               -2.07832e-15
+               -2.7321e-15,
+               -6.65335e-15
             },
          (88,1): {
-               -1.74894e-17,
-               -1.53083e-17
+               8.32261e-18,
+               8.10529e-19
             },
          (89,0): {
-               -6.94095e-16,
-               -1.48043e-16
+               -5.96411e-16,
+               4.75152e-17
             },
          (89,1): {
-               -1.07042e-17,
-               -3.87432e-16
+               -2.22319e-16,
+               -5.68949e-18
             },
          (90,0): {
-               -4.7406e-16,
-               3.90339e-18
+               -3.68615e-16,
+               3.53064e-18
             },
          (90,1): {
-               5.44803e-18,
-               -1.03764e-16
+               -1.30046e-16,
+               -1.19354e-17
             },
          (91,0): {
-               -3.19368e-16,
-               4.29108e-18
+               -8.84337e-17,
+               1.65597e-18
             },
          (91,1): {
-               1.4462e-17,
-               8.87611e-17
+               2.46211e-16,
+               5.8228e-18
             },
          (92,0): {
-               -1.15859e-16,
-               6.57934e-18
+               -3.57109e-17,
+               3.82766e-19
             },
          (92,1): {
-               -1.3716e-17,
-               1.8727e-16
+               5.41397e-16,
+               1.44767e-17
             },
          (93,0): {
-               -5.62403e-17,
-               1.23009e-17
+               -6.7737e-17,
+               5.3462e-19
             },
          (93,1): {
-               -4.49624e-17,
-               2.02391e-16
+               1.62452e-16,
+               3.50179e-18
             },
          (94,0): {
-               -4.25877e-18,
-               -1.90678e-18
+               1.86638e-18,
+               3.45584e-19
             },
          (94,1): {
-               7.12017e-18,
-               4.68973e-18
+               1.09183e-17,
+               5.82529e-18
             },
          (95,0): {
-               -1.70875e-16,
-               1.15296e-18
+               -3.45308e-18,
+               1.68009e-18
             },
          (95,1): {
-               2.60552e-17,
-               -4.26654e-17
+               6.09104e-17,
+               -5.40992e-18
             },
          (96,0): {
-               -1.67185e-17,
-               2.10324e-17
+               -1.11162e-17,
+               -1.28945e-20
             },
          (96,1): {
-               2.52179e-18,
-               1.63574e-16
+               4.509e-17,
+               -4.28707e-18
             },
          (97,0): {
-               1.04653e-17,
-               2.41036e-19
+               -1.55284e-16,
+               -4.40956e-19
             },
          (97,1): {
-               -7.662e-18,
-               1.8781e-16
+               2.43073e-16,
+               9.04901e-19
             },
          (98,0): {
-               1.6345e-17,
-               -1.31883e-17
+               -1.84754e-17,
+               -7.87844e-19
             },
          (98,1): {
-               4.9442e-18,
-               1.38003e-16
+               1.83064e-17,
+               8.94914e-19
             },
          (99,0): {
-               -5.58853e-17,
-               1.30641e-17
+               -1.15979e-16,
+               2.56442e-19
             },
          (99,1): {
-               -4.48606e-18,
-               1.12105e-18
+               1.32727e-17,
+               1.89216e-18
             },
          (100,0): {
-               -3.78339e-17,
-               6.91177e-18
+               3.81864e-19,
+               -2.45153e-19
             },
          (100,1): {
-               1.1526e-17,
-               4.96312e-19
+               -1.3949e-17,
+               2.51534e-20
             },
          (101,0): {
-               -5.60955e-17,
-               -1.08669e-17
+               6.31164e-18,
+               -3.83385e-19
             },
          (101,1): {
-               9.31229e-18,
-               7.60021e-17
+               -7.10463e-17,
+               -2.21328e-18
             },
          (102,0): {
-               -3.12764e-17,
-               -7.18913e-19
+               -2.91575e-17,
+               -2.85202e-19
             },
          (102,1): {
-               5.7815e-18,
-               1.10349e-16
+               -1.93148e-17,
+               -2.82807e-19
             },
          (103,0): {
-               -8.29331e-18,
-               -2.28366e-18
+               -2.48393e-17,
+               -3.74343e-19
             },
          (103,1): {
-               -2.91307e-18,
-               6.49925e-17
+               -1.31336e-17,
+               -1.27219e-18
             },
          (104,0): {
-               -3.90432e-17,
-               -2.26963e-18
+               -8.42618e-17,
+               -8.73284e-19
             },
          (104,1): {
-               -5.29075e-18,
-               5.11263e-17
+               -2.44542e-17,
+               -2.47847e-18
             },
          (105,0): {
-               -3.10387e-19,
-               -5.72345e-19
+               -5.49107e-17,
+               -1.304e-20
             },
          (105,1): {
-               7.41661e-18,
-               -5.00839e-17
+               4.38015e-18,
+               -1.91076e-18
             },
          (106,0): {
-               1.26925e-17,
-               -6.00046e-18
+               3.32213e-17,
+               -1.1923e-20
             },
          (106,1): {
-               1.68086e-18,
-               1.03149e-17
+               1.35498e-17,
+               -3.49738e-19
             },
          (107,0): {
-               3.55126e-17,
-               -4.6957e-18
+               5.18828e-17,
+               -5.22371e-19
             },
          (107,1): {
-               3.15532e-19,
-               2.88187e-17
+               9.13e-17,
+               2.44609e-18
             },
          (108,0): {
-               1.39996e-16,
-               -1.54197e-18
+               1.96053e-16,
+               3.98366e-19
             },
          (108,1): {
-               -1.19639e-17,
-               -2.79575e-17
+               7.31791e-17,
+               1.92345e-18
             },
          (109,0): {
-               7.12856e-17,
-               5.71634e-18
+               4.36327e-17,
+               7.68284e-19
             },
          (109,1): {
-               -8.5415e-18,
-               1.80613e-17
+               1.58346e-17,
+               -1.61798e-19
             },
          (110,0): {
-               4.46689e-17,
-               3.22267e-19
+               2.11111e-17,
+               -5.92365e-20
             },
          (110,1): {
-               2.36366e-18,
-               -1.66865e-17
+               -4.16968e-18,
+               -2.23219e-18
             },
          (111,0): {
-               6.28669e-17,
-               1.46266e-18
+               -2.06374e-17,
+               2.51861e-19
             },
          (111,1): {
-               3.44196e-18,
-               -5.15393e-18
+               -2.16956e-17,
+               -3.61897e-18
             },
          (112,0): {
-               3.88102e-17,
-               5.50008e-18
+               2.32259e-17,
+               3.17969e-19
             },
          (112,1): {
-               5.79728e-19,
-               -4.96104e-18
+               4.17849e-17,
+               2.49631e-19
             },
          (113,0): {
-               1.40975e-16,
-               5.39855e-18
+               1.83454e-17,
+               -1.38186e-19
             },
          (113,1): {
-               7.16652e-18,
-               3.77068e-18
+               4.0466e-17,
+               1.38578e-18
             },
          (114,0): {
-               9.33407e-18,
-               7.74216e-18
+               1.3258e-17,
+               1.53261e-19
             },
          (114,1): {
-               -4.83299e-18,
-               -6.12511e-19
+               8.4532e-18,
+               5.20367e-18
             },
          (115,0): {
-               -4.62767e-17,
-               3.95588e-18
+               6.86483e-17,
+               -5.8347e-20
             },
          (115,1): {
-               2.04131e-19,
-               7.67879e-17
+               -4.76768e-17,
+               -4.54168e-19
             },
          (116,0): {
-               3.5476e-18,
-               2.04494e-18
+               3.99402e-19,
+               -1.2238e-18
             },
          (116,1): {
-               1.64716e-18,
-               8.35438e-18
+               -9.02349e-18,
+               -4.55852e-18
             },
          (117,0): {
-               -1.38849e-17,
-               5.05254e-18
+               9.90605e-18,
+               -1.0412e-18
             },
          (117,1): {
-               -1.06946e-17,
-               1.26207e-17
+               -3.01798e-17,
+               -2.40399e-18
             },
          (118,0): {
-               -4.39431e-17,
-               4.49872e-18
+               1.52164e-18,
+               -1.25618e-18
             },
          (118,1): {
-               2.01465e-18,
-               1.39076e-17
+               -3.61691e-17,
+               -5.29225e-18
             },
          (119,0): {
-               -1.11948e-16,
-               3.92062e-18
+               4.29829e-17,
+               1.89847e-19
             },
          (119,1): {
-               3.53873e-19,
-               -9.15811e-18
+               -9.05586e-18,
+               2.30436e-18
             },
          (120,0): {
-               9.00009e-08,
-               -1.29134e-08
+               1.29753e-08,
+               9.00168e-08
             },
          (120,1): {
-               4.29916e-05,
-               5.61538e-05
+               4.30237e-05,
+               -5.59286e-05
             },
          (121,0): {
-               3.70434e-08,
-               -6.91822e-06
+               6.91781e-06,
+               3.17227e-08
             },
          (121,1): {
-               0.00382344,
-               -0.00426171
+               -0.00512106,
+               -0.00259605
             },
          (122,0): {
-               -1.06788e-07,
-               1.90704e-08
+               -1.91267e-08,
+               -1.06729e-07
             },
          (122,1): {
-               -4.86158e-05,
-               -6.80847e-05
+               -5.32679e-05,
+               6.47992e-05
             },
          (123,0): {
-               3.22418e-10,
-               3.28035e-09
+               -3.27703e-09,
+               3.242e-10
             },
          (123,1): {
-               -1.56673e-06,
-               1.27003e-06
+               1.63842e-06,
+               1.18716e-06
             },
          (124,0): {
-               4.06066e-11,
-               -1.44598e-11
+               1.44897e-11,
+               4.0503e-11
             },
          (124,1): {
-               1.54382e-08,
-               2.85838e-08
+               2.36591e-08,
+               -2.24088e-08
             },
          (125,0): {
-               -2.04861e-13,
-               -1.05621e-12
+               1.05346e-12,
+               -2.05409e-13
             },
          (125,1): {
-               5.04954e-10,
-               -2.64762e-10
+               -3.88403e-10,
+               -4.20157e-10
             },
          (126,0): {
-               -7.73271e-15,
-               6.95798e-15
+               -7.12133e-15,
+               -7.48608e-15
             },
          (126,1): {
-               -2.73647e-12,
-               -8.74369e-12
+               -7.7552e-12,
+               4.93685e-12
             },
          (127,0): {
-               -9.77763e-17,
-               1.65858e-16
+               -2.98011e-16,
+               8.83487e-17
             },
          (127,1): {
-               -1.37579e-13,
-               2.86726e-14
+               6.37733e-14,
+               1.25795e-13
             },
          (128,0): {
-               -8.24343e-16,
-               -2.69604e-18
+               -2.55064e-16,
+               -8.20931e-19
             },
          (128,1): {
-               3.5623e-17,
-               1.9441e-15
+               2.31814e-15,
+               -6.06266e-16
             },
          (129,0): {
-               -9.44537e-17,
-               2.02527e-18
+               3.98514e-17,
+               1.23334e-18
             },
          (129,1): {
-               3.87747e-17,
-               -7.9125e-17
+               4.80698e-17,
+               -3.96558e-17
             },
          (130,0): {
-               -1.1278e-16,
-               -9.29352e-19
+               -3.8589e-17,
+               -1.34008e-18
             },
          (130,1): {
-               1.51318e-18,
-               -1.15268e-17
+               -4.28238e-17,
+               -7.74797e-18
             },
          (131,0): {
-               -1.38897e-16,
-               1.49086e-19
+               -8.58498e-17,
+               5.72639e-19
             },
          (131,1): {
-               -7.49333e-19,
-               4.04217e-17
+               1.26604e-16,
+               -6.39648e-20
             },
          (132,0): {
-               -4.01371e-17,
-               -2.98875e-19
+               1.76209e-18,
+               1.1619e-19
             },
          (132,1): {
-               -3.35936e-18,
-               2.8983e-17
+               1.02058e-16,
+               4.0917e-18
             },
          (133,0): {
-               -8.70221e-17,
-               -3.18132e-18
+               -3.17643e-18,
+               -3.68292e-19
             },
          (133,1): {
-               -9.31414e-18,
-               1.25009e-16
+               3.28758e-16,
+               1.41007e-17
             },
          (134,0): {
-               -1.75961e-16,
-               4.3907e-19
+               1.40078e-16,
+               2.18686e-19
             },
          (134,1): {
-               6.47392e-18,
-               -1.71872e-17
+               2.94147e-16,
+               3.534e-18
             },
          (135,0): {
-               -4.27126e-17,
-               2.24845e-18
+               7.76566e-17,
+               -1.11014e-18
             },
          (135,1): {
-               3.57449e-18,
-               1.65673e-18
+               2.31826e-17,
+               -7.57376e-18
             },
          (136,0): {
-               -2.93368e-17,
-               1.67192e-19
+               4.22653e-18,
+               -8.02889e-20
             },
          (136,1): {
-               -2.61723e-18,
-               3.49102e-17
+               -1.10927e-17,
+               -4.48967e-18
             },
          (137,0): {
-               -6.43257e-17,
-               -4.93381e-20
+               -6.83577e-17,
+               3.98459e-19
             },
          (137,1): {
-               -4.0412e-18,
-               2.69152e-16
+               2.74013e-17,
+               1.02787e-18
             },
          (138,0): {
-               4.18883e-19,
-               6.38828e-19
+               -2.41233e-17,
+               -4.38892e-19
             },
          (138,1): {
-               4.29567e-18,
-               1.29513e-16
+               1.4071e-16,
+               2.48443e-18
             },
          (139,0): {
-               1.23706e-17,
-               2.01272e-20
+               -1.31153e-17,
+               -5.09161e-20
             },
          (139,1): {
-               4.61379e-18,
-               1.48129e-17
+               5.80135e-18,
+               1.22623e-18
             },
          (140,0): {
-               -9.75454e-17,
-               -1.84802e-18
+               -6.73539e-17,
+               -1.6204e-18
             },
          (140,1): {
-               4.39149e-18,
-               7.28763e-18
+               -3.25159e-17,
+               1.13928e-18
             },
          (141,0): {
-               -1.00225e-16,
-               -5.27299e-19
+               -9.61273e-17,
+               -1.98614e-19
             },
          (141,1): {
-               -8.30995e-19,
-               8.56041e-17
+               -7.79806e-17,
+               -3.92196e-18
             },
          (142,0): {
-               1.85064e-17,
-               -8.94775e-19
+               -3.7642e-17,
+               7.42324e-19
             },
          (142,1): {
-               -3.41564e-18,
-               2.74759e-16
+               -1.1605e-16,
+               -1.45892e-18
             },
          (143,0): {
-               -1.16934e-17,
-               -1.81231e-19
+               -2.18833e-17,
+               -1.30574e-19
             },
          (143,1): {
-               -3.85793e-18,
-               3.30812e-17
+               7.67884e-18,
+               1.95748e-18
             },
          (144,0): {
-               3.9765e-17,
-               -1.68043e-19
+               -8.58956e-17,
+               3.12453e-20
             },
          (144,1): {
-               9.93949e-19,
-               4.01338e-17
+               2.77328e-18,
+               2.82088e-19
             },
          (145,0): {
-               5.23265e-17,
-               5.14819e-20
+               1.00266e-17,
+               1.43164e-19
             },
          (145,1): {
-               6.82292e-18,
-               -6.77067e-18
+               -1.02206e-18,
+               1.67169e-18
             },
          (146,0): {
-               1.86659e-17,
-               -1.84706e-18
+               2.3125e-17,
+               2.76477e-19
             },
          (146,1): {
-               1.14694e-18,
-               -2.63658e-17
+               -6.9065e-18,
+               -1.03168e-18
             },
          (147,0): {
-               1.36566e-16,
-               -6.99201e-19
+               4.11532e-17,
+               1.9395e-19
             },
          (147,1): {
-               -1.28153e-18,
-               1.77884e-16
+               1.33666e-16,
+               1.61208e-19
             },
          (148,0): {
-               6.97835e-17,
-               2.13833e-19
+               -1.02575e-17,
+               2.99316e-19
             },
          (148,1): {
-               -2.19575e-18,
-               4.24612e-17
+               7.52021e-17,
+               1.11006e-18
             },
          (149,0): {
-               1.00981e-16,
-               1.00914e-18
+               8.3312e-17,
+               -5.30511e-19
             },
          (149,1): {
-               -3.03687e-20,
-               -1.01834e-18
+               8.00633e-18,
+               -9.94061e-19
             },
          (150,0): {
-               2.22592e-17,
-               1.06041e-18
+               -5.7783e-19,
+               -6.54345e-19
             },
          (150,1): {
-               2.78957e-18,
-               6.28752e-18
+               -3.8967e-18,
+               -3.38231e-19
             },
          (151,0): {
-               4.24164e-17,
-               5.13453e-19
+               1.12835e-17,
+               2.40236e-19
             },
          (151,1): {
-               -1.60224e-19,
-               -8.12116e-18
+               -4.332e-18,
+               -9.51374e-19
             },
          (152,0): {
-               5.81931e-17,
-               7.58988e-19
+               1.75154e-17,
+               -5.87241e-20
             },
          (152,1): {
-               -9.33595e-20,
-               -3.44198e-17
+               -1.21409e-18,
+               -1.782e-18
             },
          (153,0): {
-               7.358e-17,
-               4.6504e-19
+               3.60933e-17,
+               2.36664e-20
             },
          (153,1): {
-               1.99981e-18,
-               1.49469e-17
+               2.23416e-17,
+               3.08268e-18
             },
          (154,0): {
-               5.54404e-17,
-               4.85512e-19
+               2.07207e-17,
+               -4.80246e-19
             },
          (154,1): {
-               1.71281e-18,
-               -1.79762e-17
+               8.54144e-18,
+               3.03124e-18
             },
          (155,0): {
-               6.06109e-17,
-               4.38496e-19
+               4.50655e-17,
+               -4.68656e-19
             },
          (155,1): {
-               -1.43648e-18,
-               2.36919e-17
+               -7.55481e-17,
+               4.23893e-20
             },
          (156,0): {
-               -3.91196e-18,
-               1.1068e-18
+               1.30149e-18,
+               -6.75809e-19
             },
          (156,1): {
-               -1.41104e-18,
-               -5.86907e-18
+               -1.05863e-16,
+               -6.24447e-19
             },
          (157,0): {
-               -4.58838e-17,
-               7.85926e-19
+               5.09344e-19,
+               6.00376e-20
             },
          (157,1): {
-               -2.99516e-18,
-               2.62516e-17
+               -1.16597e-16,
+               -1.96954e-18
             },
          (158,0): {
-               -3.63428e-17,
-               1.64645e-18
+               4.26157e-17,
+               -1.07585e-18
             },
          (158,1): {
-               1.62424e-18,
-               -3.95921e-17
+               -5.63357e-17,
+               -2.38439e-18
             },
          (159,0): {
-               -1.85224e-16,
-               -2.01672e-18
+               9.5594e-18,
+               2.13647e-18
             },
          (159,1): {
-               2.19542e-18,
-               -2.41296e-17
+               6.53315e-18,
+               5.25052e-18
             },
          (160,0): {
-               8.7142e-11,
-               -8.78325e-10
+               -6.76843e-11,
+               8.35101e-10
             },
          (160,1): {
-               -2.63945e-05,
-               2.15677e-05
+               -1.93917e-05,
+               2.83492e-05
             },
          (161,0): {
-               -7.43521e-08,
-               -1.41248e-08
+               7.29334e-08,
+               1.24548e-08
             },
          (161,1): {
-               -0.00247148,
-               -0.00230724
+               -0.00300109,
+               -0.00150753
             },
          (162,0): {
-               -9.47148e-11,
-               -1.0284e-09
+               1.23726e-10,
+               1.08114e-09
             },
          (162,1): {
-               -3.66515e-05,
-               3.17407e-05
+               -2.59767e-05,
+               4.05441e-05
             },
          (163,0): {
-               -5.00638e-11,
-               8.5146e-12
+               5.12319e-11,
+               -9.50447e-12
             },
          (163,1): {
-               8.81661e-07,
-               9.45672e-07
+               1.1067e-06,
+               6.53905e-07
             },
          (164,0): {
-               1.05585e-12,
-               1.07811e-12
+               -1.08533e-12,
+               -1.00189e-12
             },
          (164,1): {
-               1.6473e-08,
-               -1.24617e-08
+               1.21862e-08,
+               -1.65289e-08
             },
          (165,0): {
-               -1.12492e-14,
-               -3.55674e-14
+               1.29304e-14,
+               3.50936e-14
             },
          (165,1): {
-               -2.40286e-10,
-               -3.14847e-10
+               -3.18202e-10,
+               -2.32543e-10
             },
          (166,0): {
-               -8.27355e-16,
-               -2.74872e-15
+               5.02033e-16,
+               2.67415e-15
             },
          (166,1): {
-               -5.45181e-12,
-               3.2244e-12
+               -4.2877e-12,
+               4.61955e-12
             },
          (167,0): {
-               -4.61595e-16,
-               4.60155e-17
+               -1.12671e-16,
+               -3.08799e-17
             },
          (167,1): {
-               4.88375e-14,
-               9.19863e-14
+               7.31351e-14,
+               7.36676e-14
             },
          (168,0): {
-               -7.65692e-17,
-               1.02441e-17
+               2.73344e-17,
+               -2.57176e-18
             },
          (168,1): {
-               1.51286e-15,
-               -3.88127e-16
+               1.63963e-15,
+               -9.45998e-16
             },
          (169,0): {
-               -3.58193e-17,
-               7.29886e-18
+               3.78787e-17,
+               4.89381e-20
             },
          (169,1): {
-               -1.60829e-17,
-               -1.62046e-17
+               1.47522e-16,
+               -2.37564e-17
             },
          (170,0): {
-               4.33766e-19,
-               8.01326e-18
+               2.12322e-17,
+               -1.01474e-19
             },
          (170,1): {
-               -1.09841e-17,
-               -1.14587e-18
+               -8.78145e-18,
+               8.87313e-21
             },
          (171,0): {
-               -2.14427e-17,
-               2.2816e-18
+               5.63016e-18,
+               -4.72498e-19
             },
          (171,1): {
-               4.70731e-18,
-               6.21169e-17
+               2.33865e-17,
+               2.72433e-18
             },
          (172,0): {
-               -4.1315e-17,
-               1.61922e-18
+               -7.3761e-17,
+               -1.72589e-19
             },
          (172,1): {
-               -1.01908e-17,
-               3.46075e-16
+               -4.24555e-17,
+               -1.21615e-18
             },
          (173,0): {
-               8.13076e-17,
-               -1.45482e-19
+               4.77201e-18,
+               -1.4318e-19
             },
          (173,1): {
-               -3.48664e-18,
-               1.81837e-16
+               1.43192e-16,
+               2.37065e-18
             },
          (174,0): {
-               -4.64027e-17,
-               -3.65228e-19
+               -6.0958e-17,
+               -6.00735e-19
             },
          (174,1): {
-               1.03342e-17,
-               6.42345e-17
+               6.82901e-17,
+               8.25697e-19
             },
          (175,0): {
-               3.15622e-18,
-               -8.56673e-18
+               -1.83444e-17,
+               -2.5663e-19
             },
          (175,1): {
-               7.34526e-18,
-               -7.22179e-18
+               -6.99256e-18,
+               -3.224e-18
             },
          (176,0): {
-               1.056e-18,
-               -7.80932e-18
+               -3.25182e-17,
+               7.80126e-19
             },
          (176,1): {
-               2.87511e-18,
-               3.12831e-17
+               -1.20502e-17,
+               1.38539e-18
             },
          (177,0): {
-               3.15285e-17,
-               -1.26793e-17
+               3.52071e-17,
+               -8.30633e-20
             },
          (177,1): {
-               1.10535e-17,
-               1.51587e-16
+               -1.12752e-16,
+               -2.99176e-20
             },
          (178,0): {
-               -3.63696e-18,
-               -1.13702e-17
+               -1.87976e-17,
+               -2.11406e-19
             },
          (178,1): {
-               9.58913e-18,
-               7.84883e-17
+               -1.16863e-17,
+               1.18639e-18
             },
          (179,0): {
-               2.16271e-17,
-               -1.1549e-17
+               -6.22412e-18,
+               -1.35843e-19
             },
          (179,1): {
-               7.81237e-18,
-               6.82996e-17
+               -7.48201e-17,
+               7.54526e-20
             },
          (180,0): {
-               2.19658e-18,
-               -1.42402e-17
+               -3.03074e-17,
+               4.84426e-19
             },
          (180,1): {
-               3.10825e-18,
-               -6.07367e-18
+               8.92603e-19,
+               2.83915e-18
             },
          (181,0): {
-               5.41812e-19,
-               -8.53031e-18
+               -1.69046e-18,
+               -5.20529e-19
             },
          (181,1): {
-               -7.43509e-19,
-               6.40792e-20
+               1.5606e-17,
+               7.63944e-19
             },
          (182,0): {
-               5.68596e-17,
-               -7.87005e-18
+               -6.29725e-17,
+               2.75888e-19
             },
          (182,1): {
-               -2.19909e-18,
-               -7.91662e-17
+               1.48965e-16,
+               -5.35139e-19
             },
          (183,0): {
-               1.20583e-17,
-               -1.22483e-17
+               2.87131e-18,
+               3.98127e-19
             },
          (183,1): {
-               -8.33129e-19,
-               1.95768e-17
+               1.69147e-17,
+               2.71244e-18
             },
          (184,0): {
-               9.48603e-17,
-               -7.0149e-18
+               -6.25018e-19,
+               1.00173e-19
             },
          (184,1): {
-               -3.21803e-18,
-               1.13849e-17
+               5.99358e-17,
+               4.31886e-18
             },
          (185,0): {
-               1.2087e-16,
-               -4.45561e-18
+               1.27339e-17,
+               5.89719e-19
             },
          (185,1): {
-               -2.01411e-18,
-               -3.68012e-17
+               -2.29422e-18,
+               -4.30085e-18
             },
          (186,0): {
-               7.77617e-17,
-               4.79623e-18
+               3.53862e-17,
+               2.51536e-19
             },
          (186,1): {
-               2.5261e-18,
-               -3.63561e-17
+               -3.29898e-17,
+               -2.63366e-18
             },
          (187,0): {
-               7.16577e-17,
-               -1.40188e-17
+               2.89173e-17,
+               -1.83928e-19
             },
          (187,1): {
-               -2.7132e-18,
-               -1.93882e-17
+               -8.51688e-17,
+               1.57207e-18
             },
          (188,0): {
-               5.23033e-18,
-               -8.27832e-18
+               -6.78662e-18,
+               -7.14172e-19
             },
          (188,1): {
-               -7.55788e-18,
-               9.56384e-18
+               4.4306e-18,
+               3.07712e-18
             },
          (189,0): {
-               1.18986e-16,
-               3.29456e-18
+               1.11031e-17,
+               -1.25686e-19
             },
          (189,1): {
-               1.61422e-18,
-               -6.88121e-18
+               4.59077e-18,
+               9.51252e-19
             },
          (190,0): {
-               3.67842e-17,
-               -3.94462e-18
+               2.03238e-18,
+               -3.29911e-19
             },
          (190,1): {
-               -3.88041e-18,
-               2.47503e-18
+               -1.12104e-17,
+               -1.66742e-18
             },
          (191,0): {
-               3.31074e-18,
-               -9.01923e-19
+               2.86281e-20,
+               1.0172e-19
             },
          (191,1): {
-               -3.39119e-18,
-               2.4812e-18
+               -8.10999e-18,
+               2.11434e-18
             },
          (192,0): {
-               -3.29663e-17,
-               -7.02822e-19
+               -4.58982e-17,
+               -6.92969e-19
             },
          (192,1): {
-               -6.35614e-18,
-               8.81918e-17
+               -3.48763e-17,
+               -1.68552e-19
             },
          (193,0): {
-               -4.18511e-17,
-               -5.14757e-19
+               2.06663e-17,
+               4.74241e-19
             },
          (193,1): {
-               -8.93087e-18,
-               -2.75008e-17
+               -2.82774e-17,
+               1.97584e-18
             },
          (194,0): {
-               -2.59377e-17,
-               6.03718e-18
+               2.26251e-17,
+               -6.99785e-20
             },
          (194,1): {
-               -1.02878e-18,
-               -3.82072e-18
+               -1.41497e-18,
+               1.45678e-18
             },
          (195,0): {
-               -1.18653e-16,
-               -9.80354e-19
+               3.92113e-17,
+               -2.29674e-19
             },
          (195,1): {
-               -1.41658e-17,
-               -5.44687e-18
+               -1.56722e-17,
+               -1.64966e-18
             },
          (196,0): {
-               -1.12234e-16,
-               9.56677e-18
+               3.46042e-17,
+               2.12524e-19
             },
          (196,1): {
-               -7.65767e-18,
-               2.31732e-17
+               3.95401e-17,
+               -3.09343e-18
             },
          (197,0): {
-               -1.76891e-16,
-               -4.26251e-18
+               1.04851e-16,
+               2.43686e-19
             },
          (197,1): {
-               -4.15313e-18,
-               7.95895e-17
+               -3.8716e-18,
+               1.34782e-18
             },
          (198,0): {
-               -5.18027e-17,
-               8.2448e-18
+               2.62657e-17,
+               3.99557e-19
             },
          (198,1): {
-               -9.60423e-18,
-               2.38518e-17
+               -2.03505e-18,
+               -5.03171e-18
             },
          (199,0): {
-               -4.88698e-17,
-               3.80046e-18
+               3.15649e-17,
+               3.72465e-19
             },
          (199,1): {
-               1.51708e-17,
-               -1.82149e-17
+               4.63716e-18,
+               -5.64759e-18
             },
          (200,0): {
-               -2.6142e-06,
-               -2.5303e-05
+               2.54107e-06,
+               2.53968e-05
             },
          (200,1): {
-               -3.62284e-09,
-               1.14072e-09
+               -3.20814e-09,
+               2.04189e-09
             },
          (201,0): {
-               0.00251925,
-               9.12552e-06
+               -0.00251156,
+               -1.64574e-05
             },
          (201,1): {
-               -1.89965e-08,
-               -5.95114e-08
+               -3.35887e-08,
+               -5.24584e-08
             },
          (202,0): {
-               -1.29991e-06,
-               -3.59265e-05
+               1.10728e-06,
+               3.58205e-05
             },
          (202,1): {
-               -6.66906e-10,
-               4.91293e-09
+               6.31816e-10,
+               4.91133e-09
             },
          (203,0): {
-               -9.3247e-07,
-               2.15982e-08
+               9.2772e-07,
+               -1.73592e-08
             },
          (203,1): {
-               9.56836e-11,
-               9.76673e-11
+               1.17272e-10,
+               6.91774e-11
             },
          (204,0): {
-               1.12873e-09,
-               1.45892e-08
+               -1.02945e-09,
+               -1.45081e-08
             },
          (204,1): {
-               2.17851e-12,
-               -2.42586e-12
+               1.45444e-12,
+               -2.8868e-12
             },
          (205,0): {
-               3.30996e-10,
-               -2.16556e-11
+               -3.28777e-10,
+               1.96468e-11
             },
          (205,1): {
-               -2.38523e-14,
-               -3.80318e-14
+               -3.23341e-14,
+               -3.02043e-14
             },
          (206,0): {
-               -6.37437e-13,
-               -5.62447e-12
+               5.9234e-13,
+               5.58505e-12
             },
          (206,1): {
-               -2.51676e-15,
-               2.26595e-15
+               -1.27994e-15,
+               2.81563e-15
             },
          (207,0): {
-               -1.17336e-13,
-               1.2271e-14
+               1.16274e-13,
+               -1.13843e-14
             },
          (207,1): {
-               4.90226e-17,
-               6.95558e-17
+               2.21677e-16,
+               4.95196e-17
             },
          (208,0): {
-               2.83107e-16,
-               2.04418e-15
+               -3.29342e-16,
+               -2.02625e-15
             },
          (208,1): {
-               7.5252e-18,
-               -1.30325e-17
+               9.91367e-19,
+               -4.36273e-18
             },
          (209,0): {
-               -1.12032e-17,
-               -5.04809e-18
+               -2.53955e-17,
+               5.76589e-18
             },
          (209,1): {
-               -1.72841e-20,
-               1.51181e-16
+               6.75359e-17,
+               -8.92514e-19
             },
          (210,0): {
-               -1.32711e-17,
-               -5.74071e-19
+               -2.80745e-18,
+               7.96161e-19
             },
          (210,1): {
-               -4.77246e-18,
-               4.08627e-17
+               9.02186e-18,
+               1.43031e-18
             },
          (211,0): {
-               2.22715e-17,
-               -4.37026e-19
+               -1.63818e-17,
+               2.69503e-19
             },
          (211,1): {
-               -1.24813e-18,
-               5.85976e-17
+               5.54061e-17,
+               1.124e-18
             },
          (212,0): {
-               7.36296e-19,
-               -3.64721e-19
+               -1.80092e-17,
+               4.0037e-19
             },
          (212,1): {
-               1.77867e-18,
-               8.14279e-18
+               3.54606e-17,
+               3.78595e-18
             },
          (213,0): {
-               -6.65562e-17,
-               -1.56041e-19
+               -3.08014e-17,
+               6.80917e-19
             },
          (213,1): {
-               1.28395e-17,
-               2.22429e-17
+               -3.48051e-17,
+               3.07464e-18
             },
          (214,0): {
-               -9.81163e-18,
-               -5.92168e-19
+               -5.38952e-17,
+               -4.66241e-19
             },
          (214,1): {
-               -4.05377e-18,
-               1.47126e-16
+               -2.41218e-16,
+               -2.87197e-18
             },
          (215,0): {
-               -3.03436e-17,
-               -3.70822e-19
+               -5.84989e-17,
+               1.42734e-18
             },
          (215,1): {
-               -1.22615e-18,
-               2.43072e-16
+               -3.39741e-17,
+               -8.94537e-19
             },
          (216,0): {
-               -9.20011e-18,
-               -1.55749e-20
+               -1.1301e-17,
+               -5.72959e-20
             },
          (216,1): {
-               -1.95525e-18,
-               3.97947e-17
+               -1.05409e-17,
+               -1.50261e-19
             },
          (217,0): {
-               3.38421e-17,
-               -1.38846e-19
+               -1.19906e-16,
+               -6.9084e-19
             },
          (217,1): {
-               -2.29871e-18,
-               2.45568e-17
+               2.36687e-18,
+               3.12027e-19
             },
          (218,0): {
-               3.56205e-17,
-               6.93387e-19
+               -3.75154e-17,
+               4.11966e-19
             },
          (218,1): {
-               9.46718e-19,
-               -1.07094e-17
+               1.73944e-17,
+               -9.83861e-19
             },
          (219,0): {
-               8.41036e-18,
-               -2.41149e-19
+               4.39234e-18,
+               -2.71394e-20
             },
          (219,1): {
-               2.1998e-18,
-               -5.11469e-18
+               6.33118e-18,
+               -5.47834e-19
             },
          (220,0): {
-               5.22049e-17,
-               -6.95674e-19
+               5.70926e-17,
+               2.85205e-19
             },
          (220,1): {
-               1.16714e-18,
-               2.89164e-17
+               3.20304e-17,
+               1.05245e-18
             },
          (221,0): {
-               8.26432e-17,
-               1.52766e-19
+               1.12653e-16,
+               4.05359e-20
             },
          (221,1): {
-               9.7887e-20,
-               1.57994e-17
+               6.80146e-17,
+               1.78221e-18
             },
          (222,0): {
-               6.63811e-17,
-               7.04091e-20
+               -1.97291e-17,
+               -5.43521e-20
             },
          (222,1): {
-               8.76971e-19,
-               3.04042e-17
+               2.07821e-17,
+               -2.17097e-18
             },
          (223,0): {
-               2.09869e-16,
-               3.30432e-19
+               4.11536e-17,
+               1.30947e-19
             },
          (223,1): {
-               2.53357e-18,
-               -6.7748e-17
+               -4.32859e-17,
+               -2.10161e-18
             },
          (224,0): {
-               7.29063e-17,
-               4.06248e-19
+               5.41944e-17,
+               -5.58723e-19
             },
          (224,1): {
-               2.14324e-19,
-               -1.55606e-17
+               -8.38582e-18,
+               -5.25396e-19
             },
          (225,0): {
-               1.21986e-16,
-               -2.54567e-19
+               -2.76346e-17,
+               -1.9161e-19
             },
          (225,1): {
-               7.60132e-19,
-               -7.03407e-17
+               1.64056e-18,
+               -1.61531e-18
             },
          (226,0): {
-               2.25351e-17,
-               -1.1379e-19
+               -1.05307e-17,
+               -2.1437e-19
             },
          (226,1): {
-               3.86741e-19,
-               -3.84444e-18
+               3.29158e-18,
+               1.79446e-18
             },
          (227,0): {
-               2.50159e-17,
-               2.58589e-18
+               -1.45435e-17,
+               -4.10893e-19
             },
          (227,1): {
-               3.15903e-18,
-               -1.11766e-17
+               1.1449e-17,
+               7.4678e-18
             },
          (228,0): {
-               8.20633e-17,
-               -8.76096e-20
+               -2.63984e-17,
+               -2.15494e-19
             },
          (228,1): {
-               -1.26019e-18,
-               3.57449e-18
+               -9.73875e-18,
+               -5.44237e-19
             },
          (229,0): {
-               -6.85605e-19,
-               -2.55438e-18
+               -1.43534e-17,
+               -6.76762e-19
             },
          (229,1): {
-               -8.05673e-19,
-               2.57807e-17
+               -1.01081e-17,
+               -4.13303e-19
             },
          (230,0): {
-               6.35788e-19,
-               8.52795e-19
+               -1.42055e-18,
+               -4.04109e-19
             },
          (230,1): {
-               -2.18164e-18,
-               5.90681e-19
+               -2.98435e-18,
+               -1.29874e-18
             },
          (231,0): {
-               -4.55507e-17,
-               1.02133e-18
+               3.37518e-18,
+               -1.39009e-18
             },
          (231,1): {
-               -2.98304e-18,
-               -2.60578e-17
+               -1.76935e-17,
+               -3.29517e-18
             },
          (232,0): {
-               -1.19317e-16,
-               -3.3346e-19
+               -5.00316e-17,
+               -5.3799e-19
             },
          (232,1): {
-               2.60956e-18,
-               -7.62805e-18
+               -9.60124e-18,
+               8.68023e-19
             },
          (233,0): {
-               -8.7375e-17,
-               -1.41218e-18
+               3.51984e-17,
+               1.64409e-18
             },
          (233,1): {
-               4.0298e-19,
-               6.20849e-17
+               7.85963e-19,
+               2.16418e-19
             },
          (234,0): {
-               -6.81357e-17,
-               -4.97796e-19
+               1.86981e-17,
+               4.45934e-20
             },
          (234,1): {
-               6.25898e-19,
-               4.3146e-17
+               -6.88827e-18,
+               -6.70416e-18
             },
          (235,0): {
-               -1.72697e-16,
-               -4.60849e-20
+               7.42212e-17,
+               2.19514e-19
             },
          (235,1): {
-               -1.50346e-20,
-               1.42659e-16
+               4.45132e-17,
+               -6.5166e-19
             },
          (236,0): {
-               -2.05932e-17,
-               -8.75388e-20
+               1.25423e-17,
+               1.47225e-18
             },
          (236,1): {
-               4.36841e-18,
-               -6.73998e-18
+               -3.6024e-18,
+               2.49798e-18
             },
          (237,0): {
-               -7.54789e-17,
-               -2.0459e-18
+               3.69707e-17,
+               -7.17794e-20
             },
          (237,1): {
-               7.27802e-18,
-               -1.47755e-17
+               9.45155e-18,
+               7.72279e-18
             },
          (238,0): {
-               -6.23696e-18,
-               -8.50779e-19
+               2.52723e-17,
+               -1.16741e-19
             },
          (238,1): {
-               -1.35379e-18,
-               -6.54598e-17
+               -5.207e-18,
+               -1.79145e-18
             },
          (239,0): {
-               -4.40254e-17,
-               1.29255e-19
+               2.91328e-17,
+               2.22018e-19
             },
          (239,1): {
-               1.12114e-17,
-               -1.0787e-16
+               -1.98845e-17,
+               4.51627e-18
             },
          (240,0): {
-               -2.49915e-05,
-               7.48093e-07
+               2.49905e-05,
+               -7.19975e-07
             },
          (240,1): {
-               -5.63527e-07,
-               -5.12297e-07
+               -6.76527e-07,
+               -3.5002e-07
             },
          (241,0): {
-               -8.80042e-05,
-               2.87979e-07
+               8.7846e-05,
+               -1.85087e-07
             },
          (241,1): {
-               1.06538e-06,
-               -1.54345e-07
+               9.86826e-07,
+               -4.20736e-07
             },
          (242,0): {
-               3.31136e-05,
-               1.43887e-06
+               -3.31097e-05,
+               -1.47571e-06
             },
          (242,1): {
-               7.28118e-07,
-               6.34074e-07
+               8.70393e-07,
+               4.2713e-07
             },
          (243,0): {
-               -7.882e-08,
-               -5.7889e-07
+               7.82919e-08,
+               5.78945e-07
             },
          (243,1): {
-               1.2741e-08,
-               -9.07658e-09
+               1.00086e-08,
+               -1.21197e-08
             },
          (244,0): {
-               -1.92375e-08,
-               1.6945e-09
+               1.92254e-08,
+               -1.67474e-09
             },
          (244,1): {
-               -2.69793e-10,
-               -3.2698e-10
+               -3.46833e-10,
+               -2.47505e-10
             },
          (245,0): {
-               7.84493e-11,
-               3.46297e-10
+               -7.8069e-11,
+               -3.46078e-10
             },
          (245,1): {
-               -6.2206e-12,
-               3.24304e-12
+               -5.19547e-12,
+               4.77021e-12
             },
          (246,0): {
-               8.73088e-12,
-               -1.59654e-12
+               -8.72254e-12,
+               1.58643e-12
             },
          (246,1): {
-               5.94402e-14,
-               1.14211e-13
+               8.7499e-14,
+               9.5445e-14
             },
          (247,0): {
-               -4.66959e-14,
-               -1.60826e-13
+               4.65674e-14,
+               1.60673e-13
             },
          (247,1): {
-               1.967e-15,
-               -4.19985e-16
+               1.81165e-15,
+               -1.02461e-15
             },
          (248,0): {
-               -3.59398e-15,
-               9.53711e-16
+               3.59033e-15,
+               -9.33449e-16
             },
          (248,1): {
-               -2.90929e-17,
-               1.17754e-16
+               6.35074e-17,
+               -2.80377e-17
             },
          (249,0): {
-               -1.83309e-17,
-               7.77364e-17
+               -1.07985e-17,
+               -6.55134e-17
             },
          (249,1): {
-               -9.23861e-18,
-               4.54587e-17
+               8.72458e-17,
+               2.32171e-18
             },
          (250,0): {
-               4.53177e-18,
-               -8.02929e-18
+               -7.01667e-18,
+               5.41844e-19
             },
          (250,1): {
-               1.57284e-17,
-               -6.04544e-19
+               -9.73756e-18,
+               -8.10226e-19
             },
          (251,0): {
-               -7.05422e-18,
-               -6.82672e-18
+               -2.71159e-17,
+               -2.98586e-19
             },
          (251,1): {
-               1.75433e-17,
-               5.40683e-18
+               -4.58307e-17,
+               -1.81127e-18
             },
          (252,0): {
-               -1.01321e-17,
-               -8.65365e-18
+               -1.96003e-17,
+               9.01487e-20
             },
          (252,1): {
-               1.80047e-18,
-               6.12713e-17
+               -5.37162e-17,
+               -4.72983e-19
             },
          (253,0): {
-               -1.12246e-17,
-               -6.79664e-18
+               2.55752e-17,
+               -2.35331e-19
             },
          (253,1): {
-               -4.78401e-18,
-               1.06418e-16
+               -2.46773e-17,
+               -1.00359e-18
             },
          (254,0): {
-               -5.07681e-18,
-               -6.62949e-19
+               -9.4651e-17,
+               -4.81176e-20
             },
          (254,1): {
-               -3.34111e-18,
-               1.33822e-16
+               -7.55396e-17,
+               3.73488e-19
             },
          (255,0): {
-               9.91483e-19,
-               5.76237e-19
+               5.68639e-19,
+               6.3099e-19
             },
          (255,1): {
-               7.81129e-18,
-               -7.28316e-19
+               -1.28342e-18,
+               2.43011e-18
             },
          (256,0): {
-               1.23325e-17,
-               -2.14656e-18
+               8.07016e-18,
+               -3.07384e-19
             },
          (256,1): {
-               1.27197e-17,
-               -3.60307e-18
+               1.22804e-18,
+               -3.63525e-19
             },
          (257,0): {
-               7.01553e-17,
-               -2.46592e-18
+               2.79909e-17,
+               -1.19945e-20
             },
          (257,1): {
-               -8.6927e-19,
-               1.94784e-18
+               6.07253e-17,
+               -4.31809e-19
             },
          (258,0): {
-               5.99038e-18,
-               -9.59421e-19
+               5.23592e-18,
+               -1.3178e-19
             },
          (258,1): {
-               -1.0649e-17,
-               2.75847e-18
+               4.32638e-18,
+               2.08824e-18
             },
          (259,0): {
-               8.92857e-17,
-               2.41096e-18
+               -7.82919e-19,
+               -2.10901e-19
             },
          (259,1): {
-               -4.4898e-18,
-               8.2232e-17
+               -6.91173e-18,
+               1.55021e-18
             },
          (260,0): {
-               1.50678e-17,
-               8.23755e-19
+               -1.38189e-17,
+               7.43595e-21
             },
          (260,1): {
-               5.48539e-18,
-               1.79724e-18
+               -1.19503e-17,
+               -6.31999e-19
             },
          (261,0): {
-               3.30552e-17,
-               1.00887e-18
+               3.36659e-18,
+               1.15504e-19
             },
          (261,1): {
-               9.97303e-18,
-               -4.88612e-18
+               1.38722e-17,
+               -8.88777e-19
             },
          (262,0): {
-               6.01114e-17,
-               -1.07696e-18
+               1.86539e-17,
+               1.88328e-19
             },
          (262,1): {
-               2.37523e-18,
-               -6.43956e-18
+               -4.10081e-17,
+               -1.05128e-18
             },
          (263,0): {
-               2.8804e-17,
-               9.20197e-19
+               7.2427e-17,
+               -8.15694e-20
             },
          (263,1): {
-               -5.06094e-18,
-               -1.41203e-17
+               4.84085e-17,
+               -1.22486e-18
             },
          (264,0): {
-               7.19139e-18,
-               -9.51703e-19
+               -1.16867e-17,
+               -3.64965e-19
             },
          (264,1): {
-               -1.071e-18,
-               -9.23693e-18
+               2.86856e-17,
+               -7.01542e-19
             },
          (265,0): {
-               4.00677e-18,
-               -1.23846e-18
+               -3.71407e-18,
+               -9.42363e-20
             },
          (265,1): {
-               -1.24757e-18,
-               -9.03336e-19
+               -5.58032e-19,
+               3.42875e-18
             },
          (266,0): {
-               5.38279e-17,
-               4.63264e-19
+               -1.14372e-17,
+               -4.31026e-19
             },
          (266,1): {
-               6.39329e-18,
-               5.39658e-17
+               -2.71541e-17,
+               9.41569e-19
             },
          (267,0): {
-               -3.86133e-17,
-               -5.86571e-18
+               2.83831e-17,
+               -5.19928e-19
             },
          (267,1): {
-               7.3336e-21,
-               9.6449e-17
+               -2.35551e-16,
+               -2.07519e-18
             },
          (268,0): {
-               -9.8512e-17,
-               -3.01991e-18
+               1.53201e-17,
+               -1.38811e-19
             },
          (268,1): {
-               5.71039e-18,
-               1.83271e-17
+               -1.55398e-16,
+               -1.34591e-18
             },
          (269,0): {
-               -8.6272e-17,
-               1.81472e-18
+               4.68583e-17,
+               2.14382e-19
             },
          (269,1): {
-               1.20917e-18,
-               -1.21824e-17
+               -2.82289e-17,
+               1.37899e-18
             },
          (270,0): {
-               -1.13537e-16,
-               1.87228e-18
+               4.79183e-17,
+               -5.64664e-19
             },
          (270,1): {
-               2.8648e-18,
-               -3.57369e-18
+               3.23793e-17,
+               -6.10967e-20
             },
          (271,0): {
-               -1.30018e-16,
-               -2.64045e-18
+               3.22111e-17,
+               -8.77906e-21
             },
          (271,1): {
-               9.55223e-19,
-               2.68544e-18
+               4.03011e-17,
+               2.46518e-18
             },
          (272,0): {
-               -1.20315e-16,
-               -9.32629e-18
+               7.41326e-17,
+               7.6326e-19
             },
          (272,1): {
-               -1.42631e-17,
-               1.27047e-16
+               5.15487e-17,
+               -1.4385e-18
             },
          (273,0): {
-               -1.12128e-16,
-               1.46598e-18
+               9.62949e-17,
+               4.41815e-19
             },
          (273,1): {
-               1.74706e-18,
-               2.18457e-17
+               3.59664e-17,
+               1.57192e-18
             },
          (274,0): {
-               -1.75829e-16,
-               3.41994e-18
+               2.03931e-17,
+               2.04212e-19
             },
          (274,1): {
-               1.50064e-18,
-               1.33221e-18
+               -9.78596e-18,
+               -1.0328e-20
             },
          (275,0): {
-               -4.77807e-17,
-               7.16895e-21
+               4.0271e-17,
+               -3.37005e-19
             },
          (275,1): {
-               -1.93275e-18,
-               -4.41775e-17
+               2.69374e-17,
+               6.18662e-18
             },
          (276,0): {
-               -1.00412e-16,
-               6.62994e-19
+               6.02563e-17,
+               -1.94355e-19
             },
          (276,1): {
-               -2.005e-18,
-               2.20707e-17
+               -1.79354e-16,
+               -3.12645e-18
             },
          (277,0): {
-               -3.10176e-17,
-               2.47988e-18
+               6.24361e-17,
+               -5.81668e-19
             },
          (277,1): {
-               5.05778e-18,
-               -4.14513e-17
+               4.7473e-18,
+               -2.50054e-18
             },
          (278,0): {
-               4.23369e-17,
-               5.44579e-18
+               1.1278e-16,
+               -2.81406e-19
             },
          (278,1): {
-               -4.08457e-18,
-               1.45977e-18
+               -3.55236e-17,
+               2.87623e-18
             },
          (279,0): {
-               1.98831e-18,
-               -8.99561e-19
+               1.59305e-18,
+               1.74873e-18
             },
          (279,1): {
-               -5.5664e-18,
-               3.57461e-18
+               -1.62432e-18,
+               1.0496e-17
             },
          (280,0): {
-               2.16693e-08,
-               7.41581e-07
+               -7.41186e-07,
+               2.91325e-08
             },
          (280,1): {
-               1.73076e-05,
-               -1.89041e-05
+               -2.28619e-05,
+               -1.16057e-05
             },
          (281,0): {
-               8.30412e-07,
-               2.44052e-06
+               -2.42908e-06,
+               8.54645e-07
             },
          (281,1): {
-               -1.56102e-05,
-               1.60905e-05
+               1.96994e-05,
+               1.07274e-05
             },
          (282,0): {
-               3.73613e-08,
-               -9.84324e-07
+               9.84502e-07,
+               2.74557e-08
             },
          (282,1): {
-               -2.15153e-05,
-               2.44013e-05
+               2.94065e-05,
+               1.42443e-05
             },
          (283,0): {
-               -1.87805e-08,
-               2.41226e-09
+               -2.60176e-09,
+               -1.87489e-08
             },
          (283,1): {
-               3.41421e-07,
-               4.7011e-07
+               3.62257e-07,
+               -4.57321e-07
             },
          (284,0): {
-               5.76371e-11,
-               5.99005e-10
+               -5.97863e-10,
+               6.36432e-11
             },
          (284,1): {
-               1.19409e-08,
-               -9.56467e-09
+               -1.24849e-08,
+               -8.96741e-09
             },
          (285,0): {
-               1.14403e-11,
-               -2.46013e-12
+               2.57282e-12,
+               1.14026e-11
             },
          (285,1): {
-               -1.28111e-10,
-               -2.37831e-10
+               -1.95287e-10,
+               1.88384e-10
             },
          (286,0): {
-               -5.33703e-14,
-               -2.80962e-13
+               2.80061e-13,
+               -5.60731e-14
             },
          (286,1): {
-               -4.44318e-12,
-               2.2642e-12
+               3.39681e-12,
+               3.68437e-12
             },
          (287,0): {
-               -5.46662e-15,
-               1.49965e-15
+               -1.58788e-15,
+               -5.40974e-15
             },
          (287,1): {
-               2.46914e-14,
-               8.06615e-14
+               7.10429e-14,
+               -4.57321e-14
             },
          (288,0): {
-               8.69264e-17,
-               1.19175e-16
+               -9.64047e-17,
+               3.27941e-17
             },
          (288,1): {
-               1.3095e-15,
-               -1.56091e-19
+               -4.35626e-16,
+               -1.19587e-15
             },
          (289,0): {
-               -1.75385e-17,
-               -1.03628e-18
+               -2.17841e-17,
+               1.87577e-18
             },
          (289,1): {
-               2.41513e-18,
-               5.20638e-17
+               1.24243e-16,
+               6.97735e-18
             },
          (290,0): {
-               -6.54854e-17,
-               6.55292e-20
+               -3.91191e-17,
+               -7.88531e-20
             },
          (290,1): {
-               5.91289e-18,
-               4.54959e-19
+               1.62513e-17,
+               2.35192e-18
             },
          (291,0): {
-               -5.63575e-17,
-               -1.2807e-19
+               -4.99296e-17,
+               -1.7621e-19
             },
          (291,1): {
-               -2.22391e-19,
-               9.05457e-17
+               -1.24938e-16,
+               -4.9959e-19
             },
          (292,0): {
-               -3.35038e-17,
-               -4.68236e-19
+               -2.85969e-17,
+               -4.63651e-19
             },
          (292,1): {
-               -6.02978e-18,
-               9.13724e-17
+               -1.34722e-18,
+               -7.66283e-19
             },
          (293,0): {
-               -3.40943e-17,
-               9.00156e-20
+               -4.64512e-17,
+               -4.23129e-20
             },
          (293,1): {
-               2.24684e-20,
-               8.69311e-17
+               -1.07537e-17,
+               -2.84363e-19
             },
          (294,0): {
-               -4.47956e-18,
-               -3.35054e-19
+               -1.7822e-17,
+               -5.86752e-19
             },
          (294,1): {
-               -4.19453e-18,
-               3.67049e-17
+               -3.35255e-17,
+               -1.48704e-18
             },
          (295,0): {
-               5.90136e-17,
-               -1.38552e-19
+               -5.90029e-17,
+               -9.76084e-20
             },
          (295,1): {
-               4.02003e-19,
-               -1.82529e-17
+               -6.06038e-18,
+               1.63325e-19
             },
          (296,0): {
-               -6.21295e-18,
-               1.06776e-18
+               -9.6631e-18,
+               7.53515e-19
             },
          (296,1): {
-               2.08699e-18,
-               -6.93874e-19
+               2.02054e-17,
+               5.07606e-18
             },
          (297,0): {
-               1.63844e-17,
-               -2.84836e-20
+               2.90564e-18,
+               -4.86277e-19
             },
          (297,1): {
-               1.25553e-18,
-               1.39991e-19
+               4.13821e-18,
+               2.34116e-18
             },
          (298,0): {
-               1.00563e-16,
-               -1.62286e-18
+               6.45028e-17,
+               8.96151e-19
             },
          (298,1): {
-               6.00478e-19,
-               7.16055e-17
+               1.11737e-16,
+               3.33505e-18
             },
          (299,0): {
-               6.17975e-17,
-               -9.77028e-21
+               6.927e-17,
+               2.89724e-19
             },
          (299,1): {
-               9.81469e-19,
-               8.19192e-18
+               4.21274e-17,
+               2.15306e-18
             },
          (300,0): {
-               1.70036e-16,
-               7.63268e-19
+               3.46838e-17,
+               -6.40929e-19
             },
          (300,1): {
-               5.42016e-19,
-               -8.07875e-18
+               -1.08251e-17,
+               -4.36099e-18
             },
          (301,0): {
-               3.54955e-17,
-               4.86555e-19
+               1.23019e-17,
+               1.88758e-19
             },
          (301,1): {
-               -1.52379e-18,
-               -5.48104e-18
+               -2.16941e-17,
+               3.42841e-19
             },
          (302,0): {
-               1.43329e-16,
-               4.55548e-19
+               8.4828e-17,
+               1.11427e-19
             },
          (302,1): {
-               4.71989e-19,
-               -2.15651e-17
+               -3.16089e-17,
+               -4.55108e-19
             },
          (303,0): {
-               2.82258e-17,
-               1.64256e-20
+               3.02395e-17,
+               -3.15811e-19
             },
          (303,1): {
-               -1.03671e-18,
-               -2.18749e-18
+               2.05948e-17,
+               -1.22139e-18
             },
          (304,0): {
-               5.32786e-17,
-               7.27965e-19
+               9.87677e-18,
+               -1.6635e-20
             },
          (304,1): {
-               3.76149e-18,
-               -1.83122e-18
+               -1.50329e-17,
+               2.63846e-18
             },
          (305,0): {
-               2.40175e-17,
-               -4.37881e-19
+               -5.0974e-18,
+               -4.44679e-19
             },
          (305,1): {
-               4.31805e-20,
-               1.75657e-17
+               -8.98417e-18,
+               -4.88877e-19
             },
          (306,0): {
-               8.61734e-18,
-               1.16916e-18
+               1.32576e-17,
+               -3.27539e-19
             },
          (306,1): {
-               2.02353e-18,
-               7.44972e-18
+               -6.25316e-18,
+               -1.17337e-19
             },
          (307,0): {
-               -2.99354e-17,
-               1.47768e-18
+               1.07669e-16,
+               -5.61845e-19
             },
          (307,1): {
-               -1.77486e-18,
-               7.00481e-17
+               -7.15166e-17,
+               -9.45765e-19
             },
          (308,0): {
-               -6.2132e-17,
-               1.46648e-19
+               5.81326e-17,
+               -2.32636e-19
             },
          (308,1): {
-               -1.14757e-18,
-               1.01496e-17
+               -7.30353e-17,
+               -2.39816e-19
             },
          (309,0): {
-               -9.94901e-17,
-               3.33132e-20
+               -4.62944e-18,
+               8.98813e-20
             },
          (309,1): {
-               1.05096e-18,
-               -2.33889e-17
+               -1.82273e-17,
+               -5.05245e-19
             },
          (310,0): {
-               -1.24828e-16,
-               -1.13387e-18
+               2.19321e-17,
+               7.42736e-19
             },
          (310,1): {
-               6.6016e-19,
-               4.08624e-17
+               7.97864e-18,
+               2.07167e-18
             },
          (311,0): {
-               -7.78837e-17,
-               -5.08772e-19
+               5.12019e-17,
+               6.96705e-19
             },
          (311,1): {
-               -2.99209e-18,
-               -2.47986e-18
+               2.24901e-18,
+               -1.15081e-18
             },
          (312,0): {
-               -6.82457e-17,
-               -5.38644e-19
+               3.63857e-17,
+               -3.84881e-20
             },
          (312,1): {
-               -4.30254e-18,
-               5.56537e-18
+               1.90567e-17,
+               2.26285e-18
             },
          (313,0): {
-               -1.49329e-16,
-               -1.60078e-18
+               8.88961e-17,
+               5.13008e-19
             },
          (313,1): {
-               -5.55634e-18,
-               5.52261e-17
+               3.38481e-17,
+               1.83868e-19
             },
          (314,0): {
-               -1.86679e-16,
-               6.91693e-19
+               1.96132e-16,
+               -1.02798e-18
             },
          (314,1): {
-               5.30413e-18,
-               -1.69002e-17
+               -4.4469e-17,
+               -3.05384e-18
             },
          (315,0): {
-               -6.98075e-18,
-               1.21701e-18
+               8.05377e-18,
+               -9.71738e-20
             },
          (315,1): {
-               -6.90365e-19,
-               6.92697e-18
+               -1.08316e-17,
+               -4.40798e-18
             },
          (316,0): {
-               -2.56483e-17,
-               -1.25534e-18
+               -5.21344e-18,
+               -2.57413e-19
             },
          (316,1): {
-               -3.50327e-18,
-               -1.34086e-17
+               -5.0366e-17,
+               -3.66378e-18
             },
          (317,0): {
-               -1.07408e-16,
-               -3.29405e-18
+               1.1236e-16,
+               -5.49316e-19
             },
          (317,1): {
-               7.42797e-18,
-               -7.45228e-17
+               -4.30038e-17,
+               -4.64771e-18
             },
          (318,0): {
-               6.24208e-17,
-               -1.76135e-18
+               2.11616e-17,
+               5.45867e-19
             },
          (318,1): {
-               -1.25198e-17,
-               2.11492e-17
+               6.94235e-18,
+               -8.45988e-18
             },
          (319,0): {
-               -8.20432e-18,
-               3.80699e-18
+               9.59085e-17,
+               1.20088e-19
             },
          (319,1): {
-               -1.44228e-18,
-               1.40836e-16
+               3.14121e-16,
+               1.34877e-17
             },
          (320,0): {
-               1.14521e-09,
-               2.12208e-10
+               3.99928e-10,
+               -1.14164e-09
             },
          (320,1): {
-               2.13517e-06,
-               -2.08577e-06
+               2.63672e-06,
+               1.55497e-06
             },
          (321,0): {
-               5.14675e-09,
-               6.52948e-08
+               6.55949e-08,
+               -1.13179e-08
             },
          (321,1): {
-               1.11583e-05,
-               -1.24559e-05
+               1.60397e-05,
+               8.18751e-06
             },
          (322,0): {
-               -2.42535e-09,
-               1.63853e-10
+               -9.70056e-11,
+               2.51766e-09
             },
          (322,1): {
-               1.80189e-05,
-               -2.04947e-05
+               2.4277e-05,
+               1.20925e-05
             },
          (323,0): {
-               3.2787e-11,
-               -1.01315e-10
+               -9.89612e-11,
+               -1.55011e-11
             },
          (323,1): {
-               -3.24685e-07,
-               -3.51867e-07
+               2.54591e-07,
+               -4.01868e-07
             },
          (324,0): {
-               -1.51306e-12,
-               1.07258e-13
+               4.82506e-13,
+               1.4026e-12
             },
          (324,1): {
-               -9.65578e-09,
-               9.36669e-09
+               -1.14679e-08,
+               -6.88334e-09
             },
          (325,0): {
-               -6.31932e-14,
-               7.52826e-14
+               7.24301e-14,
+               5.14866e-14
             },
          (325,1): {
-               1.43228e-10,
-               1.85335e-10
+               -1.41273e-10,
+               1.85081e-10
             },
          (326,0): {
-               1.70406e-15,
-               7.73343e-16
+               5.06535e-16,
+               -1.71149e-15
             },
          (326,1): {
-               3.64176e-12,
-               -2.75757e-12
+               3.58391e-12,
+               2.79235e-12
             },
          (327,0): {
-               1.24901e-18,
-               -4.57765e-17
+               -8.88864e-17,
+               -7.30286e-17
             },
          (327,1): {
-               -3.7666e-14,
-               -6.59682e-14
+               5.38658e-14,
+               -5.31836e-14
             },
          (328,0): {
-               2.97313e-17,
-               -5.40558e-18
+               -2.13007e-17,
+               1.63934e-18
             },
          (328,1): {
-               -1.13074e-15,
-               5.81938e-16
+               -8.0119e-16,
+               -9.43697e-16
             },
          (329,0): {
-               -7.0493e-18,
-               -2.17529e-18
+               5.88676e-18,
+               -5.04486e-19
             },
          (329,1): {
-               -1.06774e-18,
-               1.0142e-17
+               -2.28251e-17,
+               1.14091e-17
             },
          (330,0): {
-               1.13932e-16,
-               -1.00358e-19
+               -6.9181e-17,
+               -2.99869e-19
             },
          (330,1): {
-               3.96835e-18,
-               -4.15602e-17
+               3.84082e-17,
+               5.80451e-19
             },
          (331,0): {
-               5.37715e-17,
-               3.20214e-18
+               2.69744e-17,
+               3.59089e-19
             },
          (331,1): {
-               7.91241e-18,
-               -2.91628e-17
+               1.17754e-17,
+               1.37638e-18
             },
          (332,0): {
-               3.44604e-17,
-               9.07816e-19
+               1.34702e-17,
+               1.18718e-19
             },
          (332,1): {
-               4.8196e-18,
-               3.22888e-17
+               1.09721e-16,
+               9.91105e-19
             },
          (333,0): {
-               9.30864e-17,
-               -7.72752e-19
+               -9.15514e-18,
+               2.62364e-20
             },
          (333,1): {
-               -4.65867e-18,
-               3.61233e-17
+               1.50713e-17,
+               1.40372e-18
             },
          (334,0): {
-               1.67068e-16,
-               -2.84093e-18
+               -4.00724e-17,
+               7.40023e-19
             },
          (334,1): {
-               -5.88375e-18,
-               -1.47214e-17
+               -2.27178e-17,
+               8.45476e-19
             },
          (335,0): {
-               1.30187e-16,
-               -2.11717e-18
+               3.45489e-17,
+               8.90793e-20
             },
          (335,1): {
-               1.48293e-18,
-               -8.03954e-17
+               -5.77755e-18,
+               -2.67416e-18
             },
          (336,0): {
-               5.24791e-17,
-               1.65901e-18
+               -1.056e-17,
+               -2.67273e-19
             },
          (336,1): {
-               8.61378e-18,
-               -1.55378e-17
+               -3.50615e-18,
+               -1.76808e-18
             },
          (337,0): {
-               1.0533e-18,
-               -1.82172e-19
+               1.39813e-17,
+               -2.61154e-19
             },
          (337,1): {
-               8.30457e-19,
-               -3.61772e-18
+               1.5486e-18,
+               3.64631e-19
             },
          (338,0): {
-               9.05534e-18,
-               -3.57969e-19
+               1.21452e-18,
+               -1.27606e-20
             },
          (338,1): {
-               -1.17543e-18,
-               5.52768e-18
+               1.05571e-17,
+               3.77917e-19
             },
          (339,0): {
-               1.00498e-17,
-               -4.79005e-19
+               3.3331e-18,
+               2.34408e-20
             },
          (339,1): {
-               -1.28687e-18,
-               2.96275e-18
+               4.56433e-19,
+               -1.02266e-19
             },
          (340,0): {
-               -2.28847e-18,
-               -5.35992e-19
+               -1.57225e-18,
+               -8.10071e-20
             },
          (340,1): {
-               -1.60723e-18,
-               2.37467e-18
+               -4.57877e-18,
+               -1.69428e-19
             },
          (341,0): {
-               5.96729e-18,
-               -3.35665e-18
+               -7.32952e-18,
+               -1.03612e-20
             },
          (341,1): {
-               -4.19561e-18,
-               1.28259e-17
+               -1.38084e-17,
+               -1.74321e-19
             },
          (342,0): {
-               -3.35761e-18,
-               1.36937e-18
+               2.21155e-18,
+               -6.66482e-19
             },
          (342,1): {
-               -2.37943e-19,
-               3.13967e-18
+               1.18943e-18,
+               -1.32433e-18
             },
          (343,0): {
-               -1.14085e-16,
-               -4.3574e-19
+               5.82424e-17,
+               -1.49288e-18
             },
          (343,1): {
-               8.03682e-18,
-               -5.05314e-18
+               -7.92016e-17,
+               -2.8717e-18
             },
          (344,0): {
-               -1.46529e-16,
-               -5.59325e-18
+               4.7524e-17,
+               -2.77215e-19
             },
          (344,1): {
-               1.0017e-18,
-               1.64809e-18
+               5.99942e-18,
+               4.66371e-19
             },
          (345,0): {
-               -1.48712e-16,
-               2.8496e-18
+               7.22026e-17,
+               4.52867e-19
             },
          (345,1): {
-               -3.48816e-18,
-               1.37336e-17
+               9.32104e-17,
+               2.64003e-18
             },
          (346,0): {
-               -6.45965e-17,
-               -5.90962e-18
+               3.49659e-17,
+               1.05742e-18
             },
          (346,1): {
-               -5.0601e-18,
-               3.78845e-17
+               -2.04176e-17,
+               -1.142e-19
             },
          (347,0): {
-               -2.86993e-17,
-               1.8386e-18
+               1.58492e-17,
+               5.98233e-19
             },
          (347,1): {
-               -9.60082e-20,
-               3.56928e-18
+               3.74682e-18,
+               -6.24482e-19
             },
          (348,0): {
-               -2.50236e-16,
-               5.38246e-18
+               1.03246e-16,
+               -1.89892e-20
             },
          (348,1): {
-               1.36006e-18,
-               -2.36278e-18
+               -1.3935e-17,
+               2.40216e-19
             },
          (349,0): {
-               5.25125e-18,
-               -2.11833e-18
+               1.68098e-17,
+               4.94371e-19
             },
          (349,1): {
-               -8.04852e-19,
-               4.52154e-18
+               -2.87653e-17,
+               1.19994e-19
             },
          (350,0): {
-               -4.79162e-17,
-               1.38089e-18
+               2.86944e-17,
+               -1.05298e-19
             },
          (350,1): {
-               5.7103e-19,
-               -4.04789e-17
+               -8.38455e-17,
+               -2.26622e-18
             },
          (351,0): {
-               1.55061e-17,
-               -1.75267e-18
+               6.94458e-17,
+               1.56943e-19
             },
          (351,1): {
-               8.54168e-18,
-               -6.12383e-17
+               -5.34365e-17,
+               -9.74195e-18
             },
          (352,0): {
-               1.2412e-16,
-               1.40378e-18
+               1.96395e-16,
+               -6.19027e-19
             },
          (352,1): {
-               -3.91604e-18,
-               6.4617e-18
+               -6.78818e-17,
+               2.6864e-18
             },
          (353,0): {
-               6.88089e-17,
-               2.49018e-18
+               2.79872e-17,
+               -3.16523e-19
             },
          (353,1): {
-               -1.2036e-17,
-               1.01502e-16
+               1.59687e-16,
+               4.19065e-18
             },
          (354,0): {
-               1.24551e-16,
-               4.41389e-18
+               1.08116e-16,
+               -2.98085e-19
             },
          (354,1): {
-               2.56768e-18,
-               -6.74695e-17
+               1.86218e-16,
+               1.39616e-17
             },
          (355,0): {
-               6.29797e-17,
-               1.11511e-17
+               3.94591e-17,
+               -1.26252e-19
             },
          (355,1): {
-               2.24488e-17,
-               -1.08691e-17
+               7.79794e-17,
+               1.54496e-17
             },
          (356,0): {
-               1.02343e-17,
-               1.18714e-17
+               2.00481e-16,
+               -3.92301e-18
             },
          (356,1): {
-               -2.12987e-17,
-               2.00185e-16
+               -3.57999e-16,
+               -1.99877e-17
             },
          (357,0): {
-               -1.21364e-16,
-               -1.03073e-18
+               2.66306e-16,
+               6.57487e-19
             },
          (357,1): {
-               1.31394e-19,
-               2.50787e-16
+               -4.259e-16,
+               -1.95425e-17
             },
          (358,0): {
-               -1.98724e-16,
-               -7.71655e-18
+               1.76277e-16,
+               3.30354e-19
             },
          (358,1): {
-               6.81693e-18,
-               1.49558e-16
+               2.69138e-17,
+               6.75905e-17
             },
          (359,0): {
-               -1.43113e-16,
-               -5.82398e-18
+               5.81676e-17,
+               -2.5299e-19
             },
          (359,1): {
-               -2.3669e-17,
-               6.63679e-16
+               -7.1165e-16,
+               -7.95804e-17
             },
          (360,0): {
-               8.96891e-06,
-               2.98902e-06
+               -9.08073e-06,
+               -2.99718e-06
             },
          (360,1): {
-               -1.44333e-09,
-               -2.59404e-09
+               -2.0797e-09,
+               -2.15503e-09
             },
          (361,0): {
-               -0.00029103,
-               -1.87197e-06
+               0.000291502,
+               2.28552e-06
             },
          (361,1): {
-               -6.29667e-08,
-               8.0814e-08
+               -3.92041e-08,
+               9.37892e-08
             },
          (362,0): {
-               8.9041e-06,
-               4.19979e-06
+               -9.34452e-06,
+               -4.22221e-06
             },
          (362,1): {
-               3.94515e-09,
-               4.89796e-10
+               3.89802e-09,
+               -5.45348e-10
             },
          (363,0): {
-               7.59535e-08,
-               -1.55468e-07
+               -7.40186e-08,
+               1.63172e-07
             },
          (363,1): {
-               1.42769e-10,
-               -2.11739e-10
+               8.29239e-11,
+               -2.41881e-10
             },
          (364,0): {
-               -4.25534e-09,
-               -1.05085e-09
+               4.48888e-09,
+               1.01315e-09
             },
          (364,1): {
-               -3.92464e-12,
-               -2.8936e-12
+               -4.54935e-12,
+               -1.78014e-12
             },
          (365,0): {
-               -1.69714e-11,
-               7.23432e-11
+               1.54495e-11,
+               -7.64409e-11
             },
          (365,1): {
-               -8.72555e-14,
-               9.62991e-14
+               -5.87089e-14,
+               1.14722e-13
             },
          (366,0): {
-               1.67595e-12,
-               2.46014e-13
+               -1.77497e-12,
+               -2.16698e-13
             },
          (366,1): {
-               1.79374e-15,
-               1.69998e-15
+               2.16221e-15,
+               1.14138e-15
             },
          (367,0): {
-               3.15255e-15,
-               -2.98544e-14
+               -2.37047e-15,
+               3.16494e-14
             },
          (367,1): {
-               2.35345e-17,
-               2.51254e-17
+               9.16437e-18,
+               -3.22155e-17
             },
          (368,0): {
-               -5.88522e-16,
-               -3.79048e-17
+               6.99175e-16,
+               2.0826e-17
             },
          (368,1): {
-               -2.92288e-19,
-               2.99368e-17
+               1.79525e-17,
+               -1.24687e-19
             },
          (369,0): {
-               -1.68886e-17,
-               1.07871e-17
+               -3.81349e-17,
+               -1.19841e-17
             },
          (369,1): {
-               2.26189e-18,
-               -4.20017e-17
+               2.25324e-17,
+               1.02741e-19
             },
          (370,0): {
-               -1.1755e-17,
-               4.54668e-19
+               3.28434e-17,
+               1.87499e-19
             },
          (370,1): {
-               -1.79466e-18,
-               -1.26251e-17
+               4.87999e-17,
+               2.34551e-18
             },
          (371,0): {
-               4.565e-17,
-               6.60579e-20
+               5.30471e-17,
+               3.77588e-20
             },
          (371,1): {
-               -1.8523e-18,
-               7.44168e-18
+               1.01724e-16,
+               1.54345e-18
             },
          (372,0): {
-               8.20854e-17,
-               7.3965e-19
+               6.93487e-17,
+               1.61779e-19
             },
          (372,1): {
-               -2.89766e-18,
-               -9.02554e-18
+               4.93377e-17,
+               1.83774e-18
             },
          (373,0): {
-               1.0916e-16,
-               5.41583e-19
+               8.44618e-18,
+               2.44826e-19
             },
          (373,1): {
-               9.76675e-19,
-               1.03226e-18
+               -4.7484e-18,
+               -1.12328e-18
             },
          (374,0): {
-               1.08758e-16,
-               -2.66996e-19
+               -4.70205e-18,
+               4.14984e-19
             },
          (374,1): {
-               7.29979e-19,
-               -1.83304e-17
+               1.30036e-17,
+               -1.06041e-18
             },
          (375,0): {
-               1.46145e-16,
-               3.75146e-20
+               2.22656e-17,
+               3.9022e-19
             },
          (375,1): {
-               6.28434e-19,
-               -4.93191e-17
+               -1.08933e-16,
+               -2.59908e-19
             },
          (376,0): {
-               -1.85023e-17,
-               -3.02712e-19
+               1.29716e-17,
+               -8.26742e-19
             },
          (376,1): {
-               -1.5814e-18,
-               3.07578e-17
+               3.13917e-18,
+               4.13173e-18
             },
          (377,0): {
-               6.92945e-18,
-               -3.2468e-19
+               3.90035e-18,
+               -6.24544e-19
             },
          (377,1): {
-               5.73799e-20,
-               9.18074e-18
+               2.58147e-17,
+               -6.28245e-20
             },
          (378,0): {
-               -4.67989e-18,
-               8.2144e-19
+               -5.82555e-18,
+               9.34731e-19
             },
          (378,1): {
-               1.64269e-18,
-               2.48698e-17
+               -1.21837e-17,
+               6.18772e-20
             },
          (379,0): {
-               1.67923e-17,
-               7.50546e-19
+               7.59415e-18,
+               -4.25305e-19
             },
          (379,1): {
-               2.60935e-19,
-               2.29695e-17
+               -3.00187e-17,
+               1.70373e-18
             },
          (380,0): {
-               -4.92365e-18,
-               -1.76398e-18
+               1.84523e-17,
+               3.84416e-19
             },
          (380,1): {
-               4.85079e-19,
-               1.28005e-17
+               -4.40169e-17,
+               -4.27169e-18
             },
          (381,0): {
-               -2.05661e-17,
-               1.49862e-18
+               1.33136e-17,
+               -6.28157e-19
             },
          (381,1): {
-               -2.846e-19,
-               -9.12791e-18
+               8.45752e-18,
+               -3.61954e-18
             },
          (382,0): {
-               -9.86355e-17,
-               9.74218e-19
+               6.31192e-17,
+               -2.78895e-19
             },
          (382,1): {
-               -5.41478e-20,
-               3.58615e-17
+               -1.08721e-16,
+               -6.69647e-19
             },
          (383,0): {
-               -5.39292e-17,
-               -1.20513e-18
+               1.76103e-17,
+               5.37124e-19
             },
          (383,1): {
-               -6.30082e-20,
-               -5.95314e-18
+               2.43925e-17,
+               3.23347e-19
             },
          (384,0): {
-               -1.62653e-16,
-               -3.47812e-19
+               3.8986e-17,
+               4.69304e-19
             },
          (384,1): {
-               -2.8542e-18,
-               2.20609e-18
+               -1.57703e-17,
+               -2.90029e-18
             },
          (385,0): {
-               -2.45285e-17,
-               -3.04484e-19
+               2.02694e-17,
+               -6.09241e-20
             },
          (385,1): {
-               -1.68365e-18,
-               -1.00432e-17
+               5.95013e-19,
+               1.27072e-18
             },
          (386,0): {
-               -1.64376e-16,
-               1.12798e-20
+               5.19158e-17,
+               -2.21456e-19
             },
          (386,1): {
-               1.28827e-19,
-               6.81962e-17
+               7.45035e-18,
+               -5.58314e-19
             },
          (387,0): {
-               1.35949e-17,
-               4.77916e-19
+               -4.21903e-18,
+               -1.92819e-19
             },
          (387,1): {
-               4.44441e-18,
-               -1.30568e-17
+               -1.45074e-17,
+               9.81313e-19
             },
          (388,0): {
-               -1.38483e-17,
-               -8.94023e-19
+               1.60435e-17,
+               5.41051e-19
             },
          (388,1): {
-               -8.61212e-19,
-               -9.5216e-18
+               -2.11074e-17,
+               4.81043e-19
             },
          (389,0): {
-               -8.44993e-18,
-               -1.25901e-18
+               2.80793e-17,
+               -2.47918e-19
             },
          (389,1): {
-               -7.57498e-19,
-               -6.27774e-18
+               -8.10517e-17,
+               -6.88935e-19
             },
          (390,0): {
-               -4.29251e-17,
-               1.26693e-18
+               4.61781e-17,
+               -1.37211e-19
             },
          (390,1): {
-               -1.58295e-19,
-               -5.69271e-17
+               -1.28657e-16,
+               1.64893e-19
             },
          (391,0): {
-               9.84638e-19,
-               2.09166e-18
+               -7.81274e-18,
+               3.03599e-19
             },
          (391,1): {
-               -2.26389e-18,
-               7.0452e-18
+               1.25533e-17,
+               4.84154e-18
             },
          (392,0): {
-               5.35023e-18,
-               -1.14336e-18
+               4.18892e-18,
+               -1.47336e-18
             },
          (392,1): {
-               -4.67519e-18,
-               -4.77503e-17
+               6.69285e-17,
+               -1.0291e-17
             },
          (393,0): {
-               1.61242e-16,
-               1.77016e-18
+               1.42937e-16,
+               -5.03542e-19
             },
          (393,1): {
-               -3.02012e-18,
-               -2.36471e-17
+               2.83281e-16,
+               5.23494e-18
             },
          (394,0): {
-               6.89904e-17,
-               7.39993e-19
+               1.57176e-16,
+               4.2356e-19
             },
          (394,1): {
-               7.81196e-18,
-               -4.55295e-17
+               1.5273e-16,
+               3.92005e-18
             },
          (395,0): {
-               -1.42477e-17,
-               1.36374e-18
+               1.21609e-16,
+               1.22007e-19
             },
          (395,1): {
-               -3.91335e-18,
-               1.67405e-16
+               -2.36709e-16,
+               -2.15608e-17
             },
          (396,0): {
-               -1.07518e-16,
-               1.29979e-18
+               1.83627e-16,
+               5.61345e-20
             },
          (396,1): {
-               -1.33642e-17,
-               1.1632e-16
+               -1.66555e-16,
+               -1.36598e-17
             },
          (397,0): {
-               -1.4314e-16,
-               2.66118e-18
+               9.9477e-17,
+               -1.10334e-19
             },
          (397,1): {
-               -3.34907e-17,
-               -2.94673e-17
+               7.50766e-17,
+               -2.008e-17
             },
          (398,0): {
-               -3.28666e-16,
-               2.49117e-17
+               1.03772e-16,
+               -4.36318e-18
             },
          (398,1): {
-               -1.44043e-16,
-               -8.34216e-17
+               -1.52955e-16,
+               -7.77117e-17
             },
          (399,0): {
-               -9.93386e-16,
-               -1.09977e-17
+               4.33634e-16,
+               3.73596e-18
             },
          (399,1): {
-               5.1914e-17,
-               -2.41208e-16
+               -2.86156e-16,
+               2.94624e-17
             }
          }
       }
    }
    GROUP "__dicts" {
       GROUP "system_params" {
          ATTRIBUTE "EC" {
@@ -3397,19 +3397,19 @@
    }
    GROUP "__objects" {
    }
    DATASET "energy_table" {
       DATATYPE  H5T_STD_I64LE
       DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
       DATA {
-      (0): -6741523309743639754
+      (0): -5522267930686899526
       }
    }
    DATASET "state_table" {
       DATATYPE  H5T_STD_I64LE
       DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
       DATA {
-      (0): 7040608736081761962
+      (0): 2543333760430554360
       }
    }
 }
 }
```

### Comparing `scqubits-3.1.0/scqubits/tests/data/transmon_2.hdf5` & `scqubits-3.1.1/scqubits/tests/data/transmon_2.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/data/transmon_4.hdf5` & `scqubits-3.1.1/scqubits/tests/data/transmon_4.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/data/zeropi-test.hdf5` & `scqubits-3.1.1/scqubits/tests/data/zeropi-test.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/data/zeropi_1.hdf5` & `scqubits-3.1.1/scqubits/tests/data/zeropi_1.hdf5`

 * *Files 14% similar despite different names*

#### h5dump {}

```diff
@@ -1,21 +1,31 @@
-HDF5 "/tmp/diffoscope_t77nf7_l_/tmp7aiew04k_TarContainer/0/84.hdf5" {
+HDF5 "/tmp/diffoscope_t77nf7_l_/tmp8yvfas64_TarContainer/0/83.hdf5" {
 GROUP "/" {
    ATTRIBUTE "__type" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
       }
       DATASPACE  SCALAR
       DATA {
       (0): "SpectrumData"
       }
    }
+   GROUP "__data" {
+      DATASET "4953642392006230098" {
+         DATATYPE  H5T_IEEE_F64LE
+         DATASPACE  SIMPLE { ( 7 ) / ( 7 ) }
+         DATA {
+         (0): 0.458796, 0.489459, 0.501329, 0.51865, 0.530471, 0.54609,
+         (6): 0.557581
+         }
+      }
+   }
    GROUP "__dicts" {
       GROUP "system_params" {
          ATTRIBUTE "EC" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
             (0): 0.00100203
@@ -71,28 +81,47 @@
          ATTRIBUTE "flux" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
             (0): 0.23
             }
          }
+         ATTRIBUTE "id_str" {
+            DATATYPE  H5T_STRING {
+               STRSIZE H5T_VARIABLE;
+               STRPAD H5T_STR_NULLTERM;
+               CSET H5T_CSET_UTF8;
+               CTYPE H5T_C_S1;
+            }
+            DATASPACE  SCALAR
+            DATA {
+            (0): "ZeroPi_1"
+            }
+         }
          ATTRIBUTE "ncut" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
             (0): 30
             }
          }
          ATTRIBUTE "ng" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
             (0): 0.1
             }
          }
+         ATTRIBUTE "truncated_dim" {
+            DATATYPE  H5T_STD_I32LE
+            DATASPACE  SCALAR
+            DATA {
+            (0): 6
+            }
+         }
          GROUP "__objects" {
             GROUP "grid" {
                ATTRIBUTE "__type" {
                   DATATYPE  H5T_STRING {
                      STRSIZE H5T_VARIABLE;
                      STRPAD H5T_STR_NULLTERM;
                      CSET H5T_CSET_UTF8;
@@ -129,15 +158,15 @@
             }
          }
       }
    }
    GROUP "__objects" {
    }
    DATASET "energy_table" {
-      DATATYPE  H5T_IEEE_F64LE
-      DATASPACE  SIMPLE { ( 7 ) / ( 7 ) }
+      DATATYPE  H5T_STD_I64LE
+      DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
       DATA {
-      (0): 0.458795, 0.489459, 0.501328, 0.51865, 0.530471, 0.54609, 0.557581
+      (0): 4953642392006230098
       }
    }
 }
 }
```

### Comparing `scqubits-3.1.0/scqubits/tests/data/zeropi_5.hdf5` & `scqubits-3.1.1/scqubits/tests/data/cos2phiqubit_5.hdf5`

 * *Files 13% similar despite different names*

#### h5dump {}

```diff
@@ -1,61 +1,460 @@
-HDF5 "/tmp/diffoscope_t77nf7_l_/tmp7aiew04k_TarContainer/0/87.hdf5" {
+HDF5 "/tmp/diffoscope_t77nf7_l_/tmp8yvfas64_TarContainer/0/67.hdf5" {
 GROUP "/" {
    ATTRIBUTE "__type" {
       DATATYPE  H5T_STRING {
          STRSIZE H5T_VARIABLE;
          STRPAD H5T_STR_NULLTERM;
          CSET H5T_CSET_UTF8;
          CTYPE H5T_C_S1;
       }
       DATASPACE  SCALAR
       DATA {
       (0): "DataStore"
       }
    }
-   ATTRIBUTE "param_name" {
-      DATATYPE  H5T_STRING {
-         STRSIZE H5T_VARIABLE;
-         STRPAD H5T_STR_NULLTERM;
-         CSET H5T_CSET_UTF8;
-         CTYPE H5T_C_S1;
-      }
-      DATASPACE  SCALAR
-      DATA {
-      (0): ""
+   GROUP "__data" {
+      DATASET "-2016379437075879995" {
+         DATATYPE  H5T_COMPOUND {
+            H5T_IEEE_F64LE "r";
+            H5T_IEEE_F64LE "i";
+         }
+         DATASPACE  SIMPLE { ( 10, 10 ) / ( 10, 10 ) }
+         DATA {
+         (0,0): {
+               0.299926,
+               4.92318e-19
+            },
+         (0,1): {
+               0.516247,
+               1.01823
+            },
+         (0,2): {
+               0.000965611,
+               1.16177e-06
+            },
+         (0,3): {
+               0.000153038,
+               -0.000386591
+            },
+         (0,4): {
+               5.46105e-05,
+               -7.21952e-05
+            },
+         (0,5): {
+               4.74092e-06,
+               4.48441e-06
+            },
+         (0,6): {
+               1.2976e-05,
+               4.72693e-06
+            },
+         (0,7): {
+               9.08831e-06,
+               4.42239e-05
+            },
+         (0,8): {
+               4.58012e-05,
+               -0.000423773
+            },
+         (0,9): {
+               -0.000187267,
+               -0.000502794
+            },
+         (1,0): {
+               0.516247,
+               -1.01823
+            },
+         (1,1): {
+               0.298983,
+               1.49247e-18
+            },
+         (1,2): {
+               -1.26048,
+               -1.00698
+            },
+         (1,3): {
+               0.000540986,
+               -0.00243927
+            },
+         (1,4): {
+               0.000465638,
+               -0.00171066
+            },
+         (1,5): {
+               0.000302691,
+               -0.000313541
+            },
+         (1,6): {
+               8.89835e-05,
+               -0.000265563
+            },
+         (1,7): {
+               9.20035e-06,
+               -0.000477569
+            },
+         (1,8): {
+               6.88034e-05,
+               -0.000171046
+            },
+         (1,9): {
+               0.000101017,
+               -0.000490496
+            },
+         (2,0): {
+               0.000965611,
+               -1.16177e-06
+            },
+         (2,1): {
+               -1.26048,
+               1.00698
+            },
+         (2,2): {
+               0.293317,
+               -1.36213e-18
+            },
+         (2,3): {
+               1.94363,
+               0.32748
+            },
+         (2,4): {
+               -0.00116899,
+               0.0071061
+            },
+         (2,5): {
+               -0.00417262,
+               0.00443228
+            },
+         (2,6): {
+               -0.00279374,
+               0.000111553
+            },
+         (2,7): {
+               -0.00198505,
+               0.00195546
+            },
+         (2,8): {
+               0.00186488,
+               -0.000113803
+            },
+         (2,9): {
+               0.00193468,
+               -0.00134133
+            },
+         (3,0): {
+               0.000153038,
+               0.000386591
+            },
+         (3,1): {
+               0.000540986,
+               0.00243927
+            },
+         (3,2): {
+               1.94363,
+               -0.32748
+            },
+         (3,3): {
+               0.273101,
+               -4.61433e-17
+            },
+         (3,4): {
+               1.25021,
+               1.88325
+            },
+         (3,5): {
+               -0.016298,
+               0.00878247
+            },
+         (3,6): {
+               -0.0123719,
+               -0.019131
+            },
+         (3,7): {
+               -0.00487502,
+               -0.00629242
+            },
+         (3,8): {
+               0.00103539,
+               0.0103952
+            },
+         (3,9): {
+               0.00822643,
+               0.00705879
+            },
+         (4,0): {
+               5.46105e-05,
+               7.21952e-05
+            },
+         (4,1): {
+               0.000465638,
+               0.00171066
+            },
+         (4,2): {
+               -0.00116899,
+               -0.0071061
+            },
+         (4,3): {
+               1.25021,
+               -1.88325
+            },
+         (4,4): {
+               0.226207,
+               1.21294e-18
+            },
+         (4,5): {
+               1.00803,
+               2.27599
+            },
+         (4,6): {
+               -0.0272672,
+               -0.0609807
+            },
+         (4,7): {
+               -0.00264755,
+               -0.0693742
+            },
+         (4,8): {
+               -0.013939,
+               0.0504656
+            },
+         (4,9): {
+               0.000860131,
+               0.0223785
+            },
+         (5,0): {
+               4.74092e-06,
+               -4.48441e-06
+            },
+         (5,1): {
+               0.000302691,
+               0.000313541
+            },
+         (5,2): {
+               -0.00417262,
+               -0.00443228
+            },
+         (5,3): {
+               -0.016298,
+               -0.00878247
+            },
+         (5,4): {
+               1.00803,
+               -2.27599
+            },
+         (5,5): {
+               0.155241,
+               -3.85564e-18
+            },
+         (5,6): {
+               -0.821331,
+               2.21055
+            },
+         (5,7): {
+               0.118279,
+               -1.21192
+            },
+         (5,8): {
+               -0.0553382,
+               0.113912
+            },
+         (5,9): {
+               -0.054119,
+               0.132703
+            },
+         (6,0): {
+               1.2976e-05,
+               -4.72693e-06
+            },
+         (6,1): {
+               8.89835e-05,
+               0.000265563
+            },
+         (6,2): {
+               -0.00279374,
+               -0.000111553
+            },
+         (6,3): {
+               -0.0123719,
+               0.019131
+            },
+         (6,4): {
+               -0.0272672,
+               0.0609807
+            },
+         (6,5): {
+               -0.821331,
+               -2.21055
+            },
+         (6,6): {
+               0.132822,
+               -3.67443e-18
+            },
+         (6,7): {
+               0.23893,
+               0.54013
+            },
+         (6,8): {
+               0.234506,
+               -1.28062
+            },
+         (6,9): {
+               0.527156,
+               1.85718
+            },
+         (7,0): {
+               9.08831e-06,
+               -4.42239e-05
+            },
+         (7,1): {
+               9.20035e-06,
+               0.000477569
+            },
+         (7,2): {
+               -0.00198505,
+               -0.00195546
+            },
+         (7,3): {
+               -0.00487502,
+               0.00629242
+            },
+         (7,4): {
+               -0.00264755,
+               0.0693742
+            },
+         (7,5): {
+               0.118279,
+               1.21192
+            },
+         (7,6): {
+               0.23893,
+               -0.54013
+            },
+         (7,7): {
+               0.24586,
+               5.69444e-18
+            },
+         (7,8): {
+               -0.851309,
+               1.5953
+            },
+         (7,9): {
+               -0.0737944,
+               -0.407129
+            },
+         (8,0): {
+               4.58012e-05,
+               0.000423773
+            },
+         (8,1): {
+               6.88034e-05,
+               0.000171046
+            },
+         (8,2): {
+               0.00186488,
+               0.000113803
+            },
+         (8,3): {
+               0.00103539,
+               -0.0103952
+            },
+         (8,4): {
+               -0.013939,
+               -0.0504656
+            },
+         (8,5): {
+               -0.0553382,
+               -0.113912
+            },
+         (8,6): {
+               0.234506,
+               1.28062
+            },
+         (8,7): {
+               -0.851309,
+               -1.5953
+            },
+         (8,8): {
+               0.125001,
+               -3.39141e-18
+            },
+         (8,9): {
+               0.365791,
+               0.378203
+            },
+         (9,0): {
+               -0.000187267,
+               0.000502794
+            },
+         (9,1): {
+               0.000101017,
+               0.000490496
+            },
+         (9,2): {
+               0.00193468,
+               0.00134133
+            },
+         (9,3): {
+               0.00822643,
+               -0.00705879
+            },
+         (9,4): {
+               0.000860131,
+               -0.0223785
+            },
+         (9,5): {
+               -0.054119,
+               -0.132703
+            },
+         (9,6): {
+               0.527156,
+               -1.85718
+            },
+         (9,7): {
+               -0.0737944,
+               0.407129
+            },
+         (9,8): {
+               0.365791,
+               -0.378203
+            },
+         (9,9): {
+               0.19337,
+               -1.01921e-17
+            }
+         }
       }
    }
    GROUP "__dicts" {
       GROUP "system_params" {
          ATTRIBUTE "EC" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.00100203
+            (0): 0.04
             }
          }
          ATTRIBUTE "ECJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.49375
+            (0): 2.2
             }
          }
          ATTRIBUTE "EJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.253165
+            (0): 15
             }
          }
          ATTRIBUTE "EL" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.01
+            (0): 1.2
             }
          }
          ATTRIBUTE "__type" {
             DATATYPE  H5T_STRING {
                STRSIZE H5T_VARIABLE;
                STRPAD H5T_STR_NULLTERM;
                CSET H5T_CSET_UTF8;
@@ -66,492 +465,93 @@
             (0): "dict"
             }
          }
          ATTRIBUTE "dCJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.04
+            (0): 0.2
             }
          }
          ATTRIBUTE "dEJ" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.03
+            (0): 0.3
+            }
+         }
+         ATTRIBUTE "dL" {
+            DATATYPE  H5T_IEEE_F64LE
+            DATASPACE  SCALAR
+            DATA {
+            (0): 0.1
             }
          }
          ATTRIBUTE "flux" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.23
+            (0): 0.2
+            }
+         }
+         ATTRIBUTE "id_str" {
+            DATATYPE  H5T_STRING {
+               STRSIZE H5T_VARIABLE;
+               STRPAD H5T_STR_NULLTERM;
+               CSET H5T_CSET_UTF8;
+               CTYPE H5T_C_S1;
+            }
+            DATASPACE  SCALAR
+            DATA {
+            (0): "Cos2PhiQubit_1"
             }
          }
          ATTRIBUTE "ncut" {
             DATATYPE  H5T_STD_I32LE
             DATASPACE  SCALAR
             DATA {
-            (0): 30
+            (0): 7
             }
          }
          ATTRIBUTE "ng" {
             DATATYPE  H5T_IEEE_F64LE
             DATASPACE  SCALAR
             DATA {
-            (0): 0.1
+            (0): 0.3
             }
          }
-         GROUP "__objects" {
-            GROUP "grid" {
-               ATTRIBUTE "__type" {
-                  DATATYPE  H5T_STRING {
-                     STRSIZE H5T_VARIABLE;
-                     STRPAD H5T_STR_NULLTERM;
-                     CSET H5T_CSET_UTF8;
-                     CTYPE H5T_C_S1;
-                  }
-                  DATASPACE  SCALAR
-                  DATA {
-                  (0): "Grid1d"
-                  }
-               }
-               ATTRIBUTE "max_val" {
-                  DATATYPE  H5T_IEEE_F64LE
-                  DATASPACE  SCALAR
-                  DATA {
-                  (0): 18.8496
-                  }
-               }
-               ATTRIBUTE "min_val" {
-                  DATATYPE  H5T_IEEE_F64LE
-                  DATASPACE  SCALAR
-                  DATA {
-                  (0): -18.8496
-                  }
-               }
-               ATTRIBUTE "pt_count" {
-                  DATATYPE  H5T_STD_I32LE
-                  DATASPACE  SCALAR
-                  DATA {
-                  (0): 200
-                  }
-               }
-               GROUP "__objects" {
-               }
+         ATTRIBUTE "phi_cut" {
+            DATATYPE  H5T_STD_I32LE
+            DATASPACE  SCALAR
+            DATA {
+            (0): 7
+            }
+         }
+         ATTRIBUTE "truncated_dim" {
+            DATATYPE  H5T_STD_I32LE
+            DATASPACE  SCALAR
+            DATA {
+            (0): 6
+            }
+         }
+         ATTRIBUTE "zeta_cut" {
+            DATATYPE  H5T_STD_I32LE
+            DATASPACE  SCALAR
+            DATA {
+            (0): 30
             }
          }
+         GROUP "__objects" {
+         }
       }
    }
    GROUP "__objects" {
    }
    DATASET "matrixelem_table" {
-      DATATYPE  H5T_COMPOUND {
-         H5T_IEEE_F64LE "r";
-         H5T_IEEE_F64LE "i";
-      }
-      DATASPACE  SIMPLE { ( 10, 10 ) / ( 10, 10 ) }
+      DATATYPE  H5T_STD_I64LE
+      DATASPACE  SIMPLE { ( 1 ) / ( 1 ) }
       DATA {
-      (0,0): {
-            -0.1,
-            -9.92617e-24
-         },
-      (0,1): {
-            1.93186,
-            0.315386
-         },
-      (0,2): {
-            -4.54204e-06,
-            1.51803e-07
-         },
-      (0,3): {
-            0.000911647,
-            0.000117906
-         },
-      (0,4): {
-            -2.24147e-06,
-            -5.44984e-05
-         },
-      (0,5): {
-            -0.0320144,
-            0.0468737
-         },
-      (0,6): {
-            -6.19999e-05,
-            2.86056e-05
-         },
-      (0,7): {
-            7.41788e-05,
-            -4.37232e-05
-         },
-      (0,8): {
-            -0.000233212,
-            0.000280425
-         },
-      (0,9): {
-            0.00193516,
-            -0.00149884
-         },
-      (1,0): {
-            1.93186,
-            -0.315386
-         },
-      (1,1): {
-            -0.1,
-            -1.38778e-17
-         },
-      (1,2): {
-            -7.7426e-05,
-            2.70064e-05
-         },
-      (1,3): {
-            -0.0896458,
-            -2.69845
-         },
-      (1,4): {
-            -1.32725e-05,
-            -0.00021164
-         },
-      (1,5): {
-            -0.00197433,
-            -0.000924133
-         },
-      (1,6): {
-            -0.00135851,
-            0.00124512
-         },
-      (1,7): {
-            -0.0856668,
-            -0.0970713
-         },
-      (1,8): {
-            -0.00104908,
-            0.00128194
-         },
-      (1,9): {
-            4.4596e-05,
-            0.000584804
-         },
-      (2,0): {
-            -4.54204e-06,
-            -1.51803e-07
-         },
-      (2,1): {
-            -7.7426e-05,
-            -2.70064e-05
-         },
-      (2,2): {
-            -0.1,
-            1.05879e-22
-         },
-      (2,3): {
-            -2.93777e-05,
-            0.000171759
-         },
-      (2,4): {
-            0.249949,
-            -1.89125
-         },
-      (2,5): {
-            0.000993855,
-            -0.00101529
-         },
-      (2,6): {
-            -0.000757821,
-            -0.00176699
-         },
-      (2,7): {
-            0.000676951,
-            0.00123528
-         },
-      (2,8): {
-            -0.0610339,
-            0.0521267
-         },
-      (2,9): {
-            -0.00624451,
-            0.00325247
-         },
-      (3,0): {
-            0.000911647,
-            -0.000117906
-         },
-      (3,1): {
-            -0.0896458,
-            2.69845
-         },
-      (3,2): {
-            -2.93777e-05,
-            -0.000171759
-         },
-      (3,3): {
-            -0.1,
-            2.77556e-17
-         },
-      (3,4): {
-            0.00272149,
-            -0.000469602
-         },
-      (3,5): {
-            -2.85481,
-            -1.45231
-         },
-      (3,6): {
-            -0.00239257,
-            -0.00375987
-         },
-      (3,7): {
-            0.00286013,
-            0.00375819
-         },
-      (3,8): {
-            -0.0260578,
-            -0.0164994
-         },
-      (3,9): {
-            0.168722,
-            0.167976
-         },
-      (4,0): {
-            -2.24147e-06,
-            5.44984e-05
-         },
-      (4,1): {
-            -1.32725e-05,
-            0.00021164
-         },
-      (4,2): {
-            0.249949,
-            1.89125
-         },
-      (4,3): {
-            0.00272149,
-            0.000469602
-         },
-      (4,4): {
-            -0.0999986,
-            8.67356e-18
-         },
-      (4,5): {
-            -0.00370911,
-            -0.00207545
-         },
-      (4,6): {
-            1.33447,
-            2.22905
-         },
-      (4,7): {
-            0.0261154,
-            -0.0148433
-         },
-      (4,8): {
-            -0.00416014,
-            0.0030246
-         },
-      (4,9): {
-            0.0146916,
-            0.0169803
-         },
-      (5,0): {
-            -0.0320144,
-            -0.0468737
-         },
-      (5,1): {
-            -0.00197433,
-            0.000924133
-         },
-      (5,2): {
-            0.000993855,
-            0.00101529
-         },
-      (5,3): {
-            -2.85481,
-            1.45231
-         },
-      (5,4): {
-            -0.00370911,
-            0.00207545
-         },
-      (5,5): {
-            -0.10004,
-            0
-         },
-      (5,6): {
-            0.0438626,
-            0.0180354
-         },
-      (5,7): {
-            -1.41016,
-            3.24153
-         },
-      (5,8): {
-            0.0516424,
-            0.0126296
-         },
-      (5,9): {
-            0.0173344,
-            -0.00685343
-         },
-      (6,0): {
-            -6.19999e-05,
-            -2.86056e-05
-         },
-      (6,1): {
-            -0.00135851,
-            -0.00124512
-         },
-      (6,2): {
-            -0.000757821,
-            0.00176699
-         },
-      (6,3): {
-            -0.00239257,
-            0.00375987
-         },
-      (6,4): {
-            1.33447,
-            -2.22905
-         },
-      (6,5): {
-            0.0438626,
-            -0.0180354
-         },
-      (6,6): {
-            -0.0996054,
-            3.46945e-18
-         },
-      (6,7): {
-            0.00592456,
-            0.0546863
-         },
-      (6,8): {
-            -2.8588,
-            0.880557
-         },
-      (6,9): {
-            -0.316044,
-            0.0234734
-         },
-      (7,0): {
-            7.41788e-05,
-            4.37232e-05
-         },
-      (7,1): {
-            -0.0856668,
-            0.0970713
-         },
-      (7,2): {
-            0.000676951,
-            -0.00123528
-         },
-      (7,3): {
-            0.00286013,
-            -0.00375819
-         },
-      (7,4): {
-            0.0261154,
-            0.0148433
-         },
-      (7,5): {
-            -1.41016,
-            -3.24153
-         },
-      (7,6): {
-            0.00592456,
-            -0.0546863
-         },
-      (7,7): {
-            -0.105194,
-            9.97463e-18
-         },
-      (7,8): {
-            -0.147755,
-            -0.448124
-         },
-      (7,9): {
-            0.351712,
-            3.58789
-         },
-      (8,0): {
-            -0.000233212,
-            -0.000280425
-         },
-      (8,1): {
-            -0.00104908,
-            -0.00128194
-         },
-      (8,2): {
-            -0.0610339,
-            -0.0521267
-         },
-      (8,3): {
-            -0.0260578,
-            0.0164994
-         },
-      (8,4): {
-            -0.00416014,
-            -0.0030246
-         },
-      (8,5): {
-            0.0516424,
-            -0.0126296
-         },
-      (8,6): {
-            -2.8588,
-            -0.880557
-         },
-      (8,7): {
-            -0.147755,
-            0.448124
-         },
-      (8,8): {
-            -0.0647038,
-            -6.93895e-18
-         },
-      (8,9): {
-            -0.396711,
-            -0.0408396
-         },
-      (9,0): {
-            0.00193516,
-            0.00149884
-         },
-      (9,1): {
-            4.4596e-05,
-            -0.000584804
-         },
-      (9,2): {
-            -0.00624451,
-            -0.00325247
-         },
-      (9,3): {
-            0.168722,
-            -0.167976
-         },
-      (9,4): {
-            0.0146916,
-            -0.0169803
-         },
-      (9,5): {
-            0.0173344,
-            0.00685343
-         },
-      (9,6): {
-            -0.316044,
-            -0.0234734
-         },
-      (9,7): {
-            0.351712,
-            -3.58789
-         },
-      (9,8): {
-            -0.396711,
-            0.0408396
-         },
-      (9,9): {
-            -0.340506,
-            2.60209e-17
-         }
+      (0): -2016379437075879995
       }
    }
 }
 }
```

### Comparing `scqubits-3.1.0/scqubits/tests/data/zpifull-test.hdf5` & `scqubits-3.1.1/scqubits/tests/data/zpifull-test.hdf5`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_centraldispatch.py` & `scqubits-3.1.1/scqubits/tests/test_centraldispatch.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_circuit.py` & `scqubits-3.1.1/scqubits/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_circuit_plot.py` & `scqubits-3.1.1/scqubits/tests/test_circuit_plot.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_cos2phiqubit.py` & `scqubits-3.1.1/scqubits/tests/test_cos2phiqubit.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_explorer.py` & `scqubits-3.1.1/scqubits/tests/test_explorer.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_fluxonium.py` & `scqubits-3.1.1/scqubits/tests/test_fluxonium.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_fluxqubit.py` & `scqubits-3.1.1/scqubits/tests/test_fluxqubit.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_fullzeropi.py` & `scqubits-3.1.1/scqubits/tests/test_fullzeropi.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_gui.py` & `scqubits-3.1.1/scqubits/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_hilbertspace.py` & `scqubits-3.1.1/scqubits/tests/test_hilbertspace.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #    LICENSE file in the root directory of this source tree.
 ############################################################################
 
 import numpy as np
 import pytest
 
 import scqubits as scq
+import qutip as qt
 
 from scqubits.core.hilbert_space import HilbertSpace
 from scqubits.utils.spectrum_utils import get_matrixelement_table
 
 
 @pytest.mark.usefixtures("num_cpus")
 class TestHilbertSpace:
@@ -379,7 +380,94 @@
         hilbertspc.generate_lookup()
         hilbertspc.filewrite(self.tmpdir + "test.h5")
         hilbertspc_copy = scq.read(self.tmpdir + "test.h5")
 
     @staticmethod
     def test_HilbertSpace_GUI():
         hilbertspace_new = scq.HilbertSpace.create()
+
+    def test_HilbertSpace_op_in_dressed_basis(self):
+        E_osc_a = 4.0
+        E_osc_b = 3.2
+        g = 0.01
+        Delta = E_osc_a - E_osc_b
+        truncated_dim = 4
+        theta = 0.5 * np.arctan(2 * g / Delta)
+        osc_a = scq.Oscillator(E_osc=E_osc_a, truncated_dim=truncated_dim)
+        osc_b = scq.Oscillator(E_osc=E_osc_b, truncated_dim=truncated_dim)
+        hilbert_space = scq.HilbertSpace([osc_a, osc_b])
+        hilbert_space.add_interaction(
+            g=g,
+            op1=osc_a.creation_operator,
+            op2=osc_b.annihilation_operator,
+            add_hc=True,
+        )
+        hilbert_space.generate_lookup()
+        hilbert_space.standardize_eigenvector_phases()
+        # analytic answer for the dressed operator based on a Bogoliubov transformation
+        a_id_wrap = scq.utils.spectrum_utils.identity_wrap(
+            osc_a.annihilation_operator(), osc_a, hilbert_space.subsystem_list
+        )
+        b_id_wrap = scq.utils.spectrum_utils.identity_wrap(
+            osc_b.annihilation_operator(), osc_b, hilbert_space.subsystem_list
+        )
+        analytic_op = np.cos(theta) * a_id_wrap - np.sin(theta) * b_id_wrap
+        # need to order this operator according to the dressed indices for later
+        # comparison with operators expressed in the dressed basis
+        ordered_bare_indices = [
+            hilbert_space.bare_index(idx) for idx in range(truncated_dim**2)
+        ]
+        ordered_basis_states = [
+            qt.tensor(qt.basis(truncated_dim, idx_a), qt.basis(truncated_dim, idx_b))
+            for (idx_a, idx_b) in ordered_bare_indices
+        ]
+        # consider only matrix elements unaffected by the truncation level
+        analytic_op_ordered = qt.Qobj(
+            analytic_op.transform(ordered_basis_states)[0:10, 0:10]
+        )
+        op1 = qt.Qobj(
+            hilbert_space.op_in_dressed_eigenbasis(op=osc_a.annihilation_operator)[
+                0:10, 0:10
+            ]
+        )
+        op2 = qt.Qobj(
+            hilbert_space.op_in_dressed_eigenbasis(
+                op=(osc_a.annihilation_operator(), osc_a)
+            )[0:10, 0:10]
+        )
+        op3 = qt.Qobj(
+            hilbert_space.op_in_dressed_eigenbasis(
+                op=(osc_a.annihilation_operator(), osc_a), op_in_bare_eigenbasis=True
+            )[0:10, 0:10]
+        )
+        op4 = qt.Qobj(
+            hilbert_space.op_in_dressed_eigenbasis(
+                op=(osc_a.annihilation_operator(), osc_a), op_in_bare_eigenbasis=False
+            )[0:10, 0:10]
+        )
+        assert analytic_op_ordered == op1
+        assert analytic_op_ordered == op2
+        assert analytic_op_ordered == op3
+        assert analytic_op_ordered == op4
+
+    def test_HilbertSpace_op_in_dressed_basis_native_vs_bare_basis(self):
+        E_osc = 4.0
+        g = 0.01
+        truncated_dim = 4
+        tmon = scq.Transmon(
+            EJ=10.0, EC=0.2, ng=0.0, ncut=15, truncated_dim=truncated_dim
+        )
+        osc = scq.Oscillator(E_osc=E_osc, truncated_dim=truncated_dim)
+        hilbert_space = scq.HilbertSpace([tmon, osc])
+        hilbert_space.add_interaction(
+            g=g,
+            op1=tmon.n_operator,
+            op2=osc.annihilation_operator,
+            add_hc=True,
+        )
+        hilbert_space.generate_lookup()
+        op1 = hilbert_space.op_in_dressed_eigenbasis(op=tmon.n_operator)
+        n_op_bare_eigenbasis_v2 = tmon.n_operator(energy_esys=True)
+        op2 = hilbert_space.op_in_dressed_eigenbasis(
+            op=(n_op_bare_eigenbasis_v2, tmon), op_in_bare_eigenbasis=True
+        )
+        assert op1 == op2
```

### Comparing `scqubits-3.1.0/scqubits/tests/test_namedslotsndarray.py` & `scqubits-3.1.1/scqubits/tests/test_namedslotsndarray.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_noise.py` & `scqubits-3.1.1/scqubits/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_parameters.py` & `scqubits-3.1.1/scqubits/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_parametersweep.py` & `scqubits-3.1.1/scqubits/tests/test_parametersweep.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_spectrumlookup.py` & `scqubits-3.1.1/scqubits/tests/test_spectrumlookup.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_transmon.py` & `scqubits-3.1.1/scqubits/tests/test_transmon.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_units.py` & `scqubits-3.1.1/scqubits/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/tests/test_zeropi.py` & `scqubits-3.1.1/scqubits/tests/test_zeropi.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/ui/__init__.py` & `scqubits-3.1.1/scqubits/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/ui/explorer_widget.py` & `scqubits-3.1.1/scqubits/ui/explorer_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from scqubits.ui.gui_defaults import (
     composite_panel_names,
     default_panels,
     mode_dropdown_list,
     subsys_panel_names,
 )
 from scqubits.utils import misc as utils
+from scqubits.settings import matplotlib_settings
 
 if TYPE_CHECKING:
     from scqubits.core.param_sweep import ParameterSweep
 
 try:
     from IPython.display import display
 except ImportError:
@@ -86,15 +87,14 @@
     return Layout(width=str(pixels) + "px")
 
 
 @utils.Required(ipywidgets=_HAS_IPYWIDGETS)
 def boxed(pixels: int = 900) -> Layout:
     return Layout(
         width=str(pixels) + "px",
-        align="top",
         border="1px solid lightgrey",
         padding="10px 10px 10px 10px",
     )
 
 
 class Explorer:
     """
@@ -160,14 +160,15 @@
         # +----------------+-----------------------------------------------------------+
 
         self.ui_main_tab = self.build_ui_main_tab()
         self.ui_hbox["main_display"] = self.build_ui_main_display()
         self.gui_display.children = [self.ui_main_tab, self.ui_hbox["main_display"]]
         display(self.gui_display)
 
+    @matplotlib.rc_context(matplotlib_settings)
     def build_figure_and_axes_table(self) -> Tuple[Figure, np.ndarray]:
         # the %inline and %widget backends somehow scale differently; try to compensate
         self.figwidth = 6.4
         self.figheight = 2.6
 
         plt.ioff()
         fig = plt.figure(figsize=(self.figwidth, self.figheight))
@@ -420,28 +421,30 @@
                 VBox([HTML("<br>Sample value"), self.ui["sweep_value_slider"]]),
                 HTML("<br>"),
                 self.ui_vbox["fixed_param_sliders"],
             ],
             layout=boxed(260),
         )
 
+    @matplotlib.rc_context(matplotlib_settings)
     def build_ui_figure_display(self):
         if _HAS_WIDGET_BACKEND:
             out = self.fig.canvas
             self.fig.tight_layout()
         else:
             out = Output(layout=width(750))
             out.layout.object_fit = "contain"
             out.layout.width = "100%"
             with out:
                 out.clear_output(wait=True)
                 self.fig.tight_layout()
                 display(self.fig)
         return out
 
+    @matplotlib.rc_context(matplotlib_settings)
     def display_panel(
         self,
         full_panel_name: str,
         param_slice: ParameterSlice,
         fig_ax: Tuple[Figure, Axes],
     ):
         subsys_name, panel_name = full_panel_name.split(SEP)
@@ -650,14 +653,15 @@
         return ParameterSlice(
             self.ui["sweep_param_dropdown"].value,
             self.ui["sweep_value_slider"].value,
             self.fixed_params,
             list(self.sweep.param_info.keys()),
         )
 
+    @matplotlib.rc_context(matplotlib_settings)
     def update_layout_and_plots(self: "Explorer", change):
         panels = self.get_panels_list()
 
         nrows = len(panels) // self.ncols
         if len(panels) % self.ncols != 0:
             nrows += 1
 
@@ -683,14 +687,15 @@
 
         if not _HAS_WIDGET_BACKEND:
             with self.ui["figure_display"]:
                 self.ui["figure_display"].clear_output(wait=True)
                 self.fig.tight_layout()
                 display(self.fig)
 
+    @matplotlib.rc_context(matplotlib_settings)
     def update_plots(self: "Explorer", change):
         if not hasattr(self, "fig"):
             return
 
         param_val = self.ui["sweep_value_slider"].value
         panels = self.get_panels_list()
 
@@ -808,18 +813,15 @@
                 options=self.subsys_names,
                 value=[self.subsys_names[0]],
                 rows=4,
                 layout=width(185),
             )
 
             self.ui["transitions"]["initial_bare_dressed_toggle"] = ToggleButtons(
-                options=["bare", "dressed"],
-                value="bare",
-                description="",
-                disable=False,
+                options=["bare", "dressed"], value="bare", description=""
             )
             self.ui["transitions"][
                 "initial_bare_dressed_toggle"
             ].style.button_width = "45px"
 
             self.ui["transitions"]["sidebands_checkbox"] = Checkbox(
                 description="show sidebands", value=False, layout=width(250)
```

### Comparing `scqubits-3.1.0/scqubits/ui/gui.py` & `scqubits-3.1.1/scqubits/ui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from matplotlib import get_backend as get_matplotlib_backend
 from matplotlib.figure import Axes, Figure
 
 from scqubits.core.discretization import Grid1d
 from scqubits.core.flux_qubit import FluxQubit
 from scqubits.core.zeropi import ZeroPi
 from scqubits.core.zeropi_full import FullZeroPi
+from scqubits.settings import matplotlib_settings
 
 try:
     from ipywidgets import (
         Box,
         Button,
         Checkbox,
         Dropdown,
@@ -169,26 +170,24 @@
         """Creates all the widgets associated with manually updating and
         saving plots.
         """
         self.manual_update_and_save_widgets = {
             "manual_update_checkbox": Checkbox(
                 value=False,
                 description="Manual Update",
-                disabled=False,
                 indent=False,
                 layout=Layout(width="125px"),
             ),
             "update_button": Button(
                 description="Update", disabled=True, layout=Layout(width="100px")
             ),
             "save_button": Button(icon="save", layout=Layout(width="35px")),
             "filename_text": Text(
                 value=str(Path.cwd().joinpath("plot.pdf")),
                 description="",
-                disabled=False,
                 layout=Layout(width="500px"),
             ),
         }
 
     def initialize_noise_param_widgets(self) -> None:
         """Creates all the widgets associated with coherence times plots"""
         self.noise_param_widgets.clear()
@@ -211,22 +210,21 @@
         if "t1_quasiparticle_tunneling" in noise_channels:
             noise_params.append("x_qp")
             noise_params.append("Delta")
 
         for noise_param in noise_params:
             self.noise_param_widgets[noise_param] = FloatText(
                 value=noise.NOISE_PARAMS[noise_param],
-                disalbed=False,
                 description=noise_param,
                 step=0.001,
             )
 
     def set_qubit(self, qubit_name: str) -> None:
         """Sets up the chosen qubit to be the active qubit
-        and updates the activedefaults and widget dictionaries
+        and updates the active defaults and widget dictionaries
         accordingly.
         """
         if qubit_name in gui_defaults.slow_qubits:
             scq.settings.PROGRESSBAR_DISABLED = False
         else:
             scq.settings.PROGRESSBAR_DISABLED = True
 
@@ -284,82 +282,74 @@
             "qubit_info_image_widget": Image(
                 value=image, format="jpg", layout=Layout(width="80%")
             ),
             "scan_dropdown": Dropdown(
                 options=scan_dropdown_list,
                 value=self.active_defaults["scan_param"],
                 description="Scan over",
-                disabled=False,
                 layout=std_layout,
             ),
             "mode_dropdown": Dropdown(
                 options=gui_defaults.mode_dropdown_list,
                 description="Plot as:",
-                disabled=False,
                 layout=std_layout,
             ),
             "operator_dropdown": Dropdown(
                 options=operator_dropdown_list,
                 value=self.active_defaults["operator"],
                 description="Operator",
-                disabled=False,
                 layout=std_layout,
             ),
             "noise_channel_multi-select": SelectMultiple(
                 options=noise_channel_list,
                 value=noise_channel_list,
                 description="Noise Channels",
-                disabled=False,
                 layout=std_layout,
             ),
             "highest_state_slider": IntSlider(
                 min=1,
                 max=10,
                 value=5,
                 continuous_update=False,
                 layout=std_layout,
                 description="Highest State",
             ),
             "show_numbers_checkbox": Checkbox(
-                value=False, description="Show values", disabled=False, indent=False
+                value=False, description="Show values", indent=False
             ),
             "show3d_checkbox": Checkbox(
-                value=True, description="Show 3D", disabled=False, indent=False
+                value=True, description="Show 3D", indent=False
             ),
             "subtract_ground_checkbox": Checkbox(
                 value=True,
                 description="Subtract E\u2080",
-                disabled=False,
                 indent=False,
             ),
-            "i_text": IntText(value=1, disabled=False, step=1),
-            "j_text": IntText(value=0, disabled=False, step=1),
+            "i_text": IntText(value=1, step=1),
+            "j_text": IntText(value=0, step=1),
             "t1_checkbox": Checkbox(
                 value=False,
                 description="Effective T1",
-                disabled=False,
                 indent=False,
             ),
             "t2_checkbox": Checkbox(
                 value=False,
                 description="Effective T2",
-                disabled=False,
                 indent=False,
             ),
         }
 
         if current_qubit in ["Transmon", "TunableTransmon", "Fluxonium"]:
             self.qubit_plot_options_widgets["manual_scale_checkbox"] = Checkbox(
-                value=False, description="Manual Scaling", disabled=False, indent=False
+                value=False, description="Manual Scaling", indent=False
             )
             self.qubit_plot_options_widgets["multi_state_selector"] = SelectMultiple(
                 options=range(0, 10),
                 value=[0, 1, 2, 3, 4],
                 description="States",
-                disabled=False,
                 continuous_update=False,
                 layout=std_layout,
             )
             self.qubit_plot_options_widgets["wavefunction_scale_slider"] = FloatSlider(
                 min=0.1,
                 max=4,
                 value=self.active_defaults["scale"],
@@ -380,15 +370,15 @@
 
         if current_qubit in gui_defaults.paramvals_from_papers.keys():
             common_params_dropdown_list = ["Manual"]
             common_params_dropdown_list.extend(
                 gui_defaults.paramvals_from_papers[current_qubit].keys()
             )
             self.qubit_plot_options_widgets["common_params_dropdown"] = Dropdown(
-                options=common_params_dropdown_list, disabled=False, layout=std_layout
+                options=common_params_dropdown_list, layout=std_layout
             )
         else:
             self.qubit_plot_options_widgets["common_params_dropdown"] = Label(
                 value="None"
             )
 
         self.qubit_plot_options_widgets["link_HTML"] = HTML(value="")
@@ -967,33 +957,38 @@
             ].disabled = False
         else:
             self.qubit_plot_options_widgets["wavefunction_scale_slider"].disabled = True
 
     def coherence_text(self, change) -> None:
         self.unobserve_coherence_elements()
         self.unobserve_plot_refresh()
+        isNoiseParamChange = None
         widget_key = change["owner"].description
-        widget = None
 
         if widget_key in self.noise_param_widgets.keys():
+            isNoiseParamChange = True
             widget = self.noise_param_widgets[widget_key]
         else:
+            isNoiseParamChange = False
             i_text_widget = self.qubit_plot_options_widgets["i_text"]
             j_text_widget = self.qubit_plot_options_widgets["j_text"]
 
         if change["new"] <= 0:
-            if i_text_widget.value <= 0:
-                i_text_widget.value = 0
-            if j_text_widget.value <= 0:
-                j_text_widget.value = 0
-            if widget_key in self.noise_param_widgets.keys():
-                widget.value = widget.step
-
-        if i_text_widget.value == j_text_widget.value:
-            i_text_widget.value = j_text_widget.value + j_text_widget.step
+            if isNoiseParamChange:
+                if widget_key in self.noise_param_widgets.keys():
+                    widget.value = widget.step
+            else:
+                if i_text_widget.value <= 0:
+                    i_text_widget.value = 0
+                if j_text_widget.value <= 0:
+                    j_text_widget.value = 0
+
+        if not isNoiseParamChange:
+            if i_text_widget.value == j_text_widget.value:
+                i_text_widget.value = j_text_widget.value + j_text_widget.step
         self.observe_coherence_elements()
         self.observe_plot_refresh()
 
     def plot_change_bool_update(self, change):
         self.plot_output.clear_output()
         self.plot_change_bool = True
 
@@ -1205,14 +1200,15 @@
             "eigenvalue_state_value": self.qubit_plot_options_widgets[
                 "highest_state_slider"
             ].get_interact_value(),
         }
 
         self.evals_vs_paramvals_plot(**value_dict)
 
+    @matplotlib.rc_context(matplotlib_settings)
     def wavefunctions_plot_refresh(self, change) -> None:
         value_dict = {
             "mode_value": self.qubit_plot_options_widgets[
                 "mode_dropdown"
             ].get_interact_value(),
         }
 
@@ -1780,14 +1776,15 @@
                 layout=Layout(width="95%"),
             ),
         )
 
         return plot_options_widgets_tuple
 
     # Plot functions------------------------------------------------------------------
+    @matplotlib.rc_context(matplotlib_settings)
     def evals_vs_paramvals_plot(
         self,
         scan_value: str,
         scan_range: Tuple[float, float],
         eigenvalue_state_value: int,
         subtract_ground_tf: bool,
     ) -> None:
@@ -1835,14 +1832,15 @@
         self.fig.set_figwidth(gui_defaults.FIG_WIDTH_INCHES)
         if not _HAS_WIDGET_BACKEND:
             plt.close("all")
             with self.plot_output:
                 display(self.fig)
         GUI.fig_ax = self.fig, self.fig.axes[0]
 
+    @matplotlib.rc_context(matplotlib_settings)
     def wavefunctions_plot(
         self,
         eigenvalue_states: Union[List[int], int],
         mode_value: str,
         scale_value: Optional[float] = None,
         phi_grid: Optional[Grid1d] = None,
         theta_grid: Optional[Grid1d] = None,
```

### Comparing `scqubits-3.1.0/scqubits/ui/gui_defaults.py` & `scqubits-3.1.1/scqubits/ui/gui_defaults.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/ui/hspace_widget.py` & `scqubits-3.1.1/scqubits/ui/hspace_widget.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/ui/qubit_widget.py` & `scqubits-3.1.1/scqubits/ui/qubit_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
             enter_widget = ipywidgets.FloatText
         else:
             enter_widget = ipywidgets.IntText
 
         widgets[name] = enter_widget(
             value=value,
             description="",
-            disabled=False,
             layout=ipywidgets.Layout(width="150px"),
         )
         box_list.append(
             ipywidgets.HBox(
                 [label, widgets[name]],
                 layout=ipywidgets.Layout(justify_content="flex-end"),
             )
```

### Comparing `scqubits-3.1.0/scqubits/utils/__init__.py` & `scqubits-3.1.1/scqubits/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/utils/cpu_switch.py` & `scqubits-3.1.1/scqubits/utils/cpu_switch.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits/utils/misc.py` & `scqubits-3.1.1/scqubits/utils/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -158,14 +158,28 @@
                     Warning,
                 )
         return func(self, *args, **kwargs)
 
     return wrapper
 
 
+def check_lookup_exists(func: Callable) -> Callable:
+    @functools.wraps(func)
+    def wrapper(self, *args, **kwargs):
+        if not self._lookup_exists:
+            raise Exception(
+                "Lookup data not found. For HilbertSpace: data must be generated with .generate_lookup(). "
+                "For ParameterSweep: data should be automatically generated unless disabled manually. In "
+                "the latter case, apply .run()."
+            )
+        return func(self, *args, **kwargs)
+
+    return wrapper
+
+
 class DeprecationMessage:
     """Decorator class, producing an adjustable warning and info upon usage of the
     decorated function.
 
     Parameters
     ----------
     warning_message:
```

### Comparing `scqubits-3.1.0/scqubits/utils/plot_defaults.py` & `scqubits-3.1.1/scqubits/utils/plot_defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
       scaling factor
     """
     # Do not attempt to scale down amplitudes to very small energy spacings, i.e. if
     # energy spacing is smaller than y_range * Y_RANGE_THRESHOLD_FRACTION, then do
     # not apply additional downscaling
     Y_RANGE_THRESHOLD_FRACTION = 1 / 12
 
-    # If energy spacing is used for scaling, fill no more than this  fraction of the
+    # If energy spacing is used for scaling, fill no more than this fraction of the
     # spacing.
     FILLING_FRACTION = 0.9
 
     # Largest allowed wavefunction amplitude range as fraction of y_range.
     MAX_AMPLITUDE_FRACTION = 1 / 7
 
     # Amplitude threshold for applying any scaling at all. Note that the imaginary
@@ -71,16 +71,16 @@
 
     wavefunc_count = len(wavefunctions)
     energies = [wavefunc.energy for wavefunc in wavefunctions]
 
     e_max = np.max(energies)
     e_min = np.min(energies)
     e_range = e_max - e_min
-    y_min = np.min(potential_vals)
-    y_max = e_max + 0.3 * e_range
+    y_min = np.min(potential_vals)  # lowest value of potential energy
+    y_max = e_max + 0.3 * e_range  # maximum eigenenergy plus padding
     y_range = y_max - y_min
 
     amplitudes = np.asarray([wavefunc.amplitudes for wavefunc in wavefunctions])
 
     def amplitude_mins() -> np.ndarray:
         return np.apply_along_axis(func1d=np.min, axis=1, arr=amplitudes)
```

### Comparing `scqubits-3.1.0/scqubits/utils/plot_utils.py` & `scqubits-3.1.1/scqubits/utils/plot_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 from numpy import ndarray
 
 from scqubits import settings as settings
 from scqubits.utils import plot_defaults as defaults
+from scqubits.settings import matplotlib_settings
 
 if TYPE_CHECKING:
     from scqubits.core.storage import WaveFunction
 
 
 # A dictionary of plotting options that are directly passed to specific matplotlib's
 # plot commands.
@@ -42,14 +43,15 @@
         "label",
     ),
     "imshow": ("interpolation",),
     "contourf": tuple(),  # empty for now
 }
 
 
+@mpl.rc_context(matplotlib_settings)
 def _extract_kwargs_options(
     kwargs: Dict[str, Any], plot_type: str, direct_plot_options: Dict[str, Any] = None
 ) -> Dict[str, Any]:
     """
     Select options from kwargs for a given plot_type and return them in a dictionary.
 
     Parameters
@@ -74,14 +76,15 @@
 
     for key in kwargs:
         if key in direct_plot_options[plot_type]:
             selected_options[key] = kwargs[key]
     return selected_options
 
 
+@mpl.rc_context(matplotlib_settings)
 def _process_options(
     figure: Figure, axes: Axes, opts: Dict[str, Any] = None, **kwargs
 ) -> None:
     """
     Processes plotting options.
 
     Parameters
@@ -119,14 +122,15 @@
     if filename:
         figure.savefig(os.path.splitext(filename)[0] + ".pdf")
 
     if settings.DESPINE and not axes.name == "3d":
         despine_axes(axes)
 
 
+@mpl.rc_context(matplotlib_settings)
 def _process_special_option(figure: Figure, axes: Axes, key: str, value: Any) -> None:
     """Processes a single 'special' option, i.e., one internal to scqubits and not to be
     handed further down to matplotlib.
     """
     if key == "ymax":
         ymax = value
         ymin, _ = axes.get_ylim()
@@ -137,24 +141,26 @@
     elif key == "grid":
         if isinstance(value, dict):
             axes.grid(**value)
         else:
             axes.grid(value)
 
 
+@mpl.rc_context(matplotlib_settings)
 def despine_axes(axes: Axes) -> None:
     # Hide the right and top spines
     axes.spines["right"].set_visible(False)
     axes.spines["top"].set_visible(False)
 
     # Only show ticks on the left and bottom spines
     axes.yaxis.set_ticks_position("left")
     axes.xaxis.set_ticks_position("bottom")
 
 
+@mpl.rc_context(matplotlib_settings)
 def scale_wavefunctions(
     wavefunc_list: List["WaveFunction"],
     potential_vals: np.ndarray,
     scaling: Optional[float],
 ) -> List["WaveFunction"]:
     for wavefunc in wavefunc_list:
         wavefunc.rescale_to_potential(potential_vals)
@@ -162,27 +168,29 @@
         wavefunc_list, potential_vals
     )
     for wavefunc in wavefunc_list:
         wavefunc.rescale(adaptive_scalefactor)
     return wavefunc_list
 
 
+@mpl.rc_context(matplotlib_settings)
 def plot_wavefunction_to_axes(
     axes: Axes, wavefunction: "WaveFunction", energy_offset: float, **kwargs
 ) -> None:
     x_vals = wavefunction.basis_labels
     y_vals = energy_offset + wavefunction.amplitudes
     offset_vals = [energy_offset] * len(x_vals)
 
     axes.plot(x_vals, y_vals, **_extract_kwargs_options(kwargs, "plot"))
     axes.fill_between(
         x_vals, y_vals, offset_vals, where=(y_vals != offset_vals), interpolate=True
     )
 
 
+@mpl.rc_context(matplotlib_settings)
 def plot_potential_to_axes(
     axes: Axes,
     x_vals: ndarray,
     potential_vals: Union[ndarray, List[float]],
     offset_list: Union[ndarray, List[float]],
     **kwargs,
 ) -> None:
@@ -195,14 +203,15 @@
     axes.set_ylim([y_min, y_max])
 
     axes.plot(
         x_vals, potential_vals, color="gray", **_extract_kwargs_options(kwargs, "plot")
     )
 
 
+@mpl.rc_context(matplotlib_settings)
 def add_numbers_to_axes(
     axes: Axes, matrix: ndarray, modefunc: Callable, fontsize: int = 8
 ) -> None:
     for y_index in range(matrix.shape[0]):
         for x_index in range(matrix.shape[1]):
             axes.text(
                 x_index,
@@ -212,14 +221,15 @@
                 ha="center",
                 fontsize=fontsize,
                 rotation=45,
                 color="white",
             )
 
 
+@mpl.rc_context(matplotlib_settings)
 def color_normalize(vals, mode: str) -> Tuple[float, float, mpl.colors.Normalize]:
     minval = min(vals)
     maxval = max(vals)
     if mode in ["abs", "abs_sqr"]:
         minval = 0
 
     nrm = mpl.colors.Normalize(minval, maxval)
```

### Comparing `scqubits-3.1.0/scqubits/utils/plotting.py` & `scqubits-3.1.1/scqubits/utils/plotting.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,26 +29,28 @@
     _process_options,
     add_numbers_to_axes,
     color_normalize,
     plot_potential_to_axes,
     plot_wavefunction_to_axes,
     scale_wavefunctions,
 )
+from scqubits.settings import matplotlib_settings
 
 if TYPE_CHECKING:
     from scqubits.core.storage import SpectrumData, WaveFunction, WaveFunctionOnGrid
 
 try:
     from labellines import labelLines
 
     _LABELLINES_ENABLED = True
 except ImportError:
     _LABELLINES_ENABLED = False
 
 
+@mpl.rc_context(matplotlib_settings)
 def wavefunction1d(
     wavefuncs: Union["WaveFunction", "List[WaveFunction]"],
     potential_vals: np.ndarray,
     offset: Union[float, Iterable[float]] = 0,
     scaling: Optional[float] = None,
     **kwargs,
 ) -> Tuple[Figure, Axes]:
@@ -85,14 +87,15 @@
     x_vals = wavefunc_list[0].basis_labels
     plot_potential_to_axes(axes, x_vals, potential_vals, offset_list, **kwargs)
 
     _process_options(fig, axes, **kwargs)
     return fig, axes
 
 
+@mpl.rc_context(matplotlib_settings)
 def wavefunction1d_nopotential(
     wavefuncs: Union["WaveFunction", "List[WaveFunction]"],
     offset: Union[float, Iterable[float]] = 0,
     **kwargs,
 ) -> Tuple[Figure, Axes]:
     """
     Plots the amplitude of a single real-valued 1d wave function, along with the
@@ -123,14 +126,15 @@
     for wavefunction, energy_offset in zip(wavefunc_list, offset_list):
         plot_wavefunction_to_axes(axes, wavefunction, energy_offset, **kwargs)
 
     _process_options(fig, axes, **kwargs)
     return fig, axes
 
 
+@mpl.rc_context(matplotlib_settings)
 def wavefunction1d_discrete(wavefunc: "WaveFunction", **kwargs) -> Tuple[Figure, Axes]:
     """
     Plots the amplitude of a real-valued 1d wave function in a discrete basis.
     (Example: transmon in the charge basis.)
 
     Parameters
     ----------
@@ -152,14 +156,15 @@
     axes.set_xticks(x_vals)
     axes.set_xticklabels(x_vals)
     _process_options(fig, axes, defaults.wavefunction1d_discrete(), **kwargs)
 
     return fig, axes
 
 
+@mpl.rc_context(matplotlib_settings)
 def wavefunction2d(
     wavefunc: "WaveFunctionOnGrid", zero_calibrate: bool = False, **kwargs
 ) -> Tuple[Figure, Axes]:
     """
     Creates a density plot of the amplitude of a real-valued wave function in 2
     "spatial" dimensions.
 
@@ -205,14 +210,15 @@
     cax = divider.append_axes("right", size="2%", pad=0.05)
     fig.colorbar(im, cax=cax)
 
     _process_options(fig, axes, defaults.wavefunction2d(), **kwargs)
     return fig, axes
 
 
+@mpl.rc_context(matplotlib_settings)
 def contours(
     x_vals: Union[List[float], np.ndarray],
     y_vals: Union[List[float], np.ndarray],
     func: Callable,
     contour_vals: Union[List[float], np.ndarray] = None,
     show_colorbar: bool = True,
     **kwargs,
@@ -257,14 +263,15 @@
         cax = divider.append_axes("right", size="2%", pad=0.05)
         fig.colorbar(im, cax=cax)
 
     _process_options(fig, axes, opts=defaults.contours(x_vals, y_vals), **kwargs)
     return fig, axes
 
 
+@mpl.rc_context(matplotlib_settings)
 def matrix(
     data_matrix: np.ndarray, mode: str = "abs", show_numbers: bool = False, **kwargs
 ) -> Tuple[Figure, Tuple[Axes, Axes]]:
     """
     Create a "skyscraper" plot and a 2d color-coded plot of a matrix.
 
     Parameters
@@ -295,14 +302,15 @@
     fig, ax2 = matrix2d(
         data_matrix, mode=mode, show_numbers=show_numbers, fig_ax=(fig, ax2), **kwargs
     )
     fig, ax1 = matrix_skyscraper(data_matrix, mode=mode, fig_ax=(fig, ax1), **kwargs)
     return fig, (ax1, ax2)
 
 
+@mpl.rc_context(matplotlib_settings)
 def matrix_skyscraper(
     matrix: np.ndarray, mode: str = "abs", **kwargs
 ) -> Tuple[Figure, Axes]:
     """Display a 3d skyscraper plot of the matrix
 
     Parameters
     ----------
@@ -353,19 +361,24 @@
     for axis, locs in [
         (axes.xaxis, np.arange(x_count)),
         (axes.yaxis, np.arange(y_count)),
     ]:
         axis.set_ticks(locs + 0.5, minor=True)
         axis.set(ticks=locs + 0.5, ticklabels=locs)
 
+    axes.tick_params(axis='x', pad=-5)
+    axes.tick_params(axis='y', pad=-5)
+    axes.tick_params(axis='z', pad=-2)
+
     _process_options(fig, axes, opts=defaults.matrix(), **kwargs)
 
     return fig, axes
 
 
+@mpl.rc_context(matplotlib_settings)
 def matrix2d(
     matrix: np.ndarray,
     mode: str = "abs",
     show_numbers: bool = True,
     show_colorbar: bool = True,
     **kwargs,
 ) -> Tuple[Figure, Axes]:
@@ -408,15 +421,15 @@
         )
     cax = axes.matshow(modefunction(matrix), cmap=plt.cm.viridis, interpolation=None)
 
     if show_numbers:
         fig_width, fig_height = fig.get_size_inches()
         box_width_inches = fig_width / matrix.shape[1]
         box_height_inches = fig_height / matrix.shape[0]
-        font_size = min(box_width_inches, box_height_inches) * 12
+        font_size = min(box_width_inches, box_height_inches) * 11
         add_numbers_to_axes(axes, matrix, modefunction, fontsize=font_size)
 
     # shift the grid
     for axis, locs in [
         (axes.xaxis, np.arange(matrix.shape[1])),
         (axes.yaxis, np.arange(matrix.shape[0])),
     ]:
@@ -426,14 +439,15 @@
 
     _process_options(fig, axes, **kwargs)
     axes.tick_params(axis="x", bottom=True, top=False, labelbottom=True, labeltop=False)
 
     return fig, axes
 
 
+@mpl.rc_context(matplotlib_settings)
 def data_vs_paramvals(
     xdata: np.ndarray,
     ydata: np.ndarray,
     label_list: Union[List[str], List[int]] = None,
     **kwargs,
 ) -> Tuple[Figure, Axes]:
     """Plot of a set of ydata vs xdata.
@@ -484,14 +498,15 @@
     # cannot reduce the intended x range
     axes.update_datalim(np.c_[xdata, [0] * len(xdata)], updatey=False)
     axes.autoscale()
 
     return fig, axes
 
 
+@mpl.rc_context(matplotlib_settings)
 def evals_vs_paramvals(
     specdata: "SpectrumData",
     which: Union[int, Iterable[int]] = -1,
     subtract_ground: bool = False,
     label_list: List[str] = None,
     **kwargs,
 ) -> Tuple[Figure, Axes]:
@@ -530,14 +545,15 @@
         xdata,
         ydata,
         label_list=label_list,
         **defaults.evals_vs_paramvals(specdata, **kwargs),
     )
 
 
+@mpl.rc_context(matplotlib_settings)
 def matelem_vs_paramvals(
     specdata: "SpectrumData",
     select_elems: Union[int, List[Tuple[int, int]]] = 4,
     mode: str = "abs",
     **kwargs,
 ) -> Tuple[Figure, Axes]:
     """Generates a simple plot of matrix elements as a function of one parameter.
@@ -570,22 +586,22 @@
     if isinstance(select_elems, int):
         index_pairs = [
             (row, col) for row in range(select_elems) for col in range(row + 1)
         ]
     else:
         index_pairs = select_elems
 
-    for (row, col) in index_pairs:
+    for row, col in index_pairs:
         y_vals = modefunction(specdata.matrixelem_table[:, row, col])
         axes.plot(
             x_vals,
             y_vals,
             label=f"{row},{col}",
             **_extract_kwargs_options(kwargs, "plot"),
         )
 
     if _LABELLINES_ENABLED:
         labelLines(axes.get_lines(), zorder=1.5)
     else:
-        axes.legend(loc="center left", bbox_to_anchor=(1, 0.5))
+        axes.legend(loc="center left", bbox_to_anchor=(1, 0.5), frameon=False)
     _process_options(fig, axes, opts=defaults.matelem_vs_paramvals(specdata), **kwargs)
     return fig, axes
```

### Comparing `scqubits-3.1.0/scqubits/utils/spectrum_utils.py` & `scqubits-3.1.1/scqubits/utils/spectrum_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,16 +114,16 @@
 
 
 def standardize_sign(real_array: np.ndarray) -> np.ndarray:
     """Standardizes the sign of a real-valued wavefunction by calculating the sign of
     the sum of all amplitudes up to the wavefunctions mid-position and making it
     positive.
 
-    Summing up to the midpoint only is to address the  danger that the sum is
-    actually zero, which may is the case for odd wavefunctions taken over an interval
+    Summing up to the midpoint only is to address the danger that the sum is
+    actually zero, which may be the case for odd wavefunctions taken over an interval
     centered at zero.
     """
     halfway_position = len(real_array) // 2
     return np.sign(np.sum(real_array[:halfway_position])) * real_array
 
 
 # -Matrix elements and operators (outside qutip) --------------------------------------
```

### Comparing `scqubits-3.1.0/scqubits/utils/typedefs.py` & `scqubits-3.1.1/scqubits/utils/typedefs.py`

 * *Files identical despite different names*

### Comparing `scqubits-3.1.0/scqubits.egg-info/PKG-INFO` & `scqubits-3.1.1/scqubits.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scqubits
-Version: 3.1.0
+Version: 3.1.1
 Summary: scqubits: superconducting qubits in Python
 Home-page: https://scqubits.readthedocs.io
 Author: Jens Koch, Peter Groszkowski
 Author-email: jens-koch@northwestern.edu, piotrekg@gmail.com
 License: BSD
 Keywords: superconducting qubits
 Platform: Linux
```

### Comparing `scqubits-3.1.0/scqubits.egg-info/SOURCES.txt` & `scqubits-3.1.1/scqubits.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 scqubits/tests/test_noise.py
 scqubits/tests/test_parameters.py
 scqubits/tests/test_parametersweep.py
 scqubits/tests/test_spectrumlookup.py
 scqubits/tests/test_transmon.py
 scqubits/tests/test_units.py
 scqubits/tests/test_zeropi.py
-scqubits/tests/data/.fullzeropi_1.hdf5
 scqubits/tests/data/circuit_DFC.yaml
 scqubits/tests/data/circuit_fluxonium.yaml
 scqubits/tests/data/circuit_zeropi.yaml
 scqubits/tests/data/cos2phiqubit_1.hdf5
 scqubits/tests/data/cos2phiqubit_2.hdf5
 scqubits/tests/data/cos2phiqubit_4.hdf5
 scqubits/tests/data/cos2phiqubit_5.hdf5
```

### Comparing `scqubits-3.1.0/setup.py` & `scqubits-3.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 EXTRA_KWARGS = {}
 
 # version information about scqubits goes here
 MAJOR = 3
 MINOR = 1
-MICRO = 0
+MICRO = 1
 ISRELEASED = True
 
 VERSION = "%d.%d.%d" % (MAJOR, MINOR, MICRO)
 
 CURRENT_DIR = os.path.dirname(os.path.abspath(__file__))
 with open(os.path.join(CURRENT_DIR, "requirements.txt")) as requirements:
     INSTALL_REQUIRES = requirements.read().splitlines()
```

