# Comparing `tmp/mosaicml_cli-0.3.5-py3-none-any.whl.zip` & `tmp/mosaicml_cli-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,46 +1,46 @@
-Zip file size: 289570 bytes, number of entries: 208
+Zip file size: 288577 bytes, number of entries: 208
 -rw-r--r--  2.0 unx       54 b- defN 22-Jun-27 19:47 mcli/__init__.py
 -rw-r--r--  2.0 unx    16462 b- defN 23-Apr-11 21:00 mcli/config.py
--rw-r--r--  2.0 unx     3884 b- defN 23-Apr-11 22:06 mcli/version.py
+-rw-r--r--  2.0 unx     3884 b- defN 23-Apr-11 22:32 mcli/version.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/api/__init__.py
 -rw-r--r--  2.0 unx    11677 b- defN 23-Apr-11 21:00 mcli/api/exceptions.py
 -rw-r--r--  2.0 unx      508 b- defN 23-Feb-02 19:35 mcli/api/types.py
 -rw-r--r--  2.0 unx     2354 b- defN 22-Jun-27 19:47 mcli/api/typing_future.py
 -rw-r--r--  2.0 unx      134 b- defN 22-Oct-27 18:49 mcli/api/cluster/__init__.py
 -rw-r--r--  2.0 unx     4058 b- defN 23-Apr-11 21:00 mcli/api/cluster/api_get_clusters.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/api/engine/__init__.py
--rw-r--r--  2.0 unx    26222 b- defN 23-Apr-11 22:06 mcli/api/engine/engine.py
+-rw-r--r--  2.0 unx    22935 b- defN 23-Apr-11 22:31 mcli/api/engine/engine.py
 -rw-r--r--  2.0 unx      787 b- defN 22-Sep-15 00:48 mcli/api/engine/utils.py
 -rw-r--r--  2.0 unx      879 b- defN 23-Apr-11 22:06 mcli/api/inference_deployments/__init__.py
 -rw-r--r--  2.0 unx     3388 b- defN 23-Apr-11 21:00 mcli/api/inference_deployments/api_create_inference_deployment.py
 -rw-r--r--  2.0 unx     3278 b- defN 23-Apr-11 21:00 mcli/api/inference_deployments/api_delete_inference_deployments.py
 -rw-r--r--  2.0 unx     6091 b- defN 23-Apr-11 21:00 mcli/api/inference_deployments/api_get_inference_deployments.py
 -rw-r--r--  2.0 unx     1156 b- defN 23-Apr-11 21:00 mcli/api/inference_deployments/api_ping_inference_deployment.py
 -rw-r--r--  2.0 unx     1276 b- defN 23-Apr-11 21:00 mcli/api/inference_deployments/api_predict_inference_deployment.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Aug-17 23:59 mcli/api/kube/__init__.py
 -rw-r--r--  2.0 unx      856 b- defN 22-Aug-17 23:59 mcli/api/kube/runs/__init__.py
 -rw-r--r--  2.0 unx     4900 b- defN 23-Apr-11 21:00 mcli/api/kube/runs/api_create_run.py
 -rw-r--r--  2.0 unx     5042 b- defN 23-Mar-06 23:35 mcli/api/kube/runs/api_delete_runs.py
 -rw-r--r--  2.0 unx    14458 b- defN 23-Mar-06 23:35 mcli/api/kube/runs/api_get_run_logs.py
--rw-r--r--  2.0 unx    16137 b- defN 23-Apr-11 22:06 mcli/api/kube/runs/api_get_runs.py
+-rw-r--r--  2.0 unx    16142 b- defN 23-Apr-11 22:31 mcli/api/kube/runs/api_get_runs.py
 -rw-r--r--  2.0 unx     6007 b- defN 23-Mar-06 23:35 mcli/api/kube/runs/api_stop_runs.py
 -rw-r--r--  2.0 unx     6210 b- defN 22-Oct-27 18:49 mcli/api/kube/runs/api_watch_run.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-06 23:35 mcli/api/mint/__init__.py
 -rw-r--r--  2.0 unx     4987 b- defN 23-Mar-06 23:35 mcli/api/mint/shell.py
 -rw-r--r--  2.0 unx     1530 b- defN 23-Mar-06 23:35 mcli/api/mint/tty.py
 -rw-r--r--  2.0 unx      209 b- defN 23-Apr-11 21:00 mcli/api/model/__init__.py
 -rw-r--r--  2.0 unx     5655 b- defN 23-Apr-11 21:00 mcli/api/model/cluster_details.py
 -rw-r--r--  2.0 unx     3015 b- defN 23-Apr-11 21:00 mcli/api/model/inference_deployment.py
 -rw-r--r--  2.0 unx     7946 b- defN 23-Apr-11 22:06 mcli/api/model/run.py
 -rw-r--r--  2.0 unx     1102 b- defN 23-Apr-11 22:06 mcli/api/runs/__init__.py
 -rw-r--r--  2.0 unx     2726 b- defN 23-Apr-11 22:06 mcli/api/runs/api_create_run.py
 -rw-r--r--  2.0 unx     3926 b- defN 23-Apr-11 22:06 mcli/api/runs/api_delete_runs.py
 -rw-r--r--  2.0 unx     9281 b- defN 23-Apr-11 21:00 mcli/api/runs/api_get_run_logs.py
--rw-r--r--  2.0 unx    10400 b- defN 23-Apr-11 22:06 mcli/api/runs/api_get_runs.py
+-rw-r--r--  2.0 unx     8968 b- defN 23-Apr-11 22:31 mcli/api/runs/api_get_runs.py
 -rw-r--r--  2.0 unx     5099 b- defN 23-Apr-11 22:06 mcli/api/runs/api_stop_runs.py
 -rw-r--r--  2.0 unx     3937 b- defN 23-Apr-11 22:06 mcli/api/runs/api_update_run_metadata.py
 -rw-r--r--  2.0 unx    10619 b- defN 23-Apr-11 21:00 mcli/api/runs/api_watch_run.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/api/schema/__init__.py
 -rw-r--r--  2.0 unx      636 b- defN 22-Aug-23 17:34 mcli/api/schema/generic_model.py
 -rw-r--r--  2.0 unx      309 b- defN 22-Sep-22 23:36 mcli/api/secrets/__init__.py
 -rw-r--r--  2.0 unx     2365 b- defN 23-Mar-06 23:35 mcli/api/secrets/api_create_secret.py
