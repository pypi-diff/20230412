# Comparing `tmp/opendal-0.30.5.tar.gz` & `tmp/opendal-0.31.0.tar.gz`

## Comparing `opendal-0.30.5.tar` & `opendal-0.31.0.tar`

### file list

```diff
@@ -1,231 +1,240 @@
--rw-r--r--   0        0        0     4706 1970-01-01 00:00:00.000000 opendal-0.30.5/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    56648 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1256 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6663 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5574 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2438 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1832 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/examples/object.rs
--rw-r--r--   0     1001      123     1296 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7703 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     5243 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123      926 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10782 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1768 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     4392 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    21099 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6746 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    17164 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123     9976 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    16097 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    13631 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    47056 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    32192 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123     1618 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    33280 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    11782 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3844 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3113 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    18337 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5164 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123     9055 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1181 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1548 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     7722 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     9526 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     7636 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/dns.rs
--rw-r--r--   0     1001      123     3096 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    10388 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     1974 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123     2962 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    10783 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     1978 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     4439 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15332 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4148 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     4577 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     1971 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3509 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10680 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     8918 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6861 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5443 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     3626 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    11671 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     7008 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123    34618 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123    10124 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123     5738 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      903 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14654 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2267 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    22213 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123     3437 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      890 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     6138 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     3055 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     3625 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      859 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123    22973 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123     1424 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      884 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3569 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    16014 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123     1808 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2545 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4206 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     2041 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    21125 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123     3380 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      895 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10372 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     2248 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123    20607 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2528 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    17823 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     1497 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3357 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     3081 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    13268 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1743 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    16828 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123     1871 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     8898 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123     2790 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     1975 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     1074 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
--rw-r--r--   0     1001      123     4713 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123     9954 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     3889 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      857 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     2458 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     7949 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123    16823 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     3360 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      886 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6154 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2245 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123    29369 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123     3275 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      886 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7597 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     2307 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123    10492 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      855 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     5615 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123      859 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    65304 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     3395 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123     3602 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      884 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7735 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     4468 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123     5166 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      854 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123    17571 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      616 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      521 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16943 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2532 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2207 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    23321 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     4085 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     5389 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     1812 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2219 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     2333 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     2494 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    10440 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     6197 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    15178 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1462 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    20094 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123     8731 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     2873 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1098 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    33943 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123     8668 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/ops.rs
--rw-r--r--   0     1001      123     9603 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     6901 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123     7267 2023-03-31 02:13:49.000000 opendal-0.30.5/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1408 1970-01-01 00:00:00.000000 opendal-0.30.5/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-03-31 02:13:49.000000 opendal-0.30.5/.gitignore
--rw-r--r--   0     1001      123      917 2023-03-31 02:13:49.000000 opendal-0.30.5/README.md
--rw-r--r--   0     1001      123     1529 2023-03-31 02:13:49.000000 opendal-0.30.5/pyproject.toml
--rw-r--r--   0     1001      123      867 2023-03-31 02:13:49.000000 opendal-0.30.5/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2918 2023-03-31 02:13:49.000000 opendal-0.30.5/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123    11921 2023-03-31 02:13:49.000000 opendal-0.30.5/src/asyncio.rs
--rw-r--r--   0     1001      123     3311 2023-03-31 02:13:49.000000 opendal-0.30.5/src/layers.rs
--rw-r--r--   0     1001      123    13929 2023-03-31 02:13:49.000000 opendal-0.30.5/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-03-31 02:13:49.000000 opendal-0.30.5/tests/binding.feature
--rw-r--r--   0     1001      123     2930 2023-03-31 02:13:49.000000 opendal-0.30.5/tests/steps/binding.py
--rw-r--r--   0     1001      123   110776 2023-03-31 02:13:49.000000 opendal-0.30.5/Cargo.lock
--rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 opendal-0.30.5/PKG-INFO
+-rw-r--r--   0        0        0     5090 1970-01-01 00:00:00.000000 opendal-0.31.0/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    60180 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1256 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6663 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5574 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2438 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1832 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/examples/object.rs
+-rw-r--r--   0     1001      123     1296 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7703 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     5243 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123      926 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10794 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     4392 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    22397 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6746 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    17164 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123     9976 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    16050 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    13631 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    52162 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    32204 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123     1618 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    37153 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    11794 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3844 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3113 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    21079 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5164 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123     9055 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1181 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1548 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     6441 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5404 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3394 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    10427 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2025 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11951 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     2020 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     4439 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3666 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15332 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4148 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     4577 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     1971 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3509 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10680 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     8918 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6861 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5443 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     4049 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    11671 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6387 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123    27076 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123    10124 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123     9145 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     5738 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      913 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2183 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    15592 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123     7931 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     3437 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2877 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123     3625 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123    25021 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123     1424 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      884 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3569 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    15973 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123     1808 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4206 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     2041 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    16136 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123     7533 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3380 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10014 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     2186 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123    20553 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2516 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    17767 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     1497 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     3081 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    13256 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    16810 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123     1871 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     8862 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123     2790 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     1975 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     1074 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt
+-rw-r--r--   0     1001      123     4713 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123     9954 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     3889 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      857 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     3350 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     7949 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123    13309 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     6561 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3360 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2161 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    18570 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    20500 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     3275 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      896 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     4044 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123    10492 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      855 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     5615 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123      859 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    39368 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     3395 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    27213 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     3602 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7040 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     4227 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123     5093 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      854 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123    20468 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      531 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123    16965 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/list_response.rs
+-rw-r--r--   0     1001      123      911 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123     2532 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2207 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    23279 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     4085 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     5211 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     1812 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2213 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     2333 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     2494 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    10546 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     6197 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    15166 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1462 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    23847 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123     8731 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3235 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1098 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    37805 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123     9437 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/ops.rs
+-rw-r--r--   0     1001      123     9603 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     5698 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123     7267 2023-04-12 03:51:19.000000 opendal-0.31.0/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.31.0/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-04-12 03:51:19.000000 opendal-0.31.0/.gitignore
+-rw-r--r--   0     1001      123      917 2023-04-12 03:51:19.000000 opendal-0.31.0/README.md
+-rw-r--r--   0     1001      123      765 2023-04-12 03:51:19.000000 opendal-0.31.0/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-04-12 03:51:19.000000 opendal-0.31.0/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-04-12 03:51:19.000000 opendal-0.31.0/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123     1638 2023-04-12 03:51:19.000000 opendal-0.31.0/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-04-12 03:51:19.000000 opendal-0.31.0/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-04-12 03:51:19.000000 opendal-0.31.0/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123    11963 2023-04-12 03:51:19.000000 opendal-0.31.0/src/asyncio.rs
+-rw-r--r--   0     1001      123     3311 2023-04-12 03:51:19.000000 opendal-0.31.0/src/layers.rs
+-rw-r--r--   0     1001      123    13929 2023-04-12 03:51:19.000000 opendal-0.31.0/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-04-12 03:51:19.000000 opendal-0.31.0/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-04-12 03:51:19.000000 opendal-0.31.0/tests/steps/binding.py
+-rw-r--r--   0     1001      123   110910 2023-04-12 03:51:19.000000 opendal-0.31.0/Cargo.lock
+-rw-r--r--   0        0        0     2051 1970-01-01 00:00:00.000000 opendal-0.31.0/PKG-INFO
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/Cargo.toml` & `opendal-0.31.0/local_dependencies/opendal/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -12,93 +12,139 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [package]
-authors = ["OpenDAL Contributors <dev@opendal.apache.org>"]
 categories = ["filesystem"]
 description = "OpenDAL: Access data freely, painlessly, and efficiently."
-edition = "2021"
 exclude = ["tests/"]
-homepage = "https://opendal.apache.org/"
 keywords = ["storage", "fs", "s3", "azblob", "gcs"]
-license = "Apache-2.0"
 name = "opendal"
-repository = "https://github.com/apache/incubator-opendal"
-rust-version = "1.60"                                                     # MSRV for this project - please update while bump versions
-version = "0.30.5"
+
+authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
+edition= "2021"
+homepage= "https://opendal.apache.org/"
+license= "Apache-2.0"
+repository= "https://github.com/apache/incubator-opendal"
+rust-version= "1.64"
+version= "0.31.0"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
-default = ["rustls"]
+default = [
+  "rustls",
+  "services-azblob",
+  "services-azdfs",
+  "services-fs",
+  "services-gcs",
+  "services-ghac",
+  "services-http",
+  "services-ipmfs",
+  "services-memory",
+  "services-obs",
+  "services-oss",
+  "services-s3",
+  "services-sled",
+  "services-webdav",
+  "services-webhdfs",
+]
 
 # Build docs or not.
 #
 # This features is used to control whether or not to build opendal's docs.
 # And doesn't have any other effects.
 docs = []
 
 # Enable trust-dns for pure rust dns cache.
-trust-dns = ["reqwest/trust-dns", "dep:trust-dns-resolver"]
+trust-dns = ["reqwest/trust-dns"]
 
 # Enable rustls for TLS support
-rustls = ["reqwest/rustls-tls-native-roots", "ureq/tls", "ureq/native-certs"]
+rustls = ["reqwest/rustls-tls-native-roots"]
 # Enable native-tls for TLS support
-native-tls = ["reqwest/native-tls", "ureq/native-tls"]
+native-tls = ["reqwest/native-tls"]
 # Enable vendored native-tls for TLS support
-native-tls-vendored = ["reqwest/native-tls-vendored", "ureq/native-tls"]
+native-tls-vendored = ["reqwest/native-tls-vendored"]
 
 # Enable all layers.
 layers-all = ["layers-chaos", "layers-metrics", "layers-tracing"]
 # Enable layers chaos support
 layers-chaos = ["dep:rand"]
 # Enable layers metrics support
 layers-metrics = ["dep:metrics"]
 # Enable layers tracing support.
 layers-tracing = ["dep:tracing"]
 
-# Enable services dashmap support
+services-azblob = [
+  "dep:reqsign",
+  "reqsign?/services-azblob",
+  "reqsign?/reqwest_request",
+]
+services-azdfs = [
+  "dep:reqsign",
+  "reqsign?/services-azblob",
+  "reqsign?/reqwest_request",
+]
 services-dashmap = ["dep:dashmap"]
-# Enable services ftp support
+services-fs = ["tokio/fs"]
 services-ftp = ["dep:suppaftp", "dep:lazy-regex", "dep:bb8", "dep:async-tls"]
-# Enable services hdfs support
+services-gcs = [
+  "dep:reqsign",
+  "reqsign?/services-google",
+  "reqsign?/reqwest_request",
+]
+services-ghac = []
 services-hdfs = ["dep:hdrs"]
-# Enable services ipfs support
+services-http = []
 services-ipfs = ["dep:prost"]
-# Enable services memcached support
+services-ipmfs = []
 services-memcached = ["dep:bb8"]
-# Enable services moka support
+services-memory = []
 services-moka = ["dep:moka"]
-# Enable services redis support
+services-obs = [
+  "dep:reqsign",
+  "reqsign?/services-huaweicloud",
+  "reqsign?/reqwest_request",
+]
+services-oss = [
+  "dep:reqsign",
+  "reqsign?/services-aliyun",
+  "reqsign?/reqwest_request",
+]
 services-redis = ["dep:redis"]
-# Enable services rocksdb support
 services-rocksdb = ["dep:rocksdb"]
-# Enable services sled support
+services-s3 = [
+  "dep:reqsign",
+  "reqsign?/services-aws",
+  "reqsign?/reqwest_request",
+]
 services-sled = ["dep:sled"]
+services-webdav = []
+services-webhdfs = []
 
 [lib]
 bench = false
 
 [[bench]]
 harness = false
 name = "ops"
 
 [dependencies]
 anyhow = { version = "1.0.30", features = ["std"] }
 async-compat = "0.2"
 async-tls = { version = "0.11", optional = true }
-async-trait = "0.1.66"
+async-trait = "0.1.68"
 backon = "0.4.0"
 base64 = "0.21"
 bb8 = { version = "0.8", optional = true }
 bytes = "1.2"
+chrono = "0.4.24"
 dashmap = { version = "5.4", optional = true }
 flagset = "0.4"
 futures = { version = "0.3", features = ["alloc"] }
 hdrs = { version = "0.2", optional = true, features = ["async_file"] }
 http = "0.2.5"
 hyper = "0.14"
 lazy-regex = { version = "2.5.0", optional = true }
@@ -113,26 +159,23 @@
 prost = { version = "0.11", optional = true }
 quick-xml = { version = "0.27", features = ["serialize", "overlapped-lists"] }
 rand = { version = "0.8", optional = true }
 redis = { version = "0.22", features = [
   "tokio-comp",
   "connection-manager",
 ], optional = true }
-reqsign = "0.8.5"
+reqsign = { version = "0.9.1", default-features = false, optional = true }
 reqwest = { version = "0.11.13", features = [
   "multipart",
   "stream",
 ], default-features = false }
 rocksdb = { version = "0.20.1", default-features = false, optional = true }
 serde = { version = "1", features = ["derive"] }
 serde_json = "1"
 sled = { version = "0.34.7", optional = true }
 suppaftp = { version = "4.5", default-features = false, features = [
   "async-secure",
   "async-rustls",
 ], optional = true }
-time = { version = "0.3", features = ["serde"] }
-tokio = { version = "1.26", features = ["fs"] }
+tokio = "1.27"
 tracing = { version = "0.1", optional = true }
-trust-dns-resolver = { version = "0.22", optional = true }
-ureq = { version = "2", default-features = false }
 uuid = { version = "1", features = ["serde", "v4"] }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.31.0/local_dependencies/opendal/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,96 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.31.0] - 2023-04-12
+
+### Added
+
+- feat(bindings/java): add cucumber test (#1809)
+- feat(bindings/java): setup Java CI (#1823)
+- feat: add if_none_match support (#1832)
+- feat: Retry when some of batch operations are failing (#1840)
+- feat: add writer support for aliyun oss (#1842)
+- feat(core): Add Copy Support (#1841)
+- feat(bindings/c): fix c bindings makefile (#1849)
+- feat(core): add behavior tests for copy & blocking_copy (#1852)
+- feat(s3): allow users to specify storage_class (#1854)
+- feat(s3): Support copy (#1856)
+- Add check for s3 bucket name (#1857)
+- feat(core): Support rename (#1862)
+- feat(bindings/nodejs): add `copy` and `rename` (#1866)
+- feat(azblob): Support copy (#1868)
+- feat(gcs): copy support for GCS (#1869)
+- feat(bindings/c): framework of add basic io and init logics (#1861)
+- feat(webdav): support copy (#1870)
+- feat(services/oss): Add Copy Support (#1874)
+- feat(services/obs): Add Copy Support (#1876)
+- feat(services/webdav): Support Rename (#1878)
+- binding/c: parse opendal to use typed BlockingOperator (#1881)
+- binding/c: clean up comments and type assertion for BlockingOperator (#1883)
+- binding(python): Support python binding benchmark for opendal (#1882)
+- feat(bindings/c): add support for free heap-allocated operator (#1890)
+- feat(binding/c): add is_exist to operator (#1892)
+- feat(bindings/java): add Stat support (#1894)
+- feat(services/gcs): Add customed token loader support (#1908)
+- feat(services/oss): remove unused builder prop allow_anonymous (#1913)
+- feat: Add feature flag for all services (#1915)
+
+### Changed
+
+- refactor(core): Simplify the usage of BatchOperation and BatchResults (#1843)
+- refactor: Use reqwest blocking client instead of ureq (#1853)
+- refactor: Bump MSRV to 1.64 (#1864)
+- refactor: Remove not used blocking http client (#1895)
+- refactor: Change presign to async for future refactor (#1900)
+- refactor(services/gcs): Migrate to async reqsign (#1906)
+- refactor(services/azdfs): Migrate to async reqsign (#1903)
+- refactor(services/azblob): Adopt new reqsign  (#1902)
+- refactor(services/s3): Migrate to async reqsign (#1909)
+- refactor(services/oss): Migrate to async reqsign (#1911)
+- refactor: Use chrono instead of time to work well with ecosystem (#1912)
+- refactor(service/obs): Migrate obs to async reqsign (#1914)
+
+### Fixed
+
+- fix: podling website check (#1838)
+- fix(website): copyright update (#1839)
+- fix(core): Add checks before doing copy (#1845)
+- fix(core): S3 Copy should set SSE headers (#1860)
+- fix: Fix presign related unit tests (#1910)
+
+### Docs
+
+- docs(bindings/nodejs): fix build failed (#1819)
+- docs: fix several typos in the documentation (#1846)
+- doc(bindings/nodejs): update presign example in doc (#1901)
+
+### CI
+
+- ci: Fix build for nodejs binding on macos (#1813)
+- binding/c: build: add phony to makefile, and some improve (#1850)
+- ci: upgrade hawkeye action (#1834)
+
+### Chore
+
+- chore(bindings/nodejs): add deno benchmark (#1814)
+- chore: Add CODEOWNERS (#1817)
+- chore(deps): bump opentelemetry-jaeger from 0.16.0 to 0.18.0 (#1829)
+- chore(deps): bump opentelemetry from 0.17.0 to 0.19.0 (#1830)
+- chore(deps): bump tokio from 1.26.0 to 1.27.0 (#1828)
+- chore(deps): bump napi-derive from 2.12.1 to 2.12.2 (#1827)
+- chore(deps): bump async-trait from 0.1.67 to 0.1.68 (#1826)
+- chore: Cleanup code for oss writer (#1847)
+- chore: Make clippy happy (#1865)
+- binding(python): Format python code in binding (#1885)
+
 ## [v0.30.5] - 2023-03-31
 
 ### Added
 
 - feat(oli): implement `oli rm` (#1774)
 - feat(bindings/nodejs): Support presign (#1772)
 - feat(oli): implement `oli stat` (#1778)
@@ -1754,14 +1836,15 @@
 
 ## v0.0.1 - 2022-02-14
 
 ### Added
 
 Hello, OpenDAL!
 
+[v0.31.0]: https://github.com/apache/incubator-opendal/compare/v0.30.5...v0.31.0
 [v0.30.5]: https://github.com/apache/incubator-opendal/compare/v0.30.4...v0.30.5
 [v0.30.4]: https://github.com/apache/incubator-opendal/compare/v0.30.3...v0.30.4
 [v0.30.3]: https://github.com/apache/incubator-opendal/compare/v0.30.2...v0.30.3
 [v0.30.2]: https://github.com/apache/incubator-opendal/compare/v0.30.1...v0.30.2
 [v0.30.1]: https://github.com/apache/incubator-opendal/compare/v0.30.0...v0.30.1
 [v0.30.0]: https://github.com/apache/incubator-opendal/compare/v0.29.1...v0.30.0
 [v0.29.1]: https://github.com/apache/incubator-opendal/compare/v0.29.0...v0.29.1
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.31.0/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/README.md` & `opendal-0.31.0/local_dependencies/opendal/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.31.0/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.31.0/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.31.0/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.31.0/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.31.0/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/examples/object.rs` & `opendal-0.31.0/local_dependencies/opendal/examples/object.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.31.0/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/features.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/features.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.31.0/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-//! The internal implement details of [`Accessor`].
+//! The internal implementation details of [`Accessor`].
 //!
 //! [`Accessor`] is the core trait of OpenDAL's raw API. We operate
 //! underlying storage services via APIs provided by [`Accessor`].
 //!
 //! # Introduction
 //!
 //! [`Accessor`] can be split in the following parts:
@@ -81,17 +81,17 @@
 //!
 //! There are many trait boundings here. For now, [`Accessor`] requires the following bound:
 //!
 //! - [`Send`]: Allow user to send between threads without extra wrapper.
 //! - [`Sync`]: Allow user to sync between threads without extra lock.
 //! - [`Debug`][std::fmt::Debug]: Allow users to print underlying debug information of accessor.
 //! - [`Unpin`]: Make sure `Accessor` can be safely moved after being pinned, so users don't need to `Pin<Box<A>>`.
-//! - `'static`: Make sure `Accessor` is not a short-time reference, allow users to use `Accessor` in clouse, futures without playing with lifetime.
+//! - `'static`: Make sure `Accessor` is not a short-time reference, allow users to use `Accessor` in closures and futures without playing with lifetime.
 //!
-//! Implementer of `Accessor` should take care the following things:
+//! Implementer of `Accessor` should take care of the following things:
 //!
 //! - Implement `Debug` for backend, but don't leak credentials.
 //! - Make sure the backend is `Send` and `Sync`, wrap the internal struct with `Arc<Mutex<T>>` if necessary.
 //!
 //! ## Associated Type
 //!
 //! The first block of [`Accessor`] trait is our associated types. We
@@ -198,15 +198,15 @@
 //! /// use opendal::services::Duck;
 //! /// use opendal::Operator;
 //! ///
 //! /// #[tokio::main]
 //! /// async fn main() -> Result<()> {
 //! ///     // Create Duck backend builder.
 //! ///     let mut builder = Duck::default();
-//! ///     // Set the root for duck, all operations wilxl happen under this root.
+//! ///     // Set the root for duck, all operations will happen under this root.
 //! ///     //
 //! ///     // NOTE: the root must be absolute path.
 //! ///     builder.root("/path/to/dir");
 //! ///
 //! ///     let op: Operator = Operator::new(builder)?.finish();
 //! ///
 //! ///     Ok(())
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-//! The internal implement details of [`Layer`].
+//! The internal implementation details of [`Layer`].
 //!
-//! [`Layer`] itself is quiet simple:
+//! [`Layer`] itself is quite simple:
 //!
 //! ```ignore
 //! pub trait Layer<A: Accessor> {
 //!     type LayeredAccessor: Accessor;
 //!
 //!     fn layer(&self, inner: A) -> Self::LayeredAccessor;
 //! }
 //! ```
 //!
-//! `XxxLayer` will wrap input [`Accessor`] as inner and returns a new [`Accessor`]. So normally the implementation of [`Layer`] will be split into two parts:
+//! `XxxLayer` will wrap input [`Accessor`] as inner and return a new [`Accessor`]. So normally the implementation of [`Layer`] will be split into two parts:
 //!
-//! - `XxxLayer` will implements [`Layer`] and return `XxxAccessor` as `Self::LayeredAccessor`.
-//! - `XxxAccessor` will implements [`Accessor`] and being built by `XxxLayer`.
+//! - `XxxLayer` will implement [`Layer`] and return `XxxAccessor` as `Self::LayeredAccessor`.
+//! - `XxxAccessor` will implement [`Accessor`] and be built by `XxxLayer`.
 //!
 //! Most layer only implements part of [`Accessor`], so we provide
-//! [`LayeredAccessor`] which will forward all not implemented methods to
+//! [`LayeredAccessor`] which will forward all unimplemented methods to
 //! `inner`. It's highly recommend to implement [`LayeredAccessor`] trait
 //! instead.
 //!
 //! [`Layer`]: crate::raw::Layer
 //! [`Accessor`]: crate::raw::Accessor
 //! [`LayeredAccessor`]: crate::raw::LayeredAccessor
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.31.0/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+# Upgrade to v0.31
+
+In version v0.31 of OpenDAL, we made some internal refactoring to improve its compatibility with the ecosystem.
+
+## MSRV Bump
+
+We increased the MSRV to 1.64 from v0.31 onwards. Although it is still possible to build OpenDAL under older rustc versions, we cannot guarantee that any issues related to them will be fixed.
+
+## Accept `std::time::Duration` instead
+
+Previously, OpenDAL accepted `time::Duration` as input for `presign_xxx`. However, since v0.31, we have changed this to accept `std::time::Duration` so that users do not need to depend on `time`. Internally, we migrated from `time` to `chrono` for better integration with other parts of the ecosystem.
+
+## `disable_ec2_metadata` for services s3
+
+We have added a new configuration option called `disable_ec2_metadata` for the S3 service in response to a mistake where it was mixed up with another option called `disable_config_load`. Users who want to disable loading credentials from EC2 metadata should set this option instead.
+
+## Services Feature Flag
+
+Starting from v0.31, all services in OpenDAL are split into different feature flags. To enable only S3 support, use the following TOML configuration:
+
+```toml
+opendal = {
+    version = "0.31",
+    default-features = false,
+    features = ["services-s3"]
+}
+```
+
 # Upgrade to v0.30
 
 In version 0.30, we made significant breaking changes by removing objects. Our goal in doing so was to provide our users with APIs that are easier to understand and maintain.
 
 More detailes could be found at [RFC: Remove Object Concept][crate::docs::rfcs::rfc_1477_remove_object_concept].
 
 To upgrade to OpenDAL v0.30, users need to make the following changes:
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/complete.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files 1% similar despite different names*

```diff
@@ -198,41 +198,40 @@
                 err.with_operation(Operation::Scan)
                     .with_context("service", self.meta.scheme())
                     .with_context("path", path)
             })
             .await
     }
 
-    fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
-        self.inner.presign(path, args).map_err(|err| {
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+        self.inner.presign(path, args).await.map_err(|err| {
             err.with_operation(Operation::Presign)
                 .with_context("service", self.meta.scheme())
                 .with_context("path", path)
         })
     }
 
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         self.inner
             .batch(args)
             .map_ok(|v| {
-                let BatchedResults::Delete(res) = v.into_results();
-
-                let res = res
+                let res = v
+                    .into_results()
                     .into_iter()
                     .map(|(path, res)| {
                         let res = res.map_err(|err| {
                             err.with_operation(Operation::Delete)
                                 .with_context("service", self.meta.scheme())
                                 .with_context("path", &path)
                         });
                         (path, res)
                     })
                     .collect();
 
-                RpBatch::new(BatchedResults::Delete(res))
+                RpBatch::new(res)
             })
             .map_err(|err| {
                 err.with_operation(Operation::Batch)
                     .with_context("service", self.meta.scheme())
             })
             .await
     }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/logging.rs`

 * *Files 8% similar despite different names*

```diff
@@ -318,14 +318,96 @@
                         self.err_status(&err)
                     )
                 };
                 err
             })
     }
 
+    async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        debug!(
+            target: LOGGING_TARGET,
+            "service={} operation={} from={} to={} -> started",
+            self.scheme,
+            Operation::Copy,
+            from,
+            to
+        );
+
+        self.inner
+            .copy(from, to, args)
+            .await
+            .map(|v| {
+                debug!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} from={} to={} -> finished",
+                    self.scheme,
+                    Operation::Copy,
+                    from,
+                    to
+                );
+                v
+            })
+            .map_err(|err| {
+                if let Some(lvl) = self.err_level(&err) {
+                    log!(
+                        target: LOGGING_TARGET,
+                        lvl,
+                        "service={} operation={} from={} to={} -> {}: {err:?}",
+                        self.scheme,
+                        Operation::Copy,
+                        from,
+                        to,
+                        self.err_status(&err)
+                    )
+                };
+                err
+            })
+    }
+
+    async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        debug!(
+            target: LOGGING_TARGET,
+            "service={} operation={} from={} to={} -> started",
+            self.scheme,
+            Operation::Rename,
+            from,
+            to
+        );
+
+        self.inner
+            .rename(from, to, args)
+            .await
+            .map(|v| {
+                debug!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} from={} to={} -> finished",
+                    self.scheme,
+                    Operation::Rename,
+                    from,
+                    to
+                );
+                v
+            })
+            .map_err(|err| {
+                if let Some(lvl) = self.err_level(&err) {
+                    log!(
+                        target: LOGGING_TARGET,
+                        lvl,
+                        "service={} operation={} from={} to={} -> {}: {err:?}",
+                        self.scheme,
+                        Operation::Rename,
+                        from,
+                        to,
+                        self.err_status(&err)
+                    )
+                };
+                err
+            })
+    }
+
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         debug!(
             target: LOGGING_TARGET,
             "service={} operation={} path={} -> started",
             self.scheme,
             Operation::Stat,
             path
@@ -490,25 +572,26 @@
                     }
                     Err(err)
                 }
             })
             .await
     }
 
-    fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         debug!(
             target: LOGGING_TARGET,
             "service={} operation={} path={} -> started",
             self.scheme,
             Operation::Presign,
             path
         );
 
         self.inner
             .presign(path, args)
+            .await
             .map(|v| {
                 debug!(
                     target: LOGGING_TARGET,
                     "service={} operation={} path={} -> finished: {v:?}",
                     self.scheme,
                     Operation::Presign,
                     path
@@ -528,15 +611,15 @@
                     );
                 }
                 err
             })
     }
 
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
-        let (op, count) = (args.operation().operation(), args.operation().len());
+        let (op, count) = (args.operation()[0].1.operation(), args.operation().len());
 
         debug!(
             target: LOGGING_TARGET,
             "service={} operation={}-{op} count={count} -> started",
             self.scheme,
             Operation::Batch,
         );
@@ -546,16 +629,16 @@
             .map_ok(|v| {
                 debug!(
                     target: LOGGING_TARGET,
                     "service={} operation={}-{op} count={count} -> finished: {}, succeed: {}, failed: {}",
                     self.scheme,
                     Operation::Batch,
                     v.results().len(),
-                    v.results().len_ok(),
-                    v.results().len_err(),
+                    v.results().iter().filter(|(_, v)|v.is_ok()).count(),
+                    v.results().iter().filter(|(_, v)|v.is_err()).count(),
                 );
                 v
             })
             .map_err(|err| {
                 if let Some(lvl) = self.err_level(&err) {
                     log!(
                         target: LOGGING_TARGET,
@@ -695,14 +778,94 @@
                         self.err_status(&err)
                     );
                 }
                 err
             })
     }
 
+    fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        debug!(
+            target: LOGGING_TARGET,
+            "service={} operation={} from={} to={} -> started",
+            self.scheme,
+            Operation::BlockingCopy,
+            from,
+            to,
+        );
+
+        self.inner
+            .blocking_copy(from, to, args)
+            .map(|v| {
+                debug!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} from={} to={} -> finished",
+                    self.scheme,
+                    Operation::BlockingCopy,
+                    from,
+                    to,
+                );
+                v
+            })
+            .map_err(|err| {
+                if let Some(lvl) = self.err_level(&err) {
+                    log!(
+                        target: LOGGING_TARGET,
+                        lvl,
+                        "service={} operation={} from={} to={} -> {}: {err:?}",
+                        self.scheme,
+                        Operation::BlockingCopy,
+                        from,
+                        to,
+                        self.err_status(&err)
+                    );
+                }
+                err
+            })
+    }
+
+    fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        debug!(
+            target: LOGGING_TARGET,
+            "service={} operation={} from={} to={} -> started",
+            self.scheme,
+            Operation::BlockingMove,
+            from,
+            to,
+        );
+
+        self.inner
+            .blocking_rename(from, to, args)
+            .map(|v| {
+                debug!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} from={} to={} -> finished",
+                    self.scheme,
+                    Operation::BlockingMove,
+                    from,
+                    to,
+                );
+                v
+            })
+            .map_err(|err| {
+                if let Some(lvl) = self.err_level(&err) {
+                    log!(
+                        target: LOGGING_TARGET,
+                        lvl,
+                        "service={} operation={} from={} to={} -> {}: {err:?}",
+                        self.scheme,
+                        Operation::BlockingMove,
+                        from,
+                        to,
+                        self.err_status(&err)
+                    );
+                }
+                err
+            })
+    }
+
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         debug!(
             target: LOGGING_TARGET,
             "service={} operation={} path={} -> started",
             self.scheme,
             Operation::BlockingStat,
             path
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files 0% similar despite different names*

```diff
@@ -626,19 +626,19 @@
         result.map_err(|e| {
             self.handle
                 .increment_errors_total(Operation::Batch, e.kind());
             e
         })
     }
 
-    fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         self.handle.requests_total_presign.increment(1);
 
         let start = Instant::now();
-        let result = self.inner.presign(path, args);
+        let result = self.inner.presign(path, args).await;
         let dur = start.elapsed().as_secs_f64();
 
         self.handle.requests_duration_seconds_presign.record(dur);
 
         result.map_err(|e| {
             self.handle
                 .increment_errors_total(Operation::Presign, e.kind());
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/retry.rs`

 * *Files 2% similar despite different names*

```diff
@@ -284,24 +284,45 @@
                 })
                 .map_err(|e| e.set_persistent())
             })
             .await
     }
 
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
-        { || self.inner.batch(args.clone()) }
+        { || self.inner.batch(args.clone()).map(Err::<(), _>) }
             .retry(&self.builder)
-            .when(|e| e.is_temporary())
-            .notify(|err, dur| {
-                warn!(
+            .when(|res| match res {
+                Ok(rp) => rp.results().iter().any(|(_, v)| {
+                    if let Err(e) = v {
+                        e.is_temporary()
+                    } else {
+                        false
+                    }
+                }),
+                Err(err) => err.is_temporary(),
+            })
+            .notify(|res, dur| match res {
+                Ok(rp) => warn!(
+                    target: "opendal::service",
+                    "operation={} -> retry after {}s: error={:?}",
+                    Operation::Batch, dur.as_secs_f64(),
+                    rp.results().iter().filter_map(|(_, v)| {
+                        if let Err(e) = v  {
+                            if e.is_temporary() {
+                                return Some(e);
+                            }
+                        }
+                        None
+                }).collect::<Vec<_>>()),
+                Err(err) => warn!(
                     target: "opendal::service",
                     "operation={} -> retry after {}s: error={:?}",
-                    Operation::Batch, dur.as_secs_f64(), err)
+                    Operation::Batch, dur.as_secs_f64(), err),
             })
-            .map(|v| v.map_err(|e| e.set_persistent()))
+            .map(|v| v.unwrap_err().map_err(|e| e.set_persistent()))
             .await
     }
 
     fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         { || self.inner.blocking_create(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
@@ -805,15 +826,15 @@
         type Writer = ();
         type BlockingWriter = ();
         type Pager = MockPager;
         type BlockingPager = ();
 
         fn info(&self) -> AccessorInfo {
             let mut am = AccessorInfo::default();
-            am.set_capabilities(AccessorCapability::List);
+            am.set_capabilities(AccessorCapability::List | AccessorCapability::Batch);
             am.set_hints(AccessorHint::ReadStreamable);
 
             am
         }
 
         async fn read(&self, _: &str, _: OpRead) -> Result<(RpRead, Self::Reader)> {
             Ok((
@@ -825,14 +846,71 @@
             ))
         }
 
         async fn list(&self, _: &str, _: OpList) -> Result<(RpList, Self::Pager)> {
             let pager = MockPager::default();
             Ok((RpList::default(), pager))
         }
+
+        async fn batch(&self, op: OpBatch) -> Result<RpBatch> {
+            let mut attempt = self.attempt.lock().unwrap();
+            *attempt += 1;
+
+            match *attempt {
+                1 => Err(
+                    Error::new(ErrorKind::Unexpected, "retryable_error from reader")
+                        .set_temporary(),
+                ),
+                2 => Ok(RpBatch::new(
+                    op.into_operation()
+                        .into_iter()
+                        .map(|(s, _)| {
+                            (
+                                s,
+                                Err(Error::new(
+                                    ErrorKind::Unexpected,
+                                    "retryable_error from reader",
+                                )
+                                .set_temporary()),
+                            )
+                        })
+                        .collect(),
+                )),
+                3 => Ok(RpBatch::new(
+                    op.into_operation()
+                        .into_iter()
+                        .enumerate()
+                        .map(|(i, (s, _))| {
+                            (
+                                s,
+                                match i {
+                                    0 => Err(Error::new(
+                                        ErrorKind::Unexpected,
+                                        "retryable_error from reader",
+                                    )
+                                    .set_temporary()),
+                                    _ => Ok(RpDelete {}.into()),
+                                },
+                            )
+                        })
+                        .collect(),
+                )),
+                4 => Err(
+                    Error::new(ErrorKind::Unexpected, "retryable_error from reader")
+                        .set_temporary(),
+                ),
+                5 => Ok(RpBatch::new(
+                    op.into_operation()
+                        .into_iter()
+                        .map(|(s, _)| (s, Ok(RpDelete {}.into())))
+                        .collect(),
+                )),
+                _ => unreachable!(),
+            }
+        }
     }
 
     #[derive(Debug, Clone, Default)]
     struct MockReader {
         attempt: Arc<Mutex<usize>>,
         pos: u64,
     }
@@ -967,8 +1045,33 @@
         let mut actual = Vec::new();
         while let Some(obj) = lister.try_next().await.expect("must success") {
             actual.push(obj.name().to_owned());
         }
 
         assert_eq!(actual, expected);
     }
+
+    #[tokio::test]
+    async fn test_retry_batch() {
+        let _ = env_logger::try_init();
+
+        let builder = MockBuilder::default();
+        // set to a lower delay to make it run faster
+        let op = Operator::new(builder.clone())
+            .unwrap()
+            .layer(
+                RetryLayer::new()
+                    .with_min_delay(Duration::from_secs_f32(0.1))
+                    .with_max_times(5),
+            )
+            .finish();
+
+        let paths = vec![
+            "hello".into(),
+            "world".into(),
+            "test".into(),
+            "batch".into(),
+        ];
+        op.remove(paths).await.expect("batch must succeed");
+        assert_eq!(*builder.attempt.lock().unwrap(), 5);
+    }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files 0% similar despite different names*

```diff
@@ -194,16 +194,16 @@
         self.inner
             .scan(path, args)
             .map(|v| v.map(|(rp, s)| (rp, TracingWrapper::new(Span::current(), s))))
             .await
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
-    fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
-        self.inner.presign(path, args)
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+        self.inner.presign(path, args).await
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         self.inner.batch(args).await
     }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.31.0/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/lib.rs` & `opendal-0.31.0/local_dependencies/opendal/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files 7% similar despite different names*

```diff
@@ -127,14 +127,44 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
+    /// Invoke the `copy` operation on the specified `from` path and `to` path.
+    ///
+    /// Require [AccessorCapability::Copy]
+    ///
+    /// # Behaviour
+    ///
+    /// - `from` and `to` MUST be file path, DON'T NEED to check mode.
+    /// - Copy on existing file SHOULD succeed.
+    /// - Copy on existing file SHOULD overwrite and truncate.
+    async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        let (_, _, _) = (from, to, args);
+
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "operation is not supported",
+        ))
+    }
+
+    /// Invoke the `rename` operation on the specified `from` path and `to` path.
+    ///
+    /// Require [AccessorCapability::Rename]
+    async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        let (_, _, _) = (from, to, args);
+
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "operation is not supported",
+        ))
+    }
+
     /// Invoke the `stat` operation on the specified path.
     ///
     /// Require [`AccessorCapability::Read`]
     ///
     /// # Behavior
     ///
     /// - `stat` empty path means stat backend's root path.
