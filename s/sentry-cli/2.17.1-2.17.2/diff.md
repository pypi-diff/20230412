# Comparing `tmp/sentry_cli-2.17.1.tar.gz` & `tmp/sentry_cli-2.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_cli-2.17.1.tar", last modified: Tue Apr 11 21:13:48 2023, max compression
+gzip compressed data, was "sentry_cli-2.17.2.tar", last modified: Wed Apr 12 12:00:19 2023, max compression
```

## Comparing `sentry_cli-2.17.1.tar` & `sentry_cli-2.17.2.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.690202 sentry_cli-2.17.1/
--rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-11 21:13:48.690202 sentry_cli-2.17.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/build.rs
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.678202 sentry_cli-2.17.1/sentry_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-11 21:13:48.000000 sentry_cli-2.17.1/sentry_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-11 21:13:48.000000 sentry_cli-2.17.1/sentry_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:13:48.000000 sentry_cli-2.17.1/sentry_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 21:13:48.000000 sentry_cli-2.17.1/sentry_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-11 21:13:48.690202 sentry_cli-2.17.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.678202 sentry_cli-2.17.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)    87341 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/api.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/bashsupport.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.682202 sentry_cli-2.17.1/src/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/bash_hook.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.682202 sentry_cli-2.17.1/src/commands/debug_files/
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/debug_files/bundle_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/debug_files/check.rs
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/debug_files/find.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/debug_files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/debug_files/print_sources.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/debug_files/upload.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.682202 sentry_cli-2.17.1/src/commands/deploys/
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/deploys/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/deploys/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/deploys/new.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.682202 sentry_cli-2.17.1/src/commands/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/events/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/events/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.682202 sentry_cli-2.17.1/src/commands/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/files/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/files/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/files/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/files/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/info.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.682202 sentry_cli-2.17.1/src/commands/issues/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/issues/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/issues/mute.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/issues/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/issues/unresolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/login.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.682202 sentry_cli-2.17.1/src/commands/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/monitors/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/monitors/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/monitors/run.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.682202 sentry_cli-2.17.1/src/commands/organizations/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/organizations/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/organizations/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.682202 sentry_cli-2.17.1/src/commands/projects/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/projects/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/projects/mod.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.682202 sentry_cli-2.17.1/src/commands/react_native/
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/react_native/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/react_native/gradle.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/react_native/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/react_native/xcode.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.686202 sentry_cli-2.17.1/src/commands/releases/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/releases/archive.rs
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/releases/delete.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/releases/finalize.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/releases/info.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/releases/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/releases/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/releases/new.rs
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/releases/propose_version.rs
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/releases/restore.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/releases/set_commits.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.686202 sentry_cli-2.17.1/src/commands/repos/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/repos/list.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/repos/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/send_envelope.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/send_event.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.686202 sentry_cli-2.17.1/src/commands/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/sourcemaps/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/sourcemaps/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/sourcemaps/resolve.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/sourcemaps/upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/uninstall.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/upload_dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/upload_dsym.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/commands/upload_proguard.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/config.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/constants.rs
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/main.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.690202 sentry_cli-2.17.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/android.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/appcenter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/args.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/chunks.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/codepush.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/cordova.rs
--rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/dif.rs
--rw-r--r--   0 runner    (1001) docker     (123)    72539 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/dif_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/enc.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/event.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/file_search.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/file_upload.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/formatting.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/fs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/http.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/logging.rs
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/progress.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/releases.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/retry.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.690202 sentry_cli-2.17.1/src/utils/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 21:13:48.690202 sentry_cli-2.17.1/src/utils/sourcemaps/
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/sourcemaps/inject.rs
--rw-r--r--   0 runner    (1001) docker     (123)    33830 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/sourcemaps.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/system.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/ui.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/update.rs
--rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/vcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-04-11 21:13:21.000000 sentry_cli-2.17.1/src/utils/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    80821 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.238543 sentry_cli-2.17.2/sentry_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-04-12 12:00:19.000000 sentry_cli-2.17.2/sentry_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-12 12:00:19.000000 sentry_cli-2.17.2/sentry_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:00:19.000000 sentry_cli-2.17.2/sentry_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:00:19.000000 sentry_cli-2.17.2/sentry_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.238543 sentry_cli-2.17.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    87341 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/api.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/bashsupport.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/bash_hook.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/debug_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/bundle_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/check.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/find.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/print_sources.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/debug_files/upload.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/deploys/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/deploys/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/deploys/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/deploys/new.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/events/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/events/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/files/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/files/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/files/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/files/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/info.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/issues/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/issues/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/issues/mute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/issues/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/issues/unresolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/login.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/monitors/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/monitors/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/monitors/run.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/organizations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/organizations/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/organizations/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.242544 sentry_cli-2.17.2/src/commands/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/projects/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/projects/mod.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.246544 sentry_cli-2.17.2/src/commands/react_native/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/react_native/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/react_native/gradle.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/react_native/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14288 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/react_native/xcode.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.246544 sentry_cli-2.17.2/src/commands/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/archive.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/delete.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/finalize.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/info.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/new.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/propose_version.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/restore.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/releases/set_commits.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.246544 sentry_cli-2.17.2/src/commands/repos/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/repos/list.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/repos/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/send_envelope.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/send_event.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.246544 sentry_cli-2.17.2/src/commands/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/sourcemaps/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/sourcemaps/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/sourcemaps/resolve.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14882 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/sourcemaps/upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/uninstall.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/upload_dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/upload_dsym.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/commands/upload_proguard.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    20882 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/config.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/constants.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/main.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/android.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/appcenter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/args.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/chunks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/codepush.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/cordova.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    14479 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/dif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    72539 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/dif_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/enc.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/event.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/file_search.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16662 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/file_upload.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/formatting.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/fs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/http.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/logging.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/progress.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/releases.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/retry.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/src/utils/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_previous_commit.snap
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:00:19.250543 sentry_cli-2.17.2/src/utils/sourcemaps/
+-rw-r--r--   0 runner    (1001) docker     (123)    11403 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/sourcemaps/inject.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36190 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/sourcemaps.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/system.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/ui.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36048 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/vcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    19150 2023-04-12 12:00:03.000000 sentry_cli-2.17.2/src/utils/xcode.rs
```

### Comparing `sentry_cli-2.17.1/Cargo.lock` & `sentry_cli-2.17.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2191,15 +2191,15 @@
  "once_cell",
  "regex",
  "sentry-core",
 ]
 
 [[package]]
 name = "sentry-cli"