@@ -48,15 +48,15 @@
 -rw-r--r--  2.0 unx     3697 b- defN 23-Apr-11 21:00 mcli/api/secrets/api_get_secrets.py
 -rw-r--r--  2.0 unx      139 b- defN 23-Feb-02 20:09 mcli/api/users/__init__.py
 -rw-r--r--  2.0 unx     2694 b- defN 23-Mar-06 23:35 mcli/api/users/api_get_users.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/__init__.py
 -rw-r--r--  2.0 unx     7182 b- defN 23-Apr-11 21:00 mcli/cli/cli.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-02 19:35 mcli/cli/common/__init__.py
 -rw-r--r--  2.0 unx     2670 b- defN 23-Apr-11 21:00 mcli/cli/common/deployment_filters.py
--rw-r--r--  2.0 unx     7238 b- defN 23-Apr-11 22:06 mcli/cli/common/run_filters.py
+-rw-r--r--  2.0 unx     7180 b- defN 23-Apr-11 22:31 mcli/cli/common/run_filters.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/m_clean/__init__.py
 -rw-r--r--  2.0 unx      950 b- defN 22-Oct-27 18:49 mcli/cli/m_clean/m_clean.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-06 23:35 mcli/cli/m_connect/__init__.py
 -rw-r--r--  2.0 unx     1541 b- defN 23-Mar-06 23:35 mcli/cli/m_connect/m_connect.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/m_create/__init__.py
 -rw-r--r--  2.0 unx    11513 b- defN 22-Oct-27 18:49 mcli/cli/m_create/cluster.py
 -rw-r--r--  2.0 unx     7167 b- defN 23-Apr-11 21:00 mcli/cli/m_create/env_var.py
@@ -73,15 +73,15 @@
 -rw-r--r--  2.0 unx     1860 b- defN 23-Apr-11 21:00 mcli/cli/m_describe/m_describe.py
 -rw-r--r--  2.0 unx      549 b- defN 23-Apr-11 21:00 mcli/cli/m_get/__init__.py
 -rw-r--r--  2.0 unx     3909 b- defN 23-Apr-11 21:00 mcli/cli/m_get/clusters.py
 -rw-r--r--  2.0 unx     6452 b- defN 23-Apr-11 21:00 mcli/cli/m_get/display.py
 -rw-r--r--  2.0 unx     1315 b- defN 22-Sep-15 00:48 mcli/cli/m_get/envvars.py
 -rw-r--r--  2.0 unx     5361 b- defN 23-Apr-11 21:00 mcli/cli/m_get/inference_deployments.py
 -rw-r--r--  2.0 unx     4866 b- defN 23-Apr-11 21:00 mcli/cli/m_get/m_get.py
--rw-r--r--  2.0 unx     7104 b- defN 23-Apr-11 22:06 mcli/cli/m_get/runs.py
+-rw-r--r--  2.0 unx     6346 b- defN 23-Apr-11 22:31 mcli/cli/m_get/runs.py
 -rw-r--r--  2.0 unx     3567 b- defN 23-Apr-11 21:00 mcli/cli/m_get/secrets.py
 -rw-r--r--  2.0 unx     1580 b- defN 23-Feb-02 20:09 mcli/cli/m_get/users.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/m_init/__init__.py
 -rw-r--r--  2.0 unx     4113 b- defN 23-Apr-11 21:00 mcli/cli/m_init/m_init.py
 -rw-r--r--  2.0 unx     9374 b- defN 23-Apr-11 21:00 mcli/cli/m_init/m_init_kube.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-27 19:47 mcli/cli/m_interactive/__init__.py
 -rw-r--r--  2.0 unx     9005 b- defN 23-Mar-06 23:35 mcli/cli/m_interactive/interactive.py
@@ -198,13 +198,13 @@
 -rw-r--r--  2.0 unx     3115 b- defN 22-Aug-31 05:37 mcli/utils/utils_rich.py
 -rw-r--r--  2.0 unx     8533 b- defN 23-Mar-03 22:02 mcli/utils/utils_run_status.py
 -rw-r--r--  2.0 unx     4350 b- defN 22-Jun-27 19:47 mcli/utils/utils_serializable_dataclass.py
 -rw-r--r--  2.0 unx     1103 b- defN 23-Apr-11 21:00 mcli/utils/utils_spinner.py
 -rw-r--r--  2.0 unx    11437 b- defN 23-Mar-06 23:35 mcli/utils/utils_string_functions.py
 -rw-r--r--  2.0 unx     3954 b- defN 22-Nov-04 18:29 mcli/utils/utils_types.py
 -rw-r--r--  2.0 unx     1001 b- defN 22-Jun-27 19:47 mcli/utils/utils_yaml.py
--rw-r--r--  2.0 unx     4743 b- defN 23-Apr-11 22:08 mosaicml_cli-0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 22:08 mosaicml_cli-0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       75 b- defN 23-Apr-11 22:08 mosaicml_cli-0.3.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-11 22:08 mosaicml_cli-0.3.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    18463 b- defN 23-Apr-11 22:08 mosaicml_cli-0.3.5.dist-info/RECORD
-208 files, 877921 bytes uncompressed, 260212 bytes compressed:  70.4%
+-rw-r--r--  2.0 unx     4743 b- defN 23-Apr-11 22:32 mosaicml_cli-0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 22:32 mosaicml_cli-0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       75 b- defN 23-Apr-11 22:32 mosaicml_cli-0.3.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-11 22:32 mosaicml_cli-0.3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    18462 b- defN 23-Apr-11 22:32 mosaicml_cli-0.3.6.dist-info/RECORD
+208 files, 872390 bytes uncompressed, 259219 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -603,23 +603,23 @@
 
 Filename: mcli/utils/utils_types.py
 Comment: 
 
 Filename: mcli/utils/utils_yaml.py
 Comment: 
 
-Filename: mosaicml_cli-0.3.5.dist-info/METADATA
+Filename: mosaicml_cli-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: mosaicml_cli-0.3.5.dist-info/WHEEL
+Filename: mosaicml_cli-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: mosaicml_cli-0.3.5.dist-info/entry_points.txt
+Filename: mosaicml_cli-0.3.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: mosaicml_cli-0.3.5.dist-info/top_level.txt
+Filename: mosaicml_cli-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: mosaicml_cli-0.3.5.dist-info/RECORD
+Filename: mosaicml_cli-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mcli/version.py

