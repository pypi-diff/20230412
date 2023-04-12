# Comparing `tmp/steampunk_spotter-1.2.4rc1-py3-none-any.whl.zip` & `tmp/steampunk_spotter-1.2.5a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,37 @@
-Zip file size: 45269 bytes, number of entries: 22
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-07 11:04 spotter/__init__.py
--rw-r--r--  2.0 unx    15218 b- defN 23-Apr-05 16:13 spotter/api.py
--rw-r--r--  2.0 unx     4694 b- defN 23-Apr-07 09:48 spotter/cli.py
+Zip file size: 59097 bytes, number of entries: 35
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 09:05 spotter/__init__.py
+-rw-r--r--  2.0 unx    17100 b- defN 23-Apr-12 08:41 spotter/api.py
+-rw-r--r--  2.0 unx     5069 b- defN 23-Apr-11 07:58 spotter/cli.py
 -rw-r--r--  2.0 unx    18318 b- defN 23-Mar-20 10:48 spotter/environment.py
 -rw-r--r--  2.0 unx    24670 b- defN 23-Apr-07 06:33 spotter/parsing.py
--rw-r--r--  2.0 unx     6839 b- defN 23-Mar-30 14:43 spotter/rewriting.py
--rw-r--r--  2.0 unx     5558 b- defN 23-Apr-07 06:33 spotter/storage.py
+-rw-r--r--  2.0 unx     5558 b- defN 23-Apr-11 07:58 spotter/storage.py
 -rw-r--r--  2.0 unx     2752 b- defN 23-Mar-20 10:29 spotter/utils.py
--rw-r--r--  2.0 unx       94 b- defN 23-Apr-07 09:48 spotter/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 09:05 spotter/commands/__init__.py
+-rw-r--r--  2.0 unx     3952 b- defN 23-Apr-11 07:05 spotter/commands/clear_policies.py
 -rw-r--r--  2.0 unx     2347 b- defN 23-Apr-05 12:42 spotter/commands/login.py
 -rw-r--r--  2.0 unx     1141 b- defN 23-Mar-13 12:10 spotter/commands/register.py
--rw-r--r--  2.0 unx    38545 b- defN 23-Apr-07 09:48 spotter/commands/scan.py
+-rw-r--r--  2.0 unx    38655 b- defN 23-Apr-11 07:05 spotter/commands/scan.py
+-rw-r--r--  2.0 unx     5209 b- defN 23-Apr-11 07:05 spotter/commands/set_policies.py
 -rw-r--r--  2.0 unx     3620 b- defN 23-Mar-30 14:43 spotter/commands/suggest.py
 -rw-r--r--  2.0 unx       60 b- defN 23-Mar-14 07:59 spotter/reporting/__init__.py
 -rw-r--r--  2.0 unx     3459 b- defN 23-Mar-14 07:59 spotter/reporting/report.py
--rw-rw-rw-  2.0 unx    11358 b- defN 23-Apr-07 11:05 steampunk_spotter-1.2.4rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx    19428 b- defN 23-Apr-07 11:05 steampunk_spotter-1.2.4rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 11:05 steampunk_spotter-1.2.4rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 23-Apr-07 11:05 steampunk_spotter-1.2.4rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-07 11:05 steampunk_spotter-1.2.4rc1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-07 11:05 steampunk_spotter-1.2.4rc1.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1840 b- defN 23-Apr-07 11:05 steampunk_spotter-1.2.4rc1.dist-info/RECORD
-22 files, 160087 bytes uncompressed, 42273 bytes compressed:  73.6%
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 09:05 spotter/rewriting/__init__.py
+-rw-r--r--  2.0 unx     7545 b- defN 23-Apr-11 07:05 spotter/rewriting/models.py
+-rw-r--r--  2.0 unx     7055 b- defN 23-Apr-11 07:05 spotter/rewriting/processor.py
+-rw-r--r--  2.0 unx     1937 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_action_inline.py
+-rw-r--r--  2.0 unx     2318 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_action_object.py
+-rw-r--r--  2.0 unx      989 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_always_run.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_fqcn.py
+-rw-r--r--  2.0 unx     2087 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_inline.py
+-rw-r--r--  2.0 unx     2527 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_local_action_inline.py
+-rw-r--r--  2.0 unx     2312 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_local_object.py
+-rw-r--r--  2.0 unx      989 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_module_inline.py
+-rw-r--r--  2.0 unx      888 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_module_object.py
+-rw-rw-rw-  2.0 unx    11358 b- defN 23-Apr-12 09:06 steampunk_spotter-1.2.5a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    21591 b- defN 23-Apr-12 09:06 steampunk_spotter-1.2.5a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 09:06 steampunk_spotter-1.2.5a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 23-Apr-12 09:06 steampunk_spotter-1.2.5a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-12 09:06 steampunk_spotter-1.2.5a1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-12 09:06 steampunk_spotter-1.2.5a1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     3062 b- defN 23-Apr-12 09:06 steampunk_spotter-1.2.5a1.dist-info/RECORD
+35 files, 197696 bytes uncompressed, 54135 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -9,59 +9,98 @@
 
 Filename: spotter/environment.py
 Comment: 
 
 Filename: spotter/parsing.py
 Comment: 
 
-Filename: spotter/rewriting.py
-Comment: 
-
 Filename: spotter/storage.py
 Comment: 
 
 Filename: spotter/utils.py
 Comment: 
 
 Filename: spotter/commands/__init__.py
 Comment: 
 
+Filename: spotter/commands/clear_policies.py
+Comment: 
+
 Filename: spotter/commands/login.py
 Comment: 
 
 Filename: spotter/commands/register.py
 Comment: 
 
 Filename: spotter/commands/scan.py
 Comment: 
 
+Filename: spotter/commands/set_policies.py
+Comment: 
+
 Filename: spotter/commands/suggest.py
 Comment: 
 
 Filename: spotter/reporting/__init__.py
 Comment: 
 
 Filename: spotter/reporting/report.py
 Comment: 
 