@@ -198,15 +228,15 @@
     /// Invoke the `presign` operation on the specified path.
     ///
     /// Require [`AccessorCapability::Presign`]
     ///
     /// # Behavior
     ///
     /// - This API is optional, return [`std::io::ErrorKind::Unsupported`] if not supported.
-    fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         let (_, _) = (path, args);
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
@@ -259,14 +289,42 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
+    /// Invoke the `blocking_copy` operation on the specified `from` path and `to` path.
+    ///
+    /// This operation is the blocking version of [`Accessor::copy`]
+    ///
+    /// Require [`AccessorCapability::Copy`] and [`AccessorCapability::Blocking`]
+    fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        let (_, _, _) = (from, to, args);
+
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "operation is not supported",
+        ))
+    }
+
+    /// Invoke the `blocking_rename` operation on the specified `from` path and `to` path.
+    ///
+    /// This operation is the blocking version of [`Accessor::rename`]
+    ///
+    /// Require [`AccessorCapability::Rename`] and [`AccessorCapability::Blocking`]
+    fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        let (_, _, _) = (from, to, args);
+
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "operation is not supported",
+        ))
+    }
+
     /// Invoke the `blocking_stat` operation on the specified path.
     ///
     /// This operation is the blocking version of [`Accessor::stat`]
     ///
     /// Require [`AccessorCapability::Read`] and [`AccessorCapability::Blocking`]
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         let (_, _) = (path, args);
@@ -365,14 +423,23 @@
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         self.as_ref().read(path, args).await
     }
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         self.as_ref().write(path, args).await
     }
+
+    async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        self.as_ref().copy(from, to, args).await
+    }
+
+    async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        self.as_ref().rename(from, to, args).await
+    }
+
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.as_ref().stat(path, args).await
     }
     async fn delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         self.as_ref().delete(path, args).await
     }
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
@@ -382,27 +449,36 @@
         self.as_ref().scan(path, args).await
     }
 
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         self.as_ref().batch(args).await
     }
 
-    fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
-        self.as_ref().presign(path, args)
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+        self.as_ref().presign(path, args).await
     }
 
     fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         self.as_ref().blocking_create(path, args)
     }
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         self.as_ref().blocking_read(path, args)
     }
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
         self.as_ref().blocking_write(path, args)
     }
+
+    fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        self.as_ref().blocking_copy(from, to, args)
+    }
+
+    fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        self.as_ref().blocking_rename(from, to, args)
+    }
+
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.as_ref().blocking_stat(path, args)
     }
     fn blocking_delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         self.as_ref().blocking_delete(path, args)
     }
     fn blocking_list(&self, path: &str, args: OpList) -> Result<(RpList, Self::BlockingPager)> {
@@ -524,14 +600,18 @@
 flags! {
     /// AccessorCapability describes accessor's advanced capability.
     pub enum AccessorCapability: u32 {
         /// Add this capability if service supports `read` and `stat`
         Read,
         /// Add this capability if service supports `write` and `delete`
         Write,
+        /// Add this capability if service supports `copy`
+        Copy,
+        /// Add this capability if service supports `rename`
+        Rename,
         /// Add this capability if service supports `list`
         List,
         /// Add this capability if service supports `scan`
         Scan,
         /// Add this capability if service supports `presign`
         Presign,
         /// Add this capability if service supports `blocking`
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files 20% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::cmp::min;
 use std::cmp::Ordering;
 use std::io;
-use std::io::Read;
-use std::io::Write;
 use std::task::Context;
 use std::task::Poll;
 
 use bytes::Buf;
 use bytes::BufMut;
 use bytes::Bytes;
 use futures::ready;
@@ -31,81 +29,29 @@
 use futures::StreamExt;
 
 use crate::raw::*;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Result;
 
-/// Body used in blocking HTTP requests.
-pub enum Body {
-    /// An empty body.
-    Empty,
-    /// Body with bytes.
-    Bytes(Bytes),
-    /// Body with a Reader.
-    Reader(Box<dyn Read + Send>),
-}
-
-impl Default for Body {
-    fn default() -> Self {
-        Body::Empty
-    }
-}
-
-impl Body {
-    /// Consume the entire body.
-    pub fn consume(self) -> Result<()> {
-        if let Body::Reader(mut r) = self {
-            std::io::copy(&mut r, &mut std::io::sink()).map_err(|err| {
-                Error::new(ErrorKind::Unexpected, "consuming response")
-                    .with_operation("http_util::Body::consume")
-                    .set_source(err)
-            })?;
-        }
-
-        Ok(())
-    }
-}
-
-impl Read for Body {
-    fn read(&mut self, mut buf: &mut [u8]) -> io::Result<usize> {
-        match self {
-            Body::Empty => Ok(0),
-            Body::Bytes(bs) => {
-                let size = min(bs.len(), buf.len());
-                let rbs = bs.split_to(size);
-                bs.advance(size);
-
-                buf.write_all(&rbs).expect("write all must succeed");
-                Ok(size)
-            }
-            Body::Reader(r) => r.read(buf),
-        }
-    }
-}
-
 /// Body used in async HTTP requests.
+#[derive(Default)]
 pub enum AsyncBody {
     /// An empty body.
+    #[default]
     Empty,
     /// Body with bytes.
     Bytes(Bytes),
     /// Body with a multipart field.
     ///
     /// If input with this field, we will goto the internal multipart
     /// handle logic.
     Multipart(String, Bytes),
 }
 
-impl Default for AsyncBody {
-    fn default() -> Self {
-        AsyncBody::Empty
-    }
-}
-
 impl From<AsyncBody> for reqwest::Body {
     fn from(v: AsyncBody) -> Self {
         match v {
             AsyncBody::Empty => reqwest::Body::from(""),
             AsyncBody::Bytes(bs) => reqwest::Body::from(bs),
             AsyncBody::Multipart(_, _) => {
                 unreachable!("reqwest multipart should not be constructed by body")
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/dns.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files 27% similar despite different names*

```diff
@@ -12,226 +12,226 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
-use std::io;
-use std::net::SocketAddr;
-use std::net::ToSocketAddrs;
-use std::sync::Arc;
+use std::fmt::Debug;
 use std::time::Duration;
-use std::time::SystemTime;
 
-use futures::future;
-use parking_lot::Mutex;
+use async_trait::async_trait;
+use log::debug;
+use moka::sync::CacheBuilder;
+use moka::sync::SegmentedCache;
+
+use crate::raw::adapters::kv;
+use crate::raw::*;
+use crate::*;
 
-/// StdDnsResolver uses `getaddrinfo` to query dns.
-#[derive(Default)]
-pub struct StdDnsResolver {
-    cache: DnsCache,
+/// [moka](https://github.com/moka-rs/moka) backend support.
+///
+/// # Capabilities
+///
+/// This service can be used to:
+///
+/// - [x] read
+/// - [x] write
+/// - [ ] ~~list~~
+/// - [ ] ~~scan~~
+/// - [ ] ~~presign~~
+/// - [x] blocking
+#[derive(Default, Debug)]
+pub struct MokaBuilder {
+    /// Name for this cache instance.
+    name: Option<String>,
+    /// Sets the max capacity of the cache.
+    ///
+    /// Refer to [`moka::sync::CacheBuilder::max_capacity`](https://docs.rs/moka/latest/moka/sync/struct.CacheBuilder.html#method.max_capacity)
+    max_capacity: Option<u64>,
+    /// Sets the time to live of the cache.
+    ///
+    /// Refer to [`moka::sync::CacheBuilder::time_to_live`](https://docs.rs/moka/latest/moka/sync/struct.CacheBuilder.html#method.time_to_live)
+    time_to_live: Option<Duration>,
+    /// Sets the time to idle of the cache.
+    ///
+    /// Refer to [`moka::sync::CacheBuilder::time_to_idle`](https://docs.rs/moka/latest/moka/sync/struct.CacheBuilder.html#method.time_to_idle)
+    time_to_idle: Option<Duration>,
+    /// Sets the segments number of the cache.
+    ///
+    /// Refer to [`moka::sync::CacheBuilder::segments`](https://docs.rs/moka/latest/moka/sync/struct.CacheBuilder.html#method.segments)
+    num_segments: Option<usize>,
+    /// Decides whether to enable thread pool of the cache.
+    ///
+    /// Refer to [`moka::sync::CacheBuilder::thread_pool_enabled`](https://docs.rs/moka/latest/moka/sync/struct.CacheBuilder.html#method.thread_pool_enabled)
+    thread_pool_enabled: Option<bool>,
 }
 
-impl ureq::Resolver for StdDnsResolver {
-    fn resolve(&self, netloc: &str) -> io::Result<Vec<SocketAddr>> {
-        if let Some(v) = self.cache.get(netloc) {
-            return Ok(v);
+impl MokaBuilder {
+    /// Name for this cache instance.
+    pub fn name(&mut self, v: &str) -> &mut Self {
+        if !v.is_empty() {
+            self.name = Some(v.to_owned());
         }
-
-        ToSocketAddrs::to_socket_addrs(netloc).map(|iter| {
-            let res: Vec<_> = iter.collect();
-            // Insert into cache if resolved succeeded.
-            self.cache.insert(netloc, res.clone());
-            res
-        })
+        self
     }
-}
 
-/// AsyncStdDnsResolver uses `getaddrinfo` to query dns in tokio runtime.
-pub struct AsyncStdDnsResolver {
-    cache: DnsCache,
-    runtime: Option<tokio::runtime::Runtime>,
-}
-
-impl Default for AsyncStdDnsResolver {
-    fn default() -> Self {
-        let runtime = {
-            let mut builder = tokio::runtime::Builder::new_current_thread();
-            builder.enable_all();
+    /// Sets the max capacity of the cache.
+    ///
+    /// Refer to [`moka::sync::CacheBuilder::max_capacity`](https://docs.rs/moka/latest/moka/sync/struct.CacheBuilder.html#method.max_capacity)
+    pub fn max_capacity(&mut self, v: u64) -> &mut Self {
+        if v != 0 {
+            self.max_capacity = Some(v);
+        }
+        self
+    }
 
-            builder.build().expect("build dns runtime failed")
-        };
+    /// Sets the time to live of the cache.
+    ///
+    /// Refer to [`moka::sync::CacheBuilder::time_to_live`](https://docs.rs/moka/latest/moka/sync/struct.CacheBuilder.html#method.time_to_live)
+    pub fn time_to_live(&mut self, v: Duration) -> &mut Self {
+        if !v.is_zero() {
+            self.time_to_live = Some(v);
+        }
+        self
+    }
 
-        Self {
-            cache: DnsCache::default(),
-            runtime: Some(runtime),
+    /// Sets the time to idle of the cache.
+    ///
+    /// Refer to [`moka::sync::CacheBuilder::time_to_idle`](https://docs.rs/moka/latest/moka/sync/struct.CacheBuilder.html#method.time_to_idle)
+    pub fn time_to_idle(&mut self, v: Duration) -> &mut Self {
+        if !v.is_zero() {
+            self.time_to_idle = Some(v);
         }
+        self
     }
-}
 
-/// Make sure runtime has been dropped in background.
-impl Drop for AsyncStdDnsResolver {
-    fn drop(&mut self) {
-        let runtime = self.runtime.take().unwrap();
-        runtime.shutdown_background();
+    /// Sets the segments number of the cache.
+    ///
+    /// Refer to [`moka::sync::CacheBuilder::segments`](https://docs.rs/moka/latest/moka/sync/struct.CacheBuilder.html#method.segments)
+    pub fn segments(&mut self, v: usize) -> &mut Self {
+        assert!(v != 0);
+        self.num_segments = Some(v);
+        self
+    }
+
+    /// Decides whether to enable thread pool of the cache.
+    ///
+    /// Refer to [`moka::sync::CacheBuilder::thread_pool_enabled`](https://docs.rs/moka/latest/moka/sync/struct.CacheBuilder.html#method.thread_pool_enabled)
+    pub fn thread_pool_enabled(&mut self, v: bool) -> &mut Self {
+        self.thread_pool_enabled = Some(v);
+        self
     }
 }
 
-impl reqwest::dns::Resolve for AsyncStdDnsResolver {
-    fn resolve(&self, name: hyper::client::connect::dns::Name) -> reqwest::dns::Resolving {
-        if let Some(v) = self.cache.get(name.as_str()) {
-            return Box::pin(future::ok(Box::new(v.into_iter()) as reqwest::dns::Addrs));
-        }
+impl Builder for MokaBuilder {
+    const SCHEME: Scheme = Scheme::Moka;
+    type Accessor = MokaBackend;
 
-        debug_assert!(self.runtime.is_some(), "runtime must be valid");
-        let runtime = self.runtime.as_ref().unwrap().handle().clone();
+    fn from_map(map: HashMap<String, String>) -> Self {
+        let mut builder = MokaBuilder::default();
 
-        let cache = self.cache.clone();
-        let fut = async move {
-            match runtime
-                .spawn_blocking(move || {
-                    // hyper will set port externally, so the port here is
-                    // just used to construct a correct query.
-                    //
-                    // Ref: <https://github.com/hyperium/hyper/blob/4d89adce6122af1650165337d9d814314e7ee409/src/client/connect/http.rs#L322-L359>
-                    (name.as_str(), 0).to_socket_addrs().map(|iter| {
-                        let res: Vec<_> = iter.collect();
-                        // Insert into cache if resolved succeeded.
-                        cache.insert(name.as_str(), res.clone());
-                        res
-                    })
-                })
-                .await
-            {
-                Ok(v) => v.map(|v| Box::new(v.into_iter()) as reqwest::dns::Addrs),
-                Err(err) => Err(io::Error::new(
-                    io::ErrorKind::Other,
-                    format!("spawn dns resolving task failed: {err:?}"),
-                )),
-            }
-            .map_err(|err| Box::new(err) as Box<_>)
-        };
+        map.get("name").map(|v| builder.name(v));
+        map.get("max_capacity")
+            .map(|v| v.parse::<u64>().map(|v| builder.max_capacity(v)));
+        map.get("time_to_live").map(|v| {
+            v.parse::<u64>()
+                .map(|v| builder.time_to_live(Duration::from_secs(v)))
+        });
+        map.get("time_to_idle").map(|v| {
+            v.parse::<u64>()
+                .map(|v| builder.time_to_idle(Duration::from_secs(v)))
+        });
+        map.get("num_segments")
+            .map(|v| v.parse::<usize>().map(|v| builder.segments(v)));
+        map.get("thread_pool_enabled")
+            .map(|v| v.parse::<bool>().map(|v| builder.thread_pool_enabled(v)));
 
-        Box::pin(fut)
+        builder
     }
-}
 
-/// TrustDnsResolver will adopt `trust-dns` to query dns in tokio runtime.
-///
-/// We will only use trust dns while we have an async runtime.
-#[cfg(feature = "trust-dns")]
-pub struct AsyncTrustDnsResolver {
-    inner: Arc<trust_dns_resolver::TokioAsyncResolver>,
-}
+    fn build(&mut self) -> Result<Self::Accessor> {
+        debug!("backend build started: {:?}", &self);
 
-#[cfg(feature = "trust-dns")]
-impl AsyncTrustDnsResolver {
-    pub fn new() -> io::Result<Self> {
-        let resolver = trust_dns_resolver::TokioAsyncResolver::from_system_conf(
-            trust_dns_resolver::TokioHandle,
-        )?;
+        let mut builder: CacheBuilder<String, Vec<u8>, _> =
+            SegmentedCache::builder(self.num_segments.unwrap_or(1))
+                .thread_pool_enabled(self.thread_pool_enabled.unwrap_or(false));
+        // Use entries' bytes as capacity weigher.
+        builder = builder.weigher(|k, v| (k.len() + v.len()) as u32);
+        if let Some(v) = &self.name {
+            builder = builder.name(v);
+        }
+        if let Some(v) = self.max_capacity {
+            builder = builder.max_capacity(v)
+        }
+        if let Some(v) = self.time_to_live {
+            builder = builder.time_to_live(v)
+        }
+        if let Some(v) = self.time_to_idle {
+            builder = builder.time_to_idle(v)
+        }
 
-        Ok(Self {
-            inner: Arc::new(resolver),
-        })
+        debug!("backend build finished: {:?}", &self);
+        Ok(MokaBackend::new(Adapter {
+            inner: builder.build(),
+        }))
     }
 }
 
-#[cfg(feature = "trust-dns")]
-impl reqwest::dns::Resolve for AsyncTrustDnsResolver {
-    fn resolve(&self, name: hyper::client::connect::dns::Name) -> reqwest::dns::Resolving {
-        let resolver = self.inner.clone();
-
-        let fut = async move {
-            let lookup = resolver.lookup_ip(name.as_str()).await?;
+/// Backend is used to serve `Accessor` support in moka.
+pub type MokaBackend = kv::Backend<Adapter>;
 
-            // hyper will set port externally, so the port here is
-            // just used to construct a correct SocketAddr.
-            //
-            // Ref: <https://github.com/hyperium/hyper/blob/4d89adce6122af1650165337d9d814314e7ee409/src/client/connect/http.rs#L322-L359>
-            Ok(Box::new(lookup.into_iter().map(|v| SocketAddr::new(v, 0))) as reqwest::dns::Addrs)
-        };
+#[derive(Clone)]
+pub struct Adapter {
+    inner: SegmentedCache<String, Vec<u8>>,
+}
 
-        Box::pin(fut)
+impl Debug for Adapter {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        f.debug_struct("Adapter")
+            .field("size", &self.inner.weighted_size())
+            .field("count", &self.inner.entry_count())
+            .finish()
     }
 }
 
-/// The cache entry we maintained in memory.
-#[derive(Clone)]
-struct DnsCacheEntry {
-    value: Vec<SocketAddr>,
-    expires_in: SystemTime,
-}
+#[async_trait]
+impl kv::Adapter for Adapter {
+    fn metadata(&self) -> kv::Metadata {
+        kv::Metadata::new(
+            Scheme::Moka,
+            self.inner.name().unwrap_or("moka"),
+            AccessorCapability::Read | AccessorCapability::Write,
+        )
+    }
 
-/// DnsCache that used for accessing different storage services.
-///
-/// # Notes
-///
-/// **DON'T USE THIS DNS CACHE OUTSIDE OPENDAL.**
-///
-/// This is not a general dns cache that suitable for all use-cases.
-#[derive(Clone)]
-struct DnsCache {
-    inner: Arc<Mutex<HashMap<String, DnsCacheEntry>>>,
+    async fn get(&self, path: &str) -> Result<Option<Vec<u8>>> {
+        self.blocking_get(path)
+    }
 
-    /// The most cache entries that we can hold.
-    ///
-    /// We will use 32 as default value (the same value as trust-dns).
-    limits: usize,
-    /// Ideally, we need to set the expire based on resolved dns record. But
-    /// rust std doesn't give us this choice, so we have to use default one.
-    ///
-    /// We will use 3600s as the default expire time. In the future, we will
-    /// allow user to configure it.
-    default_expire: Duration,
-}
-
-impl Default for DnsCache {
-    fn default() -> Self {
-        DnsCache {
-            inner: Arc::default(),
-            limits: 32,
-            default_expire: Duration::from_secs(3600),
+    fn blocking_get(&self, path: &str) -> Result<Option<Vec<u8>>> {
+        match self.inner.get(path) {
+            None => Ok(None),
+            Some(bs) => Ok(Some(bs)),
         }
     }
-}
 
-impl DnsCache {
-    fn get(&self, domain: &str) -> Option<Vec<SocketAddr>> {
-        let mut guard = self.inner.lock();
-        match guard.get(domain) {
-            None => None,
-            Some(entry) => {
-                let now = SystemTime::now();
-                if entry.expires_in >= now {
-                    Some(entry.value.clone())
-                } else {
-                    // Remove already expires entry.
-                    guard.remove(domain);
-                    None
-                }
-            }
-        }
+    async fn set(&self, path: &str, value: &[u8]) -> Result<()> {
+        self.blocking_set(path, value)
     }
 
-    fn insert(&self, domain: &str, value: Vec<SocketAddr>) {
-        let mut guard = self.inner.lock();
-
-        // If we are reaching the limits of dns cache entry. We will clean the
-        // entire cache to make more space.
-        //
-        // As described in DnsCache's doc, this limit should never be reached.
-        // We expect there only few entries held in cache.
-        if guard.len() >= self.limits {
-            guard.clear()
-        }
-
-        guard.insert(
-            domain.to_string(),
-            DnsCacheEntry {
-                value,
-                expires_in: SystemTime::now() + self.default_expire,
-            },
-        );
+    fn blocking_set(&self, path: &str, value: &[u8]) -> Result<()> {
+        self.inner.insert(path.to_string(), value.to_vec());
+
+        Ok(())
+    }
+
+    async fn delete(&self, path: &str) -> Result<()> {
+        self.blocking_delete(path)
+    }
+
+    fn blocking_delete(&self, path: &str) -> Result<()> {
+        self.inner.invalidate(path);
+
+        Ok(())
     }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files 7% similar despite different names*

```diff
@@ -91,12 +91,22 @@
 pub fn new_request_build_error(err: http::Error) -> Error {
     Error::new(ErrorKind::Unexpected, "building http request")
         .with_operation("http::Request::build")
         .set_source(err)
 }
 
 /// Create a new error happened during signing request.
+pub fn new_request_credential_error(err: anyhow::Error) -> Error {
+    Error::new(
+        ErrorKind::Unexpected,
+        "loading credentail to sign http request",
+    )
+    .with_operation("reqsign::LoadCredential")
+    .set_source(err)
+}
+
+/// Create a new error happened during signing request.
 pub fn new_request_sign_error(err: anyhow::Error) -> Error {
     Error::new(ErrorKind::Unexpected, "signing http request")
         .with_operation("reqsign::Sign")
         .set_source(err)
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files 5% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use base64::engine::general_purpose;
 use base64::Engine;
+use chrono::DateTime;
+use chrono::Utc;
 use http::header::HeaderName;
 use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_RANGE;
 use http::header::CONTENT_TYPE;
 use http::header::ETAG;
 use http::header::LAST_MODIFIED;
 use http::header::LOCATION;
 use http::HeaderMap;
+use http::HeaderValue;
 use md5::Digest;
-use time::format_description::well_known::Rfc2822;
-use time::OffsetDateTime;
 
 use crate::raw::*;
 use crate::EntryMode;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Metadata;
 use crate::Result;
@@ -125,36 +126,28 @@
                 })?
                 .parse()?,
         )),
     }
 }
 
 /// Parse last modified from header map.
-pub fn parse_last_modified(headers: &HeaderMap) -> Result<Option<OffsetDateTime>> {
+pub fn parse_last_modified(headers: &HeaderMap) -> Result<Option<DateTime<Utc>>> {
     match headers.get(LAST_MODIFIED) {
         None => Ok(None),
         Some(v) => {
             let v = v.to_str().map_err(|e| {
                 Error::new(
                     ErrorKind::Unexpected,
                     "header value is not valid utf-8 string",
                 )
                 .with_operation("http_util::parse_last_modified")
                 .set_source(e)
             })?;
-            let t = OffsetDateTime::parse(v, &Rfc2822).map_err(|e| {
-                Error::new(
-                    ErrorKind::Unexpected,
-                    "header value is not valid rfc2822 time",
-                )
-                .with_operation("http_util::parse_last_modified")
-                .set_source(e)
-            })?;
 
-            Ok(Some(t))
+            Ok(Some(parse_datetime_from_rfc2822(v)?))
         }
     }
 }
 
 /// Parse etag from header map.
 pub fn parse_etag(headers: &HeaderMap) -> Result<Option<&str>> {
     match headers.get(ETAG) {
@@ -269,14 +262,26 @@
             "can't build authorization header with empty token",
         ));
     }
 
     Ok(format!("Bearer {token}"))
 }
 
+/// Build header value from given string.
+pub fn build_header_value(v: &str) -> Result<HeaderValue> {
+    HeaderValue::from_str(v).map_err(|e| {
+        Error::new(
+            ErrorKind::ConfigInvalid,
+            "header value contains invalid characters",
+        )
+        .with_operation("http_util::build_header_value")
+        .set_source(e)
+    })
+}
+
 #[cfg(test)]
 mod tests {
     use super::*;
 
     /// Test cases is from https://docs.aws.amazon.com/AmazonS3/latest/API/API_DeleteObjects.html
     #[test]
     fn test_format_content_md5() {
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 //! it easier to develop services and layers outside opendal.
 
 mod client;
 pub use client::HttpClient;
 
 mod body;
 pub use body::AsyncBody;
-pub use body::Body;
 pub use body::IncomingAsyncBody;
 
 mod header;
+pub use header::build_header_value;
 pub use header::format_authorization_by_basic;
 pub use header::format_authorization_by_bearer;
 pub use header::format_content_md5;
 pub use header::parse_content_disposition;
 pub use header::parse_content_length;
 pub use header::parse_content_md5;
 pub use header::parse_content_range;
@@ -45,18 +45,17 @@
 pub use header::parse_location;
 
 mod uri;
 pub use uri::percent_encode_path;
 
 mod error;
 pub use error::new_request_build_error;
+pub use error::new_request_credential_error;
 pub use error::new_request_sign_error;
 pub use error::parse_error_response;
 pub use error::ErrorResponse;
 
 mod bytes_range;
 pub use bytes_range::BytesRange;
 
 mod bytes_content_range;
 pub use bytes_content_range::BytesContentRange;
-
-mod dns;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/layer.rs`

 * *Files 9% similar despite different names*

```diff
@@ -155,14 +155,22 @@
         self.inner().create(path, args).await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)>;
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)>;
 
+    async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        self.inner().copy(from, to, args).await
+    }
+
+    async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        self.inner().rename(from, to, args).await
+    }
+
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.inner().stat(path, args).await
     }
 
     async fn delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         self.inner().delete(path, args).await
     }
@@ -171,26 +179,34 @@
 
     async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)>;
 
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         self.inner().batch(args).await
     }
 
-    fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
-        self.inner().presign(path, args)
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+        self.inner().presign(path, args).await
     }
 
     fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         self.inner().blocking_create(path, args)
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)>;
 
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)>;
 
+    fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        self.inner().blocking_copy(from, to, args)
+    }
+
+    fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        self.inner().blocking_rename(from, to, args)
+    }
+
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.inner().blocking_stat(path, args)
     }
 
     fn blocking_delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         self.inner().blocking_delete(path, args)
     }
@@ -221,14 +237,22 @@
         (self as &L).read(path, args).await
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         (self as &L).write(path, args).await
     }
 
+    async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        (self as &L).copy(from, to, args).await
+    }
+
+    async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        (self as &L).rename(from, to, args).await
+    }
+
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         (self as &L).stat(path, args).await
     }
 
     async fn delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         (self as &L).delete(path, args).await
     }
@@ -241,30 +265,38 @@
         (self as &L).scan(path, args).await
     }
 
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         (self as &L).batch(args).await
     }
 
-    fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
-        (self as &L).presign(path, args)
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+        (self as &L).presign(path, args).await
     }
 
     fn blocking_create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         (self as &L).blocking_create(path, args)
     }
 
     fn blocking_read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::BlockingReader)> {
         (self as &L).blocking_read(path, args)
     }
 
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
         (self as &L).blocking_write(path, args)
     }
 
+    fn blocking_copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
+        (self as &L).blocking_copy(from, to, args)
+    }
+
+    fn blocking_rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
+        (self as &L).blocking_rename(from, to, args)
+    }
+
     fn blocking_stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         (self as &L).blocking_stat(path, args)
     }
 
     fn blocking_delete(&self, path: &str, args: OpDelete) -> Result<RpDelete> {
         (self as &L).blocking_delete(path, args)
     }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -60,9 +60,12 @@
 
 mod http_util;
 pub use http_util::*;
 
 mod serde_util;
 pub use serde_util::*;
 
+mod chrono_util;
+pub use chrono_util::*;
+
 // Expose as a pub mod to avoid confusing.
 pub mod adapters;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/operation.rs`

 * *Files 12% similar despite different names*

```diff
@@ -15,25 +15,30 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Display;
 use std::fmt::Formatter;
 
 /// Operation is the name for APIs in `Accessor`.
-#[derive(Debug, Copy, Clone, Hash, Eq, PartialEq)]
+#[derive(Debug, Copy, Clone, Hash, Eq, PartialEq, Default)]
 #[non_exhaustive]
 pub enum Operation {
     /// Operation for [`crate::raw::Accessor::info`]
+    #[default]
     Info,
     /// Operation for [`crate::raw::Accessor::create`]
     Create,
     /// Operation for [`crate::raw::Accessor::read`]
     Read,
     /// Operation for [`crate::raw::Accessor::write`]
     Write,
+    /// Operation for [`crate::raw::Accessor::copy`]
+    Copy,
+    /// Operation for [`crate::raw::Accessor::rename`]
+    Rename,
     /// Operation for [`crate::raw::Accessor::stat`]
     Stat,
     /// Operation for [`crate::raw::Accessor::delete`]
     Delete,
     /// Operation for [`crate::raw::Accessor::list`]
     List,
     /// Operation for [`crate::raw::Accessor::scan`]
@@ -44,14 +49,18 @@
     Presign,
     /// Operation for [`crate::raw::Accessor::blocking_create`]
     BlockingCreate,
     /// Operation for [`crate::raw::Accessor::blocking_read`]
     BlockingRead,
     /// Operation for [`crate::raw::Accessor::blocking_write`]
     BlockingWrite,
+    /// Operation for [`crate::raw::Accessor::blocking_copy`]
+    BlockingCopy,
+    /// Operation for [`crate::raw::Accessor::blocking_rename`]
+    BlockingMove,
     /// Operation for [`crate::raw::Accessor::blocking_stat`]
     BlockingStat,
     /// Operation for [`crate::raw::Accessor::blocking_delete`]
     BlockingDelete,
     /// Operation for [`crate::raw::Accessor::blocking_list`]
     BlockingList,
     /// Operation for [`crate::raw::Accessor::blocking_scan`]
@@ -61,42 +70,40 @@
 impl Operation {
     /// Convert self into static str.
     pub fn into_static(self) -> &'static str {
         self.into()
     }
 }
 
-impl Default for Operation {
-    fn default() -> Self {
-        Operation::Info
-    }
-}
-
 impl Display for Operation {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}", self.into_static())
     }
 }
 
 impl From<Operation> for &'static str {
     fn from(v: Operation) -> &'static str {
         match v {
             Operation::Info => "metadata",
             Operation::Create => "create",
             Operation::Read => "read",
             Operation::Write => "write",
+            Operation::Copy => "copy",
+            Operation::Rename => "rename",
             Operation::Stat => "stat",
             Operation::Delete => "delete",
             Operation::List => "list",
             Operation::Scan => "scan",
             Operation::Presign => "presign",
             Operation::Batch => "batch",
             Operation::BlockingCreate => "blocking_create",
             Operation::BlockingRead => "blocking_read",
             Operation::BlockingWrite => "blocking_write",
+            Operation::BlockingCopy => "blocking_copy",
+            Operation::BlockingMove => "blocking_rename",
             Operation::BlockingStat => "blocking_stat",
             Operation::BlockingDelete => "blocking_delete",
             Operation::BlockingList => "blocking_list",
             Operation::BlockingScan => "blocking_scan",
         }
     }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/rps.rs`

 * *Files 16% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 /// Reply for `presign` operation.
 #[derive(Debug, Clone)]
 pub struct RpPresign {
     req: PresignedRequest,
 }
 
 impl RpPresign {
-    /// Create a new reply for presign.
+    /// Create a new reply for `presign`.
     pub fn new(req: PresignedRequest) -> Self {
         RpPresign { req }
     }
 
     /// Consume reply to build a presigned request.
     pub fn into_presigned_request(self) -> PresignedRequest {
         self.req
@@ -103,15 +103,15 @@
 /// Reply for `read` operation.
 #[derive(Debug, Clone)]
 pub struct RpRead {
     meta: Metadata,
 }
 
 impl RpRead {
-    /// Create a new reply.
+    /// Create a new reply for `read`.
     pub fn new(content_length: u64) -> Self {
         RpRead {
             meta: Metadata::new(EntryMode::FILE).with_content_length(content_length),
         }
     }
 
     /// Create reply read with existing metadata.
@@ -128,82 +128,54 @@
     pub fn into_metadata(self) -> Metadata {
         self.meta
     }
 }
 
 /// Reply for `batch` operation.
 pub struct RpBatch {
-    results: BatchedResults,
+    results: Vec<(String, Result<BatchedReply>)>,
 }
 
 impl RpBatch {
     /// Create a new RpBatch.
-    pub fn new(results: BatchedResults) -> Self {
+    pub fn new(results: Vec<(String, Result<BatchedReply>)>) -> Self {
         Self { results }
     }
 
     /// Get the results from RpBatch.
-    pub fn results(&self) -> &BatchedResults {
+    pub fn results(&self) -> &[(String, Result<BatchedReply>)] {
         &self.results
     }
 
     /// Consume RpBatch to get the batched results.
-    pub fn into_results(self) -> BatchedResults {
+    pub fn into_results(self) -> Vec<(String, Result<BatchedReply>)> {
         self.results
     }
 }
 
 /// Batch results of `batch` operations.
-pub enum BatchedResults {
-    /// results of delete batch operation
-    Delete(Vec<(String, Result<RpDelete>)>),
+pub enum BatchedReply {
+    /// results of `delete batch` operation
+    Delete(RpDelete),
 }
 
-impl BatchedResults {
-    /// Return the length of given results.
-    pub fn len(&self) -> usize {
-        use BatchedResults::*;
-        match self {
-            Delete(v) => v.len(),
-        }
-    }
-
-    /// Return if given results is empty.
-    pub fn is_empty(&self) -> bool {
-        use BatchedResults::*;
-        match self {
-            Delete(v) => v.is_empty(),
-        }
-    }
-
-    /// Return the length of ok results.
-    pub fn len_ok(&self) -> usize {
-        use BatchedResults::*;
-        match self {
-            Delete(v) => v.iter().filter(|v| v.1.is_ok()).count(),
-        }
-    }
-
-    /// Return the length of error results.
-    pub fn len_err(&self) -> usize {
-        use BatchedResults::*;
-        match self {
-            Delete(v) => v.iter().filter(|v| v.1.is_err()).count(),
-        }
+impl From<RpDelete> for BatchedReply {
+    fn from(rp: RpDelete) -> Self {
+        Self::Delete(rp)
     }
 }
 
 /// Reply for `stat` operation.
 #[derive(Debug, Clone)]
 pub struct RpStat {
     meta: Metadata,
 }
 
 impl RpStat {
-    /// Create a new reply for stat.
+    /// Create a new reply for `stat`.
     pub fn new(meta: Metadata) -> Self {
         RpStat { meta }
     }
 
     /// Operate on inner metadata.
     pub fn map_metadata(mut self, f: impl FnOnce(Metadata) -> Metadata) -> Self {
         self.meta = f(self.meta);
@@ -217,15 +189,37 @@
 }
 
 /// Reply for `write` operation.
 #[derive(Debug, Clone, Default)]
 pub struct RpWrite {}
 
 impl RpWrite {
-    /// Create a new reply for write.
+    /// Create a new reply for `write`.
+    pub fn new() -> Self {
+        Self {}
+    }
+}
+
+/// Reply for `copy` operation.
+#[derive(Debug, Clone, Default)]
+pub struct RpCopy {}
+
+impl RpCopy {
+    /// Create a new reply for `copy`.
+    pub fn new() -> Self {
+        Self {}
+    }
+}
+
+/// Reply for `rename` operation.
+#[derive(Debug, Clone, Default)]
+pub struct RpRename {}
+
+impl RpRename {
+    /// Create a new reply for `rename`.
     pub fn new() -> Self {
         Self {}
     }
 }
 
 #[cfg(test)]
 mod tests {
@@ -249,24 +243,15 @@
                 headers.insert(CONTENT_LENGTH, "123".parse()?);
                 headers.insert(CONTENT_TYPE, "application/json".parse()?);
 
                 headers
             },
         };
 
-        let req: Request<AsyncBody> = pr.clone().into();
-        assert_eq!(Method::PATCH, req.method());
-        assert_eq!(
-            "https://opendal.apache.org/path/to/file",
-            req.uri().to_string()
-        );
-        assert_eq!("123", req.headers().get(CONTENT_LENGTH).unwrap());
-        assert_eq!("application/json", req.headers().get(CONTENT_TYPE).unwrap());
-
-        let req: Request<Body> = pr.into();
+        let req: Request<AsyncBody> = pr.into();
         assert_eq!(Method::PATCH, req.method());
         assert_eq!(
             "https://opendal.apache.org/path/to/file",
             req.uri().to_string()
         );
         assert_eq!("123", req.headers().get(CONTENT_LENGTH).unwrap());
         assert_eq!("application/json", req.headers().get(CONTENT_TYPE).unwrap());
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.31.0/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files 15% similar despite different names*

```diff
@@ -14,41 +14,34 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
-use std::fmt::Write;
-use std::str::FromStr;
 use std::sync::Arc;
 
 use async_trait::async_trait;