```diff
@@ -111,13 +111,13 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

## mcli/api/engine/engine.py

```diff
@@ -431,79 +431,14 @@
         model_type=return_model_type,
     )
     future = cast('Future[List[ModelT]]', future)
 
     return future
 
 
-# TODO: Refactor this when we have more paginated endpoints
-def run_paginated_mapi_request(
-    query: str,
-    query_function: str,
-    return_model_type: Optional[Type[ModelT]] = None,
-    variables: Optional[Dict[str, Any]] = None,
-    connection: Optional[MAPIConnection] = None,
-) -> Future[List[ModelT]]:
-    """Run a GraphQL query against a paginated MAPI endpoint and return a future for a list of items
-
-    Args:
-        query: Query to run
-        query_function: GraphQL endpoint for the query (e.g. 'createRun')
-        return_model_type: The data type into which the response should be deserialized.
-            Required if data is expected to be returned.
-        variables: Variables to be passed to the GraphQL endpoint. Defaults to None.
-        connection: The MAPI connection that should be used. Defaults to the connection
-            returned by `MAPIConnection.get_current_connection()`.
-
-    Returns:
-        A `concurrent.futures.Future` for the request. You can retrieve the data using
-        `future.result()` with an optional `timeout` argument.
-
-    Raises:
-        MAPIException: Raised if the request fails. See ``MAPIException`` for details on
-        exception status codes
-    """
-    if not connection:
-        connection = MAPIConnection.get_current_connection()
-
-    future = connection.pool.submit(
-        _threaded_paginated_mapi_request,
-        api_key=connection.api_key,
-        endpoint=connection.endpoint,
-        query=query,
-        variables=variables,
-        query_function=query_function,
-        model_type=return_model_type,
-    )
-    future = cast('Future[List[ModelT]]', future)
-
-    return future
-
-
-def _threaded_paginated_mapi_request(
-    api_key: str,
-    endpoint: str,
-    query: str,
-    variables: Optional[Dict[str, Any]],
-    query_function: str,
-    model_type: Optional[Type[ModelT]],
-) -> List[ModelT]:
-    """Run a graphql request in a thread and return a list of items
-    """
-    if not api_key:
-        raise MCLIConfigError(MESSAGE.API_KEY_MISSING)
-    try:
-        response = _run_graphql_request(api_key, endpoint, query, variables)
-    except requests.exceptions.ConnectionError as e:
-        mapi_error = MAPIException.from_requests_error(e)
-        raise mapi_error from e
-
-    return _deserialize_response(response, query_function, model_type, paginated=True)
-
-
 def _threaded_plural_mapi_request(
     api_key: str,
     endpoint: str,
     query: str,
     variables: Optional[Dict[str, Any]],
     query_function: str,
     model_type: Optional[Type[ModelT]],
@@ -682,15 +617,14 @@
         raise mapi_error from e
 
 
 def _deserialize_response(
     response: Dict[str, Any],
     query_function: str,
     model_type: Optional[Type[ModelT]],
-    paginated: bool = False,
 ) -> List[ModelT]:
     """Given response, function, and model object, deserializes data
 
     raises
         MAPIException: Something on the MAPI side went wrong (400s) or the
             response didn't match the expected format (500)
         MultiMAPIException: Multiple errors encountered in graphql
@@ -703,33 +637,14 @@
 
     if model_type is None:
         return []
 
     try:
         data = response['data']
         query_response: List[Any] = data[query_function]
-
-        if paginated:
-            # Paginated results should have the following return type:
-            #   type <Model>Page {
-            #       <Model>s: [<Model>!]
-            #       cursor: String
-            #       hasNextPage: Boolean
-            #    }
-            # This is flexible to support not having to provide a name of the
-            # model, or explicitly neededing to select the pagination fields
-            if not isinstance(query_response, dict):
-                raise ValueError('Expected paginated response to be a dict')
-            keys = set(query_response.keys()) - {'cursor', 'hasNextPage'}
-            # However, if there's more than one key, we don't know which one
-            # to use, so we raise an error
-            if len(keys) > 1:
-                raise ValueError('Expected only one key in paginated response')
-            query_response = query_response[list(keys)[0]]
-
         return [model_type.from_mapi_response(i) for i in query_response]
     except (KeyError, TypeError) as e:
         raise MAPIException(status=HTTPStatus.INTERNAL_SERVER_ERROR,
                             message='Internal Server Error: Malformed response data') from e
 
 
 def get_return_response(response, future: bool = False, timeout: Optional[float] = 10.0):
```

## mcli/api/kube/runs/api_get_runs.py

```diff
@@ -304,15 +304,14 @@
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     user_emails: Optional[List[str]] = None,
-    limit: Optional[int] = None,
 ) -> List[Run]:
     ...
 
 
 @overload
 def get_runs(
     runs: Optional[Union[List[str], List[Run]]] = None,
@@ -322,15 +321,14 @@
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     user_emails: Optional[List[str]] = None,
-    limit: Optional[int] = None,
 ) -> Future[List[Run]]:
     ...
 
 
 def get_runs(
     runs: Optional[Union[List[str], List[Run]]] = None,
     cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
@@ -339,15 +337,14 @@
     gpu_types: Optional[Union[List[str], List[GPUType]]] = None,
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = 10,
     future: bool = False,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     user_emails: Optional[List[str]] = None,
-    limit: Optional[int] = None,
 ):
     """Get a filtered list of runs
 
     List runs that have been launched in the MosaicML platform. The returned list will
     contain all of the details stored about the requested runs.
 
     Arguments:
@@ -385,16 +382,16 @@
 
     Returns:
         If future is False:
             A list of requested :class:`~mcli.api.model.run.Run` objects
         Otherwise:
             A :class:`~concurrent.futures.Future` for the list
     """
-    if before or after or user_emails or limit is not None:
-        raise NotImplementedError('This filter is not suported in legacy mcli')
+    if before or after:
+        raise NotImplementedError('Before and after run filters not supported in legacy mcli')
 
     # Coerce arg types to strings
     run_names: Optional[List[str]] = None
     if runs is not None:
         run_names = [r.name if isinstance(r, Run) else r for r in runs]
 
     cluster_names = cluster_names or clusters
@@ -407,13 +404,16 @@
 
     if gpu_types is not None:
         gpu_types = [gt.name if isinstance(gt, GPUType) else gt for gt in gpu_types]
 
     if statuses is not None:
         statuses = [st.name if isinstance(st, RunStatus) else st for st in statuses]
 
+    if user_emails is not None:
+        raise NotImplementedError("Getting runs of another user is only supported in mapi")
+
     runs_future = _get_runs_kube(run_names, cluster_names, gpu_types, gpu_nums, statuses)
 
     if not future:
         return runs_future.result(timeout=timeout)
     else:
         return runs_future
```

## mcli/api/runs/api_get_runs.py

```diff
@@ -4,15 +4,15 @@
 from concurrent.futures import Future
 from datetime import datetime
 from http import HTTPStatus
 from typing import List, Optional, Union, overload
 
 from typing_extensions import Literal
 
-from mcli.api.engine.engine import get_return_response, run_paginated_mapi_request, run_plural_mapi_request
+from mcli.api.engine.engine import get_return_response, run_plural_mapi_request
 from mcli.api.exceptions import MAPIException
 from mcli.api.model.run import Run
 from mcli.config import MCLIConfig
 from mcli.models.mcli_cluster import Cluster
 from mcli.serverside.clusters.gpu_type import GPUType
 from mcli.utils.utils_run_status import RunStatus
 
@@ -56,33 +56,14 @@
     details {{
         originalRunInput
         metadata
     }}
   }}
 }}
 """
-QUERY_FUNCTION_PAGINATED = 'getRunsPaginated'
-VARIABLE_DATA_NAME_PAGINATED = 'getRunsPaginatedData'
-QUERY_PAGINATED = f"""
-query GetRunsPaginated(${VARIABLE_DATA_NAME_PAGINATED}: GetRunsPaginatedInput!) {{
-  {QUERY_FUNCTION_PAGINATED}({VARIABLE_DATA_NAME_PAGINATED}: ${VARIABLE_DATA_NAME_PAGINATED}) {{
-  runs {{
-    id
-    name
-    status
-    createdAt
-    startedAt
-    completedAt
-    updatedAt
-    reason
-    runInput
-    createdByEmail
-  }}
-  }}
-}}"""
 
 
 @overload
 def get_run(
     run: Union[str, Run],
     *,
     timeout: Optional[float] = 10,
@@ -145,15 +126,14 @@
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = 10,
     future: Literal[False] = False,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     user_emails: Optional[List[str]] = None,
     include_details: bool = False,
-    limit: Optional[int] = None,
 ) -> List[Run]:
     ...
 
 
 @overload
 def get_runs(
     runs: Optional[Union[List[str], List[Run]]] = None,
@@ -164,15 +144,14 @@
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = None,
     future: Literal[True] = True,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,
     user_emails: Optional[List[str]] = None,
     include_details: bool = False,
-    limit: Optional[int] = None,
 ) -> Future[List[Run]]:
     ...
 
 
 def get_runs(
     runs: Optional[Union[List[str], List[Run]]] = None,
     cluster_names: Optional[Union[List[str], List[Cluster]]] = None,
@@ -182,15 +161,14 @@
     gpu_nums: Optional[List[int]] = None,
     statuses: Optional[Union[List[str], List[RunStatus]]] = None,
     timeout: Optional[float] = 10,
     future: bool = False,
     clusters: Optional[Union[List[str], List[Cluster]]] = None,  # TODO: deprecate
     user_emails: Optional[List[str]] = None,
     include_details: bool = False,
-    limit: Optional[int] = None,
 ):
     """List runs that have been launched in the MosaicML platform
 
     The returned list will contain all of the details stored about the requested runs.
 
     Arguments:
         runs: List of runs on which to get information
@@ -214,24 +192,18 @@
             value will be ignored.
         future: Return the output as a :type concurrent.futures.Future:. If True, the
             call to `get_runs` will return immediately and the request will be
             processed in the background. This takes precedence over the ``timeout``
             argument. To get the list of runs, use ``return_value.result()``
             with an optional ``timeout`` argument.
         include_details: If true, will fetch detailed information like run input for each run.
-        limit: Maximum number of runs to return. If None, all runs will be returned.
 
     Raises:
         MAPIException: If connecting to MAPI, raised when a MAPI communication error occurs
     """
-    # We could support run details in pagination, but it goes against the point of the paginated view:
-    # This is a view that is meant to be used for listing runs, not for fetching detailed information
-    if limit and include_details:
-        raise MAPIException(HTTPStatus.BAD_REQUEST, "Cannot use limit and include_details together")
-
     filters = {}
     if runs:
         filters['name'] = {'in': [r.name if isinstance(r, Run) else r for r in runs]}
     if before or after:
         date_filters = {}
         if before:
             date_filters['lt'] = before.astimezone().isoformat() if isinstance(before, datetime) else before
@@ -245,42 +217,31 @@
     if cluster_names:
         filters['clusterName'] = {'in': [c.name if isinstance(c, Cluster) else c for c in cluster_names]}
     if gpu_types:
         filters['gpuType'] = {'in': [gt.value if isinstance(gt, GPUType) else gt for gt in gpu_types]}
     if gpu_nums:
         filters['gpuNum'] = {'in': gpu_nums}
 
-    variable_name = VARIABLE_DATA_NAME if limit is None else VARIABLE_DATA_NAME_PAGINATED
     variables = {
-        variable_name: {
+        VARIABLE_DATA_NAME: {
             'filters': filters,
             'includeDeleted': False,
         },
     }
 
     cfg = MCLIConfig.load_config(safe=True)
     if cfg.user_id:
-        variables[variable_name]['entity'] = {'userIds': [cfg.user_id]}
+        variables[VARIABLE_DATA_NAME]['entity'] = {'userIds': [cfg.user_id]}
     if user_emails:
-        if variables[variable_name].get('entity'):
-            variables[variable_name]['entity']['emails'] = user_emails
+        if variables[VARIABLE_DATA_NAME].get('entity'):
+            variables[VARIABLE_DATA_NAME]['entity']['emails'] = user_emails
         else:
-            variables[variable_name]['entity'] = {'emails': user_emails}
+            variables[VARIABLE_DATA_NAME]['entity'] = {'emails': user_emails}
 
-    if limit is None:
-        response = run_plural_mapi_request(
-            query=QUERY if not include_details else QUERY_WITH_DETAILS,
-            query_function=QUERY_FUNCTION,
-            return_model_type=Run,
-            variables=variables,
-        )
-    else:
-        # use paginated getRuns query
-        variables[variable_name]['limit'] = limit
-        response = run_paginated_mapi_request(
-            query=QUERY_PAGINATED,
-            query_function=QUERY_FUNCTION_PAGINATED,
-            return_model_type=Run,
-            variables=variables,
-        )
+    response = run_plural_mapi_request(
+        query=QUERY if not include_details else QUERY_WITH_DETAILS,
+        query_function=QUERY_FUNCTION,
+        return_model_type=Run,
+        variables=variables,
+    )
 
     return get_return_response(response, future=future, timeout=timeout)
```

## mcli/cli/common/run_filters.py

```diff
@@ -144,15 +144,14 @@
     after_filter: Optional[str] = None,
     gpu_type_filter: Optional[List[str]] = None,
     gpu_num_filter: Optional[List[int]] = None,
     status_filter: Optional[List[RunStatus]] = None,
     latest: bool = False,
     action_all: Optional[bool] = None,
     user_filter: Optional[List[str]] = None,
-    limit: Optional[int] = None,
 ) -> List[Run]:
 
     filter_used = any([
         name_filter,
         before_filter,
         after_filter,
         cluster_filter,
@@ -184,15 +183,14 @@
             user_emails=user_filter,
             before=before_filter,
             after=after_filter,
             gpu_types=gpu_type_filter,
             gpu_nums=gpu_num_filter,
             statuses=status_filter,
             timeout=None,
-            limit=limit,
         )
 
     if glob_filters:
         found_runs: Dict[str, Run] = {r.name: r for r in runs}
 
         # Any globs will be handled by additional client-side filtering
         filtered = set()
```

## mcli/cli/m_get/runs.py

```diff
@@ -9,19 +9,16 @@
 
 from mcli import config
 from mcli.api.exceptions import cli_error_handler
 from mcli.cli.common.run_filters import configure_submission_filter_argparser, get_runs_with_filters
 from mcli.cli.m_get.display import MCLIDisplayItem, MCLIGetDisplay, OutputDisplay, format_timestamp
 from mcli.sdk import Run
 from mcli.utils.utils_cli import comma_separated
-from mcli.utils.utils_logging import WARN
 from mcli.utils.utils_run_status import RunStatus
 
-DEFAULT_DISPLAY_LIMIT = 50
-
 logger = logging.getLogger(__name__)
 
 
 class RunColumns(Enum):
     ID = 'id'
     NAME = 'name'
     CLUSTER = 'cluster'
@@ -106,15 +103,14 @@
     gpu_type_filter: Optional[List[str]] = None,
     gpu_num_filter: Optional[List[int]] = None,
     status_filter: Optional[List[RunStatus]] = None,
     output: OutputDisplay = OutputDisplay.TABLE,
     include_ids: bool = False,
     latest: bool = False,
     user_filter: Optional[List[str]] = None,
-    limit: Optional[int] = DEFAULT_DISPLAY_LIMIT,
     **kwargs,
 ) -> int:
     """Get a table of ongoing and completed runs
     """
     del kwargs
 
     runs = get_runs_with_filters(
@@ -123,23 +119,19 @@
         before_filter=before_filter,
         after_filter=after_filter,
         gpu_type_filter=gpu_type_filter,
         gpu_num_filter=gpu_num_filter,
         status_filter=status_filter,
         latest=latest,
         user_filter=user_filter,
-        limit=limit,
     )
 
     display = MCLIRunDisplay(runs, include_ids=include_ids)
     display.print(output)
 
-    if len(runs) == DEFAULT_DISPLAY_LIMIT:
-        logger.warning(f'{WARN} Run view shows only the last {DEFAULT_DISPLAY_LIMIT} runs and may be truncated. '
-                       'Use --limit to increase the number of runs displayed.')
     return 0
 
 
 def get_runs_argparser(subparsers: argparse._SubParsersAction):
     """Configures the ``mcli get runs`` argparser
     """
 
@@ -180,22 +172,8 @@
         default=None,
         metavar='User',
         type=user,
         help='Fetch the runs created by a user in your organization with their email address. '
         'Multiple users should be specified using a comma-separated list, '
         'e.g. "alice@gmail.com,bob@gmail.com"',
     )
