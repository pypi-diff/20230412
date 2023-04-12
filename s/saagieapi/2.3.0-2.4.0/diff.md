# Comparing `tmp/saagieapi-2.3.0.tar.gz` & `tmp/saagieapi-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saagieapi-2.3.0.tar", max compression
+gzip compressed data, was "saagieapi-2.4.0.tar", max compression
```

## Comparing `saagieapi-2.3.0.tar` & `saagieapi-2.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11357 2023-04-05 07:34:17.018097 saagieapi-2.3.0/LICENSE
--rw-r--r--   0        0        0     4379 2023-04-05 07:34:17.018097 saagieapi-2.3.0/README.md
--rw-r--r--   0        0        0     1562 2023-04-05 07:34:54.350268 saagieapi-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      502 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/__init__.py
--rw-r--r--   0        0        0       43 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/apps/__init__.py
--rw-r--r--   0        0        0    33369 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/apps/apps.py
--rw-r--r--   0        0        0     5809 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/apps/gql_queries.py
--rw-r--r--   0        0        0       83 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/docker_credentials/__init__.py
--rw-r--r--   0        0        0     8465 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/docker_credentials/docker_credentials.py
--rw-r--r--   0        0        0     1657 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/docker_credentials/gql_queries.py
--rw-r--r--   0        0        0       53 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/env_vars/__init__.py
--rw-r--r--   0        0        0    18460 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/env_vars/env_vars.py
--rw-r--r--   0        0        0     1701 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/env_vars/gql_queries.py
--rw-r--r--   0        0        0     1871 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/gql_queries.py
--rw-r--r--   0        0        0       43 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/jobs/__init__.py
--rw-r--r--   0        0        0     7840 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/jobs/gql_queries.py
--rw-r--r--   0        0        0    36314 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/jobs/jobs.py
--rw-r--r--   0        0        0      141 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/pipelines/__init__.py
--rw-r--r--   0        0        0     6510 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/pipelines/gql_queries.py
--rw-r--r--   0        0        0     2384 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/pipelines/graph_pipeline.py
--rw-r--r--   0        0        0    28308 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/pipelines/pipelines.py
--rw-r--r--   0        0        0       55 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/projects/__init__.py
--rw-r--r--   0        0        0     2914 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/projects/gql_queries.py
--rw-r--r--   0        0        0    24403 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/projects/projects.py
--rw-r--r--   0        0        0       67 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/repositories/__init__.py
--rw-r--r--   0        0        0     6269 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/repositories/gql_queries.py
--rw-r--r--   0        0        0    10534 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/repositories/repositories.py
--rw-r--r--   0        0        0    14201 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/saagie_api.py
--rw-r--r--   0        0        0       55 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/storages/__init__.py
--rw-r--r--   0        0        0     1220 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/storages/gql_queries.py
--rw-r--r--   0        0        0     6561 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/storages/storages.py
--rw-r--r--   0        0        0        0 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/utils/__init__.py
--rw-r--r--   0        0        0     1725 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/utils/bearer_auth.py
--rw-r--r--   0        0        0     3969 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/utils/folder_functions.py
--rw-r--r--   0        0        0     3113 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/utils/gql_client.py
--rw-r--r--   0        0        0       54 2023-04-05 07:34:17.022097 saagieapi-2.3.0/saagieapi/utils/rich_console.py
--rw-r--r--   0        0        0     5328 1970-01-01 00:00:00.000000 saagieapi-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-12 13:06:35.221221 saagieapi-2.4.0/LICENSE
+-rw-r--r--   0        0        0     4379 2023-04-12 13:06:35.221221 saagieapi-2.4.0/README.md
+-rw-r--r--   0        0        0     1562 2023-04-12 13:07:06.465411 saagieapi-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      502 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/__init__.py
+-rw-r--r--   0        0        0       43 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/apps/__init__.py
+-rw-r--r--   0        0        0    33369 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/apps/apps.py
+-rw-r--r--   0        0        0     7591 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/apps/gql_queries.py
+-rw-r--r--   0        0        0       83 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/docker_credentials/__init__.py
+-rw-r--r--   0        0        0     8465 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/docker_credentials/docker_credentials.py
+-rw-r--r--   0        0        0     1657 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/docker_credentials/gql_queries.py
+-rw-r--r--   0        0        0       53 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/env_vars/__init__.py
+-rw-r--r--   0        0        0    27280 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/env_vars/env_vars.py
+-rw-r--r--   0        0        0     2671 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/env_vars/gql_queries.py
+-rw-r--r--   0        0        0     2414 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/gql_queries.py
+-rw-r--r--   0        0        0       43 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/jobs/__init__.py
+-rw-r--r--   0        0        0     9510 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/jobs/gql_queries.py
+-rw-r--r--   0        0        0    36314 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/jobs/jobs.py
+-rw-r--r--   0        0        0      141 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/pipelines/__init__.py
+-rw-r--r--   0        0        0     7785 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/pipelines/gql_queries.py
+-rw-r--r--   0        0        0     2384 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/pipelines/graph_pipeline.py
+-rw-r--r--   0        0        0    29262 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/pipelines/pipelines.py
+-rw-r--r--   0        0        0       55 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/projects/__init__.py
+-rw-r--r--   0        0        0     2962 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/projects/gql_queries.py
+-rw-r--r--   0        0        0    24403 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/projects/projects.py
+-rw-r--r--   0        0        0       67 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/repositories/__init__.py
+-rw-r--r--   0        0        0     8443 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/repositories/gql_queries.py
+-rw-r--r--   0        0        0    10534 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/repositories/repositories.py
+-rw-r--r--   0        0        0    14653 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/saagie_api.py
+-rw-r--r--   0        0        0       55 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/storages/__init__.py
+-rw-r--r--   0        0        0     1384 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/storages/gql_queries.py
+-rw-r--r--   0        0        0     6561 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/storages/storages.py
+-rw-r--r--   0        0        0        0 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/utils/__init__.py
+-rw-r--r--   0        0        0     1725 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/utils/bearer_auth.py
+-rw-r--r--   0        0        0     3969 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/utils/folder_functions.py
+-rw-r--r--   0        0        0     3113 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/utils/gql_client.py
+-rw-r--r--   0        0        0       54 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/utils/rich_console.py
+-rw-r--r--   0        0        0     5328 1970-01-01 00:00:00.000000 saagieapi-2.4.0/PKG-INFO
```

### Comparing `saagieapi-2.3.0/LICENSE` & `saagieapi-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/README.md` & `saagieapi-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/pyproject.toml` & `saagieapi-2.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saagieapi"
-version = "2.3.0"
+version = "2.4.0"
 description = "Python API to interact with Saagie"
 authors = ["Saagie"]
 license = "GLWTPL"
 readme = "README.md"
 repository = "https://github.com/saagie/api-saagie"
 
 [tool.poetry.dependencies]
