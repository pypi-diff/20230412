# Comparing `tmp/umapi-client-2.8.tar.gz` & `tmp/umapi-client-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/umapi-client-2.8.tar", last modified: Wed Oct 18 21:53:15 2017, max compression
+gzip compressed data, was "dist/umapi-client-2.9.tar", last modified: Wed Nov 15 01:47:38 2017, max compression
```

## Comparing `umapi-client-2.8.tar` & `umapi-client-2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-10-18 21:53:15.000000 umapi-client-2.8/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-10-18 21:53:15.000000 umapi-client-2.8/umapi_client/
--rw-r--r--   0 travis    (2000) travis    (2000)     1553 2017-10-18 21:51:30.000000 umapi-client-2.8/umapi_client/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)    10469 2017-10-18 21:51:30.000000 umapi-client-2.8/umapi_client/api.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3803 2017-10-18 21:51:30.000000 umapi-client-2.8/umapi_client/auth.py
--rw-r--r--   0 travis    (2000) travis    (2000)    22940 2017-10-18 21:51:30.000000 umapi-client-2.8/umapi_client/connection.py
--rw-r--r--   0 travis    (2000) travis    (2000)     2589 2017-10-18 21:51:30.000000 umapi-client-2.8/umapi_client/error.py
--rw-r--r--   0 travis    (2000) travis    (2000)    21318 2017-10-18 21:51:30.000000 umapi-client-2.8/umapi_client/functional.py
--rw-r--r--   0 travis    (2000) travis    (2000)    10696 2017-10-18 21:51:30.000000 umapi-client-2.8/umapi_client/legacy.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1154 2017-10-18 21:51:30.000000 umapi-client-2.8/umapi_client/version.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-10-18 21:53:15.000000 umapi-client-2.8/umapi_client.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     1152 2017-10-18 21:53:15.000000 umapi-client-2.8/umapi_client.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      431 2017-10-18 21:53:15.000000 umapi-client-2.8/umapi_client.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-10-18 21:53:15.000000 umapi-client-2.8/umapi_client.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-10-18 21:53:15.000000 umapi-client-2.8/umapi_client.egg-info/not-zip-safe
--rw-r--r--   0 travis    (2000) travis    (2000)       46 2017-10-18 21:53:15.000000 umapi-client-2.8/umapi_client.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       13 2017-10-18 21:53:15.000000 umapi-client-2.8/umapi_client.egg-info/top_level.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     1811 2017-10-18 21:51:30.000000 umapi-client-2.8/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)       92 2017-10-18 21:53:15.000000 umapi-client-2.8/setup.cfg
--rw-r--r--   0 travis    (2000) travis    (2000)     2964 2017-10-18 21:51:30.000000 umapi-client-2.8/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1152 2017-10-18 21:53:15.000000 umapi-client-2.8/PKG-INFO
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-11-15 01:47:38.000000 umapi-client-2.9/
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client/
+-rw-r--r--   0 travis    (2000) travis    (2000)     1553 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/__init__.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    10469 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/api.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     3803 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/auth.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    23658 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/connection.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     2589 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/error.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    22815 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/functional.py
+-rw-r--r--   0 travis    (2000) travis    (2000)    10696 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/legacy.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1154 2017-11-15 01:45:32.000000 umapi-client-2.9/umapi_client/version.py
+drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     1152 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/PKG-INFO
+-rw-r--r--   0 travis    (2000) travis    (2000)      431 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)        1 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/not-zip-safe
+-rw-r--r--   0 travis    (2000) travis    (2000)       46 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/requires.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)       13 2017-11-15 01:47:38.000000 umapi-client-2.9/umapi_client.egg-info/top_level.txt
+-rw-r--r--   0 travis    (2000) travis    (2000)     1811 2017-11-15 01:45:32.000000 umapi-client-2.9/README.md
+-rw-r--r--   0 travis    (2000) travis    (2000)       92 2017-11-15 01:47:38.000000 umapi-client-2.9/setup.cfg
+-rw-r--r--   0 travis    (2000) travis    (2000)     2964 2017-11-15 01:45:32.000000 umapi-client-2.9/setup.py
+-rw-r--r--   0 travis    (2000) travis    (2000)     1152 2017-11-15 01:47:38.000000 umapi-client-2.9/PKG-INFO
```

### Comparing `umapi-client-2.8/umapi_client/__init__.py` & `umapi-client-2.9/umapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `umapi-client-2.8/umapi_client/api.py` & `umapi-client-2.9/umapi_client/api.py`

 * *Files identical despite different names*

