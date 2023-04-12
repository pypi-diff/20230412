# Comparing `tmp/cloudsnorkel.cdk-github-runners-0.9.3.tar.gz` & `tmp/cloudsnorkel.cdk-github-runners-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudsnorkel.cdk-github-runners-0.9.3.tar", last modified: Fri Apr  7 14:03:33 2023, max compression
+gzip compressed data, was "cloudsnorkel.cdk-github-runners-0.9.4.tar", last modified: Wed Apr 12 00:08:28 2023, max compression
```

## Comparing `cloudsnorkel.cdk-github-runners-0.9.3.tar` & `cloudsnorkel.cdk-github-runners-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:03:33.148606 cloudsnorkel.cdk-github-runners-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-07 14:03:21.000000 cloudsnorkel.cdk-github-runners-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-07 14:03:21.000000 cloudsnorkel.cdk-github-runners-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-04-07 14:03:33.148606 cloudsnorkel.cdk-github-runners-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-07 14:03:21.000000 cloudsnorkel.cdk-github-runners-0.9.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-07 14:03:21.000000 cloudsnorkel.cdk-github-runners-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 14:03:33.148606 cloudsnorkel.cdk-github-runners-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-07 14:03:21.000000 cloudsnorkel.cdk-github-runners-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:03:33.144606 cloudsnorkel.cdk-github-runners-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:03:33.144606 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:03:33.144606 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel/cdk_github_runners/
--rw-r--r--   0 runner    (1001) docker     (123)   554397 2023-04-07 14:03:21.000000 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel/cdk_github_runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:03:33.144606 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel/cdk_github_runners/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-07 14:03:21.000000 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1979084 2023-04-07 14:03:21.000000 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 14:03:21.000000 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel/cdk_github_runners/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 14:03:33.144606 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel.cdk_github_runners.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-04-07 14:03:33.000000 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-07 14:03:33.000000 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 14:03:33.000000 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-07 14:03:33.000000 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 14:03:33.000000 cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.739040 cloudsnorkel.cdk-github-runners-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-04-12 00:08:28.739040 cloudsnorkel.cdk-github-runners-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 00:08:28.739040 cloudsnorkel.cdk-github-runners-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.731040 cloudsnorkel.cdk-github-runners-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.731040 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.735040 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/
+-rw-r--r--   0 runner    (1001) docker     (123)   555013 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.735040 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1986936 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 00:08:15.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 00:08:28.735040 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-04-12 00:08:28.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-12 00:08:28.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 00:08:28.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 00:08:28.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-12 00:08:28.000000 cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.3/LICENSE` & `cloudsnorkel.cdk-github-runners-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudsnorkel.cdk-github-runners-0.9.3/PKG-INFO` & `cloudsnorkel.cdk-github-runners-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-github-runners
-Version: 0.9.3
+Version: 0.9.4
 Summary: CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.
 Home-page: https://github.com/CloudSnorkel/cdk-github-runners.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-github-runners.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.3/README.md` & `cloudsnorkel.cdk-github-runners-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `cloudsnorkel.cdk-github-runners-0.9.3/setup.py` & `cloudsnorkel.cdk-github-runners-0.9.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudsnorkel.cdk-github-runners",