-Filename: steampunk_spotter-1.2.4rc1.dist-info/LICENSE
+Filename: spotter/rewriting/__init__.py
+Comment: 
+
+Filename: spotter/rewriting/models.py
+Comment: 
+
+Filename: spotter/rewriting/processor.py
+Comment: 
+
+Filename: spotter/rewriting/rewrite_action_inline.py
+Comment: 
+
+Filename: spotter/rewriting/rewrite_action_object.py
+Comment: 
+
+Filename: spotter/rewriting/rewrite_always_run.py
+Comment: 
+
+Filename: spotter/rewriting/rewrite_fqcn.py
+Comment: 
+
+Filename: spotter/rewriting/rewrite_inline.py
+Comment: 
+
+Filename: spotter/rewriting/rewrite_local_action_inline.py
+Comment: 
+
+Filename: spotter/rewriting/rewrite_local_object.py
+Comment: 
+
+Filename: spotter/rewriting/rewrite_module_inline.py
+Comment: 
+
+Filename: spotter/rewriting/rewrite_module_object.py
+Comment: 
+
+Filename: steampunk_spotter-1.2.5a1.dist-info/LICENSE
 Comment: 
 
-Filename: steampunk_spotter-1.2.4rc1.dist-info/METADATA
+Filename: steampunk_spotter-1.2.5a1.dist-info/METADATA
 Comment: 
 
-Filename: steampunk_spotter-1.2.4rc1.dist-info/WHEEL
+Filename: steampunk_spotter-1.2.5a1.dist-info/WHEEL
 Comment: 
 
-Filename: steampunk_spotter-1.2.4rc1.dist-info/entry_points.txt
+Filename: steampunk_spotter-1.2.5a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: steampunk_spotter-1.2.4rc1.dist-info/top_level.txt
+Filename: steampunk_spotter-1.2.5a1.dist-info/top_level.txt
 Comment: 
 
-Filename: steampunk_spotter-1.2.4rc1.dist-info/zip-safe
+Filename: steampunk_spotter-1.2.5a1.dist-info/zip-safe
 Comment: 
 
-Filename: steampunk_spotter-1.2.4rc1.dist-info/RECORD
+Filename: steampunk_spotter-1.2.5a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotter/api.py

