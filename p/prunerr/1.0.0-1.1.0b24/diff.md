# Comparing `tmp/prunerr-1.0.0.tar.gz` & `tmp/prunerr-1.1.0b24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prunerr-1.0.0.tar", last modified: Tue Dec 13 09:28:56 2022, max compression
+gzip compressed data, was "prunerr-1.1.0b24.tar", last modified: Tue Apr 11 23:08:35 2023, max compression
```

## Comparing `prunerr-1.0.0.tar` & `prunerr-1.1.0b24.tar`

### file list

```diff
@@ -1,1331 +1,1373 @@
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.684892 prunerr-1.0.0/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      324 2022-12-13 09:25:38.000000 prunerr-1.0.0/.dir-locals.el.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1523 2022-12-13 09:25:38.000000 prunerr-1.0.0/.dockerignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      709 2022-12-13 09:25:38.000000 prunerr-1.0.0/.env.in
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.469881 prunerr-1.0.0/.github/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.583886 prunerr-1.0.0/.github/workflows/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4236 2022-12-13 09:25:38.000000 prunerr-1.0.0/.github/workflows/ci-cd.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1523 2022-12-13 09:25:38.000000 prunerr-1.0.0/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2696 2022-12-13 09:25:38.000000 prunerr-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      555 2022-12-13 09:25:38.000000 prunerr-1.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3448 2022-12-13 09:25:38.000000 prunerr-1.0.0/CONTRIBUTING.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1798 2022-12-13 09:25:38.000000 prunerr-1.0.0/Dockerfile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2380 2022-12-13 09:25:38.000000 prunerr-1.0.0/Dockerfile.devel
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2022-12-13 09:25:38.000000 prunerr-1.0.0/LICENSE
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    23815 2022-12-13 09:25:38.000000 prunerr-1.0.0/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      406 2022-12-13 09:27:25.000000 prunerr-1.0.0/NEWS.rst
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    12512 2022-12-13 09:28:56.684892 prunerr-1.0.0/PKG-INFO
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11771 2022-12-13 09:25:38.000000 prunerr-1.0.0/README.rst
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3687 2022-12-13 09:25:38.000000 prunerr-1.0.0/TODO.rst
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.583886 prunerr-1.0.0/bin/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      885 2022-12-13 09:25:38.000000 prunerr-1.0.0/bin/entrypoint
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2596 2022-12-13 09:25:38.000000 prunerr-1.0.0/docker-compose.override.yml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3860 2022-12-13 09:25:38.000000 prunerr-1.0.0/docker-compose.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.583886 prunerr-1.0.0/home/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       65 2022-12-13 09:25:38.000000 prunerr-1.0.0/home/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2022-12-13 09:25:38.000000 prunerr-1.0.0/home/.pypirc.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2393 2022-12-13 09:27:25.000000 prunerr-1.0.0/pyproject.toml
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2679 2022-12-13 09:25:38.000000 prunerr-1.0.0/requirements-build.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      766 2022-12-13 09:25:38.000000 prunerr-1.0.0/requirements-build.txt.in
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3709 2022-12-13 09:25:38.000000 prunerr-1.0.0/requirements-devel.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      808 2022-12-13 09:27:25.000000 prunerr-1.0.0/requirements.txt
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.470881 prunerr-1.0.0/s6/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.470881 prunerr-1.0.0/s6/etc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.470881 prunerr-1.0.0/s6/etc/s6-overlay/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.470881 prunerr-1.0.0/s6/etc/s6-overlay/s6-rc.d/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.583886 prunerr-1.0.0/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      609 2022-12-13 09:25:38.000000 prunerr-1.0.0/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1440 2022-12-13 09:28:56.685892 prunerr-1.0.0/setup.cfg
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.470881 prunerr-1.0.0/src/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.585887 prunerr-1.0.0/src/prunerr/
--rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     6647 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      183 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/__main__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15313 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9785 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/downloaditem.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.471881 prunerr-1.0.0/src/prunerr/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.586887 prunerr-1.0.0/src/prunerr/home/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9696 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/home/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.587887 prunerr-1.0.0/src/prunerr/newsfragments/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/newsfragments/.gitignore
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7881 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    18374 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    12657 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/servarr.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.589887 prunerr-1.0.0/src/prunerr/tests/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/Makefile
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22080 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/__init__.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/example-5s.mkv
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.472881 prunerr-1.0.0/src/prunerr/tests/home/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.471881 prunerr-1.0.0/src/prunerr/tests/home/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.590887 prunerr-1.0.0/src/prunerr/tests/home/daemon/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3014 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/home/daemon/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.471881 prunerr-1.0.0/src/prunerr/tests/home/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.590887 prunerr-1.0.0/src/prunerr/tests/home/download-client-only/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.472881 prunerr-1.0.0/src/prunerr/tests/home/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.590887 prunerr-1.0.0/src/prunerr/tests/home/download-clients/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2767 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/home/download-clients/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.472881 prunerr-1.0.0/src/prunerr/tests/home/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.590887 prunerr-1.0.0/src/prunerr/tests/home/download-items/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/home/download-items/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.472881 prunerr-1.0.0/src/prunerr/tests/home/empty/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.590887 prunerr-1.0.0/src/prunerr/tests/home/empty/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/home/empty/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.472881 prunerr-1.0.0/src/prunerr/tests/home/move-exec/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.591887 prunerr-1.0.0/src/prunerr/tests/home/move-exec/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/home/move-exec/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.473881 prunerr-1.0.0/src/prunerr/tests/home/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.591887 prunerr-1.0.0/src/prunerr/tests/home/review-edge-cases/.config/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      725 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.558885 prunerr-1.0.0/src/prunerr/tests/responses/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.473881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.477881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.473881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.473881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.474881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.473881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.591887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.591887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.591887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.474881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.591887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.592887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.592887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.474881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.474881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.592887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.592887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.592887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.475881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.475881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.476881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.475881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.593887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.593887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.593887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.476881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.476881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.594887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.594887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.476881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.593887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.594887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.594887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.476881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.477881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.594887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.595887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.595887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.595887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.477881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.477881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.477881 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.595887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.596887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.596887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.596887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.597887 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.478881 prunerr-1.0.0/src/prunerr/tests/responses/default/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.481881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.478881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.478881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.479881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.478881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.597887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.597887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.479881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.597887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.598887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.479881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.479881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.598887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.598887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.480882 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.480882 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.481881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.480882 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.598887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.598887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.481881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.481881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.599887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.599887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.480882 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.598887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.599887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.481881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.481881 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.599887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.599887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.482882 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.482882 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.482882 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.600887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.600887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.600887 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.601888 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.601888 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.482882 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.483882 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.483882 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.483882 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.483882 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.601888 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.602887 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.602887 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.488882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.488882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.484882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.484882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.484882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.603888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.603888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.603888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.484882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.484882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.485882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.484882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.604888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.604888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.485882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.604888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.604888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.485882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.485882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.604888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.605888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.486882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.486882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.486882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.486882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.605888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.605888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.486882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.605888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.605888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.487882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.487882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.605888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.606888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.487882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.487882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.487882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.606888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.606888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.607888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.488882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.488882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.488882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.607888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.607888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.608888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.489882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.488882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.488882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.608888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.608888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.609888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.489882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.489882 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.609888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.609888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.610888 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.489882 prunerr-1.0.0/src/prunerr/tests/responses/download-items/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.490882 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.490882 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.490882 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.490882 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.610888 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.610888 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.611888 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.490882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.493882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.491882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.491882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.492882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.491882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.611888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.611888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.491882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.611888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.611888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.492882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.492882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.612888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.612888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.492882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.492882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.493882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.492882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.612888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.612888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.493882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.612888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.613888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.493882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.493882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.613888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.613888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.493882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.494882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.494882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.613888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.614888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.614888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.615888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.615888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.495882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.498882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.495882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.495882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.496882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.496882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.615888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.615888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.496882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.616888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.616888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.496882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.496882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.616888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.616888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.497882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.497882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.498882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.497882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.616888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.617888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.497882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.617888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.617888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.498882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.498882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.617888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.617888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.498882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.498882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.498882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.618888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.618888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.618888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.499882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.502883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.499882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.499882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.500882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.499882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.618888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.619888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.500882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.619888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.619888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.500882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.500882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.619888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.619888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.501882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.501882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.502883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.501882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.620888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.620888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.501882 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.620888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.620888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.502883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.502883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.621888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.621888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.502883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.502883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.502883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.621888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.621888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.622888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.622888 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.623889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.503883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.506883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.503883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.503883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.504883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.504883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.623889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.623889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.504883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.623889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.623889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.504883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.504883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.624889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.624889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.505883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.505883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.506883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.505883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.624889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.624889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.505883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.624889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.625889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.506883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.506883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.625889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.625889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.506883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.506883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.506883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.625889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.626889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.626889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.507883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.510883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.507883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.507883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.508883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.507883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.626889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.626889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.508883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.627889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.627889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.508883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.508883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.627889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.627889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.509883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.509883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.509883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.509883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.627889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.628889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.509883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.628889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.628889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.510883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.510883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.628889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.628889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.510883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.510883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.510883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.629889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.629889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.630889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.630889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.630889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.631889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.511883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.514883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.511883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.511883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.512883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.512883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.631889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.631889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.512883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.631889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.631889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.512883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.512883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.632889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.632889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.513883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.513883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.514883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.513883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.632889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.632889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.514883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.632889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.633889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.514883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.514883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.633889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.633889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.514883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.514883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.515883 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.633889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.634889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.634889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.635889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.635889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.635889 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.515883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.518883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.516883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.516883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.517883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.516883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.636889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.636889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.516883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.636889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.636889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.517883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.517883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.636889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.637889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.517883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.517883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.518883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.517883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.637889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.637889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.518883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.637889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.637889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.518883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.518883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.638889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.638889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.519883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.519883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.519883 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.638889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.638889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.639889 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.519883 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.522884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.519883 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.519883 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.520883 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.520883 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.639889 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.639889 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.520883 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.639889 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.640890 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.520883 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.521884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.640890 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.640890 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.521884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.521884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.522884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.521884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.640890 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.641889 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.522884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.641889 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.641889 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.522884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.522884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.641889 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.641889 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.522884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.523884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.523884 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.642890 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.642890 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.642890 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.523884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.526884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.523884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.523884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.524884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.524884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.643890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.643890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.524884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.643890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.643890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.524884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.524884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.643890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.644890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.525884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.525884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.526884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.525884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.644890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.644890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.525884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.644890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.644890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.526884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.526884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.645890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.645890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.526884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.526884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.526884 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.645890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.646890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.646890 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.527884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.530884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.527884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.527884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.528884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.527884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.646890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.646890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.528884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.647890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.647890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.528884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.528884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.647890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.647890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.529884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.529884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.530884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.529884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.647890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.648890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.529884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.648890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.648890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.530884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.648890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.648890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.530884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.530884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.649890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.649890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.530884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.531884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.531884 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.649890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.649890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.650890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.650890 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.536884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.539884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.536884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.536884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.537884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.536884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.655890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.655890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.537884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.655890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.656890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.537884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.537884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.656890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.656890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.537884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.537884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.538884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.538884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.656890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.656890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.538884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.657890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.657890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.538884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.538884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.657890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.657890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.539884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.539884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.539884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.657890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.658890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.658890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.531884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.535884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.531884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.532884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.532884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.532884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.650890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.651890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.532884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.651890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.651890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.533884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.533884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.651890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.652890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.533884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.533884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.534884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.533884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.652890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.652890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.534884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.652890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.652890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.534884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.653890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.653890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.534884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.535884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.653890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.653890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.535884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.535884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.535884 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.653890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.654890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.654890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.655890 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.540884 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.543885 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.540884 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.540884 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.541885 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.540884 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.658890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.659890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.540884 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.659890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.659890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.541885 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.541885 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.659890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.659890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.541885 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.541885 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.542884 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.542884 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.660890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.660890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.542884 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.660890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.660890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.542884 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.542884 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.660890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.661890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.543885 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.543885 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.543885 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.661890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.661890 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.662891 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.544885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.547885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.544885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.544885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.545885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.544885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.662891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.662891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.544885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.663891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.663891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.545885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.545885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.663891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.663891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.545885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.545885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.547885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.546885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.663891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.664891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.546885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.546885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.664891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.664891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.546885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.664891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.664891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.547885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.547885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.664891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.665891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.547885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.547885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.547885 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.665891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.665891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.666891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.666891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.667891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.667891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.668891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.668891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.669891 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.549885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.553885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.549885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.549885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.550885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.549885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.669891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.669891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.550885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.669891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.669891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.550885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.550885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.669891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.670891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.551885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.551885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.552885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.551885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.670891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.670891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.552885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.552885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.671891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.671891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.552885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.671891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.671891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.551885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.670891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.671891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.553885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.553885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.672891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.672891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.553885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.553885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.553885 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.672891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.673891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.673891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16174 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.673891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.674891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.674891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.675891 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.554885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.557885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.554885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.554885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.555885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.555885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.675891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.675891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.555885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.675891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.676891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.555885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.555885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.676891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.676891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.556885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.556885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.557885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.556885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.676891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.677891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.557885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.677891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.677891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.557885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.557885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.677891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.677891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.557885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.558885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.558885 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.678891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.678891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.678891 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.558885 prunerr-1.0.0/src/prunerr/tests/responses/verify/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.561885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.558885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.558885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.559885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.559885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.679891 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.679891 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.559885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.679891 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.679891 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.559885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.559885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.680891 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.680891 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.560886 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.560886 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.561885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.560886 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.680891 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.680891 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.561885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.681892 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.681892 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.561885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.561885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.681892 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.681892 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.561885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.561885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.561885 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.681892 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.682891 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.682891 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.683892 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.683892 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.683892 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.684892 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4216 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_cli.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2979 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_daemon.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8809 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_downloadclient.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_downloaditem.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_free_space.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17228 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_move.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8042 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_operations.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10921 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_review.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_runner.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1522 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_servarr.py
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2022-12-13 09:25:38.000000 prunerr-1.0.0/src/prunerr/tests/test_verify.py
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      176 2022-12-13 09:28:56.000000 prunerr-1.0.0/src/prunerr/version.py
-drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2022-12-13 09:28:56.586887 prunerr-1.0.0/src/prunerr.egg-info/
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    12512 2022-12-13 09:28:56.000000 prunerr-1.0.0/src/prunerr.egg-info/PKG-INFO
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)    63786 2022-12-13 09:28:56.000000 prunerr-1.0.0/src/prunerr.egg-info/SOURCES.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2022-12-13 09:28:56.000000 prunerr-1.0.0/src/prunerr.egg-info/dependency_links.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2022-12-13 09:28:56.000000 prunerr-1.0.0/src/prunerr.egg-info/entry_points.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)      190 2022-12-13 09:28:56.000000 prunerr-1.0.0/src/prunerr.egg-info/requires.txt
--rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2022-12-13 09:28:56.000000 prunerr-1.0.0/src/prunerr.egg-info/top_level.txt
--rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1990 2022-12-13 09:25:38.000000 prunerr-1.0.0/tox.ini
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      543 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.dir-locals.el.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1503 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.dockerignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1226 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.env.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.118917 prunerr-1.1.0b24/.github/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/.github/workflows/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3938 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.github/workflows/build-test.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1503 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2764 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.gitlab-ci.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      779 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.pre-commit-config.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2448 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/.prospector.yaml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3897 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/CONTRIBUTING.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2430 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2753 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/Dockerfile.devel
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1081 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/LICENSE
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    57155 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3631 2023-04-11 23:08:29.000000 prunerr-1.1.0b24/NEWS.rst
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    14120 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/PKG-INFO
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13132 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/README.rst
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3999 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/TODO.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2792 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/bin/cz-check-bump
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      918 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/bin/entrypoint
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     1101 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/bin/get-base-version
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      321 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/bin/hadolint
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/build-host/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1994 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/build-host/Dockerfile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1404 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/build-host/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      746 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/build-host/README.rst
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/build-host/bin/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)     2041 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/build-host/bin/entrypoint
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      731 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/build-host/requirements-py310.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      674 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/build-host/requirements-py311.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      948 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/build-host/requirements-py37.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      729 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/build-host/requirements-py38.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      729 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/build-host/requirements-py39.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        4 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/build-host/requirements.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/dist/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/dist/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1397 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/docker-compose-servarr.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5034 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/docker-compose.override.yml
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4029 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/docker-compose.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/gitlab-runner/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       46 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/gitlab-runner/.gitignore
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/gitlab-runner/config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1323 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/gitlab-runner/config/config.toml.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/home/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       64 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/home/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      327 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/home/.pypirc.in
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2979 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/pyproject.toml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      578 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/build.txt.in
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/py310/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2414 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/py310/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5273 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py310/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py310/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/py311/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2414 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/py311/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5024 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py311/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      859 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py311/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/py37/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2645 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/py37/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     6115 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py37/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1398 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py37/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/py38/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/py38/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5591 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py38/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py38/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/requirements/py39/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2412 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/requirements/py39/build.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5578 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py39/devel.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1158 2023-04-11 23:08:30.000000 prunerr-1.1.0b24/requirements/py39/user.txt
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/s6/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/s6/etc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/s6/etc/s6-overlay/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/s6/etc/s6-overlay/s6-rc.d/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/s6/etc/s6-overlay/s6-rc.d/svc-transmission/
+-rwxrwxrwx   0 prunerr   (1001) prunerr   (1001)      243 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1764 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/setup.cfg
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/src/prunerr/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8431 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      201 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/__main__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    15438 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11377 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/downloaditem.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/src/prunerr/home/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9913 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/home/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/src/prunerr/newsfragments/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       91 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/newsfragments/.gitignore
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     7937 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    19064 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11415 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/servarr.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      911 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/Makefile
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    22019 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/__init__.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    67861 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/example-5s.mkv
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/daemon/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3204 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/daemon/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/download-client-only/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/download-client-only/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/download-clients/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2957 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/download-clients/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/download-items/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       90 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/download-items/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/empty/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/empty/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/empty/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/move-exec/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/move-exec/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       88 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/move-exec/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/home/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/home/review-edge-cases/.config/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      820 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:07:25.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1077 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/1-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     9537 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:07:25.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5451 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.122917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       67 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.150917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13662 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2862 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1943 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5081 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      126 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.126917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1484 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1467 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.154917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1495 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1498 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.130917 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2084 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       98 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-session-set/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.158918 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.134917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1459 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1362 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1461 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      210 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-set-location/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.162917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      143 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2102 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1470 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.138917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:07:25.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D%26blacklist%3Dtrue/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    16163 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5383 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      148 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/06-torrent-set/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     5495 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:07:25.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/1%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:07:25.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue/2%3Fapikey%3D/DELETE/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2044 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    27061 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      151 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-remove/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       61 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2085 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4802 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1086 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4602 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1091 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      825 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.166917 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2087 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    10807 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3738 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      131 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3586 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1142 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      769 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/request-headers.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.142917 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       53 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2086 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1555 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      123 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-torrent-verify/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1505 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.170918 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)      122 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/request.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)       45 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-start/response.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)        3 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/request-headers.json
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     4730 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_cli.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     2906 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_daemon.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8822 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_downloadclient.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3745 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_downloaditem.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    11350 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_free_space.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    17208 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_move.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     8074 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_operations.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)    13110 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_review.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1468 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_runner.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1571 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_servarr.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1204 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/tests/test_verify.py
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     1374 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/src/prunerr/utils.py
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      163 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr/version.py
+drwxr-xr-x   0 prunerr   (1001) prunerr   (1001)        0 2023-04-11 23:08:35.146917 prunerr-1.1.0b24/src/prunerr.egg-info/
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    14120 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/PKG-INFO
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)    64631 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/SOURCES.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        1 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/dependency_links.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)       41 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/entry_points.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)      327 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/requires.txt
+-rw-r--r--   0 prunerr   (1001) prunerr   (1001)        8 2023-04-11 23:08:35.000000 prunerr-1.1.0b24/src/prunerr.egg-info/top_level.txt
+-rw-rw-rw-   0 prunerr   (1001) prunerr   (1001)     3321 2023-04-11 21:31:43.000000 prunerr-1.1.0b24/tox.ini
```

### Comparing `prunerr-1.0.0/.dockerignore` & `prunerr-1.1.0b24/.dockerignore`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,22 @@
 **/.so
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
-dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
 var/
-var-*/
 *.egg-info
 **/*.egg-info
 .installed.cfg
 *.egg
 **/.egg
 /src/*/version.py
 
@@ -50,15 +48,14 @@
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox
 **/.tox
-.tox-*
 .coverage
 .coverage.*
 coverage.*
 .cache
 **/.cache
 nosetests.xml
 pytest-junit.xml
```

