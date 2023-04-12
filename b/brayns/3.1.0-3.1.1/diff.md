# Comparing `tmp/brayns-3.1.0.tar.gz` & `tmp/brayns-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brayns-3.1.0.tar", last modified: Thu Feb  9 10:30:26 2023, max compression
+gzip compressed data, was "brayns-3.1.1.tar", last modified: Wed Apr 12 13:29:28 2023, max compression
```

## Comparing `brayns-3.1.0.tar` & `brayns-3.1.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.831411 brayns-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-09 10:30:24.000000 brayns-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-02-09 10:30:26.831411 brayns-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-02-09 10:30:24.000000 brayns-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.819411 brayns-3.1.0/brayns/
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.823411 brayns-3.1.0/brayns/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/camera_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/color_ramp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/coloring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/framebuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/gbuffer_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/opacity_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/pick.py
--rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/core/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.823411 brayns-3.1.0/brayns/movie/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/movie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/movie/movie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/movie/movie_frames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.823411 brayns-3.1.0/brayns/network/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/future.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.827411 brayns-3.1.0/brayns/network/jsonrpc/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_reply.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/jsonrpc/json_rpc_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.827411 brayns-3.1.0/brayns/network/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/websocket/async_web_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/websocket/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/websocket/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/websocket/web_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/websocket/web_socket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/websocket/web_socket_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/network/websocket/web_socket_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.827411 brayns-3.1.0/brayns/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/atlas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/bbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/cell_placement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/cylindric_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/dti.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/nrrd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/sonata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/plugins/xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.827411 brayns-3.1.0/brayns/service/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/service/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/service/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.831411 brayns-3.1.0/brayns/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/plane_equation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-09 10:30:24.000000 brayns-3.1.0/brayns/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-09 10:30:26.819411 brayns-3.1.0/brayns.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-02-09 10:30:26.000000 brayns-3.1.0/brayns.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-02-09 10:30:26.000000 brayns-3.1.0/brayns.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-09 10:30:26.000000 brayns-3.1.0/brayns.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-09 10:30:26.000000 brayns-3.1.0/brayns.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-09 10:30:26.000000 brayns-3.1.0/brayns.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-02-09 10:30:24.000000 brayns-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-09 10:30:26.831411 brayns-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-02-09 10:30:24.000000 brayns-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.590876 brayns-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-12 13:29:26.000000 brayns-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-12 13:29:28.594876 brayns-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-12 13:29:26.000000 brayns-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.566876 brayns-3.1.1/brayns/
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.578876 brayns-3.1.1/brayns/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/camera_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/color_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/coloring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/framebuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/gbuffer_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/opacity_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/core/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.578876 brayns-3.1.1/brayns/movie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/movie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/movie/movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/movie/movie_frames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.582876 brayns-3.1.1/brayns/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.586876 brayns-3.1.1/brayns/network/jsonrpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_reply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/jsonrpc/json_rpc_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.586876 brayns-3.1.1/brayns/network/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/websocket/async_web_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/websocket/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/websocket/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/websocket/web_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/websocket/web_socket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/websocket/web_socket_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/network/websocket/web_socket_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.590876 brayns-3.1.1/brayns/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/atlas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/bbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/cell_placement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/cylindric_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/dti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/nrrd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/sonata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/plugins/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.590876 brayns-3.1.1/brayns/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/service/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/service/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.590876 brayns-3.1.1/brayns/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/plane_equation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10692 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-12 13:29:26.000000 brayns-3.1.1/brayns/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 13:29:28.566876 brayns-3.1.1/brayns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-12 13:29:28.000000 brayns-3.1.1/brayns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-12 13:29:28.000000 brayns-3.1.1/brayns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 13:29:28.000000 brayns-3.1.1/brayns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 13:29:28.000000 brayns-3.1.1/brayns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 13:29:28.000000 brayns-3.1.1/brayns.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-12 13:29:26.000000 brayns-3.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-12 13:29:28.594876 brayns-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-12 13:29:26.000000 brayns-3.1.1/setup.py
```

### Comparing `brayns-3.1.0/PKG-INFO` & `brayns-3.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brayns
-Version: 3.1.0
+Version: 3.1.1
 Summary: Brayns Python API
 Home-page: https://github.com/BlueBrain/Brayns
 Author: Blue Brain Project
 Author-email: bbp-open-source@googlegroups.com
 License: LGPLv3
 Download-URL: https://github.com/BlueBrain/Brayns
 Project-URL: Tracker, https://bbpteam.epfl.ch/project/issues/projects/BRAYNS/issues
