# Comparing `tmp/dns_exporter-0.2.0b2.tar.gz` & `tmp/dns_exporter-0.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dns_exporter-0.2.0b2.tar", last modified: Sun Jan  8 16:38:34 2023, max compression
+gzip compressed data, was "dns_exporter-0.2.0b3.tar", last modified: Mon Jan  9 07:38:18 2023, max compression
```

## Comparing `dns_exporter-0.2.0b2.tar` & `dns_exporter-0.2.0b3.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-08 16:38:34.112000 dns_exporter-0.2.0b2/
--rw-r--r--   0 user      (1000) user      (1000)       55 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b2/.flake8
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-08 16:38:34.108000 dns_exporter-0.2.0b2/.github/
--rw-r--r--   0 user      (1000) user      (1000)      502 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b2/.github/dependabot.yml
--rw-r--r--   0 user      (1000) user      (1000)     1842 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b2/.gitignore
--rw-r--r--   0 user      (1000) user      (1000)      853 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b2/.pre-commit-config.yaml
--rw-r--r--   0 user      (1000) user      (1000)       60 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b2/.yamllint
--rw-r--r--   0 user      (1000) user      (1000)      350 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b2/CHANGELOG.md
--rw-r--r--   0 user      (1000) user      (1000)     1509 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b2/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)     1445 2023-01-08 16:38:34.112000 dns_exporter-0.2.0b2/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      794 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b2/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-08 16:38:34.109000 dns_exporter-0.2.0b2/dns_exporter/
--rw-r--r--   0 user      (1000) user      (1000)       46 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b2/dns_exporter/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)      162 2023-01-08 16:38:33.000000 dns_exporter-0.2.0b2/dns_exporter/_version.py
--rw-r--r--   0 user      (1000) user      (1000)    32022 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b2/dns_exporter/dns_exporter.py
--rw-r--r--   0 user      (1000) user      (1000)     1077 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b2/dns_exporter/dns_exporter.yml
--rw-r--r--   0 user      (1000) user      (1000)     3739 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b2/dns_exporter/example.yml
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-08 16:38:34.112000 dns_exporter-0.2.0b2/dns_exporter.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1445 2023-01-08 16:38:33.000000 dns_exporter-0.2.0b2/dns_exporter.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      493 2023-01-08 16:38:34.000000 dns_exporter-0.2.0b2/dns_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-01-08 16:38:33.000000 dns_exporter-0.2.0b2/dns_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       64 2023-01-08 16:38:33.000000 dns_exporter-0.2.0b2/dns_exporter.egg-info/entry_points.txt
--rw-r--r--   0 user      (1000) user      (1000)      149 2023-01-08 16:38:33.000000 dns_exporter-0.2.0b2/dns_exporter.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       13 2023-01-08 16:38:33.000000 dns_exporter-0.2.0b2/dns_exporter.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)     1097 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b2/pyproject.toml
--rwxr-xr-x   0 user      (1000) user      (1000)     1262 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b2/release.sh
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-01-08 16:38:34.112000 dns_exporter-0.2.0b2/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      114 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b2/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-09 07:38:18.288000 dns_exporter-0.2.0b3/
+-rw-r--r--   0 user      (1000) user      (1000)       55 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b3/.flake8
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-09 07:38:18.284000 dns_exporter-0.2.0b3/.github/
+-rw-r--r--   0 user      (1000) user      (1000)      502 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b3/.github/dependabot.yml
+-rw-r--r--   0 user      (1000) user      (1000)     1842 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b3/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)      853 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b3/.pre-commit-config.yaml
+-rw-r--r--   0 user      (1000) user      (1000)       60 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b3/.yamllint
+-rw-r--r--   0 user      (1000) user      (1000)      562 2023-01-09 07:37:48.000000 dns_exporter-0.2.0b3/CHANGELOG.md
+-rw-r--r--   0 user      (1000) user      (1000)     1509 2023-01-08 13:22:11.000000 dns_exporter-0.2.0b3/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    15974 2023-01-09 07:38:18.287000 dns_exporter-0.2.0b3/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)    15323 2023-01-09 07:37:48.000000 dns_exporter-0.2.0b3/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-09 07:38:18.285000 dns_exporter-0.2.0b3/dns_exporter/
+-rw-r--r--   0 user      (1000) user      (1000)       46 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b3/dns_exporter/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      162 2023-01-09 07:38:18.000000 dns_exporter-0.2.0b3/dns_exporter/_version.py
+-rw-r--r--   0 user      (1000) user      (1000)    35913 2023-01-09 07:37:48.000000 dns_exporter-0.2.0b3/dns_exporter/dns_exporter.py
+-rw-r--r--   0 user      (1000) user      (1000)     4904 2023-01-09 07:37:48.000000 dns_exporter-0.2.0b3/dns_exporter/dns_exporter_example.yml
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-09 07:38:18.286000 dns_exporter-0.2.0b3/dns_exporter.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    15974 2023-01-09 07:38:18.000000 dns_exporter-0.2.0b3/dns_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      476 2023-01-09 07:38:18.000000 dns_exporter-0.2.0b3/dns_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-01-09 07:38:18.000000 dns_exporter-0.2.0b3/dns_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       64 2023-01-09 07:38:18.000000 dns_exporter-0.2.0b3/dns_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)      163 2023-01-09 07:38:18.000000 dns_exporter-0.2.0b3/dns_exporter.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       13 2023-01-09 07:38:18.000000 dns_exporter-0.2.0b3/dns_exporter.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1120 2023-01-09 07:37:48.000000 dns_exporter-0.2.0b3/pyproject.toml
+-rwxr-xr-x   0 user      (1000) user      (1000)     1262 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b3/release.sh
+-rw-r--r--   0 user      (1000) user      (1000)       38 2023-01-09 07:38:18.288000 dns_exporter-0.2.0b3/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      114 2023-01-08 16:36:24.000000 dns_exporter-0.2.0b3/setup.py
```

### Comparing `dns_exporter-0.2.0b2/.gitignore` & `dns_exporter-0.2.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `dns_exporter-0.2.0b2/.pre-commit-config.yaml` & `dns_exporter-0.2.0b3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dns_exporter-0.2.0b2/LICENSE` & `dns_exporter-0.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `dns_exporter-0.2.0b2/dns_exporter/dns_exporter.py` & `dns_exporter-0.2.0b3/dns_exporter/dns_exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """dns_exporter is a blackbox-style Prometheus exporter for DNS."""
+import argparse
 import ipaddress
 import logging
 import random
 import re
 import socket
 import sys
 import time