```diff
@@ -159,15 +159,15 @@
         # old login - generate tokens (access and refresh token) and then save them to storage
         # note that we do not use self._request to prevent possible cyclic recursion errors
         response = requests.post(self._url("/v2/token/"), headers=self.DEFAULT_HEADERS.copy(),
                                  json={"username": self._username, "password": self._password}, timeout=timeout)
         if response.ok:
             self._update_endpoint_tokens(response.json())
         else:
-            print(self._format_api_error(response), file=sys.stderr)
+            print(self.format_api_error(response), file=sys.stderr)
             sys.exit(2)
 
     def _refresh_login(self, timeout: int = DEFAULT_TIMEOUT) -> None:
         """
         Login user to the API using the tokens (access and refresh token) from storage.
 
         :param timeout: Request timeout
@@ -187,30 +187,32 @@
             self._storage.update_json({
                 self._base_url: {
                     "access": access_token,
                     "refresh": refresh_token
                 }
             }, self._storage_tokens_path)
         else:
-            print(self._format_api_error(response_token_refresh), file=sys.stderr)
+            print(self.format_api_error(response_token_refresh), file=sys.stderr)
             sys.exit(2)
 
-    # pylint: disable=too-many-arguments,too-many-branches
+    # pylint: disable=too-many-arguments,too-many-branches,too-many-locals
     def _request(self, method: str, path: str, authorize: Optional[bool] = True,
                  headers: Optional[Dict[str, str]] = None, payload: Optional[Dict[str, Any]] = None,
-                 timeout: int = DEFAULT_TIMEOUT, allow_auth_retry: bool = True) -> requests.Response:
+                 timeout: int = DEFAULT_TIMEOUT, allow_auth_retry: bool = True,
+                 ignore_response_status_codes: Optional[bool] = False) -> requests.Response:
         """
         Send HTTP request.
 
         :param path: API endpoint path
         :param authorize: Add Authorization header to authorize request (True/False)
         :param headers: Request headers (JSON payload dict)
         :param payload: Request payload (JSON payload dict)
         :param timeout: Request timeout
         :param allow_auth_retry: Whether to allow reauthenticating and retrying the request
+        :param ignore_response_status_codes: Whether to ignore response status codes (even ones higher than 400)
         :return: Response object
         """
         # initiate login from start if API token or username and password have been provided and tokens do not exist yet
         if (self._api_token or (self._username and self._password)) and not self._storage.exists(
                 self._storage_tokens_path):
             self._storage.remove(self._storage_tokens_path)
             self.login()
@@ -244,100 +246,118 @@
             sys.exit(2)
 
         # if request fails for one time try to log in and make a request again
         if not self._api_token and response.status_code == 401:
             if allow_auth_retry:
                 self._refresh_login(timeout)
                 # retry, but don't allow any more auth retries
-                return self._request(method, path, authorize, headers, payload, timeout, allow_auth_retry=False)
+                return self._request(method, path, authorize, headers, payload, timeout, allow_auth_retry=False,
+                                     ignore_response_status_codes=ignore_response_status_codes)
 
             print("Request error after reauthenticating.", file=sys.stderr)
             sys.exit(2)
         else:
+            # just return the response no matter what the response status code is
+            if ignore_response_status_codes:
+                return response
             # check if response is ok and can be converted to JSON
             if response.ok:
                 try:
                     response.json()
                     return response
                 except ValueError as e:
                     print(f"Error: {e}", file=sys.stderr)
                     sys.exit(2)
             else:
-                print(self._format_api_error(response), file=sys.stderr)
+                print(self.format_api_error(response), file=sys.stderr)
                 sys.exit(2)
 
     def get(self, path: str, authorize: Optional[bool] = True, headers: Optional[Dict[str, str]] = None,
-            timeout: int = DEFAULT_TIMEOUT) -> requests.Response:
+            timeout: int = DEFAULT_TIMEOUT, ignore_response_status_codes: Optional[bool] = False) -> requests.Response:
         """
         Send GET request.
 
         :param path: API endpoint path
         :param authorize: Add Authorization header to authorize request (True/False)
         :param headers: Request headers (JSON payload dict)
         :param timeout: Request timeout
+        :param ignore_response_status_codes: Whether to ignore response status codes (even ones higher than 400)
         :return: Response object
         """
-        return self._request("GET", path, authorize=authorize, headers=headers, timeout=timeout)
+        return self._request("GET", path, authorize=authorize, headers=headers, timeout=timeout,
+                             ignore_response_status_codes=ignore_response_status_codes)
 
     def post(self, path: str, authorize: Optional[bool] = True, headers: Optional[Dict[str, str]] = None,
-             payload: Optional[Dict[str, Any]] = None, timeout: int = DEFAULT_TIMEOUT) -> requests.Response:
+             payload: Optional[Dict[str, Any]] = None, timeout: int = DEFAULT_TIMEOUT,
+             ignore_response_status_codes: Optional[bool] = False) -> requests.Response:
         """
         Send POST request.
 
         :param path: API endpoint path
         :param authorize: Add Authorization header to authorize request (True/False)
         :param headers: Request headers (JSON payload dict)
         :param payload: Request payload (JSON payload dict)
         :param timeout: Request timeout in seconds
+        :param ignore_response_status_codes: Whether to ignore response status codes (even ones higher than 400)
         :return: Response object
         """
-        return self._request("POST", path, authorize, headers, payload, timeout)
+        return self._request("POST", path, authorize=authorize, headers=headers, payload=payload, timeout=timeout,
+                             ignore_response_status_codes=ignore_response_status_codes)
 
     def patch(self, path: str, authorize: Optional[bool] = True, headers: Optional[Dict[str, str]] = None,
-              payload: Optional[Dict[str, Any]] = None, timeout: int = DEFAULT_TIMEOUT) -> requests.Response:
+              payload: Optional[Dict[str, Any]] = None, timeout: int = DEFAULT_TIMEOUT,
+              ignore_response_status_codes: Optional[bool] = False) -> requests.Response:
         """
         Send PATCH request.
 
         :param path: API endpoint path
         :param authorize: Add Authorization header to authorize request (True/False)
         :param headers: Request headers (JSON payload dict)
         :param payload: Request payload (JSON payload dict)
         :param timeout: Request timeout in seconds
+        :param ignore_response_status_codes: Whether to ignore response status codes (even ones higher than 400)
         :return: Response object
         """
-        return self._request("PATCH", path, authorize, headers, payload, timeout)
+        return self._request("PATCH", path, authorize=authorize, headers=headers, payload=payload, timeout=timeout,
+                             ignore_response_status_codes=ignore_response_status_codes)
 
     def put(self, path: str, authorize: Optional[bool] = True, headers: Optional[Dict[str, str]] = None,
-            payload: Optional[Dict[str, Any]] = None, timeout: int = DEFAULT_TIMEOUT) -> requests.Response:
+            payload: Optional[Dict[str, Any]] = None, timeout: int = DEFAULT_TIMEOUT,
+            ignore_response_status_codes: Optional[bool] = False) -> requests.Response:
         """
         Send PUT request.
 
         :param path: API endpoint path
         :param authorize: Add Authorization header to authorize request (True/False)
         :param headers: Request headers (JSON payload dict)
         :param payload: Request payload (JSON payload dict)
         :param timeout: Request timeout in seconds
+        :param ignore_response_status_codes: Whether to ignore response status codes (even ones higher than 400)
         :return: Response object
         """
-        return self._request("PUT", path, authorize, headers, payload, timeout)
+        return self._request("PUT", path, authorize=authorize, headers=headers, payload=payload, timeout=timeout,
+                             ignore_response_status_codes=ignore_response_status_codes)
 
     def delete(self, path: str, authorize: Optional[bool] = True, headers: Optional[Dict[str, str]] = None,
-               timeout: int = DEFAULT_TIMEOUT) -> requests.Response:
+               timeout: int = DEFAULT_TIMEOUT,
+               ignore_response_status_codes: Optional[bool] = False) -> requests.Response:
         """
         Send DELETE request.
 
         :param path: API endpoint path
         :param authorize: Add Authorization header to authorize request (True/False)
         :param headers: Request headers (JSON payload dict)
         :param timeout: Request timeout in seconds
+        :param ignore_response_status_codes: Whether to ignore response status codes (even ones higher than 400)
         :return: Response object
         """
-        return self._request("DELETE", path, authorize=authorize, headers=headers, timeout=timeout)
+        return self._request("DELETE", path, authorize=authorize, headers=headers, timeout=timeout,
+                             ignore_response_status_codes=ignore_response_status_codes)
 
-    def _format_api_error(self, response: requests.Response) -> str:
+    def format_api_error(self, response: requests.Response) -> str:
         """
         Format API error.
 
         :param response: Response object
         :return: Formatted API error as string
         """
         try:
```

## spotter/cli.py

