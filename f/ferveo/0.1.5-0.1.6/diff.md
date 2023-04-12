# Comparing `tmp/ferveo-0.1.5.tar.gz` & `tmp/ferveo-0.1.6.tar.gz`

## Comparing `ferveo-0.1.5.tar` & `ferveo-0.1.6.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/Cargo.toml
--rw-rw-r--   0     1000     1000     5872 2023-01-19 15:29:04.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/BENCHMARK.md
--rw-rw-r--   0     1000     1000      470 2023-02-22 13:25:50.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/README.md
--rw-rw-r--   0     1000     1000     9296 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/benches/arkworks.rs
--rw-rw-r--   0     1000     1000    19274 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/benches/tpke.rs
--rw-rw-r--   0     1000     1000     1076 2023-02-22 13:46:31.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/api.rs
--rw-rw-r--   0     1000     1000     7932 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/ciphertext.rs
--rw-rw-r--   0     1000     1000     5585 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/combine.rs
--rw-rw-r--   0     1000     1000     3481 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/context.rs
--rw-rw-r--   0     1000     1000    11777 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/decryption.rs
--rw-rw-r--   0     1000     1000     4428 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs
--rw-rw-r--   0     1000     1000     2191 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/key_share.rs
--rw-rw-r--   0     1000     1000    29061 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/lib.rs
--rw-rw-r--   0     1000     1000     3506 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/refresh.rs
--rw-r--r--   0        0        0     1513 1970-01-01 00:00:00.000000 ferveo-0.1.5/local_dependencies/ferveo/Cargo.toml
--rw-rw-r--   0     1000     1000    51910 2023-02-22 13:46:31.000000 ferveo-0.1.5/local_dependencies/ferveo/Cargo.lock
--rw-rw-r--   0     1000     1000      111 2023-02-22 13:25:50.000000 ferveo-0.1.5/local_dependencies/ferveo/README.md
--rw-rw-r--   0     1000     1000      214 2023-02-22 13:46:31.000000 ferveo-0.1.5/local_dependencies/ferveo/benches/bench_main.rs
--rw-rw-r--   0     1000     1000     3863 2023-02-22 13:46:31.000000 ferveo-0.1.5/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs
--rw-rw-r--   0     1000     1000       71 2023-02-02 09:17:09.000000 ferveo-0.1.5/local_dependencies/ferveo/benches/benchmarks/mod.rs
--rw-rw-r--   0     1000     1000    11868 2023-02-22 13:46:31.000000 ferveo-0.1.5/local_dependencies/ferveo/benches/benchmarks/pairing.rs
--rw-rw-r--   0     1000     1000     3544 2023-02-22 13:46:31.000000 ferveo-0.1.5/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs
--rw-rw-r--   0     1000     1000     3207 2023-02-22 13:46:31.000000 ferveo-0.1.5/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs
--rw-rw-r--   0     1000     1000     4137 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo/examples/bench_primitives_size.rs
--rw-rw-r--   0     1000     1000     2326 2023-02-22 13:46:31.000000 ferveo-0.1.5/local_dependencies/ferveo/examples/pvdkg.rs
--rw-rw-r--   0     1000     1000     6910 2023-02-22 17:24:57.000000 ferveo-0.1.5/local_dependencies/ferveo/src/api.rs
--rw-rw-r--   0     1000     1000      776 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo/src/dkg/common.rs
--rw-rw-r--   0     1000     1000    24357 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo/src/dkg/pv.rs
--rw-rw-r--   0     1000     1000      829 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo/src/dkg.rs
--rw-rw-r--   0     1000     1000    14602 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo/src/lib.rs
--rw-rw-r--   0     1000     1000      570 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo/src/primitives.rs
--rw-rw-r--   0     1000     1000    19365 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo/src/vss/pvss.rs
--rw-rw-r--   0     1000     1000      924 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo/src/vss.rs
--rw-r--r--   0        0        0      297 1970-01-01 00:00:00.000000 ferveo-0.1.5/local_dependencies/subproductdomain/Cargo.toml
--rw-rw-r--   0     1000     1000    16816 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/subproductdomain/src/lib.rs
--rw-r--r--   0        0        0      369 1970-01-01 00:00:00.000000 ferveo-0.1.5/local_dependencies/ferveo-common/Cargo.toml
--rw-rw-r--   0     1000     1000     1505 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo-common/src/keypair.rs
--rw-rw-r--   0     1000     1000      798 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo-common/src/lib.rs
--rw-rw-r--   0     1000     1000     4013 2023-02-22 13:56:25.000000 ferveo-0.1.5/local_dependencies/ferveo-common/src/serialization.rs
--rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 ferveo-0.1.5/Cargo.toml
--rw-rw-r--   0     1000     1000       54 2023-02-22 13:46:31.000000 ferveo-0.1.5/.gitignore
--rwxrwxr-x   0     1000     1000    34916 2023-02-22 13:46:31.000000 ferveo-0.1.5/LICENSE
--rw-rw-r--   0     1000     1000       77 2023-02-22 13:46:31.000000 ferveo-0.1.5/MANIFEST.in
--rw-rw-r--   0     1000     1000      161 2023-02-22 13:46:31.000000 ferveo-0.1.5/README.md
--rw-rw-r--   0     1000     1000       71 2023-02-22 13:46:31.000000 ferveo-0.1.5/build.rs
--rw-rw-r--   0     1000     1000     2654 2023-02-22 17:25:40.000000 ferveo-0.1.5/examples/server_api.py
--rw-rw-r--   0     1000     1000      261 2023-02-22 17:01:29.000000 ferveo-0.1.5/ferveo/__init__.py
--rw-rw-r--   0     1000     1000     1417 2023-02-22 13:46:31.000000 ferveo-0.1.5/ferveo/__init__.pyi
--rw-rw-r--   0     1000     1000        0 2023-02-22 13:46:31.000000 ferveo-0.1.5/ferveo/py.typed
--rw-rw-r--   0     1000     1000      316 2023-02-22 16:50:58.000000 ferveo-0.1.5/pyproject.toml
--rw-rw-r--   0     1000     1000     1444 2023-02-22 17:19:37.000000 ferveo-0.1.5/setup.py
--rw-rw-r--   0     1000     1000     7517 2023-02-22 17:24:04.000000 ferveo-0.1.5/src/lib.rs
--rw-rw-r--   0     1000     1000    58565 2023-02-22 17:19:43.000000 ferveo-0.1.5/Cargo.lock
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 ferveo-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/Cargo.toml
+-rw-rw-r--   0     1000     1000     5872 2023-01-19 15:29:04.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/BENCHMARK.md
+-rw-rw-r--   0     1000     1000      470 2023-04-05 16:16:20.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/README.md
+-rw-rw-r--   0     1000     1000     9295 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/benches/arkworks.rs
+-rw-rw-r--   0     1000     1000    19243 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/benches/tpke.rs
+-rw-rw-r--   0     1000     1000     1674 2023-04-12 08:07:58.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/api.rs
+-rw-rw-r--   0     1000     1000     7782 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/ciphertext.rs
+-rw-rw-r--   0     1000     1000     5517 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/combine.rs
+-rw-rw-r--   0     1000     1000     3471 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/context.rs
+-rw-rw-r--   0     1000     1000    11755 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/decryption.rs
+-rw-rw-r--   0     1000     1000     4254 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs
+-rw-rw-r--   0     1000     1000     2179 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/key_share.rs
+-rw-rw-r--   0     1000     1000    28991 2023-04-12 09:44:49.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/lib.rs
+-rw-rw-r--   0     1000     1000     3487 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/refresh.rs
+-rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 ferveo-0.1.6/local_dependencies/ferveo/Cargo.toml
+-rw-rw-r--   0     1000     1000    51910 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/Cargo.lock
+-rw-rw-r--   0     1000     1000      111 2023-04-05 16:16:20.000000 ferveo-0.1.6/local_dependencies/ferveo/README.md
+-rw-rw-r--   0     1000     1000      214 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/bench_main.rs
+-rw-rw-r--   0     1000     1000     3863 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs
+-rw-rw-r--   0     1000     1000       71 2023-04-05 16:15:54.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/mod.rs
+-rw-rw-r--   0     1000     1000    11868 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/pairing.rs
+-rw-rw-r--   0     1000     1000     3516 2023-04-12 09:05:33.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs
+-rw-rw-r--   0     1000     1000     3207 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs
+-rw-rw-r--   0     1000     1000     4131 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/examples/bench_primitives_size.rs
+-rw-rw-r--   0     1000     1000     2326 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/examples/pvdkg.rs
+-rw-rw-r--   0     1000     1000     6932 2023-04-12 08:08:03.000000 ferveo-0.1.6/local_dependencies/ferveo/src/api.rs
+-rw-rw-r--   0     1000     1000      410 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/src/dkg/common.rs
+-rw-rw-r--   0     1000     1000    23980 2023-04-12 08:07:58.000000 ferveo-0.1.6/local_dependencies/ferveo/src/dkg/pv.rs
+-rw-rw-r--   0     1000     1000      547 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/src/dkg.rs
+-rw-rw-r--   0     1000     1000    16561 2023-04-12 08:07:58.000000 ferveo-0.1.6/local_dependencies/ferveo/src/lib.rs
+-rw-rw-r--   0     1000     1000      560 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/src/primitives.rs
+-rw-rw-r--   0     1000     1000    19002 2023-04-12 08:07:58.000000 ferveo-0.1.6/local_dependencies/ferveo/src/vss/pvss.rs
+-rw-rw-r--   0     1000     1000      558 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/ferveo/src/vss.rs
+-rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 ferveo-0.1.6/local_dependencies/ferveo-common/Cargo.toml
+-rw-rw-r--   0     1000     1000     2469 2023-04-12 09:49:44.000000 ferveo-0.1.6/local_dependencies/ferveo-common/src/keypair.rs
+-rw-rw-r--   0     1000     1000      831 2023-04-06 21:18:33.000000 ferveo-0.1.6/local_dependencies/ferveo-common/src/lib.rs
+-rw-rw-r--   0     1000     1000     4008 2023-04-06 21:18:33.000000 ferveo-0.1.6/local_dependencies/ferveo-common/src/serialization.rs
+-rw-rw-r--   0     1000     1000       74 2023-04-06 21:18:33.000000 ferveo-0.1.6/local_dependencies/ferveo-common/src/utils.rs
+-rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 ferveo-0.1.6/local_dependencies/subproductdomain/Cargo.toml
+-rw-rw-r--   0     1000     1000    16742 2023-04-06 21:18:34.000000 ferveo-0.1.6/local_dependencies/subproductdomain/src/lib.rs
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 ferveo-0.1.6/Cargo.toml
+-rw-rw-r--   0     1000     1000       54 2023-04-06 21:18:33.000000 ferveo-0.1.6/.gitignore
+-rwxrwxr-x   0     1000     1000    34916 2023-04-06 21:18:33.000000 ferveo-0.1.6/LICENSE
+-rw-rw-r--   0     1000     1000       77 2023-04-06 21:18:33.000000 ferveo-0.1.6/MANIFEST.in
+-rw-rw-r--   0     1000     1000      161 2023-04-06 21:18:33.000000 ferveo-0.1.6/README.md
+-rw-rw-r--   0     1000     1000       71 2023-04-06 21:18:33.000000 ferveo-0.1.6/build.rs
+-rw-rw-r--   0     1000     1000     3369 2023-04-12 08:47:23.000000 ferveo-0.1.6/examples/server_api.py
+-rw-rw-r--   0     1000     1000      303 2023-04-12 08:08:03.000000 ferveo-0.1.6/ferveo/__init__.py
+-rw-rw-r--   0     1000     1000     2383 2023-04-12 09:05:42.000000 ferveo-0.1.6/ferveo/__init__.pyi
+-rw-rw-r--   0     1000     1000        0 2023-04-06 21:18:33.000000 ferveo-0.1.6/ferveo/py.typed
+-rw-rw-r--   0     1000     1000      316 2023-04-11 10:00:55.000000 ferveo-0.1.6/pyproject.toml
+-rw-rw-r--   0     1000     1000     1444 2023-04-12 09:54:09.000000 ferveo-0.1.6/setup.py
+-rw-rw-r--   0     1000     1000     9001 2023-04-12 08:37:18.000000 ferveo-0.1.6/src/lib.rs
+-rw-rw-r--   0     1000     1000    56086 2023-04-12 09:54:10.000000 ferveo-0.1.6/Cargo.lock
+-rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 ferveo-0.1.6/PKG-INFO
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/Cargo.toml` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 readme = "README.md"
 
 [lib]
 bench = false
 
 [features]
 test-common = []
+api = []
 
 [dependencies]
 subproductdomain = { path = "../subproductdomain" }
 ferveo-common = { path = "../ferveo-common" }
 rand_core = "0.6"
 rand = "0.8"
-thiserror = "=1.0.30"
-anyhow = "=1.0"
+thiserror = "1.0"
 miracl_core = "=2.3.0"
 ark-ff = "0.4"
 ark-ec = "0.4"
 ark-poly = "0.4"
 ark-serialize = "0.4"
 ark-std = "0.4"
 ark-bls12-381 = "0.4"
@@ -32,21 +32,20 @@
 chacha20poly1305 = "0.10.1"
 serde = { version = "1.0", features = ["derive"] }
 serde_with = "2.0.1"
 bincode = "1.3.3"
 sha2 = "0.10.6"
 serde_bytes = "0.11.9"
 
+[package.metadata.cargo-machete]
+ignored = ["serde_bytes"]
+
 [[bench]]
 name = "tpke"
 path = "benches/tpke.rs"
 harness = false
 required-features = ["test-common"]
 
 [[bench]]
 name = "arkworks"
 path = "benches/arkworks.rs"
 harness = false
-
-[profile.release]
-opt-level = 3
-lto = true
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/BENCHMARK.md` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/BENCHMARK.md`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/benches/arkworks.rs` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/benches/arkworks.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 #![allow(clippy::unit_arg)]
 
 use std::ops::Mul;
 
 use ark_bls12_381::{
     Bls12_381, Fr, G1Affine, G1Projective, G2Affine, G2Projective,
 };