### Comparing `prunerr-1.0.0/.env.in` & `prunerr-1.1.0b24/.env.in`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+# Make non-default `./docker-compose*.yml` files the default
+# https://pscheit.medium.com/docker-compose-advanced-configuration-541356d121de#9aa6
+COMPOSE_PATH_SEPARATOR=:
+COMPOSE_FILE=./docker-compose.yml:./docker-compose-servarr.yml:./docker-compose.override.yml
+
 # Capture local values specific to this checkout
+TZ=${TZ}
 PUID=${PUID}
 PGID=${PGID}
 # Absolute path of the git repo checkout, useful where relative paths can't be used
-CHECKOUT_DIR=${PWD}
-
+CHECKOUT_DIR=${CHECKOUT_DIR}
+# Build host variables
+DOCKER_GID=${DOCKER_GID}
 # Release variables
-DOCKER_USER=merpatterson
+DOCKER_USER=${DOCKER_USER}
 # Best to create and use a token.  Note that the token must have the `admin`/"Read,
 # Write, Delete" scope, aka "ACCESS PERMISSIONS":
 # https://hub.docker.com/settings/security?generateToken=true
 DOCKER_PASS=${DOCKER_PASS}
+# Project host credentials used here and in CI/CD to support local testing/debugging:
+CI_REGISTRY_PASSWORD=${CI_REGISTRY_PASSWORD}
+PROJECT_GITHUB_PAT=${PROJECT_GITHUB_PAT}
 
 TRANSMISSION_PASS=${TRANSMISSION_PASS}
 # The volume on which Transmission's `download-dir` is stored
-DOWNLOAD_VOLUME=/media/Library/
+DOWNLOAD_VOLUME=${DOWNLOAD_VOLUME}
 # The amount of free disk space below which to stop the container: 1GB
-CRITICAL_AVAIL=1048576
+CRITICAL_AVAIL=${CRITICAL_AVAIL}
 
 SONARR_API_KEY=
 RADARR_API_KEY=
```

### Comparing `prunerr-1.0.0/.github/workflows/ci-cd.yml` & `prunerr-1.1.0b24/.github/workflows/build-test.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,118 +1,115 @@
-name: "CI/CD"
+name: "Build and Test"
 
 on:
-  # Only run when branches are pushed, and not when tags are pushed, to allow manual
-  # creation of tags to manually control bumped versions:
+  # Only run on branches, not tags:
   # https://github.com/orgs/community/discussions/25615#discussioncomment-3397691
   push:
     branches:
       - "**"
     tags:
       - "!**"
+      # Also run for open pull requests, including when pushed to:
+  pull_request: {}
 
 jobs:
 
-  ci-cd:
+  build-test:
     runs-on: "ubuntu-latest"
+    container:
+      image: "ghcr.io/rpatterson/prunerr:build-host"
+      env:
+        PUID: "1001"
+        PGID: "123"
+        CHECKOUT_DIR: "${{ github.workspace }}"
+        # Requires the secrets to be added to GitHub either through the web UI or the
+        # GitHub CLI tool:
+        # https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository
+        GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
+        GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
+        DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
+        # Enable the GitHub CLI
+        PROJECT_GITHUB_PAT: "${{ secrets.PROJECT_GITHUB_PAT }}"
+        # Tell the `./Makefile` about GitHub specific environment details:
+        CI_IS_FORK: >-
+          ${{
+            (
+              (
+                (github.repository_owner != 'rpatterson')
+                || (github.event.pull_request.head.repo.owner.login != 'rpatterson')
+              ) && 'true'
+            ) || 'false'
+          }}
+    permissions:
+      packages: "write"
+      checks: "write"
     strategy:
       matrix:
-        python-version: ["3.10"]
+        PYTHON_MINORS:
+          - "3.11"
+          - "3.10"
+          - "3.9"
+          - "3.8"
+          - "3.7"
+    name: "build-test (python${{ matrix.PYTHON_MINORS }})"
     steps:
 
-      # Global set up
-
+      # Shared/common set up:
       - name: "Checkout source from VCS"
         uses: "actions/checkout@master"
-      # https://github.com/actions/checkout/issues/701#issuecomment-1139627817
-      - name: "Fetch versions from VCS"
-        run: "git fetch --tags origin"
-
-      - name: "Add user installs to PATH"
-        run: |
-          echo "$HOME/.local/bin" >> $GITHUB_PATH
-
-      # Cache build artifacts to speed up CI runs
-
-      - name: "Cache tox virtual environments"
-        if: "github.ref != 'refs/heads/master'"
-        uses: "actions/cache@master"
-        env:
-          # Increment to force clearing the cache
-          cache-name: "tox-v1"
-        with:
-          path: |
-            ~/.local
-            ./.tox
-            ./.tox-*
-            ./var/log
-          # Never get a cache hit to force always caching any upgraded dependencies
-          # Use hashFiles to force venv recreation when dependencies change
-          key: >-
-            ${{ env.cache-name }}-${{ runner.os }}-${{ matrix.python-version }}-${{ hashFiles('pyproject.*') }}-${{ hashFiles('setup.*') }}-${{ hashFiles('tox.ini') }}-${{ github.sha }}
-          # Always re-use the cache and then upgrade
-          restore-keys: >-
-            ${{ env.cache-name }}-${{ runner.os }}-${{ matrix.python-version }}-${{ hashFiles('pyproject.*') }}-${{ hashFiles('setup.*') }}-${{ hashFiles('requirements*.txt') }}-${{ hashFiles('tox.ini') }}-
-
-      # Delegate the rest to the `./Makefile` to keep as much portable between CI
-      # platforms
-
-      - name: "Build the container image in which to run the tests"
-        env:
-          GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
-          GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
-          DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
-        run: "make -e build-bump build-docker"
+      # TODO: Debug stale venv issues and restore cache once fixed
+      - name: "Change checkout owner"
+        # https://stackoverflow.com/a/58474340/624787
+        run: >-
+          chown -R ${PUID}:${PGID} ./ &&
+          git config --global --add safe.directory
+          /__w/${{ github.event.repository.name }}/${{ github.event.repository.name }}
+
+      # Delegate steps agnostic of the CI/CD platform to the `./Makefile`:
+      - name: "Build image and run tests and checks in a container"
+        run: >-
+          entrypoint make -e PYTHON_MINORS=${{ matrix.PYTHON_MINORS }}
+          test-push build-docker-${{ matrix.PYTHON_MINORS }}
+          test-docker-${{ matrix.PYTHON_MINORS }} test-clean
 
-      - name: "Run the tests and code checks inside the built container"
-        run: "make test-docker"
-
-      # Upload build artifacts
+      # Upload build artifacts:
       # https://github.com/actions/upload-artifact#usage
-
       - name: "Archive test suite reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "test-suite-reports"
           path: |
-            ./pytest*
+            ./build/*/pytest*
       # https://github.com/marketplace/actions/test-reporter#example
       - name: "Publish test suite report"
         uses: "dorny/test-reporter@main"
-        if: "success() || failure()"    # run this step even if previous step failed
+        # run this step even if previous step failed
+        if: >-
+          (success() || failure())
+          && (
+            (! github.event.pull_request)
+            || ! (
+              (github.repository_owner == 'rpatterson')
+              && (github.event.pull_request.head.repo.owner.login != 'rpatterson')
+            )
+          )
         with:
-          name: "PyTest Test Suite"
-          path: |
-            ./pytest-junit.xml
+          name: "PyTest Test Suite (python${{ matrix.PYTHON_MINORS }})"
+          path: >-
+            ./build/*/pytest-junit.xml,
+            ./build/*/prospector-xunit.xml
           reporter: "java-junit"
-
       - name: "Archive code coverage reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "code-coverage-reports"
           path: |
-            ./coverage*
-            ./htmlcov
-
+            ./build/*/.coverage*
+            ./build/*/coverage*
+            ./build/*/htmlcov*
       - name: "Archive linter reports"
         uses: "actions/upload-artifact@master"
         with:
           name: "linter-reports"
           path: |
-            ./pylint*
-
-      # Release and publish
-
-      - name: "Bump version and publish release artifacts if on `master`/`develop`"
-        env:
-          CODECOV_TOKEN: "${{ secrets.CODECOV_TOKEN }}"
-          # Enable the GitHub CLI
-          GITHUB_TOKEN: "${{ secrets.GITHUB_TOKEN }}"
-          # Requires the secrets to be added to GitHub either through the web UI or the
-          # GitHub CLI tool:
-          # https://docs.github.com/en/actions/security-guides/encrypted-secrets#creating-encrypted-secrets-for-a-repository
-          GPG_PASSPHRASE: "${{ secrets.GPG_PASSPHRASE }}"
-          GPG_SIGNING_PRIVATE_KEY: "${{ secrets.GPG_SIGNING_PRIVATE_KEY }}"
-          PYPI_PASSWORD: "${{ secrets.PYPI_PASSWORD }}"
-          TEST_PYPI_PASSWORD: "${{ secrets.TEST_PYPI_PASSWORD }}"
-          DOCKER_PASS: "${{ secrets.DOCKER_PASS }}"
-        run: "make -e release"
+            ./build/*/prospector*
+            ./build/*/pylint*
```

### Comparing `prunerr-1.0.0/.gitignore` & `prunerr-1.1.0b24/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,22 @@
 **/.so
 
 # Distribution / packaging
 .Python
 env/
 build/
 develop-eggs/
-dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
 var/
-var-*/
 *.egg-info
 **/*.egg-info
 .installed.cfg
 *.egg
 **/.egg
 /src/*/version.py
 
@@ -50,15 +48,14 @@
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
 .tox
 **/.tox
-.tox-*
 .coverage
 .coverage.*
 coverage.*
 .cache
 **/.cache
 nosetests.xml
 pytest-junit.xml
```

### Comparing `prunerr-1.0.0/CONTRIBUTING.rst` & `prunerr-1.1.0b24/CONTRIBUTING.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-************
+########################################################################################
 CONTRIBUTING
-************
+########################################################################################
 
 Development requires fairly standard development tools, but ``git`` and ``make`` to
 bootstrap the local development environment.  Once installed, clone the repository::
 
   $ git clone "https://gitlab.com/rpatterson/prunerr"
 
 Then hand the rest over to the `Makefile`_ to install the VCS hooks the rest of the set
@@ -41,36 +41,41 @@
 
   $ make test-debug
 
 The ``$ make test`` target also runs the ``$ make format`` target to format code
 according to this project's guidelines and rules.
 
 Once work is finished and all the tests are passing locally, open a PR and push your
-changes there.  Address any issues revealed by any failed CI/CD jobs for your PR
-branch/fork.  Once all CI/CD checks are green, project maintainers can merge your work
-into the ``develop`` branch where CI/CD will publish a pre-release for your changes.
-When the project maintainers think it's time to make a final release with all the
-outstanding work on ``develop``, they can merge ``develop`` into ``master`` and CI/CD
-will then publish a final release including container images and PyPI packages.  Project
-maintainers may test the release process locally using the `Makefile`_::
+changes there.  Address any issues revealed by any failed CI/CD jobs for your PR branch.
+Once all CI/CD checks are green, project maintainers can merge your work into the
+``develop`` branch where CI/CD will publish a pre-release for your changes including
+container images and PyPI packages.  When the project maintainers think it's time to
+make a final release with all the outstanding work on ``develop``, they can merge
+``develop`` into ``master`` and CI/CD will then publish a final release::
 
-  $ make build-bump test-docker release
+  $ make release
 
 The versions for this project's dependencies and development tools are frozen/fixed for