-version = "2.17.1"
+version = "2.17.2"
 dependencies = [
  "anyhow",
  "anylog",
  "backoff",
  "backtrace",
  "brotli2",
  "bytecount",
```

### Comparing `sentry_cli-2.17.1/Cargo.toml` & `sentry_cli-2.17.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 authors = ["Armin Ronacher <armin.ronacher@active-4.com>"]
 build = "build.rs"
 name = "sentry-cli"
-version = "2.17.1"
+version = "2.17.2"
 edition = "2021"
 rust-version = "1.65"
 
 [dependencies]
 anylog = "0.6.3"
 anyhow = { version = "1.0.69", features = ["backtrace"] }
 backoff = "0.4.0"
```

### Comparing `sentry_cli-2.17.1/LICENSE` & `sentry_cli-2.17.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/PKG-INFO` & `sentry_cli-2.17.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry_cli
-Version: 2.17.1
+Version: 2.17.2
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry_cli Version: 2.17.1 Summary: A command line
+Metadata-Version: 2.1 Name: sentry_cli Version: 2.17.2 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.17.1/README.md` & `sentry_cli-2.17.2/README.md`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/build.rs` & `sentry_cli-2.17.2/build.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/sentry_cli.egg-info/PKG-INFO` & `sentry_cli-2.17.2/sentry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-cli
-Version: 2.17.1
+Version: 2.17.2
 Summary: A command line utility to work with Sentry.
 Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry
 Author-email: oss@sentry.io
 License: BSD-3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sentry-cli Version: 2.17.1 Summary: A command line
+Metadata-Version: 2.1 Name: sentry-cli Version: 2.17.2 Summary: A command line
 utility to work with Sentry. Home-page: https://github.com/getsentry/sentry-cli
 Author: Sentry Author-email: oss@sentry.io License: BSD-3-Clause Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: Implementation :: CPython Classifier:
 Programming Language :: Python :: Implementation :: PyPy Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `sentry_cli-2.17.1/sentry_cli.egg-info/SOURCES.txt` & `sentry_cli-2.17.2/sentry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/setup.cfg` & `sentry_cli-2.17.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/setup.py` & `sentry_cli-2.17.2/setup.py`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/api.rs` & `sentry_cli-2.17.2/src/api.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/bashsupport.sh` & `sentry_cli-2.17.2/src/bashsupport.sh`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/bash_hook.rs` & `sentry_cli-2.17.2/src/commands/bash_hook.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/debug_files/bundle_sources.rs` & `sentry_cli-2.17.2/src/commands/debug_files/bundle_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/debug_files/check.rs` & `sentry_cli-2.17.2/src/commands/debug_files/check.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/debug_files/find.rs` & `sentry_cli-2.17.2/src/commands/debug_files/find.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/debug_files/mod.rs` & `sentry_cli-2.17.2/src/commands/debug_files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/debug_files/print_sources.rs` & `sentry_cli-2.17.2/src/commands/debug_files/print_sources.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/debug_files/upload.rs` & `sentry_cli-2.17.2/src/commands/debug_files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/deploys/list.rs` & `sentry_cli-2.17.2/src/commands/deploys/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/deploys/mod.rs` & `sentry_cli-2.17.2/src/commands/deploys/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/deploys/new.rs` & `sentry_cli-2.17.2/src/commands/deploys/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/events/list.rs` & `sentry_cli-2.17.2/src/commands/events/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/events/mod.rs` & `sentry_cli-2.17.2/src/commands/events/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/files/delete.rs` & `sentry_cli-2.17.2/src/commands/files/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/files/list.rs` & `sentry_cli-2.17.2/src/commands/files/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/files/mod.rs` & `sentry_cli-2.17.2/src/commands/files/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/files/upload.rs` & `sentry_cli-2.17.2/src/commands/files/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/info.rs` & `sentry_cli-2.17.2/src/commands/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/issues/mod.rs` & `sentry_cli-2.17.2/src/commands/issues/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/issues/mute.rs` & `sentry_cli-2.17.2/src/commands/issues/mute.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/issues/resolve.rs` & `sentry_cli-2.17.2/src/commands/issues/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/issues/unresolve.rs` & `sentry_cli-2.17.2/src/commands/issues/unresolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/login.rs` & `sentry_cli-2.17.2/src/commands/login.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/mod.rs` & `sentry_cli-2.17.2/src/commands/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/monitors/list.rs` & `sentry_cli-2.17.2/src/commands/monitors/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/monitors/mod.rs` & `sentry_cli-2.17.2/src/commands/monitors/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/monitors/run.rs` & `sentry_cli-2.17.2/src/commands/monitors/run.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/organizations/list.rs` & `sentry_cli-2.17.2/src/commands/organizations/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/organizations/mod.rs` & `sentry_cli-2.17.2/src/commands/organizations/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/projects/list.rs` & `sentry_cli-2.17.2/src/commands/projects/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/projects/mod.rs` & `sentry_cli-2.17.2/src/commands/projects/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/react_native/appcenter.rs` & `sentry_cli-2.17.2/src/commands/react_native/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/react_native/gradle.rs` & `sentry_cli-2.17.2/src/commands/react_native/gradle.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/react_native/mod.rs` & `sentry_cli-2.17.2/src/commands/react_native/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/react_native/xcode.rs` & `sentry_cli-2.17.2/src/commands/react_native/xcode.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/releases/archive.rs` & `sentry_cli-2.17.2/src/commands/releases/archive.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/releases/delete.rs` & `sentry_cli-2.17.2/src/commands/releases/delete.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/releases/finalize.rs` & `sentry_cli-2.17.2/src/commands/releases/finalize.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/releases/info.rs` & `sentry_cli-2.17.2/src/commands/releases/info.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/releases/list.rs` & `sentry_cli-2.17.2/src/commands/releases/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/releases/mod.rs` & `sentry_cli-2.17.2/src/commands/releases/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/releases/new.rs` & `sentry_cli-2.17.2/src/commands/releases/new.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/releases/restore.rs` & `sentry_cli-2.17.2/src/commands/releases/restore.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/releases/set_commits.rs` & `sentry_cli-2.17.2/src/commands/releases/set_commits.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/repos/list.rs` & `sentry_cli-2.17.2/src/commands/repos/list.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/repos/mod.rs` & `sentry_cli-2.17.2/src/commands/repos/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/send_envelope.rs` & `sentry_cli-2.17.2/src/commands/send_envelope.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/send_event.rs` & `sentry_cli-2.17.2/src/commands/send_event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/sourcemaps/explain.rs` & `sentry_cli-2.17.2/src/commands/sourcemaps/explain.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/sourcemaps/mod.rs` & `sentry_cli-2.17.2/src/commands/sourcemaps/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/sourcemaps/resolve.rs` & `sentry_cli-2.17.2/src/commands/sourcemaps/resolve.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/sourcemaps/upload.rs` & `sentry_cli-2.17.2/src/commands/sourcemaps/upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/uninstall.rs` & `sentry_cli-2.17.2/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/update.rs` & `sentry_cli-2.17.2/src/commands/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/commands/upload_proguard.rs` & `sentry_cli-2.17.2/src/commands/upload_proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/config.rs` & `sentry_cli-2.17.2/src/config.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/constants.rs` & `sentry_cli-2.17.2/src/constants.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/android.rs` & `sentry_cli-2.17.2/src/utils/android.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/appcenter.rs` & `sentry_cli-2.17.2/src/utils/appcenter.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/args.rs` & `sentry_cli-2.17.2/src/utils/args.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/chunks.rs` & `sentry_cli-2.17.2/src/utils/chunks.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/codepush.rs` & `sentry_cli-2.17.2/src/utils/codepush.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/cordova.rs` & `sentry_cli-2.17.2/src/utils/cordova.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/dif.rs` & `sentry_cli-2.17.2/src/utils/dif.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/dif_upload.rs` & `sentry_cli-2.17.2/src/utils/dif_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/enc.rs` & `sentry_cli-2.17.2/src/utils/enc.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/event.rs` & `sentry_cli-2.17.2/src/utils/event.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/file_search.rs` & `sentry_cli-2.17.2/src/utils/file_search.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/file_upload.rs` & `sentry_cli-2.17.2/src/utils/file_upload.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/formatting.rs` & `sentry_cli-2.17.2/src/utils/formatting.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/fs.rs` & `sentry_cli-2.17.2/src/utils/fs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/http.rs` & `sentry_cli-2.17.2/src/utils/http.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/logging.rs` & `sentry_cli-2.17.2/src/utils/logging.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/progress.rs` & `sentry_cli-2.17.2/src/utils/progress.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/releases.rs` & `sentry_cli-2.17.2/src/utils/releases.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/retry.rs` & `sentry_cli-2.17.2/src/utils/retry.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap` & `sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_default_twenty.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap` & `sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_ignore_missing.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap` & `sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__generate_patch_set_base.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap` & `sentry_cli-2.17.2/src/utils/snapshots/sentry_cli__utils__vcs__get_commits_from_git.snap`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/sourcemaps/inject.rs` & `sentry_cli-2.17.2/src/utils/sourcemaps/inject.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 use std::io::{BufRead, Write};
 use std::path::PathBuf;
 
 use anyhow::{bail, Result};
 use log::debug;
 use sentry::types::DebugId;
 use serde_json::Value;
-use uuid::Uuid;
 
 const CODE_SNIPPET_TEMPLATE: &str = r#"!function(){try{var e="undefined"!=typeof window?window:"undefined"!=typeof global?global:"undefined"!=typeof self?self:{},n=(new Error).stack;n&&(e._sentryDebugIds=e._sentryDebugIds||{},e._sentryDebugIds[n]="__SENTRY_DEBUG_ID__")}catch(e){}}()"#;
 const DEBUGID_PLACEHOLDER: &str = "__SENTRY_DEBUG_ID__";
 const SOURCEMAP_DEBUGID_KEY: &str = "debug_id";
 const DEBUGID_COMMENT_PREFIX: &str = "//# debugId";
 
 fn print_section_with_debugid(
@@ -133,14 +132,23 @@
     if let Some(sourcemap_comment) = sourcemap_comment {
         writeln!(js_contents, "{sourcemap_comment}")?;
     }
 
     Ok(())
 }
 
+/// Generates a debug ID from bytes.
+pub fn debug_id_from_bytes_hashed(bytes: &[u8]) -> DebugId {
+    let mut hash = sha1_smol::Sha1::new();
+    hash.update(bytes);
+    let mut sha1_bytes = [0u8; 16];
+    sha1_bytes.copy_from_slice(&hash.digest().bytes()[..16]);
+    DebugId::from_uuid(uuid::Builder::from_sha1_bytes(sha1_bytes).into_uuid())
+}
+
 /// Fixes up a sourcemap file with a debug id.
 ///
 /// If the file already contains a debug id under the `debug_id` key, it is left unmodified.
 /// Otherwise, a fresh debug id is inserted under that key.
 ///
 /// In either case, the value of the `debug_id` key is returned.
 pub fn fixup_sourcemap(sourcemap_contents: &mut Vec<u8>) -> Result<(DebugId, bool)> {
@@ -154,18 +162,17 @@
         Some(id) => {
             let debug_id = serde_json::from_value(id.clone())?;
             debug!("Sourcemap already has a debug id");
             Ok((debug_id, false))
         }
 
         None => {
-            let debug_id = DebugId::from_uuid(Uuid::new_v4());
+            let debug_id = debug_id_from_bytes_hashed(sourcemap_contents);
             let id = serde_json::to_value(debug_id)?;
             map.insert(SOURCEMAP_DEBUGID_KEY.to_string(), id);
-
             sourcemap_contents.clear();
             serde_json::to_writer(sourcemap_contents, &sourcemap)?;
             Ok((debug_id, true))
         }
     }
 }
```

### Comparing `sentry_cli-2.17.1/src/utils/sourcemaps.rs` & `sentry_cli-2.17.2/src/utils/sourcemaps.rs`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,31 @@
 fn is_hermes_bytecode(slice: &[u8]) -> bool {
     // The hermes bytecode format magic is defined here:
     // https://github.com/facebook/hermes/blob/5243222ef1d92b7393d00599fc5cff01d189a88a/include/hermes/BCGen/HBC/BytecodeFileFormat.h#L24-L25
     const HERMES_MAGIC: [u8; 8] = [0xC6, 0x1F, 0xBC, 0x03, 0xC1, 0x03, 0x19, 0x1F];
     slice.starts_with(&HERMES_MAGIC)
 }
 
+fn url_matches_extension(url: &str, extensions: &[&str]) -> bool {
+    if extensions.is_empty() {
+        return true;
+    }
+    url.rsplit('/')
+        .next()
+        .and_then(|filename| {
+            let mut splitter = filename.rsplit('.');
+            let rv = splitter.next();
+            // need another segment
+            splitter.next()?;
+            rv
+        })
+        .map(|ext| extensions.contains(&ext))
+        .unwrap_or(false)
+}
+
 impl SourceMapProcessor {
     /// Creates a new sourcemap validator.
     pub fn new() -> SourceMapProcessor {
         SourceMapProcessor {
             pending_sources: HashSet::new(),
             sources: HashMap::new(),
             sourcemap_references: HashMap::new(),
@@ -299,15 +316,15 @@
             .map(|x| x.1)
             .filter(|x| x.ty == SourceFileType::SourceMap)
             .map(|x| x.url.to_string())
             .collect();
 
         for source in self.sources.values_mut() {
             // Skip everything but minified JS files.
-            if source.ty != SourceFileType::MinifiedSource || !source.url.ends_with(".js") {
+            if source.ty != SourceFileType::MinifiedSource {
                 continue;
             }
 
             if self.sourcemap_references.contains_key(&source.url) {
                 continue;
             }
 
@@ -731,15 +748,18 @@
     ///
     /// If a source file refers to a sourcemap and that sourcemap is locally
     /// available, the debug id will be injected there as well so as to tie
     /// them together. If for whatever reason the sourcemap already contains
     /// a debug id, it will be reused for the source file.
     ///
     /// If `dry_run` is false, this will modify the source and sourcemap files on disk!
-    pub fn inject_debug_ids(&mut self, dry_run: bool) -> Result<()> {
+    ///
+    /// The `js_extensions` is a list of file extensions that should be considered
+    /// for JavaScript files.
+    pub fn inject_debug_ids(&mut self, dry_run: bool, js_extensions: &[&str]) -> Result<()> {
         self.flush_pending_sources();
         println!("{} Injecting debug ids", style(">").dim());
 
         let mut report = InjectReport::default();
 
         // Step 1: Produce a debug id for each source file by either reading it from the
         // sourcemap if available or else generating a fresh one.
@@ -749,28 +769,49 @@
             if let Some(debug_id) = self.debug_ids.get(source_url) {
                 report
                     .previously_injected
                     .push((source_url.into(), *debug_id));
                 continue;
             }
 
-            let Some(sourcemap_url) = sourcemap_url else {
-                debug_ids.push((source_url.clone(), DebugId::from_uuid(Uuid::new_v4())));
-                continue;
+            let sourcemap_url = match sourcemap_url {
+                Some(sourcemap_url) => sourcemap_url,
+                None => {
+                    // no source map at all, try a deterministic debug id from the contents
+                    let debug_id = self
+                        .sources
+                        .get(source_url)
+                        .map(|s| inject::debug_id_from_bytes_hashed(&s.contents))
+                        .unwrap_or_else(|| DebugId::from_uuid(Uuid::new_v4()));
+                    debug_ids.push((source_url.clone(), debug_id));
+                    continue;
+                }
             };
 
             if sourcemap_url.starts_with(DATA_PREAMBLE) {
-                debug_ids.push((source_url.clone(), DebugId::from_uuid(Uuid::new_v4())));
+                // source map is a url, hash the source map url for the debug id
+                let debug_id = inject::debug_id_from_bytes_hashed(sourcemap_url.as_bytes());
+                debug_ids.push((source_url.clone(), debug_id));
             } else {
                 let sourcemap_url = normalize_sourcemap_url(source_url, sourcemap_url);
-                let Some(sourcemap_file) = self.sources.get_mut(&sourcemap_url) else {
-                debug!("Sourcemap file {} not found", sourcemap_url);
-                debug_ids.push((source_url.clone(), DebugId::from_uuid(Uuid::new_v4())));
-                continue;
-            };
+                let sourcemap_file = match self.sources.get_mut(&sourcemap_url) {
+                    Some(sourcemap_file) => sourcemap_file,
+                    None => {
+                        debug!("Sourcemap file {} not found", sourcemap_url);
+                        // source map cannot be found, fall back to hashing the contents if
+                        // available.  The v4 fallback should not happen.
+                        let debug_id = self
+                            .sources
+                            .get(source_url)
+                            .map(|s| inject::debug_id_from_bytes_hashed(&s.contents))
+                            .unwrap_or_else(|| DebugId::from_uuid(Uuid::new_v4()));
+                        debug_ids.push((source_url.clone(), debug_id));
+                        continue;
+                    }
+                };
 
                 let (debug_id, sourcemap_modified) =
                     inject::fixup_sourcemap(&mut sourcemap_file.contents).context(format!(
                         "Failed to process {}",
                         sourcemap_file.path.display()
                     ))?;
 
@@ -798,14 +839,23 @@
 
                 debug_ids.push((source_url.clone(), debug_id));
             }
         }
 
         // Step 2: Iterate over the minified source files and inject the debug ids.
         for (source_url, debug_id) in debug_ids {
+            // We only allow injection into files that match the extension
+            if !url_matches_extension(&source_url, js_extensions) {
+                debug!(
+                    "skipping potential js file {} because it does not match extension",
+                    source_url
+                );
+                continue;
+            }
+
             let source_file = self.sources.get_mut(&source_url).unwrap();
 
             fixup_js_file(&mut source_file.contents, debug_id)
                 .context(format!("Failed to process {}", source_file.path.display()))?;
 
             source_file
                 .headers
@@ -928,7 +978,15 @@
         "https://example.com/foo.html"
     );
     assert_eq!(
         &join_url("https://example.com/", "foo.html").unwrap(),
         "https://example.com/foo.html"
     );
 }
+
+#[test]
+fn test_url_matches_extension() {
+    assert!(url_matches_extension("foo.js", &["js"][..]));
+    assert!(!url_matches_extension("foo.mjs", &["js"][..]));
+    assert!(url_matches_extension("foo.mjs", &["js", "mjs"][..]));
+    assert!(!url_matches_extension("js", &["js"][..]));
+}
```

### Comparing `sentry_cli-2.17.1/src/utils/system.rs` & `sentry_cli-2.17.2/src/utils/system.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/ui.rs` & `sentry_cli-2.17.2/src/utils/ui.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/update.rs` & `sentry_cli-2.17.2/src/utils/update.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/vcs.rs` & `sentry_cli-2.17.2/src/utils/vcs.rs`

 * *Files identical despite different names*

### Comparing `sentry_cli-2.17.1/src/utils/xcode.rs` & `sentry_cli-2.17.2/src/utils/xcode.rs`

 * *Files identical despite different names*