```diff
@@ -1,19 +1,18 @@
 """Provide main CLI parser."""
 
 import argparse
-import inspect
 import sys
 from pathlib import Path
 from typing import Dict, Union, Sequence, Optional, Any, NoReturn
 
 import colorama
 
-from spotter import commands
 from spotter.api import ApiClient
+from spotter.commands import login, register, scan, suggest, set_policies, clear_policies
 from spotter.storage import Storage
 from spotter.utils import get_current_cli_version, validate_url
 
 
 class ArgParser(argparse.ArgumentParser):
     """An argument parser that displays help on error."""
 
@@ -38,15 +37,15 @@
 def create_parser() -> ArgParser:
     """
     Create argument parser for CLI.
 
     :return: Parser as argparse.ArgumentParser object
     """
     parser = ArgParser(
-        description="Steampunk Spotter - a quality scanner for Ansible Playbooks",
+        description="Steampunk Spotter - Ansible Playbook Scanning Tool",
         formatter_class=argparse.RawDescriptionHelpFormatter,
         epilog="additional information:\n"
                "  You will need Steampunk Spotter account to be able to use the CLI.\n"
                "  Create one with spotter register command or at https://spotter.steampunk.si/.\n\n"
                "  To log in to Steampunk Spotter, you should provide your API token or username and password:\n"
                "    - using spotter login command;\n"
                "    - via --api-token/-t optional argument;\n"
@@ -81,16 +80,23 @@
     )
     parser.add_argument(
         "--no-colors", action="store_true", help="Disable output colors"
     )
 
     subparsers = parser.add_subparsers()
     subparsers_metavar = ""
-    cmds = inspect.getmembers(commands, inspect.ismodule)
-    for command_name, module in sorted(cmds, key=lambda x: x[0]):
+    cmds = [
+        (register.__name__.rsplit(".", maxsplit=1)[-1], register),
+        (login.__name__.rsplit(".", maxsplit=1)[-1], login),
+        (scan.__name__.rsplit(".", maxsplit=1)[-1], scan),
+        (suggest.__name__.rsplit(".", maxsplit=1)[-1], suggest),
+        (set_policies.__name__.rsplit(".", maxsplit=1)[-1], set_policies),
+        (clear_policies.__name__.rsplit(".", maxsplit=1)[-1], clear_policies)
+    ]
+    for command_name, module in cmds:
         # FIXME: Remove this if we decide that suggest command can be used standalone
         if command_name != "suggest":
             subparsers_metavar += f"{command_name},"
         module.add_parser(subparsers)
 
     subparsers.metavar = f"{{{subparsers_metavar.rstrip(',')}}}"
     return parser
```

## spotter/commands/__init__.py

```diff
@@ -1,6 +0,0 @@
-00000000: 6672 6f6d 2073 706f 7474 6572 2e63 6f6d  from spotter.com
-00000010: 6d61 6e64 7320 696d 706f 7274 2028 2020  mands import (  
-00000020: 2320 6e6f 7161 3a20 4634 3031 0a20 2020  # noqa: F401.   
-00000030: 206c 6f67 696e 2c0a 2020 2020 7265 6769   login,.    regi
-00000040: 7374 6572 2c0a 2020 2020 7363 616e 2c0a  ster,.    scan,.
-00000050: 2020 2020 7375 6767 6573 740a 290a           suggest.).
```

## spotter/commands/scan.py

```diff
@@ -16,16 +16,18 @@
 import yaml
 from colorama import Fore, Style
 from pydantic.json import pydantic_encoder
 
 from spotter.api import ApiClient
 from spotter.environment import Environment
 from spotter.parsing import parse_ansible_artifacts, ParsingResult
+
 from spotter.reporting.report import JUnitXml
-from spotter.rewriting import CheckType, Suggestion, update_files
+from spotter.rewriting.processor import update_files
+from spotter.rewriting.models import RewriteSuggestion, CheckType
 from spotter.storage import Storage
 from spotter.utils import prompt_yes_no_question
 
 
 class DisplayLevel(Enum):
     """Enum that holds different levels/statuses for check result."""
 
@@ -257,15 +259,15 @@
 
     correlation_id: str
     original_item: Dict[str, Any]
     metadata: Optional[ItemMetadata]
     catalog_info: CheckCatalogInfo
     level: DisplayLevel
     message: str
-    suggestion: Optional[Suggestion]
+    suggestion: Optional[RewriteSuggestion]
     doc_url: Optional[str]
     check_type: CheckType
 
     def construct_output(self, disable_colors: bool = False, disable_docs_url: bool = False) -> str:
         """
         Construct CheckResult output using its properties.
 
@@ -273,15 +275,15 @@
         :param disable_docs_url: Disable outputting URL to documentation
         :return: Formatted output for check result
         """
         # or: we can have results that relate to Environment - no file and position
         metadata = self.metadata or ItemMetadata(file_name="", line=0, column=0)
         result_level = self.level.name.strip().upper()
         file_location = f"{metadata.file_name}:{metadata.line}:{metadata.column}"
-        out_prefix = f"{file_location}: [{self.catalog_info.event_code}]"
+        out_prefix = f"{file_location}: {result_level}: [{self.catalog_info.event_code}]"
         out_message = self.message.strip()
         if not disable_colors:
             if result_level == DisplayLevel.ERROR.name:
                 out_prefix = Fore.RED + out_prefix + Fore.RESET
                 out_message = re.sub(r"'([^']*)'", Style.BRIGHT + Fore.RED + r"\1" + Fore.RESET + Style.NORMAL,
                                      out_message)
             elif result_level == DisplayLevel.WARNING.name:
@@ -401,15 +403,16 @@
         item_meta = original_item.get("spotter_metadata", None)
         if not item_meta:
             print("Meta data is missing.")
             return None
 
         suggestion = element.get("suggestion", "")
         item_metadata_object = ItemMetadata.from_item_meta(item_meta)
-        suggestion_object: Optional[Suggestion] = Suggestion.from_item(check_type, original_item, suggestion)
+        suggestion_object: Optional[RewriteSuggestion] = \
+            RewriteSuggestion.from_item(check_type, original_item, suggestion)
         display_level = DisplayLevel.from_string(element.get("level", ""))
 
         result = CheckResult(
             correlation_id=correlation_id, original_item=original_item, metadata=item_metadata_object,
             catalog_info=CheckCatalogInfo.from_api_response_element(element), level=display_level,
             message=element.get("message", ""), suggestion=suggestion_object, doc_url=element.get("doc_url", ""),
             check_type=check_type
@@ -539,15 +542,15 @@
             metadata = result.metadata or ItemMetadata(file_name="", line=0, column=0)
             catalog_info = result.catalog_info
             suggestion_dict = {}
             if result.suggestion:
                 suggestion_dict = {
                     "start_mark": result.suggestion.start_mark,
                     "end_mark": result.suggestion.end_mark,
-                    "suggestion": result.suggestion.suggestion,
+                    "suggestion": result.suggestion.suggestion_spec,
                 }
 
             check_result_outputs.append({
                 "task_id": result.correlation_id,  # It is here because we want to be back compatible
                 "file": metadata.file_name,
                 "line": metadata.line,
                 "column": metadata.column,
```