-reproducibility in ``./requirements*.txt``. The `Makefile`_ will update those versions
-as the dependencies change in ``./setup.cfg`` and ``./requirements-build.txt.in``.  Note
+reproducibility in ``./requirements/**.txt``. The `Makefile`_ will update those versions
+as the dependencies change in ``./setup.cfg`` and ``./requirements/build.txt.in``.  Note
 that this means other versions may be updated as the published versions for dependencies
 are updated on remote indexes/registries.  Maintainers can also update all dependencies
 to the latest versions::
 
   $ make upgrade
 
 See also `the ./TODO.rst file`_ which lists known bugs and desirable features for which
 contributions are most welcome.
 
+If changes to development processes, such as build or release processes, are required,
+they should be captured in the `Makefile`_.  Similarly, if a development task is
+important enough to include in the documentation, then it's important enough to capture
+in executable form in the `Makefile`_.  See the philosophy commentary at the bottom of
+the `Makefile`_ for guidance on making contributions there.
+
 
 .. _`Python's post-mortem debugger`:
    https://docs.python.org/3/library/pdb.html#pdb.post_mortem
 
 .. _`towncrier`: https://towncrier.readthedocs.io/en/stable/#philosophy
 .. _`news fragment`: https://towncrier.readthedocs.io/en/stable/quickstart.html#creating-news-fragments
```

### Comparing `prunerr-1.0.0/Dockerfile` & `prunerr-1.1.0b24/build-host/Dockerfile`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,51 @@
-## Container image for use by end users
+## Container image in which to build, test, and release the project
 
-# Stay as close to a vanilla Python environment as possible
-FROM python:3
+# I *want* something to break to let me know if something changes in the latest version
+# of the base image changes something:
+# hadolint ignore=DL3007
+FROM docker:latest
+
+# Install the minimum OS packages needed to use the `./Makefile`.  Also install any OS
+# packages the `./Makefile` might install to optimize build times.
+# hadolint ignore=DL3018
+RUN \
+    apk add --no-cache \
+    "make" \
+    "bash" \
+    "su-exec" \
+    "git" \
+    "gettext" \
+    "py3-pip" \
+    "gnupg" \
+    "curl" \
+    "tar" \
+    "github-cli" \
+    "apg" \
+    && rm -rf /var/cache/apk/*
+
+# Find the same home directory even when run as another user, e.g. `root`.
+ENV HOME="/home/runner"
+# Add user installs to PATH
+ENV PATH="${HOME}/.local/bin:${PATH}"
+
+COPY [ "./requirements-py310.txt", "${HOME}/.local/lib/" ]
+RUN mkdir -pv "${HOME}/.local/var/log/" && \
+    pip install --no-cache-dir --user -r "${HOME}/.local/lib/requirements-py310.txt" \
+    >"${HOME}/.local/var/log/prunerr-host-install.log"
 
-ARG VERSION=
-
-# Put the `ENTRYPOINT` on the `$PATH`
-RUN apt-get update && apt-get install -y gosu && rm -rf /var/lib/apt/lists/*
 COPY [ "./bin/entrypoint", "/usr/local/bin/entrypoint" ]
-
-WORKDIR "/usr/local/src/prunerr/"
-# Install dependencies with fixed versions in a separate layer to optimize build times
-# because this step takes the most time and changes the least frequently.
-COPY [ "./requirements.txt", "./" ]
-RUN pip install --no-cache-dir -r "./requirements.txt"
-# Install this package in the most common/standard Python way while still being able to
-# build the image locally.
-RUN --mount=source=./,target=./,rw,type=bind pip install --no-cache-dir "./"
-
-# Find the same configuration file even when run as another user, e.g. `root`.
-ENV HOME="/home/prunerr/"
-WORKDIR "/home/prunerr/"
-ENTRYPOINT [ "entrypoint" ]
-CMD [ "prunerr", "daemon" ]
+ENTRYPOINT [ "docker-entrypoint.sh", "entrypoint" ]
+CMD [ "make", "-e", "build-docker" ]
 
 # https://github.com/opencontainers/image-spec/blob/main/annotations.md#pre-defined-annotation-keys
 LABEL org.opencontainers.image.url="https://gitlab.com/rpatterson/prunerr"
 LABEL org.opencontainers.image.documentation="https://gitlab.com/rpatterson/prunerr"
 LABEL org.opencontainers.image.source="https://gitlab.com/rpatterson/prunerr"
-LABEL org.opencontainers.image.title="prunerr"
-LABEL org.opencontainers.image.description="Remove Servarr download client items to preserve disk space according to rules."
+LABEL org.opencontainers.image.title="Prunerr Build Host"
+LABEL org.opencontainers.image.description="The host in which Prunerr is built"
 LABEL org.opencontainers.image.licenses="MIT"
 LABEL org.opencontainers.image.authors="Ross Patterson <me@rpatterson.net>"
 LABEL org.opencontainers.image.vendor="rpatterson.net"
-LABEL org.opencontainers.image.base.name="docker.io/library/python:3"
+LABEL org.opencontainers.image.base.name="docker.io/library/docker:latest"
 # Build-time `LABEL`s
-LABEL org.opencontainers.image.version=${VERSION}
+LABEL org.opencontainers.image.version=0.0.1
```

### Comparing `prunerr-1.0.0/LICENSE` & `prunerr-1.1.0b24/LICENSE`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/PKG-INFO` & `prunerr-1.1.0b24/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,12 @@
-Metadata-Version: 2.1
-Name: prunerr
-Version: 1.0.0
-Summary: Perma-seed Servarr media libraries
-Home-page: https://gitlab.com/rpatterson/prunerr
-Author: Ross Patterson
-Author-email: me@rpatterson.net
-License: MIT
-Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: BSD
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Communications :: File Sharing
-Classifier: Topic :: Internet
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: devel
-License-File: LICENSE
-
-##################################
+########################################################################################
 Prunerr
-##################################
+########################################################################################
 Perma-seed Servarr media libraries
-**********************************
+****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/prunerr.svg?logo=pypi&label=PyPI&logoColor=gold
           :alt: PyPI latest release version
           :target: https://pypi.org/project/prunerr/
@@ -54,37 +32,45 @@
        .. figure:: https://img.shields.io/gitlab/stars/rpatterson/prunerr?gitlab_url=https%3A%2F%2Fgitlab.com&logo=gitlab
 	  :alt: GitLab repo stars
 	  :target: https://gitlab.com/rpatterson/prunerr
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/prunerr?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/prunerr/releases
-       .. figure:: https://github.com/rpatterson/prunerr/actions/workflows/ci-cd.yml/badge.svg
+       .. figure:: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
-          :target: https://github.com/rpatterson/prunerr/
-       .. figure:: https://codecov.io/github/rpatterson/prunerr/branch/master/graph/badge.svg?token=GNKVQ8VYOU 
+          :target: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml
+       .. figure:: https://codecov.io/github/rpatterson/prunerr/branch/master/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
 	  :target: https://codecov.io/github/rpatterson/prunerr
        .. figure:: https://img.shields.io/github/stars/rpatterson/prunerr?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/prunerr/
 
-     - .. figure:: https://img.shields.io/docker/v/merpatterson/prunerr?sort=semver&logo=docker
+     - .. figure:: https://img.shields.io/docker/v/merpatterson/prunerr/master?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/prunerr?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/stars/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub stars
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub image size (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
 
+TL;DR: Perma-seeding of whole Servarr libraries optimized for per-tracker ratio.
+
+- Delete torrents/items only as disk space gets low.
+- Don't delete currently imported items.  IOW, only delete upgraded items.
+- Don't delete private items that haven't met seeding requirements.
+- Delete public items first
+- Delete private items in an order to maximize tracker ratio and/or bonuses.
+- And more...
 
 *******
 Summary
 *******
 
 Seed Servarr download client torrents/items as long as possible only deleting them as
 necessary as disk space gets low, hence the name based on "to prune".  Which download
@@ -115,29 +101,31 @@
 operations to the download items in each of those download clients.  It can also be run
 independently of any Servarr instances to optimize seeding for download items added by
 other means, e.g. `FlexGet`_.
 
 See the `Usage`_ section below for full details.
 
 
-************
+****************************************************************************************
 Installation
-************
+****************************************************************************************
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ sudo pip3 install prunerr
 
+Optional shell tab completion is available via `argcomplete`_.
+
 Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
 details.
 
 
-*****
+****************************************************************************************
 Usage
-*****
+****************************************************************************************
 
 Start by writing your ``~/.config/prunerr.yml`` configuration file.  See the comments in
 `the example configuration`_ for details.
 
 Once configured, you may run individual sub-commands once, run all operations once as
 configured using the ``$ prunerr exec`` sub-command, or run all operations in a polling
 loop using the ``$ prunerr daemon`` sub-command.  See the `Order of Operations`_ section
@@ -222,29 +210,29 @@
    orphans.
 
    For the other groups delete items in the order determined by the configured
    ``indexers/priorities`` indexer order then by the configured operations for that
    item's indexer.
 
 
-************
+****************************************************************************************
 CONTRIBUTING
-************
+****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
 development.
 
 
-**********
+****************************************************************************************
 Motivation
-**********
+****************************************************************************************
 
 I didn't like the available options I could find at the time for maximizing seeding from
 a lovingly managed media library.  Deleting by a ratio threshold doesn't make sense to
 me because that can delete items when there's plenty of disk space.  Also the ratio
 threshold is a reverse indicator for items from private indexers vs items from public
 indexers.  Items from private indexers with high ratios should be kept around as long as
 possible to build user total ratio whereas items from public indexers with low ratios
@@ -262,14 +250,15 @@
 .. _`Servarr`: https://wiki.servarr.com
 .. _`Radarr`: https://wiki.servarr.com/en/radarr
 .. _`Sonarr`: https://wiki.servarr.com/en/sonarr
 .. _`download clients`: https://wiki.servarr.com/radarr/settings#download-clients
 .. _`FlexGet`: https://flexget.com/
 
 .. _pip: https://pip.pypa.io/en/stable/installation/
+.. _argcomplete: https://kislyuk.github.io/argcomplete/#installation
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/prunerr
 .. _`the example ./docker-compose.yml file`: https://gitlab.com/rpatterson/prunerr/blob/master/docker-compose.yml
 
 .. _`the example configuration`:
    https://gitlab.com/rpatterson/prunerr/blob/master/src/prunerr/home/.config/prunerr.yml
```

### Comparing `prunerr-1.0.0/README.rst` & `prunerr-1.1.0b24/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,39 @@
-##################################
+Metadata-Version: 2.1
+Name: prunerr
+Version: 1.1.0b24
+Summary: Perma-seed Servarr media libraries
+Home-page: https://gitlab.com/rpatterson/prunerr
+Author: Ross Patterson
+Author-email: me@rpatterson.net
+License: MIT
+Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: BSD
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Communications :: File Sharing
+Classifier: Topic :: Internet
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: devel
+License-File: LICENSE
+
+########################################################################################
 Prunerr
-##################################
+########################################################################################
 Perma-seed Servarr media libraries
-**********************************
+****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/prunerr.svg?logo=pypi&label=PyPI&logoColor=gold
           :alt: PyPI latest release version
           :target: https://pypi.org/project/prunerr/
@@ -32,37 +59,45 @@
        .. figure:: https://img.shields.io/gitlab/stars/rpatterson/prunerr?gitlab_url=https%3A%2F%2Fgitlab.com&logo=gitlab
 	  :alt: GitLab repo stars
 	  :target: https://gitlab.com/rpatterson/prunerr
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/prunerr?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/prunerr/releases
-       .. figure:: https://github.com/rpatterson/prunerr/actions/workflows/ci-cd.yml/badge.svg
+       .. figure:: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
-          :target: https://github.com/rpatterson/prunerr/
-       .. figure:: https://codecov.io/github/rpatterson/prunerr/branch/master/graph/badge.svg?token=GNKVQ8VYOU 
+          :target: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml
+       .. figure:: https://codecov.io/github/rpatterson/prunerr/branch/master/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
 	  :target: https://codecov.io/github/rpatterson/prunerr
        .. figure:: https://img.shields.io/github/stars/rpatterson/prunerr?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/prunerr/
 
-     - .. figure:: https://img.shields.io/docker/v/merpatterson/prunerr?sort=semver&logo=docker
+     - .. figure:: https://img.shields.io/docker/v/merpatterson/prunerr/master?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/prunerr?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/stars/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub stars
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub image size (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
 
+TL;DR: Perma-seeding of whole Servarr libraries optimized for per-tracker ratio.
+
+- Delete torrents/items only as disk space gets low.
+- Don't delete currently imported items.  IOW, only delete upgraded items.
+- Don't delete private items that haven't met seeding requirements.
+- Delete public items first
+- Delete private items in an order to maximize tracker ratio and/or bonuses.
+- And more...
 
 *******
 Summary
 *******
 
 Seed Servarr download client torrents/items as long as possible only deleting them as
 necessary as disk space gets low, hence the name based on "to prune".  Which download
@@ -93,29 +128,31 @@
 operations to the download items in each of those download clients.  It can also be run
 independently of any Servarr instances to optimize seeding for download items added by
 other means, e.g. `FlexGet`_.
 
 See the `Usage`_ section below for full details.
 
 
-************
+****************************************************************************************
 Installation
-************
+****************************************************************************************
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ sudo pip3 install prunerr
 
+Optional shell tab completion is available via `argcomplete`_.
+
 Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
 details.
 
 
-*****
+****************************************************************************************
 Usage
-*****
+****************************************************************************************
 
 Start by writing your ``~/.config/prunerr.yml`` configuration file.  See the comments in
 `the example configuration`_ for details.
 
 Once configured, you may run individual sub-commands once, run all operations once as
 configured using the ``$ prunerr exec`` sub-command, or run all operations in a polling
 loop using the ``$ prunerr daemon`` sub-command.  See the `Order of Operations`_ section
@@ -200,29 +237,29 @@
    orphans.
 
    For the other groups delete items in the order determined by the configured
    ``indexers/priorities`` indexer order then by the configured operations for that
    item's indexer.
 
 
-************
+****************************************************************************************
 CONTRIBUTING
-************
+****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
 development.
 
 
-**********
+****************************************************************************************
 Motivation
-**********
+****************************************************************************************
 
 I didn't like the available options I could find at the time for maximizing seeding from
 a lovingly managed media library.  Deleting by a ratio threshold doesn't make sense to
 me because that can delete items when there's plenty of disk space.  Also the ratio
 threshold is a reverse indicator for items from private indexers vs items from public
 indexers.  Items from private indexers with high ratios should be kept around as long as
 possible to build user total ratio whereas items from public indexers with low ratios
@@ -240,14 +277,15 @@
 .. _`Servarr`: https://wiki.servarr.com
 .. _`Radarr`: https://wiki.servarr.com/en/radarr
 .. _`Sonarr`: https://wiki.servarr.com/en/sonarr
 .. _`download clients`: https://wiki.servarr.com/radarr/settings#download-clients
 .. _`FlexGet`: https://flexget.com/
 
 .. _pip: https://pip.pypa.io/en/stable/installation/
+.. _argcomplete: https://kislyuk.github.io/argcomplete/#installation
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/prunerr
 .. _`the example ./docker-compose.yml file`: https://gitlab.com/rpatterson/prunerr/blob/master/docker-compose.yml
 
 .. _`the example configuration`:
    https://gitlab.com/rpatterson/prunerr/blob/master/src/prunerr/home/.config/prunerr.yml
```

### Comparing `prunerr-1.0.0/TODO.rst` & `prunerr-1.1.0b24/TODO.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-###########################################################################
+########################################################################################
 Seeking Contributions
-###########################################################################
+########################################################################################
 
 The following are known issues with Prunerr or features that are particularly desirable
 to implement in Prunerr.  IOW, contributions are particularly welcome for the following:
 
-********
+
+****************************************************************************************
 Required
-********
+****************************************************************************************
+
 
-*************
+****************************************************************************************
 High Priority
-*************
+****************************************************************************************
 
 #. Operations reference, perhaps done dynamically from the CLI help using operation
    method docstrings.
 
 #. Any documentation improvements!
 
    Documentation benefits perhaps most from the attention of fresh eyes.  If you find
@@ -28,36 +30,35 @@
    episodes from another.  Maybe extend the existing operations support to write CSV
    report files?
 
 #. Send a notification when no download item can be deleted and downloading is paused:
 
    Perhaps we can use the Servarr "Connect" API?
 
-************
+****************************************************************************************
 Nice to Have
-************
+****************************************************************************************
 
 #. Improve configure-ability, particularly the various download client paths:
 
-   Currently, Prunerr strongly depends on using the ``.../incomplete/``,
-   ``.../downloads/``, ``.../imported/``,  and ``.../deleted/`` paths.  In theory, these
-   paths are all configurable, but that's untested.
+   Currently, Prunerr hard-codes the ``.../incomplete/``, ``.../downloads/``, and
+   ``.../seeding/`` paths.
 
 #. Unit tests
 
    The current tests are probably most accurately described as integration tests.  Any
    tests that cover discreet units are welcome.
 
 #. Resurrect the ``rename`` command.  See the ``feat(rename): Remove series title rename
    support`` commit that removed it.
 
 #. Support other download client software, not just `Transmission`_:
 
    This would almost certainly require discussion before implementing, because how this
-   is down will be important for maintainability.  So open an issue and start the
+   is done would be important for maintainability.  So open an issue and start the
    discussion before you start implementing lest your work go to waste.  Currently,
    Prunerr is way to tightly coupled with Transmission and the `Python RPC client
    library`_ used to interface with it.  I suspect the best way to abstract it will be
    to use that client library as a de facto abstract interface and then wrap other
    client libraries to fulfill that interface, but that's one of the things to discuss.
 
    It's also worth noting that the reason Transmission is the first supported download
@@ -69,14 +70,12 @@
 #. ``$ git grep -i -e todo``:
 
    The above are the most important improvements that Prunerr definitely needs.  See ``#
    TODO: ...`` comments throughout the source for other smaller, potential improvements.
 
 #. Fix items with character mapping (Samba) treated as orphans.
 
-#. Items deleted from download client outside of Prunerr being re-added.
-
 
 .. _`Transmission`: https://transmissionbt.com/
 .. _`Python RPC client library`: https://transmission-rpc.readthedocs.io/en/v3.2.6/
 .. _`it seems to be the best`: https://www.reddit.com/r/DataHoarder/comments/3ve1oz/torrent_client_that_can_handle_lots_of_torrents/
 .. _`managing large numbers of torrents efficiently`: https://www.reddit.com/r/trackers/comments/3hiey5/does_anyone_here_seed_large_amounts_10000_of/
```

### Comparing `prunerr-1.0.0/bin/entrypoint` & `prunerr-1.1.0b24/bin/entrypoint`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 #!/bin/bash
 #
 # Perform any required volatile run-time initialization
 
 set -eu -o pipefail
 shopt -s inherit_errexit
-if [ ! -z "${DEBUG:=}" ]
+if [ "${DEBUG:=false}" = "true" ]
 then
     # Echo commands for easier debugging
-    PS4='$0:$LINENO+'
     set -x
+    PS4='$0:$LINENO+'
 fi
 
 
 main() {
-    if [ ! -z "${PUID}" ]
+    if [ -n "${PUID:-}" ]
     then
 	if (( $(id -u) != 0 ))
 	then
 	    set +x
 	    echo "ERROR: Can't create a user when not run as root" 1>&2
 	    false
 	fi
-	if ! id ${PUID}
+	if ! id "${PUID}" >"/dev/null" 2>&1
 	then
 	    # Add a user to the `passwd` DB so that the `~prunerr/`
 	    # HOME directory can be looked up.
 	    adduser --uid "${PUID}" --disabled-password \
-		    --gecos "Prunerr,,," "prunerr" 1>&2
+		    --gecos "Prunerr,,," "prunerr" >"/dev/null"
 	fi
 	# Fix the TTY ownership if the session is interactive
 	if tty_dev=$(tty)
 	then
-	    chown -c "${PUID}" "${tty_dev}"
+	    chown "${PUID}" "${tty_dev}"
 	fi
 	# Delegate the rest to the `CMD`
 	exec gosu "${PUID}:${PGID:-${PUID}}" "${@}"
     fi
 
     # Delegate the rest to the `CMD`
     exec "$@"
 }
 
-
 main "$@"
```

### Comparing `prunerr-1.0.0/docker-compose.yml` & `prunerr-1.1.0b24/docker-compose.yml`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # running Prunerr in containers.
 version: "3.8"
 
 services:
 
   transmission:
     image: "linuxserver/transmission"
+    container_name: "transmission"
     # command:
     #   # From `# pgrep -fla transmission`:
     #   # `/usr/bin/transmission-daemon -g /config -c /watch -f`
     #   - "transmission-daemon"
     #   - "-g"
     #   - "/config"
     #   - "-c"
@@ -26,78 +27,67 @@
     volumes:
       # Exit the container if the core `s6-overlay` service fails.
       # Replace with the correct path for your `$ docker compose ...` project.
       # - "./s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish:/etc/s6-overlay/s6-rc.d/svc-transmission/finish"
       # Intended for use in the image
       - "./transmission/config/:/config/"
       # The volume on which Transmission's `download-dir` is stored
-      - "${DOWNLOAD_VOLUME}:${DOWNLOAD_VOLUME}"
+      - type: bind
+        source: "${DOWNLOAD_VOLUME:-/media/Library/}"
+        target: "${DOWNLOAD_VOLUME:-/media/Library/}"
+        bind:
+          propagation: "shared"
     # Transmission seems to be very poorly behaved when disk space is exhausted: items
     # become corrupted, items lose track of their data/files, etc..  Guard against that,
     # for example if Prunerr stops running for any reason, by shutting it down before
     # disk space is exhausted.  Abuse the `HEALTHCHECK` to exit PID 1 with 0 status code
     # before that happens.  The `on-failure` restart policy ensures that `# dockerd`
     # won't restart the container again.
     restart: "on-failure"
     healthcheck:
+      # If the `transmission` service uses `network_mode: "service:..."`, such as a VPN,
+      # then it may become inaccessible on any IP other than `localhost` when the
+      # service whose network it uses is restarted.  As such, if the `transmission`
+      # service should be accessible from it's IP on the LAN set the `LAN_IP=...` in the
+      # `./.env` so that the `HEALTHCHECK` fails and the container is restart when that
+      # happens.
       test: >-
-        test "$(df --output="avail" "${DOWNLOAD_VOLUME}" | tail -n +2)"
-        -gt "${CRITICAL_AVAIL}" || /sbin/shutdown &&
-        curl -LI -u "${TRANSMISSION_USER:-transmission}:${TRANSMISSION_PASS}"
-        "http://localhost:9091/transmission/rpc/" |
+        test "$(df --output="avail" "${DOWNLOAD_DIR:-/media/Library/}" | tail -n +2)"
+        -gt "${CRITICAL_AVAIL:-1048576}" || /sbin/shutdown &&
+        curl -LI -X GET -u "${TRANSMISSION_USER:-transmission}:${TRANSMISSION_PASS}"
+        "http://${LAN_IP:-localhost}:9091/transmission/rpc/" |
         grep '^X-Transmission-Session-Id: '
     labels:
       traefik.enable: true
       # Un comment and set `TRANSMISSION_HOST` to proxy via Traefik
       # traefik.http.routers.transmission.rule: "Host(`${TRANSMISSION_HOST}`)"
       traefik.http.services.transmission.loadbalancer.server.port: 9091
       traefik.http.routers.transmission.entrypoints: "websecure"
       traefik.http.routers.transmission.tls.certresolver: "letsencrypt"
 
-  sonarr:
-    image: "ghcr.io/hotio/sonarr"
-    volumes:
-      - "./sonarr/config/:/config/"
-    # ports:
-    #   - "8989:8989"
-    restart: "unless-stopped"
-    healthcheck:
-      test: >-
-        curl -Lv
-        "http://sonarr:8989/api/system/status?apikey=${SONARR_API_KEY:-}" |
-        grep '"appData": *"/config"'
-
-  radarr:
-    image: "ghcr.io/hotio/radarr"
-    volumes:
-      - "./radarr/config/:/config/"
-    # ports:
-    #   - "7878:7878"
-    restart: "unless-stopped"
-    healthcheck:
-      test: >-
-        curl -Lv
-        "http://radarr:7878/api/v3/system/status?apikey=${RADARR_API_KEY:-}" |
-        grep '"appData": *"/config"'
+  # See `./docker-compose-servarr.yml` for example Servarr configurations
 
-  ## Container for use by end users
+  ## Container for use by end users:
   prunerr-daemon:
     image: "merpatterson/prunerr"
+    container_name: "prunerr-daemon"
     depends_on:
       - "transmission"
-      - "sonarr"
-      - "radarr"
-    # Match permissions inside and outside the container
     environment:
+      TZ: "${TZ:-Etc/UTC}"
       # Make the run-time user configurable in `./.env` to match permissions inside and
       # outside the container.  Default to the common/standard main/first user and group
       # IDs
       PUID: "${PUID:-1000}"
-      PGID: "${PGID:-${PUID:-1000}}"
+      PGID: "${PGID:-100}"
       # Un-comment to get more verbose `DEBUG` logging
       # DEBUG: "true"
     volumes:
       # Use the Prunerr config from the Prunerr checkout
       - "./home/.config/:/home/prunerr/.config/"
       # The volume on which Transmission's `download-dir` is stored
-      - "${DOWNLOAD_VOLUME}:${DOWNLOAD_VOLUME}"
+      - type: bind
+        source: "${DOWNLOAD_VOLUME:-/media/Library/}"
+        target: "${DOWNLOAD_VOLUME:-/media/Library/}"
+        bind:
+          propagation: "shared"
     restart: "unless-stopped"
```

### Comparing `prunerr-1.0.0/pyproject.toml` & `prunerr-1.1.0b24/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -12,33 +12,35 @@
 # local_scheme = "no-local-version"
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
-version = "1.0.0"
+changelog_start_rev = "v0.0.0"
+version = "1.1.0b24"
 tag_format = "v$version"
 annotated_tag = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
 """
 [tool.towncrier]
 # https://towncrier.readthedocs.io/en/stable/#quick-start
 package = "prunerr"
 package_dir = "src"
+name = "prunerr"
 
 [tool.pylint.MASTER]
-# Auto-detect the number of processors available to use from:
-#     $ pylint --generate-rcfile
-jobs = 0
+# Ensure `duplicate-code` and any other errors that depend on not runnining in parallel
+# are reported:
+jobs = 1
 enable-all-extensions = true
-output-format = "colorized,json:pylint.json"
+output-format = "colorized"
 ignore-paths = [
 # Managed by tools, best to use `# pylint: disable=...` inline comments for any other
 # ignores.
     "src/.+/version.py",
     ".*/src/.+/version.py",
 ]
 # Extend linting to usage of trusted extension packages
@@ -48,17 +50,35 @@
 # Ignore false negatives from external packages
 ignored-classes = ["lxml.etree.QName.localname"]
 # Match Black's defaults
 # https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html#pylint
 [tool.pylint.format]
 max-line-length = "88"
 [tool.pylint."messages control"]
-# I'm not sure I agree with PyLiint here.  I prefer my `TODO`s to be in the the most
-# appropriate context where the change should happen.  It helps my recall.  If someone
-# else wants to take the time to move the `TODO`s into `./TODO.rst`, I won't object as
-# long as sufficient context comes along with them.
-disable = ["fixme"]
+disable = [
+    # Workaround Prospector bug with PyLint:
+    # https://github.com/PyCQA/prospector/issues/596#issue-1592499675
+    "relative-beyond-top-level",
+    # I'm not sure I agree with PyLiint here.  I prefer my `TODO`s to be in the the most
+    # appropriate context where the change should happen.  It helps my recall.  If someone
+    # else wants to take the time to move the `TODO`s into `./TODO.rst`, I won't object as
+    # long as sufficient context comes along with them.
+    "fixme",
+]
+
+[[tool.mypy.overrides]]
+module = [
+       # BBB: Compatibility with older Python versions
+       "backports.cached_property", "pathlib3x",
+       # Direct dependencies
+       "argcomplete", "transmission_rpc", "arrapi.*",
+       ]
+ignore_missing_imports = true
+
+[tool.vulture]
+# https://github.com/jendrikseipp/vulture#ignoring-files
+exclude = ["src/prunerr/version.py"]
 
 [tool.isort]
 # Match Black's defaults
 # https://black.readthedocs.io/en/stable/guides/using_black_with_other_tools.html#isort
 profile = "black"