-
-    def limit(value: str) -> Optional[int]:
-        if value.lower() == 'none':
-            return None
-
-        return int(value)
-
-    runs_parser.add_argument(
-        '--limit',
-        help='Maximum number of runs to return. Runs will be sorted by creation time. '
-        f'Default: {DEFAULT_DISPLAY_LIMIT}',
-        default=DEFAULT_DISPLAY_LIMIT,
-        type=limit,
-    )
     return runs_parser
```

## Comparing `mosaicml_cli-0.3.5.dist-info/METADATA` & `mosaicml_cli-0.3.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.3.5
+Version: 0.3.6
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,43 +27,43 @@
 Requires-Dist: yaspin (>=2.1.0)
 Requires-Dist: jinja2
 Requires-Dist: arrow (>=1.2.2)
 Requires-Dist: slack-sdk (>=3.17.1)
 Requires-Dist: docker (>=5.0.3)
 Requires-Dist: gql[websockets] (>=3.4.0)
 Provides-Extra: all
-Requires-Dist: pyright (>=1.1.256) ; extra == 'all'
-Requires-Dist: sphinxcontrib-katex (>=0.8.6) ; extra == 'all'
+Requires-Dist: sphinxcontrib-serializinghtml (>=1.1.5) ; extra == 'all'
+Requires-Dist: sphinxcontrib-images (>=0.9.4) ; extra == 'all'
+Requires-Dist: pytest-mock (>=3.7.0) ; extra == 'all'
+Requires-Dist: sphinx-panels (>=0.6.0) ; extra == 'all'
 Requires-Dist: sphinxcontrib-htmlhelp (>=2.0.0) ; extra == 'all'