-    "version": "0.9.3",
+    "version": "0.9.4",
     "description": "CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.",
     "license": "Apache-2.0",
     "url": "https://github.com/CloudSnorkel/cdk-github-runners.git",
     "long_description_content_type": "text/markdown",
     "author": "Amir Szekely<amir@cloudsnorkel.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cloudsnorkel.cdk_github_runners",
         "cloudsnorkel.cdk_github_runners._jsii"
     ],
     "package_data": {
         "cloudsnorkel.cdk_github_runners._jsii": [
-            "cdk-github-runners@0.9.3.jsii.tgz"
+            "cdk-github-runners@0.9.4.jsii.tgz"
         ],
         "cloudsnorkel.cdk_github_runners": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.50.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel/cdk_github_runners/__init__.py` & `cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel/cdk_github_runners/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,14 +258,15 @@
 import aws_cdk.aws_ecs as _aws_cdk_aws_ecs_ceddda9d
 import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
 import aws_cdk.aws_imagebuilder as _aws_cdk_aws_imagebuilder_ceddda9d
 import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
 import aws_cdk.aws_logs as _aws_cdk_aws_logs_ceddda9d
 import aws_cdk.aws_s3_assets as _aws_cdk_aws_s3_assets_ceddda9d
 import aws_cdk.aws_secretsmanager as _aws_cdk_aws_secretsmanager_ceddda9d
+import aws_cdk.aws_sns as _aws_cdk_aws_sns_ceddda9d
 import aws_cdk.aws_stepfunctions as _aws_cdk_aws_stepfunctions_ceddda9d
 import constructs as _constructs_77d1e7e8
 
 
 @jsii.data_type(
     jsii_type="@cloudsnorkel/cdk-github-runners.AmiBuilderProps",
     jsii_struct_bases=[],
@@ -1477,14 +1478,26 @@
             vpc=vpc,
             vpc_subnets=vpc_subnets,
             webhook_access=webhook_access,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
+    @jsii.member(jsii_name="failedImageBuildsTopic")
+    def failed_image_builds_topic(self) -> _aws_cdk_aws_sns_ceddda9d.Topic:
+        '''(experimental) Creates a topic for notifications when a runner image build fails.
+
+        Runner images are rebuilt every week by default. This provides the latest GitHub Runner version and software updates.
+
+        If you want to be sure you are using the latest runner version, you can use this topic to be notified when a build fails.
+
+        :stability: experimental
+        '''
+        return typing.cast(_aws_cdk_aws_sns_ceddda9d.Topic, jsii.invoke(self, "failedImageBuildsTopic", []))
+
     @jsii.member(jsii_name="metricFailed")
     def metric_failed(
         self,
         *,
         metric_name: builtins.str,
         namespace: builtins.str,
         account: typing.Optional[builtins.str] = None,
@@ -2604,15 +2617,14 @@
     Example::
 
        new ImageBuilderComponent(this, 'AWS CLI', {
          platform: 'Windows',
          displayName: 'AWS CLI',
          description: 'Install latest version of AWS CLI',
          commands: [
-           '$ErrorActionPreference = \\'Stop\\'',
            'Start-Process msiexec.exe -Wait -ArgumentList \\'/i https://awscli.amazonaws.com/AWSCLIV2.msi /qn\\'',
          ],
        }
 
     :deprecated: Use ``RunnerImageComponent`` instead as this be internal soon.
 
     :stability: deprecated
@@ -5644,15 +5656,14 @@
            rebuildInterval: Duration.days(14),
        });
        builder.addComponent(new ImageBuilderComponent(scope, id, {
          platform: 'Linux',
          displayName: 'p7zip',
          description: 'Install some more packages',
          commands: [
-           'set -ex',
            'apt-get install p7zip',
          ],
        }));
        new Ec2Runner(this, 'EC2 provider', {
            label: 'custom-ec2',
            amiBuilder: builder,
        });
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO` & `cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudsnorkel.cdk-github-runners
-Version: 0.9.3
+Version: 0.9.4
 Summary: CDK construct to create GitHub Actions self-hosted runners. A webhook listens to events and creates ephemeral runners on the fly.
 Home-page: https://github.com/CloudSnorkel/cdk-github-runners.git
 Author: Amir Szekely<amir@cloudsnorkel.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/CloudSnorkel/cdk-github-runners.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudsnorkel.cdk-github-runners-0.9.3/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt` & `cloudsnorkel.cdk-github-runners-0.9.4/src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudsnorkel.cdk_github_runners.egg-info/SOURCES.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/dependency_links.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/requires.txt
 src/cloudsnorkel.cdk_github_runners.egg-info/top_level.txt
 src/cloudsnorkel/cdk_github_runners/__init__.py
 src/cloudsnorkel/cdk_github_runners/py.typed
 src/cloudsnorkel/cdk_github_runners/_jsii/__init__.py
-src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.3.jsii.tgz
+src/cloudsnorkel/cdk_github_runners/_jsii/cdk-github-runners@0.9.4.jsii.tgz
```