```

### Comparing `prunerr-1.0.0/requirements-build.txt` & `prunerr-1.1.0b24/requirements/py37/build.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,140 +1,135 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
-#    pip-compile --output-file=./requirements-build.txt --resolver=backtracking ./requirements-build.txt.in
+#    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.0.0
+argcomplete==2.0.6
     # via commitizen
-bleach==5.0.1
+bleach==6.0.0
     # via readme-renderer
-build==0.9.0
-    # via pip-tools
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
 cfgv==3.3.1
     # via pre-commit
 charset-normalizer==2.1.1
     # via
     #   commitizen
     #   requests
-click==8.1.3
-    # via pip-tools
 colorama==0.4.6
     # via commitizen
-commitizen==2.38.0
-    # via -r ./requirements-build.txt.in
-commonmark==0.9.1
-    # via rich
-cryptography==38.0.4
+commitizen==2.42.1
+    # via -r requirements/build.txt.in
+cryptography==40.0.1
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via readme-renderer
-filelock==3.8.2
+filelock==3.11.0
     # via virtualenv
-identify==2.5.9
+identify==2.5.22
     # via pre-commit
 idna==3.4
     # via requests
-importlib-metadata==5.1.0
+importlib-metadata==5.2.0
     # via
+    #   argcomplete
     #   keyring
+    #   pre-commit
     #   twine
+    #   virtualenv
+importlib-resources==5.12.0
+    # via keyring
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 jinja2==3.1.2
     # via commitizen
-keyring==23.11.0
+keyring==23.13.1
     # via twine
-markupsafe==2.1.1
+markdown-it-py==2.2.0
+    # via rich
+markupsafe==2.1.2
     # via jinja2
-more-itertools==9.0.0
+mdurl==0.1.2
+    # via markdown-it-py
+more-itertools==9.1.0
     # via jaraco-classes
 nodeenv==1.7.0
     # via pre-commit
-packaging==22.0
-    # via
-    #   build
-    #   commitizen
-pep517==0.13.0
-    # via build
-pip-tools==6.11.0
-    # via -r ./requirements-build.txt.in
-pkginfo==1.9.2
+packaging==23.0
+    # via commitizen
+pkginfo==1.9.6
     # via twine
-platformdirs==2.6.0
+platformdirs==3.2.0
     # via virtualenv
-pre-commit==2.20.0
-    # via -r ./requirements-build.txt.in
-prompt-toolkit==3.0.36
+pre-commit==2.21.0
+    # via -r requirements/build.txt.in
+prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
-pygments==2.13.0
+pygments==2.15.0
     # via
     #   readme-renderer
     #   rich
 pyyaml==6.0
     # via
     #   commitizen
     #   pre-commit
 questionary==1.10.0
     # via commitizen
 readme-renderer==37.3
     # via twine
-requests==2.28.1
+requests==2.28.2
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.6.0
+rich==13.3.3
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
-termcolor==2.1.1
+termcolor==2.2.0
     # via commitizen
-toml==0.10.2
-    # via pre-commit
-tomli==2.0.1
-    # via
-    #   build
-    #   pep517
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via commitizen
 twine==4.0.2
-    # via -r ./requirements-build.txt.in
-typing-extensions==4.4.0
-    # via commitizen
-urllib3==1.26.13
+    # via -r requirements/build.txt.in
+typing-extensions==4.5.0
+    # via
+    #   commitizen
+    #   importlib-metadata
+    #   markdown-it-py
+    #   platformdirs
+    #   rich
+urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.17.1
+virtualenv==20.21.0
     # via pre-commit
-wcwidth==0.2.5
+wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
-wheel==0.38.4
-    # via pip-tools
-zipp==3.11.0
-    # via importlib-metadata
+zipp==3.15.0
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `prunerr-1.0.0/requirements-devel.txt` & `prunerr-1.1.0b24/requirements/py38/devel.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,190 +1,288 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --extra=devel --output-file=./requirements-devel.txt --resolver=backtracking ./pyproject.toml
+#    pip-compile --extra=devel --output-file=requirements/py38/devel.txt --resolver=backtracking pyproject.toml
 #
-arrapi==1.4.1
-    # via prunerr (./pyproject.toml)
-astroid==2.12.13
-    # via pylint
-attrs==22.1.0
-    # via pytest
-autoflake==2.0.0
-    # via prunerr (./pyproject.toml)
-autopep8==2.0.0
-    # via prunerr (./pyproject.toml)
-black==22.12.0
-    # via flake8-black
-build==0.9.0
-    # via prunerr (./pyproject.toml)
-cachetools==5.2.0
-    # via tox
+argcomplete==3.0.5
+    # via prunerr (pyproject.toml)
+arrapi==1.4.2
+    # via prunerr (pyproject.toml)
+astroid==2.15.2
+    # via
+    #   pylint
+    #   pylint-celery
+    #   pylint-flask
+    #   requirements-detector
+autoflake==1.7.8
+    # via prunerr (pyproject.toml)
+autopep8==2.0.2
+    # via prunerr (pyproject.toml)
+bandit==1.7.5
+    # via prospector
+black==23.3.0
+    # via prunerr (pyproject.toml)
+build==0.10.0
+    # via
+    #   pip-tools
+    #   prunerr (pyproject.toml)
+    #   pyroma
 certifi==2022.12.7
     # via requests
-chardet==5.1.0
-    # via tox
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
+cli-exit-tools==1.2.3.2
+    # via
+    #   lib-detect-testenv
+    #   pathlib3x
 click==8.1.3
     # via
     #   black
+    #   cli-exit-tools
     #   click-default-group
+    #   lib-detect-testenv
+    #   pathlib3x
+    #   pip-tools
     #   towncrier
     #   typer
 click-default-group==1.2.2
     # via towncrier
 colorama==0.4.6
     # via
-    #   tox
+    #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==6.5.0
-    # via prunerr (./pyproject.toml)
+coverage==7.2.3
+    # via prunerr (pyproject.toml)
 dill==0.3.6
     # via pylint
-distlib==0.3.6
-    # via virtualenv
 docutils==0.19
-    # via rstcheck-core
-exceptiongroup==1.0.4
+    # via
+    #   pyroma
+    #   rstcheck-core
+dodgy==0.2.1
+    # via prospector
+exceptiongroup==1.1.1
     # via pytest
-filelock==3.8.2
+flake8==2.3.0
     # via
-    #   tox
-    #   virtualenv
-flake8==6.0.0
-    # via
-    #   flake8-black
-    #   prunerr (./pyproject.toml)
-flake8-black==0.3.5
-    # via prunerr (./pyproject.toml)
+    #   flake8-polyfill
+    #   prospector
+flake8-polyfill==1.0.2
+    # via pep8-naming
+future==0.18.3
+    # via radon
+gitdb==4.0.10
+    # via gitpython
+gitpython==3.1.31
+    # via
+    #   bandit
+    #   prospector
 idna==3.4
     # via requests
 incremental==22.10.0
     # via towncrier
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
-isort==5.11.0
+isort==5.12.0
     # via pylint
 jinja2==3.1.2
     # via towncrier
-lazy-object-proxy==1.8.0
+lazy-object-proxy==1.9.0
     # via astroid
+lib-detect-testenv==2.0.3
+    # via cli-exit-tools
 main-wrapper==0.1.1
     # via service-logging
-markupsafe==2.1.1
+mando==0.6.4
+    # via radon
+markupsafe==2.1.2
     # via jinja2
 mccabe==0.7.0
     # via
     #   flake8
+    #   prospector
     #   pylint
-mypy-extensions==0.4.3
-    # via black
-packaging==22.0
+mypy==1.2.0
+    # via prospector
+mypy-extensions==1.0.0
+    # via
+    #   black
+    #   mypy
+packaging==23.0
     # via
+    #   black
     #   build
-    #   pyproject-api
+    #   prospector
+    #   pyroma
     #   pytest
+    #   requirements-detector
     #   setuptools-scm
-    #   tox
-pathspec==0.10.3
+pathlib3x==2.0.2.1 ; python_version < "3.10"
+    # via prunerr (pyproject.toml)
+pathspec==0.11.1
     # via black
-pep517==0.13.0
-    # via build
-platformdirs==2.6.0
+pbr==5.11.1
+    # via stevedore
+pep8==1.7.1
+    # via flake8
+pep8-naming==0.10.0
+    # via prospector
+pip-tools==6.13.0
+    # via prunerr (pyproject.toml)
+platformdirs==3.2.0
     # via
     #   black
     #   pylint
-    #   tox
-    #   virtualenv
 pluggy==1.0.0
-    # via
-    #   pytest
-    #   tox
+    # via pytest
+poetry-semver==0.1.0
+    # via requirements-detector
+prospector[with_everything]==1.9.0
+    # via prunerr (pyproject.toml)
 pycodestyle==2.10.0
     # via
     #   autopep8
-    #   flake8
-pydantic==1.10.2
+    #   prospector
+pydantic==1.10.7
     # via rstcheck-core
-pyflakes==3.0.1
+pydocstyle==6.3.0
+    # via prospector
+pyflakes==2.5.0
     # via
     #   autoflake
     #   flake8
-pygments==2.13.0
-    # via rich
-pylint==2.15.8
-    # via prunerr (./pyproject.toml)
-pyproject-api==1.2.1
-    # via tox
-pytest==7.2.0
-    # via prunerr (./pyproject.toml)
+    #   prospector
+pygments==2.15.0
+    # via
+    #   pyroma
+    #   rich
+pylint==2.17.2
+    # via
+    #   prospector
+    #   pylint-celery
+    #   pylint-django
+    #   pylint-flask
+    #   pylint-plugin-utils
+pylint-celery==0.3
+    # via prospector
+pylint-django==2.5.3
+    # via prospector
+pylint-flask==0.6
+    # via prospector
+pylint-plugin-utils==0.7
+    # via
+    #   prospector
+    #   pylint-celery
+    #   pylint-django
+    #   pylint-flask
+pyproject-hooks==1.0.0
+    # via build
+pyroma==4.2
+    # via prospector
+pytest==7.3.0
+    # via prunerr (pyproject.toml)
 pyyaml==6.0
-    # via prunerr (./pyproject.toml)
-requests==2.28.1
+    # via
+    #   bandit
+    #   prospector
+    #   prunerr (pyproject.toml)
+    #   xenon
+radon==5.1.0
+    # via xenon
+requests==2.28.2
     # via
     #   arrapi
+    #   pyroma
     #   requests-mock
     #   transmission-rpc
+    #   xenon
 requests-mock==1.10.0
-    # via prunerr (./pyproject.toml)
+    # via prunerr (pyproject.toml)
+requirements-detector==1.1.0
+    # via prospector
 rich==12.6.0
-    # via typer
-rstcheck==6.1.1
-    # via prunerr (./pyproject.toml)
+    # via
+    #   bandit
+    #   typer
+rstcheck==6.1.2
+    # via prunerr (pyproject.toml)
 rstcheck-core==1.0.3
     # via rstcheck
 service-logging==0.1.1
-    # via prunerr (./pyproject.toml)
-setuptools-scm==7.0.5
-    # via prunerr (./pyproject.toml)
-shellingham==1.5.0
+    # via prunerr (pyproject.toml)
+setoptconf-tmp==0.3.1
+    # via prospector
+setuptools-scm==7.1.0
+    # via prunerr (pyproject.toml)
+shellingham==1.5.0.post1
     # via typer
 six==1.16.0
     # via
     #   main-wrapper
+    #   mando
     #   requests-mock
-tenacity==8.1.0
-    # via prunerr (./pyproject.toml)
+smmap==5.0.0
+    # via gitdb
+snowballstemmer==2.2.0
+    # via pydocstyle
+stevedore==5.0.0
+    # via bandit
+tenacity==8.2.2
+    # via prunerr (pyproject.toml)
+toml==0.10.2
+    # via
+    #   prospector
+    #   requirements-detector
+    #   vulture
 tomli==2.0.1
     # via
     #   autoflake
     #   autopep8
     #   black
     #   build
-    #   flake8-black
-    #   pep517
+    #   mypy
     #   pylint
-    #   pyproject-api
+    #   pyproject-hooks
     #   pytest
     #   setuptools-scm
     #   towncrier
-    #   tox
-tomlkit==0.11.6
+tomlkit==0.11.7
     # via pylint
-towncrier==22.8.0
-    # via prunerr (./pyproject.toml)
-tox==4.0.8
-    # via prunerr (./pyproject.toml)
-transmission-rpc==3.4.0
-    # via prunerr (./pyproject.toml)
+towncrier==22.12.0
+    # via prunerr (pyproject.toml)
+transmission-rpc==3.4.2
+    # via prunerr (pyproject.toml)
+trove-classifiers==2023.3.9
+    # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.1
+types-docutils==0.19.1.7
     # via rstcheck-core
-typing-extensions==4.4.0
+types-pyyaml==6.0.12.9
+    # via prunerr (pyproject.toml)
+typing-extensions==4.5.0
     # via
+    #   astroid
+    #   black
+    #   mypy
     #   pydantic
+    #   pylint
+    #   rich
     #   setuptools-scm
     #   transmission-rpc
-urllib3==1.26.13
+urllib3==1.26.15
     # via requests
-virtualenv==20.17.1
-    # via tox
-wrapt==1.14.1
+vulture==2.7
+    # via prospector
+wheel==0.40.0
+    # via pip-tools
+wrapt==1.15.0
     # via astroid
+xenon==0.9.0
+    # via prunerr (pyproject.toml)
 
 # The following packages are considered to be unsafe in a requirements file:
+# pip
 # setuptools
```

### Comparing `prunerr-1.0.0/requirements.txt` & `prunerr-1.1.0b24/requirements/py310/user.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=./requirements.txt --resolver=backtracking ./pyproject.toml
+#    pip-compile --output-file=requirements/py310/user.txt --resolver=backtracking pyproject.toml
 #
-arrapi==1.4.1
-    # via prunerr (./pyproject.toml)
+argcomplete==3.0.5
+    # via prunerr (pyproject.toml)
+arrapi==1.4.2
+    # via prunerr (pyproject.toml)
 certifi==2022.12.7
     # via requests
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
     # via requests
 idna==3.4
     # via requests
 main-wrapper==0.1.1
     # via service-logging
 pyyaml==6.0
-    # via prunerr (./pyproject.toml)
-requests==2.28.1
+    # via prunerr (pyproject.toml)
+requests==2.28.2
     # via
     #   arrapi
     #   transmission-rpc
 service-logging==0.1.1
-    # via prunerr (./pyproject.toml)
+    # via prunerr (pyproject.toml)
 six==1.16.0
     # via main-wrapper
-tenacity==8.1.0
-    # via prunerr (./pyproject.toml)
-transmission-rpc==3.4.0
-    # via prunerr (./pyproject.toml)
-typing-extensions==4.4.0
+tenacity==8.2.2
+    # via prunerr (pyproject.toml)
+transmission-rpc==3.4.2
+    # via prunerr (pyproject.toml)
+typing-extensions==4.5.0
     # via transmission-rpc
-urllib3==1.26.13
+urllib3==1.26.15
     # via requests
```

### Comparing `prunerr-1.0.0/setup.cfg` & `prunerr-1.1.0b24/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -12,30 +12,38 @@
 	servarr
 	sonarr
 	radarr
 	transmission
 	bittorent
 	torrent
 classifiers = 
+	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: POSIX :: BSD
 	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.7
 	Topic :: Communications :: File Sharing
 	Topic :: Internet
 
 [options]
 package_dir = 
 	=src
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	transmission-rpc
+	backports.cached-property; python_version < "3.8"
+	pathlib3x; python_version < "3.10"
+	argcomplete
+	transmission-rpc<4
 	service-logging
 	pyyaml
 	arrapi>=1.2
 	tenacity
 
 [options.packages.find]
 where = src
@@ -43,23 +51,24 @@
 [options.entry_points]
 console_scripts = 
 	prunerr = prunerr:main
 
 [options.extras_require]
 devel = 
 	requests-mock
-	tox
 	pytest
 	coverage
-	pylint
-	flake8
+	prospector[with_everything]
+	xenon
 	rstcheck
-	flake8-black
+	black
 	autoflake
 	autopep8
+	types-PyYAML
+	pip-tools
 	setuptools_scm
 	towncrier
 	build
 
 [tool:pytest]
 testpaths = src/prunerr
```

### Comparing `prunerr-1.0.0/src/prunerr/__init__.py` & `prunerr-1.1.0b24/src/prunerr/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,29 @@
+# PYTHON_ARGCOMPLETE_OK
 """
 Remove Servarr download client items to preserve disk space according to rules.
 """
 
-import os
+import sys
 import contextlib
 import logging
 import pathlib  # TODO: replace os.path
 import argparse
-import pprint
 import mimetypes
+import json
+import pdb
+
+import argcomplete
 
 import prunerr.runner
 import prunerr.downloadclient
+import prunerr.downloaditem
+import prunerr.operations
+import prunerr.servarr
+from . import utils
 
 logger = logging.getLogger(__name__)
 
 # Manage version through the VCS CI/CD process
 __version__ = None
 try:
     from . import version