-Requires-Dist: yapf (>=0.32.0) ; extra == 'all'
-Requires-Dist: sphinx-markdown-tables (>=0.0.15) ; extra == 'all'
-Requires-Dist: sphinx-external-toc (>=0.3.0) ; extra == 'all'
-Requires-Dist: sphinxcontrib-jsmath (>=1.0.1) ; extra == 'all'
-Requires-Dist: sphinx-copybutton (>=0.5.0) ; extra == 'all'
-Requires-Dist: sphinx-rtd-theme (>=1.0.0) ; extra == 'all'
+Requires-Dist: myst-parser (>=0.16.1) ; extra == 'all'
 Requires-Dist: pylint (>=2.12.2) ; extra == 'all'
-Requires-Dist: sphinx (>=4.4.0) ; extra == 'all'
-Requires-Dist: sphinxext-opengraph (>=0.6.1) ; extra == 'all'
-Requires-Dist: radon (>=5.1.0) ; extra == 'all'
-Requires-Dist: pytest-cov (>=4.0.0) ; extra == 'all'
 Requires-Dist: furo (>=2022.3.4) ; extra == 'all'
 Requires-Dist: pre-commit (>=2.17.0) ; extra == 'all'
-Requires-Dist: sphinx-design ; extra == 'all'
-Requires-Dist: sphinx-argparse (>=0.3.1) ; extra == 'all'
-Requires-Dist: sphinxcontrib-images (>=0.9.4) ; extra == 'all'
-Requires-Dist: sphinx-panels (>=0.6.0) ; extra == 'all'
-Requires-Dist: pytest-mock (>=3.7.0) ; extra == 'all'
+Requires-Dist: pytest (>=6.2.5) ; extra == 'all'
+Requires-Dist: sphinxcontrib-katex (>=0.8.6) ; extra == 'all'
+Requires-Dist: isort (>=5.9.3) ; extra == 'all'
 Requires-Dist: sphinxemoji (>=0.2.0) ; extra == 'all'