```

### Comparing `saagieapi-2.3.0/saagieapi/apps/apps.py` & `saagieapi-2.4.0/saagieapi/apps/apps.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/saagieapi/apps/gql_queries.py` & `saagieapi-2.4.0/saagieapi/apps/gql_queries.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,372 +1,376 @@
 # pylint: disable=duplicate-code
 GQL_LIST_APPS_FOR_PROJECT = """
 fragment versionInfo on AppVersion {
-  number
-  creationDate
-  releaseNote
-  dockerInfo {
-    image
-    dockerCredentialsId
-  }
-  runtimeContextId
-  creator
-  ports {
-    name
     number
-    isRewriteUrl
-    basePathVariableName
-    scope
-    internalUrl
-  }
-  isMajor
-  volumesWithPath {
-    path
-    volume {
-      id
-      name
-      creator
-      description
-      size
-      projectId
-      creationDate
-      linkedApp {
-        id
+    creationDate
+    releaseNote
+    dockerInfo {
+        image
+        dockerCredentialsId
+    }
+    runtimeContextId
+    creator
+    ports {
         name
-      }
+        number
+        isRewriteUrl
+        basePathVariableName
+        scope
+        internalUrl
+    }
+    isMajor
+    volumesWithPath {
+        path
+        volume {
+            id
+            name
+            creator
+            description
+            size
+            projectId
+            creationDate
+            linkedApp {
+                id
+                name
+            }
+        }
     }
-  }
 }
 
 fragment appInformations on App {
-  description
-  creationDate
-  creator
-  versions @skip(if: $versionsOnlyCurrent) {
-    ...versionInfo
-  }
-  currentVersion {
-    ...versionInfo
-  }
-  technology {
-    id
-  }
-  linkedVolumes {
-    id
-    name
-    creator
     description
-    size
     creationDate
-  }
-  isGenericApp
-  history {
-    id
-    events {
-      event {
-        recordAt
-        executionId
-        __typename
-        ... on RunAction {
-          versionNumber
-          author
-        }
-        ... on StopAction {
-          author
-        }
-        ... on RollbackAction {
-          versionNumber
-          author
-        }
-        ... on UpgradeAction {
-          versionNumber
-          author
-        }
-        ... on RestartAction {
-          versionNumber
-          author
-        }
-        ... on StatusRetrieve {
-          status
-        }
-      }
-      transitionTime
-    }
-    runningVersionNumber
-    currentDockerInfo {
-      image
-      dockerCredentialsId
-    }
-    currentStatus
-    currentExecutionId
-    startTime
-    stopTime
-  }
-  alerting {
-    emails
-    statusList
-    loginEmails {
-      login
-      email
-    }
-  }
-  resources {
-    cpu {
-      request
-      limit
-    }
-    memory {
-      request
-      limit
+    creator
+    versions @skip(if: $versionsOnlyCurrent) {
+        ...versionInfo
+    }
+    currentVersion {
+        ...versionInfo
+    }
+    technology {
+        id
+    }
+    linkedVolumes {
+        id
+        name
+        creator
+        description
+        size
+        creationDate
+    }
+    isGenericApp
+    history {
+        id
+        events {
+            event {
+                recordAt
+                executionId
+                __typename
+                ... on RunAction {
+                    versionNumber
+                    author
+                }
+                ... on StopAction {
+                    author
+                }
+                ... on RollbackAction {
+                    versionNumber
+                    author
+                }
+                ... on UpgradeAction {
+                    versionNumber
+                    author
+                }
+                ... on RestartAction {
+                    versionNumber
+                    author
+                }
+                ... on StatusRetrieve {
+                    status
+                    reason
+                }
+            }
+            transitionTime
+        }
+        runningVersionNumber
+        currentDockerInfo {
+            image
+            dockerCredentialsId
+        }
+        currentStatus
+        currentStatusReason
+        currentExecutionId
+        startTime
+        stopTime
+    }
+    alerting {
+        emails
+        statusList
+        loginEmails {
+            login
+            email
+        }
+    }
+    resources {
+        cpu {
+            request
+            limit
+        }
+        memory {
+            request
+            limit
+        }
     }
-  }
 }
 
 query projectQuery($id: UUID!, $minimal: Boolean!, $versionsOnlyCurrent: Boolean!) {
-  project(id: $id) {
-    apps {
-      id
-      name
-      ...appInformations @skip(if: $minimal)
+    project(id: $id) {
+        apps {
+            id
+            name
+            ...appInformations @skip(if: $minimal)
+        }
     }
-  }
 }
 """
 
 GQL_GET_APP_INFO = """
 fragment appVersionFieldFullInformation on AppVersion {
-  number
-  creator
-  creationDate
-  releaseNote
-  dockerInfo {
-    image
-    dockerCredentialsId
-  }
-  runtimeContextId
-  ports {
-    name
     number
-    isRewriteUrl
-    basePathVariableName
-    scope
-    internalUrl
-  }
-  volumesWithPath {
-    path
-    volume {
-      id
-      name
-      creator
-      description
-      size
-      projectId
-      creationDate
-      linkedApp {
-        id
-        name
-      }
-    }
-  }
-  isMajor
-}
-
-query app($id: UUID!, $versionsOnlyCurrent: Boolean!) {
-  app(id: $id) {
-    id
-    name
-    creationDate
-    technology {
-      id
-    }
-    project {
-      id
-      name
-    }
-    description
+    creator
     creationDate
-    versions @skip(if: $versionsOnlyCurrent) {
-      ...appVersionFieldFullInformation
-    }
-    currentVersion {
-      ...appVersionFieldFullInformation
-    }
-    history {
-      id
-      currentStatus
-      currentExecutionId
-      currentDockerInfo {
+    releaseNote
+    dockerInfo {
         image
         dockerCredentialsId
-      }
-      startTime
-      stopTime
-      events {
-        event {
-          recordAt
-          executionId
-          __typename
-          ... on RunAction {
-            versionNumber
-            author
-          }
-          ... on StopAction {
-            author
-          }
-          ... on RollbackAction {
-            versionNumber
-            author
-          }
-          ... on UpgradeAction {
-            versionNumber
-            author
-          }
-          ... on RestartAction {
-            versionNumber
-            author
-          }
-          ... on StatusRetrieve {
-            status
-          }
-        }
-        transitionTime
-      }
     }
-    isGenericApp
-    alerting {
-      emails
-      statusList
-      loginEmails {
-        login
-        email
-      }
+    runtimeContextId
+    ports {
+        name
+        number
+        isRewriteUrl
+        basePathVariableName
+        scope
+        internalUrl
     }
-    resources {
-      cpu {
-        request
-        limit
-      }
-      memory {
-        request
-        limit
-      }
+    volumesWithPath {
+        path
+        volume {
+            id
+            name
+            creator
+            description
+            size
+            projectId
+            creationDate
+            linkedApp {
+                id
+                name
+            }
+        }
     }
-    linkedVolumes {
-      id
-      name
-      creator
-      description
-      size
-      creationDate
+    isMajor
+}
+
+query app($id: UUID!, $versionsOnlyCurrent: Boolean!) {
+    app(id: $id) {
+        id
+        name
+        creationDate
+        technology {
+            id
+        }
+        project {
+            id
+            name
+        }
+        description
+        creationDate
+        versions @skip(if: $versionsOnlyCurrent) {
+            ...appVersionFieldFullInformation
+        }
+        currentVersion {
+            ...appVersionFieldFullInformation
+        }
+        history {
+            id
+            currentStatus
+            currentStatusReason
+            currentExecutionId
+            currentDockerInfo {
+                image
+                dockerCredentialsId
+            }
+            startTime
+            stopTime
+            events {
+                event {
+                    recordAt
+                    executionId
+                    __typename
+                    ... on RunAction {
+                        versionNumber
+                        author
+                    }
+                    ... on StopAction {
+                        author
+                    }
+                    ... on RollbackAction {
+                        versionNumber
+                        author
+                    }
+                    ... on UpgradeAction {
+                        versionNumber
+                        author
+                    }
+                    ... on RestartAction {
+                        versionNumber
+                        author
+                    }
+                    ... on StatusRetrieve {
+                        status
+                        reason
+                    }
+                }
+                transitionTime
+            }
+        }
+        isGenericApp
+        alerting {
+            emails
+            statusList
+            loginEmails {
+                login
+                email
+            }
+        }
+        resources {
+            cpu {
+                request
+                limit
+            }
+            memory {
+                request
+                limit
+            }
+        }
+        linkedVolumes {
+            id
+            name
+            creator
+            description
+            size
+            creationDate
+        }
     }
-  }
 }
 """
 
 GQL_CREATE_APP_CATALOG = """
 mutation installAppMutation($projectId: UUID!, $technologyId: UUID!, $contextId: String!) {
-  installApp(projectId: $projectId, technologyId: $technologyId, contextId: $contextId) {
-    id
-    name
-  }
+    installApp(projectId: $projectId, technologyId: $technologyId, contextId: $contextId) {
+        id
+        name
+    }
 }
 """
 
 GQL_CREATE_APP_SCRATCH = """
 mutation createAppMutation($app: AppInput!) {
-  createApp(app: $app) {
-    id
-  }
+    createApp(app: $app) {
+        id
+    }
 }
 """
 
 GQL_EDIT_APP = """
 mutation editAppMutation($app: AppEditionInput!) {
-  editApp(appEdition: $app) {
-    id
-  }
+    editApp(appEdition: $app) {
+        id
+    }
 }
 """
 
 GQL_DELETE_APP = """
 mutation deleteAppMutation($appId: UUID!) {
-  deleteApp(appId: $appId) {
-    id
-  }
+    deleteApp(appId: $appId) {
+        id
+    }
 }
 """
 
 GQL_STOP_APP = """
 mutation stopAppMutation($id: UUID!) {
-  stopApp(id: $id) {
-    id
-    history {
-      id
-      runningVersionNumber
-      currentStatus
+    stopApp(id: $id) {
+        id
+        history {
+            id
+            runningVersionNumber
+            currentStatus
+        }
     }
-  }
 }
 """
 
 GQL_RUN_APP = """
 mutation runAppMutation($id: UUID!) {
-  runApp(id: $id) {
-    id
-    versions {
-      number
-    }
-    history {
-      id
-      currentDockerInfo {
-        image
-        dockerCredentialsId
-      }
-      runningVersionNumber
-      currentStatus
+    runApp(id: $id) {
+        id
+        versions {
+            number
+        }
+        history {
+            id
+            currentDockerInfo {
+                image
+                dockerCredentialsId
+            }
+            runningVersionNumber
+            currentStatus
+        }
     }
-  }
 }
 """
 
 GQL_UPDATE_APP = """
 mutation addAppVersion($appId: UUID!, $appVersion: AppVersionInput!) {
-  addAppVersion(appId: $appId, version: $appVersion) {
-    number
-    releaseNote
-    dockerInfo {
-      image
-      dockerCredentialsId
-    }
-    ports {
-      number
-      name
-      basePathVariableName
-      isRewriteUrl
-      scope
-    }
-    volumesWithPath {
-      path
-      volume {
-        id
-        name
-        size
-        creator
-      }
+    addAppVersion(appId: $appId, version: $appVersion) {
+        number
+        releaseNote
+        dockerInfo {
+            image
+            dockerCredentialsId
+        }
+        ports {
+            number
+            name
+            basePathVariableName
+            isRewriteUrl
+            scope
+        }
+        volumesWithPath {
+            path
+            volume {
+                id
+                name
+                size
+                creator
+            }
+        }
     }
-  }
 }
 """
 
 GQL_ROLLBACK_APP_VERSION = """
 mutation rollbackAppVersionMutation($appId: UUID!, $versionNumber: Int!) {
-  rollbackAppVersion(appId: $appId, versionNumber: $versionNumber) {
-    id
-    versions {
-      number
-    }
-    currentVersion {
-      number
+    rollbackAppVersion(appId: $appId, versionNumber: $versionNumber) {
+        id
+        versions {
+            number
+        }
+        currentVersion {
+            number
+        }
     }
-  }
 }
 """
```

### Comparing `saagieapi-2.3.0/saagieapi/docker_credentials/docker_credentials.py` & `saagieapi-2.4.0/saagieapi/docker_credentials/docker_credentials.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/saagieapi/docker_credentials/gql_queries.py` & `saagieapi-2.4.0/saagieapi/docker_credentials/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/saagieapi/env_vars/env_vars.py` & `saagieapi-2.4.0/saagieapi/env_vars/env_vars.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class EnvVars:
     # pylint: disable=singleton-comparison
     def __init__(self, saagie_api):
         self.saagie_api = saagie_api
         self.client = saagie_api.client
 
-    def list_globals(self, pprint_result: Optional[bool] = None):
+    def list_globals(self, pprint_result: Optional[bool] = None) -> Dict:
         """Get global environment variables
         NB: You can only list environment variables if you have at least the
         viewer role on the platform
         Params
         ------
         pprint_result : bool, optional
             Whether to pretty print the result of the query, default to
@@ -46,34 +46,36 @@
 
         Returns
         -------
         dict
             Dict of created environment variable
         """
         params = {
-            "name": name,
-            "value": value,
-            "description": description,
-            "isPassword": is_password,
-            "scope": "GLOBAL",
+            "envVar": {
+                "name": name,
+                "value": value,
+                "description": description,
+                "isPassword": is_password,
+                "scope": "GLOBAL",
+            }
         }
 
         result = self.saagie_api.client.execute(query=gql(GQL_CREATE_ENV_VAR), variable_values=params)
         logging.info("✅ Environment variable [%s] successfully created", name)
         return result
 
     def update_global(
         self, name: str, new_name: str = None, value: str = None, description: str = None, is_password: bool = None
     ) -> Dict:
         """
         Update environment variable with provided function variables if it exists
         Parameters
         ----------
         name : str
-            Name of the environment to upgrade
+            Name of the environment variable to upgrade
         new_name : str, optional
             New name of the environment variable. If none provided, keep the actual one
         value: str, optional
             New value of the environment variable. If none provided, keep the actual one
         description: str, optional
             New description of the environment variable. If none provided, keep the actual one
         is_password: boolean, optional
@@ -91,29 +93,29 @@
         """
 
         existing_env_var = self.list_globals(pprint_result=False)["globalEnvironmentVariables"]
 
         if name not in [env_var["name"] for env_var in existing_env_var]:
             raise ValueError(f"❌ Environment variable {name} does not exists")
 