@@ -31,14 +39,21 @@
 
 # Define command line options and arguments
 parser = argparse.ArgumentParser(
     description=__doc__.strip(),
     formatter_class=argparse.ArgumentDefaultsHelpFormatter,
 )
 parser.add_argument(
+    "--log-level",
+    default=argparse.SUPPRESS,
+    # I only wish the `logging` module provided public access to all defined levels
+    choices=logging._nameToLevel,  # pylint: disable=protected-access
+    help="Select logging verbosity. (default: INFO)",
+)
+parser.add_argument(
     "--config",
     "-c",
     type=argparse.FileType("r"),
     default=str(pathlib.Path.home() / ".config" / "prunerr.yml"),
     help="""\
 The path to the Prunerr configuration file. Example:
 https://gitlab.com/rpatterson/prunerr/-/blob/master/src/prunerr/home/.config/prunerr.yml\
@@ -58,125 +73,159 @@
     # Wait for all verifying torrents to finish when doing a single `verify` run.
     return runner.resume_verified_items(wait=True)
 
 
 verify.__doc__ = prunerr.runner.PrunerrRunner.verify.__doc__
 parser_verify = subparsers.add_parser(
     "verify",
-    help=verify.__doc__.strip(),
-    description=verify.__doc__.strip(),
+    help=verify.__doc__.strip(),  # type: ignore
+    description=verify.__doc__.strip(),  # type: ignore
 )
 parser_verify.set_defaults(command=verify)
 
 
 def move(runner, *args, **kwargs):  # pylint: disable=missing-function-docstring
     runner.update()
     return runner.move(*args, **kwargs)
 
 
 move.__doc__ = prunerr.runner.PrunerrRunner.move.__doc__
 parser_move = subparsers.add_parser(
     "move",
-    help=move.__doc__.strip(),
-    description=move.__doc__.strip(),
+    help=move.__doc__.strip(),  # type: ignore
+    description=move.__doc__.strip(),  # type: ignore
 )
 parser_move.set_defaults(command=move)
 
 
 def review(runner, *args, **kwargs):  # pylint: disable=missing-function-docstring
     runner.update()
     return runner.review(*args, **kwargs)
 
 
 review.__doc__ = prunerr.runner.PrunerrRunner.review.__doc__
 parser_review = subparsers.add_parser(
     "review",
-    help=review.__doc__.strip(),
-    description=review.__doc__.strip(),
+    help=review.__doc__.strip(),  # type: ignore
+    description=review.__doc__.strip(),  # type: ignore
 )
 # Make the function for the sub-command specified in the CLI argument available in the
 # argument parser for delegation below.
 parser_review.set_defaults(command=review)
 
 
 def free_space(runner, *args, **kwargs):  # pylint: disable=missing-function-docstring
     runner.update()
     return runner.free_space(*args, **kwargs)
 
 
 free_space.__doc__ = prunerr.runner.PrunerrRunner.free_space.__doc__
 parser_free_space = subparsers.add_parser(
     "free-space",
-    help=free_space.__doc__.strip(),
-    description=free_space.__doc__.strip(),
+    help=free_space.__doc__.strip(),  # type: ignore
+    description=free_space.__doc__.strip(),  # type: ignore
 )
 parser_free_space.set_defaults(command=free_space)
 
 
 def exec_(runner, *args, **kwargs):  # pylint: disable=missing-function-docstring
     runner.update()
+    results = {}
     exec_results = runner.exec_(*args, **kwargs)
+    if exec_results is not None:
+        results.update(exec_results)
 
     # Wait for all verifying torrents to finish when doing a single `exec` run.
     resume_results = runner.resume_verified_items(wait=True)
     if resume_results:
-        exec_results["verify"] = resume_results
+        results["verify"] = resume_results
 
-    return exec_results
+    if results:
+        return results
+    return None  # pragma: no cover
 
 
 exec_.__doc__ = prunerr.runner.PrunerrRunner.exec_.__doc__
 parser_exec = subparsers.add_parser(
     "exec",
-    help=exec_.__doc__.strip(),
-    description=exec_.__doc__.strip(),
+    help=exec_.__doc__.strip(),  # type: ignore
+    description=exec_.__doc__.strip(),  # type: ignore
 )
 parser_exec.set_defaults(command=exec_)
 
 
 def daemon(runner, *args, **kwargs):  # pylint: disable=missing-function-docstring
     return runner.daemon(*args, **kwargs)
 
 
 daemon.__doc__ = prunerr.runner.PrunerrRunner.daemon.__doc__
 parser_daemon = subparsers.add_parser(
     "daemon",
-    help=daemon.__doc__.strip(),
-    description=daemon.__doc__.strip(),
+    help=daemon.__doc__.strip(),  # type: ignore
+    description=daemon.__doc__.strip(),  # type: ignore
 )
 parser_daemon.set_defaults(command=daemon)
+# Register shell tab completion
+argcomplete.autocomplete(parser)
 
 
 def config_cli_logging(
-    root_level=logging.INFO, **kwargs
-):  # pylint: disable=unused-argument
+    root_level=logging.INFO,
+    log_level=parser.get_default("--log-level"),
+    **_,
+):
     """
-    Configure logging CLI usage first, but also appropriate for writing to log files.
+    Configure logging CLI usage as early as possible to affect all output.
     """
     # Want just our logger's level, not others', to be controlled by options/environment
     logging.basicConfig(level=root_level)
-    if "DEBUG" in os.environ and os.getenv("DEBUG").strip().lower() in {
-        "1",
-        "true",
-        "yes",
-        "on",
-    }:
-        level = logging.DEBUG
-    else:  # pragma: no cover
-        level = logging.INFO
-    logger.setLevel(level)
+    # If the CLI option was not specified, fallback to the environment variable
+    if log_level is None:
+        log_level = "INFO"
+        if utils.DEBUG:  # pragma: no cover
+            log_level = "DEBUG"
+    logger.setLevel(getattr(logging, log_level.strip().upper()))
+    # Log a given message only once per daemon session, the first loop.
+    logger.addFilter(utils.daemon_once_filter)
+    logging.getLogger(prunerr.runner.__name__).addFilter(
+        utils.daemon_once_filter,
+    )
+    logging.getLogger(prunerr.downloadclient.__name__).addFilter(
+        utils.daemon_once_filter,
+    )
+    logging.getLogger(prunerr.downloaditem.__name__).addFilter(
+        utils.daemon_once_filter,
+    )
+    logging.getLogger(prunerr.operations.__name__).addFilter(
+        utils.daemon_once_filter,
+    )
+    logging.getLogger(prunerr.servarr.__name__).addFilter(
+        utils.daemon_once_filter,
+    )
 
     # Avoid logging all JSON responses, particularly the very large history responses
     # from Servarr APIs
     logging.getLogger("arrapi.api").setLevel(logging.INFO)
 
-    return level
+    return log_level
 
 
 def main(args=None):  # pylint: disable=missing-function-docstring
+    try:
+        _main(args=args)
+    except Exception:  # pragma: no cover
+        if utils.POST_MORTEM:
+            pdb.post_mortem()
+        raise
+
+
+def _main(args=None):
+    """
+    Inner main CLI handler for outer exception handling.
+    """
     # Parse CLI options and positional arguments
     parsed_args = parser.parse_args(args=args)
     # Avoid noisy boilerplate, functions meant to handle CLI usage should accept kwargs
     # that match the defined option and argument names.
     cli_kwargs = dict(vars(parsed_args))
     # Remove any meta options and arguments, those used to direct option and argument
     # handling, that shouldn't be passed onto functions meant to handle CLI usage.  More
@@ -196,19 +245,20 @@
     for dest, value in list(shared_kwargs.items()):
         if dest not in prunerr_dests:  # pragma: no cover
             command_kwargs[dest] = value
             del shared_kwargs[dest]
 
     # Configure logging for CLI usage
     config_cli_logging(**shared_kwargs)
+    shared_kwargs.pop("log_level", None)
 
     runner = prunerr.runner.PrunerrRunner(**shared_kwargs)
     # Delegate to the function for the sub-command CLI argument
-    logger.info("Running %r sub-command", parsed_args.command.__name__)
+    logger.debug("Running %r sub-command", parsed_args.command.__name__)
     # Sub-commands may return a result to be pretty printed, or handle output themselves
     # and return nothing.
     result = parsed_args.command(runner, **command_kwargs)
     if result is not None:
-        pprint.pprint(result)
+        json.dump(result, sys.stdout, indent=2)
 
 
 main.__doc__ = __doc__
```

### Comparing `prunerr-1.0.0/src/prunerr/downloadclient.py` & `prunerr-1.1.0b24/src/prunerr/downloadclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """
 Prunerr interaction with download clients.
 """
 
-import pathlib
+import re
 import shutil
 import urllib.parse
 import logging
 
 import transmission_rpc
 
 import prunerr.downloaditem
 import prunerr.operations
+from .utils import pathlib
 
 logger = logging.getLogger(__name__)
 
 
 class PrunerrDownloadClient:
     """
     An individual, specific download client that Prunerr interacts with.
     """
 
     # TODO: Make configurable?
     SEEDING_DIR_BASENAME = "seeding"
+    UNREGISTERED_ERROR_RE = re.compile(r".*(not |un)registered.*")
 
     config = None
     client = None
     items = None
     operations = None
 
     def __init__(self, runner):
@@ -122,15 +124,15 @@
         results = {}
         # Need to make a copy in case review leads to deleting an item and modifying
         # `self.items`.
         download_dir = pathlib.Path(self.client.session.download_dir)
         for item in [item for item in self.items if download_dir in item.path.parents]:
             item_results = item.review(servarr_queue)
             if item_results:
-                results[item] = item_results
+                results[item.hashString] = item_results
         return results
 
     # Other, non-sub-command methods
 
     def sort_items_by_tracker(self, items):
         """
         Sort the given download items according to the indexer priority operations.
@@ -274,19 +276,19 @@
         speed_limit_down = self.runner.config.get("download-clients", {}).get(
             "max-download-bandwidth",
             100,
         )
         if session.speed_limit_down_enabled and (
             not speed_limit_down or speed_limit_down != session.speed_limit_down
         ):
-            kwargs = dict(speed_limit_down_enabled=False)
+            kwargs = {"speed_limit_down_enabled": False}
             logger.info("Resuming downloading: %s", kwargs)
             self.client.set_session(**kwargs)
 
-    def find_unregistered(self):
+    def find_unregistered(self):  # noqa: V105
         """
         Filter already imported items that are no longer recognized by their tracker.
 
         For example, when a private tracker removes a duplicate/invalid/unauthorized
         item.
         """
         # TODO: Mark as failed in Servarr?
@@ -302,19 +304,20 @@
                     or [
                         seeding_dir
                         for seeding_dir in seeding_dirs
                         if seeding_dir in item.path.parents
                     ]
                 )
                 and item.error == 2
-                and "unregistered item" in item.errorString.lower()
+                and self.UNREGISTERED_ERROR_RE.match(item.errorString.lower())
+                is not None
             )
         )
 
-    def find_seeding(self):
+    def find_seeding(self):  # noqa: V105
         """
         Filter items that have not yet been imported by Servarr, order by priority.
         """
         seeding_dir = (
             pathlib.Path(self.client.session.download_dir).parent
             / self.SEEDING_DIR_BASENAME
         )
@@ -331,15 +334,14 @@
         """
         Verify and resume download items flagged as having corrupt data.
         """
         corrupt_items = {
             item.hashString: item
             for item in self.items
             if item.hashString not in self.verifying_items
-            and item.status == "stopped"
             and item.error == 3
             and (
                 "verif" in item.errorString.lower()
                 or "corrput" in item.errorString.lower()
             )
         }
         if corrupt_items:
```

### Comparing `prunerr-1.0.0/src/prunerr/downloaditem.py` & `prunerr-1.1.0b24/src/prunerr/downloaditem.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """
 Prunerr interaction with download clients.
 """
 
 import os
-import functools
 import time
-import pathlib
 import urllib.parse
 import json
 import logging
 
 import transmission_rpc
 
+from .utils import pathlib
+from .utils import cached_property
+
 logger = logging.getLogger(__name__)
 
 
 def parallel_to(base_path, parallel_path, root_basename):
     """
     Return a path with a parallel relative root to the given full path.
     """
     base_path = pathlib.Path(base_path)
     common_path = pathlib.Path(os.path.commonpath((base_path.parent, parallel_path)))
     return (
         common_path
         / root_basename
         / pathlib.Path(parallel_path).relative_to(
-            parallel_path.parents[-(len(base_path.parts))],
+            list(parallel_path.parents)[-(len(base_path.parts))],
         )
     )
 
 
 class PrunerrDownloadItem(transmission_rpc.Torrent):
     """
     Enrich download item data from the download client API.
@@ -48,15 +49,15 @@
     def update(self, timeout=None):
         """
         Update cached values when this download item is updated.
         """
         super().update(timeout=timeout)
         vars(self).pop("path", None)
 
-    @property
+    @cached_property
     def root_name(self):
         """
         Return the name of the first path element for all items in the download item.
 
         Needed because it's not always the same as the item's name.  If the download
         item has multiple files, assumes that all files are under the same top-level
         directory.
@@ -64,57 +65,58 @@
         file_roots = [pathlib.Path(item_file.name).parts[0] for item_file in self.files]
         if file_roots:
             if len(set(file_roots)) > 1:
                 logger.error(
                     "Files in %r have multiple roots, using: %s",
                     self,
                     file_roots[0],
+                    extra={"runner": self.download_client.runner},
                 )
             return file_roots[0]
         return self.name
 
-    @functools.cached_property
+    @cached_property
     def path(self):
         """
         Return the root path for all files in the download item.
 
         Needed because it's not always the same as the item's download directory plus
         the item's name.
         """
         return (pathlib.Path(self.download_dir) / self.root_name).resolve()
 
-    @property
+    @cached_property
     def files_parent(self):
         """
-        The path in which the download item's files are currently stored.
+        Determine the path in which the download item's files are currently stored.
 
         This may be the `incomplete_dir` while the item is downloading.
         """
         files_parent = pathlib.Path(self.download_dir) / self.root_name
         if (
             self.download_client.client.session.incomplete_dir_enabled
             and not files_parent.exists()
         ):
             files_parent = (
                 pathlib.Path(self.download_client.client.session.incomplete_dir)
                 / files_parent.name
             )
         return files_parent.resolve()
 
-    @property
+    @cached_property  # noqa: V105
     def age(self):
         """
-        The total time since the item was added.
+        Determine the total time since the item was added.
         """
         return time.time() - self._fields["addedDate"].value
 
-    @property
+    @cached_property
     def seconds_since_done(self):
         """
-        Number of seconds elapsed since the download item was completely downloaded.
+        Determine the number of seconds since the item was completely downloaded.
 
         Best available estimation of total seeding time.
         """
         if self._fields["leftUntilDone"].value or self._fields["percentDone"].value < 1:
             logger.warning(
                 "Can't determine seconds since done, not complete: %r",
                 self,
@@ -139,28 +141,64 @@
 
         logger.warning(
             "Missing done date for seconds since done: %r",
             self,
         )
         return None
 
-    @property
-    def rate_total(self):
+    @cached_property
+    def seconds_downloading(self):
         """
-        The total download rate across the whole download time.
+        Determine the number of seconds spent downloading the item.
+
+        Best available estimation of total downloading duration.
         """
         done_date = self._fields["doneDate"].value
+        if done_date == self._fields["addedDate"].value:
+            logger.warning(
+                "Done date is the same as added date: %r",
+                self,
+                extra={"runner": self.download_client.runner},
+            )
+        elif done_date < self._fields["addedDate"].value:
+            logger.warning(
+                "Done date is before added date: %r",
+                self,
+                extra={"runner": self.download_client.runner},
+            )
         if not done_date:
             done_date = time.time()
+            if done_date == self._fields["addedDate"].value:
+                logger.warning(  # pragma: no cover
+                    "Added date is now: %r",
+                    self,
+                    extra={"runner": self.download_client.runner},
+                )
+            elif done_date < self._fields["addedDate"].value:
+                logger.warning(
+                    "Added date is in the future: %r",
+                    self,
+                    extra={"runner": self.download_client.runner},
+                )
+        return done_date - self._fields["addedDate"].value
+
+    @cached_property
+    def rate_total(self):
+        """
+        Determine the total download rate across the whole download time.
+        """
+        seconds_downloading = self.seconds_downloading
+        if seconds_downloading <= 0:
+            return None
         return (
             self._fields["sizeWhenDone"].value - self._fields["leftUntilDone"].value
-        ) / (done_date - self._fields["addedDate"].value)
+        ) / seconds_downloading
 
-    @functools.cached_property
-    def files(self):  # pylint: disable=invalid-overridden-method
+    @cached_property
+    def files(self):  # pylint: disable=invalid-overridden-method,useless-suppression
         """
         Iterate over all download item file paths that exist.
 
         Optionally filter the list by those that are selected in the download client.
         """
         return [PrunerrDownloadItemFile(self, rpc_file) for rpc_file in super().files()]
 
@@ -202,26 +240,26 @@
         results = []
         for operation_config, sort_value in zip(operation_configs, sort_key[1:]):
             if sort_value:
                 # Sort value didn't match review operation requirements
                 continue
 
             if operation_config.get("remove", False):
-                result = dict(remove=True)
+                result = {"remove": True}
                 logger.info(
                     "Removing download item per %r review: %r",
                     operation_config["type"],
                     self,
                 )
-                if queue_id is None:
-                    if not queue_record and not self.download_client.runner.quiet:
-                        logger.warning(
-                            "Download item not in any Servarr queue: %r",
-                            self,
-                        )
+                if not queue_record:
+                    logger.warning(
+                        "Download item not in any Servarr queue: %r",
+                        self,
+                        extra={"runner": self.download_client.runner},
+                    )
                 else:
                     delete_params = {}
                     if operation_config.get("blacklist", False):
                         delete_params["blacklist"] = "true"
                         result["blacklist"] = True
                     queue_record["servarr"].client.delete(
                         f"queue/{queue_id}",
@@ -258,36 +296,39 @@
         """
         Capture a reference to the RPC client library item file.
         """
         self.download_item = download_item
         self.rpc_file = rpc_file
 
     def __getattr__(self, name):
+        """
+        Make `stat()` properties available as attributes.
+        """
         try:
             return getattr(self.rpc_file, name)
         except AttributeError:
             return getattr(self.stat, name)
 
-    @functools.cached_property
+    @cached_property
     def path(self):
         """
         Assemble a `pathlib` path for this item file only as needed and only once.
         """
         return self.download_item.path.parent / self.rpc_file.name
 
-    @functools.cached_property
+    @cached_property
     def stat(self):
         """
         Lookup item file `stat` metadata only as needed and only once.
         """
         if self.path.exists():
             return self.path.stat()
         return None
 
-    @functools.cached_property
+    @cached_property  # noqa: V105
     def size_imported(self):
         """
         Return the file's size if the file has more than one hard link.
         """
         if self.stat is not None and self.st_nlink > 1:
             return self.st_size
         return 0
```

### Comparing `prunerr-1.0.0/src/prunerr/home/.config/prunerr.yml` & `prunerr-1.1.0b24/src/prunerr/home/.config/prunerr.yml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     api-key: ""
     type: "sonarr"
   Radarr:
     url: "http://localhost:7878"
     api-key: ""
     type: "radarr"
 download-clients:
-  ## TODO: Support multiple download clients
   ## Support managing download clients without Servarr instances, use these URLs to
   ## connect to download clients instead of looking them up from Servarr settings.
   # urls:
   #   - "https://transmission:secret@transmission.example.com"
   ## Calculate an appropriate margin of disk space to keep free when deciding whether to
   ## prune download items based the maximum download bandwidth/speed in Mbps and the
   ## amount of time in seconds at that rate for which download clients should be able to
@@ -63,14 +62,18 @@
               name: "status"
               equals: "seeding"
             - type: "value"
               name: "age"
               # 1 week * 7 days * 24 hours * 60 minutes * 60 seconds
               maximum: 604800
             - type: "value"
+              name: "seconds_downloading"
+              # Don't remove items that haven't started downloading yet
+              maximum: 0
+            - type: "value"
               name: "rate_total"
               # Minimum Bps of total throughput before an item is considered stalled
               minimum: 50
           remove: true
           blacklist: true
         ## Reject download items containing archives to optimize seeding per disk space.
         - type: "files"
@@ -106,14 +109,17 @@
             - type: "value"
               name: "status"
               equals: "seeding"
             - type: "value"
               name: "age"
               maximum: 604800
             - type: "value"
+              name: "seconds_downloading"
+              maximum: 0
+            - type: "value"
               name: "rate_total"
               minimum: 50
           remove: true
           blacklist: true
         - type: "files"
           patterns:
             - ".+\\.rar$"
```

### Comparing `prunerr-1.0.0/src/prunerr/operations.py` & `prunerr-1.1.0b24/src/prunerr/operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
         include, sort_key = self.exec_operations(indexer_config["operations"], item)
         cached_results[operations_type] = (include, (indexer_idx,) + sort_key)
         return cached_results[operations_type]
 
     def exec_operations(self, operation_configs, item):
         """
-        Execute each of the configured indexer priority operations
+        Execute each of the configured indexer priority operations.
         """
         # TODO: Add `name` to operation configs and use in log/exc messages
         sort_key = []
         include = True
         for operation_config in operation_configs:
             executor = getattr(self, f"exec_operation_{operation_config['type']}", None)
             if executor is None:
@@ -88,15 +88,14 @@
             sort_key.append(sort_value)
         return include, tuple(sort_key)
 
     def apply_sort_value(self, operation_config, include, sort_value):
         """
         Apply any restrictions that can apply across different operation types.
         """
-
         sort_bool = None
         if "equals" in operation_config:
             sort_bool = sort_value == operation_config["equals"]
             if "minimum" in operation_config or "maximum" in operation_config:
                 raise ValueError(
                     f"Operation {operation_config['type']!r} "
                     f"includes both `equals` and `minimum` or `maximum`"
@@ -121,52 +120,52 @@
                 raise NotImplementedError(
                     f"Indexer priority operation value doesn't support `reversed`:"
                     f"{sort_value!r}"
                 )
 
         return include, sort_value
 
-    def exec_operation_value(self, operation_config, item):
+    def exec_operation_value(self, operation_config, item):  # noqa: V105
         """
         Return the attribute or key value for the download item.
         """
         # Use `missing_value` instead of `hasattr()`
         # to avoid redundant property method calls
         value = getattr(item, operation_config["name"], missing_value)
         if value is not missing_value:
             return value
         return None
 
-    def exec_operation_or(self, operation_config, item):
+    def exec_operation_or(self, operation_config, item):  # noqa: V105
         """
         Return `True` if any of the nested operations return `True`.
         """
         _, sort_key = self.exec_operations(
             operation_config["operations"],
             item,
         )
         for sort_value in sort_key:
             if sort_value:
                 return sort_value
         return sort_key[-1] if sort_key else False
 
-    def exec_operation_and(self, operation_config, download_item):
+    def exec_operation_and(self, operation_config, download_item):  # noqa: V105
         """
         Return `False` if any of the nested operations return `False`.
         """
         _, sort_key = self.exec_operations(
             operation_config["operations"],
             download_item,
         )
         for sort_value in sort_key:
             if not sort_value:
                 return sort_value
         return sort_key[-1]
 
-    def exec_operation_files(self, operation_config, download_item):
+    def exec_operation_files(self, operation_config, download_item):  # noqa: V105
         """
         Return aggregated values from item files.
         """
         file_attr = operation_config.get("name", "size")
         aggregation = operation_config.get("aggregation", "portion")
         total = operation_config.get("total", "size_when_done")
```

### Comparing `prunerr-1.0.0/src/prunerr/runner.py` & `prunerr-1.1.0b24/src/prunerr/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 Run Prunerr commands across multiple Servarr instances and download clients.
 """
 
+import gc
 import os
 import time
 import socket
-import functools
 import pathlib
 import json
 import logging
 
 import yaml
 import tenacity
 import transmission_rpc
 import arrapi
 
 import prunerr.downloadclient
 import prunerr.servarr
+from .utils import cached_property
 
 logger = logging.getLogger(__name__)
 
 
 class PrunerrRunner:
     """
     Run Prunerr sub-commands across multiple Servarr instances and download clients.
@@ -67,20 +68,17 @@
         with self.config_file.open(encoding="utf-8") as config_opened:
             self.config = yaml.safe_load(config_opened)
 
         # Update Servarr API clients
         servarrs = {}
         for servarr_name, servarr_config in self.config.get("servarrs", {}).items():
             servarr_config.setdefault("name", servarr_name)
-            if servarr_config["url"] in self.servarrs:
-                servarrs[servarr_config["url"]] = self.servarrs[servarr_config["url"]]
-            else:
-                servarrs[
-                    servarr_config["url"]
-                ] = prunerr.servarr.PrunerrServarrInstance(self)
+            servarrs[servarr_config["url"]] = prunerr.servarr.PrunerrServarrInstance(
+                self
+            )
             servarrs[servarr_config["url"]].update(servarr_config)
         self.servarrs = servarrs
 
         # Update download client RPC clients
         # Download clients not connected to a Servarr instance
         download_client_configs = {
             download_client_url: {"url": download_client_url}
@@ -118,15 +116,15 @@
                     download_client_url
                 ].download_client = download_clients[download_client_url]
             download_clients[download_client_url].update(download_client_config)
         self.download_clients = download_clients
 
         return self.download_clients
 
-    @functools.cached_property
+    @cached_property
     def example_confg(self):
         """
         Use the example configuration file for defaults where needed.
         """
         with self.EXAMPLE_CONFIG.open() as config_opened:
             return yaml.safe_load(config_opened)
 
@@ -143,15 +141,17 @@
         # time to finish as possible.
         self.verify()
 
         # Run `review` before `move` so it can make any changes to download items before
         # they're moved and excluded from future review.
         # Also run before `free-space` in case it removes items.
         if "reviews" in self.config.get("indexers", {}):
-            results["review"] = self.review()
+            review_results = self.review()
+            if review_results is not None:
+                results["review"] = review_results
 
         # Run `move` before `free-spacce` so that all download items that could be
         # eligible for deletion are in the `seeding` directory.
         move_results = self.move()
         if move_results:
             results["move"] = move_results
 
@@ -276,15 +276,15 @@
                 "Insufficient free space for %r but nothing can be deleted: %0.2f %s",
                 download_client_url,
                 *transmission_rpc.utils.format_size(
                     download_client.config["min-free-space"]
                     - download_client.client.session.download_dir_free_space,
                 ),
             )
-            kwargs = dict(speed_limit_down=0, speed_limit_down_enabled=True)
+            kwargs = {"speed_limit_down": 0, "speed_limit_down_enabled": True}
             # TODO: Notification when downloading is paused
             logger.info("Stopping downloading: %s", kwargs)
             download_client.client.set_session(**kwargs)
 
         return results
 
     def daemon(self):
@@ -317,21 +317,26 @@
                 )
                 # Re-connect to external services and retry
             else:
                 # Don't repeat noisy messages from now on.
                 self.quiet = True
             logger.debug("Sub-command `exec` completed in %ss", time.time() - start)
 