-use http::header::HeaderName;
-use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
-use http::Request;
-use http::Response;
 use http::StatusCode;
-use http::Uri;
 use log::debug;
+use reqsign::AzureStorageConfig;
+use reqsign::AzureStorageLoader;
 use reqsign::AzureStorageSigner;
 
 use super::batch::parse_batch_delete_response;
-use super::batch::BatchDeleteRequestBuilder;
 use super::error::parse_error;
 use super::pager::AzblobPager;
 use super::writer::AzblobWriter;
 use crate::ops::*;
 use crate::raw::*;
+use crate::services::azblob::core::AzblobCore;
 use crate::types::Metadata;
 use crate::*;
 
-const X_MS_BLOB_TYPE: &str = "x-ms-blob-type";
-
 /// Known endpoint suffix Azure Storage Blob services resource URI syntax.
 /// Azure public cloud: https://accountname.blob.core.windows.net
 /// Azure US Government: https://accountname.blob.core.usgovcloudapi.net
 /// Azure China: https://accountname.blob.core.chinacloudapi.cn
 const KNOWN_AZBLOB_ENDPOINT_SUFFIX: &[&str] = &[
     "blob.core.windows.net",
     "blob.core.usgovcloudapi.net",
@@ -61,14 +54,15 @@
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
+/// - [x] copy
 /// - [x] list
 /// - [x] scan
 /// - [ ] presign
 /// - [ ] blocking
 ///
 /// # Configuration
 ///
@@ -379,72 +373,51 @@
         } else {
             HttpClient::new().map_err(|err| {
                 err.with_operation("Builder::build")
                     .with_context("service", Scheme::Azblob)
             })?
         };
 
-        let mut signer_builder = AzureStorageSigner::builder();
-        let mut account_name: Option<String> = None;
-        if let Some(sas_token) = &self.sas_token {
-            signer_builder.security_token(sas_token);
-            match &self.account_name {
-                Some(name) => account_name = Some(name.clone()),
-                None => {
-                    account_name = infer_storage_name_from_endpoint(endpoint.as_str());
-                }
-            }
-        } else if let (Some(name), Some(key)) = (&self.account_name, &self.account_key) {
-            account_name = Some(name.clone());
-            signer_builder.account_name(name).account_key(key);
-        } else if let Some(key) = &self.account_key {
-            account_name = infer_storage_name_from_endpoint(endpoint.as_str());
-            signer_builder
-                .account_name(account_name.as_ref().unwrap_or(&String::new()))
-                .account_key(key);
-        }
+        let config_loader = AzureStorageConfig {
+            account_name: self
+                .account_name
+                .clone()
+                .or_else(|| infer_storage_name_from_endpoint(endpoint.as_str())),
+            account_key: self.account_key.clone(),
+            sas_token: self.sas_token.clone(),
+        };
 
-        let signer = signer_builder.clone().build().map_err(|e| {
-            Error::new(ErrorKind::ConfigInvalid, "build AzureStorageSigner")
-                .with_operation("Builder::build")
-                .with_context("service", Scheme::Azblob)
-                .with_context("endpoint", &endpoint)
-                .with_context("container", container.as_str())
-                .set_source(e)
-        })?;
-        signer_builder.omit_service_version();
-        let sub_req_signer = signer_builder.build().map_err(|e| {
-            Error::new(ErrorKind::ConfigInvalid, "build AzureStorageSigner")
-                .with_operation("Builder::build")
-                .with_context("service", Scheme::Azblob)
-                .with_context("endpoint", &endpoint)
-                .with_context("container", container.as_str())
-                .set_source(e)
-        })?;
+        let cred_loader = AzureStorageLoader::new(config_loader);
+
+        let signer = AzureStorageSigner::new();
+        let batch_signer = AzureStorageSigner::new().omit_service_version();
 
         debug!("backend build finished: {:?}", &self);
         Ok(AzblobBackend {
-            root,
-            endpoint,
-            signer: Arc::new(signer),
-            batch_signer: Arc::new(sub_req_signer),
-            container: self.container.clone(),
-            client,
-            _account_name: account_name.unwrap_or_default(),
+            core: Arc::new(AzblobCore {
+                root,
+                endpoint,
+                container: self.container.clone(),
+
+                client,
+                loader: cred_loader,
+                signer,
+                batch_signer,
+            }),
         })
     }
 }
 
 fn infer_storage_name_from_endpoint(endpoint: &str) -> Option<String> {
-    let _endpoint: &str = endpoint
+    let endpoint: &str = endpoint
         .strip_prefix("http://")
         .or_else(|| endpoint.strip_prefix("https://"))
         .unwrap_or(endpoint);
 
-    let mut parts = _endpoint.splitn(2, '.');
+    let mut parts = endpoint.splitn(2, '.');
     let storage_name = parts.next();
     let endpoint_suffix = parts
         .next()
         .unwrap_or_default()
         .trim_end_matches('/')
         .to_lowercase();
 
@@ -457,22 +430,15 @@
         None
     }
 }
 
 /// Backend for azblob services.
 #[derive(Debug, Clone)]
 pub struct AzblobBackend {
-    container: String,
-    // TODO: remove pub after https://github.com/apache/incubator-opendal/issues/1427
-    pub client: HttpClient,
-    root: String, // root will be "/" or /abc/
-    endpoint: String,
-    pub signer: Arc<AzureStorageSigner>,
-    pub batch_signer: Arc<AzureStorageSigner>,
-    _account_name: String,
+    core: Arc<AzblobCore>,
 }
 
 #[async_trait]
 impl Accessor for AzblobBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = AzblobWriter;
@@ -482,43 +448,45 @@
 
     fn info(&self) -> AccessorInfo {
         use AccessorCapability::*;
         use AccessorHint::*;
 
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Azblob)
-            .set_root(&self.root)
-            .set_name(&self.container)
+            .set_root(&self.core.root)
+            .set_name(&self.core.container)
             .set_max_batch_operations(AZBLOB_BATCH_LIMIT)
-            .set_capabilities(Read | Write | List | Scan | Batch)
+            .set_capabilities(Read | Write | List | Scan | Batch | Copy)
             .set_hints(ReadStreamable);
 
         am
     }
 
     async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
-        let mut req = self.azblob_put_blob_request(path, Some(0), None, AsyncBody::Empty)?;
+        let mut req = self
+            .core
+            .azblob_put_blob_request(path, Some(0), None, AsyncBody::Empty)?;
 
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
+        self.core.sign(&mut req).await?;
 
-        let resp = self.client.send_async(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(RpCreate::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.azblob_get_blob(path, args.range()).await?;
+        let resp = self.core.azblob_get_blob(path, args.range()).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
 
@@ -534,316 +502,138 @@
                 ErrorKind::Unsupported,
                 "append write is not supported",
             ));
         }
 
         Ok((
             RpWrite::default(),
-            AzblobWriter::new(self.clone(), args, path.to_string()),
+            AzblobWriter::new(self.core.clone(), args, path.to_string()),
         ))
     }
 
+    async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
+        let resp = self.core.azblob_copy_blob(from, to).await?;
+
+        let status = resp.status();
+
+        match status {
+            StatusCode::ACCEPTED => {
+                resp.into_body().consume().await?;
+                Ok(RpCopy::default())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+
     async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.azblob_get_blob_properties(path).await?;
+        let resp = self.core.azblob_get_blob_properties(path).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
                 Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let resp = self.azblob_delete_blob(path).await?;
+        let resp = self.core.azblob_delete_blob(path).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::ACCEPTED | StatusCode::NOT_FOUND => Ok(RpDelete::default()),
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         let op = AzblobPager::new(
-            Arc::new(self.clone()),
-            self.root.clone(),
+            self.core.clone(),
             path.to_string(),
             "/".to_string(),
             args.limit(),
         );
 
         Ok((RpList::default(), op))
     }
 
     async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
         let op = AzblobPager::new(
-            Arc::new(self.clone()),
-            self.root.clone(),
+            self.core.clone(),
             path.to_string(),
             "".to_string(),
             args.limit(),
         );
 
         Ok((RpScan::default(), op))
     }
 
     async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
         let ops = args.into_operation();
-        match ops {
-            BatchOperations::Delete(ops) => {
-                let paths = ops.into_iter().map(|(p, _)| p).collect::<Vec<_>>();
-                if paths.len() > AZBLOB_BATCH_LIMIT {
-                    return Err(Error::new(
-                        ErrorKind::Unsupported,
-                        "batch delete limit exceeded",
-                    ));
-                }
-                // construct and complete batch request
-                let resp = self.azblob_batch_delete(&paths).await?;
-
-                // check response status
-                if resp.status() != StatusCode::ACCEPTED {
-                    return Err(parse_error(resp).await?);
-                }
-
-                // get boundary from response header
-                let content_type = resp.headers().get(CONTENT_TYPE).ok_or_else(|| {
-                    Error::new(
-                        ErrorKind::Unexpected,
-                        "response data should have CONTENT_TYPE header",
-                    )
-                })?;
-                let content_type = content_type
-                    .to_str()
-                    .map(|ty| ty.to_string())
-                    .map_err(|e| {
-                        Error::new(
-                            ErrorKind::Unexpected,
-                            &format!("get invalid CONTENT_TYPE header in response: {:?}", e),
-                        )
-                    })?;
-                let splits = content_type.split("boundary=").collect::<Vec<&str>>();
-                let boundary = splits.get(1).to_owned().ok_or_else(|| {
-                    Error::new(
-                        ErrorKind::Unexpected,
-                        "No boundary message provided in CONTENT_TYPE",
-                    )
-                })?;
-
-                let body = resp.into_body().bytes().await?;
-                let body = String::from_utf8(body.to_vec()).map_err(|e| {
-                    Error::new(
-                        ErrorKind::Unexpected,
-                        &format!("get invalid batch response {e:?}"),
-                    )
-                })?;
-
-                let results = parse_batch_delete_response(boundary, body, paths)?;
-                Ok(RpBatch::new(BatchedResults::Delete(results)))
-            }
-        }
-    }
-}
-
-impl AzblobBackend {
-    async fn azblob_get_blob(
-        &self,
-        path: &str,
-        range: BytesRange,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!(
-            "{}/{}/{}",
-            self.endpoint,
-            self.container,
-            percent_encode_path(&p)
-        );
-
-        let mut req = Request::get(&url);
-
-        if !range.is_full() {
-            // azblob doesn't support read with suffix range.
-            //
-            // ref: https://learn.microsoft.com/en-us/rest/api/storageservices/specifying-the-range-header-for-blob-service-operations
-            if range.offset().is_none() && range.size().is_some() {
-                return Err(Error::new(
-                    ErrorKind::Unsupported,
-                    "azblob doesn't support read with suffix range",
-                ));
-            }
-
-            req = req.header(http::header::RANGE, range.to_header());
-        }
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    pub fn azblob_put_blob_request(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        content_type: Option<&str>,
-        body: AsyncBody,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!(
-            "{}/{}/{}",
-            self.endpoint,
-            self.container,
-            percent_encode_path(&p)
-        );
-
-        let mut req = Request::put(&url);
-
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size)
-        }
-
-        if let Some(ty) = content_type {
-            req = req.header(CONTENT_TYPE, ty)
+        let paths = ops.into_iter().map(|(p, _)| p).collect::<Vec<_>>();
+        if paths.len() > AZBLOB_BATCH_LIMIT {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "batch delete limit exceeded",
+            ));
         }
+        // construct and complete batch request
+        let resp = self.core.azblob_batch_delete(&paths).await?;
 
-        req = req.header(HeaderName::from_static(X_MS_BLOB_TYPE), "BlockBlob");
-
-        // Set body
-        let req = req.body(body).map_err(new_request_build_error)?;
-
-        Ok(req)
-    }
-
-    async fn azblob_get_blob_properties(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!(
-            "{}/{}/{}",
-            self.endpoint,
-            self.container,
-            percent_encode_path(&p)
-        );
-
-        let req = Request::head(&url);
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    async fn azblob_delete_blob(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!(
-            "{}/{}/{}",
-            self.endpoint,
-            self.container,
-            percent_encode_path(&p)
-        );
-
-        let req = Request::delete(&url);
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    pub(crate) async fn azblob_list_blobs(
-        &self,
-        path: &str,
-        next_marker: &str,
-        delimiter: &str,
-        limit: Option<usize>,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let mut url = format!(
-            "{}/{}?restype=container&comp=list",
-            self.endpoint, self.container
-        );
-        if !p.is_empty() {
-            write!(url, "&prefix={}", percent_encode_path(&p))
-                .expect("write into string must succeed");
-        }
-        if let Some(limit) = limit {
-            write!(url, "&maxresults={limit}").expect("write into string must succeed");
-        }
-        if !delimiter.is_empty() {
-            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
+        // check response status
+        if resp.status() != StatusCode::ACCEPTED {
+            return Err(parse_error(resp).await?);
         }
-        if !next_marker.is_empty() {
-            write!(url, "&marker={next_marker}").expect("write into string must succeed");
-        }
-
-        let mut req = Request::get(&url)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    async fn azblob_batch_delete(&self, paths: &[String]) -> Result<Response<IncomingAsyncBody>> {
-        // init batch request
-        let url = format!(
-            "{}/{}?restype=container&comp=batch",
-            self.endpoint, self.container
-        );
-        let mut batch_delete_req_builder = BatchDeleteRequestBuilder::new(&url);
-
-        for path in paths.iter() {
-            // build sub requests
-            let p = build_abs_path(&self.root, path);
-            let encoded_path = percent_encode_path(&p);
-
-            let url = Uri::from_str(&format!(
-                "{}/{}/{}",
-                self.endpoint, self.container, encoded_path
-            ))
-            .unwrap();
-
-            let mut sub_req = Request::delete(&url.to_string())
-                .header(CONTENT_LENGTH, 0)
-                .body(AsyncBody::Empty)
-                .map_err(new_request_build_error)?;
-            self.batch_signer
-                .sign(&mut sub_req)
-                .map_err(new_request_sign_error)?;
 
-            batch_delete_req_builder.append(sub_req);
-        }
+        // get boundary from response header
+        let content_type = resp.headers().get(CONTENT_TYPE).ok_or_else(|| {
+            Error::new(
+                ErrorKind::Unexpected,
+                "response data should have CONTENT_TYPE header",
+            )
+        })?;
+        let content_type = content_type
+            .to_str()
+            .map(|ty| ty.to_string())
+            .map_err(|e| {
+                Error::new(
+                    ErrorKind::Unexpected,
+                    &format!("get invalid CONTENT_TYPE header in response: {:?}", e),
+                )
+            })?;
+        let splits = content_type.split("boundary=").collect::<Vec<&str>>();
+        let boundary = splits.get(1).to_owned().ok_or_else(|| {
+            Error::new(
+                ErrorKind::Unexpected,
+                "No boundary message provided in CONTENT_TYPE",
+            )
+        })?;
 
-        let mut req = batch_delete_req_builder.try_into_req()?;
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
+        let body = resp.into_body().bytes().await?;
+        let body = String::from_utf8(body.to_vec()).map_err(|e| {
+            Error::new(
+                ErrorKind::Unexpected,
+                &format!("get invalid batch response {e:?}"),
+            )
+        })?;
 
-        self.client.send_async(req).await
+        let results = parse_batch_delete_response(boundary, body, paths)?
+            .into_iter()
+            .map(|(path, rp)| (path, rp.map(|v| v.into())))
+            .collect();
+        Ok(RpBatch::new(results))
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::AzblobBuilder;
     use crate::services::azblob::backend::infer_storage_name_from_endpoint;
@@ -870,21 +660,19 @@
         azblob_builder.container("container");
         azblob_builder.account_key("account-key");
         let azblob = azblob_builder
             .build()
             .expect("build azblob should be succeeded.");
 
         assert_eq!(
-            azblob.endpoint,
+            azblob.core.endpoint,
             "https://storagesample.blob.core.chinacloudapi.cn"
         );
 
-        assert_eq!(azblob._account_name, "storagesample".to_string());
-
-        assert_eq!(azblob.container, "container".to_string());
+        assert_eq!(azblob.core.container, "container".to_string());
 
         assert_eq!(
             azblob_builder.account_key.unwrap(),
             "account-key".to_string()
         );
     }
 
@@ -894,21 +682,19 @@
         azblob_builder.endpoint("https://storagesample.blob.core.windows.net");
         azblob_builder.container("container");
         let azblob = azblob_builder
             .build()
             .expect("build azblob should be succeeded.");
 
         assert_eq!(
-            azblob.endpoint,
+            azblob.core.endpoint,
             "https://storagesample.blob.core.windows.net"
         );
 
-        assert_eq!(azblob._account_name, "".to_string());
-
-        assert_eq!(azblob.container, "container".to_string());
+        assert_eq!(azblob.core.container, "container".to_string());
 
         assert_eq!(azblob_builder.account_key, None);
     }
 
     #[test]
     fn test_builder_from_endpoint_and_sas() {
         let mut azblob_builder = AzblobBuilder::default();
@@ -918,21 +704,19 @@
         azblob_builder.account_key("account-key");
         azblob_builder.sas_token("sas");
         let azblob = azblob_builder
             .build()
             .expect("build azblob should be succeeded.");
 
         assert_eq!(
-            azblob.endpoint,
+            azblob.core.endpoint,
             "https://storagesample.blob.core.usgovcloudapi.net"
         );
 
-        assert_eq!(azblob._account_name, "storagesample".to_string());
-
-        assert_eq!(azblob.container, "container".to_string());
+        assert_eq!(azblob.core.container, "container".to_string());
 
         assert_eq!(
             azblob_builder.account_key.unwrap(),
             "account-key".to_string()
         );
 
         assert_eq!(azblob_builder.sas_token.unwrap(), "sas".to_string());
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -15,10 +15,11 @@
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
 pub use backend::AzblobBuilder as Azblob;
 
 mod batch;
+mod core;
 mod error;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files 7% similar despite different names*

```diff
@@ -17,44 +17,40 @@
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Buf;
 use quick_xml::de;
 use serde::Deserialize;
-use time::format_description::well_known::Rfc2822;
-use time::OffsetDateTime;
 
-use super::backend::AzblobBackend;
+use super::core::AzblobCore;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
 pub struct AzblobPager {
-    backend: Arc<AzblobBackend>,
-    root: String,
+    core: Arc<AzblobCore>,
+
     path: String,
     delimiter: String,
     limit: Option<usize>,
 
     next_marker: String,
     done: bool,
 }
 
 impl AzblobPager {
     pub fn new(
-        backend: Arc<AzblobBackend>,
-        root: String,
+        core: Arc<AzblobCore>,
         path: String,
         delimiter: String,
         limit: Option<usize>,
     ) -> Self {
         Self {
-            backend,
-            root,
+            core,
             path,
             delimiter,
             limit,
 
             next_marker: "".to_string(),
             done: false,
         }
@@ -65,15 +61,15 @@
 impl oio::Page for AzblobPager {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         if self.done {
             return Ok(None);
         }
 
         let resp = self
-            .backend
+            .core
             .azblob_list_blobs(&self.path, &self.next_marker, &self.delimiter, self.limit)
             .await?;
 
         if resp.status() != http::StatusCode::OK {
             return Err(parse_error(resp).await?);
         }
 
@@ -92,15 +88,15 @@
         self.next_marker = output.next_marker.clone().unwrap_or_default();
 
         let prefixes = output.blobs.blob_prefix;
         let mut entries = Vec::with_capacity(prefixes.len() + output.blobs.blob.len());
 
         for prefix in prefixes {
             let de = oio::Entry::new(
-                &build_rel_path(&self.root, &prefix.name),
+                &build_rel_path(&self.core.root, &prefix.name),
                 Metadata::new(EntryMode::DIR),
             );
 
             entries.push(de)
         }
 
         for object in output.blobs.blob {
@@ -113,26 +109,19 @@
 
             let meta = Metadata::new(EntryMode::FILE)
                 // Keep fit with ETag header.
                 .with_etag(format!("\"{}\"", object.properties.etag.as_str()))
                 .with_content_length(object.properties.content_length)
                 .with_content_md5(object.properties.content_md5)
                 .with_content_type(object.properties.content_type)
-                .with_last_modified(
-                    OffsetDateTime::parse(object.properties.last_modified.as_str(), &Rfc2822)
-                        .map_err(|e| {
-                            Error::new(
-                                ErrorKind::Unexpected,
-                                "parse last modified RFC2822 datetime",
-                            )
-                            .set_source(e)
-                        })?,
-                );
+                .with_last_modified(parse_datetime_from_rfc2822(
+                    object.properties.last_modified.as_str(),
+                )?);
 
-            let de = oio::Entry::new(&build_rel_path(&self.root, &object.name), meta);
+            let de = oio::Entry::new(&build_rel_path(&self.core.root, &object.name), meta);
 
             entries.push(de);
         }
 
         Ok(Some(entries))
     }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -15,52 +15,49 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::AzblobBackend;
+use super::backend::WebhdfsBackend;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct AzblobWriter {
-    backend: AzblobBackend,
+pub struct WebhdfsWriter {
+    backend: WebhdfsBackend,
 
     op: OpWrite,
     path: String,
 }
 
-impl AzblobWriter {
-    pub fn new(backend: AzblobBackend, op: OpWrite, path: String) -> Self {
-        AzblobWriter { backend, op, path }
+impl WebhdfsWriter {
+    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
+        WebhdfsWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for AzblobWriter {
+impl oio::Write for WebhdfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.backend.azblob_put_blob_request(
-            &self.path,
-            Some(bs.len()),
-            self.op.content_type(),
-            AsyncBody::Bytes(bs),
-        )?;
-
-        self.backend
-            .signer
-            .sign(&mut req)
-            .map_err(new_request_sign_error)?;
+        let req = self
+            .backend
+            .webhdfs_create_object_req(
+                &self.path,
+                Some(bs.len()),
+                self.op.content_type(),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
 
-        let resp = self.backend.client.send_async(req).await?;
+        let resp = self.backend.client.send(req).await?;
 
         let status = resp.status();
-
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files 24% similar despite different names*

```diff
@@ -14,27 +14,24 @@
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
-use std::fmt::Write;
 use std::sync::Arc;
 
 use async_trait::async_trait;
-use http::header::CONTENT_DISPOSITION;
-use http::header::CONTENT_LENGTH;
-use http::header::CONTENT_TYPE;
-use http::Request;
-use http::Response;
 use http::StatusCode;
 use log::debug;
+use reqsign::AzureStorageConfig;
+use reqsign::AzureStorageLoader;
 use reqsign::AzureStorageSigner;
 
+use super::core::AzdfsCore;
 use super::error::parse_error;
 use super::pager::AzdfsPager;
 use super::writer::AzdfsWriter;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
@@ -248,43 +245,36 @@
         } else {
             HttpClient::new().map_err(|err| {
                 err.with_operation("Builder::build")
                     .with_context("service", Scheme::Azdfs)
             })?
         };
 
-        let mut signer_builder = AzureStorageSigner::builder();
-        let mut account_name = None;
-        if let (Some(name), Some(key)) = (&self.account_name, &self.account_key) {
-            account_name = Some(name.clone());
-            signer_builder.account_name(name).account_key(key);
-        } else if let Some(key) = &self.account_key {
-            account_name = infer_storage_name_from_endpoint(endpoint.as_str());
-            signer_builder
-                .account_name(account_name.as_ref().unwrap_or(&String::new()))
-                .account_key(key);
-        }
+        let config_loader = AzureStorageConfig {
+            account_name: self
+                .account_name
+                .clone()
+                .or_else(|| infer_storage_name_from_endpoint(endpoint.as_str())),
+            account_key: self.account_key.clone(),
+            sas_token: None,
+        };
 
-        let signer = signer_builder.build().map_err(|e| {
-            Error::new(ErrorKind::ConfigInvalid, "build AzureStorageSigner")
-                .with_operation("Builder::build")
-                .with_context("service", Scheme::Azdfs)
-                .with_context("endpoint", &endpoint)
-                .with_context("container", filesystem.as_str())
-                .set_source(e)
-        })?;
+        let cred_loader = AzureStorageLoader::new(config_loader);
+        let signer = AzureStorageSigner::new();
 
         debug!("backend build finished: {:?}", &self);
         Ok(AzdfsBackend {
-            root,
-            endpoint,
-            signer: Arc::new(signer),
-            filesystem: self.filesystem.clone(),
-            client,
-            _account_name: account_name.unwrap_or_default(),
+            core: Arc::new(AzdfsCore {
+                filesystem: self.filesystem.clone(),
+                root,
+                endpoint,
+                client,
+                loader: cred_loader,
+                signer,
+            }),
         })
     }
 
     fn from_map(map: HashMap<String, String>) -> Self {
         let mut builder = AzdfsBuilder::default();
 
         map.get("root").map(|v| builder.root(v));
@@ -296,37 +286,31 @@
         builder
     }
 }
 
 /// Backend for azblob services.
 #[derive(Debug, Clone)]
 pub struct AzdfsBackend {
-    filesystem: String,
-    // TODO: remove pub after https://github.com/apache/incubator-opendal/issues/1427
-    pub client: HttpClient,
-    root: String, // root will be "/" or /abc/
-    endpoint: String,
-    pub signer: Arc<AzureStorageSigner>,
-    _account_name: String,
+    core: Arc<AzdfsCore>,
 }
 
 #[async_trait]
 impl Accessor for AzdfsBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = AzdfsWriter;
     type BlockingWriter = ();
     type Pager = AzdfsPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Azdfs)
-            .set_root(&self.root)
-            .set_name(&self.filesystem)
+            .set_root(&self.core.root)
+            .set_name(&self.core.filesystem)
             .set_capabilities(
                 AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
             )
             .set_hints(AccessorHint::ReadStreamable);
 
         am
     }
@@ -334,33 +318,35 @@
     async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
         let resource = match args.mode() {
             EntryMode::FILE => "file",
             EntryMode::DIR => "directory",
             _ => unimplemented!("not supported object mode"),
         };
 
-        let mut req = self.azdfs_create_request(path, resource, None, None, AsyncBody::Empty)?;
+        let mut req =
+            self.core
+                .azdfs_create_request(path, resource, None, None, AsyncBody::Empty)?;
 
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
+        self.core.sign(&mut req).await?;
 
-        let resp = self.client.send_async(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(RpCreate::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.azdfs_read(path, args.range()).await?;
+        let resp = self.core.azdfs_read(path, args.range()).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
@@ -375,259 +361,62 @@
                 ErrorKind::Unsupported,
                 "append write is not supported",
             ));
         }
 
         Ok((
             RpWrite::default(),
-            AzdfsWriter::new(self.clone(), args, path.to_string()),
+            AzdfsWriter::new(self.core.clone(), args, path.to_string()),
         ))
     }
 
     async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.azdfs_get_properties(path).await?;
+        let resp = self.core.azdfs_get_properties(path).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
                 Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let resp = self.azdfs_delete(path).await?;
+        let resp = self.core.azdfs_delete(path).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::NOT_FOUND => Ok(RpDelete::default()),
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
-        let op = AzdfsPager::new(
-            Arc::new(self.clone()),
-            self.root.clone(),
-            path.to_string(),
-            args.limit(),
-        );
+        let op = AzdfsPager::new(self.core.clone(), path.to_string(), args.limit());
 
         Ok((RpList::default(), op))
     }
 }
 
-impl AzdfsBackend {
-    async fn azdfs_read(
-        &self,
-        path: &str,
-        range: BytesRange,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!(
-            "{}/{}/{}",
-            self.endpoint,
-            self.filesystem,
-            percent_encode_path(&p)
-        );
-
-        let mut req = Request::get(&url);
-
-        if !range.is_full() {
-            // azblob doesn't support read with suffix range.
-            //
-            // ref: https://learn.microsoft.com/en-us/rest/api/storageservices/specifying-the-range-header-for-blob-service-operations
-            if range.offset().is_none() && range.size().is_some() {
-                return Err(Error::new(
-                    ErrorKind::Unsupported,
-                    "azblob doesn't support read with suffix range",
-                ));
-            }
-
-            req = req.header(http::header::RANGE, range.to_header());
-        }
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    /// resource should be one of `file` or `directory`
-    ///
-    /// ref: https://learn.microsoft.com/en-us/rest/api/storageservices/datalakestoragegen2/path/create
-    pub fn azdfs_create_request(
-        &self,
-        path: &str,
-        resource: &str,
-        content_type: Option<&str>,
-        content_disposition: Option<&str>,
-        body: AsyncBody,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path)
-            .trim_end_matches('/')
-            .to_string();
-
-        let url = format!(
-            "{}/{}/{}?resource={resource}",
-            self.endpoint,
-            self.filesystem,
-            percent_encode_path(&p)
-        );
-
-        let mut req = Request::put(&url);
-
-        // Content length must be 0 for create request.
-        req = req.header(CONTENT_LENGTH, 0);
-
-        if let Some(ty) = content_type {
-            req = req.header(CONTENT_TYPE, ty)
-        }
-
-        if let Some(pos) = content_disposition {
-            req = req.header(CONTENT_DISPOSITION, pos)
-        }
-
-        // Set body
-        let req = req.body(body).map_err(new_request_build_error)?;
-
-        Ok(req)
-    }
-
-    /// ref: https://learn.microsoft.com/en-us/rest/api/storageservices/datalakestoragegen2/path/update
-    pub fn azdfs_update_request(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        body: AsyncBody,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        // - close: Make this is the final action to this file.
-        // - flush: Flush the file directly.
-        let url = format!(
-            "{}/{}/{}?action=append&close=true&flush=true&position=0",
-            self.endpoint,
-            self.filesystem,
-            percent_encode_path(&p)
-        );
-
-        let mut req = Request::patch(&url);
-
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size)
-        }
-
-        // Set body
-        let req = req.body(body).map_err(new_request_build_error)?;
-
-        Ok(req)
-    }
-
-    async fn azdfs_get_properties(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path)
-            .trim_end_matches('/')
-            .to_string();
-
-        let url = format!(
-            "{}/{}/{}?action=getStatus",
-            self.endpoint,
-            self.filesystem,
-            percent_encode_path(&p)
-        );
-
-        let req = Request::head(&url);
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    async fn azdfs_delete(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path)
-            .trim_end_matches('/')
-            .to_string();
-
-        let url = format!(
-            "{}/{}/{}",
-            self.endpoint,
-            self.filesystem,
-            percent_encode_path(&p)
-        );
-
-        let req = Request::delete(&url);
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    pub(crate) async fn azdfs_list(
-        &self,
-        path: &str,
-        continuation: &str,
-        limit: Option<usize>,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path)
-            .trim_end_matches('/')
-            .to_string();
-
-        let mut url = format!(
-            "{}/{}?resource=filesystem&recursive=false",
-            self.endpoint, self.filesystem
-        );
-        if !p.is_empty() {
-            write!(url, "&directory={}", percent_encode_path(&p))
-                .expect("write into string must succeed");
-        }
-        if let Some(limit) = limit {
-            write!(url, "&maxresults={limit}").expect("write into string must succeed");
-        }
-        if !continuation.is_empty() {
-            write!(url, "&continuation={continuation}").expect("write into string must succeed");
-        }
-
-        let mut req = Request::get(&url)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-}
-
 fn infer_storage_name_from_endpoint(endpoint: &str) -> Option<String> {
-    let _endpoint: &str = endpoint
+    let endpoint: &str = endpoint
         .strip_prefix("http://")
         .or_else(|| endpoint.strip_prefix("https://"))
         .unwrap_or(endpoint);
 
-    let mut parts = _endpoint.splitn(2, '.');
+    let mut parts = endpoint.splitn(2, '.');
     let storage_name = parts.next();
     let endpoint_suffix = parts
         .next()
         .unwrap_or_default()
         .trim_end_matches('/')
         .to_lowercase();
 
@@ -668,21 +457,19 @@
         azdfs_builder.account_key("account-key");
         azdfs_builder.filesystem("filesystem");
         let azdfs = azdfs_builder
             .build()
             .expect("build azdfs should be succeeded.");
 
         assert_eq!(
-            azdfs.endpoint,
+            azdfs.core.endpoint,
             "https://storagesample.dfs.core.chinacloudapi.cn"
         );
 
-        assert_eq!(azdfs._account_name, "storagesample".to_string());
-
-        assert_eq!(azdfs.filesystem, "filesystem".to_string());
+        assert_eq!(azdfs.core.filesystem, "filesystem".to_string());
 
         assert_eq!(
             azdfs_builder.account_key.unwrap(),
             "account-key".to_string()
         );
     }
 
@@ -691,16 +478,17 @@
         let mut azdfs_builder = AzdfsBuilder::default();
         azdfs_builder.endpoint("https://storagesample.dfs.core.windows.net");
         azdfs_builder.filesystem("filesystem");
         let azdfs = azdfs_builder
             .build()
             .expect("build azdfs should be succeeded.");
 
-        assert_eq!(azdfs.endpoint, "https://storagesample.dfs.core.windows.net");
-
-        assert_eq!(azdfs._account_name, "".to_string());
+        assert_eq!(
+            azdfs.core.endpoint,
+            "https://storagesample.dfs.core.windows.net"
+        );
 
-        assert_eq!(azdfs.filesystem, "filesystem".to_string());
+        assert_eq!(azdfs.core.filesystem, "filesystem".to_string());
 
         assert_eq!(azdfs_builder.account_key, None);
     }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::AzdfsBuilder as Azdfs;
+pub use backend::FsBuilder as Fs;
 
 mod error;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files 16% similar despite different names*