+Requires-Dist: sphinx-rtd-theme (>=1.0.0) ; extra == 'all'
+Requires-Dist: radon (>=5.1.0) ; extra == 'all'
+Requires-Dist: sphinx-design ; extra == 'all'
+Requires-Dist: sphinx-external-toc (>=0.3.0) ; extra == 'all'
+Requires-Dist: sphinxext-opengraph (>=0.6.1) ; extra == 'all'
+Requires-Dist: sphinx-markdown-tables (>=0.0.15) ; extra == 'all'
 Requires-Dist: sphinxcontrib-applehelp (>=1.0.2) ; extra == 'all'
-Requires-Dist: sphinxcontrib-devhelp (>=1.0.2) ; extra == 'all'
+Requires-Dist: sphinx (>=4.4.0) ; extra == 'all'
 Requires-Dist: sphinxcontrib-qthelp (>=1.0.3) ; extra == 'all'
-Requires-Dist: sphinxcontrib-serializinghtml (>=1.1.5) ; extra == 'all'
-Requires-Dist: isort (>=5.9.3) ; extra == 'all'
-Requires-Dist: pytest (>=6.2.5) ; extra == 'all'
-Requires-Dist: myst-parser (>=0.16.1) ; extra == 'all'
+Requires-Dist: yapf (>=0.32.0) ; extra == 'all'
+Requires-Dist: sphinx-argparse (>=0.3.1) ; extra == 'all'
+Requires-Dist: sphinxcontrib-jsmath (>=1.0.1) ; extra == 'all'
+Requires-Dist: sphinx-copybutton (>=0.5.0) ; extra == 'all'
+Requires-Dist: sphinxcontrib-devhelp (>=1.0.2) ; extra == 'all'
+Requires-Dist: pytest-cov (>=4.0.0) ; extra == 'all'
+Requires-Dist: pyright (>=1.1.256) ; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: isort (>=5.9.3) ; extra == 'dev'
 Requires-Dist: pre-commit (>=2.17.0) ; extra == 'dev'
 Requires-Dist: pylint (>=2.12.2) ; extra == 'dev'
 Requires-Dist: pyright (>=1.1.256) ; extra == 'dev'
 Requires-Dist: pytest (>=6.2.5) ; extra == 'dev'
 Requires-Dist: pytest-mock (>=3.7.0) ; extra == 'dev'
```

## Comparing `mosaicml_cli-0.3.5.dist-info/RECORD` & `mosaicml_cli-0.3.6.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 mcli/__init__.py,sha256=rjbBF2gbyBq8Hf3mMT7B1S_Chir9b2m6O7N95xthTPE,54
 mcli/config.py,sha256=wFms9BQwrR6YPu9kcRUs5Txgr0lig7pyMW122NgWuUw,16462
-mcli/version.py,sha256=rVZgrgErs_nD6PfOjLV1zQsYjnDdrUrVbwvfLycU_h8,3884
+mcli/version.py,sha256=8nI9AsLSPDx7mQR7JRjGn-jF0zOjfcAW9c0ubi8WncM,3884
 mcli/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/api/exceptions.py,sha256=DTs9XbfuNvXYyy4tiFVpw4kx5eWchVYyd_56HkalmjU,11677
 mcli/api/types.py,sha256=5ZDeWvycwdF70hqfNfmiBJdHY4-wVoeDh-IkBLqLQRQ,508
 mcli/api/typing_future.py,sha256=dtcpSyHS0g3gvgZ_ACrSnTAYFEuh9UjNshcfPJaXkd4,2354
 mcli/api/cluster/__init__.py,sha256=NXNkGsa4lOdwfP8oVjLjakgJxfh8u76u2I_gd3qGSho,134
 mcli/api/cluster/api_get_clusters.py,sha256=TPLdeGqCJMhxe9_jr2kFuNlnzUfJXQhcwV1xeq0fFHs,4058
 mcli/api/engine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mcli/api/engine/engine.py,sha256=VOpY1c9P5ihjDzjvBotAAXPTusbdD0lh6L49qHSu8lY,26222