-            # Wait for the next interval
+            # Determine the poll interval before clearing the config
             poll = (
                 self.config["daemon"]["poll"]
                 if self.config.get("daemon") is not None
                 and "poll" in self.config["daemon"]
                 else 60
             )
+
+            # Free any memory possible between daemon loops
+            self.clear()
+
+            # Wait for the next interval
             time_left = poll - (time.time() - start)
             if time_left > 0:
                 time.sleep(time_left)
             logger.debug("Sub-command `daemon` looping after %ss", time.time() - start)
 
     # Other methods
 
@@ -366,15 +371,15 @@
                     download_client,
                     download_client_method,
                 )():
                     removed_size = download_client.delete_files(download_item)
                     results.setdefault(
                         download_client_url,
                         [],
-                    ).append(download_item)
+                    ).append(download_item.hashString)
                     download_clients = self.free_space_download_clients()
                     break
                 if removed_size:
                     break
             else:
                 break
         return download_clients
@@ -450,7 +455,23 @@
             if wait:
                 while download_client.verifying_items:
                     time.sleep(1)
                     resumed_items.extend(download_client.resume_verified_items())
             if resumed_items:
                 resume_results[download_client_url] = resumed_items
         return resume_results
+
+    def clear(self):
+        """
+        Free any memory possible between daemon loops.
+        """
+        del self.config
+        self.servarrs.clear()
+        # Clear discreet download client caches to preserve verifying download items
+        for _, download_client in self.download_clients.items():
+            del download_client.config
+            del download_client.operations
+            del download_client.client
+            download_client.servarrs.clear()
+            del download_client.items
+        # Tell Python it's a good time to free memory
+        gc.collect()
```

### Comparing `prunerr-1.0.0/src/prunerr/servarr.py` & `prunerr-1.1.0b24/src/prunerr/servarr.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """
 Prunerr interaction with Servarr instances.
 """
 
 import dataclasses
 import time
-import datetime
 import urllib.parse
-import pathlib
 import logging
 
 import arrapi
 import arrapi.apis.base
 
 import prunerr.downloadclient
 import prunerr.downloaditem
+from .utils import pathlib
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class PrunerrServarrAPIClient:
     """
@@ -43,80 +42,53 @@
 
 class PrunerrServarrInstance:
     """
     An individual, specific Servarr instance that Prunerr interacts with.
     """
 
     # Map the different Servarr applications type terminology
-    TYPE_MAPS = dict(
-        sonarr=dict(
+    TYPE_MAPS = {
+        "sonarr": {
             # The top-level containing type, if applicable.  IOW, the type of items in
             # the top-level listing of the Servarr UI.  This is series for Sonarr as
             # contrasted with episode or season.  This is movie for Radarr.
-            dir_type="series",
+            "dir_type": "series",
             # File vs item is a little confusing.  Item refers to episodes/movies as
             # contrasted with the `dir_type`.  But an episode/movie may comprise of
             # multiple files and a file may contain multiple episodes.
-            item_type="episode",
-            file_has_multi=True,
-            client=arrapi.SonarrAPI,
-            download_dir_field="tvDirectory",
-            rename_template=(
+            "item_type": "episode",
+            "file_has_multi": True,
+            "client": arrapi.SonarrAPI,
+            "download_dir_field": "tvDirectory",
+            "rename_template": (
                 "{series[title]} - {episode[seasonEpisode]} - {episode[title]}"
             ),
-        ),
-        radarr=dict(
-            dir_type="movie",
-            item_type="movie",
-            file_has_multi=False,
-            client=arrapi.RadarrAPI,
-            download_dir_field="movieDirectory",
-            rename_template="{movie[title]} ({movie[release_year]})",
-        ),
-    )
-    EVENT_TYPES = {
-        "grabbed": 1,
-        "downloadFolderImported": 3,
-        "downloadIgnored": 7,
-        "downloadFailed": 4,
-        "fileDeleted": 5,
-        "fileRenamed": 6,
+        },
+        "radarr": {
+            "dir_type": "movie",
+            "item_type": "movie",
+            "file_has_multi": False,
+            "client": arrapi.RadarrAPI,
+            "download_dir_field": "movieDirectory",
+            "rename_template": "{movie[title]} ({movie[release_year]})",
+        },
     }
     MAX_PAGE_SIZE = 250
-    # Number of seconds to wait for new file import history records to appear in Servarr
-    # history.  This should be the maximum amount of time it might take to import a
-    # single file in the download client item, not necessarily the entire item.  Imagine
-    # how long might it take Sonarr to finish importing a download client item when:
-    #
-    # - Sonarr is configured to copy rather than making hard links
-    # - the host running Sonarr is under high load
-    # - the RAID array is being rebuilt
-    # - etc.
-    # TODO: Move to config
-    HISTORY_WAIT = datetime.timedelta(seconds=120)
 
     config = None
     client = None
     queue = None
 
     def __init__(self, runner):
         """
         Capture a references to the runner and individual Servarr configuration.
         """
         self.runner = runner
         self.download_clients = {}
 
-        # Initialize any data cached in instance state across updates
-        self.history = dict(
-            page=0,
-            records=dict(download_ids={}, source_titles={}),
-            event_types=dict(download_ids={}, source_titles={}),
-            dirs={},
-        )
-
     def __repr__(self):
         """
         Readable, informative, and specific representation to ease debugging.
         """
         return f"<{type(self).__name__} {self.config['name']!r}>"
 
     def update(self, config):
@@ -144,29 +116,24 @@
             "Requesting %s download clients settings",
             self.config["name"],
         )
         for download_client_config in self.client.get("downloadclient"):
             if (
                 not download_client_config["enable"]
                 or download_client_config["implementation"] != "Transmission"
-            ):
+            ):  # pragma: no cover
+                # BBB: Why misidentified as not covered under Python 3.9?
                 continue
             download_client_config = deserialize_servarr_download_client(
                 download_client_config,
             )
-            if download_client_config["url"] in self.download_clients:
-                # Preserve any cached state in existing download clients
-                download_clients[download_client_config["url"]] = self.download_clients[
-                    download_client_config["url"]
-                ]
-            else:
-                # Instantiate newly defined download clients
-                download_clients[
-                    download_client_config["url"]
-                ] = PrunerrServarrDownloadClient(self)
+            # Instantiate newly defined download clients
+            download_clients[
+                download_client_config["url"]
+            ] = PrunerrServarrDownloadClient(self)
             download_clients[download_client_config["url"]].update(
                 download_client_config
             )
         self.download_clients = download_clients
 
         # Update any data in instance state that should *not* be cached across updates
         self.queue = {
@@ -315,15 +282,15 @@
         # Update the download item's dir for subsequent operations, done manually to
         # minimize requests.
         for download_item in download_items:
             download_item._fields["downloadDir"] = download_item._fields[
                 "downloadDir"
             ]._replace(value=self.seeding_dir)
             vars(download_item).pop("path", None)
-        return download_items
+        return [download_item.hashString for download_item in download_items]
 
 
 def deserialize_servarr_download_client(download_client_config):
     """
     Assemble field values and a URL for a Servarr download client configuration.
     """
     download_client_config["fieldValues"] = {
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/Makefile` & `prunerr-1.1.0b24/src/prunerr/tests/Makefile`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/__init__.py` & `prunerr-1.1.0b24/src/prunerr/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 Tests for Prunerr.
 """
 
 import sys
 import os
 import functools
 import re
-import pathlib
-import subprocess
+import subprocess  # nosec B404
 import mimetypes
 import email.utils
 import email.message
 import urllib.parse
 import json
 import tempfile
 import shutil
 import unittest
 
 import yaml
 import requests_mock
 
 import prunerr
+from ..utils import pathlib
 
 
 def parse_content_type(content_type):  # pragma: no cover
     """
     Parse an RFC822-style `Content-Type` header.
 
     Useful to safely extract the MIME type from the charset.
@@ -38,15 +38,15 @@
 class PrunerrTestCase(
     unittest.TestCase
 ):  # pylint: disable=too-many-instance-attributes
     """
     Constants and set-up used in all Prunerr tests.
     """
 
-    maxDiff = None
+    maxDiff = None  # noqa: F841
 
     # HTTP methods taken from /usr/lib/python3.10/wsgiref/validate.py:340
     HTTP_METHODS_RE = re.compile("^(GET|HEAD|POST|OPTIONS|PATCH|PUT|DELETE|TRACE)")
 
     CONFIG = prunerr.runner.PrunerrRunner.EXAMPLE_CONFIG
     HOME = CONFIG.parents[1]
     ENV = {
@@ -96,15 +96,15 @@
         self.downloaded_dir = self.storage_dir / self.DOWNLOADED_DIR_BASENAME
         self.seeding_dir = (
             self.storage_dir
             / prunerr.downloadclient.PrunerrDownloadClient.SEEDING_DIR_BASENAME
         )
 
         # Convenient access to the parsed configuration file
-        with self.CONFIG.open() as config_opened:
+        with self.CONFIG.open(encoding="utf-8") as config_opened:
             self.config = yaml.safe_load(config_opened)
         if "download-clients" in self.config:
             self.min_free_space = prunerr.downloadclient.calc_free_space_margin(
                 self.config,
             )
         # Convenient access to parsed mocked API/RPC request responses
         self.servarr_download_client_responses = {}
@@ -322,47 +322,47 @@
                     ),
                 ),
             )
             url_path_split = urllib.parse.urlsplit(
                 str(url_unquoted_path.relative_to(url_unquoted_path.parents[-3])),
             )
             url_split = urllib.parse.SplitResult(
-                scheme=url_unquoted_path.parents[-2].name,  # pylint: disable=no-member
-                netloc=url_unquoted_path.parents[-3].name,  # pylint: disable=no-member
+                scheme=url_unquoted_path.parents[-2].name,
+                netloc=url_unquoted_path.parents[-3].name,
                 path=url_path_split.path,
                 query=url_path_split.query,
                 fragment=url_path_split.fragment,
             )
 
             responses = {}
             for response_path in sorted(
                 request_headers_path.parent.glob("*/response.json"),
             ):
                 if response_path.name.endswith("~"):  # pragma: no cover
                     # Ignore backup files
                     continue
-                response_mock = dict(
-                    response_dir=response_path.parent.relative_to(
+                response_mock = {
+                    "response_dir": response_path.parent.relative_to(
                         pathlib.Path().resolve(),
                     ),
-                    headers={},
-                )
+                    "headers": {},
+                }
 
                 # Assemble headers from the file metadata
                 response_stat = response_path.stat()
                 response_mock["headers"]["Last-Modified"] = email.utils.formatdate(
                     timeval=response_stat.st_mtime,
                     usegmt=True,
                 )
                 response_mock["headers"]["Content-Type"] = mimetypes.guess_type(
                     response_path.name
                 )[0]
 
                 # Optionally read the expected response JSON from a sibling file
-                response_mock["request"] = dict(json={})
+                response_mock["request"] = {"json": {}}
                 request_json_path = response_path.parent / "request.json"
                 if request_json_path.exists():
                     with request_json_path.open() as request_json_opened:
                         response_mock["request"]["json"] = self.patch_paths(
                             json.load(request_json_opened),
                         )
 
@@ -380,27 +380,30 @@
                 .get(
                     method,
                     {},
                 )
                 .items()
             ):
                 mock_kwargs["from_mock_dir"] = responses[mock_order]
-                responses[mock_order] = responses[mock_order] | mock_kwargs
+                responses[mock_order] = dict(
+                    responses[mock_order],
+                    **mock_kwargs,
+                )
 
             # Use the callback to make assertions on the request bodies
             response_list = []
             for mock_order in sorted(responses.keys()):
                 response_list.append(
-                    dict(
-                        headers=responses[mock_order]["headers"],
-                        json=functools.partial(
+                    {
+                        "headers": responses[mock_order]["headers"],
+                        "json": functools.partial(
                             self.mock_response_callback,
                             responses[mock_order],
                         ),
-                    ),
+                    },
                 )
 
             with request_headers_path.open() as request_headers_opened:
                 request_headers = json.load(request_headers_opened)
             request_mocks.setdefault(url_split.geturl(), {})[method] = (
                 self.requests_mock.register_uri(
                     method=method,
@@ -421,14 +424,16 @@
             for request_mock, mock_responses in methods.values():
                 self.assert_request_mock(request_mock, mock_responses)
 
     def assert_request_mock(self, request_mock, mock_responses):  # pragma: no cover
         """
         Assert that one request mock has been called once for each response.
         """
+        mock_method = request_mock._method  # pylint: disable=protected-access
+        mock_url = request_mock._url  # pylint: disable=protected-access
         if request_mock.call_count < len(mock_responses):
             response_contents = []
             for response_params in mock_responses.values():
                 response_content = response_params.get(
                     "json",
                     response_params.get("text", response_params.get("content")),
                 )
@@ -440,17 +445,15 @@
                     )
                     if minor_type.lower() == "json":
                         response_content = json.loads(response_content)
                 response_contents.append(response_content)
             self.assertEqual(
                 response_contents,
                 response_contents[: request_mock.call_count],
-                "Some response mocks not called: "
-                f"{request_mock._method} "  # pylint: disable=protected-access
-                f"{request_mock._url}",  # pylint: disable=protected-access
+                f"Some response mocks not called: {mock_method} {mock_url}",
             )
         elif request_mock.call_count > len(mock_responses):
             request_contents = []
             for mock_call in request_mock.request_history:
                 request_content = mock_call.text
                 if "Accept" in mock_call.headers:
                     _, minor_type = parse_content_type(
@@ -458,17 +461,15 @@
                     )
                     if minor_type.lower() == "json":
                         request_content = mock_call.json()
                 request_contents.append(request_content)
             self.assertEqual(
                 request_contents[: len(mock_responses)],
                 request_contents,
-                "More requests than mocks: "
-                f"{request_mock._method} "  # pylint: disable=protected-access
-                f"{request_mock._url}",  # pylint: disable=protected-access
+                f"More requests than mocks: {mock_method} {mock_url}",
             )
 
     def mock_download_client_complete_item(
         self,
     ):
         """
         Simulate the download client finishing a download by moving the item.