```diff
@@ -16,42 +16,34 @@
 // under the License.
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use serde::Deserialize;
 use serde_json::de;
-use time::format_description::well_known::Rfc2822;
-use time::OffsetDateTime;
 
-use super::backend::AzdfsBackend;
+use super::core::AzdfsCore;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
 pub struct AzdfsPager {
-    backend: Arc<AzdfsBackend>,
-    root: String,
+    core: Arc<AzdfsCore>,
+
     path: String,
     limit: Option<usize>,
 
     continuation: String,
     done: bool,
 }
 
 impl AzdfsPager {
-    pub fn new(
-        backend: Arc<AzdfsBackend>,
-        root: String,
-        path: String,
-        limit: Option<usize>,
-    ) -> Self {
+    pub fn new(core: Arc<AzdfsCore>, path: String, limit: Option<usize>) -> Self {
         Self {
-            backend,
-            root,
+            core,
             path,
             limit,
 
             continuation: "".to_string(),
             done: false,
         }
     }
@@ -61,15 +53,15 @@
 impl oio::Page for AzdfsPager {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         if self.done {
             return Ok(None);
         }
 
         let resp = self
-            .backend
+            .core
             .azdfs_list(&self.path, &self.continuation, self.limit)
             .await?;
 
         // Azdfs will return not found for not-exist path.
         if resp.status() == http::StatusCode::NOT_FOUND {
             resp.into_body().consume().await?;
             return Ok(None);
@@ -109,25 +101,17 @@
             let meta = Metadata::new(mode)
                 // Keep fit with ETag header.
                 .with_etag(format!("\"{}\"", &object.etag))
                 .with_content_length(object.content_length.parse().map_err(|err| {
                     Error::new(ErrorKind::Unexpected, "content length is not valid integer")
                         .set_source(err)
                 })?)
-                .with_last_modified(
-                    OffsetDateTime::parse(&object.last_modified, &Rfc2822).map_err(|e| {
-                        Error::new(
-                            ErrorKind::Unexpected,
-                            "last modified is not valid RFC2822 datetime",
-                        )
-                        .set_source(e)
-                    })?,
-                );
+                .with_last_modified(parse_datetime_from_rfc2822(&object.last_modified)?);
 
-            let mut path = build_rel_path(&self.root, &object.name);
+            let mut path = build_rel_path(&self.core.root, &object.name);
             if mode == EntryMode::DIR {
                 path += "/"
             };
 
             let de = oio::Entry::new(&path, meta);
 
             entries.push(de);
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files 8% similar despite different names*

```diff
@@ -11,77 +11,73 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::AzdfsBackend;
+use super::core::AzdfsCore;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct AzdfsWriter {
-    backend: AzdfsBackend,
+    core: Arc<AzdfsCore>,
 
     op: OpWrite,
     path: String,
 }
 
 impl AzdfsWriter {
-    pub fn new(backend: AzdfsBackend, op: OpWrite, path: String) -> Self {
-        AzdfsWriter { backend, op, path }
+    pub fn new(core: Arc<AzdfsCore>, op: OpWrite, path: String) -> Self {
+        AzdfsWriter { core, op, path }
     }
 }
 
 #[async_trait]
 impl oio::Write for AzdfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.backend.azdfs_create_request(
+        let mut req = self.core.azdfs_create_request(
             &self.path,
             "file",
             self.op.content_type(),
             self.op.content_disposition(),
             AsyncBody::Empty,
         )?;
 
-        self.backend
-            .signer
-            .sign(&mut req)
-            .map_err(new_request_sign_error)?;
+        self.core.sign(&mut req).await?;
 
-        let resp = self.backend.client.send_async(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
             }
             _ => {
                 return Err(parse_error(resp)
                     .await?
                     .with_operation("Backend::azdfs_create_request"));
             }
         }
 
         let mut req =
-            self.backend
+            self.core
                 .azdfs_update_request(&self.path, Some(bs.len()), AsyncBody::Bytes(bs))?;
 
-        self.backend
-            .signer
-            .sign(&mut req)
-            .map_err(new_request_sign_error)?;
+        self.core.sign(&mut req).await?;
 
-        let resp = self.backend.client.send_async(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
         match status {
             StatusCode::OK | StatusCode::ACCEPTED => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 use std::io;
 use std::io::SeekFrom;
 use std::path::Path;
 use std::path::PathBuf;
 
 use async_compat::Compat;
 use async_trait::async_trait;
+use chrono::DateTime;
 use log::debug;
-use time::OffsetDateTime;
 use tokio::fs;
 use uuid::Uuid;
 
 use super::error::parse_io_error;
 use super::pager::FsPager;
 use super::writer::FsWriter;
 use crate::ops::*;
@@ -40,14 +40,16 @@
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
+/// - [x] copy
+/// - [x] rename
 /// - [x] list
 /// - [ ] ~~scan~~
 /// - [ ] ~~presign~~
 /// - [x] blocking
 ///
 /// # Configuration
 ///
@@ -297,14 +299,16 @@
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Fs)
             .set_root(&self.root.to_string_lossy())
             .set_capabilities(
                 AccessorCapability::Read
                     | AccessorCapability::Write
+                    | AccessorCapability::Copy
+                    | AccessorCapability::Rename
                     | AccessorCapability::List
                     | AccessorCapability::Blocking,
             )
             .set_hints(AccessorHint::ReadSeekable);
 
         am
     }
@@ -437,14 +441,40 @@
             .open(tmp_path.as_ref().unwrap_or(&target_path))
             .await
             .map_err(parse_io_error)?;
 
         Ok((RpWrite::new(), FsWriter::new(target_path, tmp_path, f)))
     }
 
+    async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
+        let from = self.root.join(from.trim_end_matches('/'));
+
+        // try to get the metadata of the source file to ensure it exists
+        tokio::fs::metadata(&from).await.map_err(parse_io_error)?;
+
+        let to = Self::ensure_write_abs_path(&self.root, to.trim_end_matches('/')).await?;
+
+        tokio::fs::copy(from, to).await.map_err(parse_io_error)?;
+
+        Ok(RpCopy::default())
+    }
+
+    async fn rename(&self, from: &str, to: &str, _args: OpRename) -> Result<RpRename> {
+        let from = self.root.join(from.trim_end_matches('/'));
+
+        // try to get the metadata of the source file to ensure it exists
+        tokio::fs::metadata(&from).await.map_err(parse_io_error)?;
+
+        let to = Self::ensure_write_abs_path(&self.root, to.trim_end_matches('/')).await?;
+
+        tokio::fs::rename(from, to).await.map_err(parse_io_error)?;
+
+        Ok(RpRename::default())
+    }
+
     async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
         let p = self.root.join(path.trim_end_matches('/'));
 
         let meta = tokio::fs::metadata(&p).await.map_err(parse_io_error)?;
 
         if self.enable_path_check && meta.is_dir() != path.ends_with('/') {
             return Err(Error::new(
@@ -460,15 +490,15 @@
         } else {
             EntryMode::Unknown
         };
         let m = Metadata::new(mode)
             .with_content_length(meta.len())
             .with_last_modified(
                 meta.modified()
-                    .map(OffsetDateTime::from)
+                    .map(DateTime::from)
                     .map_err(parse_io_error)?,
             );
 
         Ok(RpStat::new(m))
     }
 
     async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
@@ -623,14 +653,40 @@
             .write(true)
             .open(tmp_path.as_ref().unwrap_or(&target_path))
             .map_err(parse_io_error)?;
 
         Ok((RpWrite::new(), FsWriter::new(target_path, tmp_path, f)))
     }
 
+    fn blocking_copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
+        let from = self.root.join(from.trim_end_matches('/'));
+
+        // try to get the metadata of the source file to ensure it exists
+        std::fs::metadata(&from).map_err(parse_io_error)?;
+
+        let to = Self::blocking_ensure_write_abs_path(&self.root, to.trim_end_matches('/'))?;
+
+        std::fs::copy(from, to).map_err(parse_io_error)?;
+
+        Ok(RpCopy::default())
+    }
+
+    fn blocking_rename(&self, from: &str, to: &str, _args: OpRename) -> Result<RpRename> {
+        let from = self.root.join(from.trim_end_matches('/'));
+
+        // try to get the metadata of the source file to ensure it exists
+        std::fs::metadata(&from).map_err(parse_io_error)?;
+
+        let to = Self::blocking_ensure_write_abs_path(&self.root, to.trim_end_matches('/'))?;
+
+        std::fs::rename(from, to).map_err(parse_io_error)?;
+
+        Ok(RpRename::default())
+    }
+
     fn blocking_stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
         let p = self.root.join(path.trim_end_matches('/'));
 
         let meta = std::fs::metadata(p).map_err(parse_io_error)?;
 
         if self.enable_path_check && meta.is_dir() != path.ends_with('/') {
             return Err(Error::new(
@@ -646,15 +702,15 @@
         } else {
             EntryMode::Unknown
         };
         let m = Metadata::new(mode)
             .with_content_length(meta.len())
             .with_last_modified(
                 meta.modified()
-                    .map(OffsetDateTime::from)
+                    .map(DateTime::from)
                     .map_err(parse_io_error)?,
             );
 
         Ok(RpStat::new(m))
     }
 
     fn blocking_delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -12,12 +12,8 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::FsBuilder as Fs;
-
-mod error;
-mod pager;
-mod writer;
+pub use backend::RedisBuilder as Redis;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 use log::debug;
 use suppaftp::list::File;
 use suppaftp::types::FileType;
 use suppaftp::types::Response;
 use suppaftp::FtpError;
 use suppaftp::FtpStream;
 use suppaftp::Status;
-use time::OffsetDateTime;
 use tokio::sync::OnceCell;
 
 use super::pager::FtpPager;
 use super::util::FtpReader;
 use super::writer::FtpWriter;
 use crate::ops::*;
 use crate::raw::*;
@@ -415,15 +414,15 @@
         } else if file.is_directory() {
             EntryMode::DIR
         } else {
             EntryMode::Unknown
         };
         let mut meta = Metadata::new(mode);
         meta.set_content_length(file.size() as u64);
-        meta.set_last_modified(OffsetDateTime::from(file.modified()));
+        meta.set_last_modified(file.modified().into());
 
         Ok(RpStat::new(meta))
     }
 
     async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
         let mut ftp_stream = self.ftp_connect(Operation::Delete).await?;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 use std::str;
 use std::str::FromStr;
 use std::vec::IntoIter;
 
 use async_trait::async_trait;
 use suppaftp::list::File;
