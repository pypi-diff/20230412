# Comparing `tmp/pulumi_policy-1.5.0a1665075566-py2.py3-none-any.whl.zip` & `tmp/pulumi_policy-1.6.0a1681325772-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15477 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1483 b- defN 22-Oct-06 17:01 pulumi_policy/__init__.py
--rw-r--r--  2.0 unx     3849 b- defN 22-Oct-06 17:01 pulumi_policy/deserialize.py
--rw-r--r--  2.0 unx    39857 b- defN 22-Oct-06 17:01 pulumi_policy/policy.py
--rw-r--r--  2.0 unx     6833 b- defN 22-Oct-06 17:01 pulumi_policy/proxy.py
--rw-r--r--  2.0 unx       22 b- defN 22-Oct-06 17:01 pulumi_policy/pulumiplugin.json
--rw-r--r--  2.0 unx        0 b- defN 22-Oct-06 17:01 pulumi_policy/py.typed
--rw-r--r--  2.0 unx      634 b- defN 22-Oct-06 17:01 pulumi_policy/version.py
--rw-r--r--  2.0 unx     2339 b- defN 22-Oct-06 17:01 pulumi_policy-1.5.0a1665075566.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 22-Oct-06 17:01 pulumi_policy-1.5.0a1665075566.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 22-Oct-06 17:01 pulumi_policy-1.5.0a1665075566.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      936 b- defN 22-Oct-06 17:01 pulumi_policy-1.5.0a1665075566.dist-info/RECORD
-11 files, 56077 bytes uncompressed, 13877 bytes compressed:  75.3%
+Zip file size: 15501 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1483 b- defN 23-Apr-12 18:57 pulumi_policy/__init__.py
+-rw-r--r--  2.0 unx     3849 b- defN 23-Apr-12 18:57 pulumi_policy/deserialize.py
+-rw-r--r--  2.0 unx    39992 b- defN 23-Apr-12 18:57 pulumi_policy/policy.py
+-rw-r--r--  2.0 unx     6833 b- defN 23-Apr-12 18:57 pulumi_policy/proxy.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-12 18:57 pulumi_policy/pulumiplugin.json
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-12 18:57 pulumi_policy/py.typed
+-rw-r--r--  2.0 unx      634 b- defN 23-Apr-12 18:57 pulumi_policy/version.py
+-rw-r--r--  2.0 unx     2339 b- defN 23-Apr-12 18:57 pulumi_policy-1.6.0a1681325772.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-12 18:57 pulumi_policy-1.6.0a1681325772.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-12 18:57 pulumi_policy-1.6.0a1681325772.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      936 b- defN 23-Apr-12 18:57 pulumi_policy-1.6.0a1681325772.dist-info/RECORD
+11 files, 56212 bytes uncompressed, 13901 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: pulumi_policy/py.typed
 Comment: 
 
 Filename: pulumi_policy/version.py
 Comment: 
 
-Filename: pulumi_policy-1.5.0a1665075566.dist-info/METADATA
+Filename: pulumi_policy-1.6.0a1681325772.dist-info/METADATA
 Comment: 
 
-Filename: pulumi_policy-1.5.0a1665075566.dist-info/WHEEL
+Filename: pulumi_policy-1.6.0a1681325772.dist-info/WHEEL
 Comment: 
 
-Filename: pulumi_policy-1.5.0a1665075566.dist-info/top_level.txt
+Filename: pulumi_policy-1.6.0a1681325772.dist-info/top_level.txt
 Comment: 
 
-Filename: pulumi_policy-1.5.0a1665075566.dist-info/RECORD
+Filename: pulumi_policy-1.6.0a1681325772.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pulumi_policy/policy.py