@@ -480,25 +481,25 @@
 
     def mock_move_torrent_response(
         self,
         request=None,
         context=None,
         response_mock=None,
         delay=0,
-    ):  # pylint: disable=unused-argument
+    ):
         """
         Simulate the download client changing a download items location.
         """
         location = pathlib.Path(request.json()["arguments"]["location"])
         location.mkdir(parents=True, exist_ok=True)
         dst = location / self.downloaded_item.name
         if delay:
             # Simulate a delay using a subprocess
             self.addCleanup(
-                subprocess.Popen(  # pylint: disable=consider-using-with
+                subprocess.Popen(  # nosec B603, pylint: disable=consider-using-with
                     args=[
                         sys.executable,
                         "-c",
                         "import pathlib; "
                         f"import time; time.sleep({delay}); "
                         f"pathlib.Path('{self.downloaded_item}').rename('{dst}');",
                     ],
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/example-5s.mkv` & `prunerr-1.1.0b24/src/prunerr/tests/example-5s.mkv`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/home/daemon/.config/prunerr.yml` & `prunerr-1.1.0b24/src/prunerr/tests/home/download-clients/.config/prunerr.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-daemon:
-  # Cover the `time.sleep(1)` part of the `daemon` loop.
-  poll: 1
 servarrs:
   Sonarr:
     url: "http://localhost:8989"
     api-key: ""
     type: "sonarr"
   Radarr:
     url: "http://localhost:7878"
     api-key: ""
     type: "radarr"
 download-clients:
+  urls:
+    - "https://transmission.example.com"
+    - "https://transmission.foo.example.com"
   max-download-bandwidth: 100
   min-download-time-margin: 600
 indexers:
   hostnames:
     ExamplePrivateTracker:
-      - "tracker.example.com"
+      - "https://tracker.example.com"
   reviews:
     - name: "ExamplePrivateTracker"
       operations:
         - type: "or"
           operations:
             - type: "value"
               name: "status"
               equals: "seeding"
             - type: "value"
               name: "age"
               maximum: 604800
             - type: "value"
+              name: "seconds_downloading"
+              maximum: 0
+            - type: "value"
               name: "rate_total"
               minimum: 50
           remove: true
           blacklist: true
         - type: "files"
           patterns:
             - ".+\\.rar$"
@@ -57,14 +60,17 @@
             - type: "value"
               name: "status"
               equals: "seeding"
             - type: "value"
               name: "age"
               maximum: 604800
             - type: "value"
+              name: "seconds_downloading"
+              maximum: 0
+            - type: "value"
               name: "rate_total"
               minimum: 50
           remove: true
           blacklist: true
         - type: "files"
           patterns:
             - ".+\\.rar$"
@@ -90,30 +96,20 @@
           operations:
             - type: "value"
               name: "seconds_since_done"
               minimum: 864000
             - type: "value"
               name: "ratio"
               minimum: 1.0
-        - type: "files"
-          name: "size_imported"
-          aggregation: "portion"
-          reversed: true
-          filter: true
-          minimum: 0.9
         - type: "value"
           name: "uploadedEver"
           reversed: true
         - type: "value"
           name: "size_when_done"
           minimum: 10737418240
           reversed: true
         - type: "value"
           name: "size_when_done"
     - name: null
       operations:
-        - type: "files"
-          name: "size_imported"
-          aggregation: "portion"
-          reversed: true
         - type: "value"
           name: "ratio"
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/home/download-clients/.config/prunerr.yml` & `prunerr-1.1.0b24/src/prunerr/tests/home/daemon/.config/prunerr.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,41 @@
+daemon:
+  # Cover the `time.sleep(1)` part of the `daemon` loop.
+  poll: 1
 servarrs:
   Sonarr:
     url: "http://localhost:8989"
     api-key: ""
     type: "sonarr"
   Radarr:
     url: "http://localhost:7878"
     api-key: ""
     type: "radarr"
 download-clients:
-  urls:
-    - "https://transmission.example.com"
-    - "https://transmission.foo.example.com"
   max-download-bandwidth: 100
   min-download-time-margin: 600
 indexers:
   hostnames:
     ExamplePrivateTracker:
-      - "https://tracker.example.com"
+      - "tracker.example.com"
   reviews:
     - name: "ExamplePrivateTracker"
       operations:
         - type: "or"
           operations:
             - type: "value"
               name: "status"
               equals: "seeding"
             - type: "value"
               name: "age"
               maximum: 604800
             - type: "value"
+              name: "seconds_downloading"
+              maximum: 0
+            - type: "value"
               name: "rate_total"
               minimum: 50
           remove: true
           blacklist: true
         - type: "files"
           patterns:
             - ".+\\.rar$"
@@ -57,14 +60,17 @@
             - type: "value"
               name: "status"
               equals: "seeding"
             - type: "value"
               name: "age"
               maximum: 604800
             - type: "value"
+              name: "seconds_downloading"
+              maximum: 0
+            - type: "value"
               name: "rate_total"
               minimum: 50
           remove: true
           blacklist: true
         - type: "files"
           patterns:
             - ".+\\.rar$"
@@ -90,20 +96,30 @@
           operations:
             - type: "value"
               name: "seconds_since_done"
               minimum: 864000
             - type: "value"
               name: "ratio"
               minimum: 1.0
+        - type: "files"
+          name: "size_imported"
+          aggregation: "portion"
+          reversed: true
+          filter: true
+          minimum: 0.9
         - type: "value"
           name: "uploadedEver"
           reversed: true
         - type: "value"
           name: "size_when_done"
           minimum: 10737418240
           reversed: true
         - type: "value"
           name: "size_when_done"
     - name: null
       operations:
+        - type: "files"
+          name: "size_imported"
+          aggregation: "portion"
+          reversed: true
         - type: "value"
           name: "ratio"
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml` & `prunerr-1.1.0b24/src/prunerr/tests/home/review-edge-cases/.config/prunerr.yml`

 * *Files 13% similar despite different names*

```diff
@@ -19,13 +19,16 @@
             - type: "value"
               name: "status"
               equals: "seeding"
             - type: "value"
               name: "age"
               maximum: 604800
             - type: "value"
+              name: "seconds_downloading"
+              maximum: 0
+            - type: "value"
               name: "rate_total"
               minimum: 50
           remove: true
         - type: "value"
           name: "bandwidthPriority"
           equals: 1
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/1-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/2-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/daemon/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/default/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-client-only/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/192.168.1.2%3A80/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/http/transmission%40192.168.1.1%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-clients/https/transmission.foo.example.com%3A443/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/download-items/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-imported-sufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-orphans/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/02-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-remaining/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-unregistered/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/free-space-upgraded-insufficient/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-completed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-deleted/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-grabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-import/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/history%3Fapikey%3D%26pageSize%3D250%26page%3D1%26downloadId%3D1FAFED76F4264B14934C13D7A306F94FEA4B3184/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-imported-before/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/move-ungrabbed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-downloading/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/07-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9568452380952381%*

 * *Differences: {"'arguments'": "{'torrents': {0: {'bandwidthPriority': 1, 'magnetLink': "*

 * *                "'magnet:?xt=urn:btih:909C9B954B414A87B1DCF6E2FB09650FCC35DE57&dn=Bar.Movie.1980.WEB-DL.x265.HEVC-RELEASER&tr=https%3A%2F%2Ftracker.private.example.com%2Fa%2F1fafed76f4264b14934c13d7a306f94fea4b3184%2Fannounce', "*

 * *                "'torrentFile': "*

 * *                "'/config/torrents/909C9B954B414A87B1DCF6E2FB09650FCC35DE57.torrent'}, 1: "*

 * *                "{'bandwidthPriority': 1, 'status': 4}, delete: [0]}}"}*

```diff
@@ -1,180 +1,14 @@
 {
     "arguments": {
         "torrents": [
             {
                 "activityDate": 0,
                 "addedDate": 0,
-                "bandwidthPriority": 0,
-                "comment": "",
-                "corruptEver": 0,
-                "creator": "",
-                "dateCreated": 0,
-                "desiredAvailable": 0,
-                "doneDate": 0,
-                "downloadDir": "/media/Library/downloads/Sonarr/Videos/Series/",
-                "downloadLimit": 0,
-                "downloadLimited": false,
-                "downloadedEver": 2145386496,
-                "editDate": 0,
-                "error": 0,
-                "errorString": "",
-                "eta": -1,
-                "etaIdle": -1,
-                "fileStats": [
-                    {
-                        "bytesCompleted": 2145386496,
-                        "priority": 0,
-                        "wanted": true
-                    }
-                ],
-                "files": [
-                    {
-                        "bytesCompleted": 2145386496,
-                        "length": 2147483648,
-                        "name": "Foo.Series.1970.S01E02.Grault.Episode.Title.WEB-DL.x265.HEVC-RELEASER.mkv"
-                    }
-                ],
-                "hashString": "72D08E64D0FE455A9ECE08AED0BB646D2632D339",
-                "haveUnchecked": 0,
-                "haveValid": 2145386496,
-                "honorsSessionLimits": true,
-                "id": 3,
-                "isFinished": false,
-                "isPrivate": false,
-                "isStalled": true,
-                "labels": [],
-                "leftUntilDone": 2097152,
-                "magnetLink": "magnet:?xt=urn:btih:72D08E64D0FE455A9ECE08AED0BB646D2632D339&dn=Foo.Series.1970.S01E02.Grault.Episode.Title.WEB-DL.x265.HEVC-RELEASER.mkv&tr=https%3A%2F%2Ftracker.private.example.com%2Fa%2F72d08e64d0fe455a9ece08aed0bb646d2632d339%2Fannounce",
-                "manualAnnounceTime": -1,
-                "maxConnectedPeers": 288,
-                "metadataPercentComplete": 1,
-                "name": "Foo.Series.1970.S01E02.Grault.Episode.Title.WEB-DL.x265.HEVC-RELEASER.mkv",
-                "peer-limit": 288,
-                "peers": [],
-                "peersConnected": 0,
-                "peersFrom": {
-                    "fromCache": 0,
-                    "fromDht": 0,
-                    "fromIncoming": 0,
-                    "fromLpd": 0,
-                    "fromLtep": 0,
-                    "fromPex": 0,
-                    "fromTracker": 0
-                },
-                "peersGettingFromUs": 0,
-                "peersSendingToUs": 0,
-                "percentDone": 0.09,
-                "pieceCount": 10000,
-                "pieceSize": 107269,
-                "pieces": "//////////////////////////////////////////////////////////////////",
-                "priorities": [
-                    0
-                ],
-                "queuePosition": 1,
-                "rateDownload": 0,
-                "rateUpload": 0,
-                "recheckProgress": 0,
-                "secondsDownloading": 600,
-                "secondsSeeding": 60000,
-                "seedIdleLimit": 30,
-                "seedIdleMode": 0,
-                "seedRatioLimit": 4,
-                "seedRatioMode": 0,
-                "sizeWhenDone": 2147483648,
-                "startDate": 0,
-                "status": 4,
-                "torrentFile": "/config/torrents/72D08E64D0FE455A9ECE08AED0BB646D2632D339.torrent",
-                "totalSize": 2147483648,
-                "trackerStats": [
-                    {
-                        "announce": "udp://tracker.private.example.com:6969/announce",
-                        "announceState": 2,
-                        "downloadCount": -1,
-                        "hasAnnounced": true,
-                        "hasScraped": false,
-                        "host": "udp://tracker.private.example.com:6969",
-                        "id": 0,
-                        "isBackup": false,
-                        "lastAnnouncePeerCount": 0,
-                        "lastAnnounceResult": "Success",
-                        "lastAnnounceStartTime": 0,
-                        "lastAnnounceSucceeded": true,
-                        "lastAnnounceTime": 0,
-                        "lastAnnounceTimedOut": false,
-                        "lastScrapeResult": "",
-                        "lastScrapeStartTime": 0,
-                        "lastScrapeSucceeded": false,
-                        "lastScrapeTime": 0,
-                        "lastScrapeTimedOut": false,
-                        "leecherCount": 0,
-                        "nextAnnounceTime": 0,
-                        "nextScrapeTime": 0,
-                        "scrape": "udp://tracker.private.example.com:6969/scrape",
-                        "scrapeState": 2,
-                        "seederCount": 0,
-                        "tier": 0
-                    },
-                    {
-                        "announce": "udp://tracker.private.example.com:6969/announce",
-                        "announceState": 0,
-                        "downloadCount": -1,
-                        "hasAnnounced": false,
-                        "hasScraped": false,
-                        "host": "udp://tracker.private.example.com:6969",
-                        "id": 1,
-                        "isBackup": true,
-                        "lastAnnouncePeerCount": 0,
-                        "lastAnnounceResult": "",
-                        "lastAnnounceStartTime": 0,
-                        "lastAnnounceSucceeded": false,
-                        "lastAnnounceTime": 0,
-                        "lastAnnounceTimedOut": false,
-                        "lastScrapeResult": "",
-                        "lastScrapeStartTime": 0,
-                        "lastScrapeSucceeded": false,
-                        "lastScrapeTime": 0,
-                        "lastScrapeTimedOut": false,
-                        "leecherCount": -1,
-                        "nextAnnounceTime": 0,
-                        "nextScrapeTime": 0,
-                        "scrape": "udp://tracker.private.example.com:6969/scrape",
-                        "scrapeState": 0,
-                        "seederCount": -1,
-                        "tier": 0
-                    }
-                ],
-                "trackers": [
-                    {
-                        "announce": "udp://tracker.private.example.com:6969/announce",
-                        "id": 0,
-                        "scrape": "udp://tracker.private.example.com:6969/scrape",
-                        "tier": 0
-                    },
-                    {
-                        "announce": "udp://tracker.private.example.com:6969/announce",
-                        "id": 1,
-                        "scrape": "udp://tracker.private.example.com:6969/scrape",
-                        "tier": 0
-                    }
-                ],
-                "uploadLimit": 10240,
-                "uploadLimited": false,
-                "uploadRatio": 1.5,
-                "uploadedEver": 2147483648,
-                "wanted": [
-                    1
-                ],
-                "webseeds": [],
-                "webseedsSendingToUs": 0
-            },
-            {
-                "activityDate": 0,
-                "addedDate": 0,
-                "bandwidthPriority": 0,
+                "bandwidthPriority": 1,
                 "comment": "",
                 "corruptEver": 0,
                 "creator": "",
                 "dateCreated": 0,
                 "desiredAvailable": 0,
                 "doneDate": 0,
                 "downloadDir": "/media/Library/downloads/Radarr/Videos/Movies/",
@@ -206,15 +40,15 @@
                 "honorsSessionLimits": true,
                 "id": 2,
                 "isFinished": false,
                 "isPrivate": true,
                 "isStalled": true,
                 "labels": [],
                 "leftUntilDone": 1048576,
-                "magnetLink": "magnet:?xt=urn:btih:1FAFED76F4264B14934C13D7A306F94FEA4B3184&dn=Bar.Movie.1980.WEB-DL.x265.HEVC-RELEASER&tr=https%3A%2F%2Ftracker.private.example.com%2Fa%2F1fafed76f4264b14934c13d7a306f94fea4b3184%2Fannounce",
+                "magnetLink": "magnet:?xt=urn:btih:909C9B954B414A87B1DCF6E2FB09650FCC35DE57&dn=Bar.Movie.1980.WEB-DL.x265.HEVC-RELEASER&tr=https%3A%2F%2Ftracker.private.example.com%2Fa%2F1fafed76f4264b14934c13d7a306f94fea4b3184%2Fannounce",
                 "manualAnnounceTime": -1,
                 "maxConnectedPeers": 288,
                 "metadataPercentComplete": 1,
                 "name": "Bar.Movie.1980.WEB-DL.x265.HEVC-RELEASER",
                 "peer-limit": 288,
                 "peers": [],
                 "peersConnected": 0,
@@ -245,15 +79,15 @@
                 "seedIdleLimit": 30,
                 "seedIdleMode": 0,
                 "seedRatioLimit": 4,
                 "seedRatioMode": 0,
                 "sizeWhenDone": 1073741824,
                 "startDate": 0,
                 "status": 4,
-                "torrentFile": "/config/torrents/1FAFED76F4264B14934C13D7A306F94FEA4B3184.torrent",
+                "torrentFile": "/config/torrents/909C9B954B414A87B1DCF6E2FB09650FCC35DE57.torrent",
                 "totalSize": 1073741824,
                 "trackerStats": [
                     {
                         "announce": "udp://tracker.private.example.com:6969/announce",
                         "announceState": 2,
                         "downloadCount": -1,
                         "hasAnnounced": true,
@@ -332,15 +166,15 @@
                 ],
                 "webseeds": [],
                 "webseedsSendingToUs": 0
             },
             {
                 "activityDate": 0,
                 "addedDate": 0,
-                "bandwidthPriority": 0,
+                "bandwidthPriority": 1,
                 "comment": "",
                 "corruptEver": 0,
                 "creator": "",
                 "dateCreated": 0,
                 "desiredAvailable": 0,
                 "doneDate": 0,
                 "downloadDir": "/media/Library/downloads/Sonarr/Videos/Series/",
@@ -410,15 +244,15 @@
                 "secondsSeeding": 60000,
                 "seedIdleLimit": 30,
                 "seedIdleMode": 0,
                 "seedRatioLimit": 4,
                 "seedRatioMode": 0,
                 "sizeWhenDone": 1073741824,
                 "startDate": 0,
-                "status": 6,
+                "status": 4,
                 "torrentFile": "/config/torrents/1FAFED76F4264B14934C13D7A306F94FEA4B3184.torrent",
                 "totalSize": 1073741824,
                 "trackerStats": [
                     {
                         "announce": "udp://tracker.private.example.com:6969/announce",
                         "announceState": 2,
                         "downloadCount": -1,
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-edge-cases/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/05-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/review-reviewed/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A7878/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/downloadclient%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/queue%3Fapikey%3D%26pageSize%3D250%26page%3D1/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/localhost%3A8989/api/v3/system/status%3Fapikey%3D/GET/0-response/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/00-session-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/01-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/03-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/request.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json` & `prunerr-1.1.0b24/src/prunerr/tests/responses/verify/http/transmission%3Asecret%40localhost%3A9091/transmission/rpc/POST/04-torrent-get/response.json`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_cli.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Test the Prunerr Command-Line Interface.
 """
 
 import sys
 import os
 import io
-import subprocess
+import runpy
+import subprocess  # nosec B404
 import contextlib
 import pathlib
 
 from unittest import mock
 
 import prunerr
 
@@ -22,15 +23,15 @@
     Test the prunerr Command-Line Interface.
     """
 
     def test_importable(self):
         """
         The Python package is on `sys.path` and thus importable.
         """
-        import_process = subprocess.run(
+        import_process = subprocess.run(  # nosec B603
             [sys.executable, "-c", "import prunerr"],
             check=False,
         )
         self.assertEqual(
             import_process.returncode,
             0,
             "The Python package not importable",
@@ -74,15 +75,17 @@
 
     def test_cli_options(self):
         """
         The command line script accepts options controlling behavior.
         """
         request_mocks = self.mock_responses()
         self.assertIsNone(
-            prunerr.main(args=[f"--config={self.CONFIG}", "exec"]),
+            prunerr.main(
+                args=["--log-level", "DEBUG", f"--config={self.CONFIG}", "exec"],
+            ),
             "Wrong console script options return value",
         )
         self.assert_request_mocks(request_mocks)
 
     def test_cli_option_errors(self):
         """
         The command line script displays useful messages for invalid option values.
@@ -96,40 +99,52 @@
         )
         self.assertIn(
             "error: unrecognized arguments: --non-existent-option",
             stderr,
             "Wrong invalid option message",
         )
 
-    def test_cli_module_main(self):
+    def test_cli_dash_m_option(self):
         """
-        The package/module supports execution via Python's `-m` option.
+        The package supports execution via Python's `-m` CLI option.
         """
-        module_main_process = subprocess.run(
+        module_main_process = subprocess.run(  # nosec B603
             [sys.executable, "-m", "prunerr", "exec", "--help"],
             check=False,
         )
         self.assertEqual(
             module_main_process.returncode,
             0,
             "Running via Python's `-m` option exited with non-zero status code",
         )
 
+    def test_cli_module_main(self):
+        """
+        The package supports execution via Python's `-m` option.
+        """
+        with self.assertRaises(SystemExit, msg="CLI didn't exit") as exc_context:
+            runpy.run_module("prunerr")
+        self.assertEqual(
+            exc_context.exception.code,
+            2,
+            "Wrong `runpy` exit status code",
+        )
+
     def test_cli_exit_code(self):
         """
         The command line script exits with status code zero if there are no exceptions.
         """
         # Find the location of the `console_scripts` for this test environment
         prefix_path = pathlib.Path(sys.argv[0]).parent
         while not (prefix_path / "bin").is_dir():
             prefix_path = prefix_path.parent
-            if prefix_path.parent is prefix_path.parents[-1]:  # pragma: no cover
+            if prefix_path.parent is list(prefix_path.parents)[-1]:  # pragma: no cover
                 raise ValueError(f"Could not find script prefix path: {sys.argv[0]}")
 
-        script_process = subprocess.run(
+        script_process = subprocess.run(  # nosec B603
             [prefix_path / "bin" / "prunerr", "exec", "--help"],
             check=False,
         )
         self.assertEqual(
             script_process.returncode,
             0,
             "Running the console script exited with non-zero status code",
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_daemon.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_daemon.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,26 +48,26 @@
         return response_mock["from_mock_dir"]["json"]
 
     def mock_network_retry_response(
         self,
         request=None,
         context=None,
         response_mock=None,
-    ):  # pylint: disable=unused-argument
+    ):
         """
         Raise an exception while running `exec` that `daemon` catches.
         """
         raise socket.error("Temporary network connection error")
 
     def mock_exit_daemon_response(
         self,
         request=None,
         context=None,
         response_mock=None,
-    ):  # pylint: disable=unused-argument
+    ):
         """
         Simulate an exception to exit the `daemon` sub-command.
         """
         raise PrunerrDaemonTestException("Exit the daemon loop")
 
     def test_daemon_command(self):
         """
@@ -75,25 +75,25 @@
         """
         daemon_request_mocks = self.mock_responses(
             self.RESPONSES_DIR,
             # Insert a dynamic response mock to add recent dates
             {
                 "http://transmission:secret@localhost:9091/transmission/rpc": {
                     "POST": {
-                        "01-torrent-get": dict(json=self.mock_poll_delay_response),
+                        "01-torrent-get": {"json": self.mock_poll_delay_response},
                     },
                 },
                 "http://localhost:8989/api/v3/queue/1?apikey=&blacklist=true": {
                     "DELETE": {
-                        "0-response": dict(json=self.mock_network_retry_response),
+                        "0-response": {"json": self.mock_network_retry_response},
                     },
                 },
                 "http://localhost:8989/api/v3/system/status?apikey=": {
                     "GET": {
-                        "2-response": dict(json=self.mock_exit_daemon_response),
+                        "2-response": {"json": self.mock_exit_daemon_response},
                     },
                 },
             },
         )
         with self.assertRaises(
             PrunerrDaemonTestException,
             msg="Daemon loop exited with wrong exception",
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_downloadclient.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_downloadclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             .download_clients[self.SERVARR_DOWNLOAD_CLIENT_URLS[0]]
             .download_client.client,
             "Download client's RPC client not re-used across Servarr instances",
         )
 
     def assert_download_client(self, runner, download_client_url):
         """
-        An individual download client is configured correctly.
+        Confirm that an individual download client is configured correctly.
         """
         self.assertIn(
             download_client_url,
             runner.download_clients,
             "Aggregated download clients missing URL",
         )
         download_client = runner.download_clients[download_client_url]
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_downloaditem.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_downloaditem.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_free_space.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_free_space.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_move.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_move.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Test moving download items that Servarr has acted on.
     """
 
     RESPONSES_DIR = tests.PrunerrTestCase.RESPONSES_DIR.parent / "move-ungrabbed"
 
     def test_move_usual_lifecycle(
         self,
-    ):  # pylint: disable=too-many-statements,too-many-locals
+    ):  # pylint: disable=too-many-statements
         """
         Download items are moved to `seeding` when imported by Servarr.
         """
         # 0. Verify initial assumptions and conditions
         self.assertTrue(
             self.incomplete_item.is_dir(),
             "Download item is not a directory while downloading",
@@ -210,20 +210,20 @@
         #    moved from `downloads` to `seeding`.
         import_request_mocks = self.mock_responses(
             tests.PrunerrTestCase.RESPONSES_DIR.parent / "move-import",
             # Insert a dynamic response mock to handle moving imported download items
             {
                 "http://transmission:secret@localhost:9091/transmission/rpc": {
                     "POST": {
-                        "02-torrent-set-location": dict(
-                            json=functools.partial(
+                        "02-torrent-set-location": {
+                            "json": functools.partial(
                                 self.mock_move_torrent_response,
                                 delay=1,
                             ),
-                        ),
+                        },
                     },
                 },
             },
         )
         prunerr.main(args=[f"--config={self.CONFIG}", "move"])
         self.assert_request_mocks(import_request_mocks)
         self.assertFalse(
@@ -320,17 +320,17 @@
         self.mock_servarr_import_item()
         imported_before_request_mocks = self.mock_responses(
             tests.PrunerrTestCase.RESPONSES_DIR.parent / "move-imported-before",
             # Insert a dynamic response mock to handle moving imported download items
             {
                 "http://transmission:secret@localhost:9091/transmission/rpc": {
                     "POST": {
-                        "02-torrent-set-location": dict(
-                            json=self.mock_move_torrent_response,
-                        ),
+                        "02-torrent-set-location": {
+                            "json": self.mock_move_torrent_response,
+                        },
                     },
                 },
             },
         )
         prunerr.main(args=[f"--config={self.CONFIG}", "move"])
         self.assert_request_mocks(imported_before_request_mocks)
         self.assertFalse(
@@ -370,17 +370,17 @@
         )
         self.mock_responses(
             tests.PrunerrTestCase.RESPONSES_DIR.parent / "move-import",
             # Insert a dynamic response mock to handle moving imported download items
             {
                 "http://transmission:secret@localhost:9091/transmission/rpc": {
                     "POST": {
-                        "02-torrent-set-location": dict(
-                            json=self.mock_move_torrent_response,
-                        ),
+                        "02-torrent-set-location": {
+                            "json": self.mock_move_torrent_response,
+                        },
                     },
                 },
             },
         )
         runner.update()
         exec_results = runner.exec_()
         self.assertIn(
@@ -420,20 +420,20 @@
         runner = prunerr.runner.PrunerrRunner(config=self.CONFIG)
         self.mock_responses(
             tests.PrunerrTestCase.RESPONSES_DIR.parent / "move-import",
             # Insert a dynamic response mock to handle moving imported download items
             {
                 "http://transmission:secret@localhost:9091/transmission/rpc": {
                     "POST": {
-                        "02-torrent-set-location": dict(
-                            json=functools.partial(
+                        "02-torrent-set-location": {
+                            "json": functools.partial(
                                 self.mock_move_torrent_response,
                                 delay=1,
                             ),
-                        ),
+                        },
                     },
                 },
             },
         )
         runner.update()
         servarr = list(runner.servarrs.values())[0]
         with self.assertRaises(
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_operations.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Test Prunerr's configurable operations.
     """
 
     HOME = test_downloaditem.PrunerrDownloadItemTests.HOME
     CONFIG = test_downloaditem.PrunerrDownloadItemTests.CONFIG
     RESPONSES_DIR = test_downloaditem.PrunerrDownloadItemTests.RESPONSES_DIR
 
-    def setUp(self):
+    def setUp(self):  # pylint: disable=invalid-name
         """
         Assemble the components required to run operations.
         """
         super().setUp()
 
         runner = prunerr.runner.PrunerrRunner(config=self.CONFIG)
         runner.config = self.config
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_review.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_review.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         #    torrents, one from a private indexer and one from a public indexer.
         downloading_request_mocks = self.mock_responses(
             self.RESPONSES_DIR,
             # Insert a dynamic response mock to add recent dates
             {
                 "http://transmission:secret@localhost:9091/transmission/rpc": {
                     "POST": {
-                        "01-torrent-get": dict(
-                            json=functools.partial(
+                        "01-torrent-get": {
+                            "json": functools.partial(
                                 self.mock_get_torrent_response,
                                 [
                                     {},
                                     {
                                         "addedDate": (
                                             datetime.datetime.now()
                                             - datetime.timedelta(days=1)
@@ -50,15 +50,15 @@
                                         "addedDate": (
                                             datetime.datetime.now()
                                             - datetime.timedelta(days=1)
                                         ).timestamp()
                                     },
                                 ],
                             ),
-                        ),
+                        },
                     },
                 },
             },
         )
         downloading_before_torrents = downloading_request_mocks[
             "http://transmission:secret@localhost:9091/transmission/rpc"
         ]["POST"][1]["01-torrent-get"]["from_mock_dir"]["json"]["arguments"]["torrents"]
@@ -160,31 +160,31 @@
         # made, no further changes are made.
         reviewed_request_mocks = self.mock_responses(
             self.RESPONSES_DIR.parent / "review-reviewed",
             # Insert a dynamic response mock to add recent dates
             {
                 "http://transmission:secret@localhost:9091/transmission/rpc": {
                     "POST": {
-                        "01-torrent-get": dict(
-                            json=functools.partial(
+                        "01-torrent-get": {
+                            "json": functools.partial(
                                 self.mock_get_torrent_response,
                                 [
                                     {
                                         "addedDate": (
                                             datetime.datetime.now()
                                         ).timestamp()
                                     },
                                     {
                                         "addedDate": (
                                             datetime.datetime.now()
                                         ).timestamp()
                                     },
                                 ],
                             ),
-                        ),
+                        },
                     },
                 },
             },
         )
         prunerr.main(args=[f"--config={self.CONFIG}", "review"])
         self.assert_request_mocks(reviewed_request_mocks)
         (private_indexer_reviewed_torrent, _) = reviewed_request_mocks[
@@ -222,26 +222,63 @@
             "The seeding items directory exists before Servarr import",
         )
 
     def test_review_edge_cases(self):
         """
         Review of a download item without a queue record logs a warning.
 
-        Also covers deleting download item without a blacklisting it and a review
-        without any configured change in the request mock assertions.
+        Also covers deleting download item without a blacklisting it, a review
+        without any configured change in the request mock assertions, and nonsensical
+        item timestamps.
         """
         runner = prunerr.runner.PrunerrRunner(
             config=pathlib.Path(__file__).parent
             / "home"
             / "review-edge-cases"
             / ".config"
             / "prunerr.yml",
         )
         self.mock_responses(
             self.RESPONSES_DIR.parent / "review-edge-cases",
+            # Insert a dynamic response mock to nonsensical dates
+            {
+                "http://transmission:secret@localhost:9091/transmission/rpc": {
+                    "POST": {
+                        "01-torrent-get": {
+                            "json": functools.partial(
+                                self.mock_get_torrent_response,
+                                [
+                                    {},
+                                    {},
+                                    {},
+                                    {
+                                        # Done date is before added date
+                                        "addedDate": (
+                                            datetime.datetime.now()
+                                            - datetime.timedelta(days=1)
+                                        ).timestamp(),
+                                        "doneDate": (
+                                            datetime.datetime.now()
+                                            - datetime.timedelta(days=2)
+                                        ).timestamp(),
+                                    },
+                                    {
+                                        # Added date is in the future
+                                        "addedDate": (
+                                            datetime.datetime.now()
+                                            + datetime.timedelta(days=1)
+                                        ).timestamp(),
+                                        "doneDate": 0,
+                                    },
+                                ],
+                            ),
+                        },
+                    },
+                },
+            },
         )
         runner.update()
         with self.assertLogs(
             prunerr.downloaditem.logger,
             level=logging.WARNING,
         ) as logged_msgs:
             runner.review()
@@ -263,12 +300,21 @@
             / "prunerr.yml",
         )
         runner.quiet = True
         self.mock_responses(
             self.RESPONSES_DIR.parent / "review-edge-cases",
         )
         runner.update()
-        with self.assertNoLogs(
-            prunerr.downloaditem.logger,
-            level=logging.WARNING,
-        ):
-            runner.review()
+        if hasattr(self, "assertNoLogs"):  # pragma: no cover
+            with self.assertNoLogs(
+                prunerr.downloaditem.logger,
+                level=logging.WARNING,
+            ):
+                runner.review()
+        else:  # pragma: no cover
+            # BBB: Python <3.10 compat
+            with self.assertRaises(AssertionError):
+                with self.assertLogs(
+                    prunerr.downloaditem.logger,
+                    level=logging.WARNING,
+                ):
+                    runner.review()
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_runner.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_servarr.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_servarr.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 import prunerr.servarr
 
 from .. import tests
 
 
 @mock.patch.dict(os.environ, tests.PrunerrTestCase.ENV)
-class PrunerrServarrTests(tests.PrunerrTestCase):
+class PrunerrServarrTests(
+    tests.PrunerrTestCase,
+):  # pylint: disable=too-few-public-methods
     """
     Test Prunerr's interaction with Servarr instances.
     """
 
     def test_servarr_repr(self):
         """
         The Servarr representations provide useful information for debugging.
```

### Comparing `prunerr-1.0.0/src/prunerr/tests/test_verify.py` & `prunerr-1.1.0b24/src/prunerr/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `prunerr-1.0.0/src/prunerr.egg-info/PKG-INFO` & `prunerr-1.1.0b24/src/prunerr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 Metadata-Version: 2.1
 Name: prunerr
-Version: 1.0.0
+Version: 1.1.0b24
 Summary: Perma-seed Servarr media libraries
 Home-page: https://gitlab.com/rpatterson/prunerr
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: servarr,sonarr,radarr,transmission,bittorent,torrent
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: devel
 License-File: LICENSE
 
-##################################
+########################################################################################
 Prunerr
-##################################
+########################################################################################
 Perma-seed Servarr media libraries
-**********************************
+****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
 
    * - .. figure:: https://img.shields.io/pypi/v/prunerr.svg?logo=pypi&label=PyPI&logoColor=gold
           :alt: PyPI latest release version
           :target: https://pypi.org/project/prunerr/
@@ -54,37 +59,45 @@
        .. figure:: https://img.shields.io/gitlab/stars/rpatterson/prunerr?gitlab_url=https%3A%2F%2Fgitlab.com&logo=gitlab
 	  :alt: GitLab repo stars
 	  :target: https://gitlab.com/rpatterson/prunerr
 
      - .. figure:: https://img.shields.io/github/v/release/rpatterson/prunerr?logo=github
 	  :alt: GitHub release (latest SemVer)
 	  :target: https://github.com/rpatterson/prunerr/releases
-       .. figure:: https://github.com/rpatterson/prunerr/actions/workflows/ci-cd.yml/badge.svg
+       .. figure:: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml/badge.svg
           :alt: GitHub Actions status
-          :target: https://github.com/rpatterson/prunerr/
-       .. figure:: https://codecov.io/github/rpatterson/prunerr/branch/master/graph/badge.svg?token=GNKVQ8VYOU 
+          :target: https://github.com/rpatterson/prunerr/actions/workflows/build-test.yml
+       .. figure:: https://codecov.io/github/rpatterson/prunerr/branch/master/graph/badge.svg?token=GNKVQ8VYOU
           :alt: Codecov test coverage
 	  :target: https://codecov.io/github/rpatterson/prunerr
        .. figure:: https://img.shields.io/github/stars/rpatterson/prunerr?logo=github
 	  :alt: GitHub repo stars
 	  :target: https://github.com/rpatterson/prunerr/
 
-     - .. figure:: https://img.shields.io/docker/v/merpatterson/prunerr?sort=semver&logo=docker
+     - .. figure:: https://img.shields.io/docker/v/merpatterson/prunerr/master?sort=semver&logo=docker
           :alt: Docker Hub image version (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/pulls/merpatterson/prunerr?logo=docker
           :alt: Docker Hub image pulls count
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/stars/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub stars
           :target: https://hub.docker.com/r/merpatterson/prunerr
        .. figure:: https://img.shields.io/docker/image-size/merpatterson/prunerr?logo=docker
 	  :alt: Docker Hub image size (latest semver)
           :target: https://hub.docker.com/r/merpatterson/prunerr
 
+TL;DR: Perma-seeding of whole Servarr libraries optimized for per-tracker ratio.
+
+- Delete torrents/items only as disk space gets low.
+- Don't delete currently imported items.  IOW, only delete upgraded items.
+- Don't delete private items that haven't met seeding requirements.
+- Delete public items first
+- Delete private items in an order to maximize tracker ratio and/or bonuses.
+- And more...
 
 *******
 Summary
 *******
 
 Seed Servarr download client torrents/items as long as possible only deleting them as
 necessary as disk space gets low, hence the name based on "to prune".  Which download
@@ -115,29 +128,31 @@
 operations to the download items in each of those download clients.  It can also be run
 independently of any Servarr instances to optimize seeding for download items added by
 other means, e.g. `FlexGet`_.
 
 See the `Usage`_ section below for full details.
 
 
-************
+****************************************************************************************
 Installation
-************
+****************************************************************************************
 
 Install using any tool for installing standard Python 3 distributions such as `pip`_::
 
   $ sudo pip3 install prunerr
 
+Optional shell tab completion is available via `argcomplete`_.
+
 Or use `the Docker image`_.  See `the example ./docker-compose.yml file`_ for usage
 details.
 
 
-*****
+****************************************************************************************
 Usage
-*****
+****************************************************************************************
 
 Start by writing your ``~/.config/prunerr.yml`` configuration file.  See the comments in
 `the example configuration`_ for details.
 
 Once configured, you may run individual sub-commands once, run all operations once as
 configured using the ``$ prunerr exec`` sub-command, or run all operations in a polling
 loop using the ``$ prunerr daemon`` sub-command.  See the `Order of Operations`_ section
@@ -222,29 +237,29 @@
    orphans.
 
    For the other groups delete items in the order determined by the configured
    ``indexers/priorities`` indexer order then by the configured operations for that
    item's indexer.
 
 
-************
+****************************************************************************************
 CONTRIBUTING
-************
+****************************************************************************************
 
 NOTE: `This project is hosted on GitLab`_.  There's `a mirror on GitHub`_ but please use
 GitLab for reporting issues, submitting PRs/MRs and any other development or maintenance
 activity.
 
 See `the ./CONTRIBUTING.rst file`_ for more details on how to get started with
 development.
 
 
-**********
+****************************************************************************************
 Motivation
-**********
+****************************************************************************************
 
 I didn't like the available options I could find at the time for maximizing seeding from
 a lovingly managed media library.  Deleting by a ratio threshold doesn't make sense to
 me because that can delete items when there's plenty of disk space.  Also the ratio
 threshold is a reverse indicator for items from private indexers vs items from public
 indexers.  Items from private indexers with high ratios should be kept around as long as
 possible to build user total ratio whereas items from public indexers with low ratios
@@ -262,14 +277,15 @@
 .. _`Servarr`: https://wiki.servarr.com
 .. _`Radarr`: https://wiki.servarr.com/en/radarr
 .. _`Sonarr`: https://wiki.servarr.com/en/sonarr
 .. _`download clients`: https://wiki.servarr.com/radarr/settings#download-clients
 .. _`FlexGet`: https://flexget.com/
 
 .. _pip: https://pip.pypa.io/en/stable/installation/
+.. _argcomplete: https://kislyuk.github.io/argcomplete/#installation
 
 .. _the Docker image: https://hub.docker.com/r/merpatterson/prunerr
 .. _`the example ./docker-compose.yml file`: https://gitlab.com/rpatterson/prunerr/blob/master/docker-compose.yml
 
 .. _`the example configuration`:
    https://gitlab.com/rpatterson/prunerr/blob/master/src/prunerr/home/.config/prunerr.yml
```

### Comparing `prunerr-1.0.0/src/prunerr.egg-info/SOURCES.txt` & `prunerr-1.1.0b24/src/prunerr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,73 @@
 .dir-locals.el.in
 .dockerignore
 .env.in
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
+.prospector.yaml
 CONTRIBUTING.rst
 Dockerfile
 Dockerfile.devel
 LICENSE
 Makefile
 NEWS.rst
 README.rst
 TODO.rst
+docker-compose-servarr.yml
 docker-compose.override.yml
 docker-compose.yml
 pyproject.toml
-requirements-build.txt
-requirements-build.txt.in
-requirements-devel.txt
-requirements.txt
 setup.cfg
 tox.ini
-.github/workflows/ci-cd.yml
+.github/workflows/build-test.yml
+bin/cz-check-bump
 bin/entrypoint
+bin/get-base-version
+bin/hadolint
+build-host/Dockerfile
+build-host/Makefile
+build-host/README.rst
+build-host/requirements-py310.txt
+build-host/requirements-py311.txt
+build-host/requirements-py37.txt
+build-host/requirements-py38.txt
+build-host/requirements-py39.txt
+build-host/requirements.txt.in
+build-host/bin/entrypoint
+dist/.gitignore
+gitlab-runner/.gitignore
+gitlab-runner/config/config.toml.in
 home/.gitignore
 home/.pypirc.in
+requirements/build.txt.in
+requirements/py310/build.txt
+requirements/py310/devel.txt
+requirements/py310/user.txt
+requirements/py311/build.txt
+requirements/py311/devel.txt
+requirements/py311/user.txt
+requirements/py37/build.txt
+requirements/py37/devel.txt
+requirements/py37/user.txt
+requirements/py38/build.txt
+requirements/py38/devel.txt
+requirements/py38/user.txt
+requirements/py39/build.txt
+requirements/py39/devel.txt
+requirements/py39/user.txt
 s6/etc/s6-overlay/s6-rc.d/svc-transmission/finish
 src/prunerr/__init__.py
 src/prunerr/__main__.py
 src/prunerr/downloadclient.py
 src/prunerr/downloaditem.py
 src/prunerr/operations.py
 src/prunerr/runner.py
 src/prunerr/servarr.py
+src/prunerr/utils.py
 src/prunerr/version.py
 src/prunerr.egg-info/PKG-INFO
 src/prunerr.egg-info/SOURCES.txt
 src/prunerr.egg-info/dependency_links.txt
 src/prunerr.egg-info/entry_points.txt
 src/prunerr.egg-info/requires.txt
 src/prunerr.egg-info/top_level.txt
```