-use ark_ec::pairing::{prepare_g1, prepare_g2, Pairing};
-use ark_ec::{AffineRepr, CurveGroup};
+use ark_ec::{
+    pairing::{prepare_g1, prepare_g2, Pairing},
+    AffineRepr, CurveGroup,
+};
 use ark_ff::{BigInteger256, Field, One, UniformRand, Zero};
 use criterion::{
     black_box, criterion_group, criterion_main, BenchmarkId, Criterion,
 };
 use group_threshold_cryptography::make_random_polynomial_at;
 use itertools::izip;
 use rand::prelude::StdRng;
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/benches/tpke.rs` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/benches/tpke.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #![allow(clippy::redundant_closure)]
 
 use std::collections::HashMap;
 
 use ark_bls12_381::{Bls12_381, Fr, G1Affine as G1, G2Affine as G2};
-use ark_ec::pairing::Pairing;
-use ark_ec::AffineRepr;
+use ark_ec::{pairing::Pairing, AffineRepr};
 use ark_ff::Zero;
 use criterion::{
     black_box, criterion_group, criterion_main, BenchmarkId, Criterion,
 };
-use group_threshold_cryptography::test_common::{setup_fast, setup_simple};
-use group_threshold_cryptography::*;
+use group_threshold_cryptography::{
+    test_common::{setup_fast, setup_simple},
+    *,
+};
 use rand::prelude::StdRng;
 use rand_core::{RngCore, SeedableRng};
 
 const NUM_SHARES_CASES: [usize; 5] = [4, 8, 16, 32, 64];
 const MSG_SIZE_CASES: [usize; 7] = [256, 512, 1024, 2048, 4096, 8192, 16384];
 
 type E = Bls12_381;
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/ciphertext.rs` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/ciphertext.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 use std::ops::Mul;
 
-use ark_ec::pairing::Pairing;
-use ark_ec::AffineRepr;
+use ark_ec::{pairing::Pairing, AffineRepr};
 use ark_ff::{One, UniformRand};
 use ark_serialize::{CanonicalSerialize, Compress};
 use chacha20poly1305::{
     aead::{generic_array::GenericArray, Aead, KeyInit},
     ChaCha20Poly1305, Nonce,
 };
 use ferveo_common::serialization;
 use serde::{Deserialize, Serialize};
 use serde_with::serde_as;
 use sha2::{digest::Digest, Sha256};
 