## Comparing `spotter/rewriting.py` & `spotter/rewriting/processor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,176 +1,149 @@
-"""Provide rewriting - automated applying of suggestions to the code."""
+"""Entry point of rewriting functionality."""
+from typing import Optional, List, cast
 
-from enum import Enum
-import itertools
 import os
-import re
-from pathlib import Path
-from typing import Any, Dict, List, Tuple, Optional
+import itertools
 
-import pydantic.dataclasses
 import yaml
 
+from spotter.rewriting.rewrite_action_inline import RewriteActionInline
+from spotter.rewriting.rewrite_action_object import RewriteActionObject
+from spotter.rewriting.rewrite_always_run import RewriteAlwaysRun
+from spotter.rewriting.rewrite_fqcn import RewriteFqcn
+from spotter.rewriting.rewrite_inline import RewriteInline
+from spotter.rewriting.rewrite_local_action_inline import RewriteLocalActionInline
+from spotter.rewriting.rewrite_local_object import RewriteLocalActionObject
+from spotter.rewriting.models import Replacement, RewriteResult
+from spotter.rewriting.models import RewriteSuggestion
+
+
+class RewriteProcessor:
+    """Factory that will use correct implementation depending on 'action' inside 'suggestion'."""
+
+    rewriter_mapping = {
+        "FIX_FQCN": RewriteFqcn,
+        "FIX_INLINE": RewriteInline,
+        "FIX_ALWAYS_RUN": RewriteAlwaysRun,
+        "FIX_ACTION_INLINE": RewriteActionInline,
+        "FIX_ACTION_OBJECT": RewriteActionObject,
+        "FIX_LOCAL_ACTION_OBJECT": RewriteLocalActionObject,
+        "FIX_LOCAL_ACTION_INLINE": RewriteLocalActionInline,
+    }
 
-OKGREEN = "\033[92m"
-OKRED = "\033[0;31m"
-ENDC = "\033[0m"
-
-
-class CheckType(Enum):
-    """Enum that holds different check types for check result."""
-
-    TASK = "task"
-    PLAY = "play"
-    REQUIREMENTS = "requirements"
-    ANSIBLE_CFG = "ansible_cfg"
-    OTHER = "other"
-
-    def __str__(self) -> str:
+    @classmethod
+    def execute(cls, content: str, suggestion: RewriteSuggestion) -> Optional[RewriteResult]:
         """
-        Convert CheckType to lowercase string.
+        Update task content.
 
-        :return: String in lowercase
+        :param content: Old task content
+        :param suggestion: Suggestion object for a specific task
+        :return: Tuple with updated content and content length difference, or none if matching failed.
         """
-        return str(self.name.lower())
+        replacement = cls.get_replacement(content, suggestion)
+        if not replacement:
+            return RewriteResult(content=content, diff_size=0)
+
+        return replacement.apply()
 
     @classmethod
-    def from_string(cls, check_type: str) -> "CheckType":
+    def multi_execute(cls, content: str, suggestions: List[RewriteSuggestion]) -> RewriteResult:
         """
-        Convert string level to CheckType object.
+        Update task content with multiple suggestions.
 
-        :param level: Check result level
-        :return: CheckType object
-        """
-        try:
-            return cls[check_type.upper()]
-        except KeyError:
-            print(f"Warning: nonexistent check result type: {check_type}, "
-                  f"valid values are: {list(str(e) for e in CheckType)}.")
-            return CheckType.OTHER
-
-
-@pydantic.dataclasses.dataclass
-class Suggestion:
-    """Suggestion for rewriting Ansible task or play."""
-
-    check_type: CheckType
-    item_args: Dict[str, Any]
-    file: Path
-    file_parent: Path
-    start_mark: int
-    end_mark: int
-    suggestion: Dict[str, Any]
+        :param content: Old task content
+        :param suggestions: List of suggestions of specific tasks
+        :return: List of tuples with updated content and content length difference, or none if matching failed
+        """
+        for suggestion in suggestions:
+            replacement = cls.get_replacement(content, suggestion)
+            if replacement is None:
+                raise TypeError()
+            rewrite_result = replacement.apply()
+            new_content, length_diff = rewrite_result.content, rewrite_result.diff_size
+            content = new_content
+            suggestion.end_mark = len(content)
+        return RewriteResult(content=content, diff_size=length_diff)
 
     @classmethod
-    def from_item(
-        cls, check_type: CheckType, item: Dict[str, Any], suggestion: Optional[Dict[str, Any]]
-    ) -> Optional["Suggestion"]:
+    def get_replacement(cls, content: str, suggestion: RewriteSuggestion) -> Optional[Replacement]:
         """
-        Create Suggestion object for rewriting Ansible task or play.
+        Get replacement according to action.
 