### Comparing `umapi-client-2.8/umapi_client/auth.py` & `umapi-client-2.9/umapi_client/auth.py`

 * *Files identical despite different names*

### Comparing `umapi-client-2.8/umapi_client/connection.py` & `umapi-client-2.9/umapi_client/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
                  logger=logging.getLogger("umapi_client"),
                  retry_max_attempts=4,
                  retry_first_delay=15,
                  retry_random_delay=5,
                  timeout_seconds=120.0,
                  throttle_actions=10,
                  throttle_commands=10,
+                 throttle_groups=10,
                  user_agent=None,
                  **kwargs):
         """
         Open a connection for the given parameters that has the given options.
         The connection is authorized and the auth token reused on all calls.
 
         Required parameters.  You must specify org_id and one of auth *or* auth_dict
@@ -87,14 +88,15 @@
         :param logger: The log handler to use (None suppresses logging, default is named "umapi_client")
         :param retry_max_attempts: How many times to retry on temporary errors
         :param retry_first_delay: The time to delay first retry (grows exponentially from there)
         :param retry_random_delay: The max random delay to add on each exponential backoff retry
         :param timeout_seconds: How many seconds to wait for server response (<= 0 or None means forever)
         :param throttle_actions: Max number of actions to pack into a single call
         :param throttle_commands: Max number of commands allowed in a single action
+        :param throttle_groups: Max number of groups to add/remove to/from a user
         :param user_agent: (optional) string to use as User-Agent header (umapi-client/version data will be added)
 
         Additional keywords are allowed to make it easy to pass a big dictionary with other values
         :param kwargs: any keywords passed that we ignore.
         """
         self.org_id = str(org_id)
         self.endpoint = user_management_endpoint
@@ -102,14 +104,15 @@
         self.logger = logger
         self.retry_max_attempts = retry_max_attempts
         self.retry_first_delay = retry_first_delay
         self.retry_random_delay = retry_random_delay
         self.timeout = float(timeout_seconds) if timeout_seconds and float(timeout_seconds) > 0.0 else None
         self.throttle_actions = max(int(throttle_actions), 1)
         self.throttle_commands = max(int(throttle_commands), 1)