-use crate::{htp_bls12381_g2, Result, ThresholdEncryptionError};
+use crate::{htp_bls12381_g2, Error, Result};
 
 #[serde_as]
 #[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
 pub struct Ciphertext<E: Pairing> {
     #[serde_as(as = "serialization::SerdeAs")]
     pub commitment: E::G1Affine,
     // U
@@ -72,15 +71,15 @@
     let product = E::pairing(ry_prep, h_gen).0;
     // u
     let commitment = g_gen.mul(rand_element).into();
 
     let nonce = nonce_from_commitment::<E>(commitment)?;
     let ciphertext = shared_secret_to_chacha::<E>(&product)?
         .encrypt(&nonce, message)
-        .map_err(ThresholdEncryptionError::SymmetricEncryptionError)?
+        .map_err(Error::SymmetricEncryptionError)?
         .to_vec();
     // w
     let auth_tag = construct_tag_hash::<E>(commitment, &ciphertext, aad)?
         .mul(rand_element)
         .into();
 
     // TODO: Consider adding aad to the Ciphertext struct
@@ -112,15 +111,15 @@
         [hash_g2, c.auth_tag.into()],
     )
     .0 == E::TargetField::one();
 
     if is_ciphertext_valid {
         Ok(())
     } else {
-        Err(ThresholdEncryptionError::CiphertextVerificationFailed.into())
+        Err(Error::CiphertextVerificationFailed)
     }
 }
 
 pub fn decrypt_symmetric<E: Pairing>(
     ciphertext: &Ciphertext<E>,
     aad: &[u8],
     private_key: &E::G2Affine,
@@ -140,15 +139,15 @@
     shared_secret: &E::TargetField,
 ) -> Result<Vec<u8>> {
     let nonce = nonce_from_commitment::<E>(ciphertext.commitment)?;
     let ciphertext = ciphertext.ciphertext.to_vec();
 
     let plaintext = shared_secret_to_chacha::<E>(shared_secret)?
         .decrypt(&nonce, ciphertext.as_ref())
-        .map_err(|_| ThresholdEncryptionError::CiphertextVerificationFailed)?
+        .map_err(|_| Error::CiphertextVerificationFailed)?
         .to_vec();
 
     Ok(plaintext)
 }
 
 pub fn decrypt_with_shared_secret<E: Pairing>(
     ciphertext: &Ciphertext<E>,
@@ -186,17 +185,16 @@
 
 fn hash_to_g2<T: ark_serialize::CanonicalDeserialize>(
     message: &[u8],
 ) -> Result<T> {
     let point = htp_bls12381_g2(message);
     let mut point_ser: Vec<u8> = Vec::new();
     point.serialize_uncompressed(&mut point_ser)?;
-    T::deserialize_uncompressed(&point_ser[..]).map_err(|err| {
-        ThresholdEncryptionError::ArkworksSerializationError(err).into()
-    })
+    T::deserialize_uncompressed(&point_ser[..])
+        .map_err(Error::ArkworksSerializationError)
 }
 
 fn construct_tag_hash<E: Pairing>(
     commitment: E::G1Affine,
     stream_ciphertext: &[u8],
     aad: &[u8],
 ) -> Result<E::G2Affine> {
@@ -208,16 +206,15 @@
 }
 
 #[cfg(test)]
 mod tests {
 
     use ark_std::test_rng;
 
-    use crate::test_common::*;
-    use crate::*;
+    use crate::{test_common::*, *};
 
     type E = ark_bls12_381::Bls12_381;
 
     #[test]
     fn symmetric_encryption() {
         let rng = &mut test_rng();
         let shares_num = 16;
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/combine.rs` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/combine.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 use ark_ec::{pairing::Pairing, CurveGroup};
 use ark_ff::{Field, One, PrimeField, Zero};
 use itertools::izip;
 use subproductdomain::SubproductDomain;
 
 use crate::{
     verify_decryption_shares_fast, Ciphertext, DecryptionShareFast,
-    DecryptionShareSimple, DecryptionShareSimplePrecomputed,
-    PublicDecryptionContextFast, Result, ThresholdEncryptionError,
+    DecryptionShareSimple, DecryptionShareSimplePrecomputed, Error,
+    PublicDecryptionContextFast, Result,
 };
 
 pub fn prepare_combine_fast<E: Pairing>(
     public_decryption_contexts: &[PublicDecryptionContextFast<E>],
     shares: &[DecryptionShareFast<E>],
 ) -> Vec<E::G2Prepared> {
     let mut domain = vec![]; // omega_i, vector of domain points
@@ -102,17 +102,15 @@
 ) -> Result<E::TargetField> {
     let is_valid_shares = verify_decryption_shares_fast(
         pub_contexts,
         ciphertext,
         decryption_shares,
     );
     if !is_valid_shares {
-        return Err(
-            ThresholdEncryptionError::DecryptionShareVerificationFailed.into(),
-        );
+        return Err(Error::DecryptionShareVerificationFailed);
     }
     Ok(share_combine_fast_unchecked(
         decryption_shares,
         prepared_key_shares,
     ))
 }
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/context.rs` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/context.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use std::ops::Mul;
 
-use ark_ec::pairing::Pairing;
-use ark_ec::CurveGroup;
+use ark_ec::{pairing::Pairing, CurveGroup};
 
 use crate::{
     check_ciphertext_validity, prepare_combine_simple, BlindedKeyShare,
     Ciphertext, DecryptionShareFast, DecryptionShareSimple,
     DecryptionShareSimplePrecomputed, PrivateKeyShare, PublicKeyShare, Result,
 };
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/decryption.rs` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/decryption.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 use std::ops::Mul;
 
-use anyhow::Result;
-use ark_ec::pairing::Pairing;
-use ark_ec::CurveGroup;
+use ark_ec::{pairing::Pairing, CurveGroup};
 use ark_ff::{Field, One, Zero};
 use ferveo_common::serialization;
 use itertools::{izip, zip_eq};
 use rand_core::RngCore;
 use serde::{de::DeserializeOwned, Deserialize, Serialize};
 use serde_with::serde_as;
 
 use crate::{
     check_ciphertext_validity, generate_random, Ciphertext, PrivateKeyShare,
-    PublicDecryptionContextFast, PublicDecryptionContextSimple,
+    PublicDecryptionContextFast, PublicDecryptionContextSimple, Result,
 };
 
 #[serde_as]
 #[derive(Debug, Clone, Serialize, Deserialize)]
 pub struct DecryptionShareFast<E: Pairing> {
     pub decrypter_index: usize,
     #[serde_as(as = "serialization::SerdeAs")]
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 #![allow(non_snake_case)]
 #![allow(clippy::many_single_char_names)]
 #![allow(clippy::zero_prefixed_literal)]
 #![allow(dead_code)]
 
 use ark_bls12_381::g2::Config;
-use ark_ec::short_weierstrass::Affine;
-use ark_ec::AffineRepr;
-use miracl_core::bls12381::big::BIG;
-use miracl_core::bls12381::dbig::DBIG;
-use miracl_core::bls12381::ecp;
-use miracl_core::bls12381::ecp2::ECP2;
-use miracl_core::bls12381::fp::FP;
-use miracl_core::bls12381::fp2::FP2;
-use miracl_core::bls12381::rom;
-use miracl_core::hmac;
+use ark_ec::{short_weierstrass::Affine, AffineRepr};
+use miracl_core::{
+    bls12381::{big::BIG, dbig::DBIG, ecp, ecp2::ECP2, fp::FP, fp2::FP2, rom},
+    hmac,
+};
 
 fn ceil(a: usize, b: usize) -> usize {
     (a - 1) / b + 1
 }
 
 fn hash_to_field2_bls12381(
     hash: usize,
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/key_share.rs` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/key_share.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 use std::ops::Mul;
 
-use ark_ec::pairing::Pairing;
-use ark_ec::{AffineRepr, CurveGroup};
+use ark_ec::{pairing::Pairing, AffineRepr, CurveGroup};
 use ark_ff::One;
 use ark_std::UniformRand;
 use rand_core::RngCore;
 
 #[derive(Debug, Clone)]
 pub struct PublicKeyShare<E: Pairing> {
     pub public_key_share: E::G1Affine, // A_{i, \omega_i}
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/lib.rs` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 pub use combine::*;
 pub use context::*;
 pub use decryption::*;
 pub use hash_to_curve::*;
 pub use key_share::*;
 pub use refresh::*;
 
-// TODO: Turn into a crate features
+#[cfg(feature = "api")]
 pub mod api;
 
 #[derive(Debug, thiserror::Error)]
-pub enum ThresholdEncryptionError {
+pub enum Error {
     /// Ciphertext verification failed
     /// Refers to the check 4.4.2 in the paper: https://eprint.iacr.org/2022/898.pdf
     #[error("Ciphertext verification failed")]
     CiphertextVerificationFailed,
 
     /// Symmetric ciphertext decryption failed
     #[error("Ciphertext decryption failed")]
@@ -59,29 +59,29 @@
     SymmetricEncryptionError(chacha20poly1305::aead::Error),
 
     /// Serialization failed
     #[error("Arkworks serialization failed")]
     ArkworksSerializationError(#[from] ark_serialize::SerializationError),
 }
 
-pub type Result<T> = anyhow::Result<T>;
+pub type Result<T> = std::result::Result<T, Error>;
 
 /// Factory functions for testing
 #[cfg(any(test, feature = "test-common"))]
 pub mod test_common {
-    use std::ops::Mul;
-    use std::usize;
+    use std::{ops::Mul, usize};
 
     pub use ark_bls12_381::Bls12_381 as EllipticCurve;
     use ark_ec::{pairing::Pairing, AffineRepr};
     pub use ark_ff::UniformRand;
     use ark_ff::{Field, One, Zero};
-    use ark_poly::univariate::DensePolynomial;
-    use ark_poly::DenseUVPolynomial;
-    use ark_poly::{EvaluationDomain, Polynomial};
+    use ark_poly::{
+        univariate::DensePolynomial, DenseUVPolynomial, EvaluationDomain,
+        Polynomial,
+    };
     use itertools::izip;
     use rand_core::RngCore;
     use subproductdomain::fast_multiexp;
 
     pub use super::*;
 
     pub fn setup_fast<E: Pairing>(
@@ -270,32 +270,31 @@
 
         (pubkey.into(), privkey.into(), private_contexts)
     }
 }
 
 #[cfg(test)]
 mod tests {
-    use std::collections::HashMap;
-    use std::ops::Mul;
+    use std::{collections::HashMap, ops::Mul};
 
     use ark_bls12_381::Fr;
-    use ark_ec::pairing::Pairing;
-    use ark_ec::{AffineRepr, CurveGroup};
+    use ark_ec::{pairing::Pairing, AffineRepr, CurveGroup};
     use ark_ff::Zero;
     use ark_std::{test_rng, UniformRand};
     use ferveo_common::{FromBytes, ToBytes};
     use rand_core::RngCore;
 
-    use crate::refresh::{
-        make_random_polynomial_at, prepare_share_updates_for_recovery,
-        recover_share_from_updated_private_shares, refresh_private_key_share,
-        update_share_for_recovery,
+    use crate::{
+        refresh::{
+            make_random_polynomial_at, prepare_share_updates_for_recovery,
+            recover_share_from_updated_private_shares,
+            refresh_private_key_share, update_share_for_recovery,
+        },
+        test_common::{setup_simple, *},
     };
-    use crate::test_common::setup_simple;
-    use crate::test_common::*;
 
     type E = ark_bls12_381::Bls12_381;
     type TargetField = <E as Pairing>::TargetField;
     type ScalarField = <E as Pairing>::ScalarField;
 
     fn make_shared_secret_from_contexts<E: Pairing>(
         contexts: &[PrivateDecryptionContextSimple<E>],
```

### Comparing `ferveo-0.1.5/local_dependencies/group-threshold-cryptography/src/refresh.rs` & `ferveo-0.1.6/local_dependencies/group-threshold-cryptography/src/refresh.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-use std::ops::Mul;
-use std::usize;
+use std::{ops::Mul, usize};
 
-use ark_ec::pairing::Pairing;
-use ark_ec::{AffineRepr, CurveGroup};
+use ark_ec::{pairing::Pairing, AffineRepr, CurveGroup};
 use ark_ff::Zero;
 use ark_poly::{univariate::DensePolynomial, DenseUVPolynomial, Polynomial};
 use itertools::zip_eq;
 use rand_core::RngCore;
 
 use crate::{lagrange_basis_at, PrivateKeyShare};
```

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/Cargo.toml` & `ferveo-0.1.6/local_dependencies/ferveo/Cargo.toml`

 * *Files 13% similar despite different names*

```diff
@@ -7,41 +7,34 @@
 readme = "README.md"
 description = "An implementation of a DKG protocol for front-running protection on public blockchains."
 keywords = ["DKG"]
 categories = ["cryptography"]
 authors = ["Heliax AG <hello@heliax.dev>"]
 
 [dependencies]
-group-threshold-cryptography = { path = "../group-threshold-cryptography" }
+group-threshold-cryptography = { path = "../group-threshold-cryptography", features = ["api"] }
 ferveo-common = { path = "../ferveo-common" }
 subproductdomain = { path = "../subproductdomain" }
 ark-std = "0.4"
 ark-bls12-381 = "0.4"
 ark-ec = "0.4"
 ark-ff = "0.4"
-ark-serialize = "0.4"
 ark-poly = "0.4"
 rand = "0.8"
 rand_old = { package = "rand", version = "0.7" } # used by benchmarks/pairing.rs
-either = "1.6.1"
-miracl_core = "2.3.0"
-ed25519-dalek = { version = "1", features = ["serde", "batch"] }
 serde = { version = "1.0", features = ["derive"] }
-zeroize = { version = "1", default-features = false, features = ["zeroize_derive"] }
-serde_bytes = { version = "0.11" }
 bincode = "1.3"
-anyhow = "1.0"
-subtle = "2.4"
 itertools = "0.10.1"
 measure_time = "0.8"
 rand_core = "0.6.4"
 serde_with = "2.0.1"
+thiserror = "1.0"
 
-[package.metadata.cargo-udeps.ignore]
-development = ["pprof"]
+[package.metadata.cargo-machete]
+ignored = ["ark-serialize"]
 
 [lib]
 bench = false
 
 [features]
 test-common = []
 
@@ -54,11 +47,7 @@
 #path = "benches/benchmarks/pvdkg.rs"
 #harness = false
 
 [[bench]]
 name = "benchmarks"
 path = "benches/bench_main.rs"
 harness = false
-
-[profile.release]
-opt-level = 3
-lto = true
```

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/Cargo.lock` & `ferveo-0.1.6/local_dependencies/ferveo/Cargo.lock`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs` & `ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/benches/benchmarks/pairing.rs` & `ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/pairing.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs` & `ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     let shares_num = 300;
     PubliclyVerifiableDkg::new(
         validators,
         Params {
             tau: 0,
             security_threshold: shares_num / 3,
             shares_num,
-            retry_after: 2,
         },
         &me,
         keypairs[validator],
     )
     .expect("Setup failed")
 }
```

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs` & `ferveo-0.1.6/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/examples/bench_primitives_size.rs` & `ferveo-0.1.6/local_dependencies/ferveo/examples/bench_primitives_size.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-use std::collections::BTreeSet;
-use std::fs::{create_dir_all, OpenOptions};
-use std::io::prelude::*;
-use std::path::PathBuf;
+use std::{
+    collections::BTreeSet,
+    fs::{create_dir_all, OpenOptions},
+    io::prelude::*,
+    path::PathBuf,
+};
 
 use ark_bls12_381::Bls12_381 as EllipticCurve;
 use ferveo::*;
 use ferveo_common::ExternalValidator;
 use itertools::iproduct;
 use rand::prelude::StdRng;
 use rand_core::SeedableRng;
```

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/examples/pvdkg.rs` & `ferveo-0.1.6/local_dependencies/ferveo/examples/pvdkg.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/src/api.rs` & `ferveo-0.1.6/local_dependencies/ferveo/src/api.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 use ark_poly::EvaluationDomain;
-use ark_serialize::{CanonicalDeserialize, CanonicalSerialize};
-use ferveo_common::serialization::ser::serialize;
+use ferveo_common::serialization;
 pub use ferveo_common::{ExternalValidator, Keypair, PublicKey};
 use group_threshold_cryptography as tpke;
-use rand::rngs::StdRng;
-use rand::{thread_rng, RngCore, SeedableRng};
+use rand::RngCore;
 use serde::{Deserialize, Serialize};
+use serde_with::serde_as;
 pub use tpke::api::{
     decrypt_with_shared_secret, encrypt, share_combine_simple_precomputed,
     Ciphertext, DecryptionShareSimplePrecomputed as DecryptionShare,
-    DkgPublicKey, G1Prepared, Result, SharedSecret, UnblindingKey, E,
+    DkgPublicKey, G1Prepared, SharedSecret, UnblindingKey, E,
 };
 
-pub use crate::PubliclyVerifiableSS as Transcript;
+pub use crate::{PubliclyVerifiableSS as Transcript, Result};
 
 #[derive(Clone)]
 pub struct Dkg(crate::PubliclyVerifiableDkg<E>);
 
 impl Dkg {
     pub fn new(
         tau: u64,
@@ -39,15 +38,15 @@
             me,
             session_keypair,
         )?;
         Ok(Self(dkg))
     }
 
     pub fn final_key(&self) -> DkgPublicKey {
-        self.0.final_key()
+        DkgPublicKey(self.0.final_key())
     }
 
     pub fn generate_transcript<R: RngCore>(
         &self,
         rng: &mut R,
     ) -> Result<crate::PubliclyVerifiableSS<E>> {
         self.0.create_share(rng)
@@ -61,16 +60,18 @@
         // TODO: Rewrite `deal` to not require mutability after validating this API design
         for (validator, transcript) in messages {
             self.0.deal(validator.clone(), transcript.clone())?;
         }
         Ok(AggregatedTranscript(crate::pvss::aggregate(&self.0)))
     }
 
-    pub fn g1_inv(&self) -> G1Prepared {
-        self.0.pvss_params.g_inv()
+    pub fn public_params(&self) -> DkgPublicParameters {
+        DkgPublicParameters {
+            g1_inv: self.0.pvss_params.g_inv(),
+        }
     }
 }
 
 #[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
 pub struct AggregatedTranscript(
     crate::PubliclyVerifiableSS<E, crate::Aggregated>,
 );
@@ -95,32 +96,37 @@
             dkg.0.me,
             &domain_points,
             &dkg.0.pvss_params.g_inv(),
         )
     }
 }
 
+#[serde_as]
+#[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
+pub struct DkgPublicParameters {
+    #[serde_as(as = "serialization::SerdeAs")]
+    pub g1_inv: G1Prepared,
+}
+
+impl DkgPublicParameters {
+    pub fn from_bytes(bytes: &[u8]) -> Self {
+        bincode::deserialize(bytes).unwrap()
+    }
+
+    pub fn to_bytes(&self) -> Vec<u8> {
+        bincode::serialize(self).unwrap()
+    }
+}
+
 #[cfg(test)]
 mod test_ferveo_api {
-    use std::collections::HashMap;
-    use std::fmt::format;
-
-    use ark_bls12_381::{Bls12_381 as E, G2Projective};
-    use ark_ec::CurveGroup;
-    use ark_poly::EvaluationDomain;
-    use ark_serialize::CanonicalSerialize;
-    use ark_std::UniformRand;
-    use ferveo_common::PublicKey;
-    use group_threshold_cryptography as tpke;
-    use itertools::{iproduct, izip};
-    use rand::prelude::StdRng;
-    use rand::SeedableRng;
+    use itertools::izip;
+    use rand::{prelude::StdRng, thread_rng, SeedableRng};
 
-    use crate::api::*;
-    use crate::dkg::test_common::*;
+    use crate::{api::*, dkg::test_common::*};
 
     #[test]
     fn test_server_api_simple_tdec_precomputed() {
         let rng = &mut StdRng::seed_from_u64(0);
 
         let tau = 1;
         let security_threshold = 3;
@@ -164,15 +170,15 @@
         // At this point, any given validator should be able to provide a DKG public key
         let public_key = dkg.final_key();
 
         // In the meantime, the client creates a ciphertext and decryption request
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
         let rng = &mut thread_rng();
-        let ciphertext = encrypt(msg, aad, &public_key, rng).unwrap();
+        let ciphertext = encrypt(msg, aad, &public_key.0, rng).unwrap();
 
         // Having aggregated the transcripts, the validators can now create decryption shares
         let decryption_shares: Vec<_> = izip!(&validators, &validator_keypairs)
             .map(|(validator, validator_keypair)| {
                 // Each validator holds their own instance of DKG and creates their own aggregate
                 let mut dkg = Dkg::new(
                     tau,
```

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/src/dkg/pv.rs` & `ferveo-0.1.6/local_dependencies/ferveo/src/dkg/pv.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,20 @@
 use std::collections::BTreeMap;
-use std::collections::HashMap;
 
-use anyhow::Context;
-use anyhow::{anyhow, Result};
-use ark_ec::bn::TwistType::D;
-use ark_ec::pairing::Pairing;
-use ark_ec::{AffineRepr, CurveGroup, Group};
-use ark_ff::{Field, One, PrimeField, Zero};
-use ark_poly::{polynomial::univariate::DensePolynomial, EvaluationDomain};
-use ark_serialize::*;
-use ark_std::{end_timer, start_timer};
-use ferveo_common::Rng;
-use ferveo_common::{ExternalValidator, PublicKey};
-use group_threshold_cryptography as tpke;
-use itertools::{izip, zip_eq};
+use ark_ec::{pairing::Pairing, AffineRepr, CurveGroup, Group};
+use ark_poly::EvaluationDomain;
+use ferveo_common::{is_power_of_2, ExternalValidator};
 use measure_time::print_time;
 use rand::RngCore;
 use serde::{de::DeserializeOwned, Deserialize, Serialize};
 use serde_with::serde_as;
 
 use crate::{
-    aggregate, make_validators, AggregatedPvss, DkgState, Params,
-    PubliclyVerifiableParams, PubliclyVerifiableSS, Pvss,
+    aggregate, make_validators, AggregatedPvss, DkgState, Error, Params,
+    PubliclyVerifiableParams, PubliclyVerifiableSS, Pvss, Result,
 };
 
 /// The DKG context that holds all of the local state for participating in the DKG
 // TODO: Consider removing Clone to avoid accidentally NOT-mutating state.
 //  Currently, we're assuming that the DKG is only mutated by the owner of the instance.
 //  Consider removing Clone after finalizing ferveo::api
 #[derive(Clone, Debug)]
@@ -50,24 +39,29 @@
     /// `session_keypair` the keypair for `me`
     pub fn new(
         validators: &[ExternalValidator<E>],
         params: Params,
         me: &ExternalValidator<E>,
         session_keypair: ferveo_common::Keypair<E>,
     ) -> Result<Self> {
-        use ark_std::UniformRand;
+        // Make sure that the number of shares is a power of 2 for the FFT to work (Radix-2 FFT domain is being used)
+        if !is_power_of_2(params.shares_num) {
+            return Err(Error::InvalidShareNumberParameter(params.shares_num));
+        }
+
         let domain = ark_poly::Radix2EvaluationDomain::<E::ScalarField>::new(
             params.shares_num as usize,
         )
-        .ok_or_else(|| anyhow!("unable to construct domain"))?;
+        .expect("unable to construct domain");
 
         // keep track of the owner of this instance in the validator set
-        let me = validators.iter().position(|probe| me == probe).context(
-            "could not find this validator in the provided validator set",
-        )?;
+        let me = validators
+            .iter()
+            .position(|probe| me == probe)
+            .ok_or_else(|| Error::ValidatorNotInSet(me.clone().address))?;
 
         let validators = make_validators(validators);
 
         Ok(Self {
             session_keypair,
             params,
             pvss_params: PubliclyVerifiableParams::<E> {
@@ -85,24 +79,21 @@
         })
     }
 
     /// Create a new PVSS instance within this DKG session, contributing to the final key
     /// `rng` is a cryptographic random number generator
     /// Returns a PVSS dealing message to post on-chain
     pub fn share<R: RngCore>(&mut self, rng: &mut R) -> Result<Message<E>> {
-        use ark_std::UniformRand;
         print_time!("PVSS Sharing");
         let vss = self.create_share(rng)?;
         match self.state {
             DkgState::Sharing { .. } | DkgState::Dealt => {
                 Ok(Message::Deal(vss))
             }
-            _ => {
-                Err(anyhow!("DKG is not in a valid state to deal PVSS shares"))
-            }
+            _ => Err(Error::InvalidDkgStateToDeal),
         }
     }
 
     pub fn create_share<R: RngCore>(
         &self,
         rng: &mut R,
     ) -> Result<PubliclyVerifiableSS<E>> {
@@ -116,17 +107,15 @@
             DkgState::Dealt => {
                 let final_key = self.final_key();
                 Ok(Message::Aggregate(Aggregation {
                     vss: aggregate(self),
                     final_key,
                 }))
             }
-            _ => Err(anyhow!(
-                "Not enough PVSS transcripts received to aggregate"
-            )),
+            _ => Err(Error::InvalidDkgStateToAggregate),
         }
     }
 
     /// Returns the public key generated by the DKG
     pub fn final_key(&self) -> E::G1Affine {
         self.vss
             .values()
@@ -140,69 +129,82 @@
     /// `payload` is the content of the message
     pub fn verify_message(
         &self,
         sender: &ExternalValidator<E>,
         payload: &Message<E>,
     ) -> Result<()> {
         match payload {
-            Message::Deal(pvss) if matches!(self.state, DkgState::Sharing { .. } | DkgState::Dealt) => {
+            Message::Deal(pvss)
+                if matches!(
+                    self.state,
+                    DkgState::Sharing { .. } | DkgState::Dealt
+                ) =>
+            {
                 // TODO: If this is two slow, we can convert self.validators to
                 // an address keyed hashmap after partitioning the shares shares
                 // in the [`new`] method
                 let sender = self
                     .validators
                     .iter()
                     .position(|probe| sender == &probe.validator)
-                    .context("dkg received unknown dealer")?;
+                    .ok_or_else(|| {
+                        Error::UnknownDealer(sender.clone().address)
+                    })?;
                 if self.vss.contains_key(&(sender as u32)) {
-                    Err(anyhow!("Repeat dealer {}", sender))
+                    let sender = self.validators[sender].validator.clone();
+                    Err(Error::DuplicateDealer(sender.address))
                 } else if !pvss.verify_optimistic() {
-                    Err(anyhow!("Invalid PVSS transcript"))
+                    Err(Error::InvalidPvssTranscript)
                 } else {
                     Ok(())
                 }
             }
-            Message::Aggregate(Aggregation { vss, final_key }) if matches!(self.state, DkgState::Dealt) => {
-                let minimum_shares = self.params.shares_num - self.params.security_threshold;
+            Message::Aggregate(Aggregation { vss, final_key })
+                if matches!(self.state, DkgState::Dealt) =>
+            {
+                let minimum_shares =
+                    self.params.shares_num - self.params.security_threshold;
                 let verified_shares = vss.verify_aggregation(self)?;
                 // we reject aggregations that fail to meet the security threshold
                 if verified_shares < minimum_shares {
-                    Err(anyhow!(
-                        "Aggregation failed because the verified shares was insufficient"
+                    Err(Error::InsufficientTranscriptsForAggregate(
+                        minimum_shares,
+                        verified_shares,
                     ))
                 } else if &self.final_key() == final_key {
                     Ok(())
                 } else {
-                    Err(anyhow!(
-                        "The final key was not correctly derived from the aggregated transcripts"
-                    ))
+                    Err(Error::InvalidFinalKey)
                 }
             }
-            _ => Err(anyhow!(
-                "DKG state machine is not in correct state to verify this message"
-            )),
+            _ => Err(Error::InvalidDkgStateToVerify),
         }
     }
 
     /// After consensus has agreed to include a verified
     /// message on the blockchain, we apply the chains
     /// to the state machine
     pub fn apply_message(
         &mut self,
         sender: ExternalValidator<E>,
         payload: Message<E>,
     ) -> Result<()> {
         match payload {
-            Message::Deal(pvss) if matches!(self.state, DkgState::Sharing { .. } | DkgState::Dealt) => {
+            Message::Deal(pvss)
+                if matches!(
+                    self.state,
+                    DkgState::Sharing { .. } | DkgState::Dealt
+                ) =>
+            {
                 // Add the ephemeral public key and pvss transcript
                 let sender = self
                     .validators
                     .iter()
                     .position(|probe| sender.address == probe.validator.address)
-                    .context("dkg received unknown dealer")?;
+                    .ok_or_else(|| Error::UnknownDealer(sender.address))?;
                 self.vss.insert(sender as u32, pvss);
 
                 // we keep track of the amount of shares seen until the security
                 // threshold is met. Then we may change the state of the DKG
                 if let DkgState::Sharing {
                     ref mut accumulated_shares,
                     ..
@@ -218,31 +220,29 @@
             Message::Aggregate(_) if matches!(self.state, DkgState::Dealt) => {
                 // change state and cache the final key
                 self.state = DkgState::Success {
                     final_key: self.final_key(),
                 };
                 Ok(())
             }
-            _ => Err(anyhow!(
-                "DKG state machine is not in correct state to apply this message"
-            )),
+            _ => Err(Error::InvalidDkgStateToIngest),
         }
     }
 
     pub fn deal(
         &mut self,
         sender: ExternalValidator<E>,
         pvss: Pvss<E>,
     ) -> Result<()> {
         // Add the ephemeral public key and pvss transcript
         let sender = self
             .validators
             .iter()
             .position(|probe| sender.address == probe.validator.address)
-            .context("dkg received unknown dealer")?;
+            .ok_or_else(|| Error::UnknownDealer(sender.address))?;
         self.vss.insert(sender as u32, pvss);
         Ok(())
     }
 }
 
 #[serde_as]
 #[derive(Serialize, Deserialize, Clone, Debug)]
@@ -344,18 +344,14 @@
         setup_dealt_dkg_with_n_validators(2, 4)
     }
 
     pub fn setup_dealt_dkg_with_n_validators(
         security_threshold: u32,
         shares_num: u32,
     ) -> PubliclyVerifiableDkg<EllipticCurve> {
-        // Make sure that the number of shares is a power of 2 for the FFT to work (Radix-2 FFT domain is being used)
-        let is_power_of_2 = |n: u32| n != 0 && (n & (n - 1)) == 0;
-        assert!(is_power_of_2(shares_num));
-
         let rng = &mut ark_std::test_rng();
 
         // Gather everyone's transcripts
         let transcripts = (0..shares_num).map(|i| {
             let mut dkg = setup_dkg_for_n_validators(
                 security_threshold,
                 shares_num,
@@ -391,24 +387,21 @@
             &gen_validators(&keypairs),
             Params {
                 tau: 0,
                 security_threshold: 4,
                 shares_num: 8,
             },
             &ExternalValidator::<EllipticCurve> {
-                address: "non-existant-validator".into(),
+                address: "non-existent-validator".into(),
                 public_key: keypair.public(),
             },
             keypair,
         )
         .expect_err("Test failed");
-        assert_eq!(
-            err.to_string(),
-            "could not find this validator in the provided validator set"
-        )
+        assert_eq!(err.to_string(), "Expected validator to be a part of the DKG validator set: non-existent-validator")
     }
 }
 
 /// Test the dealing phase of the DKG
 #[cfg(test)]
 mod test_dealing {
     use ark_ec::AffineRepr;
```

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/src/lib.rs` & `ferveo-0.1.6/local_dependencies/ferveo/src/lib.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,95 @@
-#![allow(unused_imports)]
-
 pub mod api;
 pub mod dkg;
 pub mod primitives;
 mod vss;
 
-// TODO: Replace with concrete error type
-pub use anyhow::Error;
 pub use dkg::*;
+use group_threshold_cryptography as tpke;
 pub use primitives::*;
 pub use vss::*;
 
+#[derive(Debug, thiserror::Error)]
+pub enum Error {
+    /// Threshold encryption error
+    #[error("Threshold encryption error")]
+    ThresholdEncryptionError(#[from] tpke::Error),
+
+    /// Number of shares parameter must be a power of two
+    #[error("Number of shares parameter must be a power of two. Got {0}")]
+    InvalidShareNumberParameter(u32),
+
+    /// DKG is not in a valid state to deal PVSS shares
+    #[error("Invalid DKG state to deal PVSS shares")]
+    InvalidDkgStateToDeal,
+
+    /// DKG is not in a valid state to aggregate PVSS transcripts
+    #[error("Invalid DKG state to aggregate PVSS transcripts")]
+    InvalidDkgStateToAggregate,
+
+    /// DKG is not in a valid state to verify PVSS transcripts
+    #[error("Invalid DKG state to verify PVSS transcripts")]
+    InvalidDkgStateToVerify,
+
+    /// DKG is not in a valid state to ingest PVSS transcripts
+    #[error("Invalid DKG state to ingest PVSS transcripts")]
+    InvalidDkgStateToIngest,
+
+    /// DKG validator set must contain the validator with the given address
+    #[error("Expected validator to be a part of the DKG validator set: {0}")]
+    ValidatorNotInSet(String),
+
+    /// DKG received an unknown dealer. Dealer must be the part of the DKG validator set.
+    #[error("DKG received an unknown dealer: {0}")]
+    UnknownDealer(String),
+
+    /// DKG received a PVSS transcript from a dealer that has already been dealt.
+    #[error("DKG received a PVSS transcript from a dealer that has already been dealt: {0}")]
+    DuplicateDealer(String),
+
+    /// DKG received an invalid transcript for which optimistic verification failed
+    #[error("DKG received an invalid transcript")]
+    InvalidPvssTranscript,
+
+    /// Aggregation failed because the DKG did not receive enough PVSS transcripts
+    #[error(
+        "Insufficient transcripts for aggregation (expected {0}, got {1})"
+    )]
+    InsufficientTranscriptsForAggregate(u32, u32),
+
+    /// Failed to derive a valid final key for the DKG
+    #[error("Failed to derive a valid final key for the DKG")]
+    InvalidFinalKey,
+
+    /// Not enough validators to perform the DKG for a given number of shares
+    #[error("Not enough validators (expected {0}, got {1})")]
+    InsufficientValidators(u32, u32),
+
+    /// Transcript aggregate doesn't match the received PVSS instances
+    #[error("Transcript aggregate doesn't match the received PVSS instances")]
+    InvalidTranscriptAggregate,
+}
+
+pub type Result<T> = std::result::Result<T, Error>;
+
 #[cfg(test)]
 mod test_dkg_full {
     use std::collections::HashMap;
 
-    use anyhow::{anyhow, Result};
-    use ark_bls12_381::{
-        Bls12_381 as E, Bls12_381, Fr, G1Affine, G2Projective,
-    };
-    use ark_ec::bls12::G2Affine;
-    use ark_ec::pairing::Pairing;
-    use ark_ec::{AffineRepr, CurveGroup};
-    use ark_ff::{Field, One, PrimeField, Zero};
-    use ark_ff::{Fp12, UniformRand};
-    use ark_poly::{polynomial::univariate::DensePolynomial, EvaluationDomain};
+    use ark_bls12_381::{Bls12_381 as E, Fr, G1Affine};
+    use ark_ec::{pairing::Pairing, AffineRepr, CurveGroup};
+    use ark_ff::{UniformRand, Zero};
+    use ark_poly::EvaluationDomain;
     use ark_std::test_rng;
-    use ark_std::{end_timer, start_timer};
-    use ferveo_common::Rng;
-    use ferveo_common::{ExternalValidator, Keypair};
+    use ferveo_common::Keypair;
     use group_threshold_cryptography as tpke;
     use group_threshold_cryptography::{
         Ciphertext, DecryptionShareSimple, DecryptionShareSimplePrecomputed,
     };
-    use itertools::Itertools;
-    use itertools::{izip, zip_eq};
-    use measure_time::print_time;
-    use rand::prelude::StdRng;
-    use rand::SeedableRng;
-    use serde::{Deserialize, Serialize};
+    use itertools::{izip, Itertools};
 
     use super::*;
     use crate::dkg::pv::test_common::*;
 
     type TargetField = <E as Pairing>::TargetField;
 
     fn make_shared_secret_simple_tdec(
```

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/src/primitives.rs` & `ferveo-0.1.6/local_dependencies/ferveo/src/primitives.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-use ark_ec::pairing::Pairing;
-use ark_ec::AffineRepr;
+use ark_ec::{pairing::Pairing, AffineRepr};
 
 // pub fn batch_to_projective<A: ark_ec::AffineCurve>(
 //     p: &[A],
 // ) -> Vec<A::Projective> {
 //     p.iter().map(|a| a.into_projective()).collect::<Vec<_>>()
 // }
```

### Comparing `ferveo-0.1.5/local_dependencies/ferveo/src/vss/pvss.rs` & `ferveo-0.1.6/local_dependencies/ferveo/src/vss/pvss.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,32 @@
-use std::collections::BTreeMap;
-use std::collections::HashMap;
-use std::marker::PhantomData;
-use std::ops::{Add, Mul};
-
-use anyhow::{anyhow, Result};
-use ark_ec::bn::G2Affine;
-use ark_ec::pairing::Pairing;
-use ark_ec::{AffineRepr, CurveGroup};
-use ark_ff::UniformRand;
-use ark_ff::{Field, One, PrimeField, Zero};
-use ark_poly::DenseUVPolynomial;
-use ark_poly::{polynomial::univariate::DensePolynomial, EvaluationDomain};
-use ark_serialize::*;
-use ark_std::{end_timer, start_timer};
-use ferveo_common::Rng;
-use ferveo_common::{Keypair, PublicKey};
+use std::{marker::PhantomData, ops::Mul};
+
+use ark_ec::{pairing::Pairing, AffineRepr, CurveGroup};
+use ark_ff::{Field, Zero};
+use ark_poly::{
+    polynomial::univariate::DensePolynomial, DenseUVPolynomial,
+    EvaluationDomain,
+};
 use group_threshold_cryptography as tpke;
-use itertools::izip;
-use itertools::{zip_eq, Itertools};
+use itertools::Itertools;
 use measure_time::print_time;
 use rand::RngCore;
-use serde::{de::DeserializeOwned, Deserialize, Serialize};
+use serde::{Deserialize, Serialize};
 use serde_with::serde_as;
 use subproductdomain::fast_multiexp;
 use tpke::{
     prepare_combine_simple, refresh_private_key_share,
-    update_share_for_recovery, Ciphertext, DecryptionShareFast,
-    DecryptionShareSimple, DecryptionShareSimplePrecomputed, PrivateKeyShare,
+    update_share_for_recovery, Ciphertext, DecryptionShareSimple,
+    DecryptionShareSimplePrecomputed, PrivateKeyShare,
 };
 
-use crate::PubliclyVerifiableDkg;
-use crate::{batch_to_projective_g1, batch_to_projective_g2};
+use crate::{
+    batch_to_projective_g1, batch_to_projective_g2, Error,
+    PubliclyVerifiableDkg, Result,
+};
 
 /// These are the blinded evaluations of shares of a single random polynomial
 pub type ShareEncryptions<E> = <E as Pairing>::G2Affine;
 
 /// Marker struct for unaggregated PVSS transcripts
 #[derive(Serialize, Deserialize, Clone, Debug, PartialEq)]
 pub struct Unaggregated;
@@ -122,16 +114,17 @@
                     // &evals.evals[i..i] = &evals.evals[i]
                     &[evals.evals[val.share_index]], // one share per validator
                     val.validator.public_key.encryption_key.into_group(),
                 )[0]
             })
             .collect::<Vec<ShareEncryptions<E>>>();
         if shares.len() != dkg.validators.len() {
-            return Err(anyhow!(
-                "Not all validator session keys have been announced"
+            return Err(Error::InsufficientValidators(
+                shares.len() as u32,
+                dkg.validators.len() as u32,
             ));
         }
         // phi.zeroize(); // TODO zeroize?
         // TODO: Cross check proof of knowledge check with the whitepaper; this check proves that there is a relationship between the secret and the pvss transcript
         // Sigma is a proof of knowledge of the secret, sigma = h^s
         let sigma = E::G2Affine::generator().mul(*s).into(); //todo hash to curve
         let vss = Self {
@@ -211,17 +204,15 @@
         for (_, pvss) in dkg.vss.iter() {
             y += pvss.coeffs[0].into_group();
             shares_total += 1
         }
         if y.into_affine() == self.coeffs[0] {
             Ok(shares_total)
         } else {
-            Err(anyhow!(
-                "aggregation does not match received PVSS instances"
-            ))
+            Err(Error::InvalidTranscriptAggregate)
         }
     }
 
     pub fn decrypt_private_key_share(
         &self,
         validator_decryption_key: &E::ScalarField,
         validator_index: usize,
@@ -256,16 +247,16 @@
             validator_index,
             validator_decryption_key,
             &private_key_share,
             ciphertext,
             aad,
             g_inv,
         )
+        .map_err(|e| e.into())
     }
-
     pub fn make_decryption_share_simple_precomputed(
         &self,
         ciphertext: &Ciphertext<E>,
         aad: &[u8],
         validator_decryption_key: &E::ScalarField,
         validator_index: usize,
         domain_points: &[E::ScalarField],
@@ -283,14 +274,15 @@
             validator_decryption_key,
             &private_key_share,
             ciphertext,
             aad,
             &lagrange_coeffs[validator_index],
             g_inv,
         )
+        .map_err(|e| e.into())
     }
 
     pub fn refresh_decryption_share(
         &self,
         ciphertext: &Ciphertext<E>,
         aad: &[u8],
         validator_decryption_key: &E::ScalarField,
@@ -314,14 +306,15 @@
             validator_index,
             validator_decryption_key,
             &refreshed_private_key_share,
             ciphertext,
             aad,
             &dkg.pvss_params.g_inv(),
         )
+        .map_err(|e| e.into())
     }
 
     pub fn update_private_key_share_for_recovery(
         &self,
         validator_decryption_key: &E::ScalarField,
         validator_index: usize,
         share_updates: &[E::G2],
@@ -404,15 +397,14 @@
 }
 
 #[cfg(test)]
 mod test_pvss {
     use ark_bls12_381::Bls12_381 as EllipticCurve;
     use ark_ec::AffineRepr;
     use ark_ff::UniformRand;
-    use ferveo_common::ExternalValidator;
 
     use super::*;
     use crate::dkg::pv::test_common::*;
 
     type ScalarField = <EllipticCurve as Pairing>::ScalarField;
     type G1 = <EllipticCurve as Pairing>::G1Affine;
     type G2 = <EllipticCurve as Pairing>::G2Affine;
@@ -505,24 +497,23 @@
         );
     }
 
     /// Check that if the aggregated pvss transcript has an
     /// incorrect constant term, the verification fails
     #[test]
     fn test_verify_aggregation_fails_if_constant_term_wrong() {
-        use std::ops::Neg;
         let dkg = setup_dealt_dkg();
         let mut aggregated = aggregate(&dkg);
         while aggregated.coeffs[0] == G1::zero() {
             let dkg = setup_dkg(0);
             aggregated = aggregate(&dkg);
         }
         aggregated.coeffs[0] = G1::zero();
         assert_eq!(
             aggregated
                 .verify_aggregation(&dkg)
                 .expect_err("Test failed")
                 .to_string(),
-            "aggregation does not match received PVSS instances"
+            "Transcript aggregate doesn't match the received PVSS instances"
         )
     }
 }
```

### Comparing `ferveo-0.1.5/local_dependencies/subproductdomain/src/lib.rs` & `ferveo-0.1.6/local_dependencies/subproductdomain/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 #![allow(non_snake_case)]
 #![allow(dead_code)]
 
 use std::mem;
 
-use ark_ec::pairing::Pairing;
-use ark_ec::scalar_mul::fixed_base::FixedBase;
-use ark_ec::AffineRepr;
-use ark_ec::CurveGroup;
+use ark_ec::{
+    pairing::Pairing, scalar_mul::fixed_base::FixedBase, AffineRepr, CurveGroup,
+};
 use ark_ff::{FftField, Field, Zero};
-use ark_poly::univariate::DensePolynomial;
-use ark_poly::DenseUVPolynomial;
-use ark_poly::EvaluationDomain;
-use ark_poly::{Polynomial, Radix2EvaluationDomain};
+use ark_poly::{
+    univariate::DensePolynomial, DenseUVPolynomial, EvaluationDomain,
+    Polynomial, Radix2EvaluationDomain,
+};
 
 /// Compute a fast multiexp of many scalars times the same base
 /// Only convenient for when called once with given base; if called
 /// more than once, it's faster to save the generated window table
 pub fn fast_multiexp<Group: CurveGroup>(
     scalars: &[Group::ScalarField],
     base: Group,
@@ -382,16 +381,15 @@
     ))
 }
 
 #[cfg(test)]
 mod tests {
     use ark_ec::pairing::Pairing;
     use ark_ff::{One, Zero};
-    use ark_poly::polynomial::univariate::DensePolynomial;
-    use ark_poly::Polynomial;
+    use ark_poly::{polynomial::univariate::DensePolynomial, Polynomial};
     use ark_std::UniformRand;
 
     use super::*;
 
     type ScalarField = <ark_bls12_381::Bls12_381 as Pairing>::ScalarField;
     #[test]
     fn test_inverse() {
```

### Comparing `ferveo-0.1.5/local_dependencies/ferveo-common/src/lib.rs` & `ferveo-0.1.6/local_dependencies/ferveo-common/src/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 use ark_ec::pairing::Pairing;
 
 pub mod keypair;
 pub mod serialization;
+pub mod utils;
 
 pub use keypair::*;
 pub use serialization::*;
+pub use utils::*;
 
 #[derive(Clone, Debug, PartialEq)]
 /// Represents an external validator
 pub struct ExternalValidator<E: Pairing> {
     /// The established address of the validator
     pub address: String,
     /// The Public key
```

### Comparing `ferveo-0.1.5/local_dependencies/ferveo-common/src/serialization.rs` & `ferveo-0.1.6/local_dependencies/ferveo-common/src/serialization.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 //! This adds a few utility functions for serializing and deserializing
 //! [arkworks](http://arkworks.rs/) types that implement [CanonicalSerialize] and [CanonicalDeserialize].
 //! Adapted from [o1-labs/proof-systems](https://raw.githubusercontent.com/o1-labs/proof-systems/31c76ceae3122f0ce09cded8260960ed5cbbe3d8/utils/src/serialization.rs).
 
 use ark_serialize::{CanonicalDeserialize, CanonicalSerialize};
-use serde;
-use serde::{Deserialize, Serialize};
+use serde::{self, Deserialize, Serialize};
 use serde_with::Bytes;
 
 //
 // Serialization with serde
 //
 
 pub mod ser {
```

### Comparing `ferveo-0.1.5/Cargo.toml` & `ferveo-0.1.6/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [package]
 name = "ferveo-python"
 authors = ["Piotr Roslaniec <p.roslaniec@gmail.com>"]
-version = "0.1.5"
+version = "0.1.6"
 edition = "2018"
 
 [lib]
 crate-type = ["cdylib"]
 name = "ferveo_py"
 
 [dependencies]
 ferveo = { path = "local_dependencies/ferveo" }
 ferveo-common = { path = "local_dependencies/ferveo-common" }
-pyo3 = { version = "0.17.3", features = ["macros", "extension-module"] }
-group-threshold-cryptography = { path = "local_dependencies/group-threshold-cryptography" }
+pyo3 = { version = "0.18.2", features = ["macros", "extension-module"] }
 derive_more = { version = "0.99", default-features = false, features = ["from", "as_ref"] }
 rand = "0.8"
 
 [build-dependencies]
 pyo3-build-config = "*"
```

### Comparing `ferveo-0.1.5/LICENSE` & `ferveo-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.5/examples/server_api.py` & `ferveo-0.1.6/examples/server_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+import os
+
 from ferveo_py import (
     encrypt,
     combine_decryption_shares,
     decrypt_with_shared_secret,
     Keypair,
-    PublicKey,
     ExternalValidator,
     Transcript,
     Dkg,
-    Ciphertext,
-    UnblindingKey,
-    DecryptionShare,
     AggregatedTranscript,
+    Ciphertext,
+    DkgPublicKey,
 )
 
 tau = 1
 security_threshold = 3
 shares_num = 4
 validator_keypairs = [Keypair.random() for _ in range(0, shares_num)]
 validators = [
@@ -31,58 +31,81 @@
         shares_num=shares_num,
         security_threshold=security_threshold,
         validators=validators,
         me=sender,
     )
     messages.append((sender, dkg.generate_transcript()))
 
-print(Dkg)
-
 # Now that every validator holds a dkg instance and a transcript for every other validator,
 # every validator can aggregate the transcripts
 me = validators[0]
 dkg = Dkg(
     tau=tau,
     shares_num=shares_num,
     security_threshold=security_threshold,
     validators=validators,
     me=me,
 )
 pvss_aggregated = dkg.aggregate_transcripts(messages)
 assert pvss_aggregated.validate(dkg)
 
-# Server can persist transcript and the aggregated transcript
+# Server can persist transcripts and the aggregated transcript
 transcripts_ser = [bytes(transcript) for _, transcript in messages]
-transcripts_deser = [Transcript.from_bytes(t) for t in transcripts_ser]
-
+_transcripts_deser = [Transcript.from_bytes(t) for t in transcripts_ser]
 agg_transcript_ser = bytes(pvss_aggregated)
-agg_transcript_deser = AggregatedTranscript.from_bytes(agg_transcript_ser)
 
 # In the meantime, the client creates a ciphertext and decryption request
 msg = "abc".encode()
 aad = "my-aad".encode()
 ciphertext = encrypt(msg, aad, dkg.final_key)
 
+# The client can serialize/deserialize ciphertext for transport
+ciphertext_ser = bytes(ciphertext)
+
 # Having aggregated the transcripts, the validators can now create decryption shares
 decryption_shares = []
 for validator, validator_keypair in zip(validators, validator_keypairs):
     dkg = Dkg(
         tau=tau,
         shares_num=shares_num,
         security_threshold=security_threshold,
         validators=validators,
         me=validator,
     )
-    aggregate = dkg.aggregate_transcripts(messages)
-    assert pvss_aggregated.validate(dkg)
-    decryption_share = aggregate.create_decryption_share(
+    # Assume the aggregated transcript is obtained through deserialization from a side-channel
+    agg_transcript_deser = AggregatedTranscript.from_bytes(agg_transcript_ser)
+    agg_transcript_deser.validate(dkg)
+
+    # The ciphertext is obtained from the client
+    ciphertext_deser = Ciphertext.from_bytes(ciphertext_ser)
+
+    # Create a decryption share for the ciphertext
+    decryption_share = agg_transcript_deser.create_decryption_share(
         dkg, ciphertext, aad, validator_keypair
     )
     decryption_shares.append(decryption_share)
 
 # Now, the decryption share can be used to decrypt the ciphertext
-# This part is part of the client API
+# This part is in the client API
 
 shared_secret = combine_decryption_shares(decryption_shares)
 
-plaintext = decrypt_with_shared_secret(ciphertext, aad, shared_secret, dkg.g1_inv)
+plaintext = decrypt_with_shared_secret(ciphertext, aad, shared_secret, dkg.public_params)
 assert bytes(plaintext) == msg
+
+# Other serializable objects
+
+# Keypair
+keypair = Keypair.random()
+keypair_ser = bytes(keypair)
+keypair_deser = Keypair.from_bytes(keypair_ser)
+
+# DKG public key
+dkg_pk = dkg.final_key
+dkg_pk_ser = bytes(dkg_pk)
+dkg_pk_deser = DkgPublicKey.from_bytes(dkg_pk_ser)
+
+# Other utilities
+
+bytes_len = Keypair.secure_randomness_size()
+secure_randomness = os.urandom(bytes_len)
+keypair = Keypair.from_secure_randomness(secure_randomness)
```

### Comparing `ferveo-0.1.5/setup.py` & `ferveo-0.1.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ferveo",
     description="Ferveo DKG scheme",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.1.5",
+    version="0.1.6",
     author="Piotr Roslaniec",
     author_email="p.roslaniec@gmail.com",
     url="https://github.com/nucypher/ferveo/tree/master/ferveo-python",
     rust_extensions=[RustExtension(
         "ferveo._ferveo", binding=Binding.PyO3, debug=False)],
     packages=["ferveo"],
     package_data={
```

### Comparing `ferveo-0.1.5/src/lib.rs` & `ferveo-0.1.6/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 extern crate alloc;
 
-use std::fmt;
+use std::fmt::{self};
 
 use ferveo::api::E;
 use ferveo_common::serialization::{FromBytes, ToBytes};
-use pyo3::exceptions::PyValueError;
-use pyo3::prelude::*;
-use pyo3::types::PyBytes;
+use pyo3::{exceptions::PyValueError, prelude::*, types::PyBytes};
 use rand::thread_rng;
 
 fn from_py_bytes<T: FromBytes>(bytes: &[u8]) -> PyResult<T> {
     T::from_bytes(bytes).map_err(map_py_error)
 }
 
 fn to_py_bytes<T: ToBytes>(t: T) -> PyResult<PyObject> {
@@ -27,15 +25,15 @@
 #[pyfunction]
 pub fn encrypt(
     message: &[u8],
     aad: &[u8],
     public_key: &DkgPublicKey,
 ) -> PyResult<Ciphertext> {
     let rng = &mut thread_rng();
-    let ciphertext = ferveo::api::encrypt(message, aad, &public_key.0, rng)
+    let ciphertext = ferveo::api::encrypt(message, aad, &public_key.0 .0, rng)
         .map_err(map_py_error)?;
     Ok(Ciphertext(ciphertext))
 }
 
 #[pyfunction]
 pub fn combine_decryption_shares(shares: Vec<DecryptionShare>) -> SharedSecret {
     let shares = shares
@@ -46,28 +44,40 @@
 }
 
 #[pyfunction]
 pub fn decrypt_with_shared_secret(
     ciphertext: &Ciphertext,
     aad: &[u8],
     shared_secret: &SharedSecret,
-    g1_inv: &G1Prepared,
+    dkg_params: &DkgPublicParameters,
 ) -> PyResult<Vec<u8>> {
     ferveo::api::decrypt_with_shared_secret(
         &ciphertext.0,
         aad,
         &shared_secret.0,
-        &g1_inv.0,
+        &dkg_params.0.g1_inv,
     )
-    .map_err(|err| PyValueError::new_err(format!("{}", err)))
+    .map_err(map_py_error)
 }
 
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::AsRef)]
-pub struct G1Prepared(ferveo::api::G1Prepared);
+pub struct DkgPublicParameters(ferveo::api::DkgPublicParameters);
+
+#[pymethods]
+impl DkgPublicParameters {
+    #[staticmethod]
+    pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
+        from_py_bytes(bytes).map(Self)
+    }
+
+    fn __bytes__(&self) -> PyResult<PyObject> {
+        to_py_bytes(self.0.clone())
+    }
+}
 
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::AsRef)]
 pub struct SharedSecret(ferveo::api::SharedSecret);
 
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::From, derive_more::AsRef)]
@@ -77,14 +87,26 @@
 impl Keypair {
     #[staticmethod]
     pub fn random() -> Self {
         Self(ferveo::api::Keypair::new(&mut thread_rng()))
     }
 
     #[staticmethod]
+    pub fn from_secure_randomness(bytes: &[u8]) -> PyResult<Self> {
+        let keypair = ferveo::api::Keypair::<E>::from_secure_randomness(bytes)
+            .map_err(map_py_error)?;
+        Ok(Self(keypair))
+    }
+
+    #[staticmethod]
+    pub fn secure_randomness_size() -> usize {
+        ferveo::api::Keypair::<E>::secure_randomness_size()
+    }
+
+    #[staticmethod]
     pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
         from_py_bytes(bytes).map(Self)
     }
 
     fn __bytes__(&self) -> PyResult<PyObject> {
         to_py_bytes(self.0)
     }
@@ -92,15 +114,15 @@
     #[getter]
     pub fn public_key(&self) -> PublicKey {
         PublicKey(self.0.public())
     }
 }
 
 #[pyclass(module = "ferveo")]
-#[derive(Clone, derive_more::From, derive_more::AsRef)]
+#[derive(Clone, PartialEq, Eq, derive_more::From, derive_more::AsRef)]
 pub struct PublicKey(ferveo::api::PublicKey<E>);
 
 #[pymethods]
 impl PublicKey {
     #[staticmethod]
     pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
         from_py_bytes(bytes).map(Self)
@@ -117,14 +139,24 @@
 
 #[pymethods]
 impl ExternalValidator {
     #[new]
     pub fn new(address: String, public_key: PublicKey) -> Self {
         Self(ferveo::api::ExternalValidator::new(address, public_key.0))
     }
+
+    #[getter]
+    pub fn address(&self) -> String {
+        self.0.address.to_string()
+    }
+
+    #[getter]
+    pub fn public_key(&self) -> PublicKey {
+        PublicKey(self.0.public_key)
+    }
 }
 
 #[pyclass(module = "ferveo")]
 #[derive(Clone, derive_more::From, derive_more::AsRef)]
 pub struct Transcript(ferveo::api::Transcript<E>);
 
 #[pymethods]
@@ -139,14 +171,26 @@
     }
 }
 
 #[pyclass(module = "ferveo")]
 #[derive(Clone, derive_more::From, derive_more::AsRef)]
 pub struct DkgPublicKey(ferveo::api::DkgPublicKey);
 
+#[pymethods]
+impl DkgPublicKey {
+    #[staticmethod]
+    pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
+        from_py_bytes(bytes).map(Self)
+    }
+
+    fn __bytes__(&self) -> PyResult<PyObject> {
+        to_py_bytes(self.0)
+    }
+}
+
 #[derive(FromPyObject)]
 pub struct ExternalValidatorMessage(ExternalValidator, Transcript);
 
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct Dkg(ferveo::api::Dkg);
 
@@ -164,62 +208,87 @@
         let dkg = ferveo::api::Dkg::new(
             tau,
             shares_num,
             security_threshold,
             &validators,
             &me.0,
         )
-        .map_err(|err| PyValueError::new_err(format!("{}", err)))?;
+        .map_err(map_py_error)?;
         Ok(Self(dkg))
     }
 
     #[getter]
     pub fn final_key(&self) -> DkgPublicKey {
         DkgPublicKey(self.0.final_key())
     }
 
     pub fn generate_transcript(&self) -> PyResult<Transcript> {
         let rng = &mut thread_rng();
-        let transcript = self
-            .0
-            .generate_transcript(rng)
-            .map_err(|err| PyValueError::new_err(format!("{}", err)))?;
+        let transcript =
+            self.0.generate_transcript(rng).map_err(map_py_error)?;
         Ok(Transcript(transcript))
     }
 