+mcli/api/engine/engine.py,sha256=nv5sL_iI-u90zi1c9Ij7mXNy7gWrT_tYn1QmKZuIHmY,22935
 mcli/api/engine/utils.py,sha256=_SVWfxUR1tfNRiKZR454oq06xw7O9qvmHT7JpdCa5BU,787
 mcli/api/inference_deployments/__init__.py,sha256=WAL54R3PjKUWRUbnOz-IaemRCa_8yAKYtuyo6zcp9OY,879
 mcli/api/inference_deployments/api_create_inference_deployment.py,sha256=PV5rURaNgWOKTHZ0ZjN1-O6XJpg-62SqlNMXdt_5yK8,3388
 mcli/api/inference_deployments/api_delete_inference_deployments.py,sha256=_HyVvxvs3SpbMsY9S86d1cyhBsoPAG98TMIByJE-ekc,3278
 mcli/api/inference_deployments/api_get_inference_deployments.py,sha256=V2liHBIT5rwGPVcbmPSKqooMxzwdRmsIVWw5a6vpxSA,6091
 mcli/api/inference_deployments/api_ping_inference_deployment.py,sha256=CgewB6lmHAqOHHQNHUNaZoukNoGPmzS1wir6g61aaAk,1156
 mcli/api/inference_deployments/api_predict_inference_deployment.py,sha256=bIKcmh1L25jVrjkx8QKqOm2BUtH6slqYXsCsu8ymMt0,1276
 mcli/api/kube/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/api/kube/runs/__init__.py,sha256=ZNMoJSzTUF8S5o1E0JgIXGmFycUiKA2ei1SsMR7dCd0,856
 mcli/api/kube/runs/api_create_run.py,sha256=zl8ZJxccRGONih02NSweT0cGRT92VlOE1WJfnGN1GA0,4900
 mcli/api/kube/runs/api_delete_runs.py,sha256=NrnhEZ2bYnsvXl2fbMZzDqiuGMy0l0Nc2Yd_BDhZitM,5042
 mcli/api/kube/runs/api_get_run_logs.py,sha256=L5pM-MAF82bOwFHOMVw2J6TSgFi_uNiQ79i282AsbWU,14458
-mcli/api/kube/runs/api_get_runs.py,sha256=rumzxdWCWlK7AxE4TS48UT3qZgfedzEQSIlS6C5NBag,16137
+mcli/api/kube/runs/api_get_runs.py,sha256=iCJFa5Uhb7c73fU8Gzappx-y7RVaA4K6jIU0C_3VqVE,16142
 mcli/api/kube/runs/api_stop_runs.py,sha256=fShzT4zQ1HmHKVwE777QpI9T8S6s37DwsgdaeE_rxUI,6007
 mcli/api/kube/runs/api_watch_run.py,sha256=y2U8hsT1FtlDhh6ui_HojqBRMTWtX8gvwEAaQ-Xr_T8,6210
 mcli/api/mint/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/api/mint/shell.py,sha256=taYNm5G4JNrTBij9r9YLaCIWCm_OHMxPVees7Ee7NjA,4987
 mcli/api/mint/tty.py,sha256=xUNMaK7f0kVO-9YJ5Ze6YjCCEOfHs2qMi9OJVMxNfJw,1530
 mcli/api/model/__init__.py,sha256=RE0PFDKAL5nAwQk30tk9ShXeUwBS9Tu0Bg2qWppsPVE,209
 mcli/api/model/cluster_details.py,sha256=bAcIVF6kgjZ53o2vJswi8tPJfLSRihOZ7slja6OXfr4,5655
 mcli/api/model/inference_deployment.py,sha256=pUa7ya1m8tKVodF22qZTX_QOQnG6QPOGsw2_7WUTW9A,3015
 mcli/api/model/run.py,sha256=nqNbltSh34H7osgpNNeYu-WNOaLyeW5f94Y770IW95Q,7946
 mcli/api/runs/__init__.py,sha256=Lx2k8QidFOo2dJarOwP4hAxrLpIKB_bJwJ7XJKZi0zI,1102
 mcli/api/runs/api_create_run.py,sha256=4OHsrS1eXsBn52RCjEfHPnQF11J8RNF9NHhut97gLgI,2726
 mcli/api/runs/api_delete_runs.py,sha256=2sED0FIKpTrJjrkqpPTedk4E6Lo8ZBpT7Ev3WvlPDOM,3926
 mcli/api/runs/api_get_run_logs.py,sha256=YHZt3j9ffpjhf-Wsumkn4h4az92OGMach9ZXZ0bGcXw,9281
-mcli/api/runs/api_get_runs.py,sha256=AVv_DMrOPT_LP8Nr0CYsLYwSsHYO_SpMllA7wf4QMH4,10400
+mcli/api/runs/api_get_runs.py,sha256=o4TIHHWDnppWSJirdREHi--hCjbIh9DEEm2gT1oq9hE,8968
 mcli/api/runs/api_stop_runs.py,sha256=sJHr2iadiGk0SaeGne_EajvC71kQ90TY4hYrmwOJVLE,5099
 mcli/api/runs/api_update_run_metadata.py,sha256=bbJ4sjPiRXS-97kKAvWJTIwzcc2A4BZjFx7FlbGEuPQ,3937
 mcli/api/runs/api_watch_run.py,sha256=i502PYIuTY1eYxfnVYlN0Gx1MAEMoO2cLCdJIsICalQ,10619
 mcli/api/schema/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/api/schema/generic_model.py,sha256=UrDz_zxAxulD9HFV2h-j0Bmgi8Jo0JFRJzqEkTioJLM,636
 mcli/api/secrets/__init__.py,sha256=bAZh1wEkxpZN18pOc-NrGPdzT7W1lJsOa_u2Rr1F2Vk,309
 mcli/api/secrets/api_create_secret.py,sha256=zjHsMCfmLBWfQ-gYOnklkSusSXGY7eXJcW_FAaq2eTw,2365
@@ -47,15 +47,15 @@
 mcli/api/secrets/api_get_secrets.py,sha256=ddkz2BQ7JPx4oumDMc15bmKaNl-wCNoEsbpShWMfeGA,3697
 mcli/api/users/__init__.py,sha256=L4JQW7sgZK7Isf6pdsNlMI0a-09kH4Nhg44BIRPzfE0,139
 mcli/api/users/api_get_users.py,sha256=qnJnAozTSsrUzWVi7NRXbLUB0928Y-SKKXHDNI-hMcg,2694
 mcli/cli/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/cli.py,sha256=OH3rAEXiY4W4djuodGmdsxtzZIw7cEJ65sBkkKQGqTg,7182
 mcli/cli/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/common/deployment_filters.py,sha256=n5SRmWO9WwJlF9tzCq5vW5MmUUKXpyUIXIjir4Cmq54,2670