```diff
@@ -673,15 +673,15 @@
 
     class IntermediateStackResource(NamedTuple):
         resource: PolicyResource
         parent: Optional[str]
         dependencies: List[str]
         property_dependencies: Dict[str, List[str]]
 
-    def Analyze(self, request, context):
+    def Analyze(self, request, _context):
         self._configure_runtime_settings()
 
         diagnostics: List[proto.AnalyzeDiagnostic] = []
         for policy in self.__policies:
             enforcement_level = self._get_enforcement_level(policy)
             if enforcement_level == EnforcementLevel.DISABLED or not isinstance(policy, ResourceValidationPolicy):
                 continue
@@ -699,27 +699,27 @@
             try:
                 result = policy.validate(args, report_violation)
                 if isawaitable(result):
                     loop = asyncio.new_event_loop()
                     loop.run_until_complete(result)
                     loop.close()
             except UnknownValueError as e:
-                diagnostics.append(proto.AnalyzeDiagnostic(
+                diagnostics.append(proto.AnalyzeDiagnostic(  # type: ignore
                     policyName=policy.name,
                     policyPackName=self.__policy_pack_name,
                     policyPackVersion=self.__policy_pack_version,
                     message=f"can't run policy '{policy.name}' during preview: {e.message}",
                     urn="",
                     description=policy.description,
                     enforcementLevel=self._map_enforcement_level(EnforcementLevel.ADVISORY),
                 ))
 
         return proto.AnalyzeResponse(diagnostics=diagnostics)
 
-    def AnalyzeStack(self, request, context):
+    def AnalyzeStack(self, request, _context):
         self._configure_runtime_settings()
 
         diagnostics: List[proto.AnalyzeDiagnostic] = []
         for policy in self.__policies:
             enforcement_level = self._get_enforcement_level(policy)
             if enforcement_level == EnforcementLevel.DISABLED or not isinstance(policy, StackValidationPolicy):
                 continue
@@ -786,15 +786,15 @@
                     urn="",
                     description=policy.description,
                     enforcementLevel=self._map_enforcement_level(EnforcementLevel.ADVISORY),
                 ))
 
         return proto.AnalyzeResponse(diagnostics=diagnostics)
 
-    def GetAnalyzerInfo(self, request, context):
+    def GetAnalyzerInfo(self, _request, _context):
         policies: List[proto.PolicyInfo] = []
         for policy in self.__policies:
             enforcement_level = (policy.enforcement_level if policy.enforcement_level is not None
                                  else self.__policy_pack_enforcement_level)
 
             schema = {}
             if policy.config_schema is not None:
@@ -834,18 +834,18 @@
             name=self.__policy_pack_name,
             version=self.__policy_pack_version,
             supportsConfig=True,
             policies=policies,
             initialConfig=initial_config,
         )
 
-    def GetPluginInfo(self, request, context):
+    def GetPluginInfo(self, _request, _context):
         return proto.PluginInfo(version=VERSION)
 
-    def Configure(self, request, context):
+    def Configure(self, request, _context):
         config, config_enforcement_level = {}, {}
         for k in request.policyConfig:
             v = request.policyConfig[k]
             config[k] = json_format.MessageToDict(v.properties)
             config_enforcement_level[k] = self._convert_enforcement_level(v.enforcementLevel)
         self.__policy_pack_config = config
         self.__policy_pack_config_enforcement_level = config_enforcement_level
@@ -889,41 +889,41 @@
             if urn is not None and not isinstance(urn, str):
                 raise TypeError("Expected urn to be a string")
 
             violation_message = policy_description
             if message:
                 violation_message += f"\n{message}"
 
-            diagnostics.append(proto.AnalyzeDiagnostic(
+            diagnostics.append(proto.AnalyzeDiagnostic(  # type: ignore
                 policyName=policy_name,
                 policyPackName=self.__policy_pack_name,
                 policyPackVersion=self.__policy_pack_version,
                 message=violation_message,
                 urn=urn if urn else "",
                 description=policy_description,
                 enforcementLevel=self._map_enforcement_level(enforcement_level),
             ))
         return report_violation
 
     def _map_enforcement_level(self, enforcement_level: EnforcementLevel) -> int:
         if enforcement_level == EnforcementLevel.ADVISORY:
-            return proto.ADVISORY
+            return proto.ADVISORY  # type: ignore
         if enforcement_level == EnforcementLevel.MANDATORY:
-            return proto.MANDATORY
+            return proto.MANDATORY  # type: ignore
         if enforcement_level == EnforcementLevel.DISABLED:
-            return proto.DISABLED
+            return proto.DISABLED  # type: ignore
         raise AssertionError(
             f"unknown enforcement level: {enforcement_level}")
 
     def _convert_enforcement_level(self, enforcement_level: int) -> EnforcementLevel:
-        if enforcement_level == proto.ADVISORY:
+        if enforcement_level == proto.ADVISORY:  # type: ignore
             return EnforcementLevel.ADVISORY
-        if enforcement_level == proto.MANDATORY:
+        if enforcement_level == proto.MANDATORY:  # type: ignore
             return EnforcementLevel.MANDATORY
-        if enforcement_level == proto.DISABLED:
+        if enforcement_level == proto.DISABLED:  # type: ignore
             return EnforcementLevel.DISABLED
         raise AssertionError(
             f"unknown enforcement level: {enforcement_level}")
 
     def _get_resource_options(self, request) -> PolicyResourceOptions:
         opts = request.options
         protect = opts.protect
```