-    pub fn aggregate_transcripts(&mut self, transcripts: Vec<(ExternalValidator, Transcript)>) -> PyResult<AggregatedTranscript> {
+    pub fn aggregate_transcripts(
+        &mut self,
+        transcripts: Vec<(ExternalValidator, Transcript)>,
+    ) -> PyResult<AggregatedTranscript> {
         let transcripts: Vec<_> = transcripts
             .into_iter()
             .map(|(validator, transcript)| (validator.0, transcript.0))
             .collect();
         let aggregated_transcript = self
             .0
             .aggregate_transcripts(&transcripts)
-            .map_err(|err| PyValueError::new_err(format!("{}", err)))?;
+            .map_err(map_py_error)?;
         Ok(AggregatedTranscript(aggregated_transcript))
     }
 
     #[getter]
-    pub fn g1_inv(&self) -> G1Prepared {
-        G1Prepared(self.0.g1_inv())
+    pub fn public_params(&self) -> DkgPublicParameters {
+        DkgPublicParameters(self.0.public_params())
     }
 }
 
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct Ciphertext(ferveo::api::Ciphertext);
 
+#[pymethods]
+impl Ciphertext {
+    #[staticmethod]
+    pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
+        from_py_bytes(bytes).map(Self)
+    }
+
+    fn __bytes__(&self) -> PyResult<PyObject> {
+        to_py_bytes(&self.0)
+    }
+}
+
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct UnblindingKey(ferveo::api::UnblindingKey);
 
 #[pyclass(module = "ferveo")]
 #[derive(Clone, derive_more::AsRef, derive_more::From)]
 pub struct DecryptionShare(ferveo::api::DecryptionShare);
 
