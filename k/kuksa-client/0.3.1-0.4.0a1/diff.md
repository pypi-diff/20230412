# Comparing `tmp/kuksa_client-0.3.1.tar.gz` & `tmp/kuksa_client-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuksa_client-0.3.1.tar", last modified: Thu Mar 30 14:21:24 2023, max compression
+gzip compressed data, was "kuksa_client-0.4.0a1.tar", last modified: Wed Apr 12 10:05:48 2023, max compression
```

## Comparing `kuksa_client-0.3.1.tar` & `kuksa_client-0.4.0a1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.747574 kuksa_client-0.3.1/
--rw-r--r--   0 scs2rng    (503) wheel        (0)    11357 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/LICENSE
--rw-r--r--   0 scs2rng    (503) wheel        (0)       35 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/MANIFEST.in
--rw-r--r--   0 scs2rng    (503) wheel        (0)     9638 2023-03-30 14:21:24.747643 kuksa_client-0.3.1/PKG-INFO
--rw-r--r--   0 scs2rng    (503) wheel        (0)     8758 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/README.md
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.740008 kuksa_client-0.3.1/kuksa/
--rw-r--r--   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa/__init__.py
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.740131 kuksa_client-0.3.1/kuksa/val/
--rw-r--r--   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa/val/__init__.py
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.740890 kuksa_client-0.3.1/kuksa/val/v1/
--rw-r--r--   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa/val/v1/__init__.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)     9374 2023-03-30 14:21:24.000000 kuksa_client-0.3.1/kuksa/val/v1/types_pb2.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)      159 2023-03-30 14:21:24.000000 kuksa_client-0.3.1/kuksa/val/v1/types_pb2_grpc.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)     3751 2023-03-30 14:21:24.000000 kuksa_client-0.3.1/kuksa/val/v1/val_pb2.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)     8731 2023-03-30 14:21:24.000000 kuksa_client-0.3.1/kuksa/val/v1/val_pb2_grpc.py
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.742468 kuksa_client-0.3.1/kuksa_certificates/
--rw-r--r--   0 scs2rng    (503) wheel        (0)     1675 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/CA.key
--rw-r--r--   0 scs2rng    (503) wheel        (0)     1342 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/CA.pem
--rw-r--r--   0 scs2rng    (503) wheel        (0)     1679 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/Client.key
--rw-r--r--   0 scs2rng    (503) wheel        (0)     1334 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/Client.pem
--rw-r--r--   0 scs2rng    (503) wheel        (0)     2267 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/README.md
--rw-r--r--   0 scs2rng    (503) wheel        (0)     1679 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/Server.key
--rw-r--r--   0 scs2rng    (503) wheel        (0)     1334 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/Server.pem
--rw-r--r--   0 scs2rng    (503) wheel        (0)      114 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/__init__.py
--rwxr-xr-x   0 scs2rng    (503) wheel        (0)     1398 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/genCerts.sh
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.744384 kuksa_client-0.3.1/kuksa_certificates/jwt/
--rw-r--r--   0 scs2rng    (503) wheel        (0)      151 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/all-read-write.json
--rw-r--r--   0 scs2rng    (503) wheel        (0)      875 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/all-read-write.json.token
--rwxr-xr-x   0 scs2rng    (503) wheel        (0)     1430 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/createToken.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)     3243 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/jwt.key
--rw-r--r--   0 scs2rng    (503) wheel        (0)      800 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/jwt.key.pub
--rwxr-xr-x   0 scs2rng    (503) wheel        (0)      901 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/recreateJWTkeyPair.sh
--rw-r--r--   0 scs2rng    (503) wheel        (0)       34 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/requirements.txt
--rw-r--r--   0 scs2rng    (503) wheel        (0)      167 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/single-read.json
--rw-r--r--   0 scs2rng    (503) wheel        (0)      895 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/single-read.json.token
--rw-r--r--   0 scs2rng    (503) wheel        (0)      175 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/super-admin.json
--rw-r--r--   0 scs2rng    (503) wheel        (0)      899 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_certificates/jwt/super-admin.json.token
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.745176 kuksa_client-0.3.1/kuksa_client/
--rw-r--r--   0 scs2rng    (503) wheel        (0)     3680 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/__init__.py
--rwxr-xr-x   0 scs2rng    (503) wheel        (0)    22102 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/__main__.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)     1708 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/_metadata.py
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.746515 kuksa_client-0.3.1/kuksa_client/cli_backend/
--rw-r--r--   0 scs2rng    (503) wheel        (0)     2114 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/cli_backend/__init__.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)     9504 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/cli_backend/grpc.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)     9070 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/cli_backend/ws.py
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.746841 kuksa_client-0.3.1/kuksa_client/grpc/
--rw-r--r--   0 scs2rng    (503) wheel        (0)    34136 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/grpc/__init__.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)    13678 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/grpc/aio.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)      385 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/logging.ini
--rw-r--r--   0 scs2rng    (503) wheel        (0)      605 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/logo
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.746993 kuksa_client-0.3.1/kuksa_client/ws/
--rw-r--r--   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/kuksa_client/ws/__init__.py
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.746022 kuksa_client-0.3.1/kuksa_client.egg-info/
--rw-r--r--   0 scs2rng    (503) wheel        (0)     9638 2023-03-30 14:21:24.000000 kuksa_client-0.3.1/kuksa_client.egg-info/PKG-INFO
--rw-r--r--   0 scs2rng    (503) wheel        (0)     1542 2023-03-30 14:21:24.000000 kuksa_client-0.3.1/kuksa_client.egg-info/SOURCES.txt
--rw-r--r--   0 scs2rng    (503) wheel        (0)        1 2023-03-30 14:21:24.000000 kuksa_client-0.3.1/kuksa_client.egg-info/dependency_links.txt
--rw-r--r--   0 scs2rng    (503) wheel        (0)       60 2023-03-30 14:21:24.000000 kuksa_client-0.3.1/kuksa_client.egg-info/entry_points.txt
--rw-r--r--   0 scs2rng    (503) wheel        (0)      227 2023-03-30 14:21:24.000000 kuksa_client-0.3.1/kuksa_client.egg-info/requires.txt
--rw-r--r--   0 scs2rng    (503) wheel        (0)       44 2023-03-30 14:21:24.000000 kuksa_client-0.3.1/kuksa_client.egg-info/top_level.txt
--rw-r--r--   0 scs2rng    (503) wheel        (0)      625 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/pyproject.toml
--rw-r--r--   0 scs2rng    (503) wheel        (0)     1388 2023-03-30 14:21:24.748027 kuksa_client-0.3.1/setup.cfg
--rw-r--r--   0 scs2rng    (503) wheel        (0)     1168 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/setup.py
-drwxr-xr-x   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:21:24.747413 kuksa_client-0.3.1/tests/
--rw-r--r--   0 scs2rng    (503) wheel        (0)        0 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/tests/__init__.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)     2545 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/tests/conftest.py
--rw-r--r--   0 scs2rng    (503) wheel        (0)    57437 2023-03-30 14:20:53.000000 kuksa_client-0.3.1/tests/test_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/
+-rw-r--r--   0 erik      (1000) erik      (1000)    11357 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/LICENSE
+-rw-r--r--   0 erik      (1000) erik      (1000)       35 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/MANIFEST.in
+-rw-r--r--   0 erik      (1000) erik      (1000)     9640 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     8758 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/README.md
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:47.997582 kuksa_client-0.4.0a1/kuksa/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:47.997582 kuksa_client-0.4.0a1/kuksa/val/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa/val/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:47.997582 kuksa_client-0.4.0a1/kuksa/val/v1/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa/val/v1/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9374 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa/val/v1/types_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      159 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa/val/v1/types_pb2_grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3751 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa/val/v1/val_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     8731 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa/val/v1/val_pb2_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.001580 kuksa_client-0.4.0a1/kuksa_certificates/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1675 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a1/kuksa_certificates/CA.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1342 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/CA.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a1/kuksa_certificates/Client.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1334 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/Client.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)     2267 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a1/kuksa_certificates/Server.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1334 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/Server.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)      114 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     1398 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/genCerts.sh
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.001580 kuksa_client-0.4.0a1/kuksa_certificates/jwt/
+-rw-r--r--   0 erik      (1000) erik      (1000)      151 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/all-read-write.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      875 2022-11-01 08:41:15.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/all-read-write.json.token
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     1430 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/createToken.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3243 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/jwt.key
+-rw-r--r--   0 erik      (1000) erik      (1000)      800 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/jwt.key.pub
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      901 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/recreateJWTkeyPair.sh
+-rw-r--r--   0 erik      (1000) erik      (1000)       34 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/requirements.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      167 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/single-read.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      895 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/single-read.json.token
+-rw-r--r--   0 erik      (1000) erik      (1000)      175 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/super-admin.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      899 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a1/kuksa_certificates/jwt/super-admin.json.token
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.001580 kuksa_client-0.4.0a1/kuksa_client/
+-rw-r--r--   0 erik      (1000) erik      (1000)     3680 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    22102 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/__main__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1708 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/_metadata.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/kuksa_client/cli_backend/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2114 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/cli_backend/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9739 2023-04-12 07:56:08.000000 kuksa_client-0.4.0a1/kuksa_client/cli_backend/grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9070 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/cli_backend/ws.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/kuksa_client/grpc/
+-rw-r--r--   0 erik      (1000) erik      (1000)    36389 2023-04-12 07:56:08.000000 kuksa_client-0.4.0a1/kuksa_client/grpc/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    15204 2023-04-12 07:56:08.000000 kuksa_client-0.4.0a1/kuksa_client/grpc/aio.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      385 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/logging.ini
+-rw-r--r--   0 erik      (1000) erik      (1000)      605 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/logo
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/kuksa_client/ws/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/kuksa_client/ws/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.001580 kuksa_client-0.4.0a1/kuksa_client.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)     9640 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1542 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       60 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      227 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       44 2023-04-12 10:05:47.000000 kuksa_client-0.4.0a1/kuksa_client.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      625 2023-04-12 10:04:35.000000 kuksa_client-0.4.0a1/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)     1388 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1168 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-12 10:05:48.005578 kuksa_client-0.4.0a1/tests/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/tests/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2545 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a1/tests/conftest.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    63303 2023-04-12 07:56:08.000000 kuksa_client-0.4.0a1/tests/test_grpc.py
```

### Comparing `kuksa_client-0.3.1/LICENSE` & `kuksa_client-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/PKG-INFO` & `kuksa_client-0.4.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuksa_client
-Version: 0.3.1
+Version: 0.4.0a1
 Summary: kuksa.val python clients and SDK
 Home-page: https://github.com/eclipse/kuksa.val
 Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
 Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
 Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
 Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `kuksa_client-0.3.1/README.md` & `kuksa_client-0.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa/val/v1/types_pb2.py` & `kuksa_client-0.4.0a1/kuksa/val/v1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa/val/v1/val_pb2.py` & `kuksa_client-0.4.0a1/kuksa/val/v1/val_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa/val/v1/val_pb2_grpc.py` & `kuksa_client-0.4.0a1/kuksa/val/v1/val_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/CA.key` & `kuksa_client-0.4.0a1/kuksa_certificates/CA.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/CA.pem` & `kuksa_client-0.4.0a1/kuksa_certificates/CA.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/Client.key` & `kuksa_client-0.4.0a1/kuksa_certificates/Client.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/Client.pem` & `kuksa_client-0.4.0a1/kuksa_certificates/Client.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/README.md` & `kuksa_client-0.4.0a1/kuksa_certificates/README.md`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/Server.key` & `kuksa_client-0.4.0a1/kuksa_certificates/Server.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/Server.pem` & `kuksa_client-0.4.0a1/kuksa_certificates/Server.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/genCerts.sh` & `kuksa_client-0.4.0a1/kuksa_certificates/genCerts.sh`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/jwt/all-read-write.json.token` & `kuksa_client-0.4.0a1/kuksa_certificates/jwt/all-read-write.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/jwt/createToken.py` & `kuksa_client-0.4.0a1/kuksa_certificates/jwt/createToken.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/jwt/jwt.key` & `kuksa_client-0.4.0a1/kuksa_certificates/jwt/jwt.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/jwt/jwt.key.pub` & `kuksa_client-0.4.0a1/kuksa_certificates/jwt/jwt.key.pub`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/jwt/recreateJWTkeyPair.sh` & `kuksa_client-0.4.0a1/kuksa_certificates/jwt/recreateJWTkeyPair.sh`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/jwt/single-read.json.token` & `kuksa_client-0.4.0a1/kuksa_certificates/jwt/single-read.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_certificates/jwt/super-admin.json.token` & `kuksa_client-0.4.0a1/kuksa_certificates/jwt/super-admin.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_client/__init__.py` & `kuksa_client-0.4.0a1/kuksa_client/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_client/__main__.py` & `kuksa_client-0.4.0a1/kuksa_client/__main__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_client/_metadata.py` & `kuksa_client-0.4.0a1/kuksa_client/_metadata.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_client/cli_backend/__init__.py` & `kuksa_client-0.4.0a1/kuksa_client/cli_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_client/cli_backend/grpc.py` & `kuksa_client-0.4.0a1/kuksa_client/cli_backend/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,16 @@
     # Function to implement get
     def getValue(self, path, attribute="value", timeout=5):
         return self.getValues((path,), attribute, timeout)
 
     def getValues(self, paths, attribute="value", timeout=5):
         if attribute in self.AttrDict:
             field, view = self.AttrDict[attribute]
-            entries = [kuksa_client.grpc.EntryRequest(path=path, view=view, fields=(field,)) for path in paths]
+            entries = [kuksa_client.grpc.EntryRequest(
+                path=path, view=view, fields=(field,)) for path in paths]
             requestArgs = {'entries': entries}
             return self._sendReceiveMsg(("get", requestArgs), timeout)
 
         return json.dumps({"error": "Invalid Attribute"})
 
     # Function to implement set
     def setValue(self, path, value, attribute="value", timeout=5):
@@ -93,50 +94,56 @@
 
     def setValues(self, updates: Dict[str, Any], attribute="value", timeout=5):
         if attribute in self.AttrDict:
             field, _ = self.AttrDict[attribute]
             entry_updates = []
             for path, value in updates.items():
                 if field is kuksa_client.grpc.Field.VALUE:
-                    entry = kuksa_client.grpc.DataEntry(path=path, value=kuksa_client.grpc.Datapoint(value=value))
+                    entry = kuksa_client.grpc.DataEntry(
+                        path=path, value=kuksa_client.grpc.Datapoint(value=value))
                 elif field is kuksa_client.grpc.Field.ACTUATOR_TARGET:
                     entry = kuksa_client.grpc.DataEntry(
-                        path=path, actuator_target=kuksa_client.grpc.Datapoint(value=value),
+                        path=path, actuator_target=kuksa_client.grpc.Datapoint(
+                            value=value),
                     )
                 elif field is kuksa_client.grpc.Field.METADATA:
                     try:
                         metadata_dict = json.loads(value)
                     except json.JSONDecodeError:
                         return json.dumps({"error": "Metadata value needs to be a valid JSON object"})
                     entry = kuksa_client.grpc.DataEntry(
-                        path=path, metadata=kuksa_client.grpc.Metadata.from_dict(metadata_dict),
+                        path=path, metadata=kuksa_client.grpc.Metadata.from_dict(
+                            metadata_dict),
                     )
-                entry_updates.append(kuksa_client.grpc.EntryUpdate(entry=entry, fields=(field,)))
+                entry_updates.append(kuksa_client.grpc.EntryUpdate(
+                    entry=entry, fields=(field,)))
             requestArgs = {'updates': entry_updates}
             return self._sendReceiveMsg(("set", requestArgs), timeout)
         return json.dumps({"error": "Invalid Attribute"})
 
     # Function for authorization
     def authorize(self, tokenfile=None, timeout=5):
         if tokenfile is None:
             tokenfile = self.tokenfile
         tokenfile = pathlib.Path(tokenfile)
-        requestArgs = {'token': tokenfile.expanduser().read_text(encoding='utf-8')}
+        requestArgs = {
+            'token': tokenfile.expanduser().read_text(encoding='utf-8').rstrip('\n')}
 
         return self._sendReceiveMsg(("authorize", requestArgs), timeout)
 
     # Subscribe value changes of to a given path.
     # The given callback function will be called then, if the given path is updated.
     def subscribe(self, path, callback, attribute="value", timeout=5):
         return self.subscribeMultiple((path,), callback, attribute, timeout)
 
     def subscribeMultiple(self, paths, callback, attribute="value", timeout=5):
         if attribute in self.AttrDict:
             field, view = self.AttrDict[attribute]
-            entries = [kuksa_client.grpc.SubscribeEntry(path=path, view=view, fields=(field,)) for path in paths]
+            entries = [kuksa_client.grpc.SubscribeEntry(
+                path=path, view=view, fields=(field,)) for path in paths]
             requestArgs = {
                 'entries': entries,
                 'callback': callback_wrapper(callback),
             }
             return self._sendReceiveMsg(("subscribe", requestArgs), timeout)
 
         return json.dumps({"error": "Invalid Attribute"})
@@ -167,45 +174,48 @@
             respJson = json.dumps({"error": "Timeout"})
         return respJson
 
     # Async function to handle the gRPC calls
     async def _grpcHandler(self, vss_client):
         self.grpcConnected = True
         self.run = True
-        subscriber_manager = kuksa_client.grpc.aio.SubscriberManager(vss_client)
+        subscriber_manager = kuksa_client.grpc.aio.SubscriberManager(
+            vss_client)
         while self.run:
             try:
                 (call, requestArgs, responseQueue) = self.sendMsgQueue.get_nowait()
             except queue.Empty:
                 await asyncio.sleep(0.01)
                 continue
             try:
                 if call == "get":
                     resp = await vss_client.get(**requestArgs)
                     resp = [entry.to_dict() for entry in resp]
                     resp = resp[0] if len(resp) == 1 else resp
                 elif call == "set":
                     resp = await vss_client.set(**requestArgs)
                 elif call == "authorize":
-                    resp = await vss_client.authorize(**requestArgs)
+                    resp = await vss_client.authorize(str(requestArgs["token"]))
                 elif call == "subscribe":
                     callback = requestArgs.pop('callback')
-                    subscriber_response_stream = vss_client.subscribe(**requestArgs)
+                    subscriber_response_stream = vss_client.subscribe(
+                        **requestArgs)
                     resp = await subscriber_manager.add_subscriber(subscriber_response_stream, callback)
                     resp = {"subscriptionId": str(resp)}
                 elif call == "unsubscribe":
                     resp = await subscriber_manager.remove_subscriber(**requestArgs)
                 else:
                     raise Exception("Not Implemented.")
 
                 responseQueue.put((resp, None))
             except kuksa_client.grpc.VSSClientError as exc:
                 responseQueue.put((None, exc.to_dict()))
             except ValueError as exc:
-                responseQueue.put((None, {"error": "ValueError in casting the value."}))
+                responseQueue.put(
+                    (None, {"error": "ValueError in casting the value."}))
 
         self.grpcConnected = False
 
     # Main loop for handling gRPC communication
     async def mainLoop(self):
         if self.insecure:
             async with kuksa_client.grpc.aio.VSSClient(self.serverIP, self.serverPort) as vss_client:
```