-        params = [d for d in existing_env_var if d["name"] == name][0]
-
-        if params["isPassword"] == True:
-            params.pop("value")
+        params = {
+            "envVar": [d for d in existing_env_var if d["name"] == name][0],
+        }
+        params["envVar"].pop("isValid")
+        params["envVar"].pop("invalidReasons")
+        if params["envVar"]["isPassword"] == True:
+            params["envVar"].pop("value")
         if new_name:
-            params["name"] = new_name
+            params["envVar"]["name"] = new_name
         if value:
-            params["value"] = value
+            params["envVar"]["value"] = value
         if description:
-            params["description"] = description
-        if is_password == True:
-            params["isPassword"] = is_password
-        elif is_password == False:
-            params["isPassword"] = is_password
-
+            params["envVar"]["description"] = description
+        if is_password in {True, False}:
+            params["envVar"]["isPassword"] = is_password
         result = self.saagie_api.client.execute(query=gql(GQL_UPDATE_ENV_VAR), variable_values=params)
         logging.info("✅ Environment variable [%s] successfully updated", name)
         return result
 
     def create_or_update_global(self, name: str, value: str, description: str = "", is_password: bool = False) -> Dict:
         """
         Create a new global environnement variable or update it if it already exists
@@ -219,20 +221,22 @@
 
         Returns
         -------
         dict
             Dict of created environment variable
         """
         params = {
-            "projectId": project_id,
-            "name": name,
-            "value": value,
-            "description": description,
-            "isPassword": is_password,
-            "scope": "PROJECT",
+            "entityId": project_id,
+            "envVar": {
+                "name": name,
+                "value": value,
+                "description": description,
+                "isPassword": is_password,
+                "scope": "PROJECT",
+            },
         }
 
         result = self.saagie_api.client.execute(query=gql(GQL_CREATE_ENV_VAR), variable_values=params)
         logging.info("✅ Environment variable [%s] successfully created", name)
         return result
 
     def update_for_project(
@@ -248,15 +252,15 @@
         Update environment variable with provided function variables if it exists
 
         Parameters
         ----------
         project_id : str
             ID of the project
         name : str
-            Name of the environment to upgrade
+            Name of the environment variable to upgrade
         new_name : str, optional
             New name of the environment variable. If none provided, keep the actual one
         value: str, optional
             New value of the environment variable. If none provided, keep the actual one
         description: str, optional
             New description of the environment variable. If none provided, keep the actual one
         is_password: boolean, optional
@@ -274,29 +278,31 @@
         """
 
         existing_env_var = self.list_for_project(project_id, pprint_result=False)["projectEnvironmentVariables"]
 
         if name not in [env_var["name"] for env_var in existing_env_var if env_var["scope"] == "PROJECT"]:
             raise ValueError(f"❌ Environment variable {name} does not exists")
 
-        params = [d for d in existing_env_var if d["name"] == name][0]
-        params["projectId"] = project_id
-        if params["isPassword"] == True:
-            params.pop("value")
+        params = {
+            "entityId": project_id,
+            "envVar": [d for d in existing_env_var if d["name"] == name][0],
+        }
+        params["envVar"].pop("isValid")
+        params["envVar"].pop("overriddenValues")
+        params["envVar"].pop("invalidReasons")
+        if params["envVar"]["isPassword"] == True:
+            params["envVar"].pop("value")
         if new_name:
-            params["name"] = new_name
+            params["envVar"]["name"] = new_name
         if value:
-            params["value"] = value
+            params["envVar"]["value"] = value
         if description:
-            params["description"] = description
-        if is_password == True:
-            params["isPassword"] = is_password
-        elif is_password == False:
-            params["isPassword"] = is_password
-
+            params["envVar"]["description"] = description
+        if is_password in {True, False}:
+            params["envVar"]["isPassword"] = is_password
         result = self.saagie_api.client.execute(query=gql(GQL_UPDATE_ENV_VAR), variable_values=params)
         logging.info("✅ Environment variable [%s] successfully updated", name)
         return result
 
     def create_or_update_for_project(
         self, project_id: str, name: str, value: str, description: str = "", is_password: bool = False
     ) -> Dict:
@@ -368,15 +374,248 @@
 
         project_env_id = project_env[0]["id"]
 
         result = self.saagie_api.client.execute(query=gql(GQL_DELETE_ENV_VAR), variable_values={"id": project_env_id})
         logging.info("✅ Environment variable [%s] successfully deleted", name)
         return result
 
-    def export(self, project_id, output_folder: str, error_folder: Optional[str] = "", project_only: bool = False):
+    def list_for_pipeline(self, pipeline_id: str, pprint_result: Optional[bool] = None) -> Dict:
+        """Get pipeline environment variables
+        NB: You can only list environment variables if you have at least the
+        viewer role on the project
+
+        Parameters
+        ----------
+        pipeline_id : str
+            UUID of your pipeline (see README on how to find it)
+        pprint_result : bool, optional
+            Whether to pretty print the result of the query, default to
+            saagie_api.pprint_global
+        Returns
+        -------
+        dict
+            Dict of pipeline environment variables
+        """
+        params = {
+            "pipelineId": pipeline_id,
+        }
+
+        return self.saagie_api.client.execute(
+            query=gql(GQL_LIST_PIPELINE_ENV_VARS), variable_values=params, pprint_result=pprint_result
+        )
+
+    def create_for_pipeline(
+        self, pipeline_id: str, name: str, value: str, description: str = "", is_password: bool = False
+    ) -> Dict:
+        """Create an environment variable in a given pipeline
+
+        Parameters
+        ----------
+        pipeline_id : str
+            UUID of your pipeline (see README on how to find it)
+        name : str
+            Name of the environment variable to create
+        value : str
+            Value of the environment variable to create
+        description : str, optional
+            Description of the environment variable to create
+        is_password : bool, optional
+            Weather the environment variable to create is a password or not
+
+        Returns
+        -------
+        dict
+            Dict of created environment variable
+        """
+        params = {
+            "entityId": pipeline_id,
+            "envVar": {
+                "name": name,
+                "value": value,
+                "description": description,
+                "isPassword": is_password,
+                "scope": "PIPELINE",
+            },
+        }
+
+        result = self.saagie_api.client.execute(query=gql(GQL_CREATE_ENV_VAR), variable_values=params)
+        logging.info("✅ Environment variable [%s] successfully created", name)
+        return result
+
+    def bulk_create_for_pipeline(self, pipeline_id: str, env_vars: Dict) -> Dict:
+        """Delete all existing env vars and create new ones for the pipeline
+
+        Parameters
+        ----------
+        pipeline_id : str
+            Pipeline ID
+        env_vars : Dict
+            Dict that contains all the variables for the pipeline
+
+        Returns
+        -------
+        dict
+            Dict of created environment variables for pipeline
+        """
+
+        # need to transform the dict in parameter to a string with the following format"var1=val1\nvar2=val2"
+        var_str = "".join(f"{key}={env_vars[key]}\n" for key in env_vars)
+
+        params = {
+            "entityId": pipeline_id,
+            "scope": "PIPELINE",
+            "rawEnvironmentVariables": var_str,
+        }
+
+        result = self.saagie_api.client.execute(query=gql(GQL_CREATE_PIPELINE_ENV_VAR), variable_values=params)
+        logging.info("✅ Environment variables for pipeline [%s] successfully created", pipeline_id)
+        return result
+
+    def update_for_pipeline(
+        self,
+        pipeline_id: str,
+        name: str,
+        new_name: str = None,
+        value: str = None,
+        description: str = None,
+        is_password: bool = None,
+    ) -> Dict:
+        """
+        Update environment variable with provided function variables if it exists
+
+        Parameters
+        ----------
+        pipeline_id : str
+            ID of the project
+        name : str
+            Name of the environment variable to upgrade
+        new_name : str, optional
+            New name of the environment variable. If none provided, keep the actual one
+        value: str, optional
+            New value of the environment variable. If none provided, keep the actual one
+        description: str, optional
+            New description of the environment variable. If none provided, keep the actual one
+        is_password: boolean, optional
+            New password boolean status. If none provided, keep the actual one
+
+        Returns
+        -------
+        dict
+            Dict containing the id of the updated environment variable
+
+        Raises
+        ------
+        ValueError
+            When the variable doesn't already exist
+        """
+
+        existing_env_var = self.list_for_pipeline(pipeline_id, pprint_result=False)["pipelineEnvironmentVariables"]
+
+        if name not in [env_var["name"] for env_var in existing_env_var if env_var["scope"] == "PIPELINE"]:
+            raise ValueError(f"❌ Environment variable {name} does not exists")
+
+        params = {
+            "entityId": pipeline_id,
+            "envVar": [d for d in existing_env_var if d["name"] == name][0],
+        }
+        params["envVar"].pop("isValid")
+        params["envVar"].pop("overriddenValues")
+        params["envVar"].pop("invalidReasons")
+        if params["envVar"]["isPassword"] == True:
+            params["envVar"].pop("value")
+        if new_name:
+            params["envVar"]["name"] = new_name
+        if value:
+            params["envVar"]["value"] = value
+        if description:
+            params["envVar"]["description"] = description
+        if is_password in {True, False}:
+            params["envVar"]["isPassword"] = is_password
+        result = self.saagie_api.client.execute(query=gql(GQL_UPDATE_ENV_VAR), variable_values=params)
+        logging.info("✅ Environment variable [%s] successfully updated", name)
+        return result
+
+    def create_or_update_for_pipeline(
+        self, pipeline_id: str, name: str, value: str, description: str = "", is_password: bool = False
+    ) -> Dict:
+        """
+        Create a new pipeline environment variable or update it if it already exists
+
+        Parameters
+        ----------
+        pipeline_id : str
+            UUID of your pipeline (see README on how to find it)
+        name: str
+            Unique name of the environment variable to create or modify
+        value: str
+            Value of the environment variable to create or modify
+        description: str, optional
+            Description of the variable
+        is_password: boolean, optional
+            Weather the variable is a password or not (default: False)
+
+        Returns
+        -------
+        dict
+            Dict of created or updated environment variable
+        """
+
+        existing_env_var = self.list_for_pipeline(pipeline_id, pprint_result=False)["pipelineEnvironmentVariables"]
+        present = name in [env["name"] for env in existing_env_var if env["scope"] == "PIPELINE"]
+
+        # If variable not present, create it
+        if not present:
+            return self.create_for_pipeline(
+                pipeline_id=pipeline_id, name=name, value=value, description=description, is_password=is_password
+            )
+        return self.update_for_pipeline(
+            pipeline_id=pipeline_id,
+            name=name,
+            new_name=None,
+            value=value,
+            description=description,
+            is_password=is_password,
+        )
+
+    def delete_for_pipeline(self, pipeline_id: str, name: str) -> Dict:
+        """Delete a given environment variable inside a given pipeline
+
+        Parameters
+        ----------
+        pipeline_id : str
+            UUID of your pipeline (see README on how to find it)
+        name : str
+            Name of the environment variable to delete inside the given pipeline
+
+        Returns
+        -------
+        dict
+            Dict of deleted environment variable
+
+        Raises
+        ------
+        ValueError
+            When the given name doesn't correspond to an existing environment
+            variable inside the given pipeline
+        """
+        pipeline_envs = self.list_for_pipeline(pipeline_id, pprint_result=False)
+        pipeline_env = [env for env in pipeline_envs["pipelineEnvironmentVariables"] if env["name"] == name]
+
+        if len(pipeline_env) == 0:
+            raise ValueError("❌ 'name' must be the name of an existing " "environment variable in the given pipeline")
+
+        pipeline_env_id = pipeline_env[0]["id"]
+
+        result = self.saagie_api.client.execute(query=gql(GQL_DELETE_ENV_VAR), variable_values={"id": pipeline_env_id})
+        logging.info("✅ Environment variable [%s] successfully deleted", name)
+        return result
+
+    def export(
+        self, project_id, output_folder: str, error_folder: Optional[str] = "", project_only: bool = False
+    ) -> bool:
         """Export the environment variables in a folder
 
         Parameters
         ----------
         project_id : str
             Project ID
         output_folder : str
@@ -387,15 +626,15 @@
             Path to store the project ID in case of error. If not set, project ID is not write
 
         Returns
         -------
         bool
             True if environment variables are exported False otherwise
         """
-        result = True
+
         output_folder = check_folder_path(output_folder)
         project_env_var = None
 
         try:
             project_env_var = self.list_for_project(project_id)["projectEnvironmentVariables"]
             if project_only:
                 project_env_var = [env for env in project_env_var if env["scope"] == "PROJECT"]
@@ -412,20 +651,19 @@
                 logging.info("✅ Environment variables of the project [%s] have been successfully exported", project_id)
             except Exception as exception:
                 logging.warning(
                     "❌ Environment variables of the project [%s] have not been successfully exported", project_id
                 )
                 logging.error("Something went wrong %s", exception)
                 write_error(error_folder, "env_vars", project_id)
-                result = False
-                return result
+                return False
         else:
             logging.info("✅ The project [%s] doesn't have any environment variable", project_id)
 
-        return result
+        return True
 
     def import_from_json(self, json_file: str, project_id: str = None) -> bool:
         """Import environment variables from JSON format
         Parameters
         ----------
         json_file : str
             Path to the JSON file that contains env var information
```

### Comparing `saagieapi-2.3.0/saagieapi/gql_queries.py` & `saagieapi-2.4.0/saagieapi/gql_queries.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,57 +4,85 @@
 # | |   | | | | / __| __/ _ \ '__|
 # | |___| | |_| \__ \ ||  __/ |
 #  \____|_|\__,_|___/\__\___|_|
 
 
 GQL_GET_CLUSTER_INFO = """
 {
-  getClusterCapacity {
-    cpu
-    gpu
-    memory
-  }
+    getClusterCapacity {
+        cpu
+        gpu
+        memory
+    }
 }
 """
 
+#        _       _    __
+#  _ __ | | __ _| |_ / _| ___  _ __ _ __ ___
+# | '_ \| |/ _` | __| |_ / _ \| '__| '_ ` _ \
+# | |_) | | (_| | |_|  _| (_) | |  | | | | | |
+# | .__/|_|\__,_|\__|_|  \___/|_|  |_| |_| |_|
+# |_|
+
+GQL_GET_PLATFORM_INFO = """
+{
+    platform{
+        id
+        counts{
+            projects
+            jobs
+            apps
+            pipelines
+        }
+    }
+}
+"""
+
+
 #                                 _  _                 _
 #  _ __   ___  _ __    ___   ___ (_)| |_   ___   _ __ (_)  ___  ___
 # | '__| / _ \| '_ \  / _ \ / __|| || __| / _ \ | '__|| | / _ \/ __|
 # | |   |  __/| |_) || (_) |\__ \| || |_ | (_) || |   | ||  __/\__ \
 # |_|    \___|| .__/  \___/ |___/|_| \__| \___/ |_|   |_| \___||___/
 #             |_|
 
 
 GQL_GET_REPOSITORIES_INFO = """
-  {
+{
     repositories {
-      id
-      name
-      technologies {
         id
-        label
-        available
-        __typename
-      }
+        name
+        technologies {
+            id
+            label
+            available
+            __typename
+        }
     }
-  }
+}
 """
 
 GQL_GET_RUNTIMES = """
 query technologyQuery($id: UUID!){
     technology(id: $id){ 
         __typename 
-        ... on JobTechnology {contexts{
-        id 
-        label 
-        available}}
-        ... on SparkTechnology {contexts{
-        id
-        label
-        available}}
+        ... on JobTechnology {
+            contexts{
+                id 
+                label 
+                available
+            }
+        }
+        ... on SparkTechnology {
+            contexts{
+                id
+                label
+                available
+            }
+        }
         ... on AppTechnology{
             id
             label
             available
             appContexts{
                 id
                 available
```

### Comparing `saagieapi-2.3.0/saagieapi/jobs/gql_queries.py` & `saagieapi-2.4.0/saagieapi/jobs/gql_queries.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 # pylint: disable=duplicate-code
 GQL_LIST_JOBS_FOR_PROJECT_MINIMAL = """
 query jobsQuery($projectId: UUID!){
     jobs(projectId: $projectId){
         id
         name
+        alias
     }
 }
 """
 
 GQL_LIST_JOBS_FOR_PROJECT = """
 query jobsQuery($projectId: UUID!, $category: String, $technologyId: UUID, $instancesLimit: Int, $versionsLimit: Int, $versionsOnlyCurrent: Boolean){
     jobs(projectId: $projectId, category: $category, technologyId: $technologyId){
         id
         name
+        alias
         description
         alerting{
-        emails
-        loginEmails{
-          login
-          email
-        }
-        statusList
+            emails
+            loginEmails{
+                login
+                email
+            }
+            statusList
         }
         countJobInstance
         instances(limit: $instancesLimit){
             id
             status
+            history {
+                currentStatus {
+                    status
+                    details
+                    reason
+                }
+            }
             startTime
             endTime
         }
         versions(limit: $versionsLimit, onlyCurrent: $versionsOnlyCurrent) {
             number
             creationDate
             releaseNote
@@ -78,58 +87,110 @@
             memory{
                 request
                 limit
             }
         }
     }
 }
-  """
+"""
 
 GQL_GET_JOB_INSTANCE = """
 query jobInstanceQuery($jobInstanceId: UUID!){
     jobInstance(id: $jobInstanceId){
-      id
-      number
-      status
-      startTime
-      endTime
-      jobId
-      version {
+        id
         number
-        releaseNote
-        runtimeVersion
-        commandLine
-        isMajor
-        isCurrent
-      }
+        status
+        history {
+            currentStatus {
+                status
+                details
+                reason
+            }
+        }
+        startTime
+        endTime
+        jobId
+        jobAlias
+        version {
+            number
+            releaseNote
+            runtimeVersion
+            commandLine
+            isMajor
+            isCurrent
+        }
+        executionGlobalVariablesInput{
+            key
+            value
+            isPassword
+        }
+        executionVariablesInput {
+            parentJobInstanceId
+            parentJobId
+            parentJobAlias
+            isDirectParent
+            executionVariables {
+                key
+                value
+                isPassword
+            }
+            isGlobalVariables
+        }
+        executionVariablesOutput {
+            key
+            value
+            isPassword
+        }
+        executionVariablesByKey {
+            keyVariable
+            isPassword
+            valueVariablesInputByJobInstance{
+                jobInstanceId
+                jobId
+                jobAlias
+                jobName
+                isDirectParent
+                value
+                isPassword
+            }
+            valueGlobalVariableInput
+            valueVariableOutput
+        }
     }
-  }
-  """
+}
+"""
 
 GQL_RUN_JOB = """