+#[pymethods]
+impl DecryptionShare {
+    #[staticmethod]
+    pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
+        from_py_bytes(bytes).map(Self)
+    }
+
+    fn __bytes__(&self) -> PyResult<PyObject> {
+        to_py_bytes(&self.0)
+    }
+}
+
 #[pyclass(module = "ferveo")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct AggregatedTranscript(ferveo::api::AggregatedTranscript);
 
 #[pymethods]
 impl AggregatedTranscript {
     pub fn validate(&self, dkg: &Dkg) -> bool {
@@ -237,15 +306,15 @@
             .0
             .create_decryption_share(
                 &dkg.0,
                 &ciphertext.0,
                 aad,
                 &validator_keypair.0,
             )
-            .map_err(|err| PyValueError::new_err(format!("{}", err)))?;
+            .map_err(map_py_error)?;
         Ok(DecryptionShare(decryption_share))
     }
 
     #[staticmethod]
     pub fn from_bytes(bytes: &[u8]) -> PyResult<Self> {
         from_py_bytes(bytes).map(Self)
     }
@@ -266,9 +335,10 @@
     m.add_class::<ExternalValidator>()?;
     m.add_class::<Transcript>()?;
     m.add_class::<Dkg>()?;
     m.add_class::<Ciphertext>()?;
     m.add_class::<UnblindingKey>()?;
     m.add_class::<DecryptionShare>()?;
     m.add_class::<AggregatedTranscript>()?;
+    m.add_class::<DkgPublicKey>()?;
     Ok(())
 }
