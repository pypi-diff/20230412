# Comparing `tmp/tsdownsample-0.1.1.tar.gz` & `tmp/tsdownsample-0.1.2a0.tar.gz`

## Comparing `tsdownsample-0.1.1.tar` & `tsdownsample-0.1.2a0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/Cargo.toml
--rw-r--r--   0     1001      123     1078 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/LICENSE
--rw-r--r--   0     1001      123       82 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/README.md
--rw-r--r--   0     1001      123     1765 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/benches/bench_lttb.rs
--rw-r--r--   0     1001      123     4073 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/benches/bench_m4.rs
--rw-r--r--   0     1001      123     5825 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/benches/bench_minmax.rs
--rw-r--r--   0     1001      123     5546 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/benches/bench_minmaxlttb.rs
--rw-r--r--   0     1001      123     6060 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/benches/results
--rw-r--r--   0     1001      123     1886 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/helpers.rs
--rw-r--r--   0     1001      123      211 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/lib.rs
--rw-r--r--   0     1001      123       31 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/lttb/mod.rs
--rw-r--r--   0     1001      123     8462 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/lttb/scalar.rs
--rw-r--r--   0     1001      123     7283 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/m4/generic.rs
--rw-r--r--   0     1001      123       97 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/m4/mod.rs
--rw-r--r--   0     1001      123     8644 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/m4/scalar.rs
--rw-r--r--   0     1001      123     8613 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/m4/simd.rs
--rw-r--r--   0     1001      123     6282 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmax/generic.rs
--rw-r--r--   0     1001      123       97 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmax/mod.rs
--rw-r--r--   0     1001      123     8763 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmax/scalar.rs
--rw-r--r--   0     1001      123     8855 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmax/simd.rs
--rw-r--r--   0     1001      123     2775 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmaxlttb/generic.rs
--rw-r--r--   0     1001      123       97 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmaxlttb/mod.rs
--rw-r--r--   0     1001      123     4220 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmaxlttb/scalar.rs
--rw-r--r--   0     1001      123     4214 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmaxlttb/simd.rs
--rw-r--r--   0     1001      123    10544 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/searchsorted.rs
--rw-r--r--   0     1001      123      375 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/downsample_rs/src/types.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 tsdownsample-0.1.1/local_dependencies/dev_utils/Cargo.toml
--rw-r--r--   0     1001      123      187 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/dev_utils/src/config.rs
--rw-r--r--   0     1001      123       68 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/dev_utils/src/lib.rs
--rw-r--r--   0     1001      123     1087 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/local_dependencies/dev_utils/src/utils.rs
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 tsdownsample-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123     4159 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/.github/workflows/ci-downsample_rs.yml
--rw-r--r--   0     1001      123     5546 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/.github/workflows/ci-tsdownsample.yml
--rw-r--r--   0     1001      123     2302 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/.gitignore
--rw-r--r--   0     1001      123     2859 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/CONTRIBUTING.md
--rw-r--r--   0     1001      123     1078 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/LICENSE
--rw-r--r--   0     1001      123     1292 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/Makefile
--rw-r--r--   0     1001      123     5812 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/README.md
--rw-r--r--   0     1001      123     1833 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123    13461 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123       29 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/tests/requirements-linting.txt
--rw-r--r--   0     1001      123       17 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/tests/requirements.txt
--rw-r--r--   0     1001      123      599 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/tests/test_config.py
--rw-r--r--   0     1001      123     1489 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/tests/test_rust_mods.py
--rw-r--r--   0     1001      123     9872 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/tests/test_tsdownsample.py
--rw-r--r--   0     1001      123      435 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/tsdownsample/__init__.py
--rw-r--r--   0     1001      123       58 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/tsdownsample/_rust/__init__.py
--rw-r--r--   0     1001      123     2098 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/tsdownsample/downsamplers.py
--rw-r--r--   0     1001      123    11729 2023-01-30 08:50:13.000000 tsdownsample-0.1.1/tsdownsample/downsampling_interface.py
--rw-r--r--   0     1001      123    13034 2023-01-30 08:50:58.000000 tsdownsample-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     6846 1970-01-01 00:00:00.000000 tsdownsample-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/Cargo.toml
+-rw-r--r--   0     1001      123     1078 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/LICENSE
+-rw-r--r--   0     1001      123       82 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/README.md
+-rw-r--r--   0     1001      123     1736 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_lttb.rs
+-rw-r--r--   0     1001      123     4043 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_m4.rs
+-rw-r--r--   0     1001      123     5795 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_minmax.rs
+-rw-r--r--   0     1001      123     5517 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_minmaxlttb.rs
+-rw-r--r--   0     1001      123     6060 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/results
+-rw-r--r--   0     1001      123     1886 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/helpers.rs
+-rw-r--r--   0     1001      123      211 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/lib.rs
+-rw-r--r--   0     1001      123       31 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/lttb/mod.rs
+-rw-r--r--   0     1001      123     8462 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/lttb/scalar.rs
+-rw-r--r--   0     1001      123     7630 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/generic.rs
+-rw-r--r--   0     1001      123       97 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/mod.rs
+-rw-r--r--   0     1001      123     8766 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/scalar.rs
+-rw-r--r--   0     1001      123     8728 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/simd.rs
+-rw-r--r--   0     1001      123     6691 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/generic.rs
+-rw-r--r--   0     1001      123       97 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/mod.rs
+-rw-r--r--   0     1001      123     8824 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/scalar.rs
+-rw-r--r--   0     1001      123     8852 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/simd.rs
+-rw-r--r--   0     1001      123     2775 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/generic.rs
+-rw-r--r--   0     1001      123       97 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/mod.rs
+-rw-r--r--   0     1001      123     4220 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/scalar.rs
+-rw-r--r--   0     1001      123     4214 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/simd.rs
+-rw-r--r--   0     1001      123    11715 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/searchsorted.rs
+-rw-r--r--   0     1001      123      375 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/types.rs
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 tsdownsample-0.1.2a0/Cargo.toml
+-rw-r--r--   0     1001      123     4159 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/.github/workflows/ci-downsample_rs.yml
+-rw-r--r--   0     1001      123     5514 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/.github/workflows/ci-tsdownsample.yml
+-rw-r--r--   0     1001      123     1195 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/.github/workflows/codspeed.yml
+-rw-r--r--   0     1001      123     2302 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/.gitignore
+-rw-r--r--   0     1001      123     3004 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     1078 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/LICENSE
+-rw-r--r--   0     1001      123     1336 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/Makefile
+-rw-r--r--   0     1001      123     5931 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/README.md
+-rw-r--r--   0     1001      123     1616 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/pyproject.toml
+-rw-r--r--   0     1001      123    13461 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/benchmarks/__init__.py
+-rw-r--r--   0     1001      123     6594 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/benchmarks/test_downsamplers.py
+-rw-r--r--   0     1001      123       16 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/requirements-linting.txt
+-rw-r--r--   0     1001      123       35 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/requirements.txt
+-rw-r--r--   0     1001      123     1026 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/test_algos_python_compliance.py
+-rw-r--r--   0     1001      123      599 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/test_config.py
+-rw-r--r--   0     1001      123     1489 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/test_rust_mods.py
+-rw-r--r--   0     1001      123    10222 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tests/test_tsdownsample.py
+-rw-r--r--   0     1001      123      437 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/_python/__init__.py
+-rw-r--r--   0     1001      123     6358 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/_python/downsamplers.py
+-rw-r--r--   0     1001      123       58 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/_rust/__init__.py
+-rw-r--r--   0     1001      123     2107 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/downsamplers.py
+-rw-r--r--   0     1001      123    12370 2023-04-12 17:21:29.000000 tsdownsample-0.1.2a0/tsdownsample/downsampling_interface.py
+-rw-r--r--   0     1001      123    13037 2023-04-12 17:22:03.000000 tsdownsample-0.1.2a0/Cargo.lock
+-rw-r--r--   0        0        0     6952 1970-01-01 00:00:00.000000 tsdownsample-0.1.2a0/PKG-INFO
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/Cargo.toml` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,24 +5,20 @@
 authors = ["Jeroen Van Der Donckt"]
 description = "Downsample time series data"
 license = "MIT"
 
 [dependencies]
 # TODO: perhaps use polars?
 ndarray = {version = "0.15.6", default-features = false, features = ["rayon"] }
-argminmax = { version = "0.3.1" , features = ["half"] }
+argminmax = { version = "0.3.1", features = ["half"] }
 # argminmax = { path = "../../argminmax" , features = ["half", "ndarray"] }
 half = { version = "2.1", default-features = false , features=["num-traits"], optional = true}
 num-traits = { version = "0.2.15", default-features = false }
 rayon = { version = "1.6.0", default-features = false }
 
-[dev-dependencies]
-criterion = "0.4.0"
-dev_utils = { path = "../dev_utils" }
-
 [[bench]]
 name = "bench_m4"
 harness = false
 
 [[bench]]
 name = "bench_minmax"
 harness = false
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/LICENSE` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/LICENSE`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/benches/bench_lttb.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_lttb.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-#[macro_use]
-extern crate criterion;
-extern crate dev_utils;
-
 use downsample_rs::lttb as lttb_mod;
 
-use criterion::{black_box, Criterion};
+use criterion::{black_box, criterion_group, criterion_main, Criterion};
 use dev_utils::{config, utils};
 use ndarray::Array1;
 
 fn lttb_f32_random_array_long(c: &mut Criterion) {
     let n = config::ARRAY_LENGTH_LONG;
     let x = Array1::from((0..n).map(|i| i as i32).collect::<Vec<i32>>());
     let y = utils::get_random_array::<f32>(n, f32::MIN, f32::MAX);
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/benches/bench_m4.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_m4.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-#[macro_use]
-extern crate criterion;
-extern crate dev_utils;
-
 use downsample_rs::m4 as m4_mod;
 
-use criterion::{black_box, Criterion};
+use criterion::{black_box, criterion_group, criterion_main, Criterion};
 use dev_utils::{config, utils};
-
 use ndarray::Array1;
 
 fn m4_f32_random_array_long_single_core(c: &mut Criterion) {
     let n = config::ARRAY_LENGTH_LONG;
     let data = utils::get_random_array::<f32>(n, f32::MIN, f32::MAX);
     c.bench_function("m4_scal_f32", |b| {
         b.iter(|| m4_mod::m4_scalar_without_x(black_box(data.view()), black_box(2_000)))
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/benches/bench_minmax.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_minmax.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-#[macro_use]
-extern crate criterion;
-extern crate dev_utils;
-
 use downsample_rs::minmax as minmax_mod;
 
-use criterion::{black_box, Criterion};
+use criterion::{black_box, criterion_group, criterion_main, Criterion};
 use dev_utils::{config, utils};
-
 use ndarray::Array1;
 
 fn minmax_f32_random_array_long_single_core(c: &mut Criterion) {
     let n = config::ARRAY_LENGTH_LONG;
     let data = utils::get_random_array::<f32>(n, f32::MIN, f32::MAX);
     c.bench_function("minmax_scal_f32", |b| {
         b.iter(|| minmax_mod::min_max_scalar_without_x(black_box(data.view()), black_box(2_000)))
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/benches/bench_minmaxlttb.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/bench_minmaxlttb.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-#[macro_use]
-extern crate criterion;
-extern crate dev_utils;
-
 use downsample_rs::minmaxlttb as minmaxlttb_mod;
 
-use criterion::{black_box, Criterion};
+use criterion::{black_box, criterion_group, criterion_main, Criterion};
 use dev_utils::{config, utils};
 use ndarray::Array1;
 
 const MINMAX_RATIO: usize = 30;
 
 fn minmaxlttb_f32_random_array_long_single_core(c: &mut Criterion) {
     let n = config::ARRAY_LENGTH_LONG;
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/benches/results` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/benches/results`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/helpers.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/lttb/scalar.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/lttb/scalar.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/m4/generic.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/generic.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,192 +1,177 @@
 use ndarray::Zip;
-use ndarray::{s, Array1, ArrayView1};
+use ndarray::{Array1, ArrayView1};
 
 use rayon::iter::IndexedParallelIterator;
 use rayon::prelude::*;
 
-// TODO: check for duplicate data in the output array
-// -> In the current implementation we always add 4 datapoints per bin (if of
-//    course the bin has >= 4 datapoints). However, the argmin and argmax might
-//    be the start and end of the bin, which would result in duplicate data in
-//    the output array. (this is for example the case for monotonic data).
-
 // --------------------- WITHOUT X
 
 #[inline(always)]
-pub(crate) fn m4_generic<T: Copy + PartialOrd>(
+pub(crate) fn min_max_generic<T: Copy>(
     arr: ArrayView1<T>,
     n_out: usize,
     f_argminmax: fn(ArrayView1<T>) -> (usize, usize),
 ) -> Array1<usize> {
-    // Assumes n_out is a multiple of 4
+    // Assumes n_out is a multiple of 2
     if n_out >= arr.len() {
         return Array1::from((0..arr.len()).collect::<Vec<usize>>());
     }
 
-    let block_size = arr.len() as f64 / (n_out as f64) * 4.0;
-    let block_size = block_size.floor() as usize;
+    // arr.len() - 1 is used to match the delta of a range-index (0..arr.len()-1)
+    let block_size: f64 = (arr.len() - 1) as f64 / (n_out / 2) as f64;
+    let arr_ptr = arr.as_ptr();
 
     let mut sampled_indices: Array1<usize> = Array1::<usize>::default(n_out);
 
-    arr.slice(s![..block_size * n_out / 4])
-        .exact_chunks(block_size)
-        .into_iter()
-        .enumerate()
-        .for_each(|(i, step)| {
-            let (min_index, max_index) = f_argminmax(step);
-
-            let start_idx = block_size * i;
-            sampled_indices[4 * i] = start_idx;
-
-            // Add the indexes in sorted order
-            if min_index < max_index {
-                sampled_indices[4 * i + 1] = min_index + start_idx;
-                sampled_indices[4 * i + 2] = max_index + start_idx;
-            } else {
-                sampled_indices[4 * i + 1] = max_index + start_idx;
-                sampled_indices[4 * i + 2] = min_index + start_idx;
-            }
-            sampled_indices[4 * i + 3] = start_idx + block_size - 1;
+    let mut start_idx: usize = 0;
+    for i in 0..n_out / 2 {
+        // Decided to use multiplication instead of adding to the accumulator (end)
+        // as multiplication seems to be less prone to rounding errors.
+        let end: f64 = block_size * (i + 1) as f64;
+        let end_idx: usize = end as usize + 1;
+
+        let (min_index, max_index) = f_argminmax(unsafe {
+            ArrayView1::from_shape_ptr((end_idx - start_idx,), arr_ptr.add(start_idx))
         });
 
+        // Add the indexes in sorted order
+        if min_index < max_index {
+            sampled_indices[2 * i] = min_index + start_idx;
+            sampled_indices[2 * i + 1] = max_index + start_idx;
+        } else {
+            sampled_indices[2 * i] = max_index + start_idx;
+            sampled_indices[2 * i + 1] = min_index + start_idx;
+        }
+
+        start_idx = end_idx;
+    }
+
     sampled_indices
 }
 
 #[inline(always)]
-pub(crate) fn m4_generic_parallel<T: Copy + PartialOrd + Send + Sync>(
+pub(crate) fn min_max_generic_parallel<T: Copy + PartialOrd + Send + Sync>(
     arr: ArrayView1<T>,
     n_out: usize,
     f_argminmax: fn(ArrayView1<T>) -> (usize, usize),
 ) -> Array1<usize> {
-    // Assumes n_out is a multiple of 4
+    // Assumes n_out is a multiple of 2
     if n_out >= arr.len() {
         return Array1::from((0..arr.len()).collect::<Vec<usize>>());
     }
 
-    let block_size = arr.len() as f64 / (n_out as f64) * 4.0;
-    let block_size = block_size.floor() as usize;
+    // arr.len() - 1 is used to match the delta of a range-index (0..arr.len()-1)
+    let block_size: f64 = (arr.len() - 1) as f64 / (n_out / 2) as f64;
 
     // Store the enumerated indexes in the output array
     let mut sampled_indices: Array1<usize> = Array1::from_vec((0..n_out).collect::<Vec<usize>>());
 
-    // Iterate over the sample_index pointers and the array chunks
-    Zip::from(
-        arr.slice(s![..block_size * n_out / 4])
-            .exact_chunks(block_size),
-    )
-    .and(sampled_indices.exact_chunks_mut(4))
-    .par_for_each(|step, mut sampled_index| {
-        let (min_index, max_index) = f_argminmax(step);
+    Zip::from(sampled_indices.exact_chunks_mut(2)).par_for_each(|mut sampled_index| {
+        let i: f64 = unsafe { *sampled_index.uget(0) >> 1 } as f64;
+        let start_idx: usize = (block_size * i) as usize + (i != 0.0) as usize;
+        let end_idx: usize = (block_size * (i + 1.0)) as usize + 1;
 
-        let start_idx = block_size * unsafe { *sampled_index.uget(0) >> 2 };
-        sampled_index[0] = start_idx;
+        let (min_index, max_index) = f_argminmax(unsafe {
+            ArrayView1::from_shape_ptr((end_idx - start_idx,), arr.as_ptr().add(start_idx))
+        });
 
         // Add the indexes in sorted order
         if min_index < max_index {
-            sampled_index[1] = min_index + start_idx;
-            sampled_index[2] = max_index + start_idx;
-        } else {
+            sampled_index[0] = min_index + start_idx;
             sampled_index[1] = max_index + start_idx;
-            sampled_index[2] = min_index + start_idx;
+        } else {
+            sampled_index[0] = max_index + start_idx;
+            sampled_index[1] = min_index + start_idx;
         }
-        sampled_index[3] = start_idx + block_size - 1;
     });
 
     sampled_indices
 }
 
 // --------------------- WITH X
 
 #[inline(always)]
-pub(crate) fn m4_generic_with_x<T: Copy>(
+pub(crate) fn min_max_generic_with_x<T: Copy>(
     arr: ArrayView1<T>,
     bin_idx_iterator: impl Iterator<Item = Option<(usize, usize)>>,
     n_out: usize,
     f_argminmax: fn(ArrayView1<T>) -> (usize, usize),
 ) -> Array1<usize> {
-    // Assumes n_out is a multiple of 4
+    // Assumes n_out is a multiple of 2
     if n_out >= arr.len() {
         return Array1::from((0..arr.len()).collect::<Vec<usize>>());
     }
 
-    let arr_ptr = arr.as_ptr();
+    let ptr = arr.as_ptr();
     let mut sampled_indices: Vec<usize> = Vec::with_capacity(n_out);
 
     bin_idx_iterator.for_each(|bin| {
         if let Some((start, end)) = bin {
-            if end <= start + 4 {
-                // If the bin has <= 4 elements, just add them all
+            if end <= start + 2 {
+                // If the bin has <= 2 elements, just add them all
                 for i in start..end {
                     sampled_indices.push(i);
                 }
             } else {
-                // If the bin has > 4 elements, add the first and last + argmin and argmax
-                let step = unsafe { ArrayView1::from_shape_ptr(end - start, arr_ptr.add(start)) };
+                // If the bin has at least two elements, add the argmin and argmax
+                let step = unsafe { ArrayView1::from_shape_ptr(end - start, ptr.add(start)) };
                 let (min_index, max_index) = f_argminmax(step);
 
-                sampled_indices.push(start);
-
                 // Add the indexes in sorted order
                 if min_index < max_index {
                     sampled_indices.push(min_index + start);
                     sampled_indices.push(max_index + start);
                 } else {
                     sampled_indices.push(max_index + start);
                     sampled_indices.push(min_index + start);
                 }
-
-                sampled_indices.push(end - 1);
             }
         }
     });
 
     Array1::from_vec(sampled_indices)
 }
 
 #[inline(always)]
-pub(crate) fn m4_generic_with_x_parallel<T: Copy + PartialOrd + Send + Sync>(
+pub(crate) fn min_max_generic_with_x_parallel<T: Copy + Send + Sync>(
     arr: ArrayView1<T>,
     bin_idx_iterator: impl IndexedParallelIterator<Item = impl Iterator<Item = Option<(usize, usize)>>>,
     n_out: usize,
     f_argminmax: fn(ArrayView1<T>) -> (usize, usize),
 ) -> Array1<usize> {
-    // Assumes n_out is a multiple of 4
+    // Assumes n_out is a multiple of 2
     if n_out >= arr.len() {
         return Array1::from((0..arr.len()).collect::<Vec<usize>>());
     }
 
     Array1::from_vec(
         bin_idx_iterator
             .flat_map(|bin_idx_iterator| {
                 bin_idx_iterator
                     .map(|bin| {
                         match bin {
                             Some((start, end)) => {
-                                if end <= start + 4 {
-                                    // If the bin has <= 4 elements, just return them all
+                                if end <= start + 2 {
+                                    // If the bin has <= 2 elements, just return them all
                                     return (start..end).collect::<Vec<usize>>();
                                 }
 
-                                // If the bin has > 4 elements, return the first and last + argmin and argmax
+                                // If the bin has at least two elements, return the argmin and argmax
                                 let step = unsafe {
                                     ArrayView1::from_shape_ptr(end - start, arr.as_ptr().add(start))
                                 };
                                 let (min_index, max_index) = f_argminmax(step);
 
                                 // Return the indexes in sorted order
-                                let mut sampled_index = vec![start, 0, 0, end - 1];
                                 if min_index < max_index {
-                                    sampled_index[1] = min_index + start;
-                                    sampled_index[2] = max_index + start;
+                                    vec![min_index + start, max_index + start]
                                 } else {
-                                    sampled_index[1] = max_index + start;
-                                    sampled_index[2] = min_index + start;
+                                    vec![max_index + start, min_index + start]
                                 }
-                                sampled_index
                             } // If the bin is empty, return empty Vec
                             None => {
                                 vec![]
                             }
                         }
                     })
                     .collect::<Vec<Vec<usize>>>()
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/m4/scalar.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/scalar.rs`

 * *Files 8% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     fn test_m4_scalar_without_x_correct() {
         let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_scalar_without_x(arr.view(), 12);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
-        let expected_indices = vec![0, 0, 32, 32, 33, 33, 65, 65, 66, 66, 98, 98];
+        let expected_indices = vec![0, 0, 33, 33, 34, 34, 66, 66, 67, 67, 99, 99];
         let expected_values = expected_indices
             .iter()
             .map(|x| *x as f32)
             .collect::<Vec<f32>>();
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
@@ -112,15 +112,15 @@
     fn test_m4_scalar_without_x_parallel_correct() {
         let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_scalar_without_x_parallel(arr.view(), 12);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
-        let expected_indices = vec![0, 0, 32, 32, 33, 33, 65, 65, 66, 66, 98, 98];
+        let expected_indices = vec![0, 0, 33, 33, 34, 34, 66, 66, 67, 67, 99, 99];
         let expected_values = expected_indices
             .iter()
             .map(|x| *x as f32)
             .collect::<Vec<f32>>();
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
@@ -132,15 +132,15 @@
         let x = Array1::from(x);
         let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_scalar_with_x(x.view(), arr.view(), 12);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
-        let expected_indices = vec![0, 0, 32, 32, 33, 33, 65, 65, 66, 66, 98, 98];
+        let expected_indices = vec![0, 0, 33, 33, 34, 34, 66, 66, 67, 67, 99, 99];
         let expected_values = expected_indices
             .iter()
             .map(|x| *x as f32)
             .collect::<Vec<f32>>();
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
@@ -152,36 +152,36 @@
         let x = Array1::from(x);
         let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_scalar_with_x_parallel(x.view(), arr.view(), 12);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
-        let expected_indices = vec![0, 0, 32, 32, 33, 33, 65, 65, 66, 66, 98, 98];
+        let expected_indices = vec![0, 0, 33, 33, 34, 34, 66, 66, 67, 67, 99, 99];
         let expected_values = expected_indices
             .iter()
             .map(|x| *x as f32)
             .collect::<Vec<f32>>();
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
     }
 
     #[test]
     fn test_m4_scalar_with_x_gap() {
         // We will create a gap in the middle of the array
-        let x = (0..101).collect::<Vec<i32>>();
+        let x = (0..100).collect::<Vec<i32>>();
 
         // Increment the second half of the array by 50
         let x = x
             .iter()
             .map(|x| if *x > 50 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_scalar_with_x(x.view(), arr.view(), 20);
         assert_eq!(sampled_indices.len(), 16); // One full gap
         let expected_indices = vec![0, 0, 29, 29, 30, 30, 50, 50, 51, 51, 69, 69, 70, 70, 99, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
 
@@ -191,30 +191,31 @@
             .map(|x| if *x > 101 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
 
         let sampled_indices = m4_scalar_with_x(x.view(), arr.view(), 20);
         assert_eq!(sampled_indices.len(), 17); // Gap with 1 value
         let expected_indices = vec![
-            0, 0, 29, 29, 30, 30, 50, 50, 51, 51, 69, 69, 70, 70, 99, 99, 100,
+            0, 0, 39, 39, 40, 40, 50, 50, 51, 52, 52, 59, 59, 60, 60, 99, 99,
         ];
+        assert_eq!(sampled_indices, Array1::from(expected_indices));
     }
 
     #[test]
     fn test_m4_scalar_with_x_gap_parallel() {
         // We will create a gap in the middle of the array
-        let x = (0..101).collect::<Vec<i32>>();
+        let x = (0..100).collect::<Vec<i32>>();
 
         // Increment the second half of the array by 50
         let x = x
             .iter()
             .map(|x| if *x > 50 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_scalar_with_x_parallel(x.view(), arr.view(), 20);
         assert_eq!(sampled_indices.len(), 16); // One full gap
         let expected_indices = vec![0, 0, 29, 29, 30, 30, 50, 50, 51, 51, 69, 69, 70, 70, 99, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
 
@@ -224,28 +225,30 @@
             .map(|x| if *x > 101 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
 
         let sampled_indices = m4_scalar_with_x_parallel(x.view(), arr.view(), 20);
         assert_eq!(sampled_indices.len(), 17); // Gap with 1 value
         let expected_indices = vec![
-            0, 0, 29, 29, 30, 30, 50, 50, 51, 51, 69, 69, 70, 70, 99, 99, 100,
+            0, 0, 39, 39, 40, 40, 50, 50, 51, 52, 52, 59, 59, 60, 60, 99, 99,
         ];
+        assert_eq!(sampled_indices, Array1::from(expected_indices));
     }
 
     #[test]
     fn test_many_random_runs_correct() {
-        let n: usize = 20_001; // not 20_000 because then the last bin is not "full"
+        let n: usize = 20_003;
+        let n_out: usize = 204;
         let x = (0..n as i32).collect::<Vec<i32>>();
         let x = Array1::from(x);
         for _ in 0..100 {
             let arr = get_array_f32(n);
-            let idxs1 = m4_scalar_without_x(arr.view(), 100);
-            let idxs2 = m4_scalar_without_x_parallel(arr.view(), 100);
-            let idxs3 = m4_scalar_with_x(x.view(), arr.view(), 100);
-            let idxs4 = m4_scalar_with_x_parallel(x.view(), arr.view(), 100);
+            let idxs1 = m4_scalar_without_x(arr.view(), n_out);
+            let idxs2 = m4_scalar_without_x_parallel(arr.view(), n_out);
+            let idxs3 = m4_scalar_with_x(x.view(), arr.view(), n_out);
+            let idxs4 = m4_scalar_with_x_parallel(x.view(), arr.view(), n_out);
             assert_eq!(idxs1, idxs2);
             assert_eq!(idxs1, idxs3);
             assert_eq!(idxs1, idxs4);
         }
     }
 }
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/m4/simd.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/simd.rs`

 * *Files 6% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     fn test_m4_simd_without_x_correct() {
         let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_simd_without_x(arr.view(), 12);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
-        let expected_indices = vec![0, 0, 32, 32, 33, 33, 65, 65, 66, 66, 98, 98];
+        let expected_indices = vec![0, 0, 33, 33, 34, 34, 66, 66, 67, 67, 99, 99];
         let expected_values = expected_indices
             .iter()
             .map(|x| *x as f32)
             .collect::<Vec<f32>>();
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
@@ -107,15 +107,15 @@
     fn test_m4_simd_without_x_parallel_correct() {
         let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_simd_without_x_parallel(arr.view(), 12);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
-        let expected_indices = vec![0, 0, 32, 32, 33, 33, 65, 65, 66, 66, 98, 98];
+        let expected_indices = vec![0, 0, 33, 33, 34, 34, 66, 66, 67, 67, 99, 99];
         let expected_values = expected_indices
             .iter()
             .map(|x| *x as f32)
             .collect::<Vec<f32>>();
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
@@ -127,15 +127,15 @@
         let x = Array1::from(x);
         let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_simd_with_x(x.view(), arr.view(), 12);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
-        let expected_indices = vec![0, 0, 32, 32, 33, 33, 65, 65, 66, 66, 98, 98];
+        let expected_indices = vec![0, 0, 33, 33, 34, 34, 66, 66, 67, 67, 99, 99];
         let expected_values = expected_indices
             .iter()
             .map(|x| *x as f32)
             .collect::<Vec<f32>>();
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
@@ -147,36 +147,36 @@
         let x = Array1::from(x);
         let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_simd_with_x_parallel(x.view(), arr.view(), 12);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
-        let expected_indices = vec![0, 0, 32, 32, 33, 33, 65, 65, 66, 66, 98, 98];
+        let expected_indices = vec![0, 0, 33, 33, 34, 34, 66, 66, 67, 67, 99, 99];
         let expected_values = expected_indices
             .iter()
             .map(|x| *x as f32)
             .collect::<Vec<f32>>();
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
     }
 
     #[test]
     fn test_m4_simd_with_x_gap() {
         // We will create a gap in the middle of the array
-        let x = (0..101).collect::<Vec<i32>>();
+        let x = (0..100).collect::<Vec<i32>>();
 
         // Increment the second half of the array by 50
         let x = x
             .iter()
             .map(|x| if *x > 50 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_simd_with_x(x.view(), arr.view(), 20);
         assert_eq!(sampled_indices.len(), 16); // One full gap
         let expected_indices = vec![0, 0, 29, 29, 30, 30, 50, 50, 51, 51, 69, 69, 70, 70, 99, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
 
@@ -186,30 +186,31 @@
             .map(|x| if *x > 101 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
 
         let sampled_indices = m4_simd_with_x(x.view(), arr.view(), 20);
         assert_eq!(sampled_indices.len(), 17); // Gap with 1 value
         let expected_indices = vec![
-            0, 0, 29, 29, 30, 30, 50, 50, 51, 51, 69, 69, 70, 70, 99, 99, 100,
+            0, 0, 39, 39, 40, 40, 50, 50, 51, 52, 52, 59, 59, 60, 60, 99, 99,
         ];
+        assert_eq!(sampled_indices, Array1::from(expected_indices));
     }
 
     #[test]
     fn test_m4_simd_with_x_gap_parallel() {
         // We will create a gap in the middle of the array
-        let x = (0..101).collect::<Vec<i32>>();
+        let x = (0..100).collect::<Vec<i32>>();
 
         // Increment the second half of the array by 50
         let x = x
             .iter()
             .map(|x| if *x > 50 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = m4_simd_with_x_parallel(x.view(), arr.view(), 20);
         assert_eq!(sampled_indices.len(), 16); // One full gap
         let expected_indices = vec![0, 0, 29, 29, 30, 30, 50, 50, 51, 51, 69, 69, 70, 70, 99, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
 
@@ -219,28 +220,30 @@
             .map(|x| if *x > 101 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
 
         let sampled_indices = m4_simd_with_x_parallel(x.view(), arr.view(), 20);
         assert_eq!(sampled_indices.len(), 17); // Gap with 1 value
         let expected_indices = vec![
-            0, 0, 29, 29, 30, 30, 50, 50, 51, 51, 69, 69, 70, 70, 99, 99, 100,
+            0, 0, 39, 39, 40, 40, 50, 50, 51, 52, 52, 59, 59, 60, 60, 99, 99,
         ];
+        assert_eq!(sampled_indices, Array1::from(expected_indices));
     }
 
     #[test]
     fn test_many_random_runs_correct() {
-        let n = 20_001; // not 20_000 because then the last bin is not "full"
+        let n = 20_003;
+        let n_out = 204;
         let x = (0..n).map(|x| x as i32).collect::<Vec<i32>>();
         let x = Array1::from(x);
         for _ in 0..100 {
             let arr = get_array_f32(n);
-            let idxs1 = m4_simd_without_x(arr.view(), 100);
-            let idxs2 = m4_simd_without_x_parallel(arr.view(), 100);
-            let idxs3 = m4_simd_with_x(x.view(), arr.view(), 100);
-            let idxs4 = m4_simd_with_x_parallel(x.view(), arr.view(), 100);
+            let idxs1 = m4_simd_without_x(arr.view(), n_out);
+            let idxs2 = m4_simd_without_x_parallel(arr.view(), n_out);
+            let idxs3 = m4_simd_with_x(x.view(), arr.view(), n_out);
+            let idxs4 = m4_simd_with_x_parallel(x.view(), arr.view(), n_out);
             assert_eq!(idxs1, idxs2);
             assert_eq!(idxs1, idxs3);
             assert_eq!(idxs1, idxs4);
         }
     }
 }
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmax/generic.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/m4/generic.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,172 +1,195 @@
 use ndarray::Zip;
-use ndarray::{s, Array1, ArrayView1};
+use ndarray::{Array1, ArrayView1};
 
 use rayon::iter::IndexedParallelIterator;
 use rayon::prelude::*;
 
+// TODO: check for duplicate data in the output array
+// -> In the current implementation we always add 4 datapoints per bin (if of
+//    course the bin has >= 4 datapoints). However, the argmin and argmax might
+//    be the start and end of the bin, which would result in duplicate data in
+//    the output array. (this is for example the case for monotonic data).
+
 // --------------------- WITHOUT X
 
 #[inline(always)]
-pub(crate) fn min_max_generic<T: Copy>(
+pub(crate) fn m4_generic<T: Copy + PartialOrd>(
     arr: ArrayView1<T>,
     n_out: usize,
     f_argminmax: fn(ArrayView1<T>) -> (usize, usize),
 ) -> Array1<usize> {
-    // Assumes n_out is a multiple of 2
+    // Assumes n_out is a multiple of 4
     if n_out >= arr.len() {
         return Array1::from((0..arr.len()).collect::<Vec<usize>>());
     }
 
-    let block_size = arr.len() as f64 / (n_out as f64) * 2.0;
-    let block_size = block_size.floor() as usize;
+    // arr.len() - 1 is used to match the delta of a range-index (0..arr.len()-1)
+    let block_size: f64 = (arr.len() - 1) as f64 / (n_out / 4) as f64;
+    let arr_ptr = arr.as_ptr();
 
     let mut sampled_indices: Array1<usize> = Array1::<usize>::default(n_out);
 
-    let mut i: usize = 0; // TODO: for some reason is this faster than enumerate
-    arr.slice(s![..block_size * n_out / 2])
-        .exact_chunks(block_size)
-        .into_iter()
-        .for_each(|step| {
-            let (min_index, max_index) = f_argminmax(step);
-            let offset = block_size * i;
-
-            // Add the indexes in sorted order
-            if min_index < max_index {
-                sampled_indices[2 * i] = min_index + offset;
-                sampled_indices[2 * i + 1] = max_index + offset;
-            } else {
-                sampled_indices[2 * i] = max_index + offset;
-                sampled_indices[2 * i + 1] = min_index + offset;
-            }
-            i += 1;
+    let mut start_idx: usize = 0;
+    for i in 0..n_out / 4 {
+        // Decided to use multiplication instead of adding to the accumulator (end)
+        // as multiplication seems to be less prone to rounding errors.
+        let end: f64 = block_size * (i + 1) as f64;
+        let end_idx: usize = end as usize + 1;
+
+        let (min_index, max_index) = f_argminmax(unsafe {
+            ArrayView1::from_shape_ptr((end_idx - start_idx,), arr_ptr.add(start_idx))
         });
 
+        // Add the indexes in sorted order
+        sampled_indices[4 * i] = start_idx;
+        if min_index < max_index {
+            sampled_indices[4 * i + 1] = min_index + start_idx;
+            sampled_indices[4 * i + 2] = max_index + start_idx;
+        } else {
+            sampled_indices[4 * i + 1] = max_index + start_idx;
+            sampled_indices[4 * i + 2] = min_index + start_idx;
+        }
+        sampled_indices[4 * i + 3] = end_idx - 1;
+
+        start_idx = end_idx;
+    }
+
     sampled_indices
 }
 
 #[inline(always)]
-pub(crate) fn min_max_generic_parallel<T: Copy + PartialOrd + Send + Sync>(
+pub(crate) fn m4_generic_parallel<T: Copy + PartialOrd + Send + Sync>(
     arr: ArrayView1<T>,
     n_out: usize,
     f_argminmax: fn(ArrayView1<T>) -> (usize, usize),
 ) -> Array1<usize> {
-    // Assumes n_out is a multiple of 2
+    // Assumes n_out is a multiple of 4
     if n_out >= arr.len() {
         return Array1::from((0..arr.len()).collect::<Vec<usize>>());
     }
 
-    let block_size = arr.len() as f64 / (n_out as f64) * 2.0;
-    let block_size = block_size.floor() as usize;
+    // arr.len() - 1 is used to match the delta of a range-index (0..arr.len()-1)
+    let block_size: f64 = (arr.len() - 1) as f64 / (n_out / 4) as f64;
 
     // Store the enumerated indexes in the output array
     let mut sampled_indices: Array1<usize> = Array1::from_vec((0..n_out).collect::<Vec<usize>>());
 
-    Zip::from(
-        arr.slice(s![..block_size * n_out / 2])
-            .exact_chunks(block_size),
-    )
-    .and(sampled_indices.exact_chunks_mut(2))
-    .par_for_each(|step, mut sampled_index| {
-        let (min_index, max_index) = f_argminmax(step);
+    Zip::from(sampled_indices.exact_chunks_mut(4)).par_for_each(|mut sampled_index| {
+        let i: f64 = unsafe { *sampled_index.uget(0) >> 2 } as f64;
+        let start_idx: usize = (block_size * i) as usize + (i != 0.0) as usize;
+        let end_idx: usize = (block_size * (i + 1.0)) as usize + 1;
 
+        let (min_index, max_index) = f_argminmax(unsafe {
+            ArrayView1::from_shape_ptr((end_idx - start_idx,), arr.as_ptr().add(start_idx))
+        });
+
+        sampled_index[0] = start_idx;
         // Add the indexes in sorted order
-        let offset = block_size * unsafe { *sampled_index.uget(0) >> 1 };
         if min_index < max_index {
-            sampled_index[0] = min_index + offset;
-            sampled_index[1] = max_index + offset;
+            sampled_index[1] = min_index + start_idx;
+            sampled_index[2] = max_index + start_idx;
         } else {
-            sampled_index[0] = max_index + offset;
-            sampled_index[1] = min_index + offset;
+            sampled_index[1] = max_index + start_idx;
+            sampled_index[2] = min_index + start_idx;
         }
+        sampled_index[3] = end_idx - 1;
     });
 
     sampled_indices
 }
 
 // --------------------- WITH X
 
 #[inline(always)]
-pub(crate) fn min_max_generic_with_x<T: Copy>(
+pub(crate) fn m4_generic_with_x<T: Copy>(
     arr: ArrayView1<T>,
     bin_idx_iterator: impl Iterator<Item = Option<(usize, usize)>>,
     n_out: usize,
     f_argminmax: fn(ArrayView1<T>) -> (usize, usize),
 ) -> Array1<usize> {
-    // Assumes n_out is a multiple of 2
+    // Assumes n_out is a multiple of 4
     if n_out >= arr.len() {
         return Array1::from((0..arr.len()).collect::<Vec<usize>>());
     }
 
-    let ptr = arr.as_ptr();
+    let arr_ptr = arr.as_ptr();
     let mut sampled_indices: Vec<usize> = Vec::with_capacity(n_out);
 
     bin_idx_iterator.for_each(|bin| {
         if let Some((start, end)) = bin {
-            if end <= start + 2 {
-                // If the bin has <= 2 elements, just add them all
+            if end <= start + 4 {
+                // If the bin has <= 4 elements, just add them all
                 for i in start..end {
                     sampled_indices.push(i);
                 }
             } else {
-                // If the bin has at least two elements, add the argmin and argmax
-                let step = unsafe { ArrayView1::from_shape_ptr(end - start, ptr.add(start)) };
+                // If the bin has > 4 elements, add the first and last + argmin and argmax
+                let step = unsafe { ArrayView1::from_shape_ptr(end - start, arr_ptr.add(start)) };
                 let (min_index, max_index) = f_argminmax(step);
 
+                sampled_indices.push(start);
+
                 // Add the indexes in sorted order
                 if min_index < max_index {
                     sampled_indices.push(min_index + start);
                     sampled_indices.push(max_index + start);
                 } else {
                     sampled_indices.push(max_index + start);
                     sampled_indices.push(min_index + start);
                 }
+
+                sampled_indices.push(end - 1);
             }
         }
     });
 
     Array1::from_vec(sampled_indices)
 }
 
 #[inline(always)]
-pub(crate) fn min_max_generic_with_x_parallel<T: Copy + Send + Sync>(
+pub(crate) fn m4_generic_with_x_parallel<T: Copy + PartialOrd + Send + Sync>(
     arr: ArrayView1<T>,
     bin_idx_iterator: impl IndexedParallelIterator<Item = impl Iterator<Item = Option<(usize, usize)>>>,
     n_out: usize,
     f_argminmax: fn(ArrayView1<T>) -> (usize, usize),
 ) -> Array1<usize> {
-    // Assumes n_out is a multiple of 2
+    // Assumes n_out is a multiple of 4
     if n_out >= arr.len() {
         return Array1::from((0..arr.len()).collect::<Vec<usize>>());
     }
 
     Array1::from_vec(
         bin_idx_iterator
             .flat_map(|bin_idx_iterator| {
                 bin_idx_iterator
                     .map(|bin| {
                         match bin {
                             Some((start, end)) => {
-                                if end <= start + 2 {
-                                    // If the bin has <= 2 elements, just return them all
+                                if end <= start + 4 {
+                                    // If the bin has <= 4 elements, just return them all
                                     return (start..end).collect::<Vec<usize>>();
                                 }
 
-                                // If the bin has at least two elements, return the argmin and argmax
+                                // If the bin has > 4 elements, return the first and last + argmin and argmax
                                 let step = unsafe {
                                     ArrayView1::from_shape_ptr(end - start, arr.as_ptr().add(start))
                                 };
                                 let (min_index, max_index) = f_argminmax(step);
 
                                 // Return the indexes in sorted order
+                                let mut sampled_index = vec![start, 0, 0, end - 1];
                                 if min_index < max_index {
-                                    vec![min_index + start, max_index + start]
+                                    sampled_index[1] = min_index + start;
+                                    sampled_index[2] = max_index + start;
                                 } else {
-                                    vec![max_index + start, min_index + start]
+                                    sampled_index[1] = max_index + start;
+                                    sampled_index[2] = min_index + start;
                                 }
+                                sampled_index
                             } // If the bin is empty, return empty Vec
                             None => {
                                 vec![]
                             }
                         }
                     })
                     .collect::<Vec<Vec<usize>>>()
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmax/scalar.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/scalar.rs`

 * *Files 1% similar despite different names*

```diff
@@ -127,17 +127,17 @@
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
     }
 
     #[test]
     fn test_min_max_scalar_with_x_correct() {
-        let x = (0..101).collect::<Vec<i32>>();
+        let x = (0..100).collect::<Vec<i32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = min_max_scalar_with_x(x.view(), arr.view(), 10);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
         let expected_indices = vec![0, 19, 20, 39, 40, 59, 60, 79, 80, 99];
         let expected_values = expected_indices
@@ -147,17 +147,17 @@
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
     }
 
     #[test]
     fn test_min_max_scalar_with_x_parallel_correct() {
-        let x = (0..101).collect::<Vec<i32>>();
+        let x = (0..100).collect::<Vec<i32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = min_max_scalar_with_x_parallel(x.view(), arr.view(), 10);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
         let expected_indices = vec![0, 19, 20, 39, 40, 59, 60, 79, 80, 99];
         let expected_values = expected_indices
@@ -168,23 +168,23 @@
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
     }
 
     #[test]
     fn test_min_max_scalar_with_x_gap() {
         // We will create a gap in the middle of the array
-        let x = (0..101).collect::<Vec<i32>>();
+        let x = (0..100).collect::<Vec<i32>>();
 
         // Increment the second half of the array by 50
         let x = x
             .iter()
             .map(|x| if *x > 50 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = min_max_scalar_with_x(x.view(), arr.view(), 10);
         assert_eq!(sampled_indices.len(), 8); // One full gap
         let expected_indices = vec![0, 29, 30, 50, 51, 69, 70, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
 
@@ -200,52 +200,52 @@
         let expected_indices = vec![0, 39, 40, 50, 51, 52, 59, 60, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
     }
 
     #[test]
     fn test_min_max_scalar_with_x_parallel_gap() {
         // Create a gap in the middle of the array
-        let x = (0..101).collect::<Vec<i32>>();
+        let x = (0..100).collect::<Vec<i32>>();
 
         // Increment the second half of the array by 50
         let x = x
             .iter()
             .map(|x| if *x > 50 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = min_max_scalar_with_x_parallel(x.view(), arr.view(), 10);
         assert_eq!(sampled_indices.len(), 8); // One full gap
         let expected_indices = vec![0, 29, 30, 50, 51, 69, 70, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
 
         // Increment the second half of the array by 50 again
         let x = x
             .iter()
             .map(|x| if *x > 101 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
-        println!("{:?}", x);
         let x = Array1::from(x);
 
         let sampled_indices = min_max_scalar_with_x_parallel(x.view(), arr.view(), 10);
         assert_eq!(sampled_indices.len(), 9); // Gap with 1 value
         let expected_indices = vec![0, 39, 40, 50, 51, 52, 59, 60, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
     }
 
     #[test]
     fn test_many_random_runs_same_output() {
-        let n: usize = 20_001;
-        let n_out = 200;
+        let n: usize = 20_003;
+        let n_out = 202;
         let x = (0..n as i32).collect::<Vec<i32>>();
         let x = Array1::from(x);
         for _ in 0..100 {
-            let arr = get_array_f32(n);
+            let mut arr = get_array_f32(n);
+            arr[n - 1] = f32::INFINITY; // Make sure the last value is always the max
             let idxs1 = min_max_scalar_without_x(arr.view(), n_out);
             let idxs2 = min_max_scalar_without_x_parallel(arr.view(), n_out);
             let idxs3 = min_max_scalar_with_x(x.view(), arr.view(), n_out);
             let idxs4 = min_max_scalar_with_x_parallel(x.view(), arr.view(), n_out);
             assert_eq!(idxs1, idxs2);
             assert_eq!(idxs1, idxs3);
             assert_eq!(idxs1, idxs4);
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmax/simd.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmax/simd.rs`

 * *Files 2% similar despite different names*

```diff
@@ -127,18 +127,17 @@
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
     }
 
     #[test]
     fn test_min_max_simd_with_x_correct() {
-        // 101 elements to avoid rounding errors in the binning
-        let x = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let x = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = min_max_simd_with_x(x.view(), arr.view(), 10);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
         let expected_indices = vec![0, 19, 20, 39, 40, 59, 60, 79, 80, 99];
         let expected_values = expected_indices
@@ -148,17 +147,17 @@
 
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
     }
 
     #[test]
     fn test_min_max_simd_with_x_parallel_correct() {
-        let x = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let x = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = min_max_simd_with_x_parallel(x.view(), arr.view(), 10);
         let sampled_values = sampled_indices.mapv(|x| arr[x]);
 
         let expected_indices = vec![0, 19, 20, 39, 40, 59, 60, 79, 80, 99];
         let expected_values = expected_indices
@@ -169,23 +168,23 @@
         assert_eq!(sampled_indices, Array1::from(expected_indices));
         assert_eq!(sampled_values, Array1::from(expected_values));
     }
 
     #[test]
     fn test_min_max_simd_with_x_gap() {
         // We will create a gap in the middle of the array
-        let x = (0..101).collect::<Vec<i32>>();
+        let x = (0..100).collect::<Vec<i32>>();
 
         // Increment the second half of the array by 50
         let x = x
             .iter()
             .map(|x| if *x > 50 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = min_max_simd_with_x(x.view(), arr.view(), 10);
         assert_eq!(sampled_indices.len(), 8); // One full gap
         let expected_indices = vec![0, 29, 30, 50, 51, 69, 70, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
 
@@ -201,52 +200,52 @@
         let expected_indices = vec![0, 39, 40, 50, 51, 52, 59, 60, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
     }
 
     #[test]
     fn test_min_max_simd_with_x_parallel_gap() {
         // Create a gap in the middle of the array
-        let x = (0..101).collect::<Vec<i32>>();
+        let x = (0..100).collect::<Vec<i32>>();
 
         // Increment the second half of the array by 50
         let x = x
             .iter()
             .map(|x| if *x > 50 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
         let x = Array1::from(x);
-        let arr = (0..101).map(|x| x as f32).collect::<Vec<f32>>();
+        let arr = (0..100).map(|x| x as f32).collect::<Vec<f32>>();
         let arr = Array1::from(arr);
 
         let sampled_indices = min_max_simd_with_x_parallel(x.view(), arr.view(), 10);
         assert_eq!(sampled_indices.len(), 8); // One full gap
         let expected_indices = vec![0, 29, 30, 50, 51, 69, 70, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
 
         // Increment the second half of the array by 50 again
         let x = x
             .iter()
             .map(|x| if *x > 101 { *x + 50 } else { *x })
             .collect::<Vec<i32>>();
-        println!("{:?}", x);
         let x = Array1::from(x);
 
         let sampled_indices = min_max_simd_with_x_parallel(x.view(), arr.view(), 10);
         assert_eq!(sampled_indices.len(), 9); // Gap with 1 value
         let expected_indices = vec![0, 39, 40, 50, 51, 52, 59, 60, 99];
         assert_eq!(sampled_indices, Array1::from(expected_indices));
     }
 
     #[test]
     fn test_many_random_runs_same_output() {
-        let n = 20_001;
-        let n_out = 200;
+        let n = 20_003;
+        let n_out = 202;
         let x = (0..n).map(|x| x as i32).collect::<Vec<i32>>();
         let x = Array1::from(x);
         for _ in 0..100 {
-            let arr = get_array_f32(n);
+            let mut arr = get_array_f32(n);
+            arr[n - 1] = f32::INFINITY; // Make sure the last value is always the max
             let idxs1 = min_max_simd_without_x(arr.view(), n_out);
             let idxs2 = min_max_simd_without_x_parallel(arr.view(), n_out);
             let idxs3 = min_max_simd_with_x(x.view(), arr.view(), n_out);
             let idxs4 = min_max_simd_with_x_parallel(x.view(), arr.view(), n_out);
             assert_eq!(idxs1, idxs2);
             assert_eq!(idxs1, idxs3);
             assert_eq!(idxs1, idxs4);
```

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmaxlttb/generic.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/generic.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmaxlttb/scalar.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/scalar.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/minmaxlttb/simd.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/minmaxlttb/simd.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/local_dependencies/downsample_rs/src/searchsorted.rs` & `tsdownsample-0.1.2a0/local_dependencies/downsample_rs/src/searchsorted.rs`

 * *Files 17% similar despite different names*

```diff
@@ -5,37 +5,55 @@
 use std::thread::available_parallelism;
 
 use super::types::Num;
 use num_traits::{AsPrimitive, FromPrimitive};
 
 // ---------------------- Binary search ----------------------
 
+/// Binary search for the index position of the given value in the given array.
+/// The array must be sorted in ascending order and contain no duplicates.
+///
+/// Complies with the Python bisect function
+/// https://docs.python.org/3/library/bisect.html#bisect.bisect
+///
 // #[inline(always)]
 fn binary_search<T: Copy + PartialOrd>(
     arr: ArrayView1<T>,
     value: T,
     left: usize,
     right: usize,
 ) -> usize {
     let mut size: usize = right - left;
     let mut left: usize = left;
     let mut right: usize = right;
-    // Return the index where the value is <= arr[index] and arr[index+1] < value
+    // Return the index where the value is >= arr[index] and arr[index-1] < value
     while left < right {
         let mid = left + size / 2;
         if arr[mid] < value {
             left = mid + 1;
         } else {
             right = mid;
         }
         size = right - left;
     }
-    left
+    if arr[left] <= value {
+        left + 1
+    } else {
+        left
+    }
 }
 
+/// Binary search for the index position of the given value in the given array.
+/// The array must be sorted in ascending order and contain no duplicates.
+///
+/// The mid index is pre-guessed to speed up the search.
+///
+/// Complies with the Python bisect function
+/// https://docs.python.org/3/library/bisect.html#bisect.bisect
+///
 // #[inline(always)]
 fn binary_search_with_mid<T: Copy + PartialOrd>(
     arr: ArrayView1<T>,
     value: T,
     left: usize,
     right: usize,
     mid: usize,
@@ -50,16 +68,19 @@
             left = mid + 1;
         } else {
             right = mid;
         }
         let size = right - left;
         mid = left + size / 2;
     }
-    // if arr[left] == value { left + 1 } else { left }
-    left
+    if arr[left] <= value {
+        left + 1
+    } else {
+        left
+    }
 }
 
 // ------------------- Equidistant binning --------------------
 
 // --- Sequential version
 
 pub(crate) fn get_equidistant_bin_idx_iterator<T>(
@@ -72,23 +93,25 @@
     assert!(nb_bins >= 2);
     // 1. Compute the step between each bin
     // Divide by nb_bins to avoid overflow!
     let val_step: f64 =
         (arr[arr.len() - 1].as_() / nb_bins as f64) - (arr[0].as_() / nb_bins as f64);
     // Estimate the step between each index (used to pre-guess the mid index)
     let idx_step: usize = arr.len() / nb_bins;
+
     // 2. The moving index & value
-    let mut value: f64 = arr[0].as_(); // Search value
+    let arr0: f64 = arr[0].as_(); // The first value of the array
     let mut idx: usize = 0; // Index of the search value
-                            // 3. Iterate over the bins
-    (0..nb_bins).map(move |_| {
+
+    // 3. Iterate over the bins
+    (0..nb_bins).map(move |i| {
         let start_idx: usize = idx; // Start index of the bin (previous end index)
-                                    // Update the search value
-        value += val_step;
-        let search_value: T = T::from_f64(value).unwrap();
+
+        // Update the search value
+        let search_value: T = T::from_f64(arr0 + val_step * (i + 1) as f64).unwrap();
         if arr[start_idx] >= search_value {
             // If the first value of the bin is already >= the search value,
             // then the bin is empty.
             return None;
         }
         // Update the pre-guess index
         let mid: usize = std::cmp::min(idx + idx_step, arr.len() - 2);
@@ -129,30 +152,34 @@
     let nb_bins_per_thread = nb_bins / nb_threads;
     let nb_bins_last_thread = nb_bins - nb_bins_per_thread * (nb_threads - 1);
     // 3. Iterate over the number of threads
     // -> for each thread perform the binary search sorted with moving left and
     // yield the indices (using the same idea as for the sequential version)
     (0..nb_threads).into_par_iter().map(move |i| {
         // The moving index & value (for the thread)
-        let mut value: f64 = sequential_add_mul(arr0, val_step, i * nb_bins_per_thread); // Search value
-        let start_value: T = T::from_f64(value).unwrap();
+        let arr0_thr: f64 = sequential_add_mul(arr0, val_step, i * nb_bins_per_thread); // Search value
+        let start_value: T = T::from_f64(arr0_thr).unwrap();
         // Search the start of the fist bin (of the thread)
-        let mut idx: usize = binary_search(arr, start_value, 0, arr.len() - 1); // Index of the search value
-                                                                                // The number of bins for the thread
+        let mut idx: usize = 0; // Index of the search value
+        if i > 0 {
+            idx = binary_search(arr, start_value, 0, arr.len() - 1);
+        }
+
+        // The number of bins for the thread
         let nb_bins_thread = if i == nb_threads - 1 {
             nb_bins_last_thread
         } else {
             nb_bins_per_thread
         };
         // Perform sequential binary search for the end of the bins (of the thread)
-        (0..nb_bins_thread).map(move |_| {
+        (0..nb_bins_thread).map(move |i| {
             let start_idx: usize = idx; // Start index of the bin (previous end index)
-                                        // Update the search value
-            value += val_step;
-            let search_value: T = T::from_f64(value).unwrap();
+
+            // Update the search value
+            let search_value: T = T::from_f64(arr0_thr + val_step * (i + 1) as f64).unwrap();
             if arr[start_idx] >= search_value {
                 // If the first value of the bin is already >= the search value,
                 // then the bin is empty.
                 return None;
             }
             idx = binary_search(arr, search_value, idx, arr.len() - 1); // End index of the bin
             Some((start_idx, idx))
@@ -167,93 +194,109 @@
     use super::*;
     use ndarray::Array1;
 
     extern crate dev_utils;
     use dev_utils::utils::get_random_array;
 
     #[test]
+    fn test_search_sorted_identicial_to_np_linspace_searchsorted() {
+        // Create a 0..9999 array
+        let arr = Array1::from((0..10_000).collect::<Vec<usize>>());
+        assert!(arr.len() == 10_000);
+        let iterator = get_equidistant_bin_idx_iterator(arr.view(), 4);
+        // Check the iterator
+        let mut idx: usize = 0;
+        for bin in iterator {
+            let (start_idx, end_idx) = bin.unwrap();
+            assert!(start_idx == idx);
+            assert!(end_idx == idx + 2_500);
+            idx += 2_500;
+        }
+    }
+
+    #[test]
     fn test_binary_search() {
         let arr = Array1::from(vec![1, 2, 3, 4, 5, 6, 7, 8, 9, 10]);
         assert_eq!(binary_search(arr.view(), 0, 0, arr.len() - 1), 0);
-        assert_eq!(binary_search(arr.view(), 1, 0, arr.len() - 1), 0);
-        assert_eq!(binary_search(arr.view(), 2, 0, arr.len() - 1), 1);
-        assert_eq!(binary_search(arr.view(), 3, 0, arr.len() - 1), 2);
-        assert_eq!(binary_search(arr.view(), 4, 0, arr.len() - 1), 3);
-        assert_eq!(binary_search(arr.view(), 5, 0, arr.len() - 1), 4);
-        assert_eq!(binary_search(arr.view(), 6, 0, arr.len() - 1), 5);
-        assert_eq!(binary_search(arr.view(), 7, 0, arr.len() - 1), 6);
-        assert_eq!(binary_search(arr.view(), 8, 0, arr.len() - 1), 7);
-        assert_eq!(binary_search(arr.view(), 9, 0, arr.len() - 1), 8);
-        assert_eq!(binary_search(arr.view(), 10, 0, arr.len() - 1), 9);
-        assert_eq!(binary_search(arr.view(), 11, 0, arr.len() - 1), 9);
+        assert_eq!(binary_search(arr.view(), 1, 0, arr.len() - 1), 1);
+        assert_eq!(binary_search(arr.view(), 2, 0, arr.len() - 1), 2);
+        assert_eq!(binary_search(arr.view(), 3, 0, arr.len() - 1), 3);
+        assert_eq!(binary_search(arr.view(), 4, 0, arr.len() - 1), 4);
+        assert_eq!(binary_search(arr.view(), 5, 0, arr.len() - 1), 5);
+        assert_eq!(binary_search(arr.view(), 6, 0, arr.len() - 1), 6);
+        assert_eq!(binary_search(arr.view(), 7, 0, arr.len() - 1), 7);
+        assert_eq!(binary_search(arr.view(), 8, 0, arr.len() - 1), 8);
+        assert_eq!(binary_search(arr.view(), 9, 0, arr.len() - 1), 9);
+        assert_eq!(binary_search(arr.view(), 10, 0, arr.len() - 1), 10);
+        assert_eq!(binary_search(arr.view(), 11, 0, arr.len() - 1), 10);
     }
 
     #[test]
     fn test_binary_search_with_mid() {
         let arr = Array1::from(vec![1, 2, 3, 4, 5, 6, 7, 8, 9, 10]);
         assert_eq!(
             binary_search_with_mid(arr.view(), 0, 0, arr.len() - 1, 0),
             0
         );
         assert_eq!(
             binary_search_with_mid(arr.view(), 1, 0, arr.len() - 1, 0),
-            0
+            1
         );
         assert_eq!(
             binary_search_with_mid(arr.view(), 2, 0, arr.len() - 1, 1),
-            1
+            2
         );
         assert_eq!(
             binary_search_with_mid(arr.view(), 3, 0, arr.len() - 1, 2),
-            2
+            3
         );
         assert_eq!(
             binary_search_with_mid(arr.view(), 4, 0, arr.len() - 1, 3),
-            3
+            4
         );
         assert_eq!(
             binary_search_with_mid(arr.view(), 5, 0, arr.len() - 1, 4),
-            4
+            5
         );
         assert_eq!(
             binary_search_with_mid(arr.view(), 6, 0, arr.len() - 1, 5),
-            5
+            6
         );
         assert_eq!(
             binary_search_with_mid(arr.view(), 7, 0, arr.len() - 1, 6),
-            6
+            7
         );
         assert_eq!(
             binary_search_with_mid(arr.view(), 8, 0, arr.len() - 1, 7),
-            7
+            8
         );
         assert_eq!(
             binary_search_with_mid(arr.view(), 9, 0, arr.len() - 1, 8),
-            8
+            9
         );
         assert_eq!(
             binary_search_with_mid(arr.view(), 10, 0, arr.len() - 1, 9),
-            9
+            10
         );
         // This line causes the code to crash -> because value higher than arr[mid]
-        // assert_eq!(binary_search_with_mid(arr.view(), 11, 0, arr.len() - 1, 9), 9);
+        // assert_eq!(binary_search_with_mid(arr.view(), 11, 0, arr.len() - 1, 9), 10);
     }
 
     #[test]
     fn test_get_equidistant_bin_idxs() {
         let arr = Array1::from(vec![1, 2, 3, 4, 5, 6, 7, 8, 9, 10]);
         let bin_idxs_iter = get_equidistant_bin_idx_iterator(arr.view(), 3);
         let bin_idxs = bin_idxs_iter.map(|x| x.unwrap().0).collect::<Vec<usize>>();
-        assert_eq!(bin_idxs, vec![0, 3, 6]);
+        assert_eq!(bin_idxs, vec![0, 4, 7]);
         let bin_idxs_iter = get_equidistant_bin_idx_iterator_parallel(arr.view(), 3);
         let bin_idxs = bin_idxs_iter
             .map(|x| x.map(|x| x.unwrap().0).collect::<Vec<usize>>())
             .flatten()
             .collect::<Vec<usize>>();
-        assert_eq!(bin_idxs, vec![0, 3, 6]);
+        assert_eq!(bin_idxs, vec![0, 4, 7]);
     }
 
     #[test]
     fn test_many_random_same_result() {
         let n = 5_000;
         let nb_bins = 100;
         for _ in 0..100 {
```

### Comparing `tsdownsample-0.1.1/Cargo.toml` & `tsdownsample-0.1.2a0/Cargo.toml`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/.github/workflows/ci-downsample_rs.yml` & `tsdownsample-0.1.2a0/.github/workflows/ci-downsample_rs.yml`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/.github/workflows/ci-tsdownsample.yml` & `tsdownsample-0.1.2a0/.github/workflows/ci-tsdownsample.yml`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
           rustup update nightly --no-self-update
           rustup default nightly
       - name: Cache rust
         uses: Swatinem/rust-cache@v2
 
       - name: install develop version
         run: make install
-      # python setup.py develop
         
       - run: pip install -r tests/requirements.txt
 
       - run: pip freeze
 
       - run: make test  # Test Python
```

### Comparing `tsdownsample-0.1.1/.gitignore` & `tsdownsample-0.1.2a0/.gitignore`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/CONTRIBUTING.md` & `tsdownsample-0.1.2a0/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,37 @@
 
 ## The basics
 
 tsdownsample welcomes contributions in the form of Pull Requests. For small changes (e.g., bug fixes), feel free to submit a PR. For larger changes (e.g., new functionality, major refactoring), consider submitting an [Issue](https://github.com/predict-idlab/tsdownsample/issues) outlining your proposed change.
 
 ### Prerequisites
 
-tsdownsample is written in Rust. You'll need to install the [Rust toolchain](https://www.rust-lang.org/tools/install) for development.  
+tsdownsample is written in Rust. You'll need to install the [Rust toolchain](https://www.rust-lang.org/tools/install) for development.
 
 This project uses the nightly version of Rust. You can install it with:
 
 ```bash
 rustup install nightly
 ```
 
 and then set it as the default toolchain with:
 
 ```bash
 rustup default nightly
 ```
 
-### tsdownsample 
+### Installing (locally)
+
+To install the package locally, run the following command in the root directory of the project:
+
+```bash
+make install
+```
+
+### tsdownsample
 
 The structure of the tsdownsample project is as follows:
 
 ```bash
 tsdownsample
 ├── Cargo.toml
 ├── README.md
@@ -65,15 +73,15 @@
 ```
 
 To run the tests and linting:
 ```bash
 make lint
 ```
 
-### Formatting 
+### Formatting
 
 We use [black](https://github.com/psf/black) and [isort](https://github.com/PyCQA/isort) to format the Python code.
 
 To format the code, run the following command (more details in the [Makefile](Makefile)):
 ```sh
 make format
 ```
```

### Comparing `tsdownsample-0.1.1/LICENSE` & `tsdownsample-0.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/Makefile` & `tsdownsample-0.1.2a0/Makefile`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 .DEFAULT_GOAL := all
-isort = isort tsdownsample tests
 black = black tsdownsample tests
 
 install:
-	pip install -e .
+	pip install .
 
 .PHONY: install-dev-requirements
 install-dev-requirements:
 	pip install -r tests/requirements.txt
 	pip install -r tests/requirements-linting.txt
 
 .PHONY: format
 format:
-	$(isort)
+	ruff --fix tsdownsample tests
 	$(black)
 	cargo fmt
 
 .PHONY: lint-python
 lint-python:
 	ruff tsdownsample tests
-	$(isort) --check-only --df
 	$(black) --check --diff
 
 .PHONY: lint-rust
 lint-rust:
 	cargo fmt --version
 	cargo fmt --all -- --check
 	cargo clippy --version
@@ -35,15 +33,19 @@
 .PHONY: mypy
 mypy:
 	mypy tsdownsample
 
 
 .PHONY: test
 test:
-	pytest --cov=tsdownsample --cov-report=term-missing --cov-report=html --cov-report=xml
+	pytest --benchmark-skip --cov=tsdownsample --cov-report=term-missing --cov-report=html --cov-report=xml
+
+.PHONY: bench
+bench:
+	pytest --benchmark-only --benchmark-max-time=5
 
 
 .PHONY: all
 all: lint mypy test
 
 .PHONY: clean
 clean:
```

### Comparing `tsdownsample-0.1.1/README.md` & `tsdownsample-0.1.2a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![Testing](https://github.com/predict-idlab/tsdownsample/actions/workflows/ci-tsdownsample.yml/badge.svg)](https://github.com/predict-idlab/tsdownsample/actions/workflows/ci-tsdownsample.yml)
 <!-- TODO: codecov -->
 
 Extremely fast **time series downsampling 📈** for visualization, written in Rust.
 
 ## Features ✨
 
-* **Fast**: written in rust with PyO3 bindings  
+* **Fast**: written in rust with PyO3 bindings
   - leverages optimized [argminmax](https://github.com/jvdd/argminmax) - which is SIMD accelerated with runtime feature detection
   - scales linearly with the number of data points
   <!-- TODO check if it scales sublinearly -->
   - multithreaded with Rayon (in Rust)
     <details>
       <summary><i>Why we do not use Python multiprocessing</i></summary>
       Citing the <a href="https://pyo3.rs/v0.17.3/parallelism.html">PyO3 docs on parallelism</a>:<br>
@@ -55,23 +55,30 @@
 # Create a time series
 y = np.random.randn(10_000_000)
 x = np.arange(len(y))
 
 # Downsample to 1000 points (assuming constant sampling rate)
 s_ds = MinMaxLTTBDownsampler().downsample(y, n_out=1000)
 
+# Select downsampled data
+downsampled_y = y[s_ds]
+
 # Downsample to 1000 points using the (possible irregularly spaced) x-data
 s_ds = MinMaxLTTBDownsampler().downsample(x, y, n_out=1000)
+
+# Select downsampled data
+downsampled_x = x[s_ds]
+downsampled_y = y[s_ds]
 ```
 
-## Downsampling algorithms & API 
+## Downsampling algorithms & API
 
 ### Downsampling API 📑
 
-Each downsampling algorithm is implemented as a class that implements a `downsample` method.  
+Each downsampling algorithm is implemented as a class that implements a `downsample` method.
 The signature of the `downsample` method:
 
 ```
 downsample([x], y, n_out, **kwargs) -> ndarray[uint64]
 ```
 
 **Arguments**:
@@ -80,15 +87,15 @@
 - `n_out` is a mandatory keyword argument that defines the number of output values<sup>*</sup>
 - `**kwargs` are optional keyword arguments *(see [table below](#downsampling-algorithms-📈))*:
   - `parallel`: whether to use multi-threading (default: `False`)<sup>**</sup>
   - ...
 
 **Returns**: a `ndarray[uint64]` of indices that can be used to index the original data.
 
-<sup>*</sup><i>When there are gaps in the time series, fewer than `n_out` indices may be returned.</i>  
+<sup>*</sup><i>When there are gaps in the time series, fewer than `n_out` indices may be returned.</i>
 <sup>**</sup><i>`parallel` is not supported for `LTTBDownsampler`.</i>
 ### Downsampling algorithms 📈
 
 The following downsampling algorithms (classes) are implemented:
 
 | Downsampler | Description | `**kwargs` |
 | ---:| --- |--- |
```

#### html2text {}

```diff
@@ -35,33 +35,34 @@
 sufficient. This mapping allows to use the hardware supported scalar and SIMD
 i16 instructions - while not producing any memory overhead ð
 More details are described in argminmax_PR_#1.  * **Easy to use**: simple &
 flexible API ## Install ```bash pip install tsdownsample ``` ## Usage ```python
 from tsdownsample import MinMaxLTTBDownsampler import numpy as np # Create a
 time series y = np.random.randn(10_000_000) x = np.arange(len(y)) # Downsample
 to 1000 points (assuming constant sampling rate) s_ds = MinMaxLTTBDownsampler
-().downsample(y, n_out=1000) # Downsample to 1000 points using the (possible
-irregularly spaced) x-data s_ds = MinMaxLTTBDownsampler().downsample(x, y,
-n_out=1000) ``` ## Downsampling algorithms & API ### Downsampling API ð Each
-downsampling algorithm is implemented as a class that implements a `downsample`
-method. The signature of the `downsample` method: ``` downsample([x], y, n_out,
-**kwargs) -> ndarray[uint64] ``` **Arguments**: - `x` is optional - `x` and `y`
-are both positional arguments - `n_out` is a mandatory keyword argument that
-defines the number of output values* - `**kwargs` are optional keyword
-arguments *(see [table below](#downsampling-algorithms-ð))*: - `parallel`:
-whether to use multi-threading (default: `False`)** - ... **Returns**: a
-`ndarray[uint64]` of indices that can be used to index the original data. *When
-there are gaps in the time series, fewer than `n_out` indices may be returned.
-**`parallel` is not supported for `LTTBDownsampler`. ### Downsampling
-algorithms ð The following downsampling algorithms (classes) are
-implemented: | Downsampler | Description | `**kwargs` | | ---:| --- |--- | |
-`MinMaxDownsampler` | selects the **min and max** value in each bin |
-`parallel` | | `M4Downsampler` | selects the [**min, max, first and last**]
-(https://dl.acm.org/doi/pdf/10.14778/2732951.2732953) value in each bin |
-`parallel` | | `LTTBDownsampler` | performs the [**Largest Triangle Three
+().downsample(y, n_out=1000) # Select downsampled data downsampled_y = y[s_ds]
+# Downsample to 1000 points using the (possible irregularly spaced) x-data s_ds
+= MinMaxLTTBDownsampler().downsample(x, y, n_out=1000) # Select downsampled
+data downsampled_x = x[s_ds] downsampled_y = y[s_ds] ``` ## Downsampling
+algorithms & API ### Downsampling API ð Each downsampling algorithm is
+implemented as a class that implements a `downsample` method. The signature of
+the `downsample` method: ``` downsample([x], y, n_out, **kwargs) -> ndarray
+[uint64] ``` **Arguments**: - `x` is optional - `x` and `y` are both positional
+arguments - `n_out` is a mandatory keyword argument that defines the number of
+output values* - `**kwargs` are optional keyword arguments *(see [table below]
+(#downsampling-algorithms-ð))*: - `parallel`: whether to use multi-threading
+(default: `False`)** - ... **Returns**: a `ndarray[uint64]` of indices that can
+be used to index the original data. *When there are gaps in the time series,
+fewer than `n_out` indices may be returned. **`parallel` is not supported for
+`LTTBDownsampler`. ### Downsampling algorithms ð The following downsampling
+algorithms (classes) are implemented: | Downsampler | Description | `**kwargs`
+| | ---:| --- |--- | | `MinMaxDownsampler` | selects the **min and max** value
+in each bin | `parallel` | | `M4Downsampler` | selects the [**min, max, first
+and last**](https://dl.acm.org/doi/pdf/10.14778/2732951.2732953) value in each
+bin | `parallel` | | `LTTBDownsampler` | performs the [**Largest Triangle Three
 Buckets**](https://skemman.is/bitstream/1946/15343/3/SS_MSthesis.pdf) algorithm
 | | `MinMaxLTTBDownsampler` | (*new two-step algorithm ð*) first selects
 `n_out` * `minmax_ratio` **min and max** values, then further reduces these to
 `n_out` values using the **Largest Triangle Three Buckets** algorithm |
 `parallel`, `minmax_ratio`* | *Default value for `minmax_ratio` is 30, which is
 empirically proven to be a good default. (More details in our upcomming paper)
 ## Limitations & assumptions ð¨ Assumes; 1. `x`-data is (non-strictly)
```

### Comparing `tsdownsample-0.1.1/pyproject.toml` & `tsdownsample-0.1.2a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "tsdownsample"
-description = "Extremely fast time series downsampling in Rust"
-version = "0.1.1"
+description = "Time series downsampling in rust"
+version = "0.1.2a0"
 requires-python = ">=3.7"
 dependencies = ["numpy"]
 authors = [{name = "Jeroen Van Der Donckt"}]
 readme = "README.md"
 license = {text = "MIT"}
 keywords = ["time series", "downsampling", "rust", "data science", "visualization"]
 classifiers = [
@@ -32,36 +32,26 @@
 
 # Build Python bindings for rust
 [tool.maturin]
 bindings = "pyo3"
 
 # Linting
 [tool.ruff]
+select = ["E", "F", "I"]
 line-length = 88
 extend-select = ["Q"]
 ignore = ["E402", "F403"]
 
 # Formatting
 [tool.black]
 color = true
 line-length = 88
 skip-string-normalization = true
 skip-magic-trailing-comma = true
 
-# Sort imports
-[tool.isort]
-line_length = 88
-known_first_party = ["tsdownsample"]
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-combine_as_imports = true
-color_output = true
-skip = "tests/toml_test.py"
-
 # Static typing
 [tool.mypy]
 follow_imports = "normal"
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 check_untyped_defs = true
```

### Comparing `tsdownsample-0.1.1/src/lib.rs` & `tsdownsample-0.1.2a0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/tests/test_config.py` & `tsdownsample-0.1.2a0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/tests/test_rust_mods.py` & `tsdownsample-0.1.2a0/tests/test_rust_mods.py`

 * *Files identical despite different names*

### Comparing `tsdownsample-0.1.1/tests/test_tsdownsample.py` & `tsdownsample-0.1.2a0/tests/test_tsdownsample.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,195 @@
+from typing import Iterable
+
 import numpy as np
 import pytest
 from test_config import supported_dtypes_x, supported_dtypes_y
 
 from tsdownsample import (  # MeanDownsampler,; MedianDownsampler,
     EveryNthDownsampler,
     LTTBDownsampler,
     M4Downsampler,
     MinMaxDownsampler,
     MinMaxLTTBDownsampler,
 )
+from tsdownsample.downsampling_interface import AbstractDownsampler
 
 # TODO: Improve tests
 #   - compare implementations with existing plotly_resampler implementations
 
 
-def test_m4_downsampler():
-    """Test M4 downsampler."""
-    arr = np.array(np.arange(10_000))
-    s_downsampled = M4Downsampler().downsample(arr, n_out=100)
-    assert s_downsampled[0] == 0
-    assert s_downsampled[-1] == len(arr) - 1
+RUST_DOWNSAMPLERS = [
+    MinMaxDownsampler(),
+    M4Downsampler(),
+    LTTBDownsampler(),
+    MinMaxLTTBDownsampler(),
+]
 
+OTHER_DOWNSAMPLERS = [EveryNthDownsampler()]
 
-def test_minmax_downsampler():
-    """Test MinMax downsampler."""
-    arr = np.array(np.arange(10_000))
-    s_downsampled = MinMaxDownsampler().downsample(arr, n_out=100)
-    assert s_downsampled[0] == 0
-    assert s_downsampled[-1] == len(arr) - 1
 
+def generate_rust_downsamplers() -> Iterable[AbstractDownsampler]:
+    for downsampler in RUST_DOWNSAMPLERS:
+        yield downsampler
 
-def test_lttb_downsampler():
-    """Test LTTB downsampler."""
-    arr = np.array(np.arange(10_000))
-    s_downsampled = LTTBDownsampler().downsample(arr, n_out=100)
-    assert s_downsampled[0] == 0
-    assert s_downsampled[-1] == len(arr) - 1
 
+def generate_all_downsamplers() -> Iterable[AbstractDownsampler]:
+    for downsampler in RUST_DOWNSAMPLERS + OTHER_DOWNSAMPLERS:
+        yield downsampler
+
+
+@pytest.mark.parametrize("downsampler", generate_all_downsamplers())
+def test_serialization(downsampler: AbstractDownsampler):
+    """Test serialization."""
+    from copy import copy, deepcopy
+
+    dc = copy(downsampler)
+    ddc = deepcopy(downsampler)
 
-def test_minmaxlttb_downsampler():
-    """Test MinMaxLTTB downsampler."""
-    arr = np.array(np.arange(10_000))
-    s_downsampled = MinMaxLTTBDownsampler().downsample(arr, n_out=100)
+    arr = np.arange(10_000)
+    orig_downsampled = downsampler.downsample(arr, n_out=100)
+    dc_downsampled = dc.downsample(arr, n_out=100)
+    ddc_downsampled = ddc.downsample(arr, n_out=100)
+    assert np.all(orig_downsampled == dc_downsampled)
+    assert np.all(orig_downsampled == ddc_downsampled)
+
+
+@pytest.mark.parametrize("downsampler", generate_rust_downsamplers())
+def test_rust_downsampler(downsampler: AbstractDownsampler):
+    """Test the Rust downsamplers."""
+    arr = np.arange(10_000)
+    s_downsampled = downsampler.downsample(arr, n_out=100)
     assert s_downsampled[0] == 0
     assert s_downsampled[-1] == len(arr) - 1
 
 
 def test_everynth_downsampler():
     """Test EveryNth downsampler."""
-    arr = np.array(np.arange(10_000))
-    s_downsampled = EveryNthDownsampler().downsample(arr, n_out=100)
+    arr = np.arange(10_000)
+    downsampler = EveryNthDownsampler()
+    s_downsampled = downsampler.downsample(arr, n_out=100)
     assert s_downsampled[0] == 0
     assert s_downsampled[-1] == 9_900
 
 
-## Parallel downsampling
-
-rust_downsamplers = [
-    MinMaxDownsampler(),
-    M4Downsampler(),
-    LTTBDownsampler(),
-    MinMaxLTTBDownsampler(),
-]
-
-
-def test_parallel_downsampling():
+@pytest.mark.parametrize("downsampler", generate_rust_downsamplers())
+def test_parallel_downsampling(downsampler: AbstractDownsampler):
     """Test parallel downsampling."""
     arr = np.random.randn(10_000).astype(np.float32)
-    for downsampler in rust_downsamplers:
-        s_downsampled = downsampler.downsample(arr, n_out=100, parallel=False)
-        s_downsampled_p = downsampler.downsample(arr, n_out=100, parallel=True)
-        assert np.all(s_downsampled == s_downsampled_p)
+    s_downsampled = downsampler.downsample(arr, n_out=100, parallel=False)
+    s_downsampled_p = downsampler.downsample(arr, n_out=100, parallel=True)
+    assert np.all(s_downsampled == s_downsampled_p)
 
 
-def test_parallel_downsampling_with_x():
+@pytest.mark.parametrize("downsampler", generate_rust_downsamplers())
+def test_parallel_downsampling_with_x(downsampler: AbstractDownsampler):
     """Test parallel downsampling with x."""
     arr = np.random.randn(10_001).astype(np.float32)  # 10_001 to test edge case
     idx = np.arange(len(arr))
-    for downsampler in rust_downsamplers:
-        s_downsampled = downsampler.downsample(idx, arr, n_out=100, parallel=False)
-        s_downsampled_p = downsampler.downsample(idx, arr, n_out=100, parallel=True)
-        assert np.all(s_downsampled == s_downsampled_p)
-
-
-## Using x
+    s_downsampled = downsampler.downsample(idx, arr, n_out=100, parallel=False)
+    s_downsampled_p = downsampler.downsample(idx, arr, n_out=100, parallel=True)
+    assert np.all(s_downsampled == s_downsampled_p)
 
-all_downsamplers = rust_downsamplers + [EveryNthDownsampler()]
 
-
-def test_downsampling_with_x():
+@pytest.mark.parametrize("downsampler", generate_all_downsamplers())
+def test_downsampling_with_x(downsampler: AbstractDownsampler):
     """Test downsampling with x."""
     arr = np.random.randn(2_001).astype(np.float32)  # 2_001 to test edge case
     idx = np.arange(len(arr))
-    for downsampler in all_downsamplers:
-        s_downsampled = downsampler.downsample(arr, n_out=100)
-        s_downsampled_x = downsampler.downsample(idx, arr, n_out=100)
-        assert np.all(s_downsampled == s_downsampled_x)
-
-
-## Gaps in x
+    s_downsampled = downsampler.downsample(arr, n_out=100)
+    s_downsampled_x = downsampler.downsample(idx, arr, n_out=100)
+    assert np.all(s_downsampled == s_downsampled_x)
 
 
-def test_downsampling_with_gaps_in_x():
+@pytest.mark.parametrize("downsampler", generate_all_downsamplers())
+def test_downsampling_with_gaps_in_x(downsampler: AbstractDownsampler):
     """Test downsampling with gaps in x.
 
     With gap we do NOT mean a NaN in the array, but a large gap in the x values.
     """
     # TODO: might improve this test, now we just validate that the code does
     # not crash
     arr = np.random.randn(10_000).astype(np.float32)
     idx = np.arange(len(arr))
     idx[: len(idx) // 2] += len(idx) // 2  # add large gap in x
-    for downsampler in all_downsamplers:
-        s_downsampled = downsampler.downsample(idx, arr, n_out=100)
-        assert len(s_downsampled) <= 100
-        assert len(s_downsampled) >= 66
+    s_downsampled = downsampler.downsample(idx, arr, n_out=100)
+    assert len(s_downsampled) <= 100
+    assert len(s_downsampled) >= 66
 
 
-## Data types
+@pytest.mark.parametrize("downsampler", generate_rust_downsamplers())
+def test_downsampling_different_dtypes(downsampler: AbstractDownsampler):
+    """Test downsampling with different data types."""
+    arr_orig = np.random.randint(0, 100, size=10_000)
+    res = []
+    for dtype_y in supported_dtypes_y:
+        arr = arr_orig.astype(dtype_y)
+        s_downsampled = downsampler.downsample(arr, n_out=100)
+        if dtype_y is not np.bool_:
+            res += [s_downsampled]
+    for i in range(1, len(res)):
+        assert np.all(res[0] == res[i])
 
 
-def test_downsampling_different_dtypes():
-    """Test downsampling with different data types."""
+@pytest.mark.parametrize("downsampler", generate_rust_downsamplers())
+def test_downsampling_different_dtypes_with_x(downsampler: AbstractDownsampler):
+    """Test downsampling with x with different data types."""
     arr_orig = np.random.randint(0, 100, size=10_000)
-    for downsampler in rust_downsamplers:
+    idx_orig = np.arange(len(arr_orig))
+    for dtype_x in supported_dtypes_x:
         res = []
-        for dtype in supported_dtypes_y:
-            arr = arr_orig.astype(dtype)
-            s_downsampled = downsampler.downsample(arr, n_out=100)
-            if dtype is not np.bool_:
+        idx = idx_orig.astype(dtype_x)
+        for dtype_y in supported_dtypes_y:
+            arr = arr_orig.astype(dtype_y)
+            s_downsampled = downsampler.downsample(idx, arr, n_out=100)
+            if dtype_y is not np.bool_:
                 res += [s_downsampled]
         for i in range(1, len(res)):
             assert np.all(res[0] == res[i])
 
 
-def test_downsampling_different_dtypes_with_x():
-    """Test downsampling with different data types."""
-    arr_orig = np.random.randint(0, 100, size=10_000)
-    idx_orig = np.arange(len(arr_orig))
-    for downsampler in rust_downsamplers:
-        for dtype_x in supported_dtypes_x:
-            res = []
-            idx = idx_orig.astype(dtype_x)
-            for dtype_y in supported_dtypes_y:
-                arr = arr_orig.astype(dtype_y)
-                s_downsampled = downsampler.downsample(idx, arr, n_out=100)
-                if dtype_y is not np.bool_:
-                    res += [s_downsampled]
-            for i in range(1, len(res)):
-                assert np.all(res[0] == res[i])
-
-
-### Check no out of bounds indexing
+@pytest.mark.parametrize("downsampler", generate_rust_downsamplers())
+def test_downsampling_no_out_of_bounds_different_dtypes(
+    downsampler: AbstractDownsampler,
+):
+    """Test no out of bounds issues when downsampling with different data types."""
+    arr_orig = np.random.randint(0, 100, size=100)
+    res = []
+    for dtype in supported_dtypes_y:
+        arr = arr_orig.astype(dtype)
+        s_downsampled = downsampler.downsample(arr, n_out=76)
+        s_downsampled_p = downsampler.downsample(arr, n_out=76, parallel=True)
+        assert np.all(s_downsampled == s_downsampled_p)
+        if dtype is not np.bool_:
+            res += [s_downsampled]
+    for i in range(1, len(res)):
+        assert np.all(res[0] == res[i])
 
 
-def test_downsampling_no_out_of_bounds_different_dtypes():
+@pytest.mark.parametrize("downsampler", generate_rust_downsamplers())
+def test_downsampling_no_out_of_bounds_different_dtypes_with_x(
+    downsampler: AbstractDownsampler,
+):
     """Test no out of bounds issues when downsampling with different data types."""
     arr_orig = np.random.randint(0, 100, size=100)
-    for downsampler in rust_downsamplers:
+    idx_orig = np.arange(len(arr_orig))
+    for dtype_x in supported_dtypes_x:
         res = []
-        for dtype in supported_dtypes_y:
-            arr = arr_orig.astype(dtype)
-            s_downsampled = downsampler.downsample(arr, n_out=76)
-            s_downsampled_p = downsampler.downsample(arr, n_out=76, parallel=True)
+        idx = idx_orig.astype(dtype_x)
+        for dtype_y in supported_dtypes_y:
+            arr = arr_orig.astype(dtype_y)
+            s_downsampled = downsampler.downsample(idx, arr, n_out=76)
+            s_downsampled_p = downsampler.downsample(idx, arr, n_out=76, parallel=True)
             assert np.all(s_downsampled == s_downsampled_p)
-            if dtype is not np.bool_:
+            if dtype_y is not np.bool_:
                 res += [s_downsampled]
         for i in range(1, len(res)):
             assert np.all(res[0] == res[i])
 
 
-def test_downsampling_no_out_of_bounds_different_dtypes_with_x():
-    """Test no out of bounds issues when downsampling with different data types."""
-    arr_orig = np.random.randint(0, 100, size=100)
-    idx_orig = np.arange(len(arr_orig))
-    for downsampler in rust_downsamplers:
-        for dtype_x in supported_dtypes_x:
-            res = []
-            idx = idx_orig.astype(dtype_x)
-            for dtype_y in supported_dtypes_y:
-                arr = arr_orig.astype(dtype_y)
-                s_downsampled = downsampler.downsample(idx, arr, n_out=76)
-                s_downsampled_p = downsampler.downsample(
-                    idx, arr, n_out=76, parallel=True
-                )
-                assert np.all(s_downsampled == s_downsampled_p)
-                if dtype_y is not np.bool_:
-                    res += [s_downsampled]
-            for i in range(1, len(res)):
-                assert np.all(res[0] == res[i])
-
-
-### Check no overflow when calculating average
-
-
 def test_lttb_no_overflow():
     """Test no overflow when calculating average."""
     ### THIS SHOULD NOT OVERFLOW & HAVE THE SAME RESULT
     arr_orig = np.array([2 * 10**5] * 10_000, dtype=np.float64)
     s_downsampled = LTTBDownsampler().downsample(arr_orig, n_out=100)
     arr = arr_orig.astype(np.float32)
     s_downsampled_f32 = LTTBDownsampler().downsample(arr, n_out=100)
@@ -213,33 +205,27 @@
     # really account for this, I guess it is perhaps less of an issue than I
     # thought. In the end f32 MAX is 3.4028235 × 1038 & f64 MAX is
     # 1.7976931348623157 × 10308 => which is in the end quite a lot.. (and all
     # integer averages are handled using f64) - f32 is only used for f16 & f32
     # (just as in numpy).
 
 
-### Invalid n_out
-
-
 def test_invalid_nout():
     """Test invalid n_out."""
     arr = np.random.randint(0, 100, size=10_000)
     with pytest.raises(ValueError):
         LTTBDownsampler().downsample(arr, n_out=-1)
     with pytest.raises(ValueError):
         # Should be even
         MinMaxDownsampler().downsample(arr, n_out=33)
     with pytest.raises(ValueError):
         # Should be multiple of 4
         M4Downsampler().downsample(arr, n_out=34)
 
 
-### Unsupported dtype
-
-
 def test_error_unsupported_dtype():
     """Test unsupported dtype."""
     arr = np.random.randint(0, 100, size=10_000)
     arr = arr.astype("object")
     with pytest.raises(ValueError):
         MinMaxDownsampler().downsample(arr, n_out=100)
```

### Comparing `tsdownsample-0.1.1/tsdownsample/downsamplers.py` & `tsdownsample-0.1.2a0/tsdownsample/downsamplers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import math
 import warnings
 from typing import Union
 
 import numpy as np
 
 # ------------------ Rust Downsamplers ------------------
 from tsdownsample._rust import _tsdownsample_rs  # type: ignore[attr-defined]
@@ -59,9 +58,9 @@
     ) -> np.ndarray:
         if x is not None:
             name = self.__class__.__name__
             warnings.warn(
                 f"x is passed to downsample method of {name}, but is not taken "
                 "into account by the current implementation of the EveryNth algorithm."
             )
-        step = max(1, math.ceil(len(y) / n_out))
-        return np.arange(0, len(y), step)
+        step = max(1, len(y) / n_out)
+        return np.arange(start=0, stop=len(y), step=step).astype(np.uint)
```

### Comparing `tsdownsample-0.1.1/tsdownsample/downsampling_interface.py` & `tsdownsample-0.1.2a0/tsdownsample/downsampling_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """AbstractDownsampler interface-class, subclassed by concrete downsamplers."""
 
 __author__ = "Jeroen Van Der Donckt"
 
 import re
 import warnings
 from abc import ABC, abstractmethod
+from copy import deepcopy
 from types import ModuleType
 from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 
 
 class AbstractDownsampler(ABC):
@@ -46,14 +47,20 @@
         elif len(args) == 1:
             x, y = None, args[0]
         else:
             raise ValueError(
                 "downsample() takes 1 or 2 positional arguments but "
                 f"{len(args)} were given"
             )
+
+        if x is not None and not isinstance(x, np.ndarray):
+            x = np.array(x)
+        if not isinstance(y, np.ndarray):
+            y = np.array(y)
+
         # y must be 1D array
         if y.ndim != 1:
             raise ValueError("y must be 1D array")
         # x must be 1D array with same length as y or None
         if x is not None:
             if x.ndim != 1:
                 raise ValueError("x must be 1D array")
@@ -316,7 +323,20 @@
         *args,  # x and y are optional
         n_out: int,
         parallel: bool = False,
         **kwargs,
     ):
         """Downsample the data in x and y."""
         return super().downsample(*args, n_out=n_out, parallel=parallel, **kwargs)
+
+    def __deepcopy__(self, memo):
+        """Deepcopy the object."""
+        cls = self.__class__
+        result = cls.__new__(cls)
+        memo[id(self)] = result
+        for k, v in self.__dict__.items():
+            if k.endswith("_mod") or k.startswith("mod_"):
+                # Don't (deep)copy the compiled modules
+                setattr(result, k, v)
+            else:
+                setattr(result, k, deepcopy(v, memo))
+        return result
```

### Comparing `tsdownsample-0.1.1/Cargo.lock` & `tsdownsample-0.1.2a0/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -29,51 +29,51 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.13"
+version = "0.9.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01a9af1f4c2ef74bb8aa1f7e19706bc72d03598c8a570bb5de72243c7a9d9d5a"
+checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.7.1",
+ "memoffset",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.14"
+version = "0.8.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
+checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
@@ -120,17 +120,17 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
@@ -151,23 +151,14 @@
 checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
 dependencies = [
  "rawpointer",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
@@ -238,146 +229,146 @@
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.6"
+version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba1ef8814b5c993410bb3adfad7a5ed269563e4a2f90c41f5d85be7fb47133bf"
+checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.11"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d01a5bd0424d00070b0098dd17ebca6f961a959dead1dbcbbbc1d1cd8d3deeba"
+checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.50"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ef7d57beacfaf2d8aee5937dab7b7f28de3cb8b1828479bb5de2a7106f2bae2"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.0"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccd4149c8c3975099622b4e1962dac27565cf5663b76452c3e2b66e0b6824277"
+checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.8.0",
+ "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.0"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cd09fe469834db21ee60e0051030339e5d361293d8cb5ec02facf7fdcf52dbf"
+checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.0"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c427c9a96b9c5b12156dbc11f76b14f49e9aae8905ca783ea87c249044ef137"
+checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.0"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b822bbba9d60630a44d2109bc410489bb2f439b33e3a14ddeb8a40b378a7c4"
+checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.0"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84ae898104f7c99db06231160770f3e40dad6eb9021daddc0fedfa3e41dff10a"
+checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.2"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "356a0625f1954f730c0201cdab48611198dc6ce21f4acff55089b5a78e6e835b"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
@@ -406,101 +397,110 @@
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
 name = "tsdownsample"
 version = "0.1.0"
 dependencies = [
  "downsample_rs",
  "half",
  "numpy",
  "paste",
  "pyo3",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.45.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c9864e83243fdec7fc9c5444389dcbbfd258f745e7853198f365e3c4968a608"
+checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8b1b673ffc16c47a9ff48570a9d85e25d265735c503681332589af6253c6c7"
+checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3887528ad530ba7bdbb1faa8275ec7a1155a45ffa57c37993960277145d640"
+checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf4d1122317eddd6ff351aa852118a2418ad4214e6613a50e0191f7004372605"
+checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1040f221285e17ebccbc2591ffdc2d44ee1f9186324dd3e84e99ac68d699c45"
+checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "628bfdf232daa22b0d64fdb62b09fcc36bb01f05a3939e20ab73aaf9470d0463"
+checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.1"
+version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
+checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
```

### Comparing `tsdownsample-0.1.1/PKG-INFO` & `tsdownsample-0.1.2a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tsdownsample
-Version: 0.1.1
+Version: 0.1.2a0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: numpy
 License-File: LICENSE
-Summary: Extremely fast time series downsampling in Rust
+Summary: Time series downsampling in rust
 Keywords: time series,downsampling,rust,data science,visualization
 Author: Jeroen Van Der Donckt
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/predict-idlab/tsdownsample
 Project-URL: Repository, https://github.com/predict-idlab/tsdownsample
@@ -32,15 +32,15 @@
 [![Testing](https://github.com/predict-idlab/tsdownsample/actions/workflows/ci-tsdownsample.yml/badge.svg)](https://github.com/predict-idlab/tsdownsample/actions/workflows/ci-tsdownsample.yml)
 <!-- TODO: codecov -->
 
 Extremely fast **time series downsampling 📈** for visualization, written in Rust.
 
 ## Features ✨
 
-* **Fast**: written in rust with PyO3 bindings  
+* **Fast**: written in rust with PyO3 bindings
   - leverages optimized [argminmax](https://github.com/jvdd/argminmax) - which is SIMD accelerated with runtime feature detection
   - scales linearly with the number of data points
   <!-- TODO check if it scales sublinearly -->
   - multithreaded with Rayon (in Rust)
     <details>
       <summary><i>Why we do not use Python multiprocessing</i></summary>
       Citing the <a href="https://pyo3.rs/v0.17.3/parallelism.html">PyO3 docs on parallelism</a>:<br>
@@ -80,23 +80,30 @@
 # Create a time series
 y = np.random.randn(10_000_000)
 x = np.arange(len(y))
 
 # Downsample to 1000 points (assuming constant sampling rate)
 s_ds = MinMaxLTTBDownsampler().downsample(y, n_out=1000)
 
+# Select downsampled data
+downsampled_y = y[s_ds]
+
 # Downsample to 1000 points using the (possible irregularly spaced) x-data
 s_ds = MinMaxLTTBDownsampler().downsample(x, y, n_out=1000)
+
+# Select downsampled data
+downsampled_x = x[s_ds]
+downsampled_y = y[s_ds]
 ```
 
-## Downsampling algorithms & API 
+## Downsampling algorithms & API
 
 ### Downsampling API 📑
 
-Each downsampling algorithm is implemented as a class that implements a `downsample` method.  
+Each downsampling algorithm is implemented as a class that implements a `downsample` method.
 The signature of the `downsample` method:
 
 ```
 downsample([x], y, n_out, **kwargs) -> ndarray[uint64]
 ```
 
 **Arguments**:
@@ -105,15 +112,15 @@
 - `n_out` is a mandatory keyword argument that defines the number of output values<sup>*</sup>
 - `**kwargs` are optional keyword arguments *(see [table below](#downsampling-algorithms-📈))*:
   - `parallel`: whether to use multi-threading (default: `False`)<sup>**</sup>
   - ...
 
 **Returns**: a `ndarray[uint64]` of indices that can be used to index the original data.
 
-<sup>*</sup><i>When there are gaps in the time series, fewer than `n_out` indices may be returned.</i>  
+<sup>*</sup><i>When there are gaps in the time series, fewer than `n_out` indices may be returned.</i>
 <sup>**</sup><i>`parallel` is not supported for `LTTBDownsampler`.</i>
 ### Downsampling algorithms 📈
 
 The following downsampling algorithms (classes) are implemented:
 
 | Downsampler | Description | `**kwargs` |
 | ---:| --- |--- |
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1 Name: tsdownsample Version: 0.1.1 Classifier: Intended
+Metadata-Version: 2.1 Name: tsdownsample Version: 0.1.2a0 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: POSIX Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Requires-Dist:
-numpy License-File: LICENSE Summary: Extremely fast time series downsampling in
-Rust Keywords: time series,downsampling,rust,data science,visualization Author:
-Jeroen Van Der Donckt License: MIT Requires-Python: >=3.7 Description-Content-
-Type: text/markdown; charset=UTF-8; variant=GFM Project-URL: Homepage, https://
-github.com/predict-idlab/tsdownsample Project-URL: Repository, https://
-github.com/predict-idlab/tsdownsample # tsdownsample [![PyPI Latest Release]
-(https://img.shields.io/pypi/v/tsdownsample.svg)](https://pypi.org/project/
-tsdownsample/) [![support-version](https://img.shields.io/pypi/pyversions/
-tsdownsample)](https://img.shields.io/pypi/pyversions/tsdownsample) [!
-[Downloads](https://pepy.tech/badge/tsdownsample)](https://pepy.tech/project/
-tsdownsample) [![Testing](https://github.com/predict-idlab/tsdownsample/
-actions/workflows/ci-downsample_rs.yml/badge.svg)](https://github.com/predict-
-idlab/tsdownsample/actions/workflows/ci-downsample_rs.yml) [![Testing](https://
-github.com/predict-idlab/tsdownsample/actions/workflows/ci-tsdownsample.yml/
-badge.svg)](https://github.com/predict-idlab/tsdownsample/actions/workflows/ci-
-tsdownsample.yml)  Extremely fast **time series downsampling ð** for
-visualization, written in Rust. ## Features â¨ * **Fast**: written in rust
-with PyO3 bindings - leverages optimized [argminmax](https://github.com/jvdd/
-argminmax) - which is SIMD accelerated with runtime feature detection - scales
-linearly with the number of data points  - multithreaded with Rayon (in Rust)
-Why we do not use Python multiprocessing Citing the PyO3_docs_on_parallelism:
+numpy License-File: LICENSE Summary: Time series downsampling in rust Keywords:
+time series,downsampling,rust,data science,visualization Author: Jeroen Van Der
+Donckt License: MIT Requires-Python: >=3.7 Description-Content-Type: text/
+markdown; charset=UTF-8; variant=GFM Project-URL: Homepage, https://github.com/
+predict-idlab/tsdownsample Project-URL: Repository, https://github.com/predict-
+idlab/tsdownsample # tsdownsample [![PyPI Latest Release](https://
+img.shields.io/pypi/v/tsdownsample.svg)](https://pypi.org/project/tsdownsample/
+) [![support-version](https://img.shields.io/pypi/pyversions/tsdownsample)]
+(https://img.shields.io/pypi/pyversions/tsdownsample) [![Downloads](https://
+pepy.tech/badge/tsdownsample)](https://pepy.tech/project/tsdownsample) [!
+[Testing](https://github.com/predict-idlab/tsdownsample/actions/workflows/ci-
+downsample_rs.yml/badge.svg)](https://github.com/predict-idlab/tsdownsample/
+actions/workflows/ci-downsample_rs.yml) [![Testing](https://github.com/predict-
+idlab/tsdownsample/actions/workflows/ci-tsdownsample.yml/badge.svg)](https://
+github.com/predict-idlab/tsdownsample/actions/workflows/ci-tsdownsample.yml)
+Extremely fast **time series downsampling ð** for visualization, written in
+Rust. ## Features â¨ * **Fast**: written in rust with PyO3 bindings -
+leverages optimized [argminmax](https://github.com/jvdd/argminmax) - which is
+SIMD accelerated with runtime feature detection - scales linearly with the
+number of data points  - multithreaded with Rayon (in Rust)  Why we do not use
+Python multiprocessing Citing the PyO3_docs_on_parallelism:
      CPython has the infamous Global Interpreter Lock, which prevents
      several threads from executing Python bytecode in parallel. This
      makes threading in Python a bad fit for CPU-bound tasks and often
      forces developers to accept the overhead of multiprocessing.
 In Rust - which is a compiled language - there is no GIL, so CPU-bound tasks
 can be parallelized (with Rayon) with little to no overhead.  * **Efficient**:
 memory efficient - works on views of the data (no copies) - no intermediate
@@ -48,33 +48,34 @@
 sufficient. This mapping allows to use the hardware supported scalar and SIMD
 i16 instructions - while not producing any memory overhead ð
 More details are described in argminmax_PR_#1.  * **Easy to use**: simple &
 flexible API ## Install ```bash pip install tsdownsample ``` ## Usage ```python
 from tsdownsample import MinMaxLTTBDownsampler import numpy as np # Create a
 time series y = np.random.randn(10_000_000) x = np.arange(len(y)) # Downsample
 to 1000 points (assuming constant sampling rate) s_ds = MinMaxLTTBDownsampler
-().downsample(y, n_out=1000) # Downsample to 1000 points using the (possible
-irregularly spaced) x-data s_ds = MinMaxLTTBDownsampler().downsample(x, y,
-n_out=1000) ``` ## Downsampling algorithms & API ### Downsampling API ð Each
-downsampling algorithm is implemented as a class that implements a `downsample`
-method. The signature of the `downsample` method: ``` downsample([x], y, n_out,
-**kwargs) -> ndarray[uint64] ``` **Arguments**: - `x` is optional - `x` and `y`
-are both positional arguments - `n_out` is a mandatory keyword argument that
-defines the number of output values* - `**kwargs` are optional keyword
-arguments *(see [table below](#downsampling-algorithms-ð))*: - `parallel`:
-whether to use multi-threading (default: `False`)** - ... **Returns**: a
-`ndarray[uint64]` of indices that can be used to index the original data. *When
-there are gaps in the time series, fewer than `n_out` indices may be returned.
-**`parallel` is not supported for `LTTBDownsampler`. ### Downsampling
-algorithms ð The following downsampling algorithms (classes) are
-implemented: | Downsampler | Description | `**kwargs` | | ---:| --- |--- | |
-`MinMaxDownsampler` | selects the **min and max** value in each bin |
-`parallel` | | `M4Downsampler` | selects the [**min, max, first and last**]
-(https://dl.acm.org/doi/pdf/10.14778/2732951.2732953) value in each bin |
-`parallel` | | `LTTBDownsampler` | performs the [**Largest Triangle Three
+().downsample(y, n_out=1000) # Select downsampled data downsampled_y = y[s_ds]
+# Downsample to 1000 points using the (possible irregularly spaced) x-data s_ds
+= MinMaxLTTBDownsampler().downsample(x, y, n_out=1000) # Select downsampled
+data downsampled_x = x[s_ds] downsampled_y = y[s_ds] ``` ## Downsampling
+algorithms & API ### Downsampling API ð Each downsampling algorithm is
+implemented as a class that implements a `downsample` method. The signature of
+the `downsample` method: ``` downsample([x], y, n_out, **kwargs) -> ndarray
+[uint64] ``` **Arguments**: - `x` is optional - `x` and `y` are both positional
+arguments - `n_out` is a mandatory keyword argument that defines the number of
+output values* - `**kwargs` are optional keyword arguments *(see [table below]
+(#downsampling-algorithms-ð))*: - `parallel`: whether to use multi-threading
+(default: `False`)** - ... **Returns**: a `ndarray[uint64]` of indices that can
+be used to index the original data. *When there are gaps in the time series,
+fewer than `n_out` indices may be returned. **`parallel` is not supported for
+`LTTBDownsampler`. ### Downsampling algorithms ð The following downsampling
+algorithms (classes) are implemented: | Downsampler | Description | `**kwargs`
+| | ---:| --- |--- | | `MinMaxDownsampler` | selects the **min and max** value
+in each bin | `parallel` | | `M4Downsampler` | selects the [**min, max, first
+and last**](https://dl.acm.org/doi/pdf/10.14778/2732951.2732953) value in each
+bin | `parallel` | | `LTTBDownsampler` | performs the [**Largest Triangle Three
 Buckets**](https://skemman.is/bitstream/1946/15343/3/SS_MSthesis.pdf) algorithm
 | | `MinMaxLTTBDownsampler` | (*new two-step algorithm ð*) first selects
 `n_out` * `minmax_ratio` **min and max** values, then further reduces these to
 `n_out` values using the **Largest Triangle Three Buckets** algorithm |
 `parallel`, `minmax_ratio`* | *Default value for `minmax_ratio` is 30, which is
 empirically proven to be a good default. (More details in our upcomming paper)
 ## Limitations & assumptions ð¨ Assumes; 1. `x`-data is (non-strictly)
```