-  mutation runJobMutation($jobId: UUID!){
+mutation runJobMutation($jobId: UUID!){
     runJob(jobId: $jobId){
-      id
-      status
+        id
+        status
     }
-  }
-  """
+}
+"""
 
 GQL_STOP_JOB_INSTANCE = """
-  mutation stopJobInstanceMutation($jobInstanceId: UUID!){
+mutation stopJobInstanceMutation($jobInstanceId: UUID!){
     stopJobInstance(jobInstanceId: $jobInstanceId){
-      id
-      number
-      status
-      startTime
-      endTime
-      jobId
+        id
+        number
+        status
+        history {
+            currentStatus {
+                status
+                details
+                reason
+            }
+        }
+        startTime
+        endTime
+        jobId
     }
-  }
-  """
+}
+"""
 
 GQL_EDIT_JOB = """
 mutation editJobMutation($jobId: UUID!, $name: String, $description: String, 
                          $isScheduled: Boolean!, $cronScheduling: Cron, $scheduleTimezone: TimeZone,
                          $alerting: JobPipelineAlertingInput, $resources: JobResourceInput) {
     editJob(job: {
         id: $jobId
@@ -139,14 +200,15 @@
         cronScheduling: $cronScheduling
         scheduleTimezone: $scheduleTimezone
         alerting: $alerting
         resources: $resources
     }){
         id
         name
+        alias
         description
         isScheduled
         cronScheduling
         scheduleTimezone
         resources{
             cpu {
                 request
@@ -189,15 +251,16 @@
         jobVersion: {
             releaseNote: $releaseNote
             runtimeVersion: $runtimeVersion
             commandLine: $commandLine
             extraTechnology: $extraTechnology
             dockerInfo: $dockerInfo
         }
-        file: $file){
+        file: $file
+    ){
         id
         versions {
             number
             __typename
         }
         __typename
     }
@@ -214,38 +277,47 @@
             releaseNote: $releaseNote
             runtimeVersion: $runtimeVersion
             commandLine: $commandLine
             extraTechnology: $extraTechnology
             dockerInfo: $dockerInfo
             usePreviousArtifact: $usePreviousArtifact
         }
-        file: $file){
-            number
-            __typename
+        file: $file
+    ){
+        number
+        __typename
     }
 }
 """
 
 GQL_GET_JOB_INFO = """
 query jobInfoQuery($jobId: UUID!, $instancesLimit: Int, $versionsLimit: Int, $versionsOnlyCurrent: Boolean){
     job(id: $jobId){
         id
         name
+        alias
         description
         alerting{
             emails
             loginEmails{
-              login
-              email
+                login
+                email
             }
             statusList
         }
         instances(limit: $instancesLimit){
             id
             status
+            history {
+                currentStatus {
+                    status
+                    details
+                    reason
+                }
+            }
             startTime
             endTime
             version {
                 number
                 releaseNote
                 runtimeVersion
                 commandLine
```

### Comparing `saagieapi-2.3.0/saagieapi/jobs/jobs.py` & `saagieapi-2.4.0/saagieapi/jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/saagieapi/pipelines/gql_queries.py` & `saagieapi-2.4.0/saagieapi/pipelines/gql_queries.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,37 +4,46 @@
     project(id: $projectId){
         pipelines{
             id
             name
         }
     }
 }
-  """
+"""
 
 GQL_LIST_PIPELINES_FOR_PROJECT = """
-query projectPipelinesQuery($projectId: UUID!, $instancesLimit: Int, $versionsLimit: Int, $versionsOnlyCurrent: Boolean) {
+query projectPipelinesQuery($projectId: UUID!, 
+							$instancesLimit: Int, 
+                            $versionsLimit: Int, 
+                            $versionsOnlyCurrent: Boolean) {
     project(id: $projectId){
         pipelines{
             id
             name
             description
             alerting{
-              emails
-              loginEmails{
-                login
-                email
-              }
-              statusList
+                emails
+                loginEmails{
+                    login
+                    email
+                }
+                statusList
             }
             pipelineInstanceCount
             instances(limit: $instancesLimit){
-              id
-              status
-              startTime
-              endTime
+                id
+                status
+                startTime
+                endTime
+                runWithExecutionVariables
+                initialExecutionVariables{
+                    key
+                    value
+                    isPassword
+                }
             }
             versions(limit: $versionsLimit, onlyCurrent: $versionsOnlyCurrent) {
                 number
                 releaseNote
                 graph{
                     jobNodes{
                         id
@@ -66,21 +75,24 @@
             creationDate
             creator
             isScheduled
             cronScheduling
             scheduleStatus
             scheduleTimezone
             isLegacyPipeline
-          }
+        }
     }
 }
-  """
+"""
 
 GQL_GET_PIPELINE = """
-query graphPipelineQuery($id: UUID!, $instancesLimit: Int, $versionsLimit: Int, $versionsOnlyCurrent: Boolean) {
+query graphPipelineQuery($id: UUID!, 
+						 $instancesLimit: Int, 
+                         $versionsLimit: Int, 
+                         $versionsOnlyCurrent: Boolean) {
     graphPipeline(id: $id){
         id
         name
         description
         alerting{
             emails
             loginEmails{
@@ -91,14 +103,20 @@
         }
         pipelineInstanceCount
         instances(limit: $instancesLimit){
             id
             status
             startTime
             endTime
+            runWithExecutionVariables
+            initialExecutionVariables{
+                key
+                value
+                isPassword
+            }
         }
         versions(limit: $versionsLimit, onlyCurrent: $versionsOnlyCurrent) {
             number
             releaseNote
             graph{
                 jobNodes{
                     id
@@ -130,145 +148,171 @@
         creationDate
         creator
         isScheduled
         cronScheduling
         scheduleStatus
         scheduleTimezone
         isLegacyPipeline
+        hasExecutionVariablesEnabled
     }
 }
-  """
+"""
 
 GQL_STOP_PIPELINE_INSTANCE = """
 mutation stopPipelineInstanceMutation($pipelineInstanceId: UUID!){
     stopPipelineInstance(pipelineInstanceId: $pipelineInstanceId){
-      id
-      number
-      status
-      startTime
-      endTime
-      pipelineId
+        id
+        number
+        status
+        startTime
+        endTime
+        pipelineId
     }
 }
-  """
+"""
 
 GQL_EDIT_PIPELINE = """
-  mutation($id: UUID!, $name: String, $description: String, $alerting: JobPipelineAlertingInput,
-          $isScheduled: Boolean, $cronScheduling: Cron, $scheduleTimezone:TimeZone)  {
-    editPipeline(pipeline: {
-        id: $id
-        name: $name
-        description: $description
-        alerting:  $alerting
-        isScheduled: $isScheduled
-        cronScheduling: $cronScheduling
-        scheduleTimezone: $scheduleTimezone
-      })
-    {
-      id
-      name
-      description
-      alerting{
-        emails
-        statusList
-      }
-      isScheduled
-      cronScheduling
-      scheduleTimezone
+mutation($id: UUID!, 
+		 $name: String, 
+		 $description: String, 
+		 $alerting: JobPipelineAlertingInput,
+		 $isScheduled: Boolean, 
+		 $cronScheduling: Cron, 
+		 $scheduleTimezone:TimeZone, 
+		 $hasExecutionVariablesEnabled: Boolean)    {
+    editPipeline(pipeline: 
+        {
+            id: $id
+            name: $name
+            description: $description
+            alerting:    $alerting
+            isScheduled: $isScheduled
+            cronScheduling: $cronScheduling
+            scheduleTimezone: $scheduleTimezone
+            hasExecutionVariablesEnabled: $hasExecutionVariablesEnabled
+        }
+    ){
+        id
+        name
+        description
+        alerting{
+            emails
+            statusList
+        }
+        isScheduled
+        cronScheduling
+        scheduleTimezone
+        hasExecutionVariablesEnabled
     }
-  }
+}
 """
 
 GQL_RUN_PIPELINE = """
 mutation runPipelineMutation($pipelineId: UUID!){
     runPipeline(pipelineId: $pipelineId){
-      id
-      status
+        id
+        status
     }
-  }
+}
 """
 
 GQL_GET_PIPELINE_INSTANCE = """
 query pipelineInstanceQuery($id: UUID!){
     pipelineInstance(id: $id){
-          id
-          status
-          startTime
-          endTime
+        id
+        status
+        startTime
+        endTime
+        runWithExecutionVariables
+        initialExecutionVariables{
+            key
+            value
+            isPassword
+        }
     }
 }
 """
 
 GQL_CREATE_GRAPH_PIPELINE = """
-mutation createGraphPipelineMutation($name: String!, $description: String, $projectId: UUID!,
-                                     $releaseNote: String, $alerting: JobPipelineAlertingInput,
-                                     $isScheduled: Boolean!, $cronScheduling: Cron, $scheduleTimezone:TimeZone,
-                                     $jobNodes: [JobNodeInput!], $conditionNodes: [ConditionNodeInput!]) {
-  createGraphPipeline(pipeline:  {
-    name: $name
-    description: $description
-    projectId: $projectId
-    releaseNote : $releaseNote
-    alerting: $alerting
-    isScheduled: $isScheduled
-    cronScheduling: $cronScheduling
-    scheduleTimezone: $scheduleTimezone
-    graph: {
-        jobNodes: $jobNodes
-        conditionNodes: $conditionNodes
-    }
-  }
-  ) {
-    id
-  }
+mutation createGraphPipelineMutation($name: String!, 
+									 $description: String, 
+                                     $projectId: UUID!,
+									 $releaseNote: String, 
+                                     $alerting: JobPipelineAlertingInput,
+                                     $isScheduled: Boolean!, 
+                                     $cronScheduling: Cron, 
+                                     $scheduleTimezone:TimeZone,
+                                     $jobNodes: [JobNodeInput!], 
+                                     $conditionNodes: [ConditionNodeInput!]) {
+    createGraphPipeline(pipeline:    {
+        name: $name
+        description: $description
+        projectId: $projectId
+        releaseNote : $releaseNote
+        alerting: $alerting
+        isScheduled: $isScheduled
+        cronScheduling: $cronScheduling
+        scheduleTimezone: $scheduleTimezone
+        graph: {
+            jobNodes: $jobNodes
+            conditionNodes: $conditionNodes
+        }
+    }
+    ) {
+        id
+    }
 }
 """
 
 GQL_DELETE_PIPELINE = """
 mutation deletePipelineMutation($id: UUID!){
-  deletePipeline (
-    id: $id
-  )
+    deletePipeline (
+        id: $id
+    )
 }
 """
 
 GQL_UPGRADE_PIPELINE = """
-  mutation($id: UUID!, $jobNodes: [JobNodeInput!], $conditionNodes: [ConditionNodeInput!], $releaseNote: String){
-  addGraphPipelineVersion(
-    pipelineId: $id,
-    graph: {jobNodes: $jobNodes,
-                conditionNodes: $conditionNodes},
-    releaseNote: $releaseNote
-    )
-    {
-      number,
-      releaseNote,
-      graph{
-        jobNodes {
-          id,
-          job {
-            id
-          }
+mutation($id: UUID!, 
+		 $jobNodes: [JobNodeInput!], 
+         $conditionNodes: [ConditionNodeInput!], 
+         $releaseNote: String){
+    addGraphPipelineVersion(
+        pipelineId: $id,
+        graph: {
+            jobNodes: $jobNodes,
+            conditionNodes: $conditionNodes
         },
-        conditionNodes{
-          id
-        }
-      },
-      creationDate,
-      creator,
-      isCurrent,
-      isMajor
+        releaseNote: $releaseNote
+    ){
+        number,
+        releaseNote,
+        graph{
+            jobNodes {
+                id,
+                job {
+                    id
+                }
+            },
+            conditionNodes{
+                id
+            }
+        },
+        creationDate,
+        creator,
+        isCurrent,
+        isMajor
     }
-  }
+}
 """
 
 GQL_ROLLBACK_PIPELINE_VERSION = """
 mutation rollbackPipelineVersionMutation($pipelineId: UUID!, $versionNumber: Int!) {
-  rollbackPipelineVersion(pipelineId: $pipelineId, versionNumber: $versionNumber) {
-    id
-    versions {
-      number
-      isCurrent
+    rollbackPipelineVersion(pipelineId: $pipelineId, versionNumber: $versionNumber) {
+        id
+        versions {
+            number
+            isCurrent
+        }
     }
-  }
 }
 """
```

### Comparing `saagieapi-2.3.0/saagieapi/pipelines/graph_pipeline.py` & `saagieapi-2.4.0/saagieapi/pipelines/graph_pipeline.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/saagieapi/pipelines/pipelines.py` & `saagieapi-2.4.0/saagieapi/pipelines/pipelines.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         pprint_result : bool, optional
             Whether to pretty print the result of the query, default to
             saagie_api.pprint_global
 
         Returns
         -------
         dict
-            Dict of job information
+            Dict of pipeline information
         """
         return self.saagie_api.client.execute(
             query=gql(GQL_GET_PIPELINE_INSTANCE),
             variable_values={"id": pipeline_instance_id},
             pprint_result=pprint_result,
         )
 
@@ -167,14 +167,15 @@
         graph_pipeline: GraphPipeline,
         description: str = "",
         release_note: str = "",
         emails: List[str] = None,
         status_list: List[str] = None,
         cron_scheduling: str = None,
         schedule_timezone: str = "UTC",
+        has_execution_variables_enabled: bool = None,
     ) -> Dict:
         """
         Create a pipeline in a given project
 
         Parameters
         ----------
         name : str
@@ -199,14 +200,16 @@
             Receive an email when the job status change to a specific status
             Each item of the list should be one of these following values: "REQUESTED", "QUEUED",
             "RUNNING", "FAILED", "KILLED", "KILLING", "SUCCEEDED", "UNKNOWN", "AWAITING", "SKIPPED"
         cron_scheduling : str, optional
             Scheduling CRON format
         schedule_timezone : str, optional
             Timezone of the scheduling
+        has_execution_variables_enabled: bool, optional
+            Boolean to activate or desactivate the execution variables
 
         Returns
         -------
         dict
             Dict of pipeline information
         """
         if not graph_pipeline.list_job_nodes:
@@ -219,20 +222,23 @@
             "releaseNote": release_note,
             "jobNodes": graph_pipeline.list_job_nodes,
             "conditionNodes": graph_pipeline.list_conditions_nodes,
         }
 
         if cron_scheduling:
             params = self.saagie_api.check_scheduling(cron_scheduling, params, schedule_timezone)
-
         else:
             params["isScheduled"] = False
+
         if emails:
             params = self.saagie_api.check_alerting(emails, params, status_list)
 
+        if has_execution_variables_enabled:
+            params["hasExecutionVariablesEnabled"] = has_execution_variables_enabled
+
         result = self.saagie_api.client.execute(query=gql(GQL_CREATE_GRAPH_PIPELINE), variable_values=params)
         logging.info("✅ Pipeline [%s] successfully created", name)
         return result
 
     def delete(self, pipeline_id: str) -> Dict:
         """Delete a pipeline given pipeline id
 
@@ -287,15 +293,16 @@
         name: str = None,
         description: str = None,
         emails: List[str] = None,
         status_list: List[str] = None,
         is_scheduled: bool = None,
         cron_scheduling: str = None,
         schedule_timezone: str = "UTC",
-    ):
+        has_execution_variables_enabled: bool = None,
+    ) -> Dict:
         # pylint: disable=singleton-comparison
         """Edit a pipeline
         NB : You can only edit pipeline if you have at least the editor role on
         the project
 
         Parameters
         ----------
@@ -322,56 +329,57 @@
             Emails to receive alerts for the job, each item should be a valid email,
             If you want to remove alerting, please set emails to [] or list()
             if not filled, defaults to current value
         status_list: List[String], optional
             Receive an email when the job status change to a specific status
             Each item of the list should be one of these following values: "REQUESTED", "QUEUED",
             "RUNNING", "FAILED", "KILLED", "KILLING", "SUCCEEDED", "UNKNOWN", "AWAITING", "SKIPPED"
+        has_execution_variables_enabled: bool, optional
+            Boolean to activate or desactivate the execution variables
 
         Returns
         -------
         dict
             Dict of pipeline information
         """
-        params = {"id": pipeline_id}
         previous_pipeline_info = self.get_info(pipeline_id, pprint_result=False)["graphPipeline"]
 
-        if name:
-            params["name"] = name
-        else:
-            params["name"] = previous_pipeline_info["name"]
-
-        if description:
-            params["description"] = description
-        else:
-            params["description"] = previous_pipeline_info["description"]
+        params = {
+            "id": pipeline_id,
+            "name": name or previous_pipeline_info["name"],
+            "description": description or previous_pipeline_info["description"],
+        }
 
+        # cases test : True, False and None
         if is_scheduled:
             params = self.saagie_api.check_scheduling(cron_scheduling, params, schedule_timezone)
-
         elif is_scheduled == False:
             params["isScheduled"] = False
-
         else:
-            params["isScheduled"] = previous_pipeline_info["isScheduled"]
-            params["cronScheduling"] = previous_pipeline_info["cronScheduling"]
-            params["scheduleTimezone"] = previous_pipeline_info["scheduleTimezone"]
+            for k in ["isScheduled", "cronScheduling", "scheduleTimezone"]:
+                params[k] = previous_pipeline_info[k]
 
-        if emails:
+        # cases test : List non empty, List empty, None
+        if isinstance(emails, List) and emails:
             params = self.saagie_api.check_alerting(emails, params, status_list)
         elif isinstance(emails, List):
             params["alerting"] = None
         else:
             previous_alerting = previous_pipeline_info["alerting"]
             if previous_alerting:
                 params["alerting"] = {
                     "emails": previous_alerting["emails"],
                     "statusList": previous_alerting["statusList"],
                 }
 
+        if has_execution_variables_enabled in {True, False}:
+            params["hasExecutionVariablesEnabled"] = has_execution_variables_enabled
+        else:
+            params["hasExecutionVariablesEnabled"] = previous_pipeline_info["hasExecutionVariablesEnabled"]
+
         result = self.saagie_api.client.execute(query=gql(GQL_EDIT_PIPELINE), variable_values=params)
         logging.info("✅ Pipeline [%s] successfully edited", name)
         return result
 
     def create_or_upgrade(
         self,
         name: str,
@@ -380,14 +388,15 @@
         description: str = "",
         release_note: str = "",
         emails: List[str] = None,
         status_list: List[str] = None,
         is_scheduled: bool = None,
         cron_scheduling: str = None,
         schedule_timezone: str = "UTC",
+        has_execution_variables_enabled: bool = None,
     ) -> Dict:
         """Create or upgrade a pipeline in a given project
 
         Parameters
         ----------
         name : str
             Pipeline name
@@ -420,14 +429,16 @@
             Scheduling CRON format
             When is_scheduled is set to True, it will be mandatory to fill this value
             if not filled, defaults to current value
             Example: "0 0 * * *" (for every day At 00:00)
         schedule_timezone : str, optional
             Timezone of the scheduling
             Example: "UTC", "Pacific/Pago_Pago"
+        has_execution_variables_enabled: bool, optional
+            Boolean to activate or desactivate the execution variables
 
         Returns
         -------
         dict
             Dict of pipeline information
         """
         pipeline_list = self.saagie_api.pipelines.list_for_project_minimal(project_id)["project"]["pipelines"]
@@ -442,14 +453,15 @@
                 name,
                 description,
                 emails,
                 status_list,
                 is_scheduled,
                 cron_scheduling,
                 schedule_timezone,
+                has_execution_variables_enabled,
             )["editPipeline"]
 
             responses["addGraphPipelineVersion"] = self.upgrade(pipeline_id, graph_pipeline, release_note)[
                 "addGraphPipelineVersion"
             ]
 
             return responses
@@ -460,17 +472,18 @@
             graph_pipeline,
             description,
             release_note,
             emails,
             status_list,
             cron_scheduling,
             schedule_timezone,
+            has_execution_variables_enabled,
         )
 
-    def rollback(self, pipeline_id: str, version_number: str):
+    def rollback(self, pipeline_id: str, version_number: str) -> Dict:
         """Rollback a given job to the given version
 
         Parameters
         ----------
         pipeline_id : str
             UUID of your pipeline (see README on how to find it)
         version_number : str
```

### Comparing `saagieapi-2.3.0/saagieapi/projects/gql_queries.py` & `saagieapi-2.4.0/saagieapi/projects/gql_queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # pylint: disable=duplicate-code
 GQL_LIST_PROJECTS = """
-  {
-       projects{
-          id,
-          name,
-          creator,
-          description,
-          jobsCount,
-          status
-      }
-  }
-  """
+{
+    projects{
+        id,
+        name,
+        creator,
+        description,
+        jobsCount,
+        status
+    }
+}
+"""
 
 GQL_GET_PROJECT_INFO = """
 query projectQuery($id: UUID!) {
     project(id: $id){
         name
         creator
         description
@@ -38,77 +38,88 @@
 }
 """
 
 GQL_GET_PROJECT_APPS_TECHNOLOGIES = """
 query appTechnologiesQuery($id: UUID!) {
     project(id: $id){
         appTechnologies{
-                id
+            id
         }
     }
 }
 """
 
 GQL_CREATE_PROJECT = """
-mutation createProjectMutation($name: String!, $description: String, $technologies: [TechnologyInput!],
-                                $appTechnologies: [TechnologyInput!], $authorizedGroups: [SecurityGroupInput]) {
-  createProject(project: {
-                    name: $name
-                    description: $description
-                    authorizedGroups:  $authorizedGroups
-                    technologiesByCategory: [
-                      {
-                        jobCategory: "Extraction",
-                        technologies: $technologies
-                      },
-                      {
-                        jobCategory: "Processing",
-                        technologies: $technologies
-                      }
-                    ]
-                    appTechnologies: $appTechnologies
-                }) {
-    id
-    name
-    creator
-  }
+mutation createProjectMutation($name: String!, 
+                               $description: String, 
+                               $technologies: [TechnologyInput!],
+                               $appTechnologies: [TechnologyInput!], 
+                               $authorizedGroups: [SecurityGroupInput]) {
+    createProject(
+        project: {
+            name: $name
+            description: $description
+            authorizedGroups:  $authorizedGroups
+            technologiesByCategory: [
+                {
+                    jobCategory: "Extraction",
+                    technologies: $technologies
+                },
+                {
+                    jobCategory: "Processing",
+                    technologies: $technologies
+                }
+            ]
+            appTechnologies: $appTechnologies
+        }
+    ) {
+        id
+        name
+        creator
+    }
 }
 """
 
 
 GQL_DELETE_PROJECT = """
 mutation deleteProjectMutation($projectId: UUID!){
     deleteProject(projectId: $projectId)
 }
 """
 
 GQL_EDIT_PROJECT = """
-mutation editProjectMutation($projectId: UUID!, $name: String, $description: String, $technologies: [TechnologyInput!], 
-                             $appTechnologies: [TechnologyInput!], $authorizedGroups: [SecurityGroupInput]) {
-  editProject(project: {
-                    id : $projectId
-                    name: $name
-                    description: $description
-                    authorizedGroups:  $authorizedGroups
-                    technologiesByCategory: [
-                      {
-                        jobCategory: "Extraction",
-                        technologies: $technologies
-                      },
-                      {
-                        jobCategory: "Processing",
-                        technologies: $technologies
-                      }
-                    ]
-                    appTechnologies: $appTechnologies
-                }) {
-    id
-    name
-    creator
-  }
+mutation editProjectMutation($projectId: UUID!, 
+                             $name: String, 
+                             $description: String, 
+                             $technologies: [TechnologyInput!], 
+                             $appTechnologies: [TechnologyInput!], 
+                             $authorizedGroups: [SecurityGroupInput]) {
+    editProject(
+        project: {
+            id : $projectId
+            name: $name
+            description: $description
+            authorizedGroups:  $authorizedGroups
+            technologiesByCategory: [
+                {
+                    jobCategory: "Extraction",
+                    technologies: $technologies
+                },
+                {
+                    jobCategory: "Processing",
+                    technologies: $technologies
+                }
+            ]
+            appTechnologies: $appTechnologies
+        }
+    ) {
+        id
+        name
+        creator
+    }
 }
 """
 
 GQL_GET_PROJECT_RIGHTS = """
 query rightsQuery($id: UUID!) {
     rights(projectId: $id){
         name
```

### Comparing `saagieapi-2.3.0/saagieapi/projects/projects.py` & `saagieapi-2.4.0/saagieapi/projects/projects.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/saagieapi/repositories/gql_queries.py` & `saagieapi-2.4.0/saagieapi/repositories/gql_queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,333 +1,333 @@
 GQL_LIST_REPOSITORIES = """
 query repsositoriesQuery($minimal: Boolean!, $lastSynchronization: Boolean) {
-  repositories {
-    id
-    name
-    synchronizationReports(lastSynchronization: $lastSynchronization) {
-      lastReversibleId
-      ...reportInformations @skip(if: $minimal)
+    repositories {
+        id
+        name
+        synchronizationReports(lastSynchronization: $lastSynchronization) {
+            lastReversibleId
+            ...reportInformations @skip(if: $minimal)
+        }
+        ...repositoryInformations @skip(if: $minimal)
     }
-    ...repositoryInformations @skip(if: $minimal)
-  }
 }
 
 fragment repositoryInformations on Repository {
     technologies {
-      available
-      id
-      label
+        available
+        id
+        label
     }
     source {
-      ... on UrlSource {
-        url
-      }
-      ... on FileSource {
-        name
-      }
+        ... on UrlSource {
+            url
+        }
+        ... on FileSource {
+            name
+        }
     }
 }
 
 fragment reportInformations on SynchronizationReports {
     count
-      list {
+    list {
         endedAt
         ... on SuccessfulSynchronization {
-          endedAt
-          issues {
-            message
-            path
-          }
-          revert {
-            date
-            author
-          }
+            endedAt
+            issues {
+                message
+                path
+            }
+            revert {
+                date
+                author
+            }
         }
         ... on FailedSynchronization {
-          failure
+            failure
         }
-      }
+    }
 }
 """
 
 
 GQL_CREATE_REPOSITORY = """
 mutation addRepositoryMutation(
-  $repositoryInput: RepositoryInput!
-  $upload: Upload
+    $repositoryInput: RepositoryInput!
+    $upload: Upload
 ) {
-  addRepository(repositoryInput: $repositoryInput, upload: $upload) {
-    count
-    objects {
-      id
-      name
+    addRepository(repositoryInput: $repositoryInput, upload: $upload) {
+        count
+        objects {
+            id
+            name
+        }
     }
-  }
 }
 """
 
 GQL_DELETE_REPOSITORY = """
 mutation RemoveRepository($removeRepositoryId: UUID!) {
-  removeRepository(id: $removeRepositoryId) {
-    id
-    name
-  }
+    removeRepository(id: $removeRepositoryId) {
+        id
+        name
+    }
 }
 """
 
 GQL_EDIT_REPOSITORY = """
 mutation editRepositoryMutation($repositoryInput: RepositoryEditionInput!) {
-  editRepository(repositoryInput: $repositoryInput) {
-    count
-    objects {
-      name
-      source {
-        ... on UrlSource {
-          url
-        }
-        ... on FileSource {
-          name
+    editRepository(repositoryInput: $repositoryInput) {
+        count
+        objects {
+            name
+            source {
+                ... on UrlSource {
+                    url
+                }
+                ... on FileSource {
+                    name
+                }
+            }
+            id
         }
-      }
-      id
     }
-  }
 }
 """
 
 GQL_SYNCHRONIZE_REPOSITORY = """
 mutation synchronizeRepository($id: UUID!, $upload: Upload) {
-  synchronizeRepository(id: $id, upload: $upload) {
-    count
-    report {
-      id
-      endedAt
-      startedAt
-      trigger {
-        author
-        type
-      }
-      ... on SuccessfulSynchronization {
-        technologyReports {
-          status
-          technologyId
-        }
-        issues {
-          message
-          path
-        }
-      }
-      ... on FailedSynchronization {
-        failure
-      }
+    synchronizeRepository(id: $id, upload: $upload) {
+        count
+        report {
+            id
+            endedAt
+            startedAt
+            trigger {
+                author
+                type
+            }
+            ... on SuccessfulSynchronization {
+                technologyReports {
+                    status
+                    technologyId
+                }
+                issues {
+                    message
+                    path
+                }
+            }
+            ... on FailedSynchronization {
+                failure
+            }
+        }
+        repositoryId
+        repositoryName
     }
-    repositoryId
-    repositoryName
-  }
 }
 """
 
 GQL_REVERT_LAST_SYNCHRONISATION = """
 mutation revertLastSynchronization($repositoryId: UUID!, $synchronizationReportId: UUID!) {
-  revertLastSynchronization(repositoryId: $repositoryId, synchronizationReportId: $synchronizationReportId) {
-    report {
-      id
-      trigger {
-        author
-        type
-      }
-      endedAt
-      startedAt
+    revertLastSynchronization(repositoryId: $repositoryId, synchronizationReportId: $synchronizationReportId) {
+        report {
+            id
+            trigger {
+                author
+                type
+            }
+            endedAt
+            startedAt
+        }
+        repositoryName
+        repositoryId
     }
-    repositoryName
-    repositoryId
-  }
 }
 """
 
 GQL_GET_REPOSITORY_INFO = """
 query RepositoryQuery($id: UUID!, $withReverted: Boolean, $lastSynchronization: Boolean, $limit: Int) {
-  repository(id: $id) {
-    creationDate
-    creator
-    editor
-    id
-    modificationDate
-    name
-    readOnly
-    source {
-      ... on UrlSource {
-        url
-      }
-      ... on FileSource {
+    repository(id: $id) {
+        creationDate
+        creator
+        editor
+        id
+        modificationDate
         name
-      }
-    }
-    synchronizationReports(limit: $limit, withReverted: $withReverted, lastSynchronization: $lastSynchronization) {
-      count
-      list {
+        readOnly
         source {
-          ... on UrlSource {
-            url
-          }
-          ... on FileSource {
-            name
-          }
-        }
-        ... on SuccessfulSynchronization {
-          endedAt
-          startedAt
-          trigger {
-            author
-            type
-          }
-          technologyReports {
-            status
-            technologyId
-            message
-          }
-          issues {
-            message
-            path
-          }
-          revert {
-            author
-            date
-          }
+            ... on UrlSource {
+                url
+            }
+            ... on FileSource {
+                name
+            }
         }
-        ... on FailedSynchronization {
-          endedAt
-          startedAt
-          trigger {
-            author
-            type
-          }
-          failure
+        synchronizationReports(limit: $limit, withReverted: $withReverted, lastSynchronization: $lastSynchronization) {
+            count
+            list {
+                source {
+                    ... on UrlSource {
+                        url
+                    }
+                    ... on FileSource {
+                        name
+                    }
+                }
+                ... on SuccessfulSynchronization {
+                    endedAt
+                    startedAt
+                    trigger {
+                        author
+                        type
+                    }
+                    technologyReports {
+                        status
+                        technologyId
+                        message
+                    }
+                    issues {
+                        message
+                        path
+                    }
+                    revert {
+                        author
+                        date
+                    }
+                }
+                ... on FailedSynchronization {
+                    endedAt
+                    startedAt
+                    trigger {
+                        author
+                        type
+                    }
+                    failure
+                }
+            }
+            lastReversibleId
         }
-      }
-      lastReversibleId
-    }
-    connectionTypes {
-      id
-      label
-      actions {
-        checkConnection {
-          scriptId
+        connectionTypes {
+            id
+            label
+            actions {
+                checkConnection {
+                    scriptId
+                }
+            }
         }
-      }
-    }
-    technologies {
-      id
-      technologyId
-      label
-      icon
-      repositoryId
-      available
-      missingFacets
-      description
-      ... on AppTechnology {
-        appContexts {
-          id
-          label
-          available
-          missingFacets
-          recommended
-          description
-          dockerInfo {
-            image
-            version
-          }
-          trustLevel
-          deprecationDate
-          lastUpdate
-        }
-      }
-      ... on JobTechnology {
-        contexts {
-          id
-          label
-          available
-          missingFacets
-          description
-          recommended
-          dockerInfo {
-            image
-            version
-          }
-          trustLevel
-          deprecationDate
-          lastUpdate
-        }
-      }
-      ... on ExtJobTechnology {
-        iconUrl
-        contexts {
-          id
-          label
-          available
-          missingFacets
-          description
-          recommended
-          trustLevel
-          deprecationDate
-          lastUpdate
-          connectionTypeUUID
-          actions {
-            getStatus {
-              scriptId
-            }
-            start {
-              scriptId
-            }
-            stop {
-              scriptId
-            }
-            getLogs {
-              scriptId
-            }
-          }
-        }
-      }
-      ... on SparkTechnology {
-        contexts {
-          id
-          label
-          available
-          missingFacets
-          description
-          recommended
-          trustLevel
-          deprecationDate
-          dockerInfo {
-            image
-            version
-          }
-          technologyContexts {
+        technologies {
+            id
+            technologyId
+            label
+            icon
+            repositoryId
             available
             missingFacets
             description
-            id
-            label
-            recommended
-            trustLevel
-            deprecationDate
-            jobContexts {
-              available
-              description
-              dockerInfo {
-                image
-                version
-              }
-              id
-              label
-              recommended
-              trustLevel
-              deprecationDate
-              lastUpdate
+            ... on AppTechnology {
+                appContexts {
+                    id
+                    label
+                    available
+                    missingFacets
+                    recommended
+                    description
+                    dockerInfo {
+                        image
+                        version
+                    }
+                    trustLevel
+                    deprecationDate
+                    lastUpdate
+                }
+            }
+            ... on JobTechnology {
+                contexts {
+                    id
+                    label
+                    available
+                    missingFacets
+                    description
+                    recommended
+                    dockerInfo {
+                        image
+                        version
+                    }
+                    trustLevel
+                    deprecationDate
+                    lastUpdate
+                }
+            }
+            ... on ExtJobTechnology {
+                iconUrl
+                contexts {
+                    id
+                    label
+                    available
+                    missingFacets
+                    description
+                    recommended
+                    trustLevel
+                    deprecationDate
+                    lastUpdate
+                    connectionTypeUUID
+                    actions {
+                        getStatus {
+                            scriptId
+                        }
+                        start {
+                            scriptId
+                        }
+                        stop {
+                            scriptId
+                        }
+                        getLogs {
+                            scriptId
+                        }
+                    }
+                }
+            }
+            ... on SparkTechnology {
+                contexts {
+                    id
+                    label
+                    available
+                    missingFacets
+                    description
+                    recommended
+                    trustLevel
+                    deprecationDate
+                    dockerInfo {
+                        image
+                        version
+                    }
+                    technologyContexts {
+                        available
+                        missingFacets
+                        description
+                        id
+                        label
+                        recommended
+                        trustLevel
+                        deprecationDate
+                        jobContexts {
+                            available
+                            description
+                            dockerInfo {
+                                image
+                                version
+                            }
+                            id
+                            label
+                            recommended
+                            trustLevel
+                            deprecationDate
+                            lastUpdate
+                        }
+                    }
+                }
             }
-          }
         }
-      }
     }
-  }
 }
 """
```

### Comparing `saagieapi-2.3.0/saagieapi/repositories/repositories.py` & `saagieapi-2.4.0/saagieapi/repositories/repositories.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/saagieapi/saagie_api.py` & `saagieapi-2.4.0/saagieapi/saagie_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pytz
 from croniter import croniter
 from gql import gql
 
 from .apps import Apps
 from .docker_credentials import DockerCredentials
 from .env_vars import EnvVars
-from .gql_queries import GQL_GET_CLUSTER_INFO, GQL_GET_REPOSITORIES_INFO, GQL_GET_RUNTIMES
+from .gql_queries import GQL_GET_CLUSTER_INFO, GQL_GET_PLATFORM_INFO, GQL_GET_REPOSITORIES_INFO, GQL_GET_RUNTIMES
 from .jobs import Jobs
 from .pipelines import Pipelines
 from .projects import Projects
 from .repositories import Repositories
 from .storages import Storages
 from .utils.bearer_auth import BearerAuth
 from .utils.gql_client import GqlClient
@@ -56,15 +56,15 @@
 
         self.url_saagie = url_saagie
         self.auth = BearerAuth(realm=realm, url=self.url_saagie, platform=id_platform, login=user, password=password)
         logging.info("✅ Successfully connected to your platform %s", self.url_saagie)
         url_api = f"{self.url_saagie}projects/api/platform/{str(id_platform)}/graphql"
         self.client = GqlClient(auth=self.auth, api_endpoint=url_api, retries=retries)
 
-        url_gateway = self.url_saagie + "gateway/api/graphql"
+        url_gateway = f"{self.url_saagie}gateway/api/graphql"
         self.client_gateway = GqlClient(auth=self.auth, api_endpoint=url_gateway, retries=retries)
 
         self.projects = Projects(self)
         self.jobs = Jobs(self)
         self.pipelines = Pipelines(self)
         self.env_vars = EnvVars(self)
         self.apps = Apps(self)
@@ -203,14 +203,29 @@
         dict
             Dict of cluster resources
         """
         query = gql(GQL_GET_CLUSTER_INFO)
         return self.client.execute(query)
 
     # ##########################################################
+    # ###                    platform                       ####
+    # ##########################################################
+
+    def get_platform_info(self) -> Dict:
+        """
+        Get platform info (nb projects, jobs, apps, pipelines)
+        Returns
+        -------
+        dict
+            Dict of platform info
+        """
+        query = gql(GQL_GET_PLATFORM_INFO)
+        return self.client.execute(query)
+
+    # ##########################################################
     # ###                    repositories                   ####
     # ##########################################################
 
     def get_repositories_info(self) -> Dict:
         """
         Get information for all repositories (id, name, technologies)
         NB: You can only get repositories information if you have the right to
@@ -398,12 +413,9 @@
         Returns
         -------
         dict
             String of runtime label
 
         """
         runtimes = self.get_runtimes(technology_id)
-        runtime_label = [
-            runtime["label"] for runtime in runtimes["technology"]["appContexts"] if runtime["id"] == runtime_id
-        ]
 
-        return runtime_label
+        return [runtime["label"] for runtime in runtimes["technology"]["appContexts"] if runtime["id"] == runtime_id]
```

### Comparing `saagieapi-2.3.0/saagieapi/storages/gql_queries.py` & `saagieapi-2.4.0/saagieapi/storages/gql_queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 # pylint: disable=duplicate-code
 GQL_LIST_STORAGE_FOR_PROJECT = """
 fragment appVersionFieldInformation on AppVersion {
-  number
-  volumesWithPath {
-    path
-    volume {
-      id
+    number
+    volumesWithPath {
+        path
+        volume {
+            id
+        }
     }
-  }
 }
 
 fragment volumeInformation on Volume {
-  size
-  description
-  creationDate
-  creator
-  linkedApp {
-    id
-    name
-    versions {
-      ...appVersionFieldInformation
-    }
-    currentVersion {
-      ...appVersionFieldInformation
+    size
+    description
+    creationDate
+    creator
+    linkedApp {
+        id
+        name
+        versions {
+            ...appVersionFieldInformation
+        }
+        currentVersion {
+            ...appVersionFieldInformation
+        }
     }
-  }
 }
 
 query projectQuery($id: UUID!, $minimal: Boolean!) {
-  project(id: $id) {
-    volumes {
-      id
-      name
-      ...volumeInformation @skip(if: $minimal)
+    project(id: $id) {
+        volumes {
+            id
+            name
+            ...volumeInformation @skip(if: $minimal)
+        }
     }
-  }
 }
 """
 
 GQL_CREATE_STORAGE = """
 mutation createVolumeMutation($volume: VolumeInput!) {
-  createVolume(volume: $volume) {
-    id
-    name
-    description
-    size
-    creator
-    linkedApp {
-      id
+    createVolume(volume: $volume) {
+        id
+        name
+        description
+        size
+        creator
+        linkedApp {
+            id
+        }
     }
-  }
 }
 """
 
 GQL_EDIT_STORAGE = """
 mutation editVolumeMutation($volume: VolumeEditionInput!) {
-  editVolume(volumeEdition: $volume) {
-    id
-    name
-  }
+    editVolume(volumeEdition: $volume) {
+        id
+        name
+    }
 }
 """
 
 GQL_DELETE_STORAGE = """
 mutation deleteVolumeMutation($id: UUID!) {
     deleteVolume(id: $id) {
         id
         name
     }
 }
 """
 
 GQL_UNLINK_STORAGE = """
 mutation unlinkVolumeMutation($id: UUID!) {
-  unlinkVolume(id: $id) {
-    id
-    name
-  }
+    unlinkVolume(id: $id) {
+        id
+        name
+    }
 }
 """
```

### Comparing `saagieapi-2.3.0/saagieapi/storages/storages.py` & `saagieapi-2.4.0/saagieapi/storages/storages.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/saagieapi/utils/bearer_auth.py` & `saagieapi-2.4.0/saagieapi/utils/bearer_auth.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/saagieapi/utils/folder_functions.py` & `saagieapi-2.4.0/saagieapi/utils/folder_functions.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/saagieapi/utils/gql_client.py` & `saagieapi-2.4.0/saagieapi/utils/gql_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.3.0/PKG-INFO` & `saagieapi-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saagieapi
-Version: 2.3.0
+Version: 2.4.0
 Summary: Python API to interact with Saagie
 Home-page: https://github.com/saagie/api-saagie
 License: GLWTPL
 Author: Saagie
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