```

### Comparing `ferveo-0.1.5/Cargo.lock` & `ferveo-0.1.6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 checksum = "51ee31d8869a353433524dbd5a8f51f95cdafe7c66d458956ec13aa737198562"
 dependencies = [
  "ark-ff-asm",
  "ark-ff-macros",
  "ark-serialize",
  "ark-std",
  "derivative",
- "digest 0.10.6",
+ "digest",
  "itertools",
  "num-bigint",
  "num-traits",
  "paste",
  "rustc_version",
  "zeroize",
 ]
@@ -159,15 +159,15 @@
 name = "ark-serialize"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "58ea39d00a8a4c832e6f6520e58ccec7bf909c4845863512e9b8656fd47df355"
 dependencies = [
  "ark-serialize-derive",
  "ark-std",
- "digest 0.10.6",
+ "digest",
  "num-bigint",
 ]
 
 [[package]]
 name = "ark-serialize-derive"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -245,23 +245,14 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "block-buffer"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4152116fd6e9dadb291ae18fc1ec3575ed6d84c29642d97890f4b4a3417297e4"
-dependencies = [
- "generic-array",
-]
-
-[[package]]
-name = "block-buffer"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
 dependencies = [
  "generic-array",
 ]
 
@@ -286,20 +277,14 @@
 [[package]]
 name = "bytemuck"
 version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c041d3eab048880cb0b86b256447da3f18859a163c3b8d8893f4e6368abe6393"
 
 [[package]]
