# Comparing `tmp/kraken_std-0.8.3.tar.gz` & `tmp/kraken_std-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_std-0.8.3.tar", max compression
+gzip compressed data, was "kraken_std-0.8.4.tar", max compression
```

## Comparing `kraken_std-0.8.3.tar` & `kraken_std-0.8.4.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0      988 2023-01-22 14:38:01.549959 kraken_std-0.8.3/LICENSE
--rw-r--r--   0        0        0     1745 2023-04-05 22:23:38.384591 kraken_std-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     1498 2023-02-08 16:53:28.240291 kraken_std-0.8.3/readme.md
--rw-r--r--   0        0        0       22 2023-04-05 22:23:38.384591 kraken_std-0.8.3/src/kraken/std/__init__.py
--rw-r--r--   0        0        0    12840 2023-04-05 21:42:55.754805 kraken_std-0.8.3/src/kraken/std/cargo/__init__.py
--rw-r--r--   0        0        0     2403 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/cargo/config.py
--rw-r--r--   0        0        0     1753 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/cargo/data/certs/cert.pem
--rw-r--r--   0        0        0     3243 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/cargo/data/certs/key.pem
--rw-r--r--   0        0        0     7912 2023-04-05 21:42:55.754805 kraken_std-0.8.3/src/kraken/std/cargo/manifest.py
--rw-r--r--   0        0        0     2294 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/cargo/mitm.py
--rw-r--r--   0        0        0     1737 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/cargo/mitm_impl.py
--rw-r--r--   0        0        0        0 2023-03-06 13:53:50.490907 kraken_std-0.8.3/src/kraken/std/cargo/tasks/__init__.py
--rw-r--r--   0        0        0     5640 2023-03-20 14:35:25.194513 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
--rw-r--r--   0        0        0     5523 2023-03-06 13:53:50.490907 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_build_task.py
--rw-r--r--   0        0        0     3163 2023-04-05 21:42:55.754805 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_bump_version_task.py
--rw-r--r--   0        0        0     2177 2023-03-20 14:35:25.194513 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
--rw-r--r--   0        0        0      907 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_clippy_task.py
--rw-r--r--   0        0        0      704 2023-04-05 21:42:55.754805 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_deny_task.py
--rw-r--r--   0        0        0      730 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_fmt_task.py
--rw-r--r--   0        0        0     2074 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_publish_task.py
--rw-r--r--   0        0        0     2088 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
--rw-r--r--   0        0        0      493 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_test_task.py
--rw-r--r--   0        0        0      391 2023-02-14 17:29:44.373684 kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_update_task.py
--rw-r--r--   0        0        0      720 2023-03-06 13:53:50.490907 kraken_std-0.8.3/src/kraken/std/cargo/version.py
--rw-r--r--   0        0        0        0 2023-03-06 13:53:50.490907 kraken_std-0.8.3/src/kraken/std/descriptors/__init__.py
--rw-r--r--   0        0        0      874 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/descriptors/resource.py
--rw-r--r--   0        0        0    10002 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/dist.py
--rw-r--r--   0        0        0     3911 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/docker/__init__.py
--rw-r--r--   0        0        0     3254 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/docker/buildx.py
--rw-r--r--   0        0        0     1426 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/docker/dockerapi.py
--rw-r--r--   0        0        0     7438 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/docker/kaniko.py
--rw-r--r--   0        0        0     1938 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/docker/manifest_tool.py
--rw-r--r--   0        0        0     3650 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/docker/native.py
--rw-r--r--   0        0        0        0 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/docker/py.typed
--rw-r--r--   0        0        0     1214 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/docker/util.py
--rw-r--r--   0        0        0     1761 2023-04-05 21:42:55.754805 kraken_std-0.8.3/src/kraken/std/git/__init__.py
--rw-r--r--   0        0        0     1107 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/git/config.py
--rw-r--r--   0        0        0     9445 2023-04-05 21:42:55.754805 kraken_std-0.8.3/src/kraken/std/git/gitignore.py
--rw-r--r--   0        0        0        0 2023-03-06 13:53:50.490907 kraken_std-0.8.3/src/kraken/std/git/tasks/__init__.py
--rw-r--r--   0        0        0      448 2023-04-05 21:42:55.754805 kraken_std-0.8.3/src/kraken/std/git/tasks/const.py
--rw-r--r--   0        0        0     2919 2023-04-05 21:42:55.754805 kraken_std-0.8.3/src/kraken/std/git/tasks/gitignore_check_task.py
--rw-r--r--   0        0        0     2754 2023-04-05 21:42:55.754805 kraken_std-0.8.3/src/kraken/std/git/tasks/gitignore_sync_task.py
--rw-r--r--   0        0        0     2973 2023-03-06 13:53:50.490907 kraken_std-0.8.3/src/kraken/std/git/version.py
--rw-r--r--   0        0        0     6362 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/helm/__init__.py
--rw-r--r--   0        0        0     2132 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/helm/helmapi.py
--rw-r--r--   0        0        0        0 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/py.typed
--rw-r--r--   0        0        0     1598 2023-04-05 22:03:25.898196 kraken_std-0.8.3/src/kraken/std/python/__init__.py
--rw-r--r--   0        0        0     3586 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/buildsystem/__init__.py
--rw-r--r--   0        0        0     1347 2023-04-05 22:23:34.040338 kraken_std-0.8.3/src/kraken/std/python/buildsystem/helpers.py
--rw-r--r--   0        0        0     3120 2023-03-06 13:53:50.494907 kraken_std-0.8.3/src/kraken/std/python/buildsystem/maturin.py
--rw-r--r--   0        0        0     7926 2023-04-05 22:23:34.040338 kraken_std-0.8.3/src/kraken/std/python/buildsystem/poetry.py
--rw-r--r--   0        0        0     4415 2023-04-05 22:03:27.278276 kraken_std-0.8.3/src/kraken/std/python/buildsystem/slap.py
--rw-r--r--   0        0        0     4892 2023-04-05 22:23:34.040338 kraken_std-0.8.3/src/kraken/std/python/pyproject.py
--rw-r--r--   0        0        0     6401 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/python/settings.py
--rw-r--r--   0        0        0        0 2023-03-06 13:53:50.494907 kraken_std-0.8.3/src/kraken/std/python/tasks/__init__.py
--rw-r--r--   0        0        0     3249 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/tasks/base_task.py
--rw-r--r--   0        0        0     2076 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/tasks/black_task.py
--rw-r--r--   0        0        0     1922 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/python/tasks/build_task.py
--rw-r--r--   0        0        0     1046 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/tasks/flake8_task.py
--rw-r--r--   0        0        0     2834 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/python/tasks/install_task.py
--rw-r--r--   0        0        0     1844 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/tasks/isort_task.py
--rw-r--r--   0        0        0      946 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/tasks/login_task.py
--rw-r--r--   0        0        0     1463 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/tasks/mypy_subtest_task.py
--rw-r--r--   0        0        0     2352 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/tasks/mypy_task.py
--rw-r--r--   0        0        0     2598 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/python/tasks/publish_task.py
--rw-r--r--   0        0        0     2043 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/tasks/pycln_task.py
--rw-r--r--   0        0        0     1034 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/tasks/pylint_task.py
--rw-r--r--   0        0        0     2398 2023-03-06 13:53:50.494907 kraken_std-0.8.3/src/kraken/std/python/tasks/pytest_task.py
--rw-r--r--   0        0        0     4531 2023-03-06 13:53:50.494907 kraken_std-0.8.3/src/kraken/std/python/tasks/pyupgrade_task.py
--rw-r--r--   0        0        0     1778 2023-02-08 16:53:28.240291 kraken_std-0.8.3/src/kraken/std/python/tasks/update_lockfile_task.py
--rw-r--r--   0        0        0     1656 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/python/tasks/update_pyproject_task.py
--rw-r--r--   0        0        0     1127 2023-03-20 14:35:25.194513 kraken_std-0.8.3/src/kraken/std/python/version.py
--rw-r--r--   0        0        0     4042 2023-01-22 14:38:01.549959 kraken_std-0.8.3/src/kraken/std/sccache.py
--rw-r--r--   0        0        0      390 2023-03-20 14:35:25.194513 kraken_std-0.8.3/src/kraken/std/util/__init__.py
--rw-r--r--   0        0        0     1906 2023-03-20 14:35:25.194513 kraken_std-0.8.3/src/kraken/std/util/check_file_exists_and_is_committed_task.py
--rw-r--r--   0        0        0     6010 2023-03-20 14:35:25.194513 kraken_std-0.8.3/src/kraken/std/util/check_valid_readme_exists_task.py
--rw-r--r--   0        0        0     2645 2023-03-20 14:35:25.194513 kraken_std-0.8.3/src/kraken/std/util/copyright_task.py
--rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 kraken_std-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-04-12 13:02:29.929332 kraken_std-0.8.4/LICENSE
+-rw-r--r--   0        0        0     1745 2023-04-12 13:03:14.573957 kraken_std-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     1498 2023-04-12 13:02:29.933332 kraken_std-0.8.4/readme.md
+-rw-r--r--   0        0        0       22 2023-04-12 13:03:14.573957 kraken_std-0.8.4/src/kraken/std/__init__.py
+-rw-r--r--   0        0        0    13390 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/__init__.py
+-rw-r--r--   0        0        0     2403 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/config.py
+-rw-r--r--   0        0        0     1753 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/data/certs/cert.pem
+-rw-r--r--   0        0        0     3243 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/data/certs/key.pem
+-rw-r--r--   0        0        0     7912 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/manifest.py
+-rw-r--r--   0        0        0     2294 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/mitm.py
+-rw-r--r--   0        0        0     1737 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/mitm_impl.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/__init__.py
+-rw-r--r--   0        0        0     5640 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py
+-rw-r--r--   0        0        0     5959 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_build_task.py
+-rw-r--r--   0        0        0     3163 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_bump_version_task.py
+-rw-r--r--   0        0        0     2177 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py
+-rw-r--r--   0        0        0      907 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_clippy_task.py
+-rw-r--r--   0        0        0      732 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_deny_task.py
+-rw-r--r--   0        0        0      730 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_fmt_task.py
+-rw-r--r--   0        0        0     2074 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_publish_task.py
+-rw-r--r--   0        0        0     2088 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_sync_config_task.py
+-rw-r--r--   0        0        0      493 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_test_task.py
+-rw-r--r--   0        0        0      391 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_update_task.py
+-rw-r--r--   0        0        0      720 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/cargo/version.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/descriptors/__init__.py
+-rw-r--r--   0        0        0      874 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/descriptors/resource.py
+-rw-r--r--   0        0        0    10002 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/dist.py
+-rw-r--r--   0        0        0     3911 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/__init__.py
+-rw-r--r--   0        0        0     3254 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/buildx.py
+-rw-r--r--   0        0        0     1426 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/dockerapi.py
+-rw-r--r--   0        0        0     7438 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/kaniko.py
+-rw-r--r--   0        0        0     1938 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/manifest_tool.py
+-rw-r--r--   0        0        0     3650 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/native.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/py.typed
+-rw-r--r--   0        0        0     1214 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/docker/util.py
+-rw-r--r--   0        0        0     1761 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/__init__.py
+-rw-r--r--   0        0        0     1107 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/config.py
+-rw-r--r--   0        0        0     9451 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/gitignore.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/tasks/__init__.py
+-rw-r--r--   0        0        0      448 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/tasks/const.py
+-rw-r--r--   0        0        0     2919 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/tasks/gitignore_check_task.py
+-rw-r--r--   0        0        0     2754 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/tasks/gitignore_sync_task.py
+-rw-r--r--   0        0        0     2973 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/git/version.py
+-rw-r--r--   0        0        0     6368 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/helm/__init__.py
+-rw-r--r--   0        0        0     2132 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/helm/helmapi.py
+-rw-r--r--   0        0        0     2310 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/http/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/py.typed
+-rw-r--r--   0        0        0     1598 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/__init__.py
+-rw-r--r--   0        0        0     3586 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/buildsystem/__init__.py
+-rw-r--r--   0        0        0     1332 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/buildsystem/helpers.py
+-rw-r--r--   0        0        0     3120 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/buildsystem/maturin.py
+-rw-r--r--   0        0        0     7926 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/buildsystem/poetry.py
+-rw-r--r--   0        0        0     4415 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/buildsystem/slap.py
+-rw-r--r--   0        0        0     4892 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/pyproject.py
+-rw-r--r--   0        0        0     6401 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/settings.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/__init__.py
+-rw-r--r--   0        0        0     3249 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/base_task.py
+-rw-r--r--   0        0        0     2076 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/black_task.py
+-rw-r--r--   0        0        0     1922 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/build_task.py
+-rw-r--r--   0        0        0     1046 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/flake8_task.py
+-rw-r--r--   0        0        0     2834 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/install_task.py
+-rw-r--r--   0        0        0     1844 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/isort_task.py
+-rw-r--r--   0        0        0      946 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/login_task.py
+-rw-r--r--   0        0        0     1463 2023-04-12 13:02:29.933332 kraken_std-0.8.4/src/kraken/std/python/tasks/mypy_subtest_task.py
+-rw-r--r--   0        0        0     2352 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/mypy_task.py
+-rw-r--r--   0        0        0     2598 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/publish_task.py
+-rw-r--r--   0        0        0     2043 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/pycln_task.py
+-rw-r--r--   0        0        0     1034 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/pylint_task.py
+-rw-r--r--   0        0        0     2398 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/pytest_task.py
+-rw-r--r--   0        0        0     4531 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/pyupgrade_task.py
+-rw-r--r--   0        0        0     1778 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/update_lockfile_task.py
+-rw-r--r--   0        0        0     1656 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/tasks/update_pyproject_task.py
+-rw-r--r--   0        0        0     1127 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/python/version.py
+-rw-r--r--   0        0        0     4042 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/sccache.py
+-rw-r--r--   0        0        0      390 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/util/__init__.py
+-rw-r--r--   0        0        0     1906 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/util/check_file_exists_and_is_committed_task.py
+-rw-r--r--   0        0        0     6010 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/util/check_valid_readme_exists_task.py
+-rw-r--r--   0        0        0     2645 2023-04-12 13:02:29.937332 kraken_std-0.8.4/src/kraken/std/util/copyright_task.py
+-rw-r--r--   0        0        0     2516 1970-01-01 00:00:00.000000 kraken_std-0.8.4/PKG-INFO
```

### Comparing `kraken_std-0.8.3/LICENSE` & `kraken_std-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/pyproject.toml` & `kraken_std-0.8.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-std"
-version = "0.8.3"
+version = "0.8.4"
 description = "The Kraken standard library."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 packages = [{ include = "kraken/std", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `kraken_std-0.8.3/readme.md` & `kraken_std-0.8.4/readme.md`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/__init__.py` & `kraken_std-0.8.4/src/kraken/std/cargo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,14 +145,23 @@
     # Clippy builds your code.
     task.add_relationship(f":{CARGO_BUILD_SUPPORT_GROUP_NAME}?")
 
     return task
 
 
 def cargo_deny(*, project: Project | None = None, **kwargs: Any) -> CargoDenyTask:
+    """Adds a task running cargo-deny for cargo projects. This checks different rules on dependencies, such as scanning
+    for vulnerabilities, unwanted licences, or custom bans.
+
+    :param checks: The list of cargo-deny checks to run, as defined in
+    https://embarkstudios.github.io/cargo-deny/checks/index.html. If not provided, defaults to all of them.
+    :param config_file: The configuration file as defined in https://embarkstudios.github.io/cargo-deny/checks/cfg.html
+    If not provided defaults to cargo-deny default location.
+    """
+
     project = project or Project.current()
     return project.do("cargoDeny", CargoDenyTask, **kwargs)
 
 
 def cargo_fmt(*, all_packages: bool = False, project: Project | None = None) -> None:
     project = project or Project.current()
     project.do("cargoFmt", CargoFmtTask, all_packages=all_packages, group="fmt")
```

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/config.py` & `kraken_std-0.8.4/src/kraken/std/cargo/config.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/data/certs/cert.pem` & `kraken_std-0.8.4/src/kraken/std/cargo/data/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/data/certs/key.pem` & `kraken_std-0.8.4/src/kraken/std/cargo/data/certs/key.pem`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/manifest.py` & `kraken_std-0.8.4/src/kraken/std/cargo/manifest.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/mitm.py` & `kraken_std-0.8.4/src/kraken/std/cargo/mitm.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/mitm_impl.py` & `kraken_std-0.8.4/src/kraken/std/cargo/mitm_impl.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py` & `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_auth_proxy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_build_task.py` & `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_build_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,51 +74,57 @@
         command = self.get_cargo_command(env) + self.get_cargo_command_additional_flags()
 
         safe_command = command[:]
         safe_env = env.copy()
         self.make_safe(safe_command, safe_env)
         self.logger.info("%s [env: %s]", safe_command, safe_env)
 
-        out_binaries = []
-        out_libraries = []
+        out_binaries: List[CargoBinaryArtifact] = []
+        out_libraries_candidates: List[CargoLibraryArtifact] = []
         if self.target.get_or(None) in ("debug", "release"):
             # Expose the output binaries that are produced by this task.
             # We only expect a binary to be built if the target is debug or release.
             manifest = CargoMetadata.read(self.project.directory)
-            target_dir = self.project.directory / os.getenv("CARGO_TARGET_DIR", "target") / self.target.get()
+            target_dir = manifest.target_directory / self.target.get()
             for artifact in manifest.artifacts:
                 # Rust binaries have an extensionless name whereas libraries are prefixed with "lib" and suffixed with
                 #
                 # - ".rlib" for Rust libraries
                 # - ".so" (Linux), ".dylib" (macOS) or ".dll" (Windows) for dynamic Rust and system libraries
                 # - ".a" (Linux, macOS) or ".lib" (Windows) for static system libraries
-                #
-                # We create all options for libraries and check for presence of at least one later.
                 if artifact.kind is ArtifactKind.BIN:
                     out_binaries.append(CargoBinaryArtifact(artifact.name, target_dir / artifact.name))
                 elif artifact.kind is ArtifactKind.LIB:
                     base_name = f"lib{artifact.name}"
                     for file_extension in ["rlib", "so", "dylib", "dll", "a", "lib"]:
-                        filename = ".".join([base_name, file_extension]).replace("-", "_")
-                        out_libraries.append(CargoLibraryArtifact(base_name, target_dir / filename))
-
-        self.out_binaries.set(out_binaries)
-        self.out_libraries.set(out_libraries)
+                        filename = ".".join([base_name.replace("-", "_"), file_extension])
+                        out_libraries_candidates.append(CargoLibraryArtifact(base_name, target_dir / filename))
 
         total_attempts = self.retry_attempts.get() + 1
 
         while total_attempts > 0:
             result = sp.call(command, cwd=self.project.directory, env={**os.environ, **env})
 
             if result == 0:
                 # Check that binaries which were due have been built.
                 for out_bin in out_binaries:
                     assert out_bin.path.is_file(), out_bin
+                self.out_binaries.set(out_binaries)
+
                 # Check that at least one library has been built if libraries were due.
-                assert not out_libraries or any(lib.path.is_file() for lib in out_libraries), out_libraries[0].name
+                out_libraries = []
+                if len(out_libraries_candidates) != 0:
+                    for out_libraries_candidate in out_libraries_candidates:
+                        # Since we generate all possible file extensions, we must only keep the ones that exist
+                        if out_libraries_candidate.path.is_file():
+                            out_libraries.append(out_libraries_candidate)
+                    assert (
+                        len(out_libraries) != 0
+                    ), f'No libraries were built even though some were due, e.g. "{out_libraries_candidates[0].name}"'
+                self.out_libraries.set(out_libraries)
                 break
             else:
                 total_attempts -= 1
                 self.logger.warn("%s failed with result %s", safe_command, result)
                 self.logger.warn("There are %s attempts remaining", total_attempts)
                 if total_attempts > 0:
                     self.logger.info("Waiting for 10 seconds before retrying..")
```

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_bump_version_task.py` & `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_bump_version_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py` & `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_check_toolchain_version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_clippy_task.py` & `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_clippy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_deny_task.py` & `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_deny_task.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,9 +15,9 @@
         command = ["cargo", "deny", "check"]
 
         if self.config_file.is_filled():
             command.extend(["--config", str(self.config_file.get().absolute())])
 
         command.extend(self.checks.get())
 
-        result = subprocess.run(command)
+        result = subprocess.run(command, cwd=self.project.directory)
         return TaskStatus.from_exit_code(command, result.returncode)
```

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_fmt_task.py` & `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_fmt_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_publish_task.py` & `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/tasks/cargo_sync_config_task.py` & `kraken_std-0.8.4/src/kraken/std/cargo/tasks/cargo_sync_config_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/cargo/version.py` & `kraken_std-0.8.4/src/kraken/std/cargo/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/descriptors/resource.py` & `kraken_std-0.8.4/src/kraken/std/descriptors/resource.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/dist.py` & `kraken_std-0.8.4/src/kraken/std/dist.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/docker/__init__.py` & `kraken_std-0.8.4/src/kraken/std/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/docker/buildx.py` & `kraken_std-0.8.4/src/kraken/std/docker/buildx.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/docker/dockerapi.py` & `kraken_std-0.8.4/src/kraken/std/docker/dockerapi.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/docker/kaniko.py` & `kraken_std-0.8.4/src/kraken/std/docker/kaniko.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/docker/manifest_tool.py` & `kraken_std-0.8.4/src/kraken/std/docker/manifest_tool.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/docker/native.py` & `kraken_std-0.8.4/src/kraken/std/docker/native.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/docker/util.py` & `kraken_std-0.8.4/src/kraken/std/docker/util.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/git/__init__.py` & `kraken_std-0.8.4/src/kraken/std/git/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/git/config.py` & `kraken_std-0.8.4/src/kraken/std/git/config.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/git/gitignore.py` & `kraken_std-0.8.4/src/kraken/std/git/gitignore.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import io
 import re
 from itertools import islice
 from os import PathLike
 from pathlib import Path
 from typing import Iterable, NamedTuple, Optional, Sequence, TextIO
 
-import httpx
+from .. import http
 
 GITIGNORE_API_URL = "https://www.toptal.com/developers/gitignore/api/"
 GENERATED_GUARD_START_TEMPLATE = "### START-GENERATED-CONTENT [HASH: {hash}]"
 GENERATED_GUARD_START_REGEX = r"^### START-GENERATED-CONTENT \[HASH: (.*)\]$"
 PARAMETER_HASH_TEMPLATE = "### [PARAMETERS_HASH: {hash}]"
 PARAMETER_HASH_REGEX = r"^### \[PARAMETERS_HASH: (.*)\]$"
 GENERATED_GUARD_DESCRIPTION = """\
@@ -109,15 +109,15 @@
         ]
         user_content = map(str, self.entries)
         return "\n".join(guarded_section) + "\n" + "\n".join(user_content) + "\n"
 
     def refresh_generated_content(
         self, tokens: Sequence[str], extra_paths: Sequence[str], overrides: Sequence[str]
     ) -> None:
-        result = httpx.get(GITIGNORE_API_URL + ",".join(tokens))
+        result = http.get(GITIGNORE_API_URL + ",".join(tokens))
         if result.status_code != 200:
             raise GitignoreException(f"Error status code returned from {GITIGNORE_API_URL}")
 
         # MacOS's Icon file ends with a double \r, but this is removed by vscode upon saving.
         # To avoid a constant back and forth between user and sync tasks,
         # all \r chars are removed proactively
         fetched_content = result.text.replace("\r", "")
```

### Comparing `kraken_std-0.8.3/src/kraken/std/git/tasks/gitignore_check_task.py` & `kraken_std-0.8.4/src/kraken/std/git/tasks/gitignore_check_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/git/tasks/gitignore_sync_task.py` & `kraken_std-0.8.4/src/kraken/std/git/tasks/gitignore_sync_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/git/version.py` & `kraken_std-0.8.4/src/kraken/std/git/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/helm/__init__.py` & `kraken_std-0.8.4/src/kraken/std/helm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from __future__ import annotations
 
 import dataclasses
 import urllib.parse
 from pathlib import Path
 
-import httpx
 from kraken.core.api import Project, Property, Task, TaskStatus
 from nr.stream import Supplier
 
+from .. import http
 from . import helmapi
 
 
 @dataclasses.dataclass
 class HelmSettings:
     """Project-specific settings for Helm."""
 
@@ -134,14 +134,14 @@
             self.logger.info(
                 'pushing chart "%s" to %s registry %r',
                 self.chart_tarball.get(),
                 url.scheme.upper(),
                 self.registry.get(),
             )
             self.chart_url.set(urllib.parse.urljoin(self.registry.get() + "/", self.chart_name.get()))
-            response = httpx.put(self.chart_url.get(), content=self.chart_tarball.get().read_bytes(), auth=credentials)
+            response = http.put(self.chart_url.get(), content=self.chart_tarball.get().read_bytes(), auth=credentials)
             response.raise_for_status()
             self.logger.info("chart url = %s", self.chart_url.get())
         else:
             assert False, url
 
         return TaskStatus.succeeded()
```

### Comparing `kraken_std-0.8.3/src/kraken/std/helm/helmapi.py` & `kraken_std-0.8.4/src/kraken/std/helm/helmapi.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/__init__.py` & `kraken_std-0.8.4/src/kraken/std/python/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/buildsystem/__init__.py` & `kraken_std-0.8.4/src/kraken/std/python/buildsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/buildsystem/helpers.py` & `kraken_std-0.8.4/src/kraken/std/python/buildsystem/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Python build system helper functions """
 
 from __future__ import annotations
 
-import logging
 import re
 from pathlib import Path
 
 
 def update_python_version_str_in_source_files(as_version: str, package_directory: Path) -> int:
     """
     Updates the `__version__` in Python source files in the given *package_directory*. The constant is commonly
```

### Comparing `kraken_std-0.8.3/src/kraken/std/python/buildsystem/maturin.py` & `kraken_std-0.8.4/src/kraken/std/python/buildsystem/maturin.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/buildsystem/poetry.py` & `kraken_std-0.8.4/src/kraken/std/python/buildsystem/poetry.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/buildsystem/slap.py` & `kraken_std-0.8.4/src/kraken/std/python/buildsystem/slap.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/pyproject.py` & `kraken_std-0.8.4/src/kraken/std/python/pyproject.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/settings.py` & `kraken_std-0.8.4/src/kraken/std/python/settings.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/base_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/black_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/black_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/build_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/build_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/flake8_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/flake8_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/install_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/install_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/isort_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/isort_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/login_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/login_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/mypy_subtest_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/mypy_subtest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/mypy_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/mypy_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/publish_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/publish_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/pycln_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/pycln_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/pylint_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/pylint_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/pytest_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/pytest_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/pyupgrade_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/pyupgrade_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/update_lockfile_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/update_lockfile_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/tasks/update_pyproject_task.py` & `kraken_std-0.8.4/src/kraken/std/python/tasks/update_pyproject_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/python/version.py` & `kraken_std-0.8.4/src/kraken/std/python/version.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/sccache.py` & `kraken_std-0.8.4/src/kraken/std/sccache.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/util/check_file_exists_and_is_committed_task.py` & `kraken_std-0.8.4/src/kraken/std/util/check_file_exists_and_is_committed_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/util/check_valid_readme_exists_task.py` & `kraken_std-0.8.4/src/kraken/std/util/check_valid_readme_exists_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/src/kraken/std/util/copyright_task.py` & `kraken_std-0.8.4/src/kraken/std/util/copyright_task.py`

 * *Files identical despite different names*

### Comparing `kraken_std-0.8.3/PKG-INFO` & `kraken_std-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kraken-std
-Version: 0.8.3
+Version: 0.8.4
 Summary: The Kraken standard library.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