```

### Comparing `brayns-3.1.0/README.md` & `brayns-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/__init__.py` & `brayns-3.1.1/brayns/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/__init__.py` & `brayns-3.1.1/brayns/core/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/application.py` & `brayns-3.1.1/brayns/core/application.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/camera.py` & `brayns-3.1.1/brayns/core/camera.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/camera_controller.py` & `brayns-3.1.1/brayns/core/camera_controller.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/color_ramp.py` & `brayns-3.1.1/brayns/core/color_ramp.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/coloring.py` & `brayns-3.1.1/brayns/core/coloring.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/entrypoint.py` & `brayns-3.1.1/brayns/core/entrypoint.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/framebuffer.py` & `brayns-3.1.1/brayns/core/framebuffer.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/gbuffer_exporter.py` & `brayns-3.1.1/brayns/core/gbuffer_exporter.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/geometry.py` & `brayns-3.1.1/brayns/core/geometry.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/image.py` & `brayns-3.1.1/brayns/core/image.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/light.py` & `brayns-3.1.1/brayns/core/light.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/loader.py` & `brayns-3.1.1/brayns/core/loader.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/material.py` & `brayns-3.1.1/brayns/core/material.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/model.py` & `brayns-3.1.1/brayns/core/model.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/opacity_curve.py` & `brayns-3.1.1/brayns/core/opacity_curve.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/pick.py` & `brayns-3.1.1/brayns/core/pick.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/projection.py` & `brayns-3.1.1/brayns/core/projection.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,18 @@
         :return: True if other is Fovy and has same value.
         :rtype: bool
         """
         if not isinstance(other, Fovy):
             return False
         return self._angle == other._angle
 
+    def __hash__(self) -> int:
+        """Mark the class as immutable."""
+        return hash(self._angle)
+
     @property
     def radians(self) -> float:
         """Get angle in radians.
 
         :return: Angle in radians.
         :rtype: float
         """
```

### Comparing `brayns-3.1.0/brayns/core/renderer.py` & `brayns-3.1.1/brayns/core/renderer.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/simulation.py` & `brayns-3.1.1/brayns/core/simulation.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/snapshot.py` & `brayns-3.1.1/brayns/core/snapshot.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/version.py` & `brayns-3.1.1/brayns/core/version.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/core/view.py` & `brayns-3.1.1/brayns/core/view.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/movie/__init__.py` & `brayns-3.1.1/brayns/movie/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/movie/movie.py` & `brayns-3.1.1/brayns/movie/movie.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/movie/movie_frames.py` & `brayns-3.1.1/brayns/movie/movie_frames.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/__init__.py` & `brayns-3.1.1/brayns/network/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/client.py` & `brayns-3.1.1/brayns/network/client.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/connector.py` & `brayns-3.1.1/brayns/network/connector.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/future.py` & `brayns-3.1.1/brayns/network/future.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/instance.py` & `brayns-3.1.1/brayns/network/instance.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/__init__.py` & `brayns-3.1.1/brayns/network/jsonrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_dispatcher.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_dispatcher.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_error.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_error.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_future.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_future.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_handler.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_handler.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_listener.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_listener.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_manager.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_manager.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_progress.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_progress.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_reply.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_reply.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_request.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_request.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_task.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_task.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/jsonrpc/json_rpc_tasks.py` & `brayns-3.1.1/brayns/network/jsonrpc/json_rpc_tasks.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/listener.py` & `brayns-3.1.1/brayns/network/listener.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/logger.py` & `brayns-3.1.1/brayns/network/logger.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/websocket/__init__.py` & `brayns-3.1.1/brayns/network/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/websocket/async_web_socket.py` & `brayns-3.1.1/brayns/network/websocket/async_web_socket.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/websocket/errors.py` & `brayns-3.1.1/brayns/network/websocket/errors.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/websocket/event_loop.py` & `brayns-3.1.1/brayns/network/websocket/event_loop.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/websocket/web_socket.py` & `brayns-3.1.1/brayns/network/websocket/web_socket.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/websocket/web_socket_client.py` & `brayns-3.1.1/brayns/network/websocket/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/websocket/web_socket_connector.py` & `brayns-3.1.1/brayns/network/websocket/web_socket_connector.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/network/websocket/web_socket_listener.py` & `brayns-3.1.1/brayns/network/websocket/web_socket_listener.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/__init__.py` & `brayns-3.1.1/brayns/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/atlas.py` & `brayns-3.1.1/brayns/plugins/atlas.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/bbp.py` & `brayns-3.1.1/brayns/plugins/bbp.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/cell_placement.py` & `brayns-3.1.1/brayns/plugins/cell_placement.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/circuit.py` & `brayns-3.1.1/brayns/plugins/circuit.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/cylindric_camera.py` & `brayns-3.1.1/brayns/plugins/cylindric_camera.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/dti.py` & `brayns-3.1.1/brayns/plugins/dti.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/morphology.py` & `brayns-3.1.1/brayns/plugins/morphology.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/nrrd.py` & `brayns-3.1.1/brayns/plugins/nrrd.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/protein.py` & `brayns-3.1.1/brayns/plugins/protein.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/sonata.py` & `brayns-3.1.1/brayns/plugins/sonata.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/plugins/xyz.py` & `brayns-3.1.1/brayns/plugins/xyz.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/service/__init__.py` & `brayns-3.1.1/brayns/service/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/service/manager.py` & `brayns-3.1.1/brayns/service/manager.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/service/process.py` & `brayns-3.1.1/brayns/service/process.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/service/service.py` & `brayns-3.1.1/brayns/service/service.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/utils/__init__.py` & `brayns-3.1.1/brayns/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/utils/bounds.py` & `brayns-3.1.1/brayns/utils/bounds.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/utils/color.py` & `brayns-3.1.1/brayns/utils/color.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/utils/error.py` & `brayns-3.1.1/brayns/utils/error.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/utils/image.py` & `brayns-3.1.1/brayns/utils/image.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/utils/json_schema.py` & `brayns-3.1.1/brayns/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/utils/plane_equation.py` & `brayns-3.1.1/brayns/utils/plane_equation.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/utils/quaternion.py` & `brayns-3.1.1/brayns/utils/quaternion.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/utils/rotation.py` & `brayns-3.1.1/brayns/utils/rotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,18 @@
 
     def __eq__(self, other: object) -> bool:
         """Equality check using internal quaternion."""
         if not isinstance(other, Rotation):
             return False
         return self._quaternion == other.quaternion
 
+    def __hash__(self) -> int:
+        """Mark the class as immutable."""
+        return hash(self._quaternion)
+
     @property
     def quaternion(self) -> Quaternion:
         """Get rotation as normalized quaternion.
 
         :return: Normalized quaternion.
         :rtype: Quaternion
         """
```

### Comparing `brayns-3.1.0/brayns/utils/transform.py` & `brayns-3.1.1/brayns/utils/transform.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/utils/vector.py` & `brayns-3.1.1/brayns/utils/vector.py`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/brayns/version.py` & `brayns-3.1.1/brayns/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this library; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
-VERSION = "3.1.0"
+VERSION = "3.1.1"
 """Version tag of brayns Python package (major.minor.patch)."""
```

### Comparing `brayns-3.1.0/brayns.egg-info/PKG-INFO` & `brayns-3.1.1/brayns.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brayns
-Version: 3.1.0
+Version: 3.1.1
 Summary: Brayns Python API
 Home-page: https://github.com/BlueBrain/Brayns
 Author: Blue Brain Project
 Author-email: bbp-open-source@googlegroups.com
 License: LGPLv3
 Download-URL: https://github.com/BlueBrain/Brayns
 Project-URL: Tracker, https://bbpteam.epfl.ch/project/issues/projects/BRAYNS/issues
```

### Comparing `brayns-3.1.0/brayns.egg-info/SOURCES.txt` & `brayns-3.1.1/brayns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/requirements.txt` & `brayns-3.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `brayns-3.1.0/setup.cfg` & `brayns-3.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = brayns
-version = 3.1.0
+version = 3.1.1
 url = https://github.com/BlueBrain/Brayns
 download_url = https://github.com/BlueBrain/Brayns
 project_urls = 
 	Tracker = https://bbpteam.epfl.ch/project/issues/projects/BRAYNS/issues
 	Source = https://github.com/BlueBrain/Brayns
 author = Blue Brain Project
 author_email = bbp-open-source@googlegroups.com
```

### Comparing `brayns-3.1.0/setup.py` & `brayns-3.1.1/setup.py`

 * *Files identical despite different names*