-        :param task: Ansible task content.
-        :param suggestion: Suggestion as dict with action to do and data to use for update
+        :param content: Old task content
+        :param suggestion: Suggestion object for a specific task
         """
-        if not suggestion:
-            return None
-
-        if check_type == CheckType.TASK:
-            item_args = item["task_args"]
-        elif check_type == CheckType.PLAY:
-            item_args = item["play_args"]
-        else:
-            item_args = None
-
-        file_path = Path(item["spotter_metadata"]["file"])
-
-        return cls(
-            check_type=check_type,
-            item_args=item_args,
-            file=file_path,
-            file_parent=file_path.parent,
-            start_mark=item["spotter_metadata"]["start_mark_index"],
-            end_mark=item["spotter_metadata"]["end_mark_index"],
-            suggestion=suggestion
-        )
+        suggestion_dict = suggestion.suggestion_spec
+        action = cast(str, suggestion_dict.get("action"))
 
+        rewriter_class = cls.rewriter_mapping.get(action)
+        if not rewriter_class:
+            print(f"Unknown mapping: {action}")
+            return None
 
-def _update_content(content: str, suggestion: Suggestion,
-                    colorize: Optional[bool] = False) -> Optional[Tuple[str, int]]:
-    """
-    Update task content.
-
-    :param content: Old task content
-    :param suggestion: Suggestion object for a specific task
-    :param colorize: If True color things that will be changed
-    :return: Tuple with updated content and content length difference, or none if matching failed.
-    """
-    suggestion_dict = suggestion.suggestion
-    if suggestion_dict.get("action") != "FIX_FQCN":
-        return content, 0
-
-    part = content[suggestion.start_mark:suggestion.end_mark]
-    before = suggestion_dict["data"]["before"]
-    after = suggestion_dict["data"]["after"]
-    regex = rf"([\t ]*)({before})(\s*:\s*)"
-
-    replacement = f"{OKGREEN}{after}{ENDC}" if colorize else after
-    match = re.search(regex, part, re.MULTILINE)
-    if match is None:
-        print("Applying suggestion failed: could not find string to replace.")
-        return None
-
-    s_index, e_index = match.span(2)
-    end_content = content[:suggestion.start_mark + s_index] + replacement + content[suggestion.start_mark + e_index:]
-    return end_content, len(replacement) - len(before)
+        rewriter = rewriter_class()  # type: ignore[abstract]  # we assume the mapping only contains implementations
+        replacement = rewriter.get_replacement(content, suggestion)
+        return replacement
 
 
-def update_files(suggestions: List[Suggestion]) -> None:  # pylint: disable=too-many-locals
+def update_files(suggestions: List[RewriteSuggestion]) -> None:  # pylint: disable=too-many-locals
     """
     Update files by following suggestions.
 
     :param suggestions: List of suggestions as Suggestion objects
     """
     get_file_func = lambda x: x.file  # pylint: disable=unnecessary-lambda-assignment
     files = [(file, list(suggests)) for file, suggests in itertools.groupby(suggestions, get_file_func)]
 
     get_inode_func = lambda x: os.stat(x[0]).st_ino  # pylint: disable=unnecessary-lambda-assignment
     inodes = [next(group) for _, group in itertools.groupby(sorted(files, key=get_inode_func), get_inode_func)]
 
     requirements_update_suggestions = set()
     for file, suggests in inodes:
-        suggestions_reversed = list(reversed(suggests))
+        # python sort is stable, so items with same start mark, should stay in same order
+        suggestions_reversed = sorted(suggests, key=lambda x: -x.start_mark)
+        suggestions_requirements = \
+            [x for x in suggestions_reversed if x.suggestion_spec.get("action") == "FIX_REQUIREMENTS"]
+        suggestions_items = \
+            [x for x in suggestions_reversed if x.suggestion_spec.get("action") != "FIX_REQUIREMENTS"]
+
         with file.open("r", encoding="utf-8") as f:
             content = f.read()
 
         end_content = content
         try:
-            for suggestion in suggestions_reversed:
-                suggestion_dict = suggestion.suggestion
+            #  Requirements
+            for suggestion in suggestions_requirements:
+                suggestion_dict = suggestion.suggestion_spec
                 if suggestion_dict.get("action") == "FIX_REQUIREMENTS":
                     collection_name = suggestion_dict["data"]["collection_name"]
                     collection_version = suggestion_dict["data"]["version"]
                     # TODO: Update path when we are able to get it from scan input or scan result
                     requirements_yml_path = suggestion.file_parent / "requirements.yml"
                     requirements_update_suggestions.add((requirements_yml_path, collection_name, collection_version))
                     continue
 
-                update_result = _update_content(end_content, suggestion)
-                if update_result is None:
-                    continue
-                end_content, _ = update_result
+            # other
+            rewrite_result = RewriteProcessor.multi_execute(end_content, suggestions_items)
+            if rewrite_result is None:
+                continue
+            end_content = rewrite_result.content
         except Exception as e:  # pylint: disable=broad-except
-            print(f"Error when rewriting {f}: {e}")
+            print(f"Error when rewriting {file}: {e}")
 
         if end_content != content:
             with file.open("w", encoding="utf-8") as f:
                 f.write(end_content)
 
     # TODO: Consider updating this when we will be updating detection and rewriting of collection requirements
-    for requirements_yml_path, collection_name, collection_version in requirements_update_suggestions:
+    for (
+            requirements_yml_path,
+            collection_name,
+            collection_version,
+    ) in requirements_update_suggestions:
         with requirements_yml_path.open("a+", encoding="utf-8") as requirements_file:
             requirements_file.seek(0)
             try:
                 data = yaml.safe_load(requirements_file)
             except yaml.YAMLError:
                 # overwrite erroneous requirement file
                 data = None
```

## Comparing `steampunk_spotter-1.2.4rc1.dist-info/LICENSE` & `steampunk_spotter-1.2.5a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `steampunk_spotter-1.2.4rc1.dist-info/METADATA` & `steampunk_spotter-1.2.5a1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: steampunk-spotter
-Version: 1.2.4rc1
-Summary: Quality scanner for Ansible Playbooks
+Version: 1.2.5a1
+Summary: Ansible Playbook Scanning Tool
 Home-page: https://spotter.steampunk.si/
 Author: XLAB d.o.o.
 Author-email: pypi@xlab.si
 Project-URL: Source Code, https://gitlab.com/xlab-steampunk/steampunk-spotter-client/spotter-cli
 Project-URL: Bug Tracker, https://gitlab.com/xlab-steampunk/steampunk-spotter-client/spotter-cli/-/issues
 Project-URL: Documentation, https://gitlab.com/xlab-steampunk/steampunk-spotter-client/spotter-cli
 Keywords: ansible,automation,spotter,scanner,quality,playbook,steampunk
@@ -52,32 +52,34 @@
     - [Scanning](#scanning)
         - [Ansible content](#ansible-content)
         - [Selecting the target project](#selecting-the-target-project)
         - [Including values](#including-values)
         - [Including metadata](#including-metadata)
         - [Automated application of suggestions to your code](#automated-application-of-suggestions-to-your-code)
         - [Suppressing check result levels](#suppressing-check-result-levels)
+        - [Applying profiles](#applying-scan-profiles)
         - [Exporting and importing scan payload](#exporting-and-importing-scan-payload)
         - [Scan configuration](#scan-configuration)
         - [Formatting scan result](#formatting-scan-result)
         - [Omitting documentation URLs from the output](#omitting-documentation-urls-from-the-output)
+        - [Managing custom policies](#managing-custom-policies)
     - [Setting storage folder](#setting-storage-folder)
     - [Disabling colorized output](#disabling-colorized-output)
     - [Setting API endpoint](#setting-api-endpoint)
     - [CI/CD integrations](#cicd-integrations)
         - [GitLab](#gitlab)
         - [GitHub](#github)
         - [Others](#others)
 - [Development](#development)
     - [Running from source](#running-from-source)
     - [Building Docker image](#building-docker-image)
 - [Acknowledgement](#acknowledgement)
 
 ## Introduction
-[Steampunk Spotter] provides an Assisted Automation Writing tool that analyzes
+[Steampunk Spotter] provides an Ansible Playbook Scanning Tool that analyzes
 and offers recommendations for your Ansible Playbooks.
 
 The Steampunk Spotter CLI enables the use from the console with the ability
 to scan Ansible content such as playbooks, roles, collections, or task files.
 
 ## Installation
 `steampunk-spotter` requires Python 3 and is available as a
@@ -285,15 +287,15 @@
 $ spotter scan --include-values playbook.yaml
 ```
 
 #### Including metadata
 By default, CLI collects and uses metadata (file names, line and column
 numbers, YAML markers) from Ansible content just for displaying the scan
 output, which means that no data about your Ansible content structure is sent
-to the backend server. 
+to the backend server.
 For enriched user experience in the app and to get additional tips for
 improvements, you can use `--include-metadata` optional argument to send the
 metadata.
 
 ```shell
 $ spotter scan --include-metadata playbook.yaml
 ```
@@ -312,14 +314,38 @@
 levels.
 For example, to show only errors (suppress warnings and hints):
 
 ```shell
 $ spotter scan --display-level error playbook.yaml 
 ```
 
+#### Applying scan profiles
+When we run scans, we might have a particular goal in mind.
+For example, in one project we might be interested in upgrading our Ansible
+environment to a newer version of Ansible.
+In another one, we want to improve the playbooks for the Ansible version that
+we are currently in.
+This means that some check results that Steampunk Spotter produces may be
+relevant in one of the projects, but not in the other one.
+
+Using the `--profile` optional argument, we can specify a scan profile that
+contains a selected set of checks to be used for scanning. Spotter currently
+supports the following profiles:
+
+* `default` - this profile is suitable for day-to-day testing and improving
+  Ansible playbooks.
+* `full` - displays the full range of check results, which would be useful for
+  the Ansible playbook updating to work at a newer version of Ansible.
+
+For example, to run all checks (apply `full` profile):
+
+```shell
+$ spotter scan --profile full playbook.yaml 
+```
+
 #### Exporting and importing scan payload
 To see what data is collected from your Ansible content and sent to the
 backend server, you can use the optional `--export-payload` argument.
 
 ```shell
 $ spotter scan --export-payload payload.json playbook.yaml 
 Scan data saved to payload.json.
@@ -387,14 +413,50 @@
 To omit these documentation URLs from all the output, use `--no-docs-url`
 optional argument.
 
 ```console
 $ spotter scan --no-docs-url playbook.yaml
 ```
 
+#### Managing custom policies
+It is possible to create and use policies for custom Spotter checks written in
+Rego Language for Open Policy Agent (OPA).
+The use of custom policies is only available in Spotter's ENTERPRISE plan.
+
+Use `set-policies` command to set custom OPA policies.
+This will override all current policies.
+
+```shell
+# set one policy
+$ spotter set-policies policy.rego
+# set a whole dir with policies
+$ spotter set-policies policies/
+# set policy for a specific project
+$ spotter set-policies --project-id <project-id> policy.rego
+# set policy for whole organization
+$ spotter set-policies --organization-id <organization-id> policy.rego
+```
+
+After that run a scan to see check results you included.
+
+```shell
+$ spotter scan playbook.yaml
+```
+
+Use `clear-policies` command to clear custom policies.
+
+```shell
+# clear policies
+$ spotter clear-policies
+# clear policies for a specific project
+$ spotter clear-policies --project-id <project-id>
+# clear policies for whole organization
+$ spotter clear-policies --organization-id <organization-id>
+```
+
 ### Setting storage folder
 The CLI uses local storage for caching access tokens for the Steampunk
 Spotter API.
 The default location is `~/.config/steampunk-spotter`, but if you want to
 change it you can use `--storage-path` optional argument.
 
 ```console
```

## Comparing `steampunk_spotter-1.2.4rc1.dist-info/RECORD` & `steampunk_spotter-1.2.5a1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 spotter/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-spotter/api.py,sha256=kkX9XnlGGqMoUYmK5HluMCzEu80doU1KjiNKdZE0UmE,15218
-spotter/cli.py,sha256=EVSTfhSxG95iEE2xOApiytWWlOvCL1wYzxo3eirEUL0,4694
+spotter/api.py,sha256=MYiZufg2lt3jwErrlentER2PnVJim8w0kd_PrJHSr3o,17100
+spotter/cli.py,sha256=brRnJotwmFzDLnXFuAP7E0tTBG2ZEjz8e5YL-wtiNZs,5069
 spotter/environment.py,sha256=V8UehBSiH0pZThbYCpj7RYigoRDM8O201HhrMopYK14,18318
 spotter/parsing.py,sha256=2NnjOyQ8Khh19zc_ll7C7Gi5gw9Q5u8SK6F1UtxjFwg,24670
-spotter/rewriting.py,sha256=iIPHH50hN442Kah-NpE0oqkS1fbWSMzC0tM45oI_YxA,6839
 spotter/storage.py,sha256=IXUSXLz56BOABXVjehc887xOiCuIBGWZbD6DWLiDX9Y,5558
 spotter/utils.py,sha256=n6xPBZAHwhemTtFYivo0WFHxK01ir77SsrnooW6B75w,2752
-spotter/commands/__init__.py,sha256=CTut8qwGGmGz5sfcH_hXJL49UkFOhwlZa6fULxylp5U,94
+spotter/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+spotter/commands/clear_policies.py,sha256=UYp-xNrBTp4T--694Lw-jTaLI8uioG8teBm8IQivuAc,3952
 spotter/commands/login.py,sha256=lOEU1IPLdSWxFLxnTsRbhCrxkTNdadwcintmLDn7b4g,2347
 spotter/commands/register.py,sha256=BstH64-72XM-1-xAZgrn__b55qpLAFnajF8UfrOmxU8,1141
-spotter/commands/scan.py,sha256=8bVr7aplA5_Z-oWfvw9nbNyouVoggqMkaTp6Q6N49zE,38545
+spotter/commands/scan.py,sha256=H8FdAx6EYCliKhDPpJPBiNKrvFW9ik2hKn3kerK-o8k,38655
+spotter/commands/set_policies.py,sha256=-zkzrT9cso3J7eg9tezCDk5s2jgSP79mBC1l2ouIi9Y,5209
 spotter/commands/suggest.py,sha256=WAt60BGyxfMZOaWgpdprijzViyUE9DLhx9GaPs-6zWM,3620
 spotter/reporting/__init__.py,sha256=Mddj7lJk3d9SeIpItBD_NNURRF4vtyMahTomdOFAEDw,60
 spotter/reporting/report.py,sha256=LXBXWhXvWa39l-UvLq0-5ts0dK_uCRCfayvUGm0g5kQ,3459
-steampunk_spotter-1.2.4rc1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-steampunk_spotter-1.2.4rc1.dist-info/METADATA,sha256=4ZvYgc0_nriei6HIiZ2VW5iuARXLe1goLNCU5yp5p_s,19428
-steampunk_spotter-1.2.4rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-steampunk_spotter-1.2.4rc1.dist-info/entry_points.txt,sha256=_94aMdgSgx7FY17kO5nvQ5NaEqYQM1oetU0Iwq2NK6c,45
-steampunk_spotter-1.2.4rc1.dist-info/top_level.txt,sha256=3FpgMM0g2fECUU_GuaBTKGXYeWTG5uDxJXqqRD3YTck,8
-steampunk_spotter-1.2.4rc1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-steampunk_spotter-1.2.4rc1.dist-info/RECORD,,
+spotter/rewriting/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+spotter/rewriting/models.py,sha256=RCPpJ8j4Hig2RYpC_pEYKnOlRBOuPmyddBucX9RM8z4,7545
+spotter/rewriting/processor.py,sha256=Z0juLwyUGAwovuXc4xNb4tY6RUZXTuM_yIcxTKpFrkM,7055
+spotter/rewriting/rewrite_action_inline.py,sha256=pmu0onrt4DPDwhmVh_DlD7ceCg_rTyjz1lLOjQfZOa4,1937
+spotter/rewriting/rewrite_action_object.py,sha256=VHgHR2zlscJnLJjnPj_DM_xdJhpYKSqJR62tkHmxlTo,2318
+spotter/rewriting/rewrite_always_run.py,sha256=UxH-gjRr8rEGaXzT9dp4bOaFXXMaCE7vFc2jO_7B3Fw,989
+spotter/rewriting/rewrite_fqcn.py,sha256=bHjFL68p5Kx-aRBmsvlUPu4fsDbVcsDdaw0v61IvDC0,982
+spotter/rewriting/rewrite_inline.py,sha256=AWwOpqYTtokaLN65bCpPWbPqHOwYkh4b-B5NwP9quBc,2087
+spotter/rewriting/rewrite_local_action_inline.py,sha256=TTv4rF8EPSapapDShP9-Tk0ZOPHXXjiW7LluVShrYqU,2527
+spotter/rewriting/rewrite_local_object.py,sha256=oEdZsSmMf7AS9jXbUxmmYoePId2c48yJQ8pqvQsBOrE,2312
+spotter/rewriting/rewrite_module_inline.py,sha256=blQEkNzfCAiyr2nJJuTNXdj8jyVAESLzfA4cfhttRto,989
+spotter/rewriting/rewrite_module_object.py,sha256=tK5KNRCIn0ibwXwmwgAk8nKKIyOCADmsYOPsX3lcWiY,888
+steampunk_spotter-1.2.5a1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+steampunk_spotter-1.2.5a1.dist-info/METADATA,sha256=BmJIDfg46bKfT8gGiNzmHi-juODaG6EkG-lSRb32zKA,21591
+steampunk_spotter-1.2.5a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+steampunk_spotter-1.2.5a1.dist-info/entry_points.txt,sha256=_94aMdgSgx7FY17kO5nvQ5NaEqYQM1oetU0Iwq2NK6c,45
+steampunk_spotter-1.2.5a1.dist-info/top_level.txt,sha256=3FpgMM0g2fECUU_GuaBTKGXYeWTG5uDxJXqqRD3YTck,8
+steampunk_spotter-1.2.5a1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+steampunk_spotter-1.2.5a1.dist-info/RECORD,,
```