## pulumi_policy/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-VERSION = "1.5.0-alpha.1665075566+4b2bd7b5"
+VERSION = "1.6.0-alpha.1681325772+79f33b3a"
```

## Comparing `pulumi_policy-1.5.0a1665075566.dist-info/METADATA` & `pulumi_policy-1.6.0a1681325772.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-policy
-Version: 1.5.0a1665075566
+Version: 1.6.0a1681325772
 Summary: Pulumi's Policy Python SDK
 Home-page: https://github.com/pulumi/pulumi-policy
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Requires-Dist: pulumi (<4.0.0,>=3.0.0)
 Requires-Dist: protobuf (>=3.6.0)
 Requires-Dist: grpcio (>=1.9.1)
```

## Comparing `pulumi_policy-1.5.0a1665075566.dist-info/RECORD` & `pulumi_policy-1.6.0a1681325772.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pulumi_policy/__init__.py,sha256=K99pGM6N3NaP7j-FTt2oyoxHfYSmpgUXmwp-cenYV7Y,1483
 pulumi_policy/deserialize.py,sha256=DHI6Ssbv-Z4-znbQONTX_s2ylvx_l0fYKakBO3ajsgw,3849
-pulumi_policy/policy.py,sha256=CwWD0Th0DfmWay_y2Zoe89A-M92nw7E6kUkkMgJsxNY,39857
+pulumi_policy/policy.py,sha256=6nHRfPGjR6_FaT_JcoavmHccGUfUO_GWZ_y3Lfekirw,39992
 pulumi_policy/proxy.py,sha256=RMFCa72PjZ_fPSRWkCCcafDmzHQUpixfny4MQbuYH5U,6833
 pulumi_policy/pulumiplugin.json,sha256=-N5Rzo52OzMKvgqLH1JxqCkgtQ0y9JyJy0SQHEHbw24,22
 pulumi_policy/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pulumi_policy/version.py,sha256=B2Bk_h0x1JO0okrC7Etn0XX8reryg4Lo5anC9m8kAxo,634
-pulumi_policy-1.5.0a1665075566.dist-info/METADATA,sha256=M9-sR5YMc-PTwAT0Y41qOXOeIH6vgFPwBXHiVMb2gBw,2339
-pulumi_policy-1.5.0a1665075566.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-pulumi_policy-1.5.0a1665075566.dist-info/top_level.txt,sha256=Kple_6YMrdhwu7WmTNRlUqrt9Hoy368SVBiYRCF5B2k,14
-pulumi_policy-1.5.0a1665075566.dist-info/RECORD,,
+pulumi_policy/version.py,sha256=UL8mLfGarf7x6ErIlMdDpblqzseWHXRDlBvPPtONXMs,634
+pulumi_policy-1.6.0a1681325772.dist-info/METADATA,sha256=LRsqig4SX9sCikNDh2GhCw4g4zWiXO16CfvA_midyf4,2339
+pulumi_policy-1.6.0a1681325772.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+pulumi_policy-1.6.0a1681325772.dist-info/top_level.txt,sha256=Kple_6YMrdhwu7WmTNRlUqrt9Hoy368SVBiYRCF5B2k,14
+pulumi_policy-1.6.0a1681325772.dist-info/RECORD,,
```