@@ -29,38 +30,34 @@
     Histogram,
     Info,
     MetricsHandler,
     exposition,
 )
 from prometheus_client.registry import RestrictedRegistry
 
+# get version number from package metadata if possible
 __version__: str = "0.0.0"
 try:
     __version__ = version("dns_exporter")
 except PackageNotFoundError:
-    # package is not installed
+    # package is not installed, get version from file
     try:
         from _version import version as __version__  # type: ignore
     except ImportError:
+        # this must be a git checkout with no _version.py file, version unknown
         pass
 
+# initialise logger
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 ch = logging.StreamHandler()
 ch.setLevel(logging.DEBUG)
-
-# create formatter
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-
-# add formatter to ch
 ch.setFormatter(formatter)
-
-# add ch to logger
 logger.addHandler(ch)
-
 logger.info(f"dns_exporter v{__version__} starting up")
 
 # create seperate registry for the dns query metrics
 dns_registry = CollectorRegistry()
 
 # define the timing histogram
 QUERY_TIME = Histogram(
@@ -90,15 +87,14 @@
     registry=dns_registry,
 )
 # and the failure Enum
 QUERY_FAILURE = Enum(
     "dns_query_failure_reason",
     "The reason this DNS query failed",
     states=[
-        "initial_state",
         "invalid_request_module",
         "invalid_request_target",
         "invalid_request_family",
         "invalid_request_ip",
         "invalid_request_protocol",
         "timeout",
         "invalid_response_rcode",
@@ -176,23 +172,21 @@
     def validate_request_querystring(
         self,
         query: dict[str, str],
         config: dict[str, Union[str, int, float, list[str], dict[str, str]]],
     ) -> bool:
         """Validate the incoming scrape HTTP request before doing the DNS query."""
         # do we have a module in the request?
-        if "module" not in query or query["module"] not in config["modules"]:  # type: ignore
+        if "module" in query and ("modules" not in config or query["module"] not in config["modules"]):  # type: ignore
+            logger.warning(
+                "Scrape request contains a module '{query['module']}' but the module is unknown to this exporter."
+            )
             QUERY_SUCCESS.set(0)
             QUERY_FAILURE.state("invalid_request_module")
             return False
-        elif "target" not in query:
-            QUERY_SUCCESS.set(0)
-            QUERY_FAILURE.state("invalid_request_target")
-            return False
-
         # all good
         return True
 
     def get_module(self, qs: dict[str, str]) -> None:
         """Construct the module from defaults, config file, and querystring."""
         # defaults have lowest precedence
         self.module: dict[
@@ -213,17 +207,18 @@
             "valid_rcodes": ["NOERROR"],
             "validate_response_flags": {},
             "validate_answer_rrs": {},
             "validate_authority_rrs": {},
             "validate_additional_rrs": {},
         }
 
-        # the module config has middle precedence
-        assert hasattr(self, "config")  # mypy
-        self.module.update(self.config["modules"][qs["module"]])
+        # the module from the config file has middle precedence,
+        # if one was specified in the querystring
+        if "module" in qs and hasattr(self, "config") and "modules" in self.config:
+            self.module.update(self.config["modules"][qs["module"]])
 
         # and the querystring from the scrape request has highest precedence,
         # overruling values from defaults and module
         self.module.update(qs)
         return None
 
     def validate_module(self) -> bool:
@@ -621,14 +616,15 @@
             assert hasattr(self, "config")  # mypy
             if not self.validate_request_querystring(query=self.qs, config=self.config):
                 # the validate method already did everything needed so just return
                 logger.warning("invalid querystring, scrape failed")
                 self.send_metric_response(registry=dns_registry, query=self.qs)
                 return
 
+            logger.debug(f"Got scrape request from client {self.client_address}")
             # assemble module (configuration for this scrape) from defaults, config file and request
             self.get_module(qs=self.qs)
             if not self.validate_module():
                 # something is not right with the module config
                 logger.warning("invalid module config, scrape failed")
                 self.send_metric_response(registry=dns_registry, query=self.qs)
                 return
@@ -687,31 +683,34 @@
                 r = self.get_dns_response(
                     protocol=str(self.module["protocol"]),
                     target=str(self.module["target"]),
                     ip=str(self.module["ip"]),
                     query=q,
                     timeout=float(str(self.module["timeout"])),
                 )
+                logger.debug("Got a DNS query response!")
             except dns.exception.Timeout:
                 # configured timeout was reached before we got a response
                 QUERY_FAILURE.state("timeout")
+                logger.error("DNS query timeout was reached")
             except Exception:
                 logger.exception(
                     f"Got an exception while module {self.qs['module']} was looking up qname {self.module['query_name']} using target {self.module['target']}"
                 )
                 # unknown failure
                 QUERY_FAILURE.state("other")
             # clock it
             qtime = time.time() - start
 
             if r is None:
                 # we did not get a response :(
                 DNS_FAILURES.inc()
                 QUERY_SUCCESS.set(0)
                 self.send_metric_response(registry=dns_registry, query=self.qs)
+                logger.debug("Returning DNS query metrics - no response received :(")
                 return
 
             # we got a response, increase the response counter
             DNS_RESPONSES.inc()
 
             # make mypy happy
             assert hasattr(r, "opcode")
@@ -759,47 +758,140 @@
 
             # register success or not
             QUERY_SUCCESS.set(success)
             # send the response
             self.send_metric_response(
                 registry=dns_registry, query=self.qs, skip_metrics=skip_metrics
             )
+            logger.debug(f"Returning DNS query metrics - query success: {success}")
             return
 
         # this endpoint exposes metrics about the exporter itself and the python process
         elif self.url.path == "/metrics":
             self.send_metric_response(registry=self.registry, query=self.qs)
+            logger.debug("Returning exporter metrics for request to /metrics")
             return
 
         # the root just returns a bit of informational html
         elif self.url.path == "/":
             # return a basic index page
             self.send_response(200)
             self.end_headers()
             self.wfile.write(INDEX.encode("utf-8"))
             HTTP_RESPONSES.labels(path="/", response_code=200).inc()
+            logger.debug("Returning index page for request to /")
 
         # unknown endpoint
         else:
             self.send_response(404)
             self.end_headers()
             HTTP_RESPONSES.labels(path=self.url.path, response_code=404).inc()
+            logger.debug(f"Unknown endpoint '{self.url.path}' returning 404")
             return None
 
 
-def main() -> None:
+def get_parser() -> argparse.ArgumentParser:
+    """Create and return the argparse object."""
+    parser = argparse.ArgumentParser(
+        description=f"dns_exporter version {__version__}. See ReadTheDocs for more info."
+    )
+
+    # optional arguments
+    parser.add_argument(
+        "-c",
+        "--config-file",
+        dest="config-file",
+        help="The path to the yaml config file to use. Only the root 'modules' key is read from the config file.",
+        default=argparse.SUPPRESS,
+    )
+    parser.add_argument(
+        "-d",
+        "--debug",
+        action="store_const",
+        dest="log-level",
+        const="DEBUG",
+        help="Debug mode. Equal to setting --log-level=DEBUG.",
+        default=argparse.SUPPRESS,
+    )
+    parser.add_argument(
+        "-l",
+        "--log-level",
+        dest="log-level",
+        choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
+        help="Logging level. One of DEBUG, INFO, WARNING, ERROR, CRITICAL. Defaults to INFO.",
+        default=argparse.SUPPRESS,
+    )
+    parser.add_argument(
+        "-q",
+        "--quiet",
+        action="store_const",
+        dest="log-level",
+        const="WARNING",
+        help="Quiet mode. No output at all if there is nothing to do, and no errors are encountered. Equal to setting --log-level=WARNING.",
+        default=argparse.SUPPRESS,
+    )
+    parser.add_argument(
+        "-v",
+        "--version",
+        dest="version",
+        action="store_true",
+        help="Show version and exit.",
+        default=argparse.SUPPRESS,
+    )
+    return parser
+
+
+def parse_args(
+    mockargs: Optional[list[str]] = None,
+) -> tuple[argparse.ArgumentParser, argparse.Namespace]:
+    """Create an argparse monster and parse mockargs or sys.argv[1:]."""
+    parser = get_parser()
+    args = parser.parse_args(mockargs if mockargs else sys.argv[1:])
+    return parser, args
+
+
+def main(mockargs: Optional[list[str]] = None) -> None:
     """Read config and start exporter."""
-    with open("dns_exporter.yml") as f:
-        try:
-            config = yaml.load(f, Loader=yaml.SafeLoader)
-        except Exception:
-            logger.exception(
-                "Unable to parse YAML config file dns_exporter.yml - bailing out."
+    # get arpparser and parse args
+    parser, args = parse_args(mockargs)
+
+    # handle a couple of special cases before reading config
+    if hasattr(args, "version"):
+        print(f"dns_exporter version {__version__}")
+        sys.exit(0)
+
+    if hasattr(args, "config-file"):
+        with open(getattr(args, "config-file"), "r") as f:
+            try:
+                config = yaml.load(f, Loader=yaml.SafeLoader)
+            except Exception:
+                logger.exception(
+                    f"Unable to parse YAML config file {getattr(args, 'config-file')} - bailing out."
+                )
+                sys.exit(1)
+        if (
+            not config
+            or "modules" not in config
+            or not isinstance(config["modules"], dict)
+            or not config["modules"]
+        ):
+            # config is empty, missing "modules" key, or modules is empty or not a dict
+            logger.error(
+                f"Invalid config file {getattr(args, 'config-file')} - yaml was valid but no modules found"
             )
             sys.exit(1)
+        logger.debug(
+            f"The following modules were loaded from config file {getattr(args, 'config-file')}: {list(config['modules'].keys())}"
+        )
+    else:
+        # we have no config file
+        config = {}
+        logger.debug("No -c / --config-file found so a config file will not be used.")
+
+    # initialise handler and start HTTPServer
     handler = DNSRequestHandler
     handler.config = config  # type: ignore
     HTTPServer(("127.0.0.1", 15353), handler).serve_forever()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dns_exporter-0.2.0b2/pyproject.toml` & `dns_exporter-0.2.0b3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "dnspython >= 2.2.1",
+    "httpx >= 0.23.3",
     "PyYAML >= 6.0",
     "prometheus-client >= 0.15.0",
 ]
 description = "Prometheus exporter for blackbox-style DNS monitoring"
 dynamic = ["version"]
 keywords = ["prometheus", "dns", "monitoring"]
 license = {text = "BSD 3-Clause License"}
```

### Comparing `dns_exporter-0.2.0b2/release.sh` & `dns_exporter-0.2.0b3/release.sh`

 * *Files identical despite different names*