### Comparing `kuksa_client-0.3.1/kuksa_client/cli_backend/ws.py` & `kuksa_client-0.4.0a1/kuksa_client/cli_backend/ws.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_client/grpc/__init__.py` & `kuksa_client-0.4.0a1/kuksa_client/grpc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,75 +40,75 @@
 from kuksa.val.v1 import val_pb2_grpc
 
 
 logger = logging.getLogger(__name__)
 
 
 class DataType(enum.IntEnum):
-    UNSPECIFIED     = types_pb2.DATA_TYPE_UNSPECIFIED
-    STRING          = types_pb2.DATA_TYPE_STRING
-    BOOLEAN         = types_pb2.DATA_TYPE_BOOLEAN
-    INT8            = types_pb2.DATA_TYPE_INT8
-    INT16           = types_pb2.DATA_TYPE_INT16
-    INT32           = types_pb2.DATA_TYPE_INT32
-    INT64           = types_pb2.DATA_TYPE_INT64
-    UINT8           = types_pb2.DATA_TYPE_UINT8
-    UINT16          = types_pb2.DATA_TYPE_UINT16
-    UINT32          = types_pb2.DATA_TYPE_UINT32
-    UINT64          = types_pb2.DATA_TYPE_UINT64
-    FLOAT           = types_pb2.DATA_TYPE_FLOAT
-    DOUBLE          = types_pb2.DATA_TYPE_DOUBLE
-    TIMESTAMP       = types_pb2.DATA_TYPE_TIMESTAMP
-    STRING_ARRAY    = types_pb2.DATA_TYPE_STRING_ARRAY
-    BOOLEAN_ARRAY   = types_pb2.DATA_TYPE_BOOLEAN_ARRAY
-    INT8_ARRAY      = types_pb2.DATA_TYPE_INT8_ARRAY
-    INT16_ARRAY     = types_pb2.DATA_TYPE_INT16_ARRAY
-    INT32_ARRAY     = types_pb2.DATA_TYPE_INT32_ARRAY
-    INT64_ARRAY     = types_pb2.DATA_TYPE_INT64_ARRAY
-    UINT8_ARRAY     = types_pb2.DATA_TYPE_UINT8_ARRAY
-    UINT16_ARRAY    = types_pb2.DATA_TYPE_UINT16_ARRAY
-    UINT32_ARRAY    = types_pb2.DATA_TYPE_UINT32_ARRAY
-    UINT64_ARRAY    = types_pb2.DATA_TYPE_UINT64_ARRAY
-    FLOAT_ARRAY     = types_pb2.DATA_TYPE_FLOAT_ARRAY
-    DOUBLE_ARRAY    = types_pb2.DATA_TYPE_DOUBLE_ARRAY
+    UNSPECIFIED = types_pb2.DATA_TYPE_UNSPECIFIED
+    STRING = types_pb2.DATA_TYPE_STRING
+    BOOLEAN = types_pb2.DATA_TYPE_BOOLEAN
+    INT8 = types_pb2.DATA_TYPE_INT8
+    INT16 = types_pb2.DATA_TYPE_INT16
+    INT32 = types_pb2.DATA_TYPE_INT32
+    INT64 = types_pb2.DATA_TYPE_INT64
+    UINT8 = types_pb2.DATA_TYPE_UINT8
+    UINT16 = types_pb2.DATA_TYPE_UINT16
+    UINT32 = types_pb2.DATA_TYPE_UINT32
+    UINT64 = types_pb2.DATA_TYPE_UINT64
+    FLOAT = types_pb2.DATA_TYPE_FLOAT
+    DOUBLE = types_pb2.DATA_TYPE_DOUBLE
+    TIMESTAMP = types_pb2.DATA_TYPE_TIMESTAMP
+    STRING_ARRAY = types_pb2.DATA_TYPE_STRING_ARRAY
+    BOOLEAN_ARRAY = types_pb2.DATA_TYPE_BOOLEAN_ARRAY
+    INT8_ARRAY = types_pb2.DATA_TYPE_INT8_ARRAY
+    INT16_ARRAY = types_pb2.DATA_TYPE_INT16_ARRAY
+    INT32_ARRAY = types_pb2.DATA_TYPE_INT32_ARRAY
+    INT64_ARRAY = types_pb2.DATA_TYPE_INT64_ARRAY
+    UINT8_ARRAY = types_pb2.DATA_TYPE_UINT8_ARRAY
+    UINT16_ARRAY = types_pb2.DATA_TYPE_UINT16_ARRAY
+    UINT32_ARRAY = types_pb2.DATA_TYPE_UINT32_ARRAY
+    UINT64_ARRAY = types_pb2.DATA_TYPE_UINT64_ARRAY
+    FLOAT_ARRAY = types_pb2.DATA_TYPE_FLOAT_ARRAY
+    DOUBLE_ARRAY = types_pb2.DATA_TYPE_DOUBLE_ARRAY
     TIMESTAMP_ARRAY = types_pb2.DATA_TYPE_TIMESTAMP_ARRAY
 
 
 class EntryType(enum.IntEnum):
     UNSPECIFIED = types_pb2.ENTRY_TYPE_UNSPECIFIED
-    ATTRIBUTE   = types_pb2.ENTRY_TYPE_ATTRIBUTE
-    SENSOR      = types_pb2.ENTRY_TYPE_SENSOR
-    ACTUATOR    = types_pb2.ENTRY_TYPE_ACTUATOR
+    ATTRIBUTE = types_pb2.ENTRY_TYPE_ATTRIBUTE
+    SENSOR = types_pb2.ENTRY_TYPE_SENSOR
+    ACTUATOR = types_pb2.ENTRY_TYPE_ACTUATOR
 
 
 class View(enum.IntEnum):
-    UNSPECIFIED   = types_pb2.VIEW_UNSPECIFIED
+    UNSPECIFIED = types_pb2.VIEW_UNSPECIFIED
     CURRENT_VALUE = types_pb2.VIEW_CURRENT_VALUE
-    TARGET_VALUE  = types_pb2.VIEW_TARGET_VALUE
-    METADATA      = types_pb2.VIEW_METADATA
-    FIELDS        = types_pb2.VIEW_FIELDS
-    ALL           = types_pb2.VIEW_ALL
+    TARGET_VALUE = types_pb2.VIEW_TARGET_VALUE
+    METADATA = types_pb2.VIEW_METADATA
+    FIELDS = types_pb2.VIEW_FIELDS
+    ALL = types_pb2.VIEW_ALL
 
 
 class Field(enum.IntEnum):
-    UNSPECIFIED                = types_pb2.FIELD_UNSPECIFIED
-    PATH                       = types_pb2.FIELD_PATH
-    VALUE                      = types_pb2.FIELD_VALUE
-    ACTUATOR_TARGET            = types_pb2.FIELD_ACTUATOR_TARGET
-    METADATA                   = types_pb2.FIELD_METADATA
-    METADATA_DATA_TYPE         = types_pb2.FIELD_METADATA_DATA_TYPE
-    METADATA_DESCRIPTION       = types_pb2.FIELD_METADATA_DESCRIPTION
-    METADATA_ENTRY_TYPE        = types_pb2.FIELD_METADATA_ENTRY_TYPE
-    METADATA_COMMENT           = types_pb2.FIELD_METADATA_COMMENT
-    METADATA_DEPRECATION       = types_pb2.FIELD_METADATA_DEPRECATION
-    METADATA_UNIT              = types_pb2.FIELD_METADATA_UNIT
+    UNSPECIFIED = types_pb2.FIELD_UNSPECIFIED
+    PATH = types_pb2.FIELD_PATH
+    VALUE = types_pb2.FIELD_VALUE
+    ACTUATOR_TARGET = types_pb2.FIELD_ACTUATOR_TARGET
+    METADATA = types_pb2.FIELD_METADATA
+    METADATA_DATA_TYPE = types_pb2.FIELD_METADATA_DATA_TYPE
+    METADATA_DESCRIPTION = types_pb2.FIELD_METADATA_DESCRIPTION
+    METADATA_ENTRY_TYPE = types_pb2.FIELD_METADATA_ENTRY_TYPE
+    METADATA_COMMENT = types_pb2.FIELD_METADATA_COMMENT
+    METADATA_DEPRECATION = types_pb2.FIELD_METADATA_DEPRECATION
+    METADATA_UNIT = types_pb2.FIELD_METADATA_UNIT
     METADATA_VALUE_RESTRICTION = types_pb2.FIELD_METADATA_VALUE_RESTRICTION
-    METADATA_ACTUATOR          = types_pb2.FIELD_METADATA_ACTUATOR
-    METADATA_SENSOR            = types_pb2.FIELD_METADATA_SENSOR
-    METADATA_ATTRIBUTE         = types_pb2.FIELD_METADATA_ATTRIBUTE
+    METADATA_ACTUATOR = types_pb2.FIELD_METADATA_ACTUATOR
+    METADATA_SENSOR = types_pb2.FIELD_METADATA_SENSOR
+    METADATA_ATTRIBUTE = types_pb2.FIELD_METADATA_ATTRIBUTE
 
 
 class MetadataField(enum.Enum):
     ALL = Field.METADATA
     DATA_TYPE = Field.METADATA_DATA_TYPE
     DESCRIPTION = Field.METADATA_DESCRIPTION
     ENTRY_TYPE = Field.METADATA_ENTRY_TYPE
@@ -125,15 +125,15 @@
     def __init__(self, error: Dict[str, Any], errors: List[Dict[str, Any]]):
         super().__init__(error, errors)
         self.error = error
         self.errors = errors
 
     @classmethod
     def from_grpc_error(cls, error: RpcError):
-        grpc_code, grpc_reason  = error.code().value
+        grpc_code, grpc_reason = error.code().value
         # TODO: Maybe details could hold an actual Error and/or repeated DataEntryError protobuf messages.
         #       This would allow 'code' to be an actual HTTP/VISS status code not a gRPC one.
         return cls(error={'code': grpc_code, 'reason': grpc_reason, 'message': error.details()}, errors=[])
 
     def to_dict(self) -> Dict[str, Any]:
         return {'error': self.error, 'errors': self.errors}
 
@@ -154,31 +154,36 @@
     deprecation: Optional[str] = None
     unit: Optional[str] = None
     value_restriction: Optional[ValueRestriction] = None
     # No support for entry_specific for now.
 
     @classmethod
     def from_message(cls, message: types_pb2.Metadata):
-        metadata = cls(data_type=DataType(message.data_type), entry_type=EntryType(message.entry_type))
+        metadata = cls(data_type=DataType(message.data_type),
+                       entry_type=EntryType(message.entry_type))
         for field in ('description', 'comment', 'deprecation', 'unit'):
             if message.HasField(field):
                 setattr(metadata, field, getattr(message, field))
         if message.HasField('value_restriction'):
-            value_restriction = getattr(message.value_restriction, message.value_restriction.WhichOneof('type'))
+            value_restriction = getattr(
+                message.value_restriction, message.value_restriction.WhichOneof('type'))
             metadata.value_restriction = ValueRestriction()
             for field in ('min', 'max'):
                 if value_restriction.HasField(field):
-                    setattr(metadata.value_restriction, field, getattr(value_restriction, field))
+                    setattr(metadata.value_restriction, field,
+                            getattr(value_restriction, field))
             if value_restriction.allowed_values:
-                metadata.value_restriction.allowed_values = list(value_restriction.allowed_values)
+                metadata.value_restriction.allowed_values = list(
+                    value_restriction.allowed_values)
         return metadata
 
     # pylint: disable=too-many-branches
     def to_message(self, value_type: DataType = DataType.UNSPECIFIED) -> types_pb2.Metadata:
-        message = types_pb2.Metadata(data_type=self.data_type.value, entry_type=self.entry_type.value)
+        message = types_pb2.Metadata(
+            data_type=self.data_type.value, entry_type=self.entry_type.value)
         for field in ('description', 'comment', 'deprecation', 'unit'):
             field_value = getattr(self, field, None)
             if field_value is not None:
                 setattr(message, field, field_value)
         if self.value_restriction is not None:
             if value_type in (
                 DataType.INT8,
@@ -187,63 +192,74 @@
                 DataType.INT64,
                 DataType.INT8_ARRAY,
                 DataType.INT16_ARRAY,
                 DataType.INT32_ARRAY,
                 DataType.INT64_ARRAY,
             ):
                 if self.value_restriction.min is not None:
-                    message.value_restriction.signed.min = int(self.value_restriction.min)
+                    message.value_restriction.signed.min = int(
+                        self.value_restriction.min)
                 if self.value_restriction.max is not None:
-                    message.value_restriction.signed.max = int(self.value_restriction.max)
+                    message.value_restriction.signed.max = int(
+                        self.value_restriction.max)
                 if self.value_restriction.allowed_values is not None:
                     message.value_restriction.signed.allowed_values.extend(
-                        (int(value) for value in self.value_restriction.allowed_values),
+                        (int(value)
+                         for value in self.value_restriction.allowed_values),
                     )
             elif value_type in (
                 DataType.UINT8,
                 DataType.UINT16,
                 DataType.UINT32,
                 DataType.UINT64,
                 DataType.UINT8_ARRAY,
                 DataType.UINT16_ARRAY,
                 DataType.UINT32_ARRAY,
                 DataType.UINT64_ARRAY,
             ):
                 if self.value_restriction.min is not None:
-                    message.value_restriction.unsigned.min = int(self.value_restriction.min)
+                    message.value_restriction.unsigned.min = int(
+                        self.value_restriction.min)
                 if self.value_restriction.max is not None:
-                    message.value_restriction.unsigned.max = int(self.value_restriction.max)
+                    message.value_restriction.unsigned.max = int(
+                        self.value_restriction.max)
                 if self.value_restriction.allowed_values is not None:
                     message.value_restriction.unsigned.allowed_values.extend(
-                        (int(value) for value in self.value_restriction.allowed_values),
+                        (int(value)
+                         for value in self.value_restriction.allowed_values),
                     )
             elif value_type in (
                 DataType.FLOAT,
                 DataType.DOUBLE,
                 DataType.FLOAT_ARRAY,
                 DataType.DOUBLE_ARRAY,
             ):
                 if self.value_restriction.min is not None:
-                    message.value_restriction.floating_point.min = float(self.value_restriction.min)
+                    message.value_restriction.floating_point.min = float(
+                        self.value_restriction.min)
                 if self.value_restriction.max is not None:
-                    message.value_restriction.floating_point.max = float(self.value_restriction.max)
+                    message.value_restriction.floating_point.max = float(
+                        self.value_restriction.max)
                 if self.value_restriction.allowed_values is not None:
                     message.value_restriction.floating_point.allowed_values.extend(
-                        (float(value) for value in self.value_restriction.allowed_values),
+                        (float(value)
+                         for value in self.value_restriction.allowed_values),
                     )
             elif value_type in (
                 DataType.STRING,
                 DataType.STRING_ARRAY,
             ):
                 if self.value_restriction.allowed_values is not None:
                     message.value_restriction.string.allowed_values.extend(
-                        (str(value) for value in self.value_restriction.allowed_values),
+                        (str(value)
+                         for value in self.value_restriction.allowed_values),
                     )
             else:
-                raise ValueError(f"Cannot set value_restriction from data type {value_type.name}")
+                raise ValueError(
+                    f"Cannot set value_restriction from data type {value_type.name}")
         return message
     # pylint: enable=too-many-branches
 
     @classmethod
     def from_dict(cls, metadata_dict: Dict[str, Any]):
         data_type = metadata_dict.get('data_type', DataType.UNSPECIFIED)
         if isinstance(data_type, str):
@@ -266,15 +282,16 @@
             for field in ('min', 'max', 'allowed_values'):
                 field_value = value_restriction.get(field)
                 if field_value is not None:
                     setattr(instance.value_restriction, field, field_value)
         return instance
 
     def to_dict(self) -> Dict[str, Any]:
-        out_dict = {'data_type': self.data_type.name, 'entry_type': self.entry_type.name}
+        out_dict = {'data_type': self.data_type.name,
+                    'entry_type': self.entry_type.name}
         for field in ('description', 'comment', 'deprecation', 'unit'):
             field_value = getattr(self, field, None)
             if field_value is not None:
                 out_dict[field] = field_value
         if self.value_restriction is not None:
             out_dict['value_restriction'] = {}
             for field in ('min', 'max', 'allowed_values'):
@@ -296,14 +313,15 @@
             timestamp=message.timestamp.ToDatetime(
                 tzinfo=datetime.timezone.utc,
             ) if message.HasField('timestamp') else None,
         )
 
     def to_message(self, value_type: DataType) -> types_pb2.Datapoint:
         message = types_pb2.Datapoint()
+
         def set_array_attr(obj, attr, values):
             array = getattr(obj, attr)
             array.Clear()
             array.values.extend(values)
 
         def cast_array_values(cast, array):
             for item in array:
@@ -364,35 +382,39 @@
 @dataclasses.dataclass
 class DataEntry:
     path: str
     value: Optional[Datapoint] = None
     actuator_target: Optional[Datapoint] = None
     metadata: Optional[Metadata] = None
 
-    value_type: DataType = DataType.UNSPECIFIED  # Useful for serialisation, won't appear directly in serialised object
+    # Useful for serialisation, won't appear directly in serialised object
+    value_type: DataType = DataType.UNSPECIFIED
 
     @classmethod
     def from_message(cls, message: types_pb2.DataEntry):
         entry_kwargs = {'path': message.path}
         if message.HasField('value'):
             entry_kwargs['value'] = Datapoint.from_message(message.value)
         if message.HasField('actuator_target'):
-            entry_kwargs['actuator_target'] = Datapoint.from_message(message.actuator_target)
+            entry_kwargs['actuator_target'] = Datapoint.from_message(
+                message.actuator_target)
         if message.HasField('metadata'):
             entry_kwargs['metadata'] = Metadata.from_message(message.metadata)
         return cls(**entry_kwargs)
 
     def to_message(self) -> types_pb2.DataEntry:
         message = types_pb2.DataEntry(path=self.path)
         if self.value is not None:
             message.value.MergeFrom(self.value.to_message(self.value_type))
         if self.actuator_target is not None:
-            message.actuator_target.MergeFrom(self.actuator_target.to_message(self.value_type))
+            message.actuator_target.MergeFrom(
+                self.actuator_target.to_message(self.value_type))
         if self.metadata is not None:
-            message.metadata.MergeFrom(self.metadata.to_message(self.value_type))
+            message.metadata.MergeFrom(
+                self.metadata.to_message(self.value_type))
         return message
 
     def to_dict(self) -> Dict[str, Any]:
         out_dict = {'path': self.path}
         if self.value is not None:
             out_dict['value'] = self.value.to_dict()
         if self.actuator_target is not None:
@@ -448,20 +470,22 @@
 
 
 class BaseVSSClient:
     def __init__(
         self,
         host: str,
         port: int,
+        token: str = None,
         root_certificates: Optional[Path] = None,
         private_key: Optional[Path] = None,
         certificate_chain: Optional[Path] = None,
         *,
         ensure_startup_connection: bool = True,
     ):
+        self.authorization_header = self.get_authorization_header(token)
         self.target_host = f'{host}:{port}'
         self.root_certificates = root_certificates
         self.private_key = private_key
         self.certificate_chain = certificate_chain
         self.ensure_startup_connection = ensure_startup_connection
         self.client_stub = None
 
@@ -472,15 +496,16 @@
             certificate_chain = self.certificate_chain.read_bytes()
             return grpc.ssl_channel_credentials(root_certificates, private_key, certificate_chain)
         return None
 
     def _prepare_get_request(self, entries: Iterable[EntryRequest]) -> val_pb2.GetRequest:
         req = val_pb2.GetRequest(entries=[])
         for entry in entries:
-            entry_request = val_pb2.EntryRequest(path=entry.path, view=entry.view.value, fields=[])
+            entry_request = val_pb2.EntryRequest(
+                path=entry.path, view=entry.view.value, fields=[])
             for field in entry.fields:
                 entry_request.fields.append(field.value)
             req.entries.append(entry_request)
         logger.debug("%s: %s", type(req).__name__, req)
         return req
 
     def _process_get_response(self, response: val_pb2.GetResponse) -> List[DataEntry]:
@@ -522,35 +547,54 @@
         self._raise_if_invalid(response)
 
     def _prepare_subscribe_request(
         self, entries: Iterable[SubscribeEntry],
     ) -> val_pb2.SubscribeRequest:
         req = val_pb2.SubscribeRequest()
         for entry in entries:
-            entry_request = val_pb2.SubscribeEntry(path=entry.path, view=entry.view.value, fields=[])
+            entry_request = val_pb2.SubscribeEntry(
+                path=entry.path, view=entry.view.value, fields=[])
             for field in entry.fields:
                 entry_request.fields.append(field.value)
             req.entries.append(entry_request)
         logger.debug("%s: %s", type(req).__name__, req)
         return req
 
     def _raise_if_invalid(self, response):
         if response.HasField('error'):
-            error = json_format.MessageToDict(response.error, preserving_proto_field_name=True)
+            error = json_format.MessageToDict(
+                response.error, preserving_proto_field_name=True)
         else:
             error = {}
         if response.errors:
-            errors = [json_format.MessageToDict(err, preserving_proto_field_name=True) for err in response.errors]
+            errors = [json_format.MessageToDict(
+                err, preserving_proto_field_name=True) for err in response.errors]
         else:
             errors = []
         if (error and error['code'] != http.HTTPStatus.OK) or any(
             sub_error['error']['code'] != http.HTTPStatus.OK for sub_error in errors
         ):
             raise VSSClientError(error, errors)
 
+    def get_authorization_header(self, token: str):
+        if token is None:
+            return None
+        return "Bearer " + token
+
+    def generate_metadata_header(self, metadata: list, header=None) -> list:
+        if header == None:
+            header = self.authorization_header
+        if metadata:
+            metadata = dict(metadata)
+        else:
+            metadata = dict()
+        # Overrides old authorization header. This is intentional.
+        metadata["authorization"] = header
+        return list(metadata.items())
+
 
 class VSSClient(BaseVSSClient):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.channel = None
         self.exit_stack = contextlib.ExitStack()
 
@@ -558,16 +602,23 @@
         creds = self._load_creds()
         if creds is not None:
             channel = grpc.secure_channel(self.target_host, creds)
         else:
             channel = grpc.insecure_channel(self.target_host)
         self.channel = self.exit_stack.enter_context(channel)
         self.client_stub = val_pb2_grpc.VALStub(self.channel)
+        if self.authorization_header is None:
+            logger.debug(
+                "Can not ensure startup connection without token to authorize")
         if self.ensure_startup_connection:
-            logger.debug("Connected to server: %s", self.get_server_info())
+            try:
+                info = self.get_server_info()
+                logger.debug("Connected to server: %s", info)
+            except:
+                logger.debug("Connection could not be ensured")
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.exit_stack.close()
         self.client_stub = None
         self.channel = None
 
@@ -597,15 +648,15 @@
             target_values = client.get_target_values([
                 'Vehicle.ADAS.ABS.IsActive',
             ])
             is_abs_to_become_active = target_values['Vehicle.ADAS.ABS.IsActive'].value
         """
         entries = self.get(entries=(
             EntryRequest(path, View.TARGET_VALUE, (Field.ACTUATOR_TARGET,),
-        ) for path in paths), **rpc_kwargs)
+                         ) for path in paths), **rpc_kwargs)
         return {entry.path: entry.actuator_target for entry in entries}
 
     def get_metadata(
         self, paths: Iterable[str], field: MetadataField = MetadataField.ALL, **rpc_kwargs,
     ) -> Dict[str, Metadata]:
         """
         Parameters:
@@ -631,25 +682,27 @@
         Example:
             client.set_current_values({
                 'Vehicle.Speed': Datapoint(42),
                 'Vehicle.ADAS.ABS.IsActive': Datapoint(False),
             })
         """
         self.set(
-            updates=[EntryUpdate(DataEntry(path, value=dp), (Field.VALUE,)) for path, dp in updates.items()],
+            updates=[EntryUpdate(DataEntry(path, value=dp), (Field.VALUE,))
+                     for path, dp in updates.items()],
             **rpc_kwargs,
         )
 
     def set_target_values(self, updates: Dict[str, Datapoint], **rpc_kwargs) -> None:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         Example:
-            client.set_target_values({'Vehicle.ADAS.ABS.IsActive': Datapoint(True)})
+            client.set_target_values(
+                {'Vehicle.ADAS.ABS.IsActive': Datapoint(True)})
         """
         self.set(updates=[EntryUpdate(
             DataEntry(path, actuator_target=dp), (Field.ACTUATOR_TARGET,),
         ) for path, dp in updates.items()], **rpc_kwargs)
 
     def set_metadata(
         self, updates: Dict[str, Metadata], field: MetadataField = MetadataField.ALL, **rpc_kwargs,
@@ -676,15 +729,16 @@
             for updates in client.subscribe_current_values([
                 'Vehicle.Speed', 'Vehicle.ADAS.ABS.IsActive',
             ]):
                 for path, dp in updates.items():
                     print(f"Current value for {path} is now: {dp.value}")
         """
         for updates in self.subscribe(
-            entries=(SubscribeEntry(path, View.CURRENT_VALUE, (Field.VALUE,)) for path in paths),
+            entries=(SubscribeEntry(path, View.CURRENT_VALUE, (Field.VALUE,))
+                     for path in paths),
             **rpc_kwargs,
         ):
             yield {update.entry.path: update.entry.value for update in updates}
 
     def subscribe_target_values(self, paths: Iterable[str], **rpc_kwargs) -> Iterator[Dict[str, Datapoint]]:
         """
         Parameters:
@@ -694,15 +748,16 @@
             async for updates in client.subscribe_target_values([
                 'Vehicle.ADAS.ABS.IsActive',
             ]):
                 for path, dp in updates.items():
                     print(f"Target value for {path} is now: {dp.value}")
         """
         for updates in self.subscribe(
-            entries=(SubscribeEntry(path, View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)) for path in paths),
+            entries=(SubscribeEntry(path, View.TARGET_VALUE,
+                     (Field.ACTUATOR_TARGET,)) for path in paths),
             **rpc_kwargs,
         ):
             yield {update.entry.path: update.entry.actuator_target for update in updates}
 
     def subscribe_metadata(
         self, paths: Iterable[str],
         field: MetadataField = MetadataField.ALL,
@@ -717,72 +772,93 @@
                 'Vehicle.Speed',
                 'Vehicle.ADAS.ABS.IsActive',
             ]):
                 for path, md in updates.items():
                     print(f"Metadata for {path} are now: {md.to_dict()}")
         """
         for updates in self.subscribe(
-            entries=(SubscribeEntry(path, View.METADATA, (Field(field.value),)) for path in paths),
+            entries=(SubscribeEntry(path, View.METADATA, (Field(field.value),))
+                     for path in paths),
             **rpc_kwargs,
         ):
             yield {update.entry.path: update.entry.metadata for update in updates}
 
-
     def get(self, *, entries: Iterable[EntryRequest], **rpc_kwargs) -> List[DataEntry]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
+        rpc_kwargs["metadata"] = self.generate_metadata_header(
+            rpc_kwargs.get("metadata"))
         req = self._prepare_get_request(entries)
         try:
             resp = self.client_stub.Get(req, **rpc_kwargs)
         except RpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         return self._process_get_response(resp)
 
     def set(self, *, updates: Collection[EntryUpdate], **rpc_kwargs) -> None:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
+        rpc_kwargs["metadata"] = self.generate_metadata_header(
+            rpc_kwargs.get("metadata"))
         paths_with_required_type = self._get_paths_with_required_type(updates)
         paths_without_type = [
             path for path, data_type in paths_with_required_type.items() if data_type is DataType.UNSPECIFIED
         ]
-        paths_with_required_type.update(self.get_value_types(paths_without_type, **rpc_kwargs))
+        paths_with_required_type.update(
+            self.get_value_types(paths_without_type, **rpc_kwargs))
         req = self._prepare_set_request(updates, paths_with_required_type)
         try:
             resp = self.client_stub.Set(req, **rpc_kwargs)
         except RpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         self._process_set_response(resp)
 
     def subscribe(self, *, entries: Iterable[SubscribeEntry], **rpc_kwargs) -> Iterator[List[EntryUpdate]]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
+        rpc_kwargs["metadata"] = self.generate_metadata_header(
+            rpc_kwargs.get("metadata"))
         req = self._prepare_subscribe_request(entries)
         resp_stream = self.client_stub.Subscribe(req, **rpc_kwargs)
         try:
             for resp in resp_stream:
                 logger.debug("%s: %s", type(resp).__name__, resp)
                 yield [EntryUpdate.from_message(update) for update in resp.updates]
         except RpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
 
+    def authorize(self, *, token: str, **rpc_kwargs) -> str:
+        rpc_kwargs["metadata"] = self.generate_metadata_header(
+            metadata=rpc_kwargs.get("metadata"), header=self.get_authorization_header(token))
+        req = val_pb2.GetServerInfoRequest()
+        try:
+            resp = self.client_stub.GetServerInfo(req, **rpc_kwargs)
+        except RpcError as exc:
+            raise VSSClientError.from_grpc_error(exc) from exc
+        logger.debug("%s: %s", type(resp).__name__, resp)
+        self.authorization_header = self.get_authorization_header(token)
+        return "Authenticated"
+
     def get_server_info(self, **rpc_kwargs) -> ServerInfo:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
+        rpc_kwargs["metadata"] = self.generate_metadata_header(
+            metadata=rpc_kwargs.get("metadata"))
         req = val_pb2.GetServerInfoRequest()
         logger.debug("%s: %s", type(req).__name__, req)
         try:
             resp = self.client_stub.GetServerInfo(req, **rpc_kwargs)
         except RpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         logger.debug("%s: %s", type(resp).__name__, resp)
@@ -794,12 +870,13 @@
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         req = self._prepare_get_request(entries)
         """
         if paths:
             entry_requests = (EntryRequest(
-                path=path, view=View.METADATA, fields=(Field.METADATA_DATA_TYPE,),
+                path=path, view=View.METADATA, fields=(
+                    Field.METADATA_DATA_TYPE,),
             ) for path in paths)
             entries = self.get(entries=entry_requests, **rpc_kwargs)
             return {entry.path: DataType(entry.metadata.data_type) for entry in entries}
         return {}
```

### Comparing `kuksa_client-0.3.1/kuksa_client/grpc/aio.py` & `kuksa_client-0.4.0a1/kuksa_client/grpc/aio.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,16 +60,23 @@
         creds = self._load_creds()
         if creds is not None:
             channel = grpc.aio.secure_channel(self.target_host, creds)
         else:
             channel = grpc.aio.insecure_channel(self.target_host)
         self.channel = await self.exit_stack.enter_async_context(channel)
         self.client_stub = val_pb2_grpc.VALStub(self.channel)
+        if self.authorization_header is None:
+            logger.debug(
+                "Can not ensure startup connection without token to authorize")
         if self.ensure_startup_connection:
-            logger.debug("Connected to server: %s", await self.get_server_info())
+            try:
+                info = await self.get_server_info()
+                logger.debug("Connected to server: %s", info)
+            except:
+                logger.debug("Connection could not be ensured")
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback):
         await self.exit_stack.aclose()
         self.client_stub = None
         self.channel = None
 
@@ -82,15 +89,16 @@
             current_values = await client.get_current_values([
                 'Vehicle.Speed',
                 'Vehicle.ADAS.ABS.IsActive',
             ])
             speed_value = current_values['Vehicle.Speed'].value
         """
         entries = await self.get(
-            entries=(EntryRequest(path, View.CURRENT_VALUE, (Field.VALUE,)) for path in paths),
+            entries=(EntryRequest(path, View.CURRENT_VALUE, (Field.VALUE,))
+                     for path in paths),
             **rpc_kwargs,
         )
         return {entry.path: entry.value for entry in entries}
 
     async def get_target_values(self, paths: Iterable[str], **rpc_kwargs) -> Dict[str, Datapoint]:
         """
         Parameters:
@@ -100,16 +108,16 @@
             target_values = await client.get_target_values([
                 'Vehicle.ADAS.ABS.IsActive',
             ])
             is_abs_to_become_active = target_values['Vehicle.ADAS.ABS.IsActive'].value
         """
         entries = await self.get(entries=(
             EntryRequest(path, View.TARGET_VALUE, (Field.ACTUATOR_TARGET,),
-            **rpc_kwargs,
-        ) for path in paths))
+                         **rpc_kwargs,
+                         ) for path in paths))
         return {entry.path: entry.actuator_target for entry in entries}
 
     async def get_metadata(
         self, paths: Iterable[str], field: MetadataField = MetadataField.ALL, **rpc_kwargs,
     ) -> Dict[str, Metadata]:
         """
         Parameters:
@@ -119,15 +127,16 @@
             metadata = await client.get_metadata([
                 'Vehicle.Speed',
                 'Vehicle.ADAS.ABS.IsActive',
             ], MetadataField.UNIT)
             speed_unit = metadata['Vehicle.Speed'].unit
         """
         entries = await self.get(
-            entries=(EntryRequest(path, View.METADATA, (Field(field.value),)) for path in paths),
+            entries=(EntryRequest(path, View.METADATA, (Field(field.value),))
+                     for path in paths),
             **rpc_kwargs,
         )
         return {entry.path: entry.metadata for entry in entries}
 
     async def set_current_values(self, updates: Dict[str, Datapoint], **rpc_kwargs) -> None:
         """
         Parameters:
@@ -136,15 +145,16 @@
         Example:
             await client.set_current_values({
                 'Vehicle.Speed': Datapoint(42),
                 'Vehicle.ADAS.ABS.IsActive': Datapoint(False),
             })
         """
         await self.set(
-            updates=[EntryUpdate(DataEntry(path, value=dp), (Field.VALUE,)) for path, dp in updates.items()],
+            updates=[EntryUpdate(DataEntry(path, value=dp), (Field.VALUE,))
+                     for path, dp in updates.items()],
             **rpc_kwargs,
         )
 
     async def set_target_values(self, updates: Dict[str, Datapoint], **rpc_kwargs) -> None:
         """
         Parameters:
             rpc_kwargs
@@ -181,15 +191,16 @@
             async for updates in client.subscribe_current_values([
                 'Vehicle.Speed', 'Vehicle.ADAS.ABS.IsActive',
             ]):
                 for path, dp in updates.items():
                     print(f"Current value for {path} is now: {dp.value}")
         """
         async for updates in self.subscribe(
-            entries=(SubscribeEntry(path, View.CURRENT_VALUE, (Field.VALUE,)) for path in paths),
+            entries=(SubscribeEntry(path, View.CURRENT_VALUE, (Field.VALUE,))
+                     for path in paths),
             **rpc_kwargs,
         ):
             yield {update.entry.path: update.entry.value for update in updates}
 
     async def subscribe_target_values(self, paths: Iterable[str], **rpc_kwargs) -> AsyncIterator[Dict[str, Datapoint]]:
         """
         Parameters:
@@ -199,15 +210,16 @@
             async for updates in client.subscribe_target_values([
                 'Vehicle.ADAS.ABS.IsActive',
             ]):
                 for path, dp in updates.items():
                     print(f"Target value for {path} is now: {dp.value}")
         """
         async for updates in self.subscribe(
-            entries=(SubscribeEntry(path, View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)) for path in paths),
+            entries=(SubscribeEntry(path, View.TARGET_VALUE,
+                     (Field.ACTUATOR_TARGET,)) for path in paths),
             **rpc_kwargs,
         ):
             yield {update.entry.path: update.entry.actuator_target for update in updates}
 
     async def subscribe_metadata(
         self, paths: Iterable[str],
         field: MetadataField = MetadataField.ALL,
@@ -222,77 +234,95 @@
                 'Vehicle.Speed',
                 'Vehicle.ADAS.ABS.IsActive',
             ]):
                 for path, md in updates.items():
                     print(f"Metadata for {path} are now: {md.to_dict()}")
         """
         async for updates in self.subscribe(
-            entries=(SubscribeEntry(path, View.METADATA, (Field(field.value),)) for path in paths),
+            entries=(SubscribeEntry(path, View.METADATA, (Field(field.value),))
+                     for path in paths),
             **rpc_kwargs,
         ):
             yield {update.entry.path: update.entry.metadata for update in updates}
 
     async def get(self, *, entries: Iterable[EntryRequest], **rpc_kwargs) -> List[DataEntry]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
+        rpc_kwargs["metadata"] = self.generate_metadata_header(
+            rpc_kwargs.get("metadata"))
         req = self._prepare_get_request(entries)
         try:
             resp = await self.client_stub.Get(req, **rpc_kwargs)
         except AioRpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         return self._process_get_response(resp)
 
     async def set(self, *, updates: Collection[EntryUpdate], **rpc_kwargs) -> None:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
+        rpc_kwargs["metadata"] = self.generate_metadata_header(
+            rpc_kwargs.get("metadata"))
         paths_with_required_type = self._get_paths_with_required_type(updates)
         paths_without_type = [
             path for path, data_type in paths_with_required_type.items() if data_type is DataType.UNSPECIFIED
         ]
         paths_with_required_type.update(await self.get_value_types(paths_without_type, **rpc_kwargs))
         req = self._prepare_set_request(updates, paths_with_required_type)
         try:
             resp = await self.client_stub.Set(req, **rpc_kwargs)
         except AioRpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         self._process_set_response(resp)
 
-    async def authorize(self, *, token: str) -> str:
-        raise NotImplementedError('"authorize" is not yet implemented')
-
     async def subscribe(self, *,
-        entries: Iterable[SubscribeEntry],
-        **rpc_kwargs,
-    ) -> AsyncIterator[List[EntryUpdate]]:
+                        entries: Iterable[SubscribeEntry],
+                        **rpc_kwargs,
+                        ) -> AsyncIterator[List[EntryUpdate]]:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
+        rpc_kwargs["metadata"] = self.generate_metadata_header(
+            rpc_kwargs.get("metadata"))
         req = self._prepare_subscribe_request(entries)
         resp_stream = self.client_stub.Subscribe(req, **rpc_kwargs)
         try:
             async for resp in resp_stream:
                 logger.debug("%s: %s", type(resp).__name__, resp)
                 yield [EntryUpdate.from_message(update) for update in resp.updates]
         except AioRpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
 
+    async def authorize(self, token: str, **rpc_kwargs) -> str:
+        rpc_kwargs["metadata"] = self.generate_metadata_header(
+            metadata=rpc_kwargs.get("metadata"), header=self.get_authorization_header(token))
+        req = val_pb2.GetServerInfoRequest()
+        try:
+            resp = await self.client_stub.GetServerInfo(req, **rpc_kwargs)
+        except AioRpcError as exc:
+            raise VSSClientError.from_grpc_error(exc) from exc
+        logger.debug("%s: %s", type(resp).__name__, resp)
+        self.authorization_header = self.get_authorization_header(token)
+        return "Authenticated"
+
     async def get_server_info(self, **rpc_kwargs) -> ServerInfo:
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
+        rpc_kwargs["metadata"] = self.generate_metadata_header(
+            metadata=rpc_kwargs.get("metadata"))
         req = val_pb2.GetServerInfoRequest()
         logger.debug("%s: %s", type(req).__name__, req)
         try:
             resp = await self.client_stub.GetServerInfo(req, **rpc_kwargs)
         except AioRpcError as exc:
             raise VSSClientError.from_grpc_error(exc) from exc
         logger.debug("%s: %s", type(resp).__name__, resp)
@@ -303,43 +333,46 @@
         """
         Parameters:
             rpc_kwargs
                 grpc.*MultiCallable kwargs e.g. timeout, metadata, credentials.
         """
         if paths:
             entry_requests = (EntryRequest(
-                path=path, view=View.METADATA, fields=(Field.METADATA_DATA_TYPE,),
+                path=path, view=View.METADATA, fields=(
+                    Field.METADATA_DATA_TYPE,),
             ) for path in paths)
             entries = await self.get(entries=entry_requests, **rpc_kwargs)
             return {entry.path: DataType(entry.metadata.data_type) for entry in entries}
         return {}
 
 
 class SubscriberManager:
     def __init__(self, client: VSSClient):
         self.client = client
         self.subscribers = {}
 
     async def add_subscriber(self,
-        subscribe_response_stream: AsyncIterator[List[EntryUpdate]],
-        callback: Callable[[Iterable[EntryUpdate]], None],
-    ) -> uuid.UUID:
+                             subscribe_response_stream: AsyncIterator[List[EntryUpdate]],
+                             callback: Callable[[Iterable[EntryUpdate]], None],
+                             ) -> uuid.UUID:
         # We expect the first SubscribeResponse to be immediately available and to only hold a status
         await subscribe_response_stream.__aiter__().__anext__()  # pylint: disable=unnecessary-dunder-call
 
         sub_id = uuid.uuid4()
-        new_sub_task = asyncio.create_task(self._subscriber_loop(subscribe_response_stream, callback))
+        new_sub_task = asyncio.create_task(
+            self._subscriber_loop(subscribe_response_stream, callback))
         self.subscribers[sub_id] = new_sub_task
         return sub_id
 
     async def remove_subscriber(self, subscription_id: uuid.UUID):
         try:
             subscriber_task = self.subscribers.pop(subscription_id)
         except KeyError as exc:
-            raise ValueError(f"Could not find subscription {str(subscription_id)}") from exc
+            raise ValueError(
+                f"Could not find subscription {str(subscription_id)}") from exc
         subscriber_task.cancel()
         try:
             await subscriber_task
         except asyncio.CancelledError:
             pass
 
     async def _subscriber_loop(
```

### Comparing `kuksa_client-0.3.1/kuksa_client/logo` & `kuksa_client-0.4.0a1/kuksa_client/logo`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/kuksa_client.egg-info/PKG-INFO` & `kuksa_client-0.4.0a1/kuksa_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuksa-client
-Version: 0.3.1
+Version: 0.4.0a1
 Summary: kuksa.val python clients and SDK
 Home-page: https://github.com/eclipse/kuksa.val
 Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
 Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
 Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
 Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
 Classifier: Intended Audience :: Developers
```

### Comparing `kuksa_client-0.3.1/kuksa_client.egg-info/SOURCES.txt` & `kuksa_client-0.4.0a1/kuksa_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/pyproject.toml` & `kuksa_client-0.4.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/setup.cfg` & `kuksa_client-0.4.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/setup.py` & `kuksa_client-0.4.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/tests/conftest.py` & `kuksa_client-0.4.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.3.1/tests/test_grpc.py` & `kuksa_client-0.4.0a1/tests/test_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,18 +67,22 @@
         expected_client_error = VSSClientError(
             error={'code': 3, 'reason': 'invalid argument', 'message': 'No datapoints requested'}, errors=[],
         )
         assert client_error.error == expected_client_error.error
         assert client_error.errors == expected_client_error.errors
 
     def test_to_dict(self):
-        error = types_pb2.Error(code=404, reason='not_found', message="Does.Not.Exist not found")
-        errors = (types_pb2.DataEntryError(path='Does.Not.Exist', error=error),)
-        error = json_format.MessageToDict(error, preserving_proto_field_name=True)
-        errors = [json_format.MessageToDict(err, preserving_proto_field_name=True) for err in errors]
+        error = types_pb2.Error(
+            code=404, reason='not_found', message="Does.Not.Exist not found")
+        errors = (types_pb2.DataEntryError(
+            path='Does.Not.Exist', error=error),)
+        error = json_format.MessageToDict(
+            error, preserving_proto_field_name=True)
+        errors = [json_format.MessageToDict(
+            err, preserving_proto_field_name=True) for err in errors]
 
         assert VSSClientError(error, errors).to_dict() == {
             'error': {'code': 404, 'reason': 'not_found', 'message': "Does.Not.Exist not found"},
             'errors': [{'path': 'Does.Not.Exist', 'error': {
                 'code': 404, 'reason': 'not_found', 'message': "Does.Not.Exist not found",
             }}],
         }
@@ -86,16 +90,18 @@
 
 class TestMetadata:
     def test_to_message_empty(self):
         assert Metadata().to_message() == types_pb2.Metadata()
 
     def test_to_message_value_restriction_without_value_type(self):
         with pytest.raises(ValueError) as exc_info:
-            assert Metadata(value_restriction=ValueRestriction()).to_message() == types_pb2.Metadata()
-        assert exc_info.value.args == ("Cannot set value_restriction from data type UNSPECIFIED",)
+            assert Metadata(value_restriction=ValueRestriction()
+                            ).to_message() == types_pb2.Metadata()
+        assert exc_info.value.args == (
+            "Cannot set value_restriction from data type UNSPECIFIED",)
 
     @pytest.mark.parametrize('value_type', (
         DataType.INT8,
         DataType.INT16,
         DataType.INT32,
         DataType.INT64,
         DataType.INT8_ARRAY,
@@ -114,15 +120,16 @@
         (-42, 42, [-42, 0, 42]),
     ])
     def test_to_message_signed_value_restriction(self, value_type, min_value, max_value, allowed_values):
         if (min_value, max_value, allowed_values) == (None, None, None):
             expected_message = types_pb2.Metadata()
         else:
             expected_message = types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
-                signed=types_pb2.ValueRestrictionInt(min=min_value, max=max_value, allowed_values=allowed_values),
+                signed=types_pb2.ValueRestrictionInt(
+                    min=min_value, max=max_value, allowed_values=allowed_values),
             ))
         assert Metadata(value_restriction=ValueRestriction(
             min=min_value, max=max_value, allowed_values=allowed_values,
         )).to_message(value_type) == expected_message
 
     @pytest.mark.parametrize('value_type', (
         DataType.UINT8,
@@ -144,15 +151,16 @@
         (0, 42, [0, 12, 42]),
     ])
     def test_to_message_unsigned_value_restriction(self, value_type, min_value, max_value, allowed_values):
         if (min_value, max_value, allowed_values) == (None, None, None):
             expected_message = types_pb2.Metadata()
         else:
             expected_message = types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
-                unsigned=types_pb2.ValueRestrictionUint(min=min_value, max=max_value, allowed_values=allowed_values),
+                unsigned=types_pb2.ValueRestrictionUint(
+                    min=min_value, max=max_value, allowed_values=allowed_values),
             ))
         assert Metadata(value_restriction=ValueRestriction(
             min=min_value, max=max_value, allowed_values=allowed_values,
         )).to_message(value_type) == expected_message
 
     @pytest.mark.parametrize('value_type', (
         DataType.FLOAT,
@@ -171,72 +179,82 @@
         (0.5, 41.5, [0.5, 12., 41.5]),
     ])
     def test_to_message_float_value_restriction(self, value_type, min_value, max_value, allowed_values):
         if (min_value, max_value, allowed_values) == (None, None, None):
             expected_message = types_pb2.Metadata()
         else:
             expected_message = types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
-                floating_point=types_pb2.ValueRestrictionFloat(min=min_value, max=max_value, allowed_values=allowed_values),
+                floating_point=types_pb2.ValueRestrictionFloat(
+                    min=min_value, max=max_value, allowed_values=allowed_values),
             ))
         assert Metadata(value_restriction=ValueRestriction(
             min=min_value, max=max_value, allowed_values=allowed_values,
         )).to_message(value_type) == expected_message
 
     @pytest.mark.parametrize('value_type', (DataType.STRING, DataType.STRING_ARRAY))
     @pytest.mark.parametrize('allowed_values', [None, [], ['Hello', 'world']])
     def test_to_message_string_value_restriction(self, value_type, allowed_values):
         if allowed_values is None:
             expected_message = types_pb2.Metadata()
         else:
             expected_message = types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
-                string=types_pb2.ValueRestrictionString(allowed_values=allowed_values),
+                string=types_pb2.ValueRestrictionString(
+                    allowed_values=allowed_values),
             ))
         assert Metadata(value_restriction=ValueRestriction(
             allowed_values=allowed_values,
         )).to_message(value_type) == expected_message
 
     @pytest.mark.parametrize('metadata_dict, init_kwargs', [
         ({}, {}),
         ({'entry_type': 1}, {'entry_type': EntryType.ATTRIBUTE}),
-        ({'entry_type': EntryType.ATTRIBUTE}, {'entry_type': EntryType.ATTRIBUTE}),
+        ({'entry_type': EntryType.ATTRIBUTE},
+         {'entry_type': EntryType.ATTRIBUTE}),
         ({'entry_type': 'ATTRIBUTE'}, {'entry_type': EntryType.ATTRIBUTE}),
         ({'data_type': 1}, {'data_type': DataType.STRING}),
         ({'data_type': DataType.STRING}, {'data_type': DataType.STRING}),
         ({'data_type': 'STRING'}, {'data_type': DataType.STRING}),
-        ({'description': 'a real description'}, {'description': 'a real description'}),
+        ({'description': 'a real description'},
+         {'description': 'a real description'}),
         ({'comment': 'a real comment'}, {'comment': 'a real comment'}),
-        ({'deprecation': 'a real deprecation'}, {'deprecation': 'a real deprecation'}),
+        ({'deprecation': 'a real deprecation'},
+         {'deprecation': 'a real deprecation'}),
         ({'unit': 'a real unit'}, {'unit': 'a real unit'}),
         ({'value_restriction': {}}, {'value_restriction': ValueRestriction()}),
-        ({'value_restriction': {'min': 12}}, {'value_restriction': ValueRestriction(min=12)}),
-        ({'value_restriction': {'max': 42}}, {'value_restriction': ValueRestriction(max=42)}),
+        ({'value_restriction': {'min': 12}}, {
+         'value_restriction': ValueRestriction(min=12)}),
+        ({'value_restriction': {'max': 42}}, {
+         'value_restriction': ValueRestriction(max=42)}),
         ({'value_restriction': {'allowed_values': [-42, 42]}}, {
             'value_restriction': ValueRestriction(allowed_values=[-42, 42]),
         }),
         ({'value_restriction': {'min': -42, 'max': 42, 'allowed_values': [-42, 42]}}, {
             'value_restriction': ValueRestriction(min=-42, max=42, allowed_values=[-42, 42]),
         }),
     ])
     def test_from_dict(self, metadata_dict, init_kwargs):
         assert Metadata.from_dict(metadata_dict) == Metadata(**init_kwargs)
 
     @pytest.mark.parametrize('init_kwargs, metadata_dict', [
         ({}, {'data_type': 'UNSPECIFIED', 'entry_type': 'UNSPECIFIED'}),
-        ({'entry_type': EntryType.ATTRIBUTE}, {'data_type': 'UNSPECIFIED', 'entry_type': 'ATTRIBUTE'}),
-        ({'data_type': DataType.STRING}, {'data_type': 'STRING', 'entry_type': 'UNSPECIFIED'}),
+        ({'entry_type': EntryType.ATTRIBUTE}, {
+         'data_type': 'UNSPECIFIED', 'entry_type': 'ATTRIBUTE'}),
+        ({'data_type': DataType.STRING}, {
+         'data_type': 'STRING', 'entry_type': 'UNSPECIFIED'}),
         ({'description': 'a real description'}, {
             'data_type': 'UNSPECIFIED', 'entry_type': 'UNSPECIFIED', 'description': 'a real description',
         }),
         ({'comment': 'a real comment'}, {
             'data_type': 'UNSPECIFIED', 'entry_type': 'UNSPECIFIED', 'comment': 'a real comment',
         }),
         ({'deprecation': 'a real deprecation'}, {
             'data_type': 'UNSPECIFIED', 'entry_type': 'UNSPECIFIED', 'deprecation': 'a real deprecation',
         }),
-        ({'unit': 'a real unit'}, {'data_type': 'UNSPECIFIED', 'entry_type': 'UNSPECIFIED', 'unit': 'a real unit'}),
+        ({'unit': 'a real unit'}, {'data_type': 'UNSPECIFIED',
+         'entry_type': 'UNSPECIFIED', 'unit': 'a real unit'}),
         ({'value_restriction': ValueRestriction()}, {
             'data_type': 'UNSPECIFIED', 'entry_type': 'UNSPECIFIED', 'value_restriction': {},
         }),
         ({'value_restriction': ValueRestriction(min=12)}, {
             'data_type': 'UNSPECIFIED', 'entry_type': 'UNSPECIFIED',
             'value_restriction': {'min': 12},
         }),
@@ -263,24 +281,26 @@
         (DataType.BOOLEAN, ('False',), types_pb2.Datapoint(bool=False)),
         (DataType.BOOLEAN, ('false',), types_pb2.Datapoint(bool=False)),
         (DataType.BOOLEAN, ('F',), types_pb2.Datapoint(bool=False)),
         (DataType.BOOLEAN, ('f',), types_pb2.Datapoint(bool=False)),
         (DataType.BOOLEAN, (True, datetime.datetime(2022, 11, 16, tzinfo=datetime.timezone.utc)), types_pb2.Datapoint(
             bool=True, timestamp=timestamp_pb2.Timestamp(seconds=1668556800),
         )),
-        (DataType.INT8_ARRAY, ([-128, 127],), types_pb2.Datapoint(int32_array=types_pb2.Int32Array(values=[-128, 127]))),
+        (DataType.INT8_ARRAY, ([-128, 127],), types_pb2.Datapoint(
+            int32_array=types_pb2.Int32Array(values=[-128, 127]))),
     ])
     def test_to_message(self, value_type, init_args, message):
         assert Datapoint(*init_args).to_message(value_type) == message
 
     @pytest.mark.parametrize('value_type', [DataType.UNSPECIFIED, DataType.TIMESTAMP, DataType.TIMESTAMP_ARRAY])
     def test_to_message_unsupported_value_type(self, value_type):
         with pytest.raises(ValueError) as exc_info:
             Datapoint(42).to_message(value_type)
-        assert exc_info.value.args[0].startswith('Cannot determine which field to set with data type')
+        assert exc_info.value.args[0].startswith(
+            'Cannot determine which field to set with data type')
 
     @pytest.mark.parametrize('init_kwargs, datapoint_dict', [
         ({}, {}),
         ({'value': 42}, {'value': 42}),
         ({'timestamp': datetime.datetime(2022, 11, 16, tzinfo=datetime.timezone.utc)}, {
             'timestamp': '2022-11-16T00:00:00+00:00',
         }),
@@ -293,137 +313,161 @@
 
 
 class TestDataEntry:
     @pytest.mark.parametrize('value, actuator_target, metadata, entry_dict', [
         (None, None, None, {}),
         (Datapoint(42), None, None, {'value': {'value': 42}}),
         (None, Datapoint(42), None, {'actuator_target': {'value': 42}}),
-        (None, None, Metadata(), {'metadata': {'data_type': 'UNSPECIFIED', 'entry_type': 'UNSPECIFIED'}}),
+        (None, None, Metadata(), {'metadata': {
+         'data_type': 'UNSPECIFIED', 'entry_type': 'UNSPECIFIED'}}),
     ])
     def test_to_dict(self, value, actuator_target, metadata, entry_dict):
         entry_dict.update({'path': 'Test.Path'})
-        assert DataEntry('Test.Path', value, actuator_target, metadata).to_dict() == entry_dict
+        assert DataEntry('Test.Path', value, actuator_target,
+                         metadata).to_dict() == entry_dict
 
 
 class TestEntryUpdate:
     @pytest.mark.parametrize('entry, fields, update_dict', [
-        (DataEntry(path='Test.Path'), (), {'entry': {'path': 'Test.Path'}, 'fields': []}),
+        (DataEntry(path='Test.Path'), (), {
+         'entry': {'path': 'Test.Path'}, 'fields': []}),
         (DataEntry(path='Test.Path', value=Datapoint(42)), (Field.VALUE,), {
             'entry': {'path': 'Test.Path', 'value': {'value': 42}}, 'fields': ['VALUE'],
         }),
     ])
     def test_to_dict(self, entry, fields, update_dict):
         assert EntryUpdate(entry, fields).to_dict() == update_dict
 
 
 @pytest.mark.asyncio
 class TestVSSClient:
     @pytest.mark.usefixtures('secure_val_server')
     async def test_secure_connection(self, unused_tcp_port, resources_path, val_servicer):
-        val_servicer.GetServerInfo.return_value = val_pb2.GetServerInfoResponse(name='test_server', version='1.2.3')
+        val_servicer.GetServerInfo.return_value = val_pb2.GetServerInfoResponse(
+            name='test_server', version='1.2.3')
         async with VSSClient('localhost', unused_tcp_port,
-            root_certificates=resources_path / 'test-ca.pem',
-            private_key=resources_path / 'test-client.key',
-            certificate_chain=resources_path / 'test-client.pem',
-        ):
+                             root_certificates=resources_path / 'test-ca.pem',
+                             private_key=resources_path / 'test-client.key',
+                             certificate_chain=resources_path / 'test-client.pem',
+                             ensure_startup_connection=True
+                             ):
             assert val_servicer.GetServerInfo.call_count == 1
 
     async def test_get_current_values(self, mocker, unused_tcp_port):
         client = VSSClient('127.0.0.1', unused_tcp_port)
         mocker.patch.object(client, 'get', return_value=[
             DataEntry('Vehicle.Speed', value=Datapoint(
-                42.0, datetime.datetime(2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
+                42.0, datetime.datetime(
+                    2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
             )),
             DataEntry('Vehicle.ADAS.ABS.IsActive', value=Datapoint(True)),
             DataEntry('Vehicle.Chassis.Height', value=Datapoint(666)),
         ])
         assert await client.get_current_values([
             'Vehicle.Speed', 'Vehicle.ADAS.ABS.IsActive', 'Vehicle.Chassis.Height',
         ]) == {
             'Vehicle.Speed': Datapoint(
-                42.0, datetime.datetime(2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
+                42.0, datetime.datetime(
+                    2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
             ),
             'Vehicle.ADAS.ABS.IsActive': Datapoint(True),
             'Vehicle.Chassis.Height': Datapoint(666),
         }
         assert list(client.get.call_args_list[0][1]['entries']) == [
             EntryRequest('Vehicle.Speed', View.CURRENT_VALUE, (Field.VALUE,)),
-            EntryRequest('Vehicle.ADAS.ABS.IsActive', View.CURRENT_VALUE, (Field.VALUE,)),
-            EntryRequest('Vehicle.Chassis.Height', View.CURRENT_VALUE, (Field.VALUE,)),
+            EntryRequest('Vehicle.ADAS.ABS.IsActive',
+                         View.CURRENT_VALUE, (Field.VALUE,)),
+            EntryRequest('Vehicle.Chassis.Height',
+                         View.CURRENT_VALUE, (Field.VALUE,)),
         ]
 
     async def test_get_target_values(self, mocker, unused_tcp_port):
         client = VSSClient('127.0.0.1', unused_tcp_port)
         mocker.patch.object(client, 'get', return_value=[
             DataEntry('Vehicle.ADAS.ABS.IsActive', actuator_target=Datapoint(
-                True, datetime.datetime(2022, 11, 7, tzinfo=datetime.timezone.utc),
+                True, datetime.datetime(
+                    2022, 11, 7, tzinfo=datetime.timezone.utc),
             )),
-            DataEntry('Vehicle.Chassis.SteeringWheel.Tilt', actuator_target=Datapoint(42)),
+            DataEntry('Vehicle.Chassis.SteeringWheel.Tilt',
+                      actuator_target=Datapoint(42)),
         ])
         assert await client.get_target_values([
             'Vehicle.ADAS.ABS.IsActive', 'Vehicle.Chassis.SteeringWheel.Tilt',
         ]) == {
             'Vehicle.ADAS.ABS.IsActive': Datapoint(True, datetime.datetime(2022, 11, 7, tzinfo=datetime.timezone.utc)),
             'Vehicle.Chassis.SteeringWheel.Tilt': Datapoint(42),
         }
         assert list(client.get.call_args_list[0][1]['entries']) == [
-            EntryRequest('Vehicle.ADAS.ABS.IsActive', View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
-            EntryRequest('Vehicle.Chassis.SteeringWheel.Tilt', View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
+            EntryRequest('Vehicle.ADAS.ABS.IsActive',
+                         View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
+            EntryRequest('Vehicle.Chassis.SteeringWheel.Tilt',
+                         View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
         ]
 
     async def test_get_metadata(self, mocker, unused_tcp_port):
         client = VSSClient('127.0.0.1', unused_tcp_port)
         mocker.patch.object(client, 'get', return_value=[
-            DataEntry('Vehicle.Speed', metadata=Metadata(entry_type=EntryType.SENSOR)),
-            DataEntry('Vehicle.ADAS.ABS.IsActive', metadata=Metadata(entry_type=EntryType.ACTUATOR)),
-            DataEntry('Vehicle.Chassis.Height', metadata=Metadata(entry_type=EntryType.ATTRIBUTE)),
+            DataEntry('Vehicle.Speed', metadata=Metadata(
+                entry_type=EntryType.SENSOR)),
+            DataEntry('Vehicle.ADAS.ABS.IsActive', metadata=Metadata(
+                entry_type=EntryType.ACTUATOR)),
+            DataEntry('Vehicle.Chassis.Height', metadata=Metadata(
+                entry_type=EntryType.ATTRIBUTE)),
         ])
         assert await client.get_metadata([
             'Vehicle.Speed',
             'Vehicle.ADAS.ABS.IsActive',
             'Vehicle.Chassis.Height',
         ], field=MetadataField.ENTRY_TYPE) == {
             'Vehicle.Speed': Metadata(entry_type=EntryType.SENSOR),
             'Vehicle.ADAS.ABS.IsActive': Metadata(entry_type=EntryType.ACTUATOR),
             'Vehicle.Chassis.Height': Metadata(entry_type=EntryType.ATTRIBUTE),
         }
         assert list(client.get.call_args_list[0][1]['entries']) == [
-            EntryRequest('Vehicle.Speed', View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
-            EntryRequest('Vehicle.ADAS.ABS.IsActive', View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
-            EntryRequest('Vehicle.Chassis.Height', View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
+            EntryRequest('Vehicle.Speed', View.METADATA,
+                         (Field.METADATA_ENTRY_TYPE,)),
+            EntryRequest('Vehicle.ADAS.ABS.IsActive',
+                         View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
+            EntryRequest('Vehicle.Chassis.Height', View.METADATA,
+                         (Field.METADATA_ENTRY_TYPE,)),
         ]
 
     async def test_set_current_values(self, mocker, unused_tcp_port):
         client = VSSClient('127.0.0.1', unused_tcp_port)
         mocker.patch.object(client, 'set')
         await client.set_current_values({
             'Vehicle.Speed': Datapoint(42.0, datetime.datetime(2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc)),
             'Vehicle.ADAS.ABS.IsActive': Datapoint(True),
             'Vehicle.Chassis.Height': Datapoint(666),
         })
         assert list(client.set.call_args_list[0][1]['updates']) == [
             EntryUpdate(DataEntry('Vehicle.Speed', value=Datapoint(
-                42.0, datetime.datetime(2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
+                42.0, datetime.datetime(
+                    2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
             )), (Field.VALUE,)),
-            EntryUpdate(DataEntry('Vehicle.ADAS.ABS.IsActive', value=Datapoint(True)), (Field.VALUE,)),
-            EntryUpdate(DataEntry('Vehicle.Chassis.Height', value=Datapoint(666)), (Field.VALUE,)),
+            EntryUpdate(DataEntry('Vehicle.ADAS.ABS.IsActive',
+                        value=Datapoint(True)), (Field.VALUE,)),
+            EntryUpdate(DataEntry('Vehicle.Chassis.Height',
+                        value=Datapoint(666)), (Field.VALUE,)),
         ]
 
     async def test_set_target_values(self, mocker, unused_tcp_port):
         client = VSSClient('127.0.0.1', unused_tcp_port)
         mocker.patch.object(client, 'set')
         await client.set_target_values({
             'Vehicle.ADAS.ABS.IsActive': Datapoint(True, datetime.datetime(2022, 11, 7, tzinfo=datetime.timezone.utc)),
             'Vehicle.Chassis.SteeringWheel.Tilt': Datapoint(42),
         })
         assert list(client.set.call_args_list[0][1]['updates']) == [
             EntryUpdate(DataEntry('Vehicle.ADAS.ABS.IsActive', actuator_target=Datapoint(
-                True, datetime.datetime(2022, 11, 7, tzinfo=datetime.timezone.utc),
+                True, datetime.datetime(
+                    2022, 11, 7, tzinfo=datetime.timezone.utc),
             )), (Field.ACTUATOR_TARGET,)),
-            EntryUpdate(DataEntry('Vehicle.Chassis.SteeringWheel.Tilt', actuator_target=Datapoint(42)), (Field.ACTUATOR_TARGET,)),
+            EntryUpdate(DataEntry('Vehicle.Chassis.SteeringWheel.Tilt',
+                        actuator_target=Datapoint(42)), (Field.ACTUATOR_TARGET,)),
         ]
 
     async def test_set_metadata(self, mocker, unused_tcp_port):
         client = VSSClient('127.0.0.1', unused_tcp_port)
         mocker.patch.object(client, 'set')
         await client.set_metadata({
             'Vehicle.Speed': Metadata(entry_type=EntryType.SENSOR),
@@ -440,111 +484,132 @@
             EntryUpdate(DataEntry(
                 'Vehicle.Chassis.Height', metadata=Metadata(entry_type=EntryType.ATTRIBUTE),
             ), (Field.METADATA_ENTRY_TYPE,)),
         ]
 
     async def test_subscribe_current_values(self, mocker, unused_tcp_port):
         client = VSSClient('127.0.0.1', unused_tcp_port)
+
         async def subscribe_response_stream(**kwargs):
             yield [
                 EntryUpdate(DataEntry('Vehicle.Speed', value=Datapoint(
-                    42.0, datetime.datetime(2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
+                    42.0, datetime.datetime(
+                        2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
                 )), (Field.VALUE,)),
-                EntryUpdate(DataEntry('Vehicle.ADAS.ABS.IsActive', value=Datapoint(True)), (Field.VALUE,)),
-                EntryUpdate(DataEntry('Vehicle.Chassis.Height', value=Datapoint(666)), (Field.VALUE,)),
+                EntryUpdate(DataEntry('Vehicle.ADAS.ABS.IsActive',
+                            value=Datapoint(True)), (Field.VALUE,)),
+                EntryUpdate(DataEntry('Vehicle.Chassis.Height',
+                            value=Datapoint(666)), (Field.VALUE,)),
             ]
-        mocker.patch.object(client, 'subscribe', side_effect=subscribe_response_stream)
+        mocker.patch.object(client, 'subscribe',
+                            side_effect=subscribe_response_stream)
 
         received_updates = {}
         async for updates in client.subscribe_current_values([
             'Vehicle.Speed', 'Vehicle.ADAS.ABS.IsActive', 'Vehicle.Chassis.Height',
         ]):
             received_updates.update(updates)
 
         assert list(client.subscribe.call_args_list[0][1]['entries']) == [
-            SubscribeEntry('Vehicle.Speed', View.CURRENT_VALUE, (Field.VALUE,)),
-            SubscribeEntry('Vehicle.ADAS.ABS.IsActive', View.CURRENT_VALUE, (Field.VALUE,)),
-            SubscribeEntry('Vehicle.Chassis.Height', View.CURRENT_VALUE, (Field.VALUE,)),
+            SubscribeEntry('Vehicle.Speed',
+                           View.CURRENT_VALUE, (Field.VALUE,)),
+            SubscribeEntry('Vehicle.ADAS.ABS.IsActive',
+                           View.CURRENT_VALUE, (Field.VALUE,)),
+            SubscribeEntry('Vehicle.Chassis.Height',
+                           View.CURRENT_VALUE, (Field.VALUE,)),
         ]
         assert received_updates == {
             'Vehicle.Speed': Datapoint(42.0, datetime.datetime(2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc)),
             'Vehicle.ADAS.ABS.IsActive': Datapoint(True),
             'Vehicle.Chassis.Height': Datapoint(666),
         }
 
     async def test_subscribe_target_values(self, mocker, unused_tcp_port):
         client = VSSClient('127.0.0.1', unused_tcp_port)
+
         async def subscribe_response_stream(**kwargs):
             yield [
                 EntryUpdate(DataEntry('Vehicle.ADAS.ABS.IsActive', actuator_target=Datapoint(
-                    True, datetime.datetime(2022, 11, 7, tzinfo=datetime.timezone.utc),
+                    True, datetime.datetime(
+                        2022, 11, 7, tzinfo=datetime.timezone.utc),
                 )), (Field.ACTUATOR_TARGET,)),
-                EntryUpdate(DataEntry('Vehicle.Chassis.SteeringWheel.Tilt', actuator_target=Datapoint(42)), (Field.ACTUATOR_TARGET,)),
+                EntryUpdate(DataEntry('Vehicle.Chassis.SteeringWheel.Tilt',
+                            actuator_target=Datapoint(42)), (Field.ACTUATOR_TARGET,)),
             ]
-        mocker.patch.object(client, 'subscribe', side_effect=subscribe_response_stream)
+        mocker.patch.object(client, 'subscribe',
+                            side_effect=subscribe_response_stream)
 
         received_updates = {}
         async for updates in client.subscribe_target_values([
             'Vehicle.ADAS.ABS.IsActive', 'Vehicle.Chassis.SteeringWheel.Tilt',
         ]):
             received_updates.update(updates)
 
         assert list(client.subscribe.call_args_list[0][1]['entries']) == [
-            SubscribeEntry('Vehicle.ADAS.ABS.IsActive', View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
-            SubscribeEntry('Vehicle.Chassis.SteeringWheel.Tilt', View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
+            SubscribeEntry('Vehicle.ADAS.ABS.IsActive',
+                           View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
+            SubscribeEntry('Vehicle.Chassis.SteeringWheel.Tilt',
+                           View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
         ]
         assert received_updates == {
             'Vehicle.ADAS.ABS.IsActive': Datapoint(True, datetime.datetime(2022, 11, 7, tzinfo=datetime.timezone.utc)),
             'Vehicle.Chassis.SteeringWheel.Tilt': Datapoint(42),
         }
 
     async def test_subscribe_metadata(self, mocker, unused_tcp_port):
         client = VSSClient('127.0.0.1', unused_tcp_port)
+
         async def subscribe_response_stream(**kwargs):
             yield [
                 EntryUpdate(DataEntry(
                     'Vehicle.Speed', metadata=Metadata(entry_type=EntryType.SENSOR),
                 ), (Field.METADATA_ENTRY_TYPE,)),
                 EntryUpdate(DataEntry(
                     'Vehicle.ADAS.ABS.IsActive', metadata=Metadata(entry_type=EntryType.ACTUATOR),
                 ), (Field.METADATA_ENTRY_TYPE,)),
                 EntryUpdate(DataEntry(
                     'Vehicle.Chassis.Height', metadata=Metadata(entry_type=EntryType.ATTRIBUTE),
                 ), (Field.METADATA_ENTRY_TYPE,)),
             ]
-        mocker.patch.object(client, 'subscribe', side_effect=subscribe_response_stream)
+        mocker.patch.object(client, 'subscribe',
+                            side_effect=subscribe_response_stream)
 
         received_updates = {}
         async for updates in client.subscribe_metadata([
             'Vehicle.Speed', 'Vehicle.ADAS.ABS.IsActive', 'Vehicle.Chassis.Height',
         ], field=MetadataField.ENTRY_TYPE):
             received_updates.update(updates)
 
         assert list(client.subscribe.call_args_list[0][1]['entries']) == [
-            SubscribeEntry('Vehicle.Speed', View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
-            SubscribeEntry('Vehicle.ADAS.ABS.IsActive', View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
-            SubscribeEntry('Vehicle.Chassis.Height', View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
+            SubscribeEntry('Vehicle.Speed', View.METADATA,
+                           (Field.METADATA_ENTRY_TYPE,)),
+            SubscribeEntry('Vehicle.ADAS.ABS.IsActive',
+                           View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
+            SubscribeEntry('Vehicle.Chassis.Height',
+                           View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
         ]
         assert received_updates == {
             'Vehicle.Speed': Metadata(entry_type=EntryType.SENSOR),
             'Vehicle.ADAS.ABS.IsActive': Metadata(entry_type=EntryType.ACTUATOR),
             'Vehicle.Chassis.Height': Metadata(entry_type=EntryType.ATTRIBUTE),
         }
 
     @pytest.mark.usefixtures('val_server')
     async def test_get_some_entries(self, unused_tcp_port, val_servicer):
         val_servicer.Get.return_value = val_pb2.GetResponse(entries=[
             types_pb2.DataEntry(
                 path='Vehicle.Speed',
                 value=types_pb2.Datapoint(
-                    timestamp=timestamp_pb2.Timestamp(seconds=1667837915, nanos=247307674),
+                    timestamp=timestamp_pb2.Timestamp(
+                        seconds=1667837915, nanos=247307674),
                     float=42.0,
                 ),
             ),
-            types_pb2.DataEntry(path='Vehicle.ADAS.ABS.IsActive', actuator_target=types_pb2.Datapoint(bool=True)),
+            types_pb2.DataEntry(path='Vehicle.ADAS.ABS.IsActive',
+                                actuator_target=types_pb2.Datapoint(bool=True)),
             types_pb2.DataEntry(
                 path='Vehicle.Chassis.Height',
                 metadata=types_pb2.Metadata(
                     data_type=types_pb2.DATA_TYPE_UINT16,
                     entry_type=types_pb2.ENTRY_TYPE_ATTRIBUTE,
                     description="Overall vehicle height, in mm.",
                     comment="No comment.",
@@ -556,135 +621,160 @@
                 path='Vehicle.Chassis.Height', metadata=types_pb2.Metadata(data_type=types_pb2.DATA_TYPE_UINT16),
             ),
             types_pb2.DataEntry(
                 path='Vehicle.Chassis.Height', metadata=types_pb2.Metadata(entry_type=types_pb2.ENTRY_TYPE_ATTRIBUTE),
             ),
             types_pb2.DataEntry(
                 path='Vehicle.Chassis.Height',
-                metadata=types_pb2.Metadata(description="Overall vehicle height, in mm."),
+                metadata=types_pb2.Metadata(
+                    description="Overall vehicle height, in mm."),
             ),
             types_pb2.DataEntry(
                 path='Vehicle.Chassis.Height', metadata=types_pb2.Metadata(comment="No comment."),
             ),
             types_pb2.DataEntry(
                 path='Vehicle.Chassis.Height', metadata=types_pb2.Metadata(deprecation="V2.1 moved to Vehicle.Height"),
             ),
-            types_pb2.DataEntry(path='Vehicle.Chassis.Height', metadata=types_pb2.Metadata(unit="mm")),
+            types_pb2.DataEntry(path='Vehicle.Chassis.Height',
+                                metadata=types_pb2.Metadata(unit="mm")),
             types_pb2.DataEntry(
                 path='Vehicle.CurrentLocation.Heading',
                 metadata=types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
-                    floating_point=types_pb2.ValueRestrictionFloat(min=0, max=360),
+                    floating_point=types_pb2.ValueRestrictionFloat(
+                        min=0, max=360),
                 )),
             ),
             types_pb2.DataEntry(
                 path='Dummy.With.Allowed.Values',
                 metadata=types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
-                    signed=types_pb2.ValueRestrictionInt(allowed_values=[12, 42, 666]),
+                    signed=types_pb2.ValueRestrictionInt(
+                        allowed_values=[12, 42, 666]),
                 )),
             ),
         ])
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             entries = await client.get(entries=(entry for entry in (  # generator is intentional as get accepts Iterable
-                EntryRequest('Vehicle.Speed', View.CURRENT_VALUE, (Field.VALUE,)),
-                EntryRequest('Vehicle.ADAS.ABS.IsActive', View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
-                EntryRequest('Vehicle.Chassis.Height', View.METADATA, (Field.METADATA,)),
-                EntryRequest('Vehicle.Chassis.Height', View.METADATA, (Field.METADATA_DATA_TYPE,)),
-                EntryRequest('Vehicle.Chassis.Height', View.METADATA, (Field.METADATA_DESCRIPTION,)),
-                EntryRequest('Vehicle.Chassis.Height', View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
-                EntryRequest('Vehicle.Chassis.Height', View.METADATA, (Field.METADATA_COMMENT,)),
-                EntryRequest('Vehicle.Chassis.Height', View.METADATA, (Field.METADATA_DEPRECATION,)),
-                EntryRequest('Vehicle.Chassis.Height', View.METADATA, (Field.METADATA_UNIT,)),
-                EntryRequest('Vehicle.CurrentLocation.Heading', View.METADATA, (Field.METADATA_VALUE_RESTRICTION,)),
-                EntryRequest('Dummy.With.Allowed.Values', View.METADATA, (Field.METADATA_VALUE_RESTRICTION,)),
+                EntryRequest('Vehicle.Speed',
+                             View.CURRENT_VALUE, (Field.VALUE,)),
+                EntryRequest('Vehicle.ADAS.ABS.IsActive',
+                             View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
+                EntryRequest('Vehicle.Chassis.Height',
+                             View.METADATA, (Field.METADATA,)),
+                EntryRequest('Vehicle.Chassis.Height',
+                             View.METADATA, (Field.METADATA_DATA_TYPE,)),
+                EntryRequest('Vehicle.Chassis.Height',
+                             View.METADATA, (Field.METADATA_DESCRIPTION,)),
+                EntryRequest('Vehicle.Chassis.Height',
+                             View.METADATA, (Field.METADATA_ENTRY_TYPE,)),
+                EntryRequest('Vehicle.Chassis.Height',
+                             View.METADATA, (Field.METADATA_COMMENT,)),
+                EntryRequest('Vehicle.Chassis.Height',
+                             View.METADATA, (Field.METADATA_DEPRECATION,)),
+                EntryRequest('Vehicle.Chassis.Height',
+                             View.METADATA, (Field.METADATA_UNIT,)),
+                EntryRequest('Vehicle.CurrentLocation.Heading',
+                             View.METADATA, (Field.METADATA_VALUE_RESTRICTION,)),
+                EntryRequest('Dummy.With.Allowed.Values', View.METADATA,
+                             (Field.METADATA_VALUE_RESTRICTION,)),
             )))
             assert entries == [
                 DataEntry('Vehicle.Speed', value=Datapoint(
-                    42.0, datetime.datetime(2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
+                    42.0, datetime.datetime(
+                        2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
                 )),
-                DataEntry('Vehicle.ADAS.ABS.IsActive', actuator_target=Datapoint(True)),
+                DataEntry('Vehicle.ADAS.ABS.IsActive',
+                          actuator_target=Datapoint(True)),
                 DataEntry('Vehicle.Chassis.Height', metadata=Metadata(
                     data_type=DataType.UINT16,
                     entry_type=EntryType.ATTRIBUTE,
                     description="Overall vehicle height, in mm.",
                     comment="No comment.",
                     deprecation="V2.1 moved to Vehicle.Height",
                     unit="mm",
                 )),
-                DataEntry('Vehicle.Chassis.Height', metadata=Metadata(data_type=DataType.UINT16)),
-                DataEntry('Vehicle.Chassis.Height', metadata=Metadata(entry_type=EntryType.ATTRIBUTE)),
-                DataEntry('Vehicle.Chassis.Height', metadata=Metadata(description="Overall vehicle height, in mm.")),
-                DataEntry('Vehicle.Chassis.Height', metadata=Metadata(comment="No comment.")),
-                DataEntry('Vehicle.Chassis.Height', metadata=Metadata(deprecation="V2.1 moved to Vehicle.Height")),
-                DataEntry('Vehicle.Chassis.Height', metadata=Metadata(unit="mm")),
+                DataEntry('Vehicle.Chassis.Height',
+                          metadata=Metadata(data_type=DataType.UINT16)),
+                DataEntry('Vehicle.Chassis.Height', metadata=Metadata(
+                    entry_type=EntryType.ATTRIBUTE)),
+                DataEntry('Vehicle.Chassis.Height', metadata=Metadata(
+                    description="Overall vehicle height, in mm.")),
+                DataEntry('Vehicle.Chassis.Height',
+                          metadata=Metadata(comment="No comment.")),
+                DataEntry('Vehicle.Chassis.Height', metadata=Metadata(
+                    deprecation="V2.1 moved to Vehicle.Height")),
+                DataEntry('Vehicle.Chassis.Height',
+                          metadata=Metadata(unit="mm")),
                 DataEntry('Vehicle.CurrentLocation.Heading', metadata=Metadata(
                     value_restriction=ValueRestriction(min=0, max=360),
                 )),
                 DataEntry('Dummy.With.Allowed.Values', metadata=Metadata(
-                    value_restriction=ValueRestriction(allowed_values=[12, 42, 666]),
+                    value_restriction=ValueRestriction(
+                        allowed_values=[12, 42, 666]),
                 )),
             ]
             assert val_servicer.Get.call_args[0][0].entries == val_pb2.GetRequest(entries=(
                 val_pb2.EntryRequest(
                     path='Vehicle.Speed', view=types_pb2.VIEW_CURRENT_VALUE, fields=(types_pb2.FIELD_VALUE,),
                 ),
                 val_pb2.EntryRequest(
-                  path='Vehicle.ADAS.ABS.IsActive',
-                  view=types_pb2.VIEW_TARGET_VALUE,
-                  fields=(types_pb2.FIELD_ACTUATOR_TARGET,),
+                    path='Vehicle.ADAS.ABS.IsActive',
+                    view=types_pb2.VIEW_TARGET_VALUE,
+                    fields=(types_pb2.FIELD_ACTUATOR_TARGET,),
                 ),
                 val_pb2.EntryRequest(
-                  path='Vehicle.Chassis.Height',
-                  view=types_pb2.VIEW_METADATA,
-                  fields=(types_pb2.FIELD_METADATA,),
+                    path='Vehicle.Chassis.Height',
+                    view=types_pb2.VIEW_METADATA,
+                    fields=(types_pb2.FIELD_METADATA,),
                 ),
                 val_pb2.EntryRequest(
-                  path='Vehicle.Chassis.Height',
-                  view=types_pb2.VIEW_METADATA,
-                  fields=(types_pb2.FIELD_METADATA_DATA_TYPE,),
+                    path='Vehicle.Chassis.Height',
+                    view=types_pb2.VIEW_METADATA,
+                    fields=(types_pb2.FIELD_METADATA_DATA_TYPE,),
                 ),
                 val_pb2.EntryRequest(
-                  path='Vehicle.Chassis.Height',
-                  view=types_pb2.VIEW_METADATA,
-                  fields=(types_pb2.FIELD_METADATA_DESCRIPTION,),
+                    path='Vehicle.Chassis.Height',
+                    view=types_pb2.VIEW_METADATA,
+                    fields=(types_pb2.FIELD_METADATA_DESCRIPTION,),
                 ),
                 val_pb2.EntryRequest(
-                  path='Vehicle.Chassis.Height',
-                  view=types_pb2.VIEW_METADATA,
-                  fields=(types_pb2.FIELD_METADATA_ENTRY_TYPE,),
+                    path='Vehicle.Chassis.Height',
+                    view=types_pb2.VIEW_METADATA,
+                    fields=(types_pb2.FIELD_METADATA_ENTRY_TYPE,),
                 ),
                 val_pb2.EntryRequest(
-                  path='Vehicle.Chassis.Height',
-                  view=types_pb2.VIEW_METADATA,
-                  fields=(types_pb2.FIELD_METADATA_COMMENT,),
+                    path='Vehicle.Chassis.Height',
+                    view=types_pb2.VIEW_METADATA,
+                    fields=(types_pb2.FIELD_METADATA_COMMENT,),
                 ),
                 val_pb2.EntryRequest(
-                  path='Vehicle.Chassis.Height',
-                  view=types_pb2.VIEW_METADATA,
-                  fields=(types_pb2.FIELD_METADATA_DEPRECATION,),
+                    path='Vehicle.Chassis.Height',
+                    view=types_pb2.VIEW_METADATA,
+                    fields=(types_pb2.FIELD_METADATA_DEPRECATION,),
                 ),
                 val_pb2.EntryRequest(
-                  path='Vehicle.Chassis.Height',
-                  view=types_pb2.VIEW_METADATA,
-                  fields=(types_pb2.FIELD_METADATA_UNIT,),
+                    path='Vehicle.Chassis.Height',
+                    view=types_pb2.VIEW_METADATA,
+                    fields=(types_pb2.FIELD_METADATA_UNIT,),
                 ),
                 val_pb2.EntryRequest(
-                  path='Vehicle.CurrentLocation.Heading',
-                  view=types_pb2.VIEW_METADATA,
-                  fields=(types_pb2.FIELD_METADATA_VALUE_RESTRICTION,),
+                    path='Vehicle.CurrentLocation.Heading',
+                    view=types_pb2.VIEW_METADATA,
+                    fields=(types_pb2.FIELD_METADATA_VALUE_RESTRICTION,),
                 ),
                 val_pb2.EntryRequest(
-                  path='Dummy.With.Allowed.Values',
-                  view=types_pb2.VIEW_METADATA,
-                  fields=(types_pb2.FIELD_METADATA_VALUE_RESTRICTION,),
+                    path='Dummy.With.Allowed.Values',
+                    view=types_pb2.VIEW_METADATA,
+                    fields=(types_pb2.FIELD_METADATA_VALUE_RESTRICTION,),
                 ),
             )).entries
 
     @pytest.mark.usefixtures('val_server')
     async def test_get_no_entries_requested(self, unused_tcp_port, val_servicer):
-        val_servicer.Get.side_effect = generate_error(grpc.StatusCode.INVALID_ARGUMENT, 'No datapoints requested')
+        val_servicer.Get.side_effect = generate_error(
+            grpc.StatusCode.INVALID_ARGUMENT, 'No datapoints requested')
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             with pytest.raises(kuksa_client.grpc.VSSClientError) as exc_info:
                 await client.get(entries=[])
 
             assert exc_info.value.args == kuksa_client.grpc.VSSClientError(error={
                 'code': grpc.StatusCode.INVALID_ARGUMENT.value[0],
                 'reason': grpc.StatusCode.INVALID_ARGUMENT.value[1],
@@ -696,50 +786,60 @@
     async def test_get_unset_entries(self, unused_tcp_port, val_servicer):
         val_servicer.Get.return_value = val_pb2.GetResponse(entries=[
             types_pb2.DataEntry(path='Vehicle.Speed'),
             types_pb2.DataEntry(path='Vehicle.ADAS.ABS.IsActive'),
         ])
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             entries = await client.get(entries=(
-                EntryRequest('Vehicle.Speed', View.CURRENT_VALUE, (Field.VALUE,)),
-                EntryRequest('Vehicle.ADAS.ABS.IsActive', View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
+                EntryRequest('Vehicle.Speed',
+                             View.CURRENT_VALUE, (Field.VALUE,)),
+                EntryRequest('Vehicle.ADAS.ABS.IsActive',
+                             View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
             ))
 
-        assert entries == [DataEntry('Vehicle.Speed'), DataEntry('Vehicle.ADAS.ABS.IsActive')]
+        assert entries == [DataEntry('Vehicle.Speed'), DataEntry(
+            'Vehicle.ADAS.ABS.IsActive')]
 
     @pytest.mark.usefixtures('val_server')
     async def test_get_nonexistent_entries(self, unused_tcp_port, val_servicer):
-        error = types_pb2.Error(code=404, reason='not_found', message="Does.Not.Exist not found")
-        errors = (types_pb2.DataEntryError(path='Does.Not.Exist', error=error),)
-        val_servicer.Get.return_value = val_pb2.GetResponse(error=error, errors=errors)
+        error = types_pb2.Error(
+            code=404, reason='not_found', message="Does.Not.Exist not found")
+        errors = (types_pb2.DataEntryError(
+            path='Does.Not.Exist', error=error),)
+        val_servicer.Get.return_value = val_pb2.GetResponse(
+            error=error, errors=errors)
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             with pytest.raises(VSSClientError):
                 await client.get(entries=(
-                    EntryRequest('Does.Not.Exist', View.CURRENT_VALUE, (Field.VALUE,)),
+                    EntryRequest('Does.Not.Exist',
+                                 View.CURRENT_VALUE, (Field.VALUE,)),
                 ))
 
     @pytest.mark.usefixtures('val_server')
     async def test_set_some_updates(self, unused_tcp_port, val_servicer):
         val_servicer.Get.return_value = val_pb2.GetResponse(entries=(
             types_pb2.DataEntry(
                 path='Vehicle.Speed', metadata=types_pb2.Metadata(data_type=types_pb2.DATA_TYPE_FLOAT),
             ),
             types_pb2.DataEntry(
                 path='Vehicle.ADAS.ABS.IsActive',
-                metadata=types_pb2.Metadata(data_type=types_pb2.DATA_TYPE_BOOLEAN),
+                metadata=types_pb2.Metadata(
+                    data_type=types_pb2.DATA_TYPE_BOOLEAN),
             ),
             types_pb2.DataEntry(
                 path='Vehicle.Cabin.Door.Row1.Left.Shade.Position',
-                metadata=types_pb2.Metadata(data_type=types_pb2.DATA_TYPE_UINT8),
+                metadata=types_pb2.Metadata(
+                    data_type=types_pb2.DATA_TYPE_UINT8),
             ),
         ))
         val_servicer.Set.return_value = val_pb2.SetResponse()
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             await client.set(updates=[
-                EntryUpdate(DataEntry('Vehicle.Speed', value=Datapoint(value=42.0)), (Field.VALUE,)),
+                EntryUpdate(DataEntry('Vehicle.Speed',
+                            value=Datapoint(value=42.0)), (Field.VALUE,)),
                 EntryUpdate(DataEntry(
                     'Vehicle.ADAS.ABS.IsActive', actuator_target=Datapoint(value=False),
                 ), (Field.ACTUATOR_TARGET,)),
                 EntryUpdate(DataEntry('Vehicle.ADAS.CruiseControl.Error', metadata=Metadata(
                     data_type=DataType.BOOLEAN,
                     entry_type=EntryType.SENSOR,
                     description="Indicates if cruise control system incurred and error condition.",
@@ -768,15 +868,16 @@
                 )), (Field.METADATA_UNIT,)),
                 EntryUpdate(DataEntry('Vehicle.Cabin.Door.Row1.Left.Shade.Position', metadata=Metadata(
                     value_restriction=ValueRestriction(min=0, max=100),
                 )), (Field.METADATA_VALUE_RESTRICTION,)),
             ])
             assert val_servicer.Get.call_count == 1
             assert val_servicer.Get.call_args[0][0].entries == val_pb2.GetRequest(entries=(
-                val_pb2.EntryRequest(path='Vehicle.Speed', view=View.METADATA, fields=(Field.METADATA_DATA_TYPE,)),
+                val_pb2.EntryRequest(path='Vehicle.Speed', view=View.METADATA, fields=(
+                    Field.METADATA_DATA_TYPE,)),
                 val_pb2.EntryRequest(
                     path='Vehicle.ADAS.ABS.IsActive', view=View.METADATA, fields=(Field.METADATA_DATA_TYPE,),
                 ),
                 val_pb2.EntryRequest(
                     path='Vehicle.Cabin.Door.Row1.Left.Shade.Position',
                     view=View.METADATA,
                     fields=(Field.METADATA_DATA_TYPE,),
@@ -797,67 +898,77 @@
                         description="Indicates if cruise control system incurred and error condition.",
                         comment="No comment",
                         deprecation="Never to be deprecated",
                     ),
                 ), fields=(types_pb2.FIELD_METADATA,)),
                 val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                     path='Vehicle.ADAS.CruiseControl.Error',
-                    metadata=types_pb2.Metadata(data_type=types_pb2.DATA_TYPE_BOOLEAN),
+                    metadata=types_pb2.Metadata(
+                        data_type=types_pb2.DATA_TYPE_BOOLEAN),
                 ), fields=(types_pb2.FIELD_METADATA_DATA_TYPE,)),
                 val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                     path='Vehicle.ADAS.CruiseControl.Error',
                     metadata=types_pb2.Metadata(
                         description="Indicates if cruise control system incurred and error condition."
                     ),
                 ), fields=(types_pb2.FIELD_METADATA_DESCRIPTION,)),
                 val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                     path='Vehicle.ADAS.CruiseControl.Error',
-                    metadata=types_pb2.Metadata(entry_type=types_pb2.ENTRY_TYPE_SENSOR),
+                    metadata=types_pb2.Metadata(
+                        entry_type=types_pb2.ENTRY_TYPE_SENSOR),
                 ), fields=(types_pb2.FIELD_METADATA_ENTRY_TYPE,)),
                 val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                     path='Vehicle.ADAS.CruiseControl.Error',
                     metadata=types_pb2.Metadata(comment="No comment"),
                 ), fields=(types_pb2.FIELD_METADATA_COMMENT,)),
                 val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                     path='Vehicle.ADAS.CruiseControl.Error',
-                    metadata=types_pb2.Metadata(deprecation="Never to be deprecated"),
+                    metadata=types_pb2.Metadata(
+                        deprecation="Never to be deprecated"),
                 ), fields=(types_pb2.FIELD_METADATA_DEPRECATION,)),
                 val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                     path='Vehicle.Cabin.Door.Row1.Left.Shade.Position',
                     metadata=types_pb2.Metadata(unit="percent"),
                 ), fields=(types_pb2.FIELD_METADATA_UNIT,)),
                 val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                     path='Vehicle.Cabin.Door.Row1.Left.Shade.Position',
                     metadata=types_pb2.Metadata(value_restriction=types_pb2.ValueRestriction(
-                        unsigned=types_pb2.ValueRestrictionUint(min=0, max=100),
+                        unsigned=types_pb2.ValueRestrictionUint(
+                            min=0, max=100),
                     )),
                 ), fields=(types_pb2.FIELD_METADATA_VALUE_RESTRICTION,)),
             )).updates
 
     @pytest.mark.usefixtures('val_server')
     async def test_set_no_updates_provided(self, unused_tcp_port, val_servicer):
-        val_servicer.Set.side_effect = generate_error(grpc.StatusCode.INVALID_ARGUMENT, 'No datapoints requested')
+        val_servicer.Set.side_effect = generate_error(
+            grpc.StatusCode.INVALID_ARGUMENT, 'No datapoints requested')
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             with pytest.raises(kuksa_client.grpc.VSSClientError) as exc_info:
                 await client.set(updates=[])
 
             assert exc_info.value.args == kuksa_client.grpc.VSSClientError(error={
                 'code': grpc.StatusCode.INVALID_ARGUMENT.value[0],
                 'reason': grpc.StatusCode.INVALID_ARGUMENT.value[1],
                 'message': 'No datapoints requested',
             }, errors=[]).args
             assert val_servicer.Get.call_count == 0
-            assert val_servicer.Set.call_args[0][0].updates == val_pb2.SetRequest().updates
+            assert val_servicer.Set.call_args[0][0].updates == val_pb2.SetRequest(
+            ).updates
 
     @pytest.mark.usefixtures('val_server')
     async def test_set_nonexistent_entries(self, unused_tcp_port, val_servicer):
-        error = types_pb2.Error(code=404, reason='not_found', message="Does.Not.Exist not found")
-        errors = (types_pb2.DataEntryError(path='Does.Not.Exist', error=error),)
-        val_servicer.Get.return_value = val_pb2.GetResponse(error=error, errors=errors)
-        val_servicer.Set.return_value = val_pb2.SetResponse(error=error, errors=errors)
+        error = types_pb2.Error(
+            code=404, reason='not_found', message="Does.Not.Exist not found")
+        errors = (types_pb2.DataEntryError(
+            path='Does.Not.Exist', error=error),)
+        val_servicer.Get.return_value = val_pb2.GetResponse(
+            error=error, errors=errors)
+        val_servicer.Set.return_value = val_pb2.SetResponse(
+            error=error, errors=errors)
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             with pytest.raises(VSSClientError):
                 await client.set(updates=(
                     EntryUpdate(DataEntry('Does.Not.Exist', value=Datapoint(value=42.0)), (Field.VALUE,)),),
                 )
 
             assert val_servicer.Get.call_count == 1
@@ -871,28 +982,43 @@
                     ), (Field.VALUE,)),),
                 )
 
             assert val_servicer.Get.call_count == 1  # Get should'nt have been called again
             assert val_servicer.Set.call_count == 1
 
     @pytest.mark.usefixtures('val_server')
-    async def test_authorize_not_implemented(self):
-        with pytest.raises(NotImplementedError):
-            await VSSClient('127.0.0.1', 424242).authorize(token='')
+    async def test_authorize_successful(self, unused_tcp_port, val_servicer):
+        val_servicer.GetServerInfo.return_value = val_pb2.GetServerInfoResponse(
+            name='test_server', version='1.2.3')
+        async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
+            # token from kuksa.val directory under jwt/provide-vehicle-speed.token
+            success = await client.authorize(token='eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJsb2NhbCBkZXYiLCJpc3MiOiJjcmVhdGVUb2tlbi5weSIsImF1ZCI6WyJrdWtzYS52YWwiXSwiaWF0IjoxNTE2MjM5MDIyLCJleHAiOjE3NjcyMjU1OTksInNjb3BlIjoicmVhZDpWZWhpY2xlLldpZHRoIHByb3ZpZGU6VmVoaWNsZS5TcGVlZCJ9.w2c8xrYwBVgMav3f0Se6E8H8E36Nd03rJiSS2A8s-CL3GtlwB7wVanjXHhppNsCdWym3tK4JwgslQdMQF-UL4hd7vzdtt-Mx6VjH_jO9mDxz4Z0Uzw7aJtbtQSpi2h6kwceTVTllkbLRF7WRHWIpwzXFF9yZolX6lH-BE9xf1AB62d6icd9SKxFnVvYs3MVK5D1xNmDNOmm-Fr0d2K604MmIIXGW5kPZJYIvBKO4NYRLklhJe47It_lGo3gnh1ppmzTOIo1kB4sDe55hplUCbTCJVricpyQSgTYsf7aFRPK51XMRwwwJ8kShWeaTggMLKpv1W-9dhVWDk4isC8BxsOjaVloArausMmjLmTz6KwAsfARgfXtaCrMsESUBNXi5KIdAyHVXZpmERvc9yeYPcaWlknVFrFsHbV6bw4nwqBX-0Ubuga0NGNQDFKmyTKQrbuZmQ3L9iipxY8_BOSCkdiYtWbE3lpplxpS_PaZl10KAaMmUfbcF9aYZunDEzEtoJgJe2EeGu3XDBtbyXVUKruImdSEdjaImfUGQIWl5bMbVH4N4zK5jE45wT5FJiRUcA5pMN5wNmDYJJzgbxWNpYW40KZYPFc_7XUH8EZ2Cs69wDHam3ArkOs1qMgMIoEPWVzHakjlVJfrPR9zQKxfirBtNNENIoHsBjJ_P4FEJCN4')
+            assert client.authorization_header == 'Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiJ9.eyJzdWIiOiJsb2NhbCBkZXYiLCJpc3MiOiJjcmVhdGVUb2tlbi5weSIsImF1ZCI6WyJrdWtzYS52YWwiXSwiaWF0IjoxNTE2MjM5MDIyLCJleHAiOjE3NjcyMjU1OTksInNjb3BlIjoicmVhZDpWZWhpY2xlLldpZHRoIHByb3ZpZGU6VmVoaWNsZS5TcGVlZCJ9.w2c8xrYwBVgMav3f0Se6E8H8E36Nd03rJiSS2A8s-CL3GtlwB7wVanjXHhppNsCdWym3tK4JwgslQdMQF-UL4hd7vzdtt-Mx6VjH_jO9mDxz4Z0Uzw7aJtbtQSpi2h6kwceTVTllkbLRF7WRHWIpwzXFF9yZolX6lH-BE9xf1AB62d6icd9SKxFnVvYs3MVK5D1xNmDNOmm-Fr0d2K604MmIIXGW5kPZJYIvBKO4NYRLklhJe47It_lGo3gnh1ppmzTOIo1kB4sDe55hplUCbTCJVricpyQSgTYsf7aFRPK51XMRwwwJ8kShWeaTggMLKpv1W-9dhVWDk4isC8BxsOjaVloArausMmjLmTz6KwAsfARgfXtaCrMsESUBNXi5KIdAyHVXZpmERvc9yeYPcaWlknVFrFsHbV6bw4nwqBX-0Ubuga0NGNQDFKmyTKQrbuZmQ3L9iipxY8_BOSCkdiYtWbE3lpplxpS_PaZl10KAaMmUfbcF9aYZunDEzEtoJgJe2EeGu3XDBtbyXVUKruImdSEdjaImfUGQIWl5bMbVH4N4zK5jE45wT5FJiRUcA5pMN5wNmDYJJzgbxWNpYW40KZYPFc_7XUH8EZ2Cs69wDHam3ArkOs1qMgMIoEPWVzHakjlVJfrPR9zQKxfirBtNNENIoHsBjJ_P4FEJCN4'
+            assert success == "Authenticated"
+
+    @pytest.mark.usefixtures('val_server')
+    async def test_authorize_unsuccessful(self, unused_tcp_port, val_servicer):
+        val_servicer.GetServerInfo.side_effect = generate_error(
+            grpc.StatusCode.UNAUTHENTICATED, 'Invalid auth token: DecodeError(\"InvalidToken\")')
+        async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
+            with pytest.raises(VSSClientError):
+                await client.authorize(token='')
+            assert client.authorization_header == None
 
     @pytest.mark.usefixtures('val_server')
     async def test_subscribe_some_entries(self, mocker, unused_tcp_port, val_servicer):
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             responses = (
                 # 1st response is subscription ack
                 val_pb2.SubscribeResponse(updates=[
                     val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                         path='Vehicle.Speed',
                         value=types_pb2.Datapoint(
-                            timestamp=timestamp_pb2.Timestamp(seconds=1667837915, nanos=247307674),
+                            timestamp=timestamp_pb2.Timestamp(
+                                seconds=1667837915, nanos=247307674),
                             float=42.0,
                         ),
                     ), fields=(Field.VALUE,)),
                     val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                         path='Vehicle.ADAS.ABS.IsActive',
                         actuator_target=types_pb2.Datapoint(bool=True),
                     ), fields=(Field.ACTUATOR_TARGET,)),
@@ -904,15 +1030,16 @@
                     ), fields=(Field.METADATA_DATA_TYPE,)),
                 ]),
                 # Remaining responses are actual events.
                 val_pb2.SubscribeResponse(updates=[
                     val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                         path='Vehicle.Speed',
                         value=types_pb2.Datapoint(
-                            timestamp=timestamp_pb2.Timestamp(seconds=1667837912, nanos=247307674),
+                            timestamp=timestamp_pb2.Timestamp(
+                                seconds=1667837912, nanos=247307674),
                             float=43.0,
                         ),
                     ), fields=(Field.VALUE,)),
                 ]),
                 val_pb2.SubscribeResponse(updates=[
                     val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                         path='Vehicle.ADAS.ABS.IsActive',
@@ -924,41 +1051,48 @@
                         path='Vehicle.Chassis.Height',
                         metadata=types_pb2.Metadata(
                             data_type=types_pb2.DATA_TYPE_UINT8,
                         ),
                     ), fields=(Field.METADATA_DATA_TYPE,)),
                 ]),
             )
-            val_servicer.Subscribe.return_value = (response for response in responses)
+            val_servicer.Subscribe.return_value = (
+                response for response in responses)
 
             actual_responses = []
             async for updates in client.subscribe(entries=(entry for entry in (  # generator is intentional (Iterable)
-                EntryRequest('Vehicle.Speed', View.CURRENT_VALUE, (Field.VALUE,)),
-                EntryRequest('Vehicle.ADAS.ABS.IsActive', View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
-                EntryRequest('Vehicle.Chassis.Height', View.METADATA, (Field.METADATA_DATA_TYPE,)),
+                EntryRequest('Vehicle.Speed',
+                             View.CURRENT_VALUE, (Field.VALUE,)),
+                EntryRequest('Vehicle.ADAS.ABS.IsActive',
+                             View.TARGET_VALUE, (Field.ACTUATOR_TARGET,)),
+                EntryRequest('Vehicle.Chassis.Height',
+                             View.METADATA, (Field.METADATA_DATA_TYPE,)),
             ))):
                 actual_responses.append(updates)
 
             assert actual_responses == [
                 [
                     EntryUpdate(entry=DataEntry(path='Vehicle.Speed', value=Datapoint(
                         value=42.0,
-                        timestamp=datetime.datetime(2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
+                        timestamp=datetime.datetime(
+                            2022, 11, 7, 16, 18, 35, 247307, tzinfo=datetime.timezone.utc),
                     )), fields=[Field.VALUE]),
                     EntryUpdate(
-                        entry=DataEntry(path='Vehicle.ADAS.ABS.IsActive', actuator_target=Datapoint(value=True)),
+                        entry=DataEntry(
+                            path='Vehicle.ADAS.ABS.IsActive', actuator_target=Datapoint(value=True)),
                         fields=[Field.ACTUATOR_TARGET],
                     ),
                     EntryUpdate(entry=DataEntry(path='Vehicle.Chassis.Height', metadata=Metadata(
                         data_type=DataType.UINT16,
                     )), fields=[Field.METADATA_DATA_TYPE])
                 ],
                 [EntryUpdate(entry=DataEntry(path='Vehicle.Speed', value=Datapoint(
                     value=43.0,
-                    timestamp=datetime.datetime(2022, 11, 7, 16, 18, 32, 247307, tzinfo=datetime.timezone.utc),
+                    timestamp=datetime.datetime(
+                        2022, 11, 7, 16, 18, 32, 247307, tzinfo=datetime.timezone.utc),
                 )), fields=[Field.VALUE])],
                 [EntryUpdate(entry=DataEntry(path='Vehicle.ADAS.ABS.IsActive', actuator_target=Datapoint(
                     value=False,
                 )), fields=[Field.ACTUATOR_TARGET])],
                 [EntryUpdate(entry=DataEntry(path='Vehicle.Chassis.Height', metadata=Metadata(
                     data_type=DataType.UINT8,
                 )), fields=[Field.METADATA_DATA_TYPE])],
@@ -972,32 +1106,37 @@
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             with pytest.raises(VSSClientError):
                 async for _ in client.subscribe(entries=()):
                     pass
 
     @pytest.mark.usefixtures('val_server')
     async def test_subscribe_nonexistent_entries(self, mocker, unused_tcp_port, val_servicer):
-        val_servicer.Subscribe.side_effect = generate_error(grpc.StatusCode.INVALID_ARGUMENT, 'NotFound')
+        val_servicer.Subscribe.side_effect = generate_error(
+            grpc.StatusCode.INVALID_ARGUMENT, 'NotFound')
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             with pytest.raises(VSSClientError):
                 async for _ in client.subscribe(entries=(entry for entry in (  # generator is intentional (Iterable)
-                    EntryRequest('Does.Not.Exist', View.CURRENT_VALUE, (Field.VALUE,)),
+                    EntryRequest('Does.Not.Exist',
+                                 View.CURRENT_VALUE, (Field.VALUE,)),
                 ))):
                     pass
 
     @pytest.mark.usefixtures('val_server')
     async def test_get_server_info(self, unused_tcp_port, val_servicer):
-        val_servicer.GetServerInfo.return_value = val_pb2.GetServerInfoResponse(name='test_server', version='1.2.3')
+        val_servicer.GetServerInfo.return_value = val_pb2.GetServerInfoResponse(
+            name='test_server', version='1.2.3')
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             server_info = await client.get_server_info()
-            assert server_info == ServerInfo(name='test_server', version='1.2.3')
+            assert server_info == ServerInfo(
+                name='test_server', version='1.2.3')
 
     @pytest.mark.usefixtures('val_server')
     async def test_get_server_info_unavailable(self, unused_tcp_port, val_servicer):
-        val_servicer.GetServerInfo.side_effect = generate_error(grpc.StatusCode.UNAVAILABLE, 'Unavailable')
+        val_servicer.GetServerInfo.side_effect = generate_error(
+            grpc.StatusCode.UNAVAILABLE, 'Unavailable')
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             with pytest.raises(VSSClientError):
                 await client.get_server_info()
 
 
 @pytest.mark.asyncio
 class TestSubscriberManager:
@@ -1007,67 +1146,76 @@
             subscriber_manager = SubscriberManager(client)
             responses = (
                 # 1st response is subscription ack
                 val_pb2.SubscribeResponse(updates=[
                     val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                         path='Vehicle.Speed',
                         value=types_pb2.Datapoint(
-                            timestamp=timestamp_pb2.Timestamp(seconds=1667837915, nanos=247307674),
+                            timestamp=timestamp_pb2.Timestamp(
+                                seconds=1667837915, nanos=247307674),
                             float=42.0,
                         ),
                     ), fields=(Field.VALUE,)),
                 ]),
                 # Remaining responses are actual events that should invoke callback.
                 val_pb2.SubscribeResponse(updates=[
                     val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                         path='Vehicle.Speed',
                         value=types_pb2.Datapoint(
-                            timestamp=timestamp_pb2.Timestamp(seconds=1667837912, nanos=247307674),
+                            timestamp=timestamp_pb2.Timestamp(
+                                seconds=1667837912, nanos=247307674),
                             float=43.0,
                         ),
                     ), fields=(Field.VALUE,)),
                 ]),
             )
             callback = mocker.Mock()
-            val_servicer.Subscribe.return_value = (response for response in responses)
+            val_servicer.Subscribe.return_value = (
+                response for response in responses)
 
             subscribe_response_stream = client.subscribe(entries=(
-                EntryRequest('Vehicle.Speed', View.CURRENT_VALUE, (Field.VALUE,)),
+                EntryRequest('Vehicle.Speed',
+                             View.CURRENT_VALUE, (Field.VALUE,)),
             ))
             sub_uid = await subscriber_manager.add_subscriber(subscribe_response_stream, callback=callback)
 
             assert isinstance(sub_uid, uuid.UUID)
             while callback.call_count < 1:
                 await asyncio.sleep(0.01)
-            actual_updates = [list(call_args[0][0]) for call_args in callback.call_args_list]
+            actual_updates = [list(call_args[0][0])
+                              for call_args in callback.call_args_list]
             assert actual_updates == [
                 [EntryUpdate(entry=DataEntry(path='Vehicle.Speed', value=Datapoint(
                     value=43.0,
-                    timestamp=datetime.datetime(2022, 11, 7, 16, 18, 32, 247307, tzinfo=datetime.timezone.utc),
+                    timestamp=datetime.datetime(
+                        2022, 11, 7, 16, 18, 32, 247307, tzinfo=datetime.timezone.utc),
                 )), fields=[Field.VALUE])],
             ]
 
     @pytest.mark.usefixtures('val_server')
     async def test_remove_subscriber(self, mocker, unused_tcp_port, val_servicer):
         async with VSSClient('127.0.0.1', unused_tcp_port, ensure_startup_connection=False) as client:
             subscriber_manager = SubscriberManager(client)
             responses = (
                 val_pb2.SubscribeResponse(updates=[
                     val_pb2.EntryUpdate(entry=types_pb2.DataEntry(
                         path='Vehicle.Speed',
                         value=types_pb2.Datapoint(
-                            timestamp=timestamp_pb2.Timestamp(seconds=1667837915, nanos=247307674),
+                            timestamp=timestamp_pb2.Timestamp(
+                                seconds=1667837915, nanos=247307674),
                             float=42.0,
                         ),
                     ), fields=(Field.VALUE,)),
                 ]),
             )
-            val_servicer.Subscribe.return_value = (response for response in responses)
+            val_servicer.Subscribe.return_value = (
+                response for response in responses)
             subscribe_response_stream = client.subscribe(entries=(
-                EntryRequest('Vehicle.Speed', View.CURRENT_VALUE, (Field.VALUE,)),
+                EntryRequest('Vehicle.Speed',
+                             View.CURRENT_VALUE, (Field.VALUE,)),
             ))
             sub_uid = await subscriber_manager.add_subscriber(subscribe_response_stream, callback=mocker.Mock())
             subscriber = subscriber_manager.subscribers.get(sub_uid)
 
             await subscriber_manager.remove_subscriber(sub_uid)
 
             assert subscriber_manager.subscribers.get(sub_uid) is None
```