-mcli/cli/common/run_filters.py,sha256=H3jeU2t7C7_eHZfSmnnmeaHF0S_0YrpWMo70_tHguwQ,7238
+mcli/cli/common/run_filters.py,sha256=3TKjRQzJoBYOE70n_FnAb3bAYwzbYxlLIOOp20rxIrw,7180
 mcli/cli/m_clean/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_clean/m_clean.py,sha256=9M85zN1UiZC7sokgV6GEAlJaPG1sFVE4CvOMIpf8QMI,950
 mcli/cli/m_connect/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_connect/m_connect.py,sha256=3kYe2JMz38TjhyeY1ehTM4kHwT9OrrkH4csUuhWEbfw,1541
 mcli/cli/m_create/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_create/cluster.py,sha256=ZZQjvIuLniWKY_RUc8920GuYbPO53L65Yn5xplSKEp8,11513
 mcli/cli/m_create/env_var.py,sha256=8KaD4y4avIVJmtz95PwORPAaXIsHqZgLXdi5-dN7qVU,7167
@@ -72,15 +72,15 @@
 mcli/cli/m_describe/m_describe.py,sha256=L_-rKu8p1MhmC-bpEFzR5Io1E4Bk09wZ-SlhyRCnQek,1860
 mcli/cli/m_get/__init__.py,sha256=nS0qdgx4DwqtFUbnNREWSfSHY17K6xT2fr7i15nN0jc,549
 mcli/cli/m_get/clusters.py,sha256=7eV157RasxpoBIaQcG6D7k11VY3hSM15rUEcz1emJrQ,3909
 mcli/cli/m_get/display.py,sha256=IFoYOBDieSpok94Ey_q4tl3sUsbOK6ac2SexIGe0HgY,6452
 mcli/cli/m_get/envvars.py,sha256=Jqy3tnK9g3EO1xePREMhRzWo45G_ZDjbLjOszQ1Nl9Q,1315
 mcli/cli/m_get/inference_deployments.py,sha256=BRu6pojlonNjyJSDivpgvYddtUEYpeBjW9vzIYEiWv0,5361
 mcli/cli/m_get/m_get.py,sha256=goLhmY5n0_Xqr3RRgHZtfi2DiSCIwr25HnuFm_N6uwg,4866
-mcli/cli/m_get/runs.py,sha256=gPA4_d6d-Rr4YOszefMmCscMN1NVpR0bM2aAiqMg0kw,7104
+mcli/cli/m_get/runs.py,sha256=EKvA70QVMEvClQBqVQ37f87-GgpgdC8NpmcTh0WJQKs,6346
 mcli/cli/m_get/secrets.py,sha256=6HvbxJVOOsK6fYderHCHNlAHxVtUaNW4O5kses0tvP8,3567
 mcli/cli/m_get/users.py,sha256=kSYAJDRUeEGqXi2-escvzOM2_sw671crBDsqaZQDi_I,1580
 mcli/cli/m_init/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_init/m_init.py,sha256=xMOxNjQnscFuvK0wnF2UIzUYOCXl3eTabLqShtHDgWo,4113
 mcli/cli/m_init/m_init_kube.py,sha256=Vd7M1qAJG2oDKSCj3FC7m7NFiQ_jwnaT3wMlcri-YXE,9374
 mcli/cli/m_interactive/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mcli/cli/m_interactive/interactive.py,sha256=IWTsgO-VaqazPcJuA6M-NgcMgFf2Me3Q0vwYom2RKTg,9005
@@ -197,12 +197,12 @@
 mcli/utils/utils_rich.py,sha256=CbQiVIzXgf6yQzIrUj2d8JZWOF2L05gHV2Fry4tHxM4,3115
 mcli/utils/utils_run_status.py,sha256=Iv5AWtF1tDsC0VK-n3W6vynNzDtvX918krhO_oFA4MQ,8533
 mcli/utils/utils_serializable_dataclass.py,sha256=m0rhTI60NpN1ET2T7VChnjZID1JpDDRuBI4A3LMRacI,4350
 mcli/utils/utils_spinner.py,sha256=NZZ0l0OJyEs-fFZSt1S3h_LiSGP4oT67HMPXATUPZtY,1103
 mcli/utils/utils_string_functions.py,sha256=Z5ouIGOf02pxxTlE_ZijZxhsSaj9p499TA7fP65Ik-0,11437
 mcli/utils/utils_types.py,sha256=EVfUa5HG0SoOo3w7A6Wh4Vqi7ojTeiEPjudFok1u-hs,3954
 mcli/utils/utils_yaml.py,sha256=O-ucRDZr5zYlALUtngFQ1E5bf-cj6Zu7OyaiUR2SgEs,1001
-mosaicml_cli-0.3.5.dist-info/METADATA,sha256=9Df63RPX1h0nchiqYXALbQSugOn65Lv1J70hTrehK6E,4743
-mosaicml_cli-0.3.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mosaicml_cli-0.3.5.dist-info/entry_points.txt,sha256=YgBbHmB6YftDcyJhavLU_Tpcn8gyZN9M1i11AGD9HPI,75
-mosaicml_cli-0.3.5.dist-info/top_level.txt,sha256=_bnO8J2EUkliWivey_1le0UrnocFKmyVMQjbQ8iVXjc,5
-mosaicml_cli-0.3.5.dist-info/RECORD,,
+mosaicml_cli-0.3.6.dist-info/METADATA,sha256=w6GgLzBAdv3H_CXsxEHw7DdWD2gdZLSBJWfIc63jYXg,4743
+mosaicml_cli-0.3.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mosaicml_cli-0.3.6.dist-info/entry_points.txt,sha256=YgBbHmB6YftDcyJhavLU_Tpcn8gyZN9M1i11AGD9HPI,75
+mosaicml_cli-0.3.6.dist-info/top_level.txt,sha256=_bnO8J2EUkliWivey_1le0UrnocFKmyVMQjbQ8iVXjc,5
+mosaicml_cli-0.3.6.dist-info/RECORD,,
```