-use time::OffsetDateTime;
 
 use crate::raw::*;
 use crate::*;
 
 pub struct FtpPager {
     path: String,
     size: usize,
@@ -58,15 +57,15 @@
             let path = self.path.to_string() + de.name();
 
             let d = if de.is_file() {
                 oio::Entry::new(
                     &path,
                     Metadata::new(EntryMode::FILE)
                         .with_content_length(de.size() as u64)
-                        .with_last_modified(OffsetDateTime::from(de.modified())),
+                        .with_last_modified(de.modified().into()),
                 )
             } else if de.is_directory() {
                 oio::Entry::new(&format!("{}/", &path), Metadata::new(EntryMode::DIR))
             } else {
                 oio::Entry::new(&path, Metadata::new(EntryMode::Unknown))
             };
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 15% similar despite different names*

```diff
@@ -12,680 +12,558 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
+use std::collections::HashSet;
 use std::fmt::Debug;
 use std::fmt::Formatter;
-use std::fmt::Write;
 use std::sync::Arc;
 
 use async_trait::async_trait;
-use http::header::CONTENT_LENGTH;
-use http::header::CONTENT_TYPE;
-use http::Request;
-use http::Response;
+use bytes::Buf;
 use http::StatusCode;
+use http::Uri;
 use log::debug;
-use reqsign::GoogleSigner;
-use serde::Deserialize;
-use serde_json;
-use time::format_description::well_known::Rfc3339;
-use time::OffsetDateTime;
+use reqsign::AliyunConfig;
+use reqsign::AliyunLoader;
+use reqsign::AliyunOssSigner;
 
+use super::core::*;
 use super::error::parse_error;
-use super::pager::GcsPager;
-use super::uri::percent_encode_path;
-use super::writer::GcsWriter;
+use super::pager::OssPager;
+use super::writer::OssWriter;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
-const DEFAULT_GCS_ENDPOINT: &str = "https://storage.googleapis.com";
-const DEFAULT_GCS_SCOPE: &str = "https://www.googleapis.com/auth/devstorage.read_write";
-
-/// Google Cloud Storage service.
+/// Aliyun Object Storage Service (OSS) support
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
+/// - [x] copy
 /// - [x] list
 /// - [x] scan
 /// - [ ] presign
 /// - [ ] blocking
 ///
 /// # Configuration
 ///
-/// - `root`: Set the work directory for backend
-/// - `bucket`: Set the container name for backend
-/// - `endpoint`: Customizable endpoint setting
-/// - `credentials`: Credential string for GCS OAuth2
+/// - `root`: Set the work dir for backend.
+/// - `bucket`: Set the container name for backend.
+/// - `endpoint`: Set the endpoint for backend.
+/// - `presign_endpoint`: Set the endpoint for presign.
+/// - `access_key_id`: Set the access_key_id for backend.
+/// - `access_key_secret`: Set the access_key_secret for backend.
+/// - `role_arn`: Set the role of backend.
+/// - `oidc_token`: Set the oidc_token for backend.
+/// - `allow_anonymous`: Set the backend access OSS in anonymous way.
 ///
-/// You can refer to [`GcsBuilder`]'s docs for more information
+/// Refer to [`OssBuilder`]'s public API docs for more information.
 ///
 /// # Example
 ///
 /// ## Via Builder
 ///
 /// ```no_run
+/// use std::sync::Arc;
+///
 /// use anyhow::Result;
-/// use opendal::services::Gcs;
+/// use opendal::services::Oss;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
-///     // create backend builder
-///     let mut builder = Gcs::default();
-///
-///     // set the storage bucket for OpenDAL
-///     builder.bucket("test");
-///     // set the working directory root for GCS
-///     // all operations will happen within it
+///     // Create OSS backend builder.
+///     let mut builder = Oss::default();
+///     // Set the root for oss, all operations will happen under this root.
+///     //
+///     // NOTE: the root must be absolute path.
 ///     builder.root("/path/to/dir");
-///     // set the credentials for GCS OAUTH2 authentication
-///     builder.credential("authentication token");
+///     // Set the bucket name, this is required.
+///     builder.bucket("test");
+///     // Set the endpoint.
+///     //
+///     // For example:
+///     // - "https://oss-ap-northeast-1.aliyuncs.com"
+///     // - "https://oss-hangzhou.aliyuncs.com"
+///     builder.endpoint("https://oss-cn-beijing.aliyuncs.com");
+///     // Set the access_key_id and access_key_secret.
+///     //
+///     // OpenDAL will try load credential from the env.
+///     // If credential not set and no valid credential in env, OpenDAL will
+///     // send request without signing like anonymous user.
+///     builder.access_key_id("access_key_id");
+///     builder.access_key_secret("access_key_secret");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
+///
 ///     Ok(())
 /// }
 /// ```
-#[derive(Clone, Default)]
-pub struct GcsBuilder {
-    /// root URI, all operations happens under `root`
+#[derive(Default)]
+pub struct OssBuilder {
     root: Option<String>,
-    /// bucket name
-    bucket: String,
-    /// endpoint URI of GCS service,
-    /// default is `https://storage.googleapis.com`
+
     endpoint: Option<String>,
-    /// Scope for gcs.
-    scope: Option<String>,
-    /// Service Account for gcs.
-    service_account: Option<String>,
-
-    /// credential string for GCS service
-    credential: Option<String>,
-    /// credential path for GCS service.
-    credential_path: Option<String>,
+    presign_endpoint: Option<String>,
+    bucket: String,
+
+    // authenticate options
+    access_key_id: Option<String>,
+    access_key_secret: Option<String>,
 
     http_client: Option<HttpClient>,
-    signer: Option<Arc<GoogleSigner>>,
 }
 
-impl GcsBuilder {
-    /// set the working directory root of backend
+impl Debug for OssBuilder {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+        let mut d = f.debug_struct("Builder");
+        d.field("root", &self.root)
+            .field("bucket", &self.bucket)
+            .field("endpoint", &self.endpoint);
+
+        d.finish_non_exhaustive()
+    }
+}
+
+impl OssBuilder {
+    /// Set root of this backend.
+    ///
+    /// All operations will happen under this root.
     pub fn root(&mut self, root: &str) -> &mut Self {
-        if !root.is_empty() {
-            self.root = Some(root.to_string())
-        }
+        self.root = if root.is_empty() {
+            None
+        } else {
+            Some(root.to_string())
+        };
 
         self
     }
 
-    /// set the container's name
+    /// Set bucket name of this backend.
     pub fn bucket(&mut self, bucket: &str) -> &mut Self {
         self.bucket = bucket.to_string();
-        self
-    }
 
-    /// set the GCS service scope
-    ///
-    /// If not set, we will use `https://www.googleapis.com/auth/devstorage.read_write`.
-    ///
-    /// # Valid scope examples
-    ///
-    /// - read-only: `https://www.googleapis.com/auth/devstorage.read_only`
-    /// - read-write: `https://www.googleapis.com/auth/devstorage.read_write`
-    /// - full-control: `https://www.googleapis.com/auth/devstorage.full_control`
-    ///
-    /// Reference: [Cloud Storage authentication](https://cloud.google.com/storage/docs/authentication)
-    pub fn scope(&mut self, scope: &str) -> &mut Self {
-        if !scope.is_empty() {
-            self.scope = Some(scope.to_string())
-        };
         self
     }
 
-    /// Set the GCS service account.
-    ///
-    /// service account will be used for fetch token from vm metadata.
-    /// If not set, we will try to fetch with `default` service account.
-    pub fn service_account(&mut self, service_account: &str) -> &mut Self {
-        if !service_account.is_empty() {
-            self.service_account = Some(service_account.to_string())
-        };
+    /// Set endpoint of this backend.
+    pub fn endpoint(&mut self, endpoint: &str) -> &mut Self {
+        if !endpoint.is_empty() {
+            // Trim trailing `/` so that we can accept `http://127.0.0.1:9000/`
+            self.endpoint = Some(endpoint.trim_end_matches('/').to_string())
+        }
+
         self
     }
 
-    /// set the endpoint GCS service uses
-    pub fn endpoint(&mut self, endpoint: &str) -> &mut Self {
+    /// Set a endpoint for generating presigned urls.
+    ///
+    /// You can offer a public endpoint like <https://oss-cn-beijing.aliyuncs.com> to return a presinged url for
+    /// public accessors, along with an internal endpoint like <https://oss-cn-beijing-internal.aliyuncs.com>
+    /// to access objects in a faster path.
+    ///
+    /// - If presign_endpoint is set, we will use presign_endpoint on generating presigned urls.
+    /// - if not, we will use endpoint as default.
+    pub fn presign_endpoint(&mut self, endpoint: &str) -> &mut Self {
         if !endpoint.is_empty() {
-            self.endpoint = Some(endpoint.to_string())
-        };
+            // Trim trailing `/` so that we can accept `http://127.0.0.1:9000/`
+            self.presign_endpoint = Some(endpoint.trim_end_matches('/').to_string())
+        }
+
         self
     }
 
-    /// set the base64 hashed credentials string used for OAuth2
-    pub fn credential(&mut self, credential: &str) -> &mut Self {
-        if !credential.is_empty() {
-            self.credential = Some(credential.to_string())
-        };
+    /// Set access_key_id of this backend.
+    ///
+    /// - If access_key_id is set, we will take user's input first.
+    /// - If not, we will try to load it from environment.
+    pub fn access_key_id(&mut self, v: &str) -> &mut Self {
+        if !v.is_empty() {
+            self.access_key_id = Some(v.to_string())
+        }
+
         self
     }
 
-    /// set the credentials path of GCS.
-    pub fn credential_path(&mut self, path: &str) -> &mut Self {
-        if !path.is_empty() {
-            self.credential_path = Some(path.to_string())
-        };
+    /// Set access_key_secret of this backend.
+    ///
+    /// - If access_key_secret is set, we will take user's input first.
+    /// - If not, we will try to load it from environment.
+    pub fn access_key_secret(&mut self, v: &str) -> &mut Self {
+        if !v.is_empty() {
+            self.access_key_secret = Some(v.to_string())
+        }
+
         self
     }
 
     /// Specify the http client that used by this service.
     ///
     /// # Notes
     ///
     /// This API is part of OpenDAL's Raw API. `HttpClient` could be changed
     /// during minor updates.
     pub fn http_client(&mut self, client: HttpClient) -> &mut Self {
         self.http_client = Some(client);
         self
     }
 
-    /// Specify the signer directly instead of building by OpenDAL.
-    ///
-    /// If signer is specified, the following settings will not be used
-    /// any more:
-    ///
-    /// - `scope`
-    /// - `service_account`
-    /// - `credential`
-    /// - `credential_path`
-    ///
-    /// PLEASE USE THIS API CAREFULLY.
-    pub fn signer(&mut self, signer: GoogleSigner) -> &mut Self {
-        self.signer = Some(Arc::new(signer));
-        self
-    }
-}
-
-impl Debug for GcsBuilder {
-    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        let mut ds = f.debug_struct("Builder");
-
-        ds.field("root", &self.root)
-            .field("bucket", &self.bucket)
-            .field("endpoint", &self.endpoint);
-        if self.credential.is_some() {
-            ds.field("credentials", &"<redacted>");
-        }
-        ds.finish()
+    /// preprocess the endpoint option
+    fn parse_endpoint(&self, endpoint: &Option<String>, bucket: &str) -> Result<(String, String)> {
+        let (endpoint, host) = match endpoint.clone() {
+            Some(ep) => {
+                let uri = ep.parse::<Uri>().map_err(|err| {
+                    Error::new(ErrorKind::ConfigInvalid, "endpoint is invalid")
+                        .with_context("service", Scheme::Oss)
+                        .with_context("endpoint", &ep)
+                        .set_source(err)
+                })?;
+                let host = uri.host().ok_or_else(|| {
+                    Error::new(ErrorKind::ConfigInvalid, "endpoint host is empty")
+                        .with_context("service", Scheme::Oss)
+                        .with_context("endpoint", &ep)
+                })?;
+                let full_host = format!("{bucket}.{host}");
+                let endpoint = match uri.scheme_str() {
+                    Some(scheme_str) => match scheme_str {
+                        "http" | "https" => format!("{scheme_str}://{full_host}"),
+                        _ => {
+                            return Err(Error::new(
+                                ErrorKind::ConfigInvalid,
+                                "endpoint protocol is invalid",
+                            )
+                            .with_context("service", Scheme::Oss));
+                        }
+                    },
+                    None => format!("https://{full_host}"),
+                };
+                (endpoint, full_host)
+            }
+            None => {
+                return Err(Error::new(ErrorKind::ConfigInvalid, "endpoint is empty")
+                    .with_context("service", Scheme::Oss));
+            }
+        };
+        Ok((endpoint, host))
     }
 }
 
-impl Builder for GcsBuilder {
-    const SCHEME: Scheme = Scheme::Gcs;
-    type Accessor = GcsBackend;
+impl Builder for OssBuilder {
+    const SCHEME: Scheme = Scheme::Oss;
+    type Accessor = OssBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
-        let mut builder = GcsBuilder::default();
+        let mut builder = OssBuilder::default();
 
         map.get("root").map(|v| builder.root(v));
         map.get("bucket").map(|v| builder.bucket(v));
         map.get("endpoint").map(|v| builder.endpoint(v));
-        map.get("credential").map(|v| builder.credential(v));
-        map.get("scope").map(|v| builder.scope(v));
+        map.get("presign_endpoint")
+            .map(|v| builder.presign_endpoint(v));
+        map.get("access_key_id").map(|v| builder.access_key_id(v));
+        map.get("access_key_secret")
+            .map(|v| builder.access_key_secret(v));
 
         builder
     }
 
     fn build(&mut self) -> Result<Self::Accessor> {
-        debug!("backend build started: {:?}", self);
+        debug!("backend build started: {:?}", &self);
 
-        let root = normalize_root(&self.root.take().unwrap_or_default());
-        debug!("backend use root {}", root);
+        let root = normalize_root(&self.root.clone().unwrap_or_default());
+        debug!("backend use root {}", &root);
 
-        // Handle endpoint and bucket name
+        // Handle endpoint, region and bucket name.
         let bucket = match self.bucket.is_empty() {
             false => Ok(&self.bucket),
             true => Err(
                 Error::new(ErrorKind::ConfigInvalid, "The bucket is misconfigured")
-                    .with_operation("Builder::build")
-                    .with_context("service", Scheme::Gcs),
+                    .with_context("service", Scheme::Oss),
             ),
         }?;
 
-        // TODO: server side encryption
-
         let client = if let Some(client) = self.http_client.take() {
             client
         } else {
             HttpClient::new().map_err(|err| {
                 err.with_operation("Builder::build")
-                    .with_context("service", Scheme::Gcs)
+                    .with_context("service", Scheme::Oss)
             })?
         };
 
-        let endpoint = self
-            .endpoint
-            .clone()
-            .unwrap_or_else(|| DEFAULT_GCS_ENDPOINT.to_string());
-
-        debug!("backend use endpoint: {endpoint}");
+        // Retrieve endpoint and host by parsing the endpoint option and bucket. If presign_endpoint is not
+        // set, take endpoint as default presign_endpoint.
+        let (endpoint, host) = self.parse_endpoint(&self.endpoint, bucket)?;
+        debug!("backend use bucket {}, endpoint: {}", &bucket, &endpoint);
 
-        let signer = if let Some(signer) = &self.signer {
-            signer.clone()
+        let presign_endpoint = if self.presign_endpoint.is_some() {
+            self.parse_endpoint(&self.presign_endpoint, bucket)?.0
         } else {
-            // build signer
-            let mut signer_builder = GoogleSigner::builder();
-            if let Some(scope) = &self.scope {
-                signer_builder.scope(scope);
-            } else {
-                signer_builder.scope(DEFAULT_GCS_SCOPE);
-            }
-            if let Some(account) = &self.service_account {
-                signer_builder.service_account(account);
-            }
-            if let Some(cred) = &self.credential {
-                signer_builder.credential_content(cred);
-            }
-            if let Some(cred) = &self.credential_path {
-                signer_builder.credential_path(cred);
-            }
-            let signer = signer_builder.build().map_err(|e| {
-                Error::new(ErrorKind::ConfigInvalid, "build GoogleSigner")
-                    .with_operation("Builder::build")
-                    .with_context("service", Scheme::Gcs)
-                    .with_context("bucket", bucket)
-                    .with_context("endpoint", &endpoint)
-                    .set_source(e)
-            })?;
-            Arc::new(signer)
+            endpoint.clone()
         };
+        debug!("backend use presign_endpoint: {}", &presign_endpoint);
 
-        let backend = GcsBackend {
-            root,
-            endpoint,
-            bucket: bucket.clone(),
-            signer,
-            client,
-        };
+        let mut cfg = AliyunConfig::default();
 
-        Ok(backend)
-    }
-}
+        if let Some(v) = self.access_key_id.take() {
+            cfg.access_key_id = Some(v);
+        }
 
-/// GCS storage backend
-#[derive(Clone)]
-pub struct GcsBackend {
-    endpoint: String,
-    bucket: String,
-    // root should end with "/"
-    root: String,
+        if let Some(v) = self.access_key_secret.take() {
+            cfg.access_key_secret = Some(v);
+        }
 
-    pub client: HttpClient,
-    pub signer: Arc<GoogleSigner>,
-}
+        let loader = AliyunLoader::new(client.client(), cfg);
 
-impl Debug for GcsBackend {
-    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        let mut de = f.debug_struct("Backend");
-        de.field("endpoint", &self.endpoint)
-            .field("bucket", &self.bucket)
-            .field("root", &self.root)
-            .field("client", &self.client)
-            .field("signer", &"<redacted>")
-            .finish()
+        let signer = AliyunOssSigner::new(bucket);
+
+        debug!("Backend build finished");
+
+        Ok(OssBackend {
+            core: Arc::new(OssCore {
+                root,
+                bucket: bucket.to_owned(),
+                endpoint,
+                host,
+                presign_endpoint,
+                signer,
+                loader,
+                client,
+            }),
+        })
     }
 }
 
+#[derive(Debug, Clone)]
+/// Aliyun Object Storage Service backend
+pub struct OssBackend {
+    core: Arc<OssCore>,
+}
+
 #[async_trait]
-impl Accessor for GcsBackend {
+impl Accessor for OssBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
-    type Writer = GcsWriter;
+    type Writer = OssWriter;
     type BlockingWriter = ();
-    type Pager = GcsPager;
+    type Pager = OssPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         use AccessorCapability::*;
         use AccessorHint::*;
 
         let mut am = AccessorInfo::default();
-        am.set_scheme(Scheme::Gcs)
-            .set_root(&self.root)
-            .set_name(&self.bucket)
-            .set_capabilities(Read | Write | List | Scan)
+        am.set_scheme(Scheme::Oss)
+            .set_root(&self.core.root)
+            .set_name(&self.core.bucket)
+            .set_max_batch_operations(1000)
+            .set_capabilities(Read | Write | Copy | List | Scan | Presign | Batch)
             .set_hints(ReadStreamable);
+
         am
     }
 
     async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
-        let mut req = self.gcs_insert_object_request(path, Some(0), None, AsyncBody::Empty)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        let resp = self.client.send_async(req).await?;
-
-        if resp.status().is_success() {
-            resp.into_body().consume().await?;
-            Ok(RpCreate::default())
-        } else {
-            Err(parse_error(resp).await?)
+        let resp = self
+            .core
+            .oss_put_object(path, None, None, None, AsyncBody::Empty)
+            .await?;
+        let status = resp.status();
+
+        match status {
+            StatusCode::CREATED | StatusCode::OK => {
+                resp.into_body().consume().await?;
+                Ok(RpCreate::default())
+            }
+            _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.gcs_get_object(path, args.range()).await?;
+        let resp = self.core.oss_get_object(path, args.range()).await?;
 
-        if resp.status().is_success() {
-            let meta = parse_into_metadata(path, resp.headers())?;
-            Ok((RpRead::with_metadata(meta), resp.into_body()))
-        } else {
-            Err(parse_error(resp).await?)
+        let status = resp.status();
+
+        match status {
+            StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
+                let meta = parse_into_metadata(path, resp.headers())?;
+                Ok((RpRead::with_metadata(meta), resp.into_body()))
+            }
+            _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
-            return Err(Error::new(
-                ErrorKind::Unsupported,
-                "append write is not supported",
-            ));
-        }
+        let upload_id = if args.append() {
+            let resp = self.core.oss_initiate_upload(path).await?;
+            match resp.status() {
+                StatusCode::OK => {
+                    let bs = resp.into_body().bytes().await?;
+                    let result: InitiateMultipartUploadResult =
+                        quick_xml::de::from_reader(bs.reader())
+                            .map_err(new_xml_deserialize_error)?;
+                    Some(result.upload_id)
+                }
+                _ => return Err(parse_error(resp).await?),
+            }
+        } else {
+            None
+        };
 
         Ok((
             RpWrite::default(),
-            GcsWriter::new(self.clone(), args, path.to_string()),
+            OssWriter::new(self.core.clone(), args, path.to_string(), upload_id),
         ))
     }
 
+    async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
+        let resp = self.core.oss_copy_object(from, to).await?;
+        let status = resp.status();
+
+        match status {
+            StatusCode::OK => {
+                resp.into_body().consume().await?;
+                Ok(RpCopy::default())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+
     async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
-        // Stat root always returns a DIR.
         if path == "/" {
-            return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
+            let m = Metadata::new(EntryMode::DIR);
+            return Ok(RpStat::new(m));
         }
 
-        let resp = self.gcs_get_object_metadata(path).await?;
+        let resp = self.core.oss_head_object(path).await?;
+
+        let status = resp.status();
 
-        if resp.status().is_success() {
-            // read http response body
-            let slc = resp.into_body().bytes().await?;
-            let meta: GetObjectJsonResponse =
-                serde_json::from_slice(&slc).map_err(new_json_deserialize_error)?;
-
-            let mode = if path.ends_with('/') {
-                EntryMode::DIR
-            } else {
-                EntryMode::FILE
-            };
-            let mut m = Metadata::new(mode);
-
-            m.set_etag(&meta.etag);
-            m.set_content_md5(&meta.md5_hash);
-
-            let size = meta
-                .size
-                .parse::<u64>()
-                .map_err(|e| Error::new(ErrorKind::Unexpected, "parse u64").set_source(e))?;
-            m.set_content_length(size);
-            if !meta.content_type.is_empty() {
-                m.set_content_type(&meta.content_type);
+        match status {
+            StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
+            StatusCode::NOT_FOUND if path.ends_with('/') => {
+                let m = Metadata::new(EntryMode::DIR);
+                Ok(RpStat::new(m))
             }
 
-            let datetime = OffsetDateTime::parse(&meta.updated, &Rfc3339).map_err(|e| {
-                Error::new(ErrorKind::Unexpected, "parse date time with rfc 3339").set_source(e)
-            })?;
-            m.set_last_modified(datetime);
-
-            Ok(RpStat::new(m))
-        } else if resp.status() == StatusCode::NOT_FOUND && path.ends_with('/') {
-            Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
-        } else {
-            Err(parse_error(resp).await?)
+            _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let resp = self.gcs_delete_object(path).await?;
-
-        // deleting not existing objects is ok
-        if resp.status().is_success() || resp.status() == StatusCode::NOT_FOUND {
-            Ok(RpDelete::default())
-        } else {
-            Err(parse_error(resp).await?)
+        let resp = self.core.oss_delete_object(path).await?;
+        let status = resp.status();
+        match status {
+            StatusCode::NO_CONTENT | StatusCode::NOT_FOUND => {
+                resp.into_body().consume().await?;
+                Ok(RpDelete::default())
+            }
+            _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
-            GcsPager::new(Arc::new(self.clone()), &self.root, path, "/", args.limit()),
+            OssPager::new(self.core.clone(), path, "/", args.limit()),
         ))
     }
 
     async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
         Ok((
             RpScan::default(),
-            GcsPager::new(Arc::new(self.clone()), &self.root, path, "", args.limit()),
+            OssPager::new(self.core.clone(), path, "", args.limit()),
         ))
     }
-}
-
-impl GcsBackend {
-    fn gcs_get_object_request(&self, path: &str, range: BytesRange) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!(
-            "{}/storage/v1/b/{}/o/{}?alt=media",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
-        );
-
-        let mut req = Request::get(&url);
-
-        if !range.is_full() {
-            req = req.header(http::header::RANGE, range.to_header());
-        }
-
-        let req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        Ok(req)
-    }
-
-    async fn gcs_get_object(
-        &self,
-        path: &str,
-        range: BytesRange,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.gcs_get_object_request(path, range)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    pub fn gcs_insert_object_request(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        content_type: Option<&str>,
-        body: AsyncBody,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
 
-        let url = format!(
-            "{}/upload/storage/v1/b/{}/o?uploadType=media&name={}",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
-        );
-
-        let mut req = Request::post(&url);
-
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size)
-        }
-
-        if let Some(mime) = content_type {
-            req = req.header(CONTENT_TYPE, mime)
-        }
-
-        // Set body
-        let req = req.body(body).map_err(new_request_build_error)?;
-
-        Ok(req)
-    }
-
-    async fn gcs_get_object_metadata(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!(
-            "{}/storage/v1/b/{}/o/{}",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
-        );
-
-        let req = Request::get(&url);
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    async fn gcs_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+        // We will not send this request out, just for signing.
+        let mut req = match args.operation() {
+            PresignOperation::Stat(_) => self.core.oss_head_object_request(path, true)?,
+            PresignOperation::Read(v) => self.core.oss_get_object_request(path, v.range(), true)?,
+            PresignOperation::Write(v) => self.core.oss_put_object_request(
+                path,
+                None,
+                v.content_type(),
+                v.content_disposition(),
+                AsyncBody::Empty,
+                true,
+            )?,
+        };
 
-        let url = format!(
-            "{}/storage/v1/b/{}/o/{}",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
-        );
+        self.core.sign_query(&mut req, args.expire()).await?;
 
-        let mut req = Request::delete(&url)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
+        // We don't need this request anymore, consume it directly.
+        let (parts, _) = req.into_parts();
 
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
+        Ok(RpPresign::new(PresignedRequest::new(
+            parts.method,
+            parts.uri,
+            parts.headers,
+        )))
+    }
+
+    async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
+        let ops = args.into_operation();
+        // Sadly, OSS will not return failed keys, so we will build
+        // a set to calculate the failed keys.
+        let mut keys = HashSet::new();
 
-        self.client.send_async(req).await
-    }
-
-    pub(crate) async fn gcs_list_objects(
-        &self,
-        path: &str,
-        page_token: &str,
-        delimiter: &str,
-        limit: Option<usize>,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
+        let ops_len = ops.len();
+        if ops_len > 1000 {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "oss services only allow delete up to 1000 keys at once",
+            )
+            .with_context("length", ops_len.to_string()));
+        }
+
+        let paths = ops
+            .into_iter()
+            .map(|(p, _)| {
+                keys.insert(p.clone());
+                p
+            })
+            .collect();
+
+        let resp = self.core.oss_delete_objects(paths).await?;
+
+        let status = resp.status();
+
+        if let StatusCode::OK = status {
+            let bs = resp.into_body().bytes().await?;
+
+            let result: DeleteObjectsResult =
+                quick_xml::de::from_reader(bs.reader()).map_err(new_xml_deserialize_error)?;
+
+            let mut batched_result = Vec::with_capacity(ops_len);
+            for i in result.deleted {
+                let path = build_rel_path(&self.core.root, &i.key);
+                keys.remove(&path);
+                batched_result.push((path, Ok(RpDelete::default().into())));
+            }
+            // TODO: we should handle those errors with code.
+            for i in keys {
+                batched_result.push((
+                    i,
+                    Err(Error::new(
+                        ErrorKind::Unexpected,
+                        "oss delete this key failed for reason we don't know",
+                    )),
+                ));
+            }
 
-        let mut url = format!(
-            "{}/storage/v1/b/{}/o?prefix={}",
-            self.endpoint,
-            self.bucket,
-            percent_encode_path(&p)
-        );
-        if !delimiter.is_empty() {
-            write!(url, "&delimiter={delimiter}").expect("write into string must succeed");
-        }
-        if let Some(limit) = limit {
-            write!(url, "&maxResults={limit}").expect("write into string must succeed");
-        }
-        if !page_token.is_empty() {
-            // NOTE:
-            //
-            // GCS uses pageToken in request and nextPageToken in response
-            //
-            // Don't know how will those tokens be like so this part are copied
-            // directly from AWS S3 service.
-            write!(url, "&pageToken={}", percent_encode_path(page_token))
-                .expect("write into string must succeed");
+            Ok(RpBatch::new(batched_result))
+        } else {
+            Err(parse_error(resp).await?)
         }
-
-        let mut req = Request::get(&url)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-}
-
-/// The raw json response returned by [`get`](https://cloud.google.com/storage/docs/json_api/v1/objects/get)
-#[derive(Debug, Default, Deserialize)]
-#[serde(default, rename_all = "camelCase")]
-struct GetObjectJsonResponse {
-    /// GCS will return size in string.
-    ///
-    /// For example: `"size": "56535"`
-    size: String,
-    /// etag is not quoted.
-    ///
-    /// For example: `"etag": "CKWasoTgyPkCEAE="`
-    etag: String,
-    /// RFC3339 styled datetime string.
-    ///
-    /// For example: `"updated": "2022-08-15T11:33:34.866Z"`
-    updated: String,
-    /// Content md5 hash
-    ///
-    /// For example: `"md5Hash": "fHcEH1vPwA6eTPqxuasXcg=="`
-    md5_hash: String,
-    /// Content type of this object.
-    ///
-    /// For example: `"contentType": "image/png",`
-    content_type: String,
-}
-
-#[cfg(test)]
-mod tests {
-    use super::*;
-
-    #[test]
-    fn test_deserialize_get_object_json_response() {
-        let content = r#"{
-  "kind": "storage#object",
-  "id": "example/1.png/1660563214863653",
-  "selfLink": "https://www.googleapis.com/storage/v1/b/example/o/1.png",
-  "mediaLink": "https://content-storage.googleapis.com/download/storage/v1/b/example/o/1.png?generation=1660563214863653&alt=media",
-  "name": "1.png",
-  "bucket": "example",
-  "generation": "1660563214863653",
-  "metageneration": "1",
-  "contentType": "image/png",
-  "storageClass": "STANDARD",
-  "size": "56535",
-  "md5Hash": "fHcEH1vPwA6eTPqxuasXcg==",
-  "crc32c": "j/un9g==",
-  "etag": "CKWasoTgyPkCEAE=",
-  "timeCreated": "2022-08-15T11:33:34.866Z",
-  "updated": "2022-08-15T11:33:34.866Z",
-  "timeStorageClassUpdated": "2022-08-15T11:33:34.866Z"
-}"#;
-
-        let meta: GetObjectJsonResponse =
-            serde_json::from_str(content).expect("json Deserialize must succeed");
-
-        assert_eq!(meta.size, "56535");
-        assert_eq!(meta.updated, "2022-08-15T11:33:34.866Z");
-        assert_eq!(meta.md5_hash, "fHcEH1vPwA6eTPqxuasXcg==");
-        assert_eq!(meta.etag, "CKWasoTgyPkCEAE=");
-        assert_eq!(meta.content_type, "image/png");
     }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/oss/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::GcsBuilder as Gcs;
+pub use backend::OssBuilder as Oss;
 
+mod core;
 mod error;
 mod pager;
-mod uri;
 mod writer;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files 3% similar despite different names*

```diff
@@ -16,47 +16,39 @@
 // under the License.
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use serde::Deserialize;
 use serde_json;
-use time::format_description::well_known::Rfc3339;
-use time::OffsetDateTime;
 
-use super::backend::GcsBackend;
+use super::core::GcsCore;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::*;
 
 /// GcsPager takes over task of listing objects and
 /// helps walking directory
 pub struct GcsPager {
-    backend: Arc<GcsBackend>,
-    root: String,
+    core: Arc<GcsCore>,
+
     path: String,
     delimiter: String,
     limit: Option<usize>,
 
     page_token: String,
     done: bool,
 }
 
 impl GcsPager {
     /// Generate a new directory walker
-    pub fn new(
-        backend: Arc<GcsBackend>,
-        root: &str,
-        path: &str,
-        delimiter: &str,
-        limit: Option<usize>,
-    ) -> Self {
+    pub fn new(core: Arc<GcsCore>, path: &str, delimiter: &str, limit: Option<usize>) -> Self {
         Self {
-            backend,
-            root: root.to_string(),
+            core,
+
             path: path.to_string(),
             delimiter: delimiter.to_string(),
             limit,
 
             page_token: "".to_string(),
             done: false,
         }
@@ -67,15 +59,15 @@
 impl oio::Page for GcsPager {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         if self.done {
             return Ok(None);
         }
 
         let resp = self
-            .backend
+            .core
             .gcs_list_objects(&self.path, &self.page_token, &self.delimiter, self.limit)
             .await?;
 
         if !resp.status().is_success() {
             return Err(parse_error(resp).await?);
         }
         let bytes = resp.into_body().bytes().await?;
@@ -89,15 +81,15 @@
             self.done = true;
         }
 
         let mut entries = Vec::with_capacity(output.prefixes.len() + output.items.len());
 
         for prefix in output.prefixes {
             let de = oio::Entry::new(
-                &build_rel_path(&self.root, &prefix),
+                &build_rel_path(&self.core.root, &prefix),
                 Metadata::new(EntryMode::DIR),
             );
 
             entries.push(de);
         }
 
         for object in output.items {
@@ -115,20 +107,17 @@
                 Error::new(ErrorKind::Unexpected, "parse u64 from list response").set_source(e)
             })?;
             meta.set_content_length(size);
             if !object.content_type.is_empty() {
                 meta.set_content_type(&object.content_type);
             }
 
-            let dt = OffsetDateTime::parse(object.updated.as_str(), &Rfc3339).map_err(|e| {
-                Error::new(ErrorKind::Unexpected, "parse last modified as rfc3339").set_source(e)
-            })?;
-            meta.set_last_modified(dt);
+            meta.set_last_modified(parse_datetime_from_rfc3339(object.updated.as_str())?);
 
-            let de = oio::Entry::new(&build_rel_path(&self.root, &object.name), meta);
+            let de = oio::Entry::new(&build_rel_path(&self.core.root, &object.name), meta);
 
             entries.push(de);
         }
 
         Ok(Some(entries))
     }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files 14% similar despite different names*

```diff
@@ -11,53 +11,52 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::GcsBackend;
+use super::core::AzblobCore;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct GcsWriter {
-    backend: GcsBackend,
+pub struct AzblobWriter {
+    core: Arc<AzblobCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl GcsWriter {
-    pub fn new(backend: GcsBackend, op: OpWrite, path: String) -> Self {
-        GcsWriter { backend, op, path }
+impl AzblobWriter {
+    pub fn new(core: Arc<AzblobCore>, op: OpWrite, path: String) -> Self {
+        AzblobWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for GcsWriter {
+impl oio::Write for AzblobWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.backend.gcs_insert_object_request(
+        let mut req = self.core.azblob_put_blob_request(
             &self.path,
             Some(bs.len()),
             self.op.content_type(),
             AsyncBody::Bytes(bs),
         )?;
 
-        self.backend
-            .signer
-            .sign(&mut req)
-            .map_err(new_request_sign_error)?;
+        self.core.sign(&mut req).await?;
 
-        let resp = self.backend.client.send_async(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -315,15 +315,15 @@
                 ErrorKind::Unsupported,
                 "ghac service doesn't support create empty file",
             ));
         }
 
         let req = self.ghac_reserve(path).await?;
 
-        let resp = self.client.send_async(req).await?;
+        let resp = self.client.send(req).await?;
 
         let cache_id = if resp.status().is_success() {
             let slc = resp.into_body().bytes().await?;
             let reserve_resp: GhacReserveResponse =
                 serde_json::from_slice(&slc).map_err(new_json_deserialize_error)?;
             reserve_resp.cache_id
         } else if resp.status().as_u16() == StatusCode::CONFLICT {
@@ -336,53 +336,53 @@
         };
 
         // Write only 1 byte to allow create.
         let req = self
             .ghac_upload(cache_id, 1, AsyncBody::Bytes(Bytes::from_static(&[0])))
             .await?;
 
-        let resp = self.client.send_async(req).await?;
+        let resp = self.client.send(req).await?;
 
         if resp.status().is_success() {
             resp.into_body().consume().await?;
         } else {
             return Err(parse_error(resp)
                 .await
                 .map(|err| err.with_operation("Backend::ghac_upload"))?);
         }
 
         let req = self.ghac_commit(cache_id, 1).await?;
-        let resp = self.client.send_async(req).await?;
+        let resp = self.client.send(req).await?;
 
         if resp.status().is_success() {
             resp.into_body().consume().await?;
             Ok(RpCreate::default())
         } else {
             Err(parse_error(resp)
                 .await
                 .map(|err| err.with_operation("Backend::ghac_commit"))?)
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let req = self.ghac_query(path).await?;
 
-        let resp = self.client.send_async(req).await?;
+        let resp = self.client.send(req).await?;
 
         let location = if resp.status() == StatusCode::OK {
             let slc = resp.into_body().bytes().await?;
             let query_resp: GhacQueryResponse =
                 serde_json::from_slice(&slc).map_err(new_json_deserialize_error)?;
             query_resp.archive_location
         } else {
             return Err(parse_error(resp).await?);
         };
 
         let req = self.ghac_get_location(&location, args.range()).await?;
-        let resp = self.client.send_async(req).await?;
+        let resp = self.client.send(req).await?;
 
         let status = resp.status();
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
@@ -396,15 +396,15 @@
                 ErrorKind::Unsupported,
                 "append write is not supported",
             ));
         }
 
         let req = self.ghac_reserve(path).await?;
 
-        let resp = self.client.send_async(req).await?;
+        let resp = self.client.send(req).await?;
 
         let cache_id = if resp.status().is_success() {
             let slc = resp.into_body().bytes().await?;
             let reserve_resp: GhacReserveResponse =
                 serde_json::from_slice(&slc).map_err(new_json_deserialize_error)?;
             reserve_resp.cache_id
         } else {
@@ -420,29 +420,29 @@
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
         let req = self.ghac_query(path).await?;
 
-        let resp = self.client.send_async(req).await?;
+        let resp = self.client.send(req).await?;
 
         let location = if resp.status() == StatusCode::OK {
             let slc = resp.into_body().bytes().await?;
             let query_resp: GhacQueryResponse =
                 serde_json::from_slice(&slc).map_err(new_json_deserialize_error)?;
             query_resp.archive_location
         } else if resp.status() == StatusCode::NO_CONTENT && path.ends_with('/') {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         } else {
             return Err(parse_error(resp).await?);
         };
 
         let req = self.ghac_head_location(&location).await?;
-        let resp = self.client.send_async(req).await?;
+        let resp = self.client.send(req).await?;
 
         let status = resp.status();
         match status {
             StatusCode::OK => {
                 let mut meta = parse_into_metadata(path, resp.headers())?;
 
                 // Hack for enable_create_simulation.
@@ -611,15 +611,15 @@
         req = req.header(USER_AGENT, format!("opendal/{VERSION} (service ghac)"));
         req = req.header("X-GitHub-Api-Version", GITHUB_API_VERSION);
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 }
 
 #[derive(Deserialize)]
 #[serde(rename_all = "camelCase")]
 struct GhacQueryResponse {
     // Not used fields.
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let size = bs.len() as u64;
         let req = self
             .backend
             .ghac_upload(self.cache_id, size, AsyncBody::Bytes(bs))
             .await?;
 
-        let resp = self.backend.client.send_async(req).await?;
+        let resp = self.backend.client.send(req).await?;
 
         if resp.status().is_success() {
             resp.into_body().consume().await?;
             self.size += size;
             Ok(())
         } else {
             Err(parse_error(resp)
@@ -69,15 +69,15 @@
             ErrorKind::Unsupported,
             "output writer doesn't support append",
         ))
     }
 
     async fn close(&mut self) -> Result<()> {
         let req = self.backend.ghac_commit(self.cache_id, self.size).await?;
-        let resp = self.backend.client.send_async(req).await?;
+        let resp = self.backend.client.send(req).await?;
 
         if resp.status().is_success() {
             resp.into_body().consume().await?;
             Ok(())
         } else {
             Err(parse_error(resp)
                 .await
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 use std::io;
 use std::io::SeekFrom;
 use std::path::PathBuf;
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use log::debug;
-use time::OffsetDateTime;
 
 use super::error::parse_io_error;
 use super::pager::HdfsPager;
 use super::writer::HdfsWriter;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
@@ -358,15 +357,15 @@
         } else if meta.is_file() {
             EntryMode::FILE
         } else {
             EntryMode::Unknown
         };
         let mut m = Metadata::new(mode);
         m.set_content_length(meta.len());
-        m.set_last_modified(OffsetDateTime::from(meta.modified()));
+        m.set_last_modified(meta.modified().into());
 
         Ok(RpStat::new(m))
     }
 
     async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
         let p = build_rooted_abs_path(&self.root, path);
 
@@ -525,15 +524,15 @@
         } else if meta.is_file() {
             EntryMode::FILE
         } else {
             EntryMode::Unknown
         };
         let mut m = Metadata::new(mode);
         m.set_content_length(meta.len());
-        m.set_last_modified(OffsetDateTime::from(meta.modified()));
+        m.set_last_modified(meta.modified().into());
 
         Ok(RpStat::new(m))
     }
 
     fn blocking_delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
         let p = build_rooted_abs_path(&self.root, path);
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files 7% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             };
 
             let path = build_rel_path(&self.root, de.path());
 
             let d = if de.is_file() {
                 let meta = Metadata::new(EntryMode::FILE)
                     .with_content_length(de.len())
-                    .with_last_modified(time::OffsetDateTime::from(de.modified()));
+                    .with_last_modified(de.modified().into());
                 oio::Entry::new(&path, meta)
             } else if de.is_dir() {
                 // Make sure we are returning the correct path.
                 oio::Entry::new(&format!("{path}/"), Metadata::new(EntryMode::DIR))
             } else {
                 oio::Entry::new(&path, Metadata::new(EntryMode::Unknown))
             };
@@ -83,15 +83,15 @@
             };
 
             let path = build_rel_path(&self.root, de.path());
 
             let d = if de.is_file() {
                 let meta = Metadata::new(EntryMode::FILE)
                     .with_content_length(de.len())
-                    .with_last_modified(time::OffsetDateTime::from(de.modified()));
+                    .with_last_modified(de.modified().into());
                 oio::Entry::new(&path, meta)
             } else if de.is_dir() {
                 // Make sure we are returning the correct path.
                 oio::Entry::new(&format!("{path}/"), Metadata::new(EntryMode::DIR))
             } else {
                 oio::Entry::new(&path, Metadata::new(EntryMode::Unknown))
             };
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
             req = req.header(header::RANGE, range.to_header());
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     async fn http_head(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!("{}{}", self.endpoint, percent_encode_path(&p));
 
@@ -332,15 +332,15 @@
             req = req.header(header::AUTHORIZATION, auth.clone())
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 }
 
 #[cfg(test)]
 mod tests {
     use anyhow::Result;
     use wiremock::matchers::basic_auth;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/http/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -410,29 +410,29 @@
             req = req.header(http::header::RANGE, range.to_header());
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     async fn ipfs_head(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!("{}{}", self.endpoint, percent_encode_path(&p));
 
         let req = Request::head(&url);
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     async fn ipfs_list(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!("{}{}", self.endpoint, percent_encode_path(&p));
 
@@ -444,15 +444,15 @@
         // ref: https://github.com/ipfs/specs/blob/main/http-gateways/PATH_GATEWAY.md
         req = req.header(http::header::ACCEPT, "application/vnd.ipld.raw");
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 }
 
 pub struct DirStream {
     backend: Arc<IpfsBackend>,
     path: String,
     consumed: bool,
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files 4% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         );
 
         let req = Request::post(url);
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     async fn ipmfs_read(
         &self,
         path: &str,
         range: BytesRange,
     ) -> Result<Response<IncomingAsyncBody>> {
@@ -220,15 +220,15 @@
         }
 
         let req = Request::post(url);
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     async fn ipmfs_rm(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!(
             "{}/api/v0/files/rm?arg={}",
@@ -237,15 +237,15 @@
         );
 
         let req = Request::post(url);
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     pub(crate) async fn ipmfs_ls(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!(
             "{}/api/v0/files/ls?arg={}&long=true",
@@ -254,15 +254,15 @@
         );
 
         let req = Request::post(url);
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     async fn ipmfs_mkdir(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_rooted_abs_path(&self.root, path);
 
         let url = format!(
             "{}/api/v0/files/mkdir?arg={}&parents=true",
@@ -271,15 +271,15 @@
         );
 
         let req = Request::post(url);
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     /// Support write from reader.
     pub async fn ipmfs_write(
         &self,
         path: &str,
         body: AsyncBody,
@@ -292,15 +292,15 @@
             percent_encode_path(&p)
         );
 
         let req = Request::post(url);
 
         let req = req.body(body).map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 }
 
 #[derive(Deserialize, Default, Debug)]
 #[serde(default)]
 struct IpfsStatResponse {
     #[serde(rename = "Size")]
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt` & `opendal-0.31.0/local_dependencies/opendal/src/services/memcached/MIT-ascii.txt`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 16% similar despite different names*

```diff
@@ -16,23 +16,22 @@
 // under the License.
 
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::sync::Arc;
 
 use async_trait::async_trait;
-use http::header::CONTENT_LENGTH;
-use http::header::CONTENT_TYPE;
-use http::Request;
-use http::Response;
 use http::StatusCode;
 use http::Uri;
 use log::debug;
+use reqsign::HuaweicloudObsConfig;
+use reqsign::HuaweicloudObsCredentialLoader;
 use reqsign::HuaweicloudObsSigner;
 
+use super::core::ObsCore;
 use super::error::parse_error;
 use super::pager::ObsPager;
 use super::writer::ObsWriter;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
@@ -40,14 +39,15 @@
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
+/// - [x] copy
 /// - [x] list
 /// - [x] scan
 /// - [ ] presign
 /// - [ ] blocking
 ///
 /// # Configuration
 ///
@@ -244,61 +244,55 @@
         } else {
             HttpClient::new().map_err(|err| {
                 err.with_operation("Builder::build")
                     .with_context("service", Scheme::Obs)
             })?
         };
 
-        let mut signer_builder = HuaweicloudObsSigner::builder();
-        if let (Some(access_key_id), Some(secret_access_key)) =
-            (&self.access_key_id, &self.secret_access_key)
-        {
-            signer_builder
-                .access_key(access_key_id)
-                .secret_key(secret_access_key);
-        }
+        let config = HuaweicloudObsConfig {
+            access_key_id: self.access_key_id.take(),
+            secret_access_key: self.secret_access_key.take(),
+            security_token: None,
+        };
+
+        let cred_loader = HuaweicloudObsCredentialLoader::new(config);
 
         // Set the bucket name in CanonicalizedResource.
         // 1. If the bucket is bound to a user domain name, use the user domain name as the bucket name,
         // for example, `/obs.ccc.com/object`. `obs.ccc.com` is the user domain name bound to the bucket.
         // 2. If you do not access OBS using a user domain name, this field is in the format of `/bucket/object`.
         //
         // Please refer to this doc for more details:
         // https://support.huaweicloud.com/intl/en-us/api-obs/obs_04_0010.html
-        if is_obs_default {
-            signer_builder.bucket(&bucket);
-        } else {
-            signer_builder.bucket(&endpoint);
-        }
-
-        let signer = signer_builder.build().map_err(|e| {
-            Error::new(ErrorKind::Unexpected, "build HuaweicloudObsSigner")
-                .with_context("service", Scheme::Obs)
-                .set_source(e)
-        })?;
+        let signer = HuaweicloudObsSigner::new({
+            if is_obs_default {
+                &bucket
+            } else {
+                &endpoint
+            }
+        });
 
-        debug!("backend build finished: {:?}", &self);
+        debug!("backend build finished");
         Ok(ObsBackend {
-            client,
-            root,
-            endpoint: format!("{}://{}", &scheme, &endpoint),
-            signer: Arc::new(signer),
-            bucket,
+            core: Arc::new(ObsCore {
+                bucket,
+                root,
+                endpoint: format!("{}://{}", &scheme, &endpoint),
+                signer,
+                loader: cred_loader,
+                client,
+            }),
         })
     }
 }
 
 /// Backend for Huaweicloud OBS services.
 #[derive(Debug, Clone)]
 pub struct ObsBackend {
-    pub client: HttpClient,
-    root: String,
-    endpoint: String,
-    pub signer: Arc<HuaweicloudObsSigner>,
-    bucket: String,
+    core: Arc<ObsCore>,
 }
 
 #[async_trait]
 impl Accessor for ObsBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = ObsWriter;
@@ -308,42 +302,44 @@
 
     fn info(&self) -> AccessorInfo {
         use AccessorCapability::*;
         use AccessorHint::*;
 
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Obs)
-            .set_root(&self.root)
-            .set_name(&self.bucket)
-            .set_capabilities(Read | Write | List | Scan)
+            .set_root(&self.core.root)
+            .set_name(&self.core.bucket)
+            .set_capabilities(Read | Write | Copy | List | Scan)
             .set_hints(ReadStreamable);
 
         am
     }
 
     async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
-        let mut req = self.obs_put_object_request(path, Some(0), None, AsyncBody::Empty)?;
+        let mut req = self
+            .core
+            .obs_put_object_request(path, Some(0), None, AsyncBody::Empty)?;
 
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
+        self.core.sign(&mut req).await?;
 
-        let resp = self.client.send_async(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(RpCreate::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.obs_get_object(path, args.range()).await?;
+        let resp = self.core.obs_get_object(path, args.range()).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
                 let meta = parse_into_metadata(path, resp.headers())?;
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
@@ -358,183 +354,72 @@
                 ErrorKind::Unsupported,
                 "append write is not supported",
             ));
         }
 
         Ok((
             RpWrite::default(),
-            ObsWriter::new(self.clone(), args, path.to_string()),
+            ObsWriter::new(self.core.clone(), args, path.to_string()),
         ))
     }
 
+    async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
+        let resp = self.core.obs_copy_object(from, to).await?;
+
+        let status = resp.status();
+
+        match status {
+            StatusCode::OK => {
+                resp.into_body().consume().await?;
+                Ok(RpCopy::default())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+
     async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.obs_get_head_object(path).await?;
+        let resp = self.core.obs_get_head_object(path).await?;
 
         let status = resp.status();
 
         // The response is very similar to azblob.
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
                 Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let resp = self.obs_delete_object(path).await?;
+        let resp = self.core.obs_delete_object(path).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::NO_CONTENT | StatusCode::ACCEPTED | StatusCode::NOT_FOUND => {
                 Ok(RpDelete::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         Ok((
             RpList::default(),
-            ObsPager::new(Arc::new(self.clone()), &self.root, path, "/", args.limit()),
+            ObsPager::new(self.core.clone(), path, "/", args.limit()),
         ))
     }
 
     async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
         Ok((
             RpScan::default(),
-            ObsPager::new(Arc::new(self.clone()), &self.root, path, "", args.limit()),
+            ObsPager::new(self.core.clone(), path, "", args.limit()),
         ))
     }
 }
-
-impl ObsBackend {
-    async fn obs_get_object(
-        &self,
-        path: &str,
-        range: BytesRange,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
-
-        let mut req = Request::get(&url);
-
-        if !range.is_full() {
-            req = req.header(http::header::RANGE, range.to_header())
-        }
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    pub fn obs_put_object_request(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        content_type: Option<&str>,
-        body: AsyncBody,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
-
-        let mut req = Request::put(&url);
-
-        if let Some(size) = size {
-            req = req.header(CONTENT_LENGTH, size)
-        }
-
-        if let Some(mime) = content_type {
-            req = req.header(CONTENT_TYPE, mime)
-        }
-
-        let req = req.body(body).map_err(new_request_build_error)?;
-
-        Ok(req)
-    }
-
-    async fn obs_get_head_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
-
-        // The header 'Origin' is optional for API calling, the doc has mistake, confirmed with customer service of huaweicloud.
-        // https://support.huaweicloud.com/intl/en-us/api-obs/obs_04_0084.html
-
-        let req = Request::head(&url);
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    async fn obs_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
-
-        let req = Request::delete(&url);
-
-        let mut req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-
-    pub(crate) async fn obs_list_objects(
-        &self,
-        path: &str,
-        next_marker: &str,
-        delimiter: &str,
-        limit: Option<usize>,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let mut queries = vec![];
-        if !path.is_empty() {
-            queries.push(format!("prefix={}", percent_encode_path(&p)));
-        }
-        if !delimiter.is_empty() {
-            queries.push(format!("delimiter={delimiter}"));
-        }
-        if let Some(limit) = limit {
-            queries.push(format!("max-keys={limit}"));
-        }
-        if !next_marker.is_empty() {
-            queries.push(format!("marker={next_marker}"));
-        }
-
-        let url = if queries.is_empty() {
-            self.endpoint.to_string()
-        } else {
-            format!("{}?{}", self.endpoint, queries.join("&"))
-        };
-
-        let mut req = Request::get(&url)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-
-        self.client.send_async(req).await
-    }
-}
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -12,12 +12,9 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::ObsBuilder as Obs;
 
-mod error;
-mod pager;
-mod writer;
+pub use backend::SledBuilder as Sled;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files 12% similar despite different names*

```diff
@@ -18,45 +18,37 @@
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Buf;
 use quick_xml::de;
 use serde::Deserialize;
 
-use super::backend::ObsBackend;
+use super::core::ObsCore;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::EntryMode;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Metadata;
 use crate::Result;
 
 pub struct ObsPager {
-    backend: Arc<ObsBackend>,
-    root: String,
+    core: Arc<ObsCore>,
     path: String,
     delimiter: String,
     limit: Option<usize>,
 
     next_marker: String,
     done: bool,
 }
 
 impl ObsPager {
-    pub fn new(
-        backend: Arc<ObsBackend>,
-        root: &str,
-        path: &str,
-        delimiter: &str,
-        limit: Option<usize>,
-    ) -> Self {
+    pub fn new(core: Arc<ObsCore>, path: &str, delimiter: &str, limit: Option<usize>) -> Self {
         Self {
-            backend,
-            root: root.to_string(),
+            core,
             path: path.to_string(),
             delimiter: delimiter.to_string(),
             limit,
 
             next_marker: "".to_string(),
             done: false,
         }
@@ -67,15 +59,15 @@
 impl oio::Page for ObsPager {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         if self.done {
             return Ok(None);
         }
 
         let resp = self
-            .backend
+            .core
             .obs_list_objects(&self.path, &self.next_marker, &self.delimiter, self.limit)
             .await?;
 
         if resp.status() != http::StatusCode::OK {
             return Err(parse_error(resp).await?);
         }
 
@@ -94,29 +86,29 @@
         self.next_marker = output.next_marker.clone().unwrap_or_default();
 
         let common_prefixes = output.common_prefixes;
         let mut entries = Vec::with_capacity(common_prefixes.len() + output.contents.len());
 
         for prefix in common_prefixes {
             let de = oio::Entry::new(
-                &build_rel_path(&self.root, &prefix.prefix),
+                &build_rel_path(&self.core.root, &prefix.prefix),
                 Metadata::new(EntryMode::DIR),
             );
 
             entries.push(de);
         }
 
         for object in output.contents {
             if object.key.ends_with('/') {
                 continue;
             }
 
             let meta = Metadata::new(EntryMode::FILE).with_content_length(object.size);
 
-            let de = oio::Entry::new(&build_rel_path(&self.root, &object.key), meta);
+            let de = oio::Entry::new(&build_rel_path(&self.core.root, &object.key), meta);
 
             entries.push(de);
         }
 
         Ok(Some(entries))
     }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files 12% similar despite different names*

```diff
@@ -11,53 +11,52 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::ObsBackend;
+use super::core::ObsCore;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct ObsWriter {
-    backend: ObsBackend,
+    core: Arc<ObsCore>,
 
     op: OpWrite,
     path: String,
 }
 
 impl ObsWriter {
-    pub fn new(backend: ObsBackend, op: OpWrite, path: String) -> Self {
-        ObsWriter { backend, op, path }
+    pub fn new(core: Arc<ObsCore>, op: OpWrite, path: String) -> Self {
+        ObsWriter { core, op, path }
     }
 }
 
 #[async_trait]
 impl oio::Write for ObsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.backend.obs_put_object_request(
+        let mut req = self.core.obs_put_object_request(
             &self.path,
             Some(bs.len()),
             self.op.content_type(),
             AsyncBody::Bytes(bs),
         )?;
 
-        self.backend
-            .signer
-            .sign(&mut req)
-            .map_err(new_request_sign_error)?;
+        self.core.sign(&mut req).await?;
 
-        let resp = self.backend.client.send_async(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files 25% similar despite different names*

```diff
@@ -11,907 +11,683 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use core::fmt::Debug;
 use std::collections::HashMap;
-use std::collections::HashSet;
-use std::fmt::Debug;
-use std::fmt::Formatter;
-use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Buf;
-use bytes::Bytes;
-use http::header::CONTENT_DISPOSITION;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
-use http::header::RANGE;
+use http::response::Parts;
 use http::Request;
 use http::Response;
 use http::StatusCode;
-use http::Uri;
 use log::debug;
-use reqsign::AliyunOssBuilder;
-use reqsign::AliyunOssSigner;
-use serde::Deserialize;
-use serde::Serialize;
+use log::error;
+use tokio::sync::OnceCell;
 
 use super::error::parse_error;
-use super::pager::OssPager;
-use super::writer::OssWriter;
+use super::message::BooleanResp;
+use super::message::FileStatusType;
+use super::message::FileStatusWrapper;
+use super::message::FileStatusesWrapper;
+use super::pager::WebhdfsPager;
+use super::writer::WebhdfsWriter;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
-/// Aliyun Object Storage Service (OSS) support
+const WEBHDFS_DEFAULT_ENDPOINT: &str = "http://127.0.0.1:9870";
+
+/// [WebHDFS](https://hadoop.apache.org/docs/stable/hadoop-project-dist/hadoop-hdfs/WebHDFS.html)'s REST API support.
+///
+/// There two implementations of WebHDFS REST API:
+///
+/// - Native via HDFS Namenode and Datanode, data are transferred between nodes directly.
+/// - [HttpFS](https://hadoop.apache.org/docs/stable/hadoop-hdfs-httpfs/index.html) is a gateway before hdfs nodes, data are proxied.
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
 /// - [x] list
-/// - [x] scan
-/// - [ ] presign
+/// - [ ] ~~scan~~
+/// - [ ] ~~presign~~
 /// - [ ] blocking
 ///
-/// # Configuration
+/// # Differences with hdfs
 ///
-/// - `root`: Set the work dir for backend.
-/// - `bucket`: Set the container name for backend.
-/// - `endpoint`: Set the endpoint for backend.
-/// - `presign_endpoint`: Set the endpoint for presign.
-/// - `access_key_id`: Set the access_key_id for backend.
-/// - `access_key_secret`: Set the access_key_secret for backend.
-/// - `role_arn`: Set the role of backend.
-/// - `oidc_token`: Set the oidc_token for backend.
-/// - `allow_anonymous`: Set the backend access OSS in anonymous way.
+/// [Hdfs][crate::services::Hdfs] is powered by HDFS's native java client. Users need to setup the hdfs services correctly. But webhdfs can access from HTTP API and no extra setup needed.
 ///
-/// Refer to [`OssBuilder`]'s public API docs for more information.
+/// # Configurations
 ///
-/// # Example
+/// - `root`: The root path of the WebHDFS service.
+/// - `endpoint`: The endpoint of the WebHDFS service.
+/// - `delegation`: The delegation token for WebHDFS.
 ///
-/// ## Via Builder
+/// Refer to [`Builder`]'s public API docs for more information
+///
+/// # Examples
 ///
+/// ## Via Builder
 /// ```no_run
 /// use std::sync::Arc;
 ///
 /// use anyhow::Result;
-/// use opendal::services::Oss;
+/// use opendal::services::Webhdfs;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
-///     // Create OSS backend builder.
-///     let mut builder = Oss::default();
-///     // Set the root for oss, all operations will happen under this root.
+///     let mut builder = Webhdfs::default();
+///     // set the root for WebHDFS, all operations will happen under this root
 ///     //
-///     // NOTE: the root must be absolute path.
+///     // Note:
+///     // if the root is not exists, the builder will automatically create the
+///     // root directory for you
+///     // if the root exists and is a directory, the builder will continue working
+///     // if the root exists and is a folder, the builder will fail on building backend
 ///     builder.root("/path/to/dir");
-///     // Set the bucket name, this is required.
-///     builder.bucket("test");
-///     // Set the endpoint.
-///     //
-///     // For example:
-///     // - "https://oss-ap-northeast-1.aliyuncs.com"
-///     // - "https://oss-hangzhou.aliyuncs.com"
-///     builder.endpoint("https://oss-cn-beijing.aliyuncs.com");
-///     // Set the access_key_id and access_key_secret.
-///     //
-///     // OpenDAL will try load credential from the env.
-///     // If credential not set and no valid credential in env, OpenDAL will
-///     // send request without signing like anonymous user.
-///     builder.access_key_id("access_key_id");
-///     builder.access_key_secret("access_key_secret");
+///     // set the endpoint of webhdfs namenode, controlled by dfs.namenode.http-address
+///     // default is http://127.0.0.1:9870
+///     builder.endpoint("http://127.0.0.1:9870");
+///     // set the delegation_token for builder
+///     builder.delegation("delegation_token");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
 ///
 ///     Ok(())
 /// }
 /// ```
 #[derive(Default, Clone)]
-pub struct OssBuilder {
+pub struct WebhdfsBuilder {
     root: Option<String>,
-
     endpoint: Option<String>,
-    presign_endpoint: Option<String>,
-    bucket: String,
-
-    // authenticate options
-    access_key_id: Option<String>,
-    access_key_secret: Option<String>,
-
-    allow_anonymous: bool,
-
-    http_client: Option<HttpClient>,
+    delegation: Option<String>,
 }
 
-impl Debug for OssBuilder {
-    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        let mut d = f.debug_struct("Builder");
-        d.field("root", &self.root)
-            .field("bucket", &self.bucket)
-            .field("endpoint", &self.endpoint)
-            .field("presign_endpoint", &self.presign_endpoint)
-            .field("allow_anonymous", &self.allow_anonymous);
-
-        if self.access_key_id.is_some() {
-            d.field("access_key_id", &"<redacted>");
+impl Debug for WebhdfsBuilder {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        let mut ds = f.debug_struct("Builder");
+        ds.field("root", &self.root)
+            .field("endpoint", &self.endpoint);
+        if self.delegation.is_some() {
+            ds.field("delegation", &"<redacted>");
         }
-
-        if self.access_key_secret.is_some() {
-            d.field("access_key_secret", &"<redacted>");
-        }
-
-        d.finish()
+        ds.finish()
     }
 }
 
-impl OssBuilder {
-    /// Set root of this backend.
+impl WebhdfsBuilder {
+    /// Set the working directory of this backend
     ///
-    /// All operations will happen under this root.
+    /// All operations will happen under this root
+    /// # Note
+    /// The root will be automatically created if not exists.
+    /// If the root is occupied by a file, building of directory will fail
     pub fn root(&mut self, root: &str) -> &mut Self {
         self.root = if root.is_empty() {
             None
         } else {
             Some(root.to_string())
         };
 
         self
     }
 
-    /// Set bucket name of this backend.
-    pub fn bucket(&mut self, bucket: &str) -> &mut Self {
-        self.bucket = bucket.to_string();
-
-        self
-    }
-
-    /// Set endpoint of this backend.
-    pub fn endpoint(&mut self, endpoint: &str) -> &mut Self {
-        if !endpoint.is_empty() {
-            // Trim trailing `/` so that we can accept `http://127.0.0.1:9000/`
-            self.endpoint = Some(endpoint.trim_end_matches('/').to_string())
-        }
-
-        self
-    }
-
-    /// Set a endpoint for generating presigned urls.
+    /// Set the remote address of this backend
+    /// default to `http://127.0.0.1:9870`
     ///
-    /// You can offer a public endpoint like <https://oss-cn-beijing.aliyuncs.com> to return a presinged url for
-    /// public accessors, along with an internal endpoint like <https://oss-cn-beijing-internal.aliyuncs.com>
-    /// to access objects in a faster path.
+    /// Endpoints should be full uri, e.g.
     ///
-    /// - If presign_endpoint is set, we will use presign_endpoint on generating presigned urls.
-    /// - if not, we will use endpoint as default.
-    pub fn presign_endpoint(&mut self, endpoint: &str) -> &mut Self {
+    /// - `https://webhdfs.example.com:9870`
+    /// - `http://192.168.66.88:9870`
+    ///
+    /// If user inputs endpoint without scheme, we will
+    /// prepend `http://` to it.
+    pub fn endpoint(&mut self, endpoint: &str) -> &mut Self {
         if !endpoint.is_empty() {
-            // Trim trailing `/` so that we can accept `http://127.0.0.1:9000/`
-            self.presign_endpoint = Some(endpoint.trim_end_matches('/').to_string())
+            // trim tailing slash so we can accept `http://127.0.0.1:9870/`
+            self.endpoint = Some(endpoint.trim_end_matches('/').to_string());
         }
-
         self
     }
 
-    /// Set access_key_id of this backend.
-    ///
-    /// - If access_key_id is set, we will take user's input first.
-    /// - If not, we will try to load it from environment.
-    pub fn access_key_id(&mut self, v: &str) -> &mut Self {
-        if !v.is_empty() {
-            self.access_key_id = Some(v.to_string())
+    /// Set the delegation token of this backend,
+    /// used for authentication
+    /// # Note
+    /// The builder prefers using delegation token over username.
+    /// If both are set, delegation token will be used.
+    pub fn delegation(&mut self, delegation: &str) -> &mut Self {
+        if !delegation.is_empty() {
+            self.delegation = Some(delegation.to_string());
         }
-
         self
     }
+}
 
-    /// Set access_key_secret of this backend.
-    ///
-    /// - If access_key_secret is set, we will take user's input first.
-    /// - If not, we will try to load it from environment.
-    pub fn access_key_secret(&mut self, v: &str) -> &mut Self {
-        if !v.is_empty() {
-            self.access_key_secret = Some(v.to_string())
+impl WebhdfsBuilder {
+    fn auth_str(&mut self) -> Option<String> {
+        if let Some(dt) = self.delegation.take() {
+            return Some(format!("delegation_token={dt}"));
         }
-
-        self
-    }
-
-    /// Anonymously access the bucket.
-    pub fn allow_anonymous(&mut self) -> &mut Self {
-        self.allow_anonymous = true;
-        self
-    }
-
-    /// Specify the http client that used by this service.
-    ///
-    /// # Notes
-    ///
-    /// This API is part of OpenDAL's Raw API. `HttpClient` could be changed
-    /// during minor updates.
-    pub fn http_client(&mut self, client: HttpClient) -> &mut Self {
-        self.http_client = Some(client);
-        self
-    }
-
-    /// preprocess the endpoint option
-    fn parse_endpoint(&self, endpoint: &Option<String>, bucket: &str) -> Result<(String, String)> {
-        let (endpoint, host) = match endpoint.clone() {
-            Some(ep) => {
-                let uri = ep.parse::<Uri>().map_err(|err| {
-                    Error::new(ErrorKind::ConfigInvalid, "endpoint is invalid")
-                        .with_context("service", Scheme::Oss)
-                        .with_context("endpoint", &ep)
-                        .set_source(err)
-                })?;
-                let host = uri.host().ok_or_else(|| {
-                    Error::new(ErrorKind::ConfigInvalid, "endpoint host is empty")
-                        .with_context("service", Scheme::Oss)
-                        .with_context("endpoint", &ep)
-                })?;
-                let full_host = format!("{bucket}.{host}");
-                let endpoint = match uri.scheme_str() {
-                    Some(scheme_str) => match scheme_str {
-                        "http" | "https" => format!("{scheme_str}://{full_host}"),
-                        _ => {
-                            return Err(Error::new(
-                                ErrorKind::ConfigInvalid,
-                                "endpoint protocol is invalid",
-                            )
-                            .with_context("service", Scheme::Oss));
-                        }
-                    },
-                    None => format!("https://{full_host}"),
-                };
-                (endpoint, full_host)
-            }
-            None => {
-                return Err(Error::new(ErrorKind::ConfigInvalid, "endpoint is empty")
-                    .with_context("service", Scheme::Oss));
-            }
-        };
-        Ok((endpoint, host))
+        None
     }
 }
 
-impl Builder for OssBuilder {
-    const SCHEME: Scheme = Scheme::Oss;
-    type Accessor = OssBackend;
+impl Builder for WebhdfsBuilder {
+    const SCHEME: Scheme = Scheme::Webhdfs;
+    type Accessor = WebhdfsBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
-        let mut builder = OssBuilder::default();
+        let mut builder = WebhdfsBuilder::default();
 
-        map.get("root").map(|v| builder.root(v));
-        map.get("bucket").map(|v| builder.bucket(v));
-        map.get("endpoint").map(|v| builder.endpoint(v));
-        map.get("presign_endpoint")
-            .map(|v| builder.presign_endpoint(v));
-        map.get("access_key_id").map(|v| builder.access_key_id(v));
-        map.get("access_key_secret")
-            .map(|v| builder.access_key_secret(v));
-        map.get("allow_anonymous")
-            .filter(|v| *v == "on" || *v == "true")
-            .map(|_| builder.allow_anonymous());
+        for (k, v) in map.iter() {
+            let v = v.as_str();
+            match k.as_str() {
+                "root" => builder.root(v),
+                "endpoint" => builder.endpoint(v),
+                "delegation" => builder.delegation(v),
+                _ => continue,
+            };
+        }
 
         builder
     }
 
+    /// build the backend
+    ///
+    /// # Note:
+    /// when building backend, the built backend will check if the root directory
+    /// exits.
+    /// if the directory does not exits, the directory will be automatically created
+    /// if the root path is occupied by a file, a failure will be returned
     fn build(&mut self) -> Result<Self::Accessor> {
-        debug!("backend build started: {:?}", &self);
+        debug!("building backend: {:?}", self);
 
-        let root = normalize_root(&self.root.clone().unwrap_or_default());
-        debug!("backend use root {}", &root);
+        let root = normalize_root(&self.root.take().unwrap_or_default());
+        debug!("backend use root {root}");
 
-        // Handle endpoint, region and bucket name.
-        let bucket = match self.bucket.is_empty() {
-            false => Ok(&self.bucket),
-            true => Err(
-                Error::new(ErrorKind::ConfigInvalid, "The bucket is misconfigured")
-                    .with_context("service", Scheme::Oss),
-            ),
-        }?;
-
-        let client = if let Some(client) = self.http_client.take() {
-            client
-        } else {
-            HttpClient::new().map_err(|err| {
-                err.with_operation("Builder::build")
-                    .with_context("service", Scheme::Oss)
-            })?
+        // check scheme
+        let endpoint = match self.endpoint.take() {
+            Some(endpoint) => {
+                if endpoint.starts_with("http") {
+                    endpoint
+                } else {
+                    format!("http://{endpoint}")
+                }
+            }
+            None => WEBHDFS_DEFAULT_ENDPOINT.to_string(),
         };
+        debug!("backend use endpoint {}", endpoint);
 
-        // Retrieve endpoint and host by parsing the endpoint option and bucket. If presign_endpoint is not
-        // set, take endpoint as default presign_endpoint.
-        let (endpoint, host) = self.parse_endpoint(&self.endpoint, bucket)?;
-        debug!("backend use bucket {}, endpoint: {}", &bucket, &endpoint);
+        let auth = self.auth_str();
+        let client = HttpClient::new()?;
 
-        let presign_endpoint = if self.presign_endpoint.is_some() {
-            self.parse_endpoint(&self.presign_endpoint, bucket)?.0
-        } else {
-            endpoint.clone()
+        let backend = WebhdfsBackend {
+            root: root.clone(),
+            endpoint,
+            auth,
+            client,
+            root_checker: OnceCell::new(),
         };
-        debug!("backend use presign_endpoint: {}", &presign_endpoint);
 
-        let mut signer_builder = AliyunOssBuilder::default();
-
-        if self.allow_anonymous {
-            signer_builder.allow_anonymous();
-        }
+        debug!("checking working directory: {}", root);
 
-        signer_builder.bucket(bucket);
-
-        if let (Some(ak), Some(sk)) = (&self.access_key_id, &self.access_key_secret) {
-            signer_builder.access_key_id(ak);
-            signer_builder.access_key_secret(sk);
-        }
-
-        let signer = signer_builder.build().map_err(|e| {
-            Error::new(ErrorKind::ConfigInvalid, "build AliyunOssSigner")
-                .with_context("service", Scheme::Oss)
-                .with_context("endpoint", &endpoint)
-                .with_context("bucket", bucket)
-                .set_source(e)
-        })?;
-
-        debug!("Backend build finished: {:?}", &self);
-
-        Ok(OssBackend {
-            root,
-            endpoint,
-            presign_endpoint,
-            host,
-            client,
-            bucket: self.bucket.clone(),
-            signer: Arc::new(signer),
-        })
+        Ok(backend)
     }
 }
 
-#[derive(Clone)]
-/// Aliyun Object Storage Service backend
-pub struct OssBackend {
-    pub client: HttpClient,
-
+/// Backend for WebHDFS service
+#[derive(Debug, Clone)]
+pub struct WebhdfsBackend {
     root: String,
-    bucket: String,
-    /// buffered host string
-    ///
-    /// format: <bucket-name>.<endpoint-domain-name>
-    host: String,
     endpoint: String,
-    presign_endpoint: String,
-    pub signer: Arc<AliyunOssSigner>,
-}
-
-impl Debug for OssBackend {
-    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        f.debug_struct("Backend")
-            .field("root", &self.root)
-            .field("bucket", &self.bucket)
-            .field("endpoint", &self.endpoint)
-            .field("host", &self.host)
-            .finish()
-    }
+    pub client: HttpClient,
+    auth: Option<String>,
+    root_checker: OnceCell<()>,
 }
 
-#[async_trait]
-impl Accessor for OssBackend {
-    type Reader = IncomingAsyncBody;
-    type BlockingReader = ();
-    type Writer = OssWriter;
-    type BlockingWriter = ();
-    type Pager = OssPager;
-    type BlockingPager = ();
-
-    fn info(&self) -> AccessorInfo {
-        use AccessorCapability::*;
-        use AccessorHint::*;
-
-        let mut am = AccessorInfo::default();
-        am.set_scheme(Scheme::Oss)
-            .set_root(&self.root)
-            .set_name(&self.bucket)
-            .set_max_batch_operations(1000)
-            .set_capabilities(Read | Write | List | Scan | Presign | Batch)
-            .set_hints(ReadStreamable);
-
-        am
-    }
+impl WebhdfsBackend {
+    // create object or make a directory
+    pub async fn webhdfs_create_object_req(
+        &self,
+        path: &str,
+        size: Option<usize>,
+        content_type: Option<&str>,
+        body: AsyncBody,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+        let op = if path.ends_with('/') {
+            "MKDIRS"
+        } else {
+            "CREATE"
+        };
+        let mut url = format!(
+            "{}/webhdfs/v1/{}?op={}&overwrite=true",
+            self.endpoint,
+            percent_encode_path(&p),
+            op,
+        );
+        if let Some(auth) = &self.auth {
+            url += format!("&{auth}").as_str();
+        }
 
-    async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
-        let resp = self
-            .oss_put_object(path, None, None, None, AsyncBody::Empty)
-            .await?;
-        let status = resp.status();
+        let req = Request::put(&url)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
 
-        match status {
-            StatusCode::CREATED | StatusCode::OK => {
-                resp.into_body().consume().await?;
-                Ok(RpCreate::default())
-            }
-            _ => Err(parse_error(resp).await?),
+        // mkdir does not redirect
+        if path.ends_with('/') {
+            return Ok(req);
         }
-    }
 
-    async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.oss_get_object(path, args.range()).await?;
-
-        let status = resp.status();
+        let resp = self.client.send(req).await?;
 
-        match status {
-            StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
-                let meta = parse_into_metadata(path, resp.headers())?;
-                Ok((RpRead::with_metadata(meta), resp.into_body()))
-            }
-            _ => Err(parse_error(resp).await?),
+        // should be a 307 TEMPORARY_REDIRECT
+        if resp.status() != StatusCode::TEMPORARY_REDIRECT {
+            return Err(parse_error(resp).await?);
         }
-    }
+        let re_url = self.follow_redirect(resp)?;
 
-    async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.append() {
-            return Err(Error::new(
-                ErrorKind::Unsupported,
-                "append write is not supported",
-            ));
+        let mut re_builder = Request::put(re_url);
+        if let Some(size) = size {
+            re_builder = re_builder.header(CONTENT_LENGTH, size.to_string());
+        }
+        if let Some(content_type) = content_type {
+            re_builder = re_builder.header(CONTENT_TYPE, content_type);
         }
 
-        Ok((
-            RpWrite::default(),
-            OssWriter::new(self.clone(), args, path.to_string()),
-        ))
+        re_builder.body(body).map_err(new_request_build_error)
     }
 
-    async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
-        if path == "/" {
-            let m = Metadata::new(EntryMode::DIR);
-            return Ok(RpStat::new(m));
+    async fn webhdfs_open_req(&self, path: &str, range: &BytesRange) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+        let mut url = format!(
+            "{}/webhdfs/v1/{}?op=OPEN",
+            self.endpoint,
+            percent_encode_path(&p),
+        );
+        if let Some(auth) = &self.auth {
+            url += format!("&{auth}").as_str();
         }
 
-        let resp = self.oss_head_object(path).await?;
-
-        let status = resp.status();
-
-        match status {
-            StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
-            StatusCode::NOT_FOUND if path.ends_with('/') => {
-                let m = Metadata::new(EntryMode::DIR);
-                Ok(RpStat::new(m))
+        // make a Webhdfs compatible bytes range
+        //
+        // Webhdfs does not support read from end
+        // have to solve manually
+        let range = match (range.offset(), range.size()) {
+            // avoiding reading the whole file
+            (None, Some(size)) => {
+                debug!("converting bytes range to webhdfs compatible");
+                let status = self.stat(path, OpStat::default()).await?;
+                let total_size = status.into_metadata().content_length();
+                let offset = total_size - size;
+                BytesRange::new(Some(offset), Some(size))
             }
+            _ => *range,
+        };
 
-            _ => Err(parse_error(resp).await?),
-        }
-    }
+        let (offset, size) = (range.offset(), range.size());
 
-    async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let resp = self.oss_delete_object(path).await?;
-        let status = resp.status();
-        match status {
-            StatusCode::NO_CONTENT | StatusCode::NOT_FOUND => {
-                resp.into_body().consume().await?;
-                Ok(RpDelete::default())
+        match (offset, size) {
+            (Some(offset), Some(size)) => {
+                url += format!("&offset={offset}&length={size}").as_str();
+            }
+            (Some(offset), None) => {
+                url += format!("&offset={offset}").as_str();
+            }
+            (None, None) => {
+                // read all, do nothing
+            }
+            (None, Some(_)) => {
+                // already handled
+                unreachable!()
             }
-            _ => Err(parse_error(resp).await?),
         }
-    }
-
-    async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
-        Ok((
-            RpList::default(),
-            OssPager::new(Arc::new(self.clone()), &self.root, path, "/", args.limit()),
-        ))
-    }
-
-    async fn scan(&self, path: &str, args: OpScan) -> Result<(RpScan, Self::Pager)> {
-        Ok((
-            RpScan::default(),
-            OssPager::new(Arc::new(self.clone()), &self.root, path, "", args.limit()),
-        ))
-    }
-
-    fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
-        // We will not send this request out, just for signing.
-        let mut req = match args.operation() {
-            PresignOperation::Stat(_) => self.oss_head_object_request(path, true)?,
-            PresignOperation::Read(v) => self.oss_get_object_request(path, v.range(), true)?,
-            PresignOperation::Write(v) => self.oss_put_object_request(
-                path,
-                None,
-                v.content_type(),
-                v.content_disposition(),
-                AsyncBody::Empty,
-                true,
-            )?,
-        };
-
-        self.signer
-            .sign_query(&mut req, args.expire())
-            .map_err(new_request_sign_error)?;
-
-        // We don't need this request anymore, consume it directly.
-        let (parts, _) = req.into_parts();
-
-        Ok(RpPresign::new(PresignedRequest::new(
-            parts.method,
-            parts.uri,
-            parts.headers,
-        )))
-    }
-
-    async fn batch(&self, args: OpBatch) -> Result<RpBatch> {
-        let ops = args.into_operation();
-        match ops {
-            BatchOperations::Delete(ops) => {
-                // Sadly, OSS will not return failed keys, so we will build
-                // a set to calculate the failed keys.
-                let mut keys = HashSet::new();
-
-                let ops_len = ops.len();
-                if ops_len > 1000 {
-                    return Err(Error::new(
-                        ErrorKind::Unsupported,
-                        "oss services only allow delete up to 1000 keys at once",
-                    )
-                    .with_context("length", ops_len.to_string()));
-                }
 
-                let paths = ops
-                    .into_iter()
-                    .map(|(p, _)| {
-                        keys.insert(p.clone());
-                        p
-                    })
-                    .collect();
-
-                let resp = self.oss_delete_objects(paths).await?;
-
-                let status = resp.status();
-
-                if let StatusCode::OK = status {
-                    let bs = resp.into_body().bytes().await?;
-
-                    let result: DeleteObjectsResult = quick_xml::de::from_reader(bs.reader())
-                        .map_err(new_xml_deserialize_error)?;
-
-                    let mut batched_result = Vec::with_capacity(ops_len);
-                    for i in result.deleted {
-                        let path = build_rel_path(&self.root, &i.key);
-                        keys.remove(&path);
-                        batched_result.push((path, Ok(RpDelete::default())));
-                    }
-                    // TODO: we should handle those errors with code.
-                    for i in keys {
-                        batched_result.push((
-                            i,
-                            Err(Error::new(
-                                ErrorKind::Unexpected,
-                                "oss delete this key failed for reason we don't know",
-                            )),
-                        ));
-                    }
+        let req = Request::get(&url)
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
 
-                    Ok(RpBatch::new(BatchedResults::Delete(batched_result)))
-                } else {
-                    Err(parse_error(resp).await?)
-                }
-            }
-        }
+        Ok(req)
     }
-}
 
-impl OssBackend {
-    pub fn oss_put_object_request(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        content_type: Option<&str>,
-        content_disposition: Option<&str>,
-        body: AsyncBody,
-        is_presign: bool,
-    ) -> Result<Request<AsyncBody>> {
+    fn webhdfs_list_status_req(&self, path: &str) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
-        let endpoint = self.get_endpoint(is_presign);
-        let url = format!("{}/{}", endpoint, percent_encode_path(&p));
-
-        let mut req = Request::put(&url);
-
-        req = req.header(CONTENT_LENGTH, size.unwrap_or_default());
-
-        if let Some(mime) = content_type {
-            req = req.header(CONTENT_TYPE, mime);
-        }
-
-        if let Some(pos) = content_disposition {
-            req = req.header(CONTENT_DISPOSITION, pos);
+        let mut url = format!(
+            "{}/webhdfs/v1/{}?op=LISTSTATUS",
+            self.endpoint,
+            percent_encode_path(&p),
+        );
+        if let Some(auth) = &self.auth {
+            url += format!("&{auth}").as_str();
         }
 
-        let req = req.body(body).map_err(new_request_build_error)?;
+        let req = Request::get(&url);
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
         Ok(req)
     }
+}
 
-    fn oss_get_object_request(
+impl WebhdfsBackend {
+    /// get object from webhdfs
+    ///
+    /// # Notes
+    ///
+    /// looks like webhdfs doesn't support range request from file end.
+    /// so if we want to read the tail of object, the whole object should be transferred.
+    async fn webhdfs_get_object(
         &self,
         path: &str,
         range: BytesRange,
-        is_presign: bool,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-        let endpoint = self.get_endpoint(is_presign);
-        let url = format!("{}/{}", endpoint, percent_encode_path(&p));
-
-        let mut req = Request::get(&url);
-        req = req.header(CONTENT_TYPE, "application/octet-stream");
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let req = self.webhdfs_open_req(path, &range).await?;
+        let resp = self.client.send(req).await?;
 
-        if !range.is_full() {
-            req = req.header(RANGE, range.to_header());
-            // Adding `x-oss-range-behavior` header to use standard behavior.
-            // ref: https://help.aliyun.com/document_detail/39571.html
-            req = req.header("x-oss-range-behavior", "standard");
+        // this should be a 307 redirect
+        if resp.status() != StatusCode::TEMPORARY_REDIRECT {
+            return Err(parse_error(resp).await?);
         }
 
-        let req = req
+        let re_url = self.follow_redirect(resp)?;
+        let re_req = Request::get(&re_url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
-
-        Ok(req)
+        self.client.send(re_req).await
     }
 
-    fn oss_delete_object_request(&self, path: &str) -> Result<Request<AsyncBody>> {
+    async fn webhdfs_status_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
-        let endpoint = self.get_endpoint(false);
-        let url = format!("{}/{}", endpoint, percent_encode_path(&p));
-        let req = Request::delete(&url);
+        let mut url = format!(
+            "{}/webhdfs/v1/{}?op=GETFILESTATUS",
+            self.endpoint,
+            percent_encode_path(&p),
+        );
+        debug!("webhdfs status url: {}", url);
+        if let Some(auth) = &self.auth {
+            url += format!("&{auth}").as_str();
+        }
 
+        let req = Request::get(&url);
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        Ok(req)
+        self.client.send(req).await
     }
 
-    fn oss_head_object_request(&self, path: &str, is_presign: bool) -> Result<Request<AsyncBody>> {
+    async fn webhdfs_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
-        let endpoint = self.get_endpoint(is_presign);
-        let url = format!("{}/{}", endpoint, percent_encode_path(&p));
+        let mut url = format!(
+            "{}/webhdfs/v1/{}?op=DELETE&recursive=false",
+            self.endpoint,
+            percent_encode_path(&p),
+        );
+        if let Some(auth) = &self.auth {
+            url += format!("&{auth}").as_str();
+        }
 
-        let req = Request::head(&url);
+        let req = Request::delete(&url);
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        Ok(req)
+        self.client.send(req).await
     }
+}
 
-    fn oss_list_object_request(
-        &self,
-        path: &str,
-        token: Option<&str>,
-        delimiter: &str,
-        limit: Option<usize>,
-    ) -> Result<Request<AsyncBody>> {
-        let p = build_abs_path(&self.root, path);
-
-        let endpoint = self.get_endpoint(false);
-        let url = format!(
-            "{}/?list-type=2&delimiter={delimiter}&prefix={}{}{}",
-            endpoint,
-            percent_encode_path(&p),
-            limit.map(|t| format!("&max-keys={t}")).unwrap_or_default(),
-            token
-                .map(|t| format!("&continuation-token={}", percent_encode_path(t)))
-                .unwrap_or_default(),
-        );
-
-        let req = Request::get(&url)
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
-        Ok(req)
+impl WebhdfsBackend {
+    /// get redirect destination from 307 TEMPORARY_REDIRECT http response
+    fn follow_redirect(&self, resp: Response<IncomingAsyncBody>) -> Result<String> {
+        let loc = match parse_location(resp.headers())? {
+            Some(p) => {
+                if !p.starts_with('/') {
+                    // is not relative path
+                    p.to_string()
+                } else {
+                    // is relative path
+                    // prefix with endpoint url
+                    let url = self.endpoint.clone();
+                    format!("{url}/{p}")
+                }
+            }
+            None => {
+                let err = Error::new(
+                    ErrorKind::Unexpected,
+                    "redirection fail: no location header",
+                );
+                return Err(err);
+            }
+        };
+        Ok(loc)
     }
 
-    async fn oss_get_object(
-        &self,
-        path: &str,
-        range: BytesRange,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.oss_get_object_request(path, range, false)?;
+    fn consume_success_mkdir(&self, path: &str, parts: Parts, body: &str) -> Result<RpCreate> {
+        let mkdir_rsp = serde_json::from_str::<BooleanResp>(body).map_err(|e| {
+            Error::new(ErrorKind::Unexpected, "cannot parse mkdir response")
+                .set_temporary()
+                .with_context("service", Scheme::Webhdfs)
+                .with_context("response", format!("{parts:?}"))
+                .set_source(e)
+        })?;
 
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-        self.client.send_async(req).await
+        if mkdir_rsp.boolean {
+            Ok(RpCreate::default())
+        } else {
+            Err(Error::new(
+                ErrorKind::Unexpected,
+                &format!("mkdir failed: {path}"),
+            ))
+        }
     }
 
-    async fn oss_head_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.oss_head_object_request(path, false)?;
-
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-        self.client.send_async(req).await
-    }
+    async fn check_root(&self) -> Result<()> {
+        let resp = self.webhdfs_status_object("/").await?;
+        match resp.status() {
+            StatusCode::OK => {
+                let body_bs = resp.into_body().bytes().await?;
+
+                let file_status = serde_json::from_reader::<_, FileStatusWrapper>(body_bs.reader())
+                    .map_err(|e| {
+                        Error::new(ErrorKind::Unexpected, "cannot parse returned json")
+                            .with_context("service", Scheme::Webhdfs)
+                            .set_source(e)
+                    })?
+                    .file_status;
+
+                match file_status.ty {
+                    FileStatusType::File => {
+                        error!("working directory is occupied!");
+                        return Err(Error::new(ErrorKind::ConfigInvalid, "root is occupied!")
+                            .with_context("service", Scheme::Webhdfs));
+                    }
+                    FileStatusType::Directory => {
+                        debug!("working directory exists, do nothing");
+                    }
+                }
+            }
 
-    async fn oss_put_object(
-        &self,
-        path: &str,
-        size: Option<usize>,
-        content_type: Option<&str>,
-        content_disposition: Option<&str>,
-        body: AsyncBody,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.oss_put_object_request(
-            path,
-            size,
-            content_type,
-            content_disposition,
-            body,
-            false,
-        )?;
+            StatusCode::NOT_FOUND => {
+                debug!("working directory does not exists, creating...");
+                self.create("/", OpCreate::new(EntryMode::DIR)).await?;
+            }
 
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-        self.client.send_async(req).await
+            _ => return Err(parse_error(resp).await?),
+        }
+        debug!("working directory is ready!");
+        Ok(())
     }
+}
 
-    pub(super) async fn oss_list_object(
-        &self,
-        path: &str,
-        token: Option<&str>,
-        delimiter: &str,
-        limit: Option<usize>,
-    ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.oss_list_object_request(path, token, delimiter, limit)?;
+#[async_trait]
+impl Accessor for WebhdfsBackend {
+    type Reader = IncomingAsyncBody;
+    type BlockingReader = ();
+    type Writer = WebhdfsWriter;
+    type BlockingWriter = ();
+    type Pager = WebhdfsPager;
+    type BlockingPager = ();
 
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-        self.client.send_async(req).await
+    fn info(&self) -> AccessorInfo {
+        let mut am = AccessorInfo::default();
+        am.set_scheme(Scheme::Webhdfs)
+            .set_root(&self.root)
+            .set_capabilities(
+                AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
+            )
+            .set_hints(AccessorHint::ReadStreamable);
+        am
     }
 
-    async fn oss_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.oss_delete_object_request(path)?;
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
-        self.client.send_async(req).await
-    }
-
-    async fn oss_delete_objects(&self, paths: Vec<String>) -> Result<Response<IncomingAsyncBody>> {
-        let url = format!("{}/?delete", self.endpoint);
-
-        let req = Request::post(&url);
-
-        let content = quick_xml::se::to_string(&DeleteObjectsRequest {
-            object: paths
-                .into_iter()
-                .map(|path| DeleteObjectsRequestObject {
-                    key: build_abs_path(&self.root, &path),
-                })
-                .collect(),
-        })
-        .map_err(new_xml_deserialize_error)?;
-
-        // Make sure content length has been set to avoid post with chunked encoding.
-        let req = req.header(CONTENT_LENGTH, content.len());
-        // Set content-type to `application/xml` to avoid mixed with form post.
-        let req = req.header(CONTENT_TYPE, "application/xml");
-        // Set content-md5 as required by API.
-        let req = req.header("CONTENT-MD5", format_content_md5(content.as_bytes()));
+    /// Create a file or directory
+    async fn create(&self, path: &str, args: OpCreate) -> Result<RpCreate> {
+        // if the path ends with '/', it will be treated as a directory
+        // otherwise, it will be treated as a file
+        let path = if args.mode().is_file() && path.ends_with('/') {
+            path.trim_end_matches('/').to_owned()
+        } else if args.mode().is_dir() && !path.ends_with('/') {
+            path.to_owned() + "/"
+        } else {
+            path.to_owned()
+        };
 
-        let mut req = req
-            .body(AsyncBody::Bytes(Bytes::from(content)))
-            .map_err(new_request_build_error)?;
+        let req = self
+            .webhdfs_create_object_req(&path, Some(0), None, AsyncBody::Empty)
+            .await?;
 
-        self.signer.sign(&mut req).map_err(new_request_sign_error)?;
+        let resp = self.client.send(req).await?;
 
-        self.client.send_async(req).await
-    }
+        let status = resp.status();
 
-    fn get_endpoint(&self, is_presign: bool) -> &str {
-        if is_presign {
-            &self.presign_endpoint
-        } else {
-            &self.endpoint
+        // WebHDFS's has a two-step create/append to prevent clients to send out
+        // data before creating it.
+        // According to the redirect policy of `reqwest` HTTP Client we are using,
+        // the redirection should be done automatically.
+        match status {
+            StatusCode::CREATED | StatusCode::OK => {
+                if !path.ends_with('/') {
+                    // create file's http resp could be ignored
+                    resp.into_body().consume().await?;
+                    return Ok(RpCreate::default());
+                }
+                let (parts, body) = resp.into_parts();
+                let bs = body.bytes().await?;
+                let s = String::from_utf8_lossy(&bs);
+                self.consume_success_mkdir(&path, parts, &s)
+            }
+            _ => Err(parse_error(resp).await?),
         }
     }
-}
 
-/// Request of DeleteObjects.
-#[derive(Default, Debug, Serialize)]
-#[serde(default, rename = "Delete", rename_all = "PascalCase")]
-struct DeleteObjectsRequest {
-    object: Vec<DeleteObjectsRequestObject>,
-}
-
-#[derive(Default, Debug, Serialize)]
-#[serde(rename_all = "PascalCase")]
-struct DeleteObjectsRequestObject {
-    key: String,
-}
+    async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
+        let range = args.range();
+        let resp = self.webhdfs_get_object(path, range).await?;
+        match resp.status() {
+            StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
+                let meta = parse_into_metadata(path, resp.headers())?;
+                Ok((RpRead::with_metadata(meta), resp.into_body()))
+            }
+            StatusCode::NOT_FOUND => Err(Error::new(ErrorKind::NotFound, "object not found")
+                .with_context("service", Scheme::Webhdfs)),
+            _ => Err(parse_error(resp).await?),
+        }
+    }
 
-/// Result of DeleteObjects.
-#[derive(Default, Debug, Deserialize)]
-#[serde(default, rename = "DeleteResult", rename_all = "PascalCase")]
-struct DeleteObjectsResult {
-    deleted: Vec<DeleteObjectsResultDeleted>,
-}
+    async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
+        if args.append() {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "append write is not supported",
+            ));
+        }
 
-#[derive(Default, Debug, Deserialize)]
-#[serde(rename_all = "PascalCase")]
-struct DeleteObjectsResultDeleted {
-    key: String,
-}
+        Ok((
+            RpWrite::default(),
+            WebhdfsWriter::new(self.clone(), args, path.to_string()),
+        ))
+    }
 
-#[derive(Default, Debug, Deserialize)]
-#[serde(default, rename_all = "PascalCase")]
-struct DeleteObjectsResultError {
-    code: String,
-    key: String,
-    message: String,
-}
+    async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
+        // if root exists and is a directory, stat will be ok
+        self.root_checker
+            .get_or_try_init(|| async { self.check_root().await })
+            .await?;
 
-#[cfg(test)]
-mod tests {
-    use bytes::Buf;
-    use bytes::Bytes;
-
-    use super::*;
-
-    /// This example is from https://www.alibabacloud.com/help/zh/object-storage-service/latest/deletemultipleobjects
-    #[test]
-    fn test_serialize_delete_objects_request() {
-        let req = DeleteObjectsRequest {
-            object: vec![
-                DeleteObjectsRequestObject {
-                    key: "multipart.data".to_string(),
-                },
-                DeleteObjectsRequestObject {
-                    key: "test.jpg".to_string(),
-                },
-                DeleteObjectsRequestObject {
-                    key: "demo.jpg".to_string(),
-                },
-            ],
-        };
+        let resp = self.webhdfs_status_object(path).await?;
+        let status = resp.status();
+        match status {
+            StatusCode::OK => {
+                debug!("stat object: {} ok", path);
+                let mut meta = parse_into_metadata(path, resp.headers())?;
+                let body_bs = resp.into_body().bytes().await?;
+
+                let file_status = serde_json::from_reader::<_, FileStatusWrapper>(body_bs.reader())
+                    .map_err(|e| {
+                        Error::new(ErrorKind::Unexpected, "cannot parse returned json")
+                            .with_context("service", Scheme::Webhdfs)
+                            .set_source(e)
+                    })?
+                    .file_status;
+                debug!("file status: {:?}", file_status);
+                let status_meta: Metadata = file_status.try_into()?;
+
+                // is ok to unwrap here
+                // all metadata field of status meta is present and checked by `TryFrom`
+                meta.set_last_modified(status_meta.last_modified().unwrap())
+                    .set_content_length(status_meta.content_length());
+                Ok(RpStat::new(meta))
+            }
 
-        let actual = quick_xml::se::to_string(&req).expect("must succeed");
+            _ => Err(parse_error(resp).await?),
+        }
+    }
 
-        pretty_assertions::assert_eq!(
-            actual,
-            r#"<Delete>
-  <Object>
-    <Key>multipart.data</Key>
-  </Object>
-  <Object>
-    <Key>test.jpg</Key>
-  </Object>
-  <Object>
-    <Key>demo.jpg</Key>
-  </Object>
-</Delete>"#
-                // Cleanup space and new line
-                .replace([' ', '\n'], "")
-        )
-    }
-
-    /// This example is from https://www.alibabacloud.com/help/zh/object-storage-service/latest/deletemultipleobjects
-    #[test]
-    fn test_deserialize_delete_objects_result() {
-        let bs = Bytes::from(
-            r#"<?xml version="1.0" encoding="UTF-8"?>
-<DeleteResult xmlns="http://doc.oss-cn-hangzhou.aliyuncs.com">
-    <Deleted>
-       <Key>multipart.data</Key>
-    </Deleted>
-    <Deleted>
-       <Key>test.jpg</Key>
-    </Deleted>
-    <Deleted>
-       <Key>demo.jpg</Key>
-    </Deleted>
-</DeleteResult>"#,
-        );
+    async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
+        let resp = self.webhdfs_delete_object(path).await?;
+        match resp.status() {
+            StatusCode::OK => {
+                resp.into_body().consume().await?;
+                Ok(RpDelete::default())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
+    }
 
-        let out: DeleteObjectsResult =
-            quick_xml::de::from_reader(bs.reader()).expect("must success");
+    async fn list(&self, path: &str, _: OpList) -> Result<(RpList, Self::Pager)> {
+        let path = path.trim_end_matches('/');
+        let req = self.webhdfs_list_status_req(path)?;
+
+        let resp = self.client.send(req).await?;
+        match resp.status() {
+            StatusCode::OK => {
+                let body_bs = resp.into_body().bytes().await?;
+                let file_statuses =
+                    serde_json::from_reader::<_, FileStatusesWrapper>(body_bs.reader())
+                        .map_err(|e| {
+                            Error::new(ErrorKind::Unexpected, "cannot parse returned json")
+                                .with_context("service", Scheme::Webhdfs)
+                                .set_source(e)
+                        })?
+                        .file_statuses
+                        .file_status;
 
-        assert_eq!(out.deleted.len(), 3);
-        assert_eq!(out.deleted[0].key, "multipart.data");
-        assert_eq!(out.deleted[1].key, "test.jpg");
-        assert_eq!(out.deleted[2].key, "demo.jpg");
+                let objects = WebhdfsPager::new(path, file_statuses);
+                Ok((RpList::default(), objects))
+            }
+            StatusCode::NOT_FOUND => {
+                let objects = WebhdfsPager::new(path, vec![]);
+                Ok((RpList::default(), objects))
+            }
+            _ => Err(parse_error(resp).await?),
+        }
     }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::OssBuilder as Oss;
+pub use backend::WebdavBuilder as Webdav;
 
 mod error;
+mod list_response;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files 6% similar despite different names*

```diff
@@ -18,48 +18,39 @@
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Buf;
 use quick_xml::de;
 use quick_xml::escape::unescape;
 use serde::Deserialize;
-use time::format_description::well_known::Rfc3339;
-use time::OffsetDateTime;
 
-use super::backend::OssBackend;
+use super::core::*;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::EntryMode;
 use crate::Error;
 use crate::ErrorKind;
 use crate::Metadata;
 use crate::Result;
 
 pub struct OssPager {
-    backend: Arc<OssBackend>,
-    root: String,
+    core: Arc<OssCore>,
+
     path: String,
     delimiter: String,
     limit: Option<usize>,
 
     token: Option<String>,
     done: bool,
 }
 
 impl OssPager {
-    pub fn new(
-        backend: Arc<OssBackend>,
-        root: &str,
-        path: &str,
-        delimiter: &str,
-        limit: Option<usize>,
-    ) -> Self {
+    pub fn new(core: Arc<OssCore>, path: &str, delimiter: &str, limit: Option<usize>) -> Self {
         Self {
-            backend,
-            root: root.to_string(),
+            core,
             path: path.to_string(),
             delimiter: delimiter.to_string(),
             limit,
 
             token: None,
 
             done: false,
@@ -71,15 +62,15 @@
 impl oio::Page for OssPager {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         if self.done {
             return Ok(None);
         }
 
         let resp = self
-            .backend
+            .core
             .oss_list_object(
                 &self.path,
                 self.token.as_deref(),
                 &self.delimiter,
                 self.limit,
             )
             .await?;
@@ -96,40 +87,31 @@
         self.done = !output.is_truncated;
         self.token = output.next_continuation_token.clone();
 
         let mut entries = Vec::with_capacity(output.common_prefixes.len() + output.contents.len());
 
         for prefix in output.common_prefixes {
             let de = oio::Entry::new(
-                &build_rel_path(&self.root, &prefix.prefix),
+                &build_rel_path(&self.core.root, &prefix.prefix),
                 Metadata::new(EntryMode::DIR),
             );
             entries.push(de);
         }
 
         for object in output.contents {
             if object.key.ends_with('/') {
                 continue;
             }
             let mut meta = Metadata::new(EntryMode::FILE);
 
             meta.set_etag(&object.etag);
             meta.set_content_length(object.size);
-            let dt = OffsetDateTime::parse(object.last_modified.as_str(), &Rfc3339)
-                .map(|v| {
-                    v.replace_nanosecond(0)
-                        .expect("replace nanosecond of last modified must succeed")
-                })
-                .map_err(|e| {
-                    Error::new(ErrorKind::Unexpected, "parse str into rfc 3339 datetime")
-                        .set_source(e)
-                })?;
-            meta.set_last_modified(dt);
+            meta.set_last_modified(parse_datetime_from_rfc3339(object.last_modified.as_str())?);
 
-            let rel = build_rel_path(&self.root, &object.key);
+            let rel = build_rel_path(&self.core.root, &object.key);
             let path = unescape(&rel)
                 .map_err(|e| Error::new(ErrorKind::Unexpected, "excapse xml").set_source(e))?;
             let de = oio::Entry::new(&path, meta);
             entries.push(de);
         }
 
         Ok(Some(entries))
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files 14% similar despite different names*

```diff
@@ -15,56 +15,51 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::OssBackend;
+use super::backend::WebdavBackend;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct OssWriter {
-    backend: OssBackend,
+pub struct WebdavWriter {
+    backend: WebdavBackend,
 
     op: OpWrite,
     path: String,
 }
 
-impl OssWriter {
-    pub fn new(backend: OssBackend, op: OpWrite, path: String) -> Self {
-        OssWriter { backend, op, path }
+impl WebdavWriter {
+    pub fn new(backend: WebdavBackend, op: OpWrite, path: String) -> Self {
+        WebdavWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for OssWriter {
+impl oio::Write for WebdavWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut req = self.backend.oss_put_object_request(
-            &self.path,
-            Some(bs.len()),
-            self.op.content_type(),
-            self.op.content_disposition(),
-            AsyncBody::Bytes(bs),
-            false,
-        )?;
-
-        self.backend
-            .signer
-            .sign(&mut req)
-            .map_err(new_request_sign_error)?;
-
-        let resp = self.backend.client.send_async(req).await?;
+        let resp = self
+            .backend
+            .webdav_put(
+                &self.path,
+                Some(bs.len()),
+                self.op.content_type(),
+                self.op.content_disposition(),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
 
         let status = resp.status();
 
         match status {
-            StatusCode::CREATED | StatusCode::OK => {
+            StatusCode::CREATED | StatusCode::OK | StatusCode::NO_CONTENT => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files 22% similar despite different names*

```diff
@@ -12,8 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::RedisBuilder as Redis;
+pub use backend::ObsBuilder as Obs;
+
+mod core;
+mod error;
+mod pager;
+mod writer;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.31.0/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::S3Builder as S3;
+pub use backend::AzdfsBuilder as Azdfs;
 
+mod core;
 mod error;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files 8% similar despite different names*

```diff
@@ -17,48 +17,38 @@
 
 use std::sync::Arc;
 
 use async_trait::async_trait;
 use bytes::Buf;
 use quick_xml::de;
 use serde::Deserialize;
-use time::format_description::well_known::Rfc3339;
-use time::OffsetDateTime;
 
-use super::backend::S3Backend;
+use super::core::S3Core;
 use super::error::parse_error;
 use crate::raw::*;
 use crate::EntryMode;
-use crate::Error;
-use crate::ErrorKind;
 use crate::Metadata;
 use crate::Result;
 
 pub struct S3Pager {
-    backend: Arc<S3Backend>,
-    root: String,
+    core: Arc<S3Core>,
+
     path: String,
     delimiter: String,
     limit: Option<usize>,
 
     token: String,
     done: bool,
 }
 
 impl S3Pager {
-    pub fn new(
-        backend: Arc<S3Backend>,
-        root: &str,
-        path: &str,
-        delimiter: &str,
-        limit: Option<usize>,
-    ) -> Self {
+    pub fn new(core: Arc<S3Core>, path: &str, delimiter: &str, limit: Option<usize>) -> Self {
         Self {
-            backend,
-            root: root.to_string(),
+            core,
+
             path: path.to_string(),
             delimiter: delimiter.to_string(),
             limit,
 
             token: "".to_string(),
             done: false,
         }
@@ -69,15 +59,15 @@
 impl oio::Page for S3Pager {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         if self.done {
             return Ok(None);
         }
 
         let resp = self
-            .backend
+            .core
             .s3_list_objects(&self.path, &self.token, &self.delimiter, self.limit)
             .await?;
 
         if resp.status() != http::StatusCode::OK {
             return Err(parse_error(resp).await?);
         }
 
@@ -99,15 +89,15 @@
         };
         self.token = output.next_continuation_token.clone().unwrap_or_default();
 
         let mut entries = Vec::with_capacity(output.common_prefixes.len() + output.contents.len());
 
         for prefix in output.common_prefixes {
             let de = oio::Entry::new(
-                &build_rel_path(&self.root, &prefix.prefix),
+                &build_rel_path(&self.core.root, &prefix.prefix),
                 Metadata::new(EntryMode::DIR),
             );
 
             entries.push(de);
         }
 
         for object in output.contents {
@@ -122,29 +112,17 @@
 
             meta.set_etag(&object.etag);
             meta.set_content_md5(object.etag.trim_matches('"'));
             meta.set_content_length(object.size);
 
             // object.last_modified provides more precious time that contains
             // nanosecond, let's trim them.
-            let dt = OffsetDateTime::parse(object.last_modified.as_str(), &Rfc3339)
-                .map(|v| {
-                    v.replace_nanosecond(0)
-                        .expect("replace nanosecond of last modified must succeed")
-                })
-                .map_err(|e| {
-                    Error::new(
-                        ErrorKind::Unexpected,
-                        "parse last modified RFC3339 datetime",
-                    )
-                    .set_source(e)
-                })?;
-            meta.set_last_modified(dt);
+            meta.set_last_modified(parse_datetime_from_rfc3339(object.last_modified.as_str())?);
 
-            let de = oio::Entry::new(&build_rel_path(&self.root, &object.key), meta);
+            let de = oio::Entry::new(&build_rel_path(&self.core.root, &object.key), meta);
 
             entries.push(de);
         }
 
         Ok(Some(entries))
     }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files 10% similar despite different names*

```diff
@@ -11,70 +11,62 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::CompleteMultipartUploadRequestPart;
-use super::backend::S3Backend;
+use super::core::*;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct S3Writer {
-    backend: S3Backend,
+pub struct OssWriter {
+    core: Arc<OssCore>,
 
     op: OpWrite,
     path: String,
-
     upload_id: Option<String>,
-    parts: Vec<CompleteMultipartUploadRequestPart>,
+    parts: Vec<MultipartUploadPart>,
 }
 
-impl S3Writer {
-    pub fn new(backend: S3Backend, op: OpWrite, path: String, upload_id: Option<String>) -> Self {
-        S3Writer {
-            backend,
+impl OssWriter {
+    pub fn new(core: Arc<OssCore>, op: OpWrite, path: String, upload_id: Option<String>) -> Self {
+        OssWriter {
+            core,
             op,
             path,
             upload_id,
             parts: vec![],
         }
     }
 }
 
 #[async_trait]
-impl oio::Write for S3Writer {
+impl oio::Write for OssWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        debug_assert!(
-            self.upload_id.is_none(),
-            "Writer initiated with upload id, but users trying to call write, must be buggy"
-        );
-
-        let mut req = self.backend.s3_put_object_request(
+        let mut req = self.core.oss_put_object_request(
             &self.path,
             Some(bs.len()),
             self.op.content_type(),
             self.op.content_disposition(),
-            self.op.cache_control(),
             AsyncBody::Bytes(bs),
+            false,
         )?;
 
-        self.backend
-            .signer
-            .sign(&mut req)
-            .map_err(new_request_sign_error)?;
+        self.core.sign(&mut req).await?;
 
-        let resp = self.backend.client.send_async(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
@@ -83,71 +75,61 @@
         }
     }
 
     async fn append(&mut self, bs: Bytes) -> Result<()> {
         let upload_id = self.upload_id.as_ref().expect(
             "Writer doesn't have upload id, but users trying to call append, must be buggy",
         );
-        // AWS S3 requires part number must between [1..=10000]
+        // Aliyun OSS requires part number must between [1..=10000]
         let part_number = self.parts.len() + 1;
+        let mut req = self
+            .core
+            .oss_upload_part_request(
+                &self.path,
+                upload_id,
+                part_number,
+                false,
+                Some(bs.len() as u64),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
 
-        let mut req = self.backend.s3_upload_part_request(
-            &self.path,
-            upload_id,
-            part_number,
-            Some(bs.len() as u64),
-            AsyncBody::Bytes(bs),
-        )?;
-
-        self.backend
-            .signer
-            .sign(&mut req)
-            .map_err(new_request_sign_error)?;
-
-        let resp = self.backend.client.send_async(req).await?;
-
-        let status = resp.status();
+        self.core.sign(&mut req).await?;
 
-        match status {
+        let resp = self.core.send(req).await?;
+        match resp.status() {
             StatusCode::OK => {
                 let etag = parse_etag(resp.headers())?
                     .ok_or_else(|| {
                         Error::new(
                             ErrorKind::Unexpected,
                             "ETag not present in returning response",
                         )
                     })?
                     .to_string();
-
                 resp.into_body().consume().await?;
-
-                self.parts
-                    .push(CompleteMultipartUploadRequestPart { part_number, etag });
-
+                self.parts.push(MultipartUploadPart { part_number, etag });
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn close(&mut self) -> Result<()> {
         let upload_id = if let Some(upload_id) = &self.upload_id {
             upload_id
         } else {
             return Ok(());
         };
 
         let resp = self
-            .backend
-            .s3_complete_multipart_upload(&self.path, upload_id, &self.parts)
+            .core
+            .oss_complete_multipart_upload_request(&self.path, upload_id, false, &self.parts)
             .await?;
-
-        let status = resp.status();
-
-        match status {
+        match resp.status() {
             StatusCode::OK => {
                 resp.into_body().consume().await?;
 
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files 3% similar despite different names*

```diff
@@ -51,24 +51,22 @@
 /// # Example
 ///
 /// ## Via Builder
 ///
 /// ```no_run
 /// use anyhow::Result;
 /// use opendal::services::Sled;
-/// use opendal::Object;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
 ///     let mut builder = Sled::default();
 ///     builder.datadir("/tmp/opendal/sled");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
-///     let _: Object = op.object("test_file");
 ///     Ok(())
 /// }
 /// ```
 #[derive(Default)]
 pub struct SledBuilder {
     /// That path to the sled data directory.
     datadir: Option<String>,
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -12,9 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
+pub use backend::WebhdfsBuilder as Webhdfs;
 
-pub use backend::SledBuilder as Sled;
+mod error;
+mod message;
+mod pager;
+mod writer;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files 8% similar despite different names*

```diff
@@ -17,37 +17,39 @@
 
 use std::collections::HashMap;
 use std::fmt::Debug;
 use std::fmt::Formatter;
 
 use async_trait::async_trait;
 use bytes::Buf;
+use http::header;
+use http::HeaderMap;
 use http::Request;
 use http::Response;
 use http::StatusCode;
-use http::{header, HeaderMap};
 use log::debug;
 
-use crate::ops::*;
-use crate::raw::*;
-use crate::*;
-
 use super::error::parse_error;
 use super::list_response::Multistatus;
 use super::pager::WebdavPager;
 use super::writer::WebdavWriter;
+use crate::ops::*;
+use crate::raw::*;
+use crate::*;
 
 /// [WebDAV](https://datatracker.ietf.org/doc/html/rfc4918) backend support.
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
+/// - [x] copy
+/// - [x] rename
 /// - [x] list
 /// - [ ] ~~scan~~
 /// - [ ] ~~presign~~
 /// - [ ] blocking
 ///
 /// # Notes
 ///
@@ -261,38 +263,30 @@
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Webdav)
             .set_root(&self.root)
             .set_capabilities(
-                AccessorCapability::Read | AccessorCapability::Write | AccessorCapability::List,
+                AccessorCapability::Read
+                    | AccessorCapability::Write
+                    | AccessorCapability::Copy
+                    | AccessorCapability::Rename
+                    | AccessorCapability::List,
             )
             .set_hints(AccessorHint::ReadStreamable);
 
         ma
     }
 
     async fn create(&self, path: &str, _: OpCreate) -> Result<RpCreate> {
-        // create dir recursively, split path by `/` and create each dir except the last one
-        let abs_path = build_abs_path(&self.root, path);
-        let abs_path = abs_path.as_str();
-        let mut parts: Vec<&str> = abs_path.split('/').filter(|x| !x.is_empty()).collect();
-        if !parts.is_empty() {
-            parts.pop();
-        }
+        self.ensure_parent_path(path).await?;
 
-        let mut sub_path = String::new();
-        for sub_part in parts {
-            let sub_path_with_slash = sub_part.to_owned() + "/";
-            sub_path.push_str(&sub_path_with_slash);
-            self.create_internal(&sub_path).await?;
-        }
-
-        self.create_internal(abs_path).await
+        let abs_path = build_abs_path(&self.root, path);
+        self.create_internal(&abs_path).await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         let resp = self.webdav_get(path, args.range()).await?;
 
         let status = resp.status();
 
@@ -314,14 +308,40 @@
         }
 
         let p = build_abs_path(&self.root, path);
 
         Ok((RpWrite::default(), WebdavWriter::new(self.clone(), args, p)))
     }
 
+    async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
+        self.ensure_parent_path(to).await?;
+
+        let resp = self.webdav_copy(from, to).await?;
+
+        let status = resp.status();
+
+        match status {
+            StatusCode::CREATED | StatusCode::NO_CONTENT => Ok(RpCopy::default()),
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+
+    async fn rename(&self, from: &str, to: &str, _args: OpRename) -> Result<RpRename> {
+        self.ensure_parent_path(to).await?;
+
+        let resp = self.webdav_move(from, to).await?;
+
+        let status = resp.status();
+
+        match status {
+            StatusCode::CREATED | StatusCode::NO_CONTENT => Ok(RpRename::default()),
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+
     async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
         let mut header_map = HeaderMap::new();
@@ -424,15 +444,15 @@
             req = req.header(header::RANGE, range.to_header());
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     pub async fn webdav_put(
         &self,
         abs_path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
@@ -458,15 +478,15 @@
         if let Some(cd) = content_disposition {
             req = req.header(header::CONTENT_DISPOSITION, cd)
         }
 
         // Set body
         let req = req.body(body).map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     async fn webdav_mkcol(
         &self,
         abs_path: &str,
         content_type: Option<&str>,
         content_disposition: Option<&str>,
@@ -485,15 +505,15 @@
 
         if let Some(cd) = content_disposition {
             req = req.header(header::CONTENT_DISPOSITION, cd)
         }
 
         let req = req.body(body).map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     async fn webdav_propfind(
         &self,
         path: &str,
         headers: Option<HeaderMap>,
     ) -> Result<Response<IncomingAsyncBody>> {
@@ -524,15 +544,15 @@
             </D:propfind>
         "#;
             body = AsyncBody::Bytes(bytes::Bytes::from(all_prop_xml_body));
         }
 
         let req = req.body(body).map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
     }
 
     async fn webdav_delete(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
@@ -542,15 +562,65 @@
             req = req.header(header::AUTHORIZATION, auth.clone())
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send_async(req).await
+        self.client.send(req).await
+    }
+
+    async fn webdav_copy(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
+        let source = build_abs_path(&self.root, from);
+        let target = build_abs_path(&self.root, to);
+
+        let source = format!("{}/{}", self.endpoint, percent_encode_path(&source));
+        let target = format!("{}/{}", self.endpoint, percent_encode_path(&target));
+
+        let mut req = Request::builder().method("COPY").uri(&source);
+
+        if let Some(auth) = &self.authorization {
+            req = req.header(header::AUTHORIZATION, auth);
+        }
+
+        req = req.header("Destination", target);
+
+        // We always specific "T" for keeping to overwrite the destination.
+        req = req.header("Overwrite", "T");
+
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        self.client.send(req).await
+    }
+
+    async fn webdav_move(&self, from: &str, to: &str) -> Result<Response<IncomingAsyncBody>> {
+        let source = build_abs_path(&self.root, from);
+        let target = build_abs_path(&self.root, to);
+
+        let source = format!("{}/{}", self.endpoint, percent_encode_path(&source));
+        let target = format!("{}/{}", self.endpoint, percent_encode_path(&target));
+
+        let mut req = Request::builder().method("MOVE").uri(&source);
+
+        if let Some(auth) = &self.authorization {
+            req = req.header(header::AUTHORIZATION, auth);
+        }
+
+        req = req.header("Destination", target);
+
+        // We always specific "T" for keeping to overwrite the destination.
+        req = req.header("Overwrite", "T");
+
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        self.client.send(req).await
     }
 
     async fn create_internal(&self, abs_path: &str) -> Result<RpCreate> {
         let resp = if abs_path.ends_with('/') {
             self.webdav_mkcol(abs_path, None, None, AsyncBody::Empty)
                 .await?
         } else {
@@ -571,8 +641,27 @@
             | StatusCode::NO_CONTENT => {
                 resp.into_body().consume().await?;
                 Ok(RpCreate::default())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
+
+    async fn ensure_parent_path(&self, path: &str) -> Result<()> {
+        // create dir recursively, split path by `/` and create each dir except the last one
+        let abs_path = build_abs_path(&self.root, path);
+        let abs_path = abs_path.as_str();
+        let mut parts: Vec<&str> = abs_path.split('/').filter(|x| !x.is_empty()).collect();
+        if !parts.is_empty() {
+            parts.pop();
+        }
+
+        let mut sub_path = String::new();
+        for sub_part in parts {
+            let sub_path_with_slash = sub_part.to_owned() + "/";
+            sub_path.push_str(&sub_path_with_slash);
+            self.create_internal(&sub_path).await?;
+        }
+
+        Ok(())
+    }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     server_name  localhost;
     access_log   /tmp/access.log;
     root         /tmp/static;
 
     location / {
       client_body_temp_path /tmp;
       log_not_found off;
-      dav_methods PUT DELETE MKCOL;
+      dav_methods PUT DELETE MKCOL COPY MOVE;
       dav_ext_methods PROPFIND;
       create_full_put_path on;
       client_max_body_size 1024M;
       auth_basic           "Administrator’s Area";
       auth_basic_user_file /tmp/htpasswd;
     }
   }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files 25% similar despite different names*

```diff
@@ -13,14 +13,14 @@
     server_name  localhost;
     access_log   /tmp/access.log;
     root         /tmp/static;
 
     location / {
       client_body_temp_path /tmp;
       log_not_found off;
-      dav_methods PUT DELETE MKCOL;
+      dav_methods PUT DELETE MKCOL COPY MOVE;
       dav_ext_methods PROPFIND;
       create_full_put_path on;
       client_max_body_size 1024M;
     }
   }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/list_response.rs`

 * *Files 6% similar despite different names*

```diff
@@ -12,25 +12,28 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use serde::Deserialize;
-use time::format_description::well_known::Rfc2822;
-use time::OffsetDateTime;
 
-use crate::{EntryMode, Error, ErrorKind, Metadata, Result};
+use crate::raw::parse_datetime_from_rfc2822;
+use crate::EntryMode;
+use crate::Error;
+use crate::ErrorKind;
+use crate::Metadata;
+use crate::Result;
 
-#[derive(Deserialize, Debug, PartialEq)]
+#[derive(Deserialize, Debug, PartialEq, Eq)]
 pub struct Multistatus {
     pub response: Vec<ListOpResponse>,
 }
 
-#[derive(Deserialize, Debug, PartialEq)]
+#[derive(Deserialize, Debug, PartialEq, Eq)]
 pub struct ListOpResponse {
     pub href: String,
     pub propstat: Propstat,
 }
 
 impl ListOpResponse {
     pub fn parse_into_metadata(&self) -> Result<Metadata> {
@@ -75,43 +78,43 @@
             m.set_content_type(v);
         }
 
         if let Some(v) = getetag {
             m.set_etag(v);
         }
         // https://www.rfc-editor.org/rfc/rfc4918#section-14.18
-        m.set_last_modified(OffsetDateTime::parse(getlastmodified, &Rfc2822).unwrap());
+        m.set_last_modified(parse_datetime_from_rfc2822(getlastmodified)?);
         Ok(m)
     }
 }
 
-#[derive(Deserialize, Debug, PartialEq)]
+#[derive(Deserialize, Debug, PartialEq, Eq)]
 pub struct Propstat {
     pub prop: Prop,
     pub status: String,
 }
 
-#[derive(Deserialize, Debug, PartialEq)]
+#[derive(Deserialize, Debug, PartialEq, Eq)]
 pub struct Prop {
     #[serde(default)]
     pub displayname: String,
     pub getlastmodified: String,
     pub getetag: Option<String>,
     pub getcontentlength: Option<String>,
     pub getcontenttype: Option<String>,
     pub resourcetype: ResourceTypeContainer,
 }
 
-#[derive(Deserialize, Debug, PartialEq)]
+#[derive(Deserialize, Debug, PartialEq, Eq)]
 pub struct ResourceTypeContainer {
     #[serde(rename = "$value")]
     pub value: Option<ResourceType>,
 }
 
-#[derive(Deserialize, Debug, PartialEq)]
+#[derive(Deserialize, Debug, PartialEq, Eq)]
 #[serde(rename_all = "lowercase")]
 pub enum ResourceType {
     Collection,
 }
 
 #[cfg(test)]
 mod tests {
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 // specific language governing permissions and limitations
 // under the License.
 
 //! HTTP response messages
 
 use serde::Deserialize;
 
+use crate::raw::*;
 use crate::*;
 
 #[derive(Debug, Deserialize)]
 pub(super) struct BooleanResp {
     pub boolean: bool,
 }
 
@@ -58,20 +59,19 @@
 impl TryFrom<FileStatus> for Metadata {
     type Error = Error;
     fn try_from(value: FileStatus) -> Result<Self> {
         let mut meta = match value.ty {
             FileStatusType::Directory => Metadata::new(EntryMode::DIR),
             FileStatusType::File => Metadata::new(EntryMode::FILE),
         };
-        let till_now = time::Duration::milliseconds(value.modification_time);
-        let last_modified = time::OffsetDateTime::UNIX_EPOCH
-            .checked_add(till_now)
-            .ok_or_else(|| Error::new(ErrorKind::Unexpected, "last modification overflowed!"))?;
-        meta.set_last_modified(last_modified)
-            .set_content_length(value.length);
+
+        meta.set_last_modified(parse_datetime_from_from_timestamp_millis(
+            value.modification_time,
+        )?)
+        .set_content_length(value.length);
         Ok(meta)
     }
 }
 
 #[derive(Debug, Deserialize, PartialEq, Eq)]
 #[serde(rename_all = "UPPERCASE")]
 pub enum FileStatusType {
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::WebhdfsBuilder as Webhdfs;
+pub use backend::GcsBuilder as Gcs;
 
+mod core;
 mod error;
-mod message;
 mod pager;
+mod uri;
 mod writer;
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/services/webhdfs/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/services/gcs/writer.rs`

 * *Files 19% similar despite different names*

```diff
@@ -11,53 +11,55 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::WebhdfsBackend;
+use super::core::GcsCore;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct WebhdfsWriter {
-    backend: WebhdfsBackend,
+pub struct GcsWriter {
+    core: Arc<GcsCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl WebhdfsWriter {
-    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
-        WebhdfsWriter { backend, op, path }
+impl GcsWriter {
+    pub fn new(core: Arc<GcsCore>, op: OpWrite, path: String) -> Self {
+        GcsWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for WebhdfsWriter {
+impl oio::Write for GcsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let req = self
-            .backend
-            .webhdfs_create_object_req(
-                &self.path,
-                Some(bs.len()),
-                self.op.content_type(),
-                AsyncBody::Bytes(bs),
-            )
-            .await?;
+        let mut req = self.core.gcs_insert_object_request(
+            &percent_encode_path(&self.path),
+            Some(bs.len()),
+            self.op.content_type(),
+            AsyncBody::Bytes(bs),
+        )?;
+
+        self.core.sign(&mut req).await?;
 
-        let resp = self.backend.client.send_async(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
+
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/error.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/error.rs`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,16 @@
     IsADirectory,
     /// The given path is not a directory.
     NotADirectory,
     /// The given path already exists thus we failed to the specified operation on it.
     AlreadyExists,
     /// Requests that sent to this path is over the limit, please slow down.
     RateLimited,
+    /// The given file paths are same.
+    IsSameFile,
 }
 
 impl ErrorKind {
     /// Convert self into static str.
     pub fn into_static(self) -> &'static str {
         self.into()
     }
@@ -91,14 +93,15 @@
             ErrorKind::ConfigInvalid => "ConfigInvalid",
             ErrorKind::NotFound => "NotFound",
             ErrorKind::PermissionDenied => "PermissionDenied",
             ErrorKind::IsADirectory => "IsADirectory",
             ErrorKind::NotADirectory => "NotADirectory",
             ErrorKind::AlreadyExists => "AlreadyExists",
             ErrorKind::RateLimited => "RateLimited",
+            ErrorKind::IsSameFile => "IsSameFile",
         }
     }
 }
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq)]
 enum ErrorStatus {
     /// Permanent means without external changes, the error never changes.
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/list.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/metadata.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use chrono::prelude::*;
 use flagset::flags;
 use flagset::FlagSet;
-use time::OffsetDateTime;
 
 use crate::raw::*;
 use crate::*;
 
 /// Metadata carries all metadata associated with an path.
 ///
 /// # Notes
@@ -38,15 +38,15 @@
 
     content_disposition: Option<String>,
     content_length: Option<u64>,
     content_md5: Option<String>,
     content_range: Option<BytesContentRange>,
     content_type: Option<String>,
     etag: Option<String>,
-    last_modified: Option<OffsetDateTime>,
+    last_modified: Option<DateTime<Utc>>,
 }
 
 impl Metadata {
     /// Create a new metadata
     pub fn new(mode: EntryMode) -> Self {
         // Mode is required to be set for metadata.
         let mut bit = Metakey::Mode.into();
@@ -242,39 +242,39 @@
     }
 
     /// Last modified of this entry.
     ///
     /// `Last-Modified` is defined by [RFC 7232](https://httpwg.org/specs/rfc7232.html#header.last-modified)
     /// Refer to [MDN Last-Modified](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Last-Modified) for more information.
     ///
-    /// OpenDAL parse the raw value into [`OffsetDateTime`] for convenient.
-    pub fn last_modified(&self) -> Option<OffsetDateTime> {
+    /// OpenDAL parse the raw value into [`DateTime`] for convenient.
+    pub fn last_modified(&self) -> Option<DateTime<Utc>> {
         debug_assert!(
             self.bit.contains(Metakey::LastModified) || self.bit.contains(Metakey::Complete),
             "visiting not set metadata: last_modified, maybe a bug"
         );
 
         self.last_modified
     }
 
     /// Set Last modified of this entry.
     ///
     /// `Last-Modified` is defined by [RFC 7232](https://httpwg.org/specs/rfc7232.html#header.last-modified)
     /// Refer to [MDN Last-Modified](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Last-Modified) for more information.
-    pub fn set_last_modified(&mut self, last_modified: OffsetDateTime) -> &mut Self {
+    pub fn set_last_modified(&mut self, last_modified: DateTime<Utc>) -> &mut Self {
         self.last_modified = Some(last_modified);
         self.bit |= Metakey::LastModified;
         self
     }
 
     /// Set Last modified of this entry.
     ///
     /// `Last-Modified` is defined by [RFC 7232](https://httpwg.org/specs/rfc7232.html#header.last-modified)
     /// Refer to [MDN Last-Modified](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Last-Modified) for more information.
-    pub fn with_last_modified(mut self, last_modified: OffsetDateTime) -> Self {
+    pub fn with_last_modified(mut self, last_modified: DateTime<Utc>) -> Self {
         self.last_modified = Some(last_modified);
         self.bit |= Metakey::LastModified;
         self
     }
 
     /// ETag of this entry.
     ///
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files 10% similar despite different names*

```diff
@@ -443,14 +443,129 @@
     /// # Ok(())
     /// # }
     /// ```
     pub fn write(&self, path: &str, bs: impl Into<Bytes>) -> Result<()> {
         self.write_with(path, OpWrite::new(), bs)
     }
 
+    /// Copy a file from `from` to `to`.
+    ///
+    /// # Notes
+    ///
+    /// - `from` and `to` must be a file.
+    /// - `to` will be overwritten if it exists.
+    /// - If `from` and `to` are the same, nothing will happen.
+    /// - `copy` is idempotent. For same `from` and `to` input, the result will be the same.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use std::io::Result;
+    /// # use opendal::BlockingOperator;
+    ///
+    /// # fn test(op: BlockingOperator) -> Result<()> {
+    /// op.copy("path/to/file", "path/to/file2")?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub fn copy(&self, from: &str, to: &str) -> Result<()> {
+        let from = normalize_path(from);
+
+        if !validate_path(&from, EntryMode::FILE) {
+            return Err(
+                Error::new(ErrorKind::IsADirectory, "from path is a directory")
+                    .with_operation("BlockingOperator::copy")
+                    .with_context("service", self.info().scheme())
+                    .with_context("from", from),
+            );
+        }
+
+        let to = normalize_path(to);
+
+        if !validate_path(&to, EntryMode::FILE) {
+            return Err(
+                Error::new(ErrorKind::IsADirectory, "to path is a directory")
+                    .with_operation("BlockingOperator::copy")
+                    .with_context("service", self.info().scheme())
+                    .with_context("to", to),
+            );
+        }
+
+        if from == to {
+            return Err(
+                Error::new(ErrorKind::IsSameFile, "from and to paths are same")
+                    .with_operation("BlockingOperator::copy")
+                    .with_context("service", self.info().scheme())
+                    .with_context("from", from)
+                    .with_context("to", to),
+            );
+        }
+
+        self.inner().blocking_copy(&from, &to, OpCopy::new())?;
+
+        Ok(())
+    }
+
+    /// Rename a file from `from` to `to`.
+    ///
+    /// # Notes
+    ///
+    /// - `from` and `to` must be a file.
+    /// - `to` will be overwritten if it exists.
+    /// - If `from` and `to` are the same, a `IsSameFile` error will occur.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use std::io::Result;
+    /// # use opendal::BlockingOperator;
+    ///
+    /// # fn test(op: BlockingOperator) -> Result<()> {
+    /// op.rename("path/to/file", "path/to/file2")?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub fn rename(&self, from: &str, to: &str) -> Result<()> {
+        let from = normalize_path(from);
+
+        if !validate_path(&from, EntryMode::FILE) {
+            return Err(
+                Error::new(ErrorKind::IsADirectory, "from path is a directory")
+                    .with_operation("BlockingOperator::move")
+                    .with_context("service", self.info().scheme())
+                    .with_context("from", from),
+            );
+        }
+
+        let to = normalize_path(to);
+
+        if !validate_path(&to, EntryMode::FILE) {
+            return Err(
+                Error::new(ErrorKind::IsADirectory, "to path is a directory")
+                    .with_operation("BlockingOperator::move")
+                    .with_context("service", self.info().scheme())
+                    .with_context("to", to),
+            );
+        }
+
+        if from == to {
+            return Err(
+                Error::new(ErrorKind::IsSameFile, "from and to paths are same")
+                    .with_operation("BlockingOperator::move")
+                    .with_context("service", self.info().scheme())
+                    .with_context("from", from)
+                    .with_context("to", to),
+            );
+        }
+
+        self.inner().blocking_rename(&from, &to, OpRename::new())?;
+
+        Ok(())
+    }
+
     /// Write data with option described in OpenDAL [rfc-0661](../../docs/rfcs/0661-path-in-accessor.md)
     ///
     /// # Notes
     ///
     /// - Write will make sure all bytes has been written, or an error will be returned.
     ///
     /// # Examples
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/operator/builder.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/operator/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files 11% similar despite different names*

```diff
@@ -53,14 +53,24 @@
     }
 
     /// Check if current backend supports [`Accessor::write`] or not.
     pub fn can_write(&self) -> bool {
         self.0.capabilities().contains(AccessorCapability::Write)
     }
 
+    /// Check if current backend supports [`Accessor::copy`] or not.
+    pub fn can_copy(&self) -> bool {
+        self.0.capabilities().contains(AccessorCapability::Copy)
+    }
+
+    /// Check if current backend supports [`Accessor::rename`] or not.
+    pub fn can_rename(&self) -> bool {
+        self.0.capabilities().contains(AccessorCapability::Rename)
+    }
+
     /// Check if current backend supports [`Accessor::list`] or not.
     pub fn can_list(&self) -> bool {
         self.0.capabilities().contains(AccessorCapability::List)
     }
 
     /// Check if current backend supports [`Accessor::scan`] or not.
     pub fn can_scan(&self) -> bool {
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files 9% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::ops::RangeBounds;
+use std::time::Duration;
 
 use bytes::Bytes;
 use flagset::FlagSet;
 use futures::stream;
 use futures::AsyncReadExt;
 use futures::Stream;
 use futures::StreamExt;
 use futures::TryStreamExt;
-use time::Duration;
 use tokio::io::ReadBuf;
 
 use super::BlockingOperator;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
@@ -496,15 +496,17 @@
     /// # use std::io::Result;
     /// # use opendal::Operator;
     /// # use futures::TryStreamExt;
     /// # use opendal::Scheme;
     /// # use opendal::ops::OpRead;
     /// # #[tokio::main]
     /// # async fn test(op: Operator) -> Result<()> {
-    /// let r = op.reader_with("path/to/file", OpRead::default().with_range((0..10).into())).await?;
+    /// let r = op
+    ///     .reader_with("path/to/file", OpRead::default().with_range((0..10).into()))
+    ///     .await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn reader_with(&self, path: &str, args: OpRead) -> Result<Reader> {
         let path = normalize_path(path);
 
         if !validate_path(&path, EntryMode::FILE) {
@@ -540,14 +542,131 @@
     /// # Ok(())
     /// # }
     /// ```
     pub async fn write(&self, path: &str, bs: impl Into<Bytes>) -> Result<()> {
         self.write_with(path, OpWrite::new(), bs).await
     }
 
+    /// Copy a file from `from` to `to`.
+    ///
+    /// # Notes
+    ///
+    /// - `from` and `to` must be a file.
+    /// - `to` will be overwritten if it exists.
+    /// - If `from` and `to` are the same,  a `IsSameFile` error will occur.
+    /// - `copy` is idempotent. For same `from` and `to` input, the result will be the same.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use std::io::Result;
+    /// # use opendal::Operator;
+    ///
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// op.copy("path/to/file", "path/to/file2").await?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub async fn copy(&self, from: &str, to: &str) -> Result<()> {
+        let from = normalize_path(from);
+
+        if !validate_path(&from, EntryMode::FILE) {
+            return Err(
+                Error::new(ErrorKind::IsADirectory, "from path is a directory")
+                    .with_operation("Operator::copy")
+                    .with_context("service", self.info().scheme())
+                    .with_context("from", from),
+            );
+        }
+
+        let to = normalize_path(to);
+
+        if !validate_path(&to, EntryMode::FILE) {
+            return Err(
+                Error::new(ErrorKind::IsADirectory, "to path is a directory")
+                    .with_operation("Operator::copy")
+                    .with_context("service", self.info().scheme())
+                    .with_context("to", to),
+            );
+        }
+
+        if from == to {
+            return Err(
+                Error::new(ErrorKind::IsSameFile, "from and to paths are same")
+                    .with_operation("Operator::copy")
+                    .with_context("service", self.info().scheme())
+                    .with_context("from", from)
+                    .with_context("to", to),
+            );
+        }
+
+        self.inner().copy(&from, &to, OpCopy::new()).await?;
+
+        Ok(())
+    }
+
+    /// Rename a file from `from` to `to`.
+    ///
+    /// # Notes
+    ///
+    /// - `from` and `to` must be a file.
+    /// - `to` will be overwritten if it exists.
+    /// - If `from` and `to` are the same, a `IsSameFile` error will occur.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use std::io::Result;
+    /// # use opendal::Operator;
+    ///
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// op.rename("path/to/file", "path/to/file2").await?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub async fn rename(&self, from: &str, to: &str) -> Result<()> {
+        let from = normalize_path(from);
+
+        if !validate_path(&from, EntryMode::FILE) {
+            return Err(
+                Error::new(ErrorKind::IsADirectory, "from path is a directory")
+                    .with_operation("Operator::move_")
+                    .with_context("service", self.info().scheme())
+                    .with_context("from", from),
+            );
+        }
+
+        let to = normalize_path(to);
+
+        if !validate_path(&to, EntryMode::FILE) {
+            return Err(
+                Error::new(ErrorKind::IsADirectory, "to path is a directory")
+                    .with_operation("Operator::move_")
+                    .with_context("service", self.info().scheme())
+                    .with_context("to", to),
+            );
+        }
+
+        if from == to {
+            return Err(
+                Error::new(ErrorKind::IsSameFile, "from and to paths are same")
+                    .with_operation("Operator::move_")
+                    .with_context("service", self.info().scheme())
+                    .with_context("from", from)
+                    .with_context("to", to),
+            );
+        }
+
+        self.inner().rename(&from, &to, OpRename::new()).await?;
+
+        Ok(())
+    }
+
     /// Write multiple bytes into path.
     ///
     /// # Notes
     ///
     /// - Write will make sure all bytes has been written, or an error will be returned.
     ///
     /// # Examples
@@ -728,23 +847,24 @@
     /// let stream = stream::iter(vec!["abc".to_string(), "def".to_string()]);
     /// op.remove_via(stream).await?;
     /// # Ok(())
     /// # }
     /// ```
     pub async fn remove_via(&self, input: impl Stream<Item = String> + Unpin) -> Result<()> {
         if self.info().can_batch() {
-            let mut input = input.map(|v| (v, OpDelete::default())).chunks(self.limit());
+            let mut input = input
+                .map(|v| (v, OpDelete::default().into()))
+                .chunks(self.limit());
 
             while let Some(batches) = input.next().await {
                 let results = self
                     .inner()
-                    .batch(OpBatch::new(BatchOperations::Delete(batches)))
-                    .await?;
-
-                let BatchedResults::Delete(results) = results.into_results();
+                    .batch(OpBatch::new(batches))
+                    .await?
+                    .into_results();
 
                 // TODO: return error here directly seems not a good idea?
                 for (_, result) in results {
                     let _ = result?;
                 }
             }
         } else {
@@ -801,23 +921,22 @@
         if self.info().can_batch() {
             let mut obs = obs.try_chunks(self.limit());
 
             while let Some(batches) = obs.next().await {
                 let batches = batches
                     .map_err(|err| err.1)?
                     .into_iter()
-                    .map(|v| (v.path().to_string(), OpDelete::default()))
+                    .map(|v| (v.path().to_string(), OpDelete::default().into()))
                     .collect();
 
                 let results = self
                     .inner()
-                    .batch(OpBatch::new(BatchOperations::Delete(batches)))
-                    .await?;
-
-                let BatchedResults::Delete(results) = results.into_results();
+                    .batch(OpBatch::new(batches))
+                    .await?
+                    .into_results();
 
                 // TODO: return error here directly seems not a good idea?
                 for (_, result) in results {
                     let _ = result?;
                 }
             }
         } else {
@@ -938,168 +1057,168 @@
     ///
     /// # Example
     ///
     /// ```no_run
     /// use anyhow::Result;
     /// use futures::io;
     /// use opendal::Operator;
-    /// use time::Duration;
+    /// use std::time::Duration;
     ///
     /// #[tokio::main]
     /// async fn test(op: Operator) -> Result<()> {
-    ///     let signed_req = op.presign_stat("test",Duration::hours(1))?;
+    ///     let signed_req = op.presign_stat("test",Duration::from_secs(3600)).await?;
     ///     let req = http::Request::builder()
     ///         .method(signed_req.method())
     ///         .uri(signed_req.uri())
     ///         .body(())?;
     ///
     /// #    Ok(())
     /// # }
     /// ```
-    pub fn presign_stat(&self, path: &str, expire: Duration) -> Result<PresignedRequest> {
+    pub async fn presign_stat(&self, path: &str, expire: Duration) -> Result<PresignedRequest> {
         let path = normalize_path(path);
 
         let op = OpPresign::new(OpStat::new(), expire);
 
-        let rp = self.inner().presign(&path, op)?;
+        let rp = self.inner().presign(&path, op).await?;
         Ok(rp.into_presigned_request())
     }
 
     /// Presign an operation for read.
     ///
     /// # Example
     ///
     /// ```no_run
     /// use anyhow::Result;
     /// use futures::io;
     /// use opendal::Operator;
-    /// use time::Duration;
+    /// use std::time::Duration;
     ///
     /// #[tokio::main]
     /// async fn test(op: Operator) -> Result<()> {
-    ///     let signed_req = op.presign_read("test.txt", Duration::hours(1))?;
+    ///     let signed_req = op.presign_read("test.txt", Duration::from_secs(3600)).await?;
     /// #    Ok(())
     /// # }
     /// ```
     ///
     /// - `signed_req.method()`: `GET`
     /// - `signed_req.uri()`: `https://s3.amazonaws.com/examplebucket/test.txt?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=access_key_id/20130721/us-east-1/s3/aws4_request&X-Amz-Date=20130721T201207Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=<signature-value>`
     /// - `signed_req.headers()`: `{ "host": "s3.amazonaws.com" }`
     ///
     /// We can download this file via `curl` or other tools without credentials:
     ///
     /// ```shell
     /// curl "https://s3.amazonaws.com/examplebucket/test.txt?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=access_key_id/20130721/us-east-1/s3/aws4_request&X-Amz-Date=20130721T201207Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=<signature-value>" -O /tmp/test.txt
     /// ```
-    pub fn presign_read(&self, path: &str, expire: Duration) -> Result<PresignedRequest> {
+    pub async fn presign_read(&self, path: &str, expire: Duration) -> Result<PresignedRequest> {
         let path = normalize_path(path);
 
         let op = OpPresign::new(OpRead::new(), expire);
 
-        let rp = self.inner().presign(&path, op)?;
+        let rp = self.inner().presign(&path, op).await?;
         Ok(rp.into_presigned_request())
     }
 
     /// Presign an operation for read option described in OpenDAL [rfc-1735](../../docs/rfcs/1735_operation_extension.md).
     ///
     /// You can pass `OpRead` to this method to specify the content disposition.
     ///
     /// # Example
     ///
     /// ```no_run
     /// use anyhow::Result;
     /// use futures::io;
     /// use opendal::Operator;
-    /// use time::Duration;
+    /// use std::time::Duration;
     /// use opendal::ops::OpRead;
     ///
     /// #[tokio::main]
     /// async fn test(op: Operator) -> Result<()> {
     ///     let args = OpRead::new()
     ///         .with_override_content_disposition("attachment; filename=\"othertext.txt\"");
-    ///     let signed_req = op.presign_read_with("test.txt", args, Duration::hours(1))?;
+    ///     let signed_req = op.presign_read_with("test.txt", args, Duration::from_secs(3600)).await?;
     /// #    Ok(())
     /// # }
     /// ```
-    pub fn presign_read_with(
+    pub async fn presign_read_with(
         &self,
         path: &str,
         op: OpRead,
         expire: Duration,
     ) -> Result<PresignedRequest> {
         let path = normalize_path(path);
 
         let op = OpPresign::new(op, expire);
 
-        let rp = self.inner().presign(&path, op)?;
+        let rp = self.inner().presign(&path, op).await?;
         Ok(rp.into_presigned_request())
     }
 
     /// Presign an operation for write.
     ///
     /// # Example
     ///
     /// ```no_run
     /// use anyhow::Result;
     /// use futures::io;
     /// use opendal::Operator;
-    /// use time::Duration;
+    /// use std::time::Duration;
     ///
     /// #[tokio::main]
     /// async fn test(op: Operator) -> Result<()> {
-    ///     let signed_req = op.presign_write("test.txt", Duration::hours(1))?;
+    ///     let signed_req = op.presign_write("test.txt", Duration::from_secs(3600)).await?;
     /// #    Ok(())
     /// # }
     /// ```
     ///
     /// - `signed_req.method()`: `PUT`
     /// - `signed_req.uri()`: `https://s3.amazonaws.com/examplebucket/test.txt?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=access_key_id/20130721/us-east-1/s3/aws4_request&X-Amz-Date=20130721T201207Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=<signature-value>`
     /// - `signed_req.headers()`: `{ "host": "s3.amazonaws.com" }`
     ///
     /// We can upload file as this file via `curl` or other tools without credential:
     ///
     /// ```shell
     /// curl -X PUT "https://s3.amazonaws.com/examplebucket/test.txt?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=access_key_id/20130721/us-east-1/s3/aws4_request&X-Amz-Date=20130721T201207Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=<signature-value>" -d "Hello, World!"
     /// ```
-    pub fn presign_write(&self, path: &str, expire: Duration) -> Result<PresignedRequest> {
-        self.presign_write_with(path, OpWrite::new(), expire)
+    pub async fn presign_write(&self, path: &str, expire: Duration) -> Result<PresignedRequest> {
+        self.presign_write_with(path, OpWrite::new(), expire).await
     }
 
     /// Presign an operation for write with option described in OpenDAL [rfc-0661](../../docs/rfcs/0661-path-in-accessor.md)
     ///
     /// You can pass `OpWrite` to this method to specify the content length and content type.
     ///
     /// # Example
     ///
     /// ```no_run
     /// use anyhow::Result;
     /// use futures::io;
     /// use opendal::ops::OpWrite;
     /// use opendal::Operator;
-    /// use time::Duration;
+    /// use std::time::Duration;
     ///
     /// #[tokio::main]
     /// async fn test(op: Operator) -> Result<()> {
     ///     let args = OpWrite::new().with_content_type("text/csv");
-    ///     let signed_req = op.presign_write_with("test", args, Duration::hours(1))?;
+    ///     let signed_req = op.presign_write_with("test", args, Duration::from_secs(3600)).await?;
     ///     let req = http::Request::builder()
     ///         .method(signed_req.method())
     ///         .uri(signed_req.uri())
     ///         .body(())?;
     ///
     /// #    Ok(())
     /// # }
     /// ```
-    pub fn presign_write_with(
+    pub async fn presign_write_with(
         &self,
         path: &str,
         op: OpWrite,
         expire: Duration,
     ) -> Result<PresignedRequest> {
         let path = normalize_path(path);
 
         let op = OpPresign::new(op, expire);
 
-        let rp = self.inner().presign(&path, op)?;
+        let rp = self.inner().presign(&path, op).await?;
         Ok(rp.into_presigned_request())
     }
 }
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/ops.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/ops.rs`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 // specific language governing permissions and limitations
 // under the License.
 
 //! Ops provides the operation args struct like [`OpRead`] for user.
 //!
 //! By using ops, users can add more context for operation.
 
-use time::Duration;
+use std::time::Duration;
 
 use crate::raw::*;
 use crate::*;
 
 /// Args for `create` operation.
 ///
 /// The path must be normalized.
@@ -168,74 +168,65 @@
         Self::Write(v)
     }
 }
 
 /// Args for `batch` operation.
 #[derive(Debug, Clone)]
 pub struct OpBatch {
-    ops: BatchOperations,
+    ops: Vec<(String, BatchOperation)>,
 }
 
 impl OpBatch {
     /// Create a new batch options.
-    pub fn new(ops: BatchOperations) -> Self {
+    pub fn new(ops: Vec<(String, BatchOperation)>) -> Self {
         Self { ops }
     }
 
     /// Get operation from op.
-    pub fn operation(&self) -> &BatchOperations {
+    pub fn operation(&self) -> &[(String, BatchOperation)] {
         &self.ops
     }
 
     /// Consume OpBatch into BatchOperation
-    pub fn into_operation(self) -> BatchOperations {
+    pub fn into_operation(self) -> Vec<(String, BatchOperation)> {
         self.ops
     }
 }
 
 /// Batch operation used for batch.
 #[derive(Debug, Clone)]
 #[non_exhaustive]
-pub enum BatchOperations {
-    /// Batch delete operations.
-    Delete(Vec<(String, OpDelete)>),
+pub enum BatchOperation {
+    /// Batch delete operation.
+    Delete(OpDelete),
 }
 
-impl BatchOperations {
+impl From<OpDelete> for BatchOperation {
+    fn from(op: OpDelete) -> Self {
+        Self::Delete(op)
+    }
+}
+
+impl BatchOperation {
     /// Return the operation of this batch.
     pub fn operation(&self) -> Operation {
-        use BatchOperations::*;
+        use BatchOperation::*;
         match self {
             Delete(_) => Operation::Delete,
         }
     }
-
-    /// Return the length of given operations.
-    pub fn len(&self) -> usize {
-        use BatchOperations::*;
-        match self {
-            Delete(v) => v.len(),
-        }
-    }
-
-    /// Return if given operations is empty.
-    pub fn is_empty(&self) -> bool {
-        use BatchOperations::*;
-        match self {
-            Delete(v) => v.is_empty(),
-        }
-    }
 }
 
 /// Args for `read` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpRead {
     br: BytesRange,
     override_content_disposition: Option<String>,
     override_cache_control: Option<String>,
+    if_none_match: Option<String>,
 }
 
 impl OpRead {
     /// Create a default `OpRead` which will read whole content of path.
     pub fn new() -> Self {
         Self::default()
     }
@@ -269,24 +260,48 @@
         self
     }
 
     /// Returns the cache-control header that should be send back by the remote read operation.
     pub fn override_cache_control(&self) -> Option<&str> {
         self.override_cache_control.as_deref()
     }
+
+    /// Set the If-None-Match of the option
+    pub fn with_if_none_match(mut self, if_none_match: &str) -> Self {
+        self.if_none_match = Some(if_none_match.to_string());
+        self
+    }
+
+    /// Get If-None-Match from option
+    pub fn if_none_match(&self) -> Option<&str> {
+        self.if_none_match.as_deref()
+    }
 }
 
 /// Args for `stat` operation.
 #[derive(Debug, Clone, Default)]
-pub struct OpStat {}
+pub struct OpStat {
+    if_none_match: Option<String>,
+}
 
 impl OpStat {
     /// Create a new `OpStat`.
     pub fn new() -> Self {
-        Self {}
+        Self::default()
+    }
+
+    /// Set the If-None-Match of the option
+    pub fn with_if_none_match(mut self, if_none_match: &str) -> Self {
+        self.if_none_match = Some(if_none_match.to_string());
+        self
+    }
+
+    /// Get If-None-Match from option
+    pub fn if_none_match(&self) -> Option<&str> {
+        self.if_none_match.as_deref()
     }
 }
 
 /// Args for `write` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpWrite {
     append: bool,
@@ -297,21 +312,15 @@
 }
 
 impl OpWrite {
     /// Create a new `OpWrite`.
     ///
     /// If input path is not a file path, an error will be returned.
     pub fn new() -> Self {
-        Self {
-            append: false,
-
-            content_type: None,
-            content_disposition: None,
-            cache_control: None,
-        }
+        Self::default()
     }
 
     pub(crate) fn with_append(mut self) -> Self {
         self.append = true;
         self
     }
 
@@ -348,7 +357,29 @@
 
     /// Set the content type of option
     pub fn with_cache_control(mut self, cache_control: &str) -> Self {
         self.cache_control = Some(cache_control.to_string());
         self
     }
 }
+
+/// Args for `copy` operation.
+#[derive(Debug, Clone, Default)]
+pub struct OpCopy {}
+
+impl OpCopy {
+    /// Create a new `OpCopy`.
+    pub fn new() -> Self {
+        Self::default()
+    }
+}
+
+/// Args for `rename` operation.
+#[derive(Debug, Clone, Default)]
+pub struct OpRename {}
+
+impl OpRename {
+    /// Create a new `OpMove`.
+    pub fn new() -> Self {
+        Self::default()
+    }
+}
```

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/reader.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.31.0/local_dependencies/opendal/src/types/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/Cargo.toml` & `opendal-0.31.0/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,29 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [package]
-authors = ["OpenDAL Contributors <dev@opendal.apache.org>"]
-edition = "2021"
-homepage = "https://opendal.apache.org/"
-license = "Apache-2.0"
 name = "opendal-python"
 publish = false
-repository = "https://github.com/apache/incubator-opendal"
-version = "0.30.5"
+
+authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
+edition= "2021"
+homepage= "https://opendal.apache.org/"
+license= "Apache-2.0"
+repository= "https://github.com/apache/incubator-opendal"
+rust-version= "1.64"
+version= "0.31.0"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 chrono = { version = "0.4.24", default-features = false, features = ["std"] }
 futures = "0.3.27"
-opendal = { version = "0.30", path = "local_dependencies/opendal" }
+opendal.path = "local_dependencies/opendal"
 pyo3 = { version = "0.18", features = ["chrono"] }
 pyo3-asyncio = { version = "0.18", features = ["tokio-runtime"] }
 tokio = "1"
```

### Comparing `opendal-0.30.5/.gitignore` & `opendal-0.31.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/README.md` & `opendal-0.31.0/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/pyproject.toml` & `opendal-0.31.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -28,19 +28,27 @@
 description = "OpenDAL Python Binding"
 license = { text = "Apache-2.0" }
 name = "opendal"
 readme = "README.md"
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
-test = ["behave"]
+benchmark = [
+  "gevent",
+  "greenify",
+  "greenlet",
+  "boto3",
+  "pydantic",
+  "boto3-stubs[essential]",
+]
 docs = ["pdoc"]
+test = ["behave"]
 
 [project.urls]
 Documentation = "https://docs.rs/opendal/"
 Homepage = "https://opendal.apache.org/"
 Repository = "https://github.com/apache/incubator-opendal"
 
 [tool.maturin]
-module-name = "opendal._opendal"
 features = ["pyo3/extension-module"]
+module-name = "opendal._opendal"
 python-source = "python"
```

### Comparing `opendal-0.30.5/python/opendal/__init__.py` & `opendal-0.31.0/python/opendal/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,7 @@
 # under the License.
 
 from ._opendal import *
 
 
 __doc__ = _opendal.__doc__
 __all__ = _opendal.__all__
-
```

### Comparing `opendal-0.30.5/python/opendal/__init__.pyi` & `opendal-0.31.0/python/opendal/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
-
 from typing import AsyncIterable, Iterable, Optional
 
 class Error(Exception): ...
 
 class Operator:
     def __init__(self, scheme: str, **kwargs): ...
     def read(self, path: str) -> bytes: ...
```

### Comparing `opendal-0.30.5/src/asyncio.rs` & `opendal-0.31.0/src/asyncio.rs`

 * *Files 0% similar despite different names*

```diff
@@ -81,16 +81,17 @@
         Ok(AsyncReader::new(ReaderState::Init {
             operator: self.0.clone(),
             path,
         }))
     }
 
     /// Write bytes into given path.
-    pub fn write<'p>(&'p self, py: Python<'p>, path: String, bs: Vec<u8>) -> PyResult<&'p PyAny> {
+    pub fn write<'p>(&'p self, py: Python<'p>, path: String, bs: &PyBytes) -> PyResult<&'p PyAny> {
         let this = self.0.clone();
+        let bs = bs.as_bytes().to_vec();
         future_into_py(py, async move {
             this.write(&path, bs).await.map_err(format_pyerr)
         })
     }
 
     /// Get current path's metadata **without cache** directly.
     pub fn stat<'p>(&'p self, py: Python<'p>, path: String) -> PyResult<&'p PyAny> {
```

### Comparing `opendal-0.30.5/src/layers.rs` & `opendal-0.31.0/src/layers.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/src/lib.rs` & `opendal-0.31.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/tests/binding.feature` & `opendal-0.31.0/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.30.5/tests/steps/binding.py` & `opendal-0.31.0/tests/steps/binding.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,64 +15,76 @@
 # specific language governing permissions and limitations
 # under the License.
 
 from behave import given, when, then
 from behave.api.async_step import async_run_until_complete
 import opendal
 
-@given('A new OpenDAL Blocking Operator')
+
+@given("A new OpenDAL Blocking Operator")
 def step_impl(context):
     context.op = opendal.Operator("memory")
 
+
 @when('Blocking write path "{filename}" with content "{content}"')
 def step_impl(context, filename, content):
     context.op.write(filename, content.encode())
 
+
 @then('The blocking file "{filename}" should exist')
 def step_impl(context, filename):
     context.op.stat(filename)
 
+
 @then('The blocking file "{filename}" entry mode must be file')
 def step_impl(context, filename):
     assert context.op.stat(filename).mode.is_file()
 
+
 @then('The blocking file "{filename}" content length must be {size:d}')
 def step_impl(context, filename, size):
     assert context.op.stat(filename).content_length == size
 
+
 @then('The blocking file "{filename}" must have content "{content}"')
 def step_impl(context, filename, content):
     bs = context.op.read(filename)
     assert bs == content.encode()
 
-@given('A new OpenDAL Async Operator')
+
+@given("A new OpenDAL Async Operator")
 @async_run_until_complete
 async def step_impl(context):
     context.op = opendal.AsyncOperator("memory")
 
+
 @when('Async write path "{filename}" with content "{content}"')
 @async_run_until_complete
 async def step_impl(context, filename, content):
     await context.op.write(filename, content.encode())
 
+
 @then('The async file "{filename}" should exist')
 @async_run_until_complete
 async def step_impl(context, filename):
     await context.op.stat(filename)
 
+
 @then('The async file "{filename}" entry mode must be file')
 @async_run_until_complete
 async def step_impl(context, filename):
     meta = await context.op.stat(filename)
     assert meta.mode.is_file()
 
+
 @then('The async file "{filename}" content length must be {size:d}')
 @async_run_until_complete
 async def step_impl(context, filename, size):
     meta = await context.op.stat(filename)
     assert meta.content_length == size
 
+
 @then('The async file "{filename}" must have content "{content}"')
 @async_run_until_complete
 async def step_impl(context, filename, content):
     bs = await context.op.read(filename)
     assert bs == content.encode()
```

### Comparing `opendal-0.30.5/Cargo.lock` & `opendal-0.31.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -200,26 +200,26 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f23d769dbf1838d5df5156e7b1ad404f4c463d1ac2c6aeb6cd943630f8a8400"
 dependencies = [
  "futures-core",
  "futures-io",
  "rustls 0.19.1",
  "webpki 0.21.4",
- "webpki-roots 0.21.1",
+ "webpki-roots",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.67"
+version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86ea188f25f0255d8f92797797c97ebf5631fa88178beb1a46fdf5622c9a00e4"
+checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.4",
+ "syn 2.0.12",
 ]
 
 [[package]]
 name = "atomic-waker"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "debc29dde2e69f9e47506b525f639ed42300fc014a3e007832592448fa8e4599"
@@ -794,15 +794,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 2.0.4",
+ "syn 2.0.12",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.93"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "edc52e2eb08915cb12596d29d55f0b5384f00d697a646dbd269b6ecb0fbd9d31"
@@ -811,15 +811,15 @@
 name = "cxxbridge-macro"
 version = "1.0.93"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "631569015d0d8d54e6c241733f944042623ab6df7bc3be7466874b05fcdb1c5f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.4",
+ "syn 2.0.12",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
@@ -889,39 +889,19 @@
  "const-oid",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "dirs"
-version = "4.0.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
-dependencies = [
- "dirs-sys 0.3.7",
-]
-
-[[package]]
-name = "dirs"
 version = "5.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dece029acd3353e3a58ac2e3eb3c8d6c35827a892edc6cc4138ef9c33df46ecd"
 dependencies = [
- "dirs-sys 0.4.0",
-]
-
-[[package]]
-name = "dirs-sys"
-version = "0.3.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
-dependencies = [
- "libc",
- "redox_users",
- "winapi",
+ "dirs-sys",
 ]
 
 [[package]]
 name = "dirs-sys"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04414300db88f70d74c5ff54e50f9e1d1737d9a5b90f53fcf2e95ca2a9ab554b"
@@ -1996,36 +1976,37 @@
 name = "napi-build"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "882a73d9ef23e8dc2ebbffb6a6ae2ef467c0f18ac10711e4cc59c5485d41df0e"
 
 [[package]]
 name = "napi-derive"
-version = "2.12.1"
+version = "2.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8f63dc8e483a8ce6821932d6357ad95e79b33b0a352f482f9033c5eb2d49caf"
+checksum = "a6bd0beb0ac7e8576bc92d293361a461b42eaf41740bbdec7e0cbf64d8dc89f7"
 dependencies = [
  "convert_case",
  "napi-derive-backend",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "napi-derive-backend"
-version = "1.0.47"
+version = "1.0.48"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68f0ee68701b2bc3657cf2c4f01faaf3391cb1746db20e6887e8c816d271c7d9"
+checksum = "c713ff9ff5baa6d6ad9aedc46fad73c91e2f16ebe5ece0f41983d4e70e020c7c"
 dependencies = [
  "convert_case",
  "once_cell",
  "proc-macro2",
  "quote",
  "regex",
+ "semver",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "napi-sys"
 version = "2.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2165,33 +2146,32 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.30.5"
+version = "0.31.0"
 dependencies = [
  "async-trait",
  "bytes",
- "chrono",
  "futures",
  "object_store",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "oli"
-version = "0.30.5"
+version = "0.31.0"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "clap 4.1.11",
- "dirs 5.0.0",
+ "dirs",
  "env_logger",
  "futures",
  "log",
  "opendal",
  "predicates 2.1.5",
  "serde",
  "tokio",
@@ -2209,25 +2189,26 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.30.5"
+version = "0.31.0"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
  "base64 0.21.0",
  "bb8",
  "bytes",
  "cfg-if",
+ "chrono",
  "criterion",
  "dashmap",
  "dotenvy",
  "env_logger",
  "flagset",
  "futures",
  "hdrs",
@@ -2235,15 +2216,15 @@
  "hyper",
  "lazy-regex",
  "log",
  "md-5",
  "metrics",
  "moka",
  "once_cell",
- "opentelemetry",
+ "opentelemetry 0.19.0",
  "opentelemetry-jaeger",
  "parking_lot 0.12.1",
  "paste",
  "percent-encoding",
  "pin-project",
  "pretty_assertions",
  "prost",
@@ -2255,56 +2236,53 @@
  "rocksdb",
  "serde",
  "serde_json",
  "sha2",
  "size",
  "sled",
  "suppaftp",
- "time 0.3.17",
  "tokio",
  "tracing",
  "tracing-opentelemetry",
  "tracing-subscriber",
- "trust-dns-resolver",
- "ureq",
  "uuid",
  "wiremock",
 ]
 
 [[package]]
 name = "opendal-c"
 version = "0.1.0"
 dependencies = [
+ "bytes",
  "cbindgen",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-java"
 version = "0.1.0"
 dependencies = [
  "jni",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.30.5"
+version = "0.31.0"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
- "time 0.3.17",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.30.5"
+version = "0.31.0"
 dependencies = [
  "chrono",
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
@@ -2389,41 +2367,86 @@
  "percent-encoding",
  "pin-project",
  "rand 0.8.5",
  "thiserror",
 ]
 
 [[package]]
+name = "opentelemetry"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5f4b8347cc26099d3aeee044065ecc3ae11469796b4d65d065a23a584ed92a6f"
+dependencies = [
+ "opentelemetry_api",
+ "opentelemetry_sdk",
+]
+
+[[package]]
 name = "opentelemetry-jaeger"
-version = "0.16.0"
+version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8c0b12cd9e3f9b35b52f6e0dac66866c519b26f424f4bbf96e3fe8bfbdc5229"
+checksum = "08e028dc9f4f304e9320ce38c80e7cf74067415b1ad5a8750a38bae54a4d450d"
 dependencies = [
  "async-trait",
- "lazy_static",
- "opentelemetry",
+ "futures",
+ "futures-executor",
+ "once_cell",
+ "opentelemetry 0.19.0",
  "opentelemetry-semantic-conventions",
  "thiserror",
  "thrift",
 ]
 
 [[package]]
 name = "opentelemetry-semantic-conventions"
-version = "0.9.0"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24e33428e6bf08c6f7fcea4ddb8e358fab0fe48ab877a87c70c6ebe20f673ce5"
+dependencies = [
+ "opentelemetry 0.19.0",
+]
+
+[[package]]
+name = "opentelemetry_api"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "985cc35d832d412224b2cffe2f9194b1b89b6aa5d0bef76d080dce09d90e62bd"
+checksum = "ed41783a5bf567688eb38372f2b7a8530f5a607a4b49d38dd7573236c23ca7e2"
 dependencies = [
- "opentelemetry",
+ "futures-channel",
+ "futures-util",
+ "indexmap",
+ "once_cell",
+ "pin-project-lite",
+ "thiserror",
+ "urlencoding",
+]
+
+[[package]]
+name = "opentelemetry_sdk"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b3a2a91fdbfdd4d212c0dcc2ab540de2c2bcbbd90be17de7a7daf8822d010c1"
+dependencies = [
+ "async-trait",
+ "crossbeam-channel",
+ "futures-channel",
+ "futures-executor",
+ "futures-util",
+ "once_cell",
+ "opentelemetry_api",
+ "percent-encoding",
+ "rand 0.8.5",
+ "thiserror",
 ]
 
 [[package]]
 name = "ordered-float"
-version = "1.1.1"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3305af35278dd29f46fcdd139e0b1fbfae2153f0e5928b39b035542dd31e37b7"
+checksum = "7940cf2ca942593318d07fcf2596cdca60a85c9e7fab408a5e21a4f9dcd40d87"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "ordered-multimap"
 version = "0.4.3"
@@ -3081,41 +3104,42 @@
 name = "regex-syntax"
 version = "0.6.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
 
 [[package]]
 name = "reqsign"
-version = "0.8.5"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7db6d8d2cd7fa61403d14de670f98d7cedac38143681c124943d7bb69258b3a"
+checksum = "3875de6d7d0468315194cb8332913aae0d6803cfd5c7f089dc174ff5350f7b29"
 dependencies = [
  "anyhow",
- "backon",
+ "async-trait",
  "base64 0.21.0",
  "bytes",
- "dirs 4.0.0",
+ "chrono",
+ "dirs",
  "form_urlencoded",
  "hex",
  "hmac",
  "http",
  "jsonwebtoken",
  "log",
  "once_cell",
  "percent-encoding",
  "quick-xml 0.28.1",
  "rand 0.8.5",
+ "reqwest",
  "rsa",
  "rust-ini",
  "serde",
  "serde_json",
  "sha1",
  "sha2",
- "time 0.3.17",
- "ureq",
+ "tokio",
 ]
 
 [[package]]
 name = "reqwest"
 version = "0.11.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ba30cc2c0cd02af1222ed216ba659cdb2f879dfe3181852fe7c50b1d0005949"
@@ -3417,15 +3441,15 @@
 name = "serde_derive"
 version = "1.0.158"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e801c1712f48475582b7696ac71e0ca34ebb30e09338425384269d9717c62cad"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.4",
+ "syn 2.0.12",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
@@ -3531,15 +3555,15 @@
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adc4e5204eb1910f40f9cfa375f6f05b68c3abac4b6fd879c8ff5e7ae8a0a085"
 dependencies = [
  "num-bigint",
  "num-traits",
  "thiserror",
- "time 0.3.17",
+ "time 0.3.20",
 ]
 
 [[package]]
 name = "size"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fed904c7fb2856d868b92464fc8fa597fce366edea1a9cbfaa8cb5fe080bd6d"
@@ -3674,17 +3698,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.4"
+version = "2.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c622ae390c9302e214c31013517c2061ecb2699935882c60a9b37f82f8625ae"
+checksum = "79d9531f94112cfc3e4c8f5f02cb2b58f72c97b7efd85f70203cc6d8efda5927"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3746,15 +3770,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.4",
+ "syn 2.0.12",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
@@ -3770,17 +3794,17 @@
 checksum = "d050e60b33d41c19108b32cea32164033a9013fe3b46cbd4457559bfbf77afaa"
 dependencies = [
  "num_cpus",
 ]
 
 [[package]]
 name = "thrift"
-version = "0.15.0"
+version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b82ca8f46f95b3ce96081fe3dd89160fdea970c254bb72925255d1b62aae692e"
+checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
 dependencies = [
  "byteorder",
  "integer-encoding",
  "log",
  "ordered-float",
  "threadpool",
 ]
@@ -3794,17 +3818,17 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.17"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a561bf4617eebd33bca6434b988f39ed798e527f51a1e797d0ee4f61c0a38376"
+checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
 dependencies = [
  "itoa",
  "serde",
  "time-core",
  "time-macros",
 ]
 
@@ -3812,17 +3836,17 @@
 name = "time-core"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
 
 [[package]]
 name = "time-macros"
-version = "0.2.6"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d967f99f534ca7e495c575c62638eebc2898a8c84c119b89e250477bc4ba16b2"
+checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
@@ -3846,40 +3870,39 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.26.0"
+version = "1.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03201d01c3c27a29c8a5cee5b55a93ddae1ccf6f08f65365c2c918f8c1b76f64"
+checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
- "memchr",
  "mio",
  "num_cpus",
  "parking_lot 0.12.1",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "1.8.2"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d266c00fde287f55d3f1c3e96c500c362a2b8c695076ec180f27918820bc6df8"
+checksum = "61a573bdc87985e9d6ddeed1b3d864e8a302c847e40d647746df2f1de209d1ce"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.12",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -4009,15 +4032,15 @@
 [[package]]
 name = "tracing-opentelemetry"
 version = "0.17.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fbbe89715c1dbbb790059e2565353978564924ee85017b5fff365c872ff6721f"
 dependencies = [
  "once_cell",
- "opentelemetry",
+ "opentelemetry 0.17.0",
  "tracing",
  "tracing-core",
  "tracing-log",
  "tracing-subscriber",
 ]
 
 [[package]]
@@ -4152,43 +4175,32 @@
 [[package]]
 name = "untrusted"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
 
 [[package]]
-name = "ureq"
-version = "2.6.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "338b31dd1314f68f3aabf3ed57ab922df95ffcd902476ca7ba3c4ce7b908c46d"
-dependencies = [
- "base64 0.13.1",
- "log",
- "native-tls",
- "once_cell",
- "rustls 0.20.8",
- "rustls-native-certs",
- "url",
- "webpki 0.22.0",
- "webpki-roots 0.22.6",
-]
-
-[[package]]
 name = "url"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
 dependencies = [
  "form_urlencoded",
  "idna 0.3.0",
  "percent-encoding",
  "serde",
 ]
 
 [[package]]
+name = "urlencoding"
+version = "2.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e8db7427f936968176eaa7cdf81b7f98b980b18495ec28f1b5791ac3bfe3eea9"
+
+[[package]]
 name = "uuid"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
 dependencies = [
  "getrandom 0.2.8",
  "serde",
@@ -4390,23 +4402,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aabe153544e473b775453675851ecc86863d2a81d786d741f6b76778f2a48940"
 dependencies = [
  "webpki 0.21.4",
 ]
 
 [[package]]
-name = "webpki-roots"
-version = "0.22.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b6c71e40d7d2c34a5106301fb632274ca37242cd0c9d3e64dbece371a40a2d87"
-dependencies = [
- "webpki 0.22.0",
-]
-
-[[package]]
 name = "widestring"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17882f045410753661207383517a6f62ec3dbeb6a4ed2acce01f0728238d1983"
 
 [[package]]
 name = "winapi"
```

### Comparing `opendal-0.30.5/PKG-INFO` & `opendal-0.31.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.30.5
+Version: 0.31.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Dist: gevent; extra == 'benchmark'
+Requires-Dist: greenify; extra == 'benchmark'
+Requires-Dist: greenlet; extra == 'benchmark'
+Requires-Dist: boto3; extra == 'benchmark'
+Requires-Dist: pydantic; extra == 'benchmark'
+Requires-Dist: boto3-stubs[essential]; extra == 'benchmark'
 Requires-Dist: behave; extra == 'test'
 Requires-Dist: pdoc; extra == 'docs'
+Provides-Extra: benchmark
 Provides-Extra: test
 Provides-Extra: docs
 Summary: OpenDAL Python Binding
 Home-Page: https://opendal.apache.org/
 Author: OpenDAL Contributors <dev@opendal.apache.org>
 Author-email: OpenDAL Contributors <dev@opendal.apache.org>
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Repository, https://github.com/apache/incubator-opendal
-Project-URL: Homepage, https://opendal.apache.org/
 Project-URL: Documentation, https://docs.rs/opendal/
+Project-URL: Homepage, https://opendal.apache.org/
+Project-URL: Repository, https://github.com/apache/incubator-opendal
 
 # OpenDAL Python Binding
 
 This crate intends to build a native python binding.
 
 ## Installation
```