-name = "byteorder"
-version = "1.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
-
-[[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
@@ -615,27 +600,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "curve25519-dalek"
-version = "3.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b9fdf9972b2bd6af2d913799d9ebc165ea4d2e65878e329d9c6b372c4491b61"
-dependencies = [
- "byteorder",
- "digest 0.9.0",
- "rand_core 0.5.1",
- "subtle",
- "zeroize",
-]
-
-[[package]]
 name = "cxx"
 version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90d59d9acd2a682b4e40605a242f6670eaa58c5957471cbf85e8aa6a0b97a5e8"
 dependencies = [
  "cc",
  "cxxbridge-flags",
@@ -739,58 +711,23 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "digest"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3dd60d1080a57a05ab032377049e0591415d2b31afd7028356dbf3cc6dcb066"
-dependencies = [
- "generic-array",
-]
-
-[[package]]
-name = "digest"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
 dependencies = [
- "block-buffer 0.10.3",
+ "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
-name = "ed25519"
-version = "1.5.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91cff35c70bba8a626e3185d8cd48cc11b5437e1a5bcd15b9b5fa3c64b6dfee7"
-dependencies = [
- "serde",
- "signature",
-]
-
-[[package]]
-name = "ed25519-dalek"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c762bae6dcaf24c4c84667b8579785430908723d5c889f469d76a41d59cc7a9d"
-dependencies = [
- "curve25519-dalek",
- "ed25519",
- "merlin",
- "rand 0.7.3",
- "serde",
- "serde_bytes",
- "sha2 0.9.9",
- "zeroize",
-]
-
-[[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "fastrand"
@@ -801,63 +738,58 @@
  "instant",
 ]
 
 [[package]]
 name = "ferveo"
 version = "0.1.1"
 dependencies = [
- "anyhow",
  "ark-bls12-381",
  "ark-ec",
  "ark-ff",
  "ark-poly",
- "ark-serialize",
  "ark-std",
  "bincode",
  "criterion 0.3.6",
- "digest 0.10.6",
- "ed25519-dalek",
- "either",
+ "digest",
  "ferveo-common",
  "group-threshold-cryptography",
  "itertools",
  "measure_time",
- "miracl_core",
  "pprof",
  "rand 0.7.3",
  "rand 0.8.5",
  "rand_core 0.6.4",
  "serde",
- "serde_bytes",
  "serde_with",
  "subproductdomain",
- "subtle",
- "zeroize",
+ "thiserror",
 ]
 
 [[package]]
 name = "ferveo-common"
 version = "0.1.0"
 dependencies = [
+ "ark-bls12-381",
  "ark-ec",
  "ark-serialize",
  "ark-std",
  "bincode",
+ "rand 0.8.5",
+ "rand_core 0.6.4",
  "serde",
  "serde_with",
 ]
 
 [[package]]
 name = "ferveo-python"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "derive_more",
  "ferveo",
  "ferveo-common",
- "group-threshold-cryptography",
  "pyo3",
  "pyo3-build-config 0.17.3",
  "rand 0.8.5",
 ]
 
 [[package]]
 name = "findshlibs"
@@ -917,15 +849,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "221996f774192f0f718773def8201c4ae31f02616a54ccfc2d358bb0e5cefdec"
 
 [[package]]
 name = "group-threshold-cryptography"
 version = "0.1.0"
 dependencies = [
- "anyhow",
  "ark-bls12-381",
  "ark-ec",
  "ark-ff",
  "ark-poly",
  "ark-serialize",
  "ark-std",
  "bincode",
@@ -936,15 +867,15 @@
  "itertools",
  "miracl_core",
  "rand 0.8.5",
  "rand_core 0.6.4",
  "serde",
  "serde_bytes",
  "serde_with",
- "sha2 0.10.6",
+ "sha2",
  "subproductdomain",
  "thiserror",
 ]
 
 [[package]]
 name = "half"
 version = "1.8.2"
@@ -1103,23 +1034,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "keccak"
-version = "0.1.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3afef3b6eff9ce9d8ff9b3601125eec7f0c8cbac7abd14f355d053fa56c98768"
-dependencies = [
- "cpufeatures",
-]
-
-[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
@@ -1195,30 +1117,27 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "memory_units"
-version = "0.4.0"
+name = "memoffset"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8452105ba047068f40ff7093dd1d9da90898e63dd61736462e9cdda6a90ad3c3"
+checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+dependencies = [
+ "autocfg",
+]
 
 [[package]]
-name = "merlin"
-version = "2.0.1"
+name = "memory_units"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e261cf0f8b3c42ded9f7d2bb59dea03aa52bc8a1cbc7482f9fc3fd1229d3b42"
-dependencies = [
- "byteorder",
- "keccak",
- "rand_core 0.5.1",
- "zeroize",
-]
+checksum = "8452105ba047068f40ff7093dd1d9da90898e63dd61736462e9cdda6a90ad3c3"
 
 [[package]]
 name = "miniz_oxide"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
@@ -1455,24 +1374,24 @@
 checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if 1.0.0",
  "indoc",
  "libc",
- "memoffset 0.6.5",
+ "memoffset 0.8.0",
  "parking_lot 0.12.1",
- "pyo3-build-config 0.17.3",
+ "pyo3-build-config 0.18.2",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
@@ -1482,49 +1401,49 @@
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
- "pyo3-build-config 0.17.3",
+ "pyo3-build-config 0.18.2",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1816,43 +1735,24 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.9.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d58a1e1bf39749807d89cf2d98ac2dfa0ff1cb3faa38fbb64dd88ac8013d800"
-dependencies = [
- "block-buffer 0.9.0",
- "cfg-if 1.0.0",
- "cpufeatures",
- "digest 0.9.0",
- "opaque-debug",
-]
-
-[[package]]
-name = "sha2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
  "cfg-if 1.0.0",
  "cpufeatures",
- "digest 0.10.6",
+ "digest",
 ]
 
 [[package]]
-name = "signature"
-version = "1.6.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74233d3b3b2f6d4b006dc19dee745e73e2a6bfb6f93607cd3b02bd5b00797d7c"
-
-[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "stable_deref_trait"
@@ -1877,15 +1777,14 @@
 version = "0.1.0"
 dependencies = [
  "anyhow",
  "ark-bls12-381",
  "ark-ec",
  "ark-ff",
  "ark-poly",
- "ark-serialize",
  "ark-std",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2041,27 +1940,22 @@
 [[package]]
 name = "tpke-python"
 version = "0.1.0"
 dependencies = [
  "ferveo-common",
  "group-threshold-cryptography",
  "pyo3",
- "pyo3-build-config 0.18.1",
+ "pyo3-build-config 0.17.3",
 ]
 
 [[package]]
 name = "tpke-wasm"
 version = "0.1.0-alpha.1"
 dependencies = [
- "ark-bls12-381",
- "ark-ec",
- "ark-ff",
  "ark-serialize",
- "ark-std",
- "bincode",
  "console_error_panic_hook",
  "ferveo-common",
  "getrandom 0.2.8",
  "group-threshold-cryptography",
  "js-sys",
  "rand 0.8.5",
  "rand_core 0.6.4",
```

### Comparing `ferveo-0.1.5/PKG-INFO` & `ferveo-0.1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferveo
-Version: 0.1.5
+Version: 0.1.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Author: Piotr Roslaniec <p.roslaniec@gmail.com>
 Author-email: Piotr Roslaniec <p.roslaniec@gmail.com>
 Requires-Python: >=3.7
```

