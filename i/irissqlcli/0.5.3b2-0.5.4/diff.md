# Comparing `tmp/irissqlcli-0.5.3b2.tar.gz` & `tmp/irissqlcli-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irissqlcli-0.5.3b2.tar", last modified: Wed Apr 12 09:32:15 2023, max compression
+gzip compressed data, was "irissqlcli-0.5.4.tar", last modified: Wed Apr 12 09:32:42 2023, max compression
```

## Comparing `irissqlcli-0.5.3b2.tar` & `irissqlcli-0.5.4.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.041403 irissqlcli-0.5.3b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-12 09:32:15.041403 irissqlcli-0.5.3b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.033403 irissqlcli-0.5.3b2/intersystems_iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_BufferReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_BufferWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_ConnectionInformation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_ConnectionParameters.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_Constant.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_DBList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_Device.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_GatewayContext.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_GatewayException.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_GatewayUtility.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRIS.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRISConnection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRISEmbedded.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRISGlobalNode.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRISGlobalNodeView.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRISIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRISList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRISOREF.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRISObject.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_IRISReference.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_InStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_LegacyIterator.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_ListItem.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_ListReader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_ListWriter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_LogFileStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_MessageHeader.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_OutStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_PrintStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_PythonGateway.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/_SharedMemorySocket.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.033403 irissqlcli-0.5.3b2/intersystems_iris/dbapi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/_Column.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    94963 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/_DBAPI.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/_Descriptor.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/_IRISStream.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/_Parameter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/_ParameterCollection.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/_ResultSetRow.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/_SQLType.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.033403 irissqlcli-0.5.3b2/intersystems_iris/dbapi/preparser/
--rw-rw-rw-   0 runner    (1001) docker     (123)    78588 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/preparser/_PreParser.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/preparser/_Scanner.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/preparser/_Token.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/preparser/_TokenList.py
--rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/dbapi/preparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.037403 irissqlcli-0.5.3b2/intersystems_iris/pex/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_BusinessHost.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_BusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_BusinessProcess.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_BusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_Common.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_Director.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_IRISBusinessOperation.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_IRISBusinessService.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_IRISInboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_IRISOutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_InboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_Message.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/_OutboundAdapter.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/intersystems_iris/pex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.037403 irissqlcli-0.5.3b2/iris/
--rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/iris/__init__.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/iris/iris_site.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/iris/irisbuiltins.py
--rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/iris/irisloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.037403 irissqlcli-0.5.3b2/irisnative/
--rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/irisnative/_IRISNative.py
--rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-12 09:32:07.000000 irissqlcli-0.5.3b2/irisnative/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.037403 irissqlcli-0.5.3b2/irissqlcli/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-12 09:31:50.000000 irissqlcli-0.5.3b2/irissqlcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/clitoolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/completion_refresher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/irissqlclirc
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)    35327 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.041403 irissqlcli-0.5.3b2/irissqlcli/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/completion_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/encodingutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/filepaths.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/parseutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/prompt_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.041403 irissqlcli-0.5.3b2/irissqlcli/packages/special/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/special/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/special/dbcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/special/favoritequeries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/special/iocommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/special/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/packages/special/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/sqlcompleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/sqlexecute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/irissqlcli/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.037403 irissqlcli-0.5.3b2/irissqlcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-04-12 09:32:15.000000 irissqlcli-0.5.3b2/irissqlcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-12 09:32:15.000000 irissqlcli-0.5.3b2/irissqlcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:32:15.000000 irissqlcli-0.5.3b2/irissqlcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 09:32:15.000000 irissqlcli-0.5.3b2/irissqlcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-12 09:32:15.000000 irissqlcli-0.5.3b2/irissqlcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 09:32:15.000000 irissqlcli-0.5.3b2/irissqlcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-12 09:32:15.041403 irissqlcli-0.5.3b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:15.041403 irissqlcli-0.5.3b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:31:49.000000 irissqlcli-0.5.3b2/tests/test_sqlcompletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.309650 irissqlcli-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-12 09:32:42.309650 irissqlcli-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.297650 irissqlcli-0.5.4/intersystems_iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      299 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_BufferReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1337 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_BufferWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1896 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_ConnectionInformation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      578 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_ConnectionParameters.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1483 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_Constant.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    20104 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_DBList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2311 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_Device.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      618 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_GatewayContext.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       96 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_GatewayException.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2735 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_GatewayUtility.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    49548 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRIS.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    21467 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRISConnection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2614 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRISEmbedded.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12049 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRISGlobalNode.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      797 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRISGlobalNodeView.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6906 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRISIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10247 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRISList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6756 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)       82 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRISOREF.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14456 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRISObject.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4905 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_IRISReference.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6643 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_InStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4130 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_LegacyIterator.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      354 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_ListItem.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2966 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_ListReader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5515 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_ListWriter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3797 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_LogFileStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1662 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_MessageHeader.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1327 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_OutStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1963 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_PrintStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    41638 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_PythonGateway.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4330 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/_SharedMemorySocket.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1773 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      218 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.301650 irissqlcli-0.5.4/intersystems_iris/dbapi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2535 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/_Column.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    94963 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/_DBAPI.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1391 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/_Descriptor.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2113 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/_IRISStream.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4076 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4776 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/_Parameter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5151 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/_ParameterCollection.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    12810 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/_ResultSetRow.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      557 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/_SQLType.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.301650 irissqlcli-0.5.4/intersystems_iris/dbapi/preparser/
+-rw-rw-rw-   0 runner    (1001) docker     (123)    78588 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/preparser/_PreParser.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    16163 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/preparser/_Scanner.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2304 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/preparser/_Token.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6770 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/preparser/_TokenList.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/dbapi/preparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.301650 irissqlcli-0.5.4/intersystems_iris/pex/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4370 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_BusinessHost.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5241 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_BusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10774 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_BusinessProcess.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5441 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_BusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)    10509 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_Common.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1203 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_Director.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      172 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_IRISBusinessOperation.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      585 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_IRISBusinessService.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      171 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_IRISInboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      522 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_IRISOutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2296 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_InboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      320 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_Message.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1628 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/_OutboundAdapter.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1379 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/intersystems_iris/pex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.305650 irissqlcli-0.5.4/iris/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      922 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/iris/__init__.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      501 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/iris/iris_site.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2687 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/iris/irisbuiltins.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4808 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/iris/irisloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.305650 irissqlcli-0.5.4/irisnative/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      665 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/irisnative/_IRISNative.py
+-rw-rw-rw-   0 runner    (1001) docker     (123)      341 2023-04-12 09:32:34.000000 irissqlcli-0.5.4/irisnative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.305650 irissqlcli-0.5.4/irissqlcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/clitoolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/completion_refresher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/irissqlclirc
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35327 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.305650 irissqlcli-0.5.4/irissqlcli/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/completion_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/encodingutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/filepaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/parseutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/prompt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.305650 irissqlcli-0.5.4/irissqlcli/packages/special/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/special/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/special/dbcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/special/favoritequeries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/special/iocommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/special/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/packages/special/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/sqlcompleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/sqlexecute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/irissqlcli/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.305650 irissqlcli-0.5.4/irissqlcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-12 09:32:42.000000 irissqlcli-0.5.4/irissqlcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-12 09:32:42.000000 irissqlcli-0.5.4/irissqlcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:32:42.000000 irissqlcli-0.5.4/irissqlcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-12 09:32:42.000000 irissqlcli-0.5.4/irissqlcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-12 09:32:42.000000 irissqlcli-0.5.4/irissqlcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-12 09:32:42.000000 irissqlcli-0.5.4/irissqlcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-12 09:32:42.309650 irissqlcli-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:42.309650 irissqlcli-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6093 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:32:14.000000 irissqlcli-0.5.4/tests/test_sqlcompletion.py
```

### Comparing `irissqlcli-0.5.3b2/LICENSE` & `irissqlcli-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/PKG-INFO` & `irissqlcli-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irissqlcli
-Version: 0.5.3b2
+Version: 0.5.4
 Summary: CLI for SQL of InterSystems IRIS Databases with auto-completion and syntax highlighting.
 Home-page: https://github.com/caretdev/irissqlcli
 Author: CaretDev
 Author-email: irissqlcli@caretdev.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `irissqlcli-0.5.3b2/README.md` & `irissqlcli-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_BufferWriter.py` & `irissqlcli-0.5.4/intersystems_iris/_BufferWriter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_ConnectionInformation.py` & `irissqlcli-0.5.4/intersystems_iris/_ConnectionInformation.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_ConnectionParameters.py` & `irissqlcli-0.5.4/intersystems_iris/_ConnectionParameters.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_Constant.py` & `irissqlcli-0.5.4/intersystems_iris/_Constant.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_DBList.py` & `irissqlcli-0.5.4/intersystems_iris/_DBList.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_Device.py` & `irissqlcli-0.5.4/intersystems_iris/_Device.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_GatewayContext.py` & `irissqlcli-0.5.4/intersystems_iris/_GatewayContext.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_GatewayUtility.py` & `irissqlcli-0.5.4/intersystems_iris/_GatewayUtility.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_IRIS.py` & `irissqlcli-0.5.4/intersystems_iris/_IRIS.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_IRISConnection.py` & `irissqlcli-0.5.4/intersystems_iris/_IRISConnection.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_IRISEmbedded.py` & `irissqlcli-0.5.4/intersystems_iris/_IRISEmbedded.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_IRISGlobalNode.py` & `irissqlcli-0.5.4/intersystems_iris/_IRISGlobalNode.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_IRISGlobalNodeView.py` & `irissqlcli-0.5.4/intersystems_iris/_IRISGlobalNodeView.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_IRISIterator.py` & `irissqlcli-0.5.4/intersystems_iris/_IRISIterator.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_IRISList.py` & `irissqlcli-0.5.4/intersystems_iris/_IRISList.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_IRISNative.py` & `irissqlcli-0.5.4/intersystems_iris/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_IRISObject.py` & `irissqlcli-0.5.4/intersystems_iris/_IRISObject.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_IRISReference.py` & `irissqlcli-0.5.4/intersystems_iris/_IRISReference.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_InStream.py` & `irissqlcli-0.5.4/intersystems_iris/_InStream.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_LegacyIterator.py` & `irissqlcli-0.5.4/intersystems_iris/_LegacyIterator.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_ListReader.py` & `irissqlcli-0.5.4/intersystems_iris/_ListReader.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_ListWriter.py` & `irissqlcli-0.5.4/intersystems_iris/_ListWriter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_LogFileStream.py` & `irissqlcli-0.5.4/intersystems_iris/_LogFileStream.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_MessageHeader.py` & `irissqlcli-0.5.4/intersystems_iris/_MessageHeader.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_OutStream.py` & `irissqlcli-0.5.4/intersystems_iris/_OutStream.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_PrintStream.py` & `irissqlcli-0.5.4/intersystems_iris/_PrintStream.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_PythonGateway.py` & `irissqlcli-0.5.4/intersystems_iris/_PythonGateway.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/_SharedMemorySocket.py` & `irissqlcli-0.5.4/intersystems_iris/_SharedMemorySocket.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/__init__.py` & `irissqlcli-0.5.4/intersystems_iris/__init__.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/_Column.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/_Column.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/_DBAPI.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/_DBAPI.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/_Descriptor.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/_Descriptor.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/_IRISStream.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/_IRISStream.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/_Message.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/_Message.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/_Parameter.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/_Parameter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/_ParameterCollection.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/_ParameterCollection.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/_ResultSetRow.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/_ResultSetRow.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/_SQLType.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/_SQLType.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/preparser/_PreParser.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/preparser/_PreParser.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/preparser/_Scanner.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/preparser/_Scanner.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/preparser/_Token.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/preparser/_Token.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/dbapi/preparser/_TokenList.py` & `irissqlcli-0.5.4/intersystems_iris/dbapi/preparser/_TokenList.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/_BusinessHost.py` & `irissqlcli-0.5.4/intersystems_iris/pex/_BusinessHost.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/_BusinessOperation.py` & `irissqlcli-0.5.4/intersystems_iris/pex/_BusinessOperation.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/_BusinessProcess.py` & `irissqlcli-0.5.4/intersystems_iris/pex/_BusinessProcess.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/_BusinessService.py` & `irissqlcli-0.5.4/intersystems_iris/pex/_BusinessService.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/_Common.py` & `irissqlcli-0.5.4/intersystems_iris/pex/_Common.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/_Director.py` & `irissqlcli-0.5.4/intersystems_iris/pex/_Director.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/_IRISBusinessService.py` & `irissqlcli-0.5.4/intersystems_iris/pex/_IRISBusinessService.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/_IRISOutboundAdapter.py` & `irissqlcli-0.5.4/intersystems_iris/pex/_IRISOutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/_InboundAdapter.py` & `irissqlcli-0.5.4/intersystems_iris/pex/_InboundAdapter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/_OutboundAdapter.py` & `irissqlcli-0.5.4/intersystems_iris/pex/_OutboundAdapter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/intersystems_iris/pex/__init__.py` & `irissqlcli-0.5.4/intersystems_iris/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/iris/__init__.py` & `irissqlcli-0.5.4/iris/__init__.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/iris/irisbuiltins.py` & `irissqlcli-0.5.4/iris/irisbuiltins.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/iris/irisloader.py` & `irissqlcli-0.5.4/iris/irisloader.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irisnative/_IRISNative.py` & `irissqlcli-0.5.4/irisnative/_IRISNative.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/clitoolbar.py` & `irissqlcli-0.5.4/irissqlcli/clitoolbar.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/completion_refresher.py` & `irissqlcli-0.5.4/irissqlcli/completion_refresher.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/config.py` & `irissqlcli-0.5.4/irissqlcli/config.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/irissqlclirc` & `irissqlcli-0.5.4/irissqlcli/irissqlclirc`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/key_bindings.py` & `irissqlcli-0.5.4/irissqlcli/key_bindings.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/magic.py` & `irissqlcli-0.5.4/irissqlcli/magic.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/main.py` & `irissqlcli-0.5.4/irissqlcli/main.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/packages/completion_engine.py` & `irissqlcli-0.5.4/irissqlcli/packages/completion_engine.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/packages/encodingutils.py` & `irissqlcli-0.5.4/irissqlcli/packages/encodingutils.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/packages/filepaths.py` & `irissqlcli-0.5.4/irissqlcli/packages/filepaths.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/packages/parseutils.py` & `irissqlcli-0.5.4/irissqlcli/packages/parseutils.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/packages/prompt_utils.py` & `irissqlcli-0.5.4/irissqlcli/packages/prompt_utils.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/packages/special/dbcommands.py` & `irissqlcli-0.5.4/irissqlcli/packages/special/dbcommands.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/packages/special/favoritequeries.py` & `irissqlcli-0.5.4/irissqlcli/packages/special/favoritequeries.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/packages/special/iocommands.py` & `irissqlcli-0.5.4/irissqlcli/packages/special/iocommands.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/packages/special/main.py` & `irissqlcli-0.5.4/irissqlcli/packages/special/main.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/packages/special/utils.py` & `irissqlcli-0.5.4/irissqlcli/packages/special/utils.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/sqlcompleter.py` & `irissqlcli-0.5.4/irissqlcli/sqlcompleter.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/sqlexecute.py` & `irissqlcli-0.5.4/irissqlcli/sqlexecute.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli/style.py` & `irissqlcli-0.5.4/irissqlcli/style.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/irissqlcli.egg-info/PKG-INFO` & `irissqlcli-0.5.4/irissqlcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irissqlcli
-Version: 0.5.3b2
+Version: 0.5.4
 Summary: CLI for SQL of InterSystems IRIS Databases with auto-completion and syntax highlighting.
 Home-page: https://github.com/caretdev/irissqlcli
 Author: CaretDev
 Author-email: irissqlcli@caretdev.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `irissqlcli-0.5.3b2/irissqlcli.egg-info/SOURCES.txt` & `irissqlcli-0.5.4/irissqlcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/setup.py` & `irissqlcli-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `irissqlcli-0.5.3b2/tests/test_main.py` & `irissqlcli-0.5.4/tests/test_main.py`

 * *Files identical despite different names*