+        self.throttle_groups = max(int(throttle_groups), 1)
         self.action_queue = []
         self.local_status = {"multiple-query-count": 0,
                              "single-query-count": 0,
                              "actions-sent": 0,
                              "actions-completed": 0,
                              "actions-queued": 0}
         self.server_status = {"status": "Never contacted",
@@ -301,19 +304,28 @@
         that we had a problem understanding the server.
 
         :param actions: the list of Action objects to be executed
         :param immediate: whether to immediately send them to the server
         :return: tuple: the number of actions in the queue, that got sent, and that executed successfully.
         """
         # throttling part 1: split up each action into smaller actions, as needed
+        # optionally split large lists of groups in add/remove commands (if action supports it)
         split_actions = []
         exceptions = []
         for a in actions:
             if len(a.commands) == 0:
                 if self.logger: self.logger.warning("Sending action with no commands: %s", a.frame)
+            # maybe_split_groups is a UserAction attribute, so the call may throw an AttributeError
+            try:
+                if a.maybe_split_groups(self.throttle_groups):
+                    if self.logger: self.logger.debug(
+                        "Throttling actions %s to have a maximum of %d entries in group lists.",
+                        a.frame, self.throttle_groups)
+            except AttributeError:
+                pass
             if len(a.commands) > self.throttle_commands:
                 if self.logger: self.logger.debug("Throttling action %s to have a maximum of %d commands.",
                                                   a.frame, self.throttle_commands)
                 split_actions += a.split(self.throttle_commands)
             else:
                 split_actions.append(a)
         actions = self.action_queue + split_actions
```

### Comparing `umapi-client-2.8/umapi_client/error.py` & `umapi-client-2.9/umapi_client/error.py`

 * *Files identical despite different names*

### Comparing `umapi-client-2.8/umapi_client/functional.py` & `umapi-client-2.9/umapi_client/functional.py`

 * *Files 3% similar despite different names*

```diff
@@ -304,14 +304,47 @@
         :return: None, because you cannot follow this command with another.
         """
         if self.id_type == IdentityTypes.adobeID:
             raise ArgumentError("You cannot delete an Adobe ID account.")
         self.append(removeFromDomain={})
         return None
 
+    def maybe_split_groups(self, max_groups):
+        """
+        Check if group lists in add/remove directives should be split and split them if needed
+        :param max_groups: Max group list size
+        :return: True if at least one command was split, False if none were split
+        """
+        split_commands = []
+        # return True if we split at least once
+        maybe_split = False
+        valid_step_keys = ['add', 'addRoles', 'remove']
+        for command in self.commands:
+            # commands are assumed to contain a single key
+            step_key, step_args = next(six.iteritems(command))
+            if step_key not in valid_step_keys or not isinstance(step_args, dict):
+                split_commands.append(command)
+                continue
+            new_commands = [command]
+            while True:
+                new_command = {step_key: {}}
+                for group_type, groups in six.iteritems(command[step_key]):
+                    if len(groups) > max_groups:
+                        command[step_key][group_type], new_command[step_key][group_type] = \
+                            groups[0:max_groups], groups[max_groups:]
+                if new_command[step_key]:
+                    new_commands.append(new_command)
+                    command = new_command
+                    maybe_split = True
+                else:
+                    break
+            split_commands += new_commands
+        self.commands = split_commands
+        return maybe_split
+
 
 class UsersQuery(QueryMultiple):
     """
     Query for users meeting (optional) criteria
     """
 
     def __init__(self, connection, in_group="", in_domain="", identity_type="", direct_only=True):
```

### Comparing `umapi-client-2.8/umapi_client/legacy.py` & `umapi-client-2.9/umapi_client/legacy.py`

 * *Files identical despite different names*

### Comparing `umapi-client-2.8/umapi_client/version.py` & `umapi-client-2.9/umapi_client/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = "2.8"
+__version__ = "2.9"
```

### Comparing `umapi-client-2.8/umapi_client.egg-info/PKG-INFO` & `umapi-client-2.9/umapi_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: umapi-client
-Version: 2.8
+Version: 2.9
 Summary: Client for the User Management API (UMAPI) from Adobe - see https://adobe.ly/2h1pHgV
 Home-page: https://github.com/adobe-apiplatform/umapi-client.py
 Author: Daniel Brotsky
 Author-email: dbrotsky@adobe.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: The User Management API (aka the UMAPI) is an Adobe-hosted network service which provides Adobe Enterprise customers the ability to manage their users.  This client makes it easy to access the UMAPI from a local Python application.  This client is open source, maintained by Adobe, and distributed under the terms of the OSI-approved MIT license.  Copyright (c) 2016-2017 Adobe Systems Incorporated.
```

### Comparing `umapi-client-2.8/README.md` & `umapi-client-2.9/README.md`

 * *Files identical despite different names*

### Comparing `umapi-client-2.8/setup.py` & `umapi-client-2.9/setup.py`

 * *Files identical despite different names*

### Comparing `umapi-client-2.8/PKG-INFO` & `umapi-client-2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: umapi-client
-Version: 2.8
+Version: 2.9
 Summary: Client for the User Management API (UMAPI) from Adobe - see https://adobe.ly/2h1pHgV
 Home-page: https://github.com/adobe-apiplatform/umapi-client.py
 Author: Daniel Brotsky
 Author-email: dbrotsky@adobe.com
 License: MIT
 Description-Content-Type: UNKNOWN
 Description: The User Management API (aka the UMAPI) is an Adobe-hosted network service which provides Adobe Enterprise customers the ability to manage their users.  This client makes it easy to access the UMAPI from a local Python application.  This client is open source, maintained by Adobe, and distributed under the terms of the OSI-approved MIT license.  Copyright (c) 2016-2017 Adobe Systems Incorporated.
```

