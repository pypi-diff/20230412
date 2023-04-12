# Comparing `tmp/peek-core-user-3.3.3.tar.gz` & `tmp/peek-core-user-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-core-user-3.3.3.tar", last modified: Mon Nov 14 05:35:45 2022, max compression
+gzip compressed data, was "peek-core-user-3.4.0.tar", last modified: Wed Apr 12 11:04:30 2023, max compression
```

## Comparing `peek-core-user-3.3.3.tar` & `peek-core-user-3.4.0.tar`

### file list

```diff
@@ -1,250 +1,251 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.493359 peek-core-user-3.3.3/
--rw-r--r--   0 root         (0) root         (0)      376 2022-11-14 05:35:45.493359 peek-core-user-3.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      293 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.469359 peek-core-user-3.3.3/peek_core_user/
--rw-r--r--   0 root         (0) root         (0)      460 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      271 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/TempUnitTest.py
--rw-r--r--   0 root         (0) root         (0)     1285 2022-11-14 05:35:45.000000 peek-core-user-3.3.3/peek_core_user/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.470360 peek-core-user-3.3.3/peek_core_user/_private/
--rw-r--r--   0 root         (0) root         (0)      183 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.470360 peek-core-user-3.3.3/peek_core_user/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.470360 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-internal-group-table/
--rw-r--r--   0 root         (0) root         (0)     1643 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     2063 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.471360 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-internal-user-table/
--rw-r--r--   0 root         (0) root         (0)     5971 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     4802 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.471360 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-ldap-setting-table/
--rw-r--r--   0 root         (0) root         (0)     3847 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     2040 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.471360 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     1828 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1626 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.471360 peek-core-user-3.3.3/peek_core_user/_private/admin-app/logged-in-user/
--rw-r--r--   0 root         (0) root         (0)     1673 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.html
--rw-r--r--   0 root         (0) root         (0)     3419 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.472360 peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/
--rw-r--r--   0 root         (0) root         (0)      527 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/InternalGroupTuple.ts
--rw-r--r--   0 root         (0) root         (0)      996 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/InternalUserTuple.ts
--rw-r--r--   0 root         (0) root         (0)      541 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/InternalUserUpdatePasswordAction.ts
--rw-r--r--   0 root         (0) root         (0)      646 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/LdapSettingTuple.ts
--rw-r--r--   0 root         (0) root         (0)      580 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/SettingPropertyTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.472360 peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/constants/
--rw-r--r--   0 root         (0) root         (0)       79 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/constants/UserAuthTargetEnum.ts
--rw-r--r--   0 root         (0) root         (0)     1006 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/user.component.html
--rw-r--r--   0 root         (0) root         (0)      158 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/user.component.ts
--rw-r--r--   0 root         (0) root         (0)     2998 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/admin-app/user.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.472360 peek-core-user-3.3.3/peek_core_user/_private/agent/
--rw-r--r--   0 root         (0) root         (0)      847 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)     1282 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/agent/RpcForLogic.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.473359 peek-core-user-3.3.3/peek_core_user/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      299 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      544 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.475360 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     4602 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/0498d92479c8_implemented_internal_directory.py
--rw-r--r--   0 root         (0) root         (0)      704 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/1176bc54abf3_added_foreign_key_to_user_logged_in.py
--rw-r--r--   0 root         (0) root         (0)     1512 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/2209cf338e6d_added_ldap_table.py
--rw-r--r--   0 root         (0) root         (0)     1160 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/2c6728ebc562_separated_password.py
--rw-r--r--   0 root         (0) root         (0)     2463 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/3a9cddaf05e5_added_settings_table.py
--rw-r--r--   0 root         (0) root         (0)     2186 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/3fd59734e444_removed_string_limits.py
--rw-r--r--   0 root         (0) root         (0)     1096 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/3fec57d8da58_initial.py
--rw-r--r--   0 root         (0) root         (0)     2501 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/43df0e05c728_added_user_import_source.py
--rw-r--r--   0 root         (0) root         (0)      806 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/45c62f8acd87_added_vehical_to_loggedin.py
--rw-r--r--   0 root         (0) root         (0)     1617 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/56d805072d2a_added_importhash.py
--rw-r--r--   0 root         (0) root         (0)      852 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/5e33c6b788fd_removed_unique_logged_in_user.py
--rw-r--r--   0 root         (0) root         (0)      706 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/73d65f042834_removed_foreign_key_from_user_logged_in.py
--rw-r--r--   0 root         (0) root         (0)     1269 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/7e3f668edf0e_updated_settings.py
--rw-r--r--   0 root         (0) root         (0)      663 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/9b65be31926e_timezone_aware.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2664 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/b09fe7b3b31b_add_userkey.py
--rw-r--r--   0 root         (0) root         (0)      829 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/d79da9333e2a_drop_internaluser_rows_from_ldap_for_useruuid_change.py
--rw-r--r--   0 root         (0) root         (0)      756 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/eef485ef2e0e_added_agenturi_column_to_ldapsetting.py
--rw-r--r--   0 root         (0) root         (0)       96 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.476359 peek-core-user-3.3.3/peek_core_user/_private/both-app/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      779 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/plugin-user.module.ts
--rw-r--r--   0 root         (0) root         (0)      667 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/plugin-user.routes.ts
--rw-r--r--   0 root         (0) root         (0)      408 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/plugin-user.text.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.476359 peek-core-user-3.3.3/peek_core_user/_private/both-app/scss/
--rw-r--r--   0 root         (0) root         (0)      560 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/scss/plugin-user.dweb.scss
--rw-r--r--   0 root         (0) root         (0)      519 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/scss/plugin-user.mweb.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.476359 peek-core-user-3.3.3/peek_core_user/_private/both-app/tuples/
--rw-r--r--   0 root         (0) root         (0)      557 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/tuples/UserLoginUiSettingTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.476359 peek-core-user-3.3.3/peek_core_user/_private/both-app/user-login/
--rw-r--r--   0 root         (0) root         (0)     1571 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/user-login/user-login.component.dweb.html
--rw-r--r--   0 root         (0) root         (0)     3217 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/user-login/user-login.component.mweb.html
--rw-r--r--   0 root         (0) root         (0)     5957 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/user-login/user-login.component.ts
--rw-r--r--   0 root         (0) root         (0)      502 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/user-login/user-login.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.477360 peek-core-user-3.3.3/peek_core_user/_private/both-app/user-logout/
--rw-r--r--   0 root         (0) root         (0)      744 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/user-logout/user-logout.component.dweb.html
--rw-r--r--   0 root         (0) root         (0)     1281 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/user-logout/user-logout.component.mweb.html
--rw-r--r--   0 root         (0) root         (0)     2990 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/user-logout/user-logout.component.ts
--rw-r--r--   0 root         (0) root         (0)      507 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-app/user-logout/user-logout.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.477360 peek-core-user-3.3.3/peek_core_user/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)     5572 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/both-assets/plugin_icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.478360 peek-core-user-3.3.3/peek_core_user/_private/client/
--rw-r--r--   0 root         (0) root         (0)     1320 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/client/PluginClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      474 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/client/TupleActionProcessorProxy.py
--rw-r--r--   0 root         (0) root         (0)      466 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/client/TupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.478360 peek-core-user-3.3.3/peek_core_user/_private/ldap_auth/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/ldap_auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9117 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/ldap_auth/ldap_auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.478360 peek-core-user-3.3.3/peek_core_user/_private/server/
--rw-r--r--   0 root         (0) root         (0)     2010 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/AdminTupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)      593 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/ClientTupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     2185 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/ClientTupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)     7126 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/PluginLogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.479359 peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1810 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/InternalGroupTableHandler.py
--rw-r--r--   0 root         (0) root         (0)     4037 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/InternalUserTableHandler.py
--rw-r--r--   0 root         (0) root         (0)      683 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/LdapSettingsHandler.py
--rw-r--r--   0 root         (0) root         (0)     2234 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      836 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.479359 peek-core-user-3.3.3/peek_core_user/_private/server/admin_tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     2875 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/admin_tuple_providers/LoggedInUserStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/admin_tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.480359 peek-core-user-3.3.3/peek_core_user/_private/server/api/
--rw-r--r--   0 root         (0) root         (0)      614 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/api/UserAdminAuthApi.py
--rw-r--r--   0 root         (0) root         (0)     2325 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/api/UserApi.py
--rw-r--r--   0 root         (0) root         (0)     2037 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/api/UserFieldHookApi.py
--rw-r--r--   0 root         (0) root         (0)      888 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/api/UserImportApi.py
--rw-r--r--   0 root         (0) root         (0)     8690 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/api/UserInfoApi.py
--rw-r--r--   0 root         (0) root         (0)     1020 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/api/UserLoginApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.480359 peek-core-user-3.3.3/peek_core_user/_private/server/auth_connectors/
--rw-r--r--   0 root         (0) root         (0)     2751 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/auth_connectors/AuthABC.py
--rw-r--r--   0 root         (0) root         (0)     4945 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/auth_connectors/InternalAuth.py
--rw-r--r--   0 root         (0) root         (0)     9258 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/auth_connectors/LdapAuth.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/auth_connectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.481360 peek-core-user-3.3.3/peek_core_user/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     2104 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/controller/AdminAuthController.py
--rw-r--r--   0 root         (0) root         (0)     2168 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/controller/ImportController.py
--rw-r--r--   0 root         (0) root         (0)    18790 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/controller/LoginLogoutController.py
--rw-r--r--   0 root         (0) root         (0)     1643 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)     2098 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/controller/PasswordUpdateController.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.482360 peek-core-user-3.3.3/peek_core_user/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)      965 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/tuple_providers/GroupDetailTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1843 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/tuple_providers/UserListItemTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     2274 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/tuple_providers/UserLoggedInTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1394 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/tuple_providers/UserLoginUiSettingTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.483359 peek-core-user-3.3.3/peek_core_user/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      937 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     1191 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/storage/DirectoryTuple.py
--rw-r--r--   0 root         (0) root         (0)     1032 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/storage/InternalGroupTuple.py
--rw-r--r--   0 root         (0) root         (0)     1195 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/storage/InternalUserGroupTuple.py
--rw-r--r--   0 root         (0) root         (0)     1290 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/storage/InternalUserPassword.py
--rw-r--r--   0 root         (0) root         (0)     2377 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/storage/InternalUserTuple.py
--rw-r--r--   0 root         (0) root         (0)     1269 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/storage/LdapSetting.py
--rw-r--r--   0 root         (0) root         (0)     8700 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)     1652 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/storage/UserLoggedIn.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.484359 peek-core-user-3.3.3/peek_core_user/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      536 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/tuples/InternalGroupImportResultTuple.py
--rw-r--r--   0 root         (0) root         (0)      534 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/tuples/InternalUserImportResultTuple.py
--rw-r--r--   0 root         (0) root         (0)      447 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/tuples/InternalUserUpdatePasswordAction.py
--rw-r--r--   0 root         (0) root         (0)      696 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/tuples/LdapLoggedInUserTuple.py
--rw-r--r--   0 root         (0) root         (0)     1245 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/tuples/LoggedInUserStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      674 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/tuples/UserLoggedInTuple.py
--rw-r--r--   0 root         (0) root         (0)      504 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/tuples/UserLoginUiSettingTuple.py
--rw-r--r--   0 root         (0) root         (0)      175 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.484359 peek-core-user-3.3.3/peek_core_user/_private/worker/
--rw-r--r--   0 root         (0) root         (0)      972 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/worker/WorkerEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.484359 peek-core-user-3.3.3/peek_core_user/_private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)     3535 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/worker/tasks/UserImportInternalGroupTask.py
--rw-r--r--   0 root         (0) root         (0)     6074 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/worker/tasks/UserImportInternalUserTask.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/_private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.484359 peek-core-user-3.3.3/peek_core_user/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.486359 peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/
--rw-r--r--   0 root         (0) root         (0)    64196 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/add_group.png
--rw-r--r--   0 root         (0) root         (0)    88232 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/add_user.png
--rw-r--r--   0 root         (0) root         (0)     4375 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/configuration.rst
--rw-r--r--   0 root         (0) root         (0)    57815 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/edit-internal-groups.png
--rw-r--r--   0 root         (0) root         (0)    77342 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/edit-internal-user.png
--rw-r--r--   0 root         (0) root         (0)    64921 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/settings-general.png
--rw-r--r--   0 root         (0) root         (0)    45579 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/settings-ldap.png
--rw-r--r--   0 root         (0) root         (0)      256 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.487359 peek-core-user-3.3.3/peek_core_user/admin-doc/logged_in/
--rw-r--r--   0 root         (0) root         (0)      817 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/logged_in/logged_in.rst
--rw-r--r--   0 root         (0) root         (0)    57636 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/logged_in/logout_user.png
--rw-r--r--   0 root         (0) root         (0)    22311 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/logged_in/logout_yes.png
--rw-r--r--   0 root         (0) root         (0)    56963 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/logged_in/manage-logged-in-users.png
--rw-r--r--   0 root         (0) root         (0)      742 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.488360 peek-core-user-3.3.3/peek_core_user/both-doc/
--rw-r--r--   0 root         (0) root         (0)      109 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/both-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)    16799 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/both-doc/login.png
--rw-r--r--   0 root         (0) root         (0)    12482 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/both-doc/login_logout.png
--rwxr-xr-x   0 root         (0) root         (0)      901 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/both-doc/login_logout.rst
--rwxr-xr-x   0 root         (0) root         (0)     1171 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/both-doc/user_button.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.488360 peek-core-user-3.3.3/peek_core_user/plugin-module/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.488360 peek-core-user-3.3.3/peek_core_user/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      307 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)      172 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.488360 peek-core-user-3.3.3/peek_core_user/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      952 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/_private/tuples/LoggedInUserStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      691 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/_private/tuples/UserLoggedInTuple.ts
--rw-r--r--   0 root         (0) root         (0)     2655 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/_private/user-tuple.service.ts
--rw-r--r--   0 root         (0) root         (0)      762 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)       63 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.489359 peek-core-user-3.3.3/peek_core_user/plugin-module/services/
--rw-r--r--   0 root         (0) root         (0)      836 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/services/logged-in.guard.ts
--rw-r--r--   0 root         (0) root         (0)      445 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/services/logged-out.guard.ts
--rw-r--r--   0 root         (0) root         (0)      491 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/services/profile.service.ts
--rw-r--r--   0 root         (0) root         (0)    10343 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/services/user.service.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.489359 peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/
--rw-r--r--   0 root         (0) root         (0)      483 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/GroupDetailTuple.ts
--rw-r--r--   0 root         (0) root         (0)      867 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/UserDetailTuple.ts
--rw-r--r--   0 root         (0) root         (0)      531 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/UserListItemTuple.ts
--rw-r--r--   0 root         (0) root         (0)      268 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.490359 peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/login/
--rw-r--r--   0 root         (0) root         (0)      722 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/login/UserLoginAction.ts
--rw-r--r--   0 root         (0) root         (0)     1012 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/login/UserLoginResponseTuple.ts
--rw-r--r--   0 root         (0) root         (0)      671 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/login/UserLogoutAction.ts
--rw-r--r--   0 root         (0) root         (0)      894 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/login/UserLogoutResponseTuple.ts
--rw-r--r--   0 root         (0) root         (0)     2718 2022-11-14 05:35:45.000000 peek-core-user-3.3.3/peek_core_user/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.491359 peek-core-user-3.3.3/peek_core_user/server/
--rw-r--r--   0 root         (0) root         (0)      354 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/server/UserAdminAuthApiABC.py
--rw-r--r--   0 root         (0) root         (0)     2108 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/server/UserApiABC.py
--rw-r--r--   0 root         (0) root         (0)     1052 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/server/UserDbErrors.py
--rw-r--r--   0 root         (0) root         (0)     1817 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/server/UserFieldHookApiABC.py
--rw-r--r--   0 root         (0) root         (0)     1535 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/server/UserImportApiABC.py
--rw-r--r--   0 root         (0) root         (0)     3687 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/server/UserInfoApiABC.py
--rw-r--r--   0 root         (0) root         (0)      997 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/server/UserLoginApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.492359 peek-core-user-3.3.3/peek_core_user/tuples/
--rw-r--r--   0 root         (0) root         (0)      668 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/DeviceWithUserDetails.py
--rw-r--r--   0 root         (0) root         (0)      436 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/GroupDetailTuple.py
--rw-r--r--   0 root         (0) root         (0)       66 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/UserAuthTarget.py
--rw-r--r--   0 root         (0) root         (0)     1185 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/UserDetailTuple.py
--rw-r--r--   0 root         (0) root         (0)      582 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/UserListItemTuple.py
--rw-r--r--   0 root         (0) root         (0)      518 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/UserLoggedInInfoTuple.py
--rw-r--r--   0 root         (0) root         (0)      274 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.492359 peek-core-user-3.3.3/peek_core_user/tuples/constants/
--rw-r--r--   0 root         (0) root         (0)       70 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/constants/UserAuthTargetEnum.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/constants/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.492359 peek-core-user-3.3.3/peek_core_user/tuples/import_/
--rw-r--r--   0 root         (0) root         (0)      450 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/import_/ImportInternalGroupTuple.py
--rw-r--r--   0 root         (0) root         (0)     1123 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/import_/ImportInternalUserTuple.py
--rw-r--r--   0 root         (0) root         (0)      168 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/import_/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.493359 peek-core-user-3.3.3/peek_core_user/tuples/login/
--rw-r--r--   0 root         (0) root         (0)      715 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/login/UserLoginAction.py
--rw-r--r--   0 root         (0) root         (0)     1163 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/login/UserLoginResponseTuple.py
--rw-r--r--   0 root         (0) root         (0)      658 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/login/UserLogoutAction.py
--rw-r--r--   0 root         (0) root         (0)      993 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/login/UserLogoutResponseTuple.py
--rw-r--r--   0 root         (0) root         (0)      168 2022-11-14 05:34:27.000000 peek-core-user-3.3.3/peek_core_user/tuples/login/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 05:35:45.469359 peek-core-user-3.3.3/peek_core_user.egg-info/
--rw-r--r--   0 root         (0) root         (0)      376 2022-11-14 05:35:45.000000 peek-core-user-3.3.3/peek_core_user.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11289 2022-11-14 05:35:45.000000 peek-core-user-3.3.3/peek_core_user.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:35:45.000000 peek-core-user-3.3.3/peek_core_user.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 05:35:45.000000 peek-core-user-3.3.3/peek_core_user.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       44 2022-11-14 05:35:45.000000 peek-core-user-3.3.3/peek_core_user.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-11-14 05:35:45.000000 peek-core-user-3.3.3/peek_core_user.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-14 05:35:45.493359 peek-core-user-3.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2703 2022-11-14 05:35:45.000000 peek-core-user-3.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.477213 peek-core-user-3.4.0/
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-12 11:04:30.477213 peek-core-user-3.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      293 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.466213 peek-core-user-3.4.0/peek_core_user/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/TempUnitTest.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-04-12 11:04:30.000000 peek-core-user-3.4.0/peek_core_user/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.467213 peek-core-user-3.4.0/peek_core_user/_private/
+-rw-r--r--   0 root         (0) root         (0)      183 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.467213 peek-core-user-3.4.0/peek_core_user/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.467213 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-internal-group-table/
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     2063 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.467213 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-internal-user-table/
+-rw-r--r--   0 root         (0) root         (0)     5971 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     4802 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.467213 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-ldap-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     4398 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.467213 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.467213 peek-core-user-3.4.0/peek_core_user/_private/admin-app/logged-in-user/
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.html
+-rw-r--r--   0 root         (0) root         (0)     3419 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.468213 peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)      527 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/InternalGroupTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      996 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/InternalUserTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      541 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/InternalUserUpdatePasswordAction.ts
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/LdapSettingTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/SettingPropertyTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.468213 peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/constants/
+-rw-r--r--   0 root         (0) root         (0)       79 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/constants/UserAuthTargetEnum.ts
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/user.component.html
+-rw-r--r--   0 root         (0) root         (0)      158 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/user.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/admin-app/user.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.468213 peek-core-user-3.4.0/peek_core_user/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)      847 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/agent/RpcForLogic.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.468213 peek-core-user-3.4.0/peek_core_user/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      299 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.469213 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     4602 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/0498d92479c8_implemented_internal_directory.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/1176bc54abf3_added_foreign_key_to_user_logged_in.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/2209cf338e6d_added_ldap_table.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/2c6728ebc562_separated_password.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/3a9cddaf05e5_added_settings_table.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/3fd59734e444_removed_string_limits.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/3fec57d8da58_initial.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/43df0e05c728_added_user_import_source.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/45c62f8acd87_added_vehical_to_loggedin.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/56d805072d2a_added_importhash.py
+-rw-r--r--   0 root         (0) root         (0)      852 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/5e33c6b788fd_removed_unique_logged_in_user.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/73d65f042834_removed_foreign_key_from_user_logged_in.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/7e3f668edf0e_updated_settings.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/9b65be31926e_timezone_aware.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2664 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/b09fe7b3b31b_add_userkey.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/d03db0fcb600_convert_userkey_and_username_to_all_.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/d79da9333e2a_drop_internaluser_rows_from_ldap_for_useruuid_change.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/eef485ef2e0e_added_agenturi_column_to_ldapsetting.py
+-rw-r--r--   0 root         (0) root         (0)       95 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.469213 peek-core-user-3.4.0/peek_core_user/_private/both-app/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/plugin-user.module.ts
+-rw-r--r--   0 root         (0) root         (0)      667 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/plugin-user.routes.ts
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/plugin-user.text.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.469213 peek-core-user-3.4.0/peek_core_user/_private/both-app/scss/
+-rw-r--r--   0 root         (0) root         (0)      560 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/scss/plugin-user.dweb.scss
+-rw-r--r--   0 root         (0) root         (0)      519 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/scss/plugin-user.mweb.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.469213 peek-core-user-3.4.0/peek_core_user/_private/both-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)      557 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/tuples/UserLoginUiSettingTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.470213 peek-core-user-3.4.0/peek_core_user/_private/both-app/user-login/
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/user-login/user-login.component.dweb.html
+-rw-r--r--   0 root         (0) root         (0)     3209 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/user-login/user-login.component.mweb.html
+-rw-r--r--   0 root         (0) root         (0)     6145 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/user-login/user-login.component.ts
+-rw-r--r--   0 root         (0) root         (0)      502 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/user-login/user-login.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.470213 peek-core-user-3.4.0/peek_core_user/_private/both-app/user-logout/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/user-logout/user-logout.component.dweb.html
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/user-logout/user-logout.component.mweb.html
+-rw-r--r--   0 root         (0) root         (0)     2990 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/user-logout/user-logout.component.ts
+-rw-r--r--   0 root         (0) root         (0)      507 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-app/user-logout/user-logout.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.470213 peek-core-user-3.4.0/peek_core_user/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)     5572 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/both-assets/plugin_icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.470213 peek-core-user-3.4.0/peek_core_user/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/client/PluginClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      474 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/client/TupleActionProcessorProxy.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/client/TupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.470213 peek-core-user-3.4.0/peek_core_user/_private/ldap_auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/ldap_auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11154 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/ldap_auth/ldap_auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.470213 peek-core-user-3.4.0/peek_core_user/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/AdminTupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)      593 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/ClientTupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/ClientTupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)     7217 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/PluginLogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.471213 peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/InternalGroupTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)     4037 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/InternalUserTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/LdapSettingsHandler.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.471213 peek-core-user-3.4.0/peek_core_user/_private/server/admin_tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/admin_tuple_providers/LoggedInUserStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/admin_tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.471213 peek-core-user-3.4.0/peek_core_user/_private/server/api/
+-rw-r--r--   0 root         (0) root         (0)      714 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/api/UserAdminAuthApi.py
+-rw-r--r--   0 root         (0) root         (0)     2573 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/api/UserApi.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/api/UserFieldHookApi.py
+-rw-r--r--   0 root         (0) root         (0)      991 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/api/UserImportApi.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/api/UserInfoApi.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/api/UserLoginApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.471213 peek-core-user-3.4.0/peek_core_user/_private/server/auth_connectors/
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/auth_connectors/AuthABC.py
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/auth_connectors/InternalAuth.py
+-rw-r--r--   0 root         (0) root         (0)     9769 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/auth_connectors/LdapAuth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/auth_connectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.472213 peek-core-user-3.4.0/peek_core_user/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/controller/AdminAuthController.py
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/controller/ImportController.py
+-rw-r--r--   0 root         (0) root         (0)    18854 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/controller/LoginLogoutController.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/controller/PasswordUpdateController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.472213 peek-core-user-3.4.0/peek_core_user/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)      965 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/tuple_providers/GroupDetailTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/tuple_providers/UserListItemTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/tuple_providers/UserLoggedInTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/tuple_providers/UserLoginUiSettingTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.472213 peek-core-user-3.4.0/peek_core_user/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      937 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     1191 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/storage/DirectoryTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/storage/InternalGroupTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/storage/InternalUserGroupTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/storage/InternalUserPassword.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/storage/InternalUserTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1269 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/storage/LdapSetting.py
+-rw-r--r--   0 root         (0) root         (0)     9046 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/storage/UserLoggedIn.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.473213 peek-core-user-3.4.0/peek_core_user/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      536 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/tuples/InternalGroupImportResultTuple.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/tuples/InternalUserImportResultTuple.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/tuples/InternalUserUpdatePasswordAction.py
+-rw-r--r--   0 root         (0) root         (0)      696 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/tuples/LdapLoggedInUserTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/tuples/LoggedInUserStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/tuples/UserLoggedInTuple.py
+-rw-r--r--   0 root         (0) root         (0)      504 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/tuples/UserLoginUiSettingTuple.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.473213 peek-core-user-3.4.0/peek_core_user/_private/worker/
+-rw-r--r--   0 root         (0) root         (0)      972 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/worker/WorkerEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.473213 peek-core-user-3.4.0/peek_core_user/_private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)     3590 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/worker/tasks/UserImportInternalGroupTask.py
+-rw-r--r--   0 root         (0) root         (0)     6341 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/worker/tasks/UserImportInternalUserTask.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/_private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.473213 peek-core-user-3.4.0/peek_core_user/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.474213 peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/
+-rw-r--r--   0 root         (0) root         (0)    64196 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/add_group.png
+-rw-r--r--   0 root         (0) root         (0)    88232 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/add_user.png
+-rw-r--r--   0 root         (0) root         (0)     4375 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)    57815 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/edit-internal-groups.png
+-rw-r--r--   0 root         (0) root         (0)    77342 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/edit-internal-user.png
+-rw-r--r--   0 root         (0) root         (0)    64921 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/settings-general.png
+-rw-r--r--   0 root         (0) root         (0)    45579 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/settings-ldap.png
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.474213 peek-core-user-3.4.0/peek_core_user/admin-doc/logged_in/
+-rw-r--r--   0 root         (0) root         (0)      817 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/logged_in/logged_in.rst
+-rw-r--r--   0 root         (0) root         (0)    57636 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/logged_in/logout_user.png
+-rw-r--r--   0 root         (0) root         (0)    22311 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/logged_in/logout_yes.png
+-rw-r--r--   0 root         (0) root         (0)    56963 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/logged_in/manage-logged-in-users.png
+-rw-r--r--   0 root         (0) root         (0)      742 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.474213 peek-core-user-3.4.0/peek_core_user/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      109 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/both-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)    16799 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/both-doc/login.png
+-rw-r--r--   0 root         (0) root         (0)    12482 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/both-doc/login_logout.png
+-rwxr-xr-x   0 root         (0) root         (0)      901 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/both-doc/login_logout.rst
+-rwxr-xr-x   0 root         (0) root         (0)     1171 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/both-doc/user_button.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.474213 peek-core-user-3.4.0/peek_core_user/plugin-module/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.474213 peek-core-user-3.4.0/peek_core_user/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      307 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.475213 peek-core-user-3.4.0/peek_core_user/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      952 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/_private/tuples/LoggedInUserStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      691 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/_private/tuples/UserLoggedInTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/_private/user-tuple.service.ts
+-rw-r--r--   0 root         (0) root         (0)      762 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.475213 peek-core-user-3.4.0/peek_core_user/plugin-module/services/
+-rw-r--r--   0 root         (0) root         (0)      836 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/services/logged-in.guard.ts
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/services/logged-out.guard.ts
+-rw-r--r--   0 root         (0) root         (0)      491 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/services/profile.service.ts
+-rw-r--r--   0 root         (0) root         (0)    10343 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/services/user.service.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.475213 peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/
+-rw-r--r--   0 root         (0) root         (0)      483 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/GroupDetailTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      867 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/UserDetailTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/UserListItemTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      268 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.475213 peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/login/
+-rw-r--r--   0 root         (0) root         (0)      722 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/login/UserLoginAction.ts
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/login/UserLoginResponseTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      671 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/login/UserLogoutAction.ts
+-rw-r--r--   0 root         (0) root         (0)      894 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/login/UserLogoutResponseTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-04-12 11:04:30.000000 peek-core-user-3.4.0/peek_core_user/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.476213 peek-core-user-3.4.0/peek_core_user/server/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/server/UserAdminAuthApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/server/UserApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/server/UserDbErrors.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/server/UserFieldHookApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/server/UserImportApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     3782 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/server/UserInfoApiABC.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/server/UserLoginApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.476213 peek-core-user-3.4.0/peek_core_user/tuples/
+-rw-r--r--   0 root         (0) root         (0)      668 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/DeviceWithUserDetails.py
+-rw-r--r--   0 root         (0) root         (0)      436 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/GroupDetailTuple.py
+-rw-r--r--   0 root         (0) root         (0)       66 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/UserAuthTarget.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/UserDetailTuple.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/UserListItemTuple.py
+-rw-r--r--   0 root         (0) root         (0)      518 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/UserLoggedInInfoTuple.py
+-rw-r--r--   0 root         (0) root         (0)      274 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.476213 peek-core-user-3.4.0/peek_core_user/tuples/constants/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/constants/UserAuthTargetEnum.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/constants/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.476213 peek-core-user-3.4.0/peek_core_user/tuples/import_/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/import_/ImportInternalGroupTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/import_/ImportInternalUserTuple.py
+-rw-r--r--   0 root         (0) root         (0)      168 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/import_/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.476213 peek-core-user-3.4.0/peek_core_user/tuples/login/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/login/UserLoginAction.py
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/login/UserLoginResponseTuple.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/login/UserLogoutAction.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/login/UserLogoutResponseTuple.py
+-rw-r--r--   0 root         (0) root         (0)      168 2023-04-12 11:03:18.000000 peek-core-user-3.4.0/peek_core_user/tuples/login/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 11:04:30.467213 peek-core-user-3.4.0/peek_core_user.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      376 2023-04-12 11:04:30.000000 peek-core-user-3.4.0/peek_core_user.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11383 2023-04-12 11:04:30.000000 peek-core-user-3.4.0/peek_core_user.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:30.000000 peek-core-user-3.4.0/peek_core_user.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 11:04:30.000000 peek-core-user-3.4.0/peek_core_user.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-12 11:04:30.000000 peek-core-user-3.4.0/peek_core_user.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-12 11:04:30.000000 peek-core-user-3.4.0/peek_core_user.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-12 11:04:30.477213 peek-core-user-3.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-04-12 11:04:30.000000 peek-core-user-3.4.0/setup.py
```

### Comparing `peek-core-user-3.3.3/peek_core_user/__init__.py` & `peek-core-user-3.4.0/peek_core_user/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 from peek_plugin_base.agent.PluginAgentEntryHookABC import PluginAgentEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.worker.PluginWorkerEntryHookABC import PluginWorkerEntryHookABC
 
-__version__ = '3.3.3'
+__version__ = '3.4.0'
 
 
 def peekFieldEntryHook() -> Type[PluginClientEntryHookABC]:
     from peek_core_user._private.client.PluginClientEntryHook import (
         PluginClientEntryHook,
     )
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.html` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-internal-group-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.html` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-internal-user-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.html` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,117 +1,121 @@
 <div class="panel panel-default">
     <div class="panel-heading">
-        Edit Internal Groups
+        Edit LDAP Settings
         <div class="btn-toolbar pull-right">
             <div class="btn-group">
                 <div (click)="save()" class="btn btn-default btn-sm">Save</div>
                 <div (click)="loader.load()" class="btn btn-default btn-sm">
                     Reset
                 </div>
                 <div (click)="addRow()" class="btn btn-default btn-sm">Add</div>
             </div>
         </div>
     </div>
     <div class="panel-body">
+        <p *ngIf="(items?.length || 0) == 0">
+            There are no LDAP Settings, Please create one with the Add button
+        </p>
         <table class="table">
             <tbody *ngFor="let item of items">
-            <tr>
-                <td>
-                    Title
-                    <input
-                        [(ngModel)]="item.ldapTitle"
-                        class="form-control input-sm"
-                        required
-                        type="text"
-                    />
-                </td>
-                <td>
-                    URI
-                    <input
-                        [(ngModel)]="item.ldapUri"
-                        class="form-control input-sm"
-                        required
-                        type="text"
-                    />
-                </td>
-                <td>
-                    Domain
-                    <input
-                        [(ngModel)]="item.ldapDomain"
-                        class="form-control input-sm"
-                        required
-                        type="text"
-                    />
-                </td>
-                <td>
-                    <button
-                        (click)="removeRow(item)"
-                        [nzSize]="size"
-                        nz-button
-                        nzJustify="right"
-                        nzShape="circle"
-                        nzType="default"
-                    >
-                        <i nz-icon nzType="close"> </i>
-                    </button>
-                </td>
-            </tr>
-            <tr>
-                <td colspan="3">
-                    CN Folders
-                    <input
-                        [(ngModel)]="item.ldapCNFolders"
-                        class="form-control input-sm"
-                        required
-                        type="text"
-                    />
-                </td>
-                <td>
-                    For Admin
-                    <nz-switch [(ngModel)]="item.adminEnabled"></nz-switch>
-                </td>
-            </tr>
-            <tr>
-                <td colspan="3">
-                    OU Folders
-                    <input
-                        [(ngModel)]="item.ldapOUFolders"
-                        class="form-control input-sm"
-                        required
-                        type="text"
-                    />
-                </td>
-                <td>
-                    For Office
-                    <nz-switch
-                        [(ngModel)]="item.desktopEnabled"
-                    ></nz-switch>
-                </td>
-            </tr>
-            <tr>
-                <td colspan="3">
-                    Groups
-                    <input
-                        [(ngModel)]="item.ldapGroups"
-                        class="form-control input-sm"
-                        required
-                        type="text"
-                    />
-                </td>
-                <td>
-                    For Field
-                    <nz-switch [(ngModel)]="item.mobileEnabled"></nz-switch>
-                </td>
-            </tr>
-            <tr>
-                <td colspan="3">
-                    Agent Host
-                    <input
-                        [(ngModel)]="item.agentHost"
-                        class="form-control input-sm" type="text"
-                    />
-                </td>
-            </tr>
+                <tr>
+                    <td>
+                        Title
+                        <input
+                            [(ngModel)]="item.ldapTitle"
+                            class="form-control input-sm"
+                            required
+                            type="text"
+                        />
+                    </td>
+                    <td>
+                        URI
+                        <input
+                            [(ngModel)]="item.ldapUri"
+                            class="form-control input-sm"
+                            required
+                            type="text"
+                        />
+                    </td>
+                    <td>
+                        Domain
+                        <input
+                            [(ngModel)]="item.ldapDomain"
+                            class="form-control input-sm"
+                            required
+                            type="text"
+                        />
+                    </td>
+                    <td>
+                        <button
+                            (click)="removeRow(item)"
+                            [nzSize]="size"
+                            nz-button
+                            nzJustify="right"
+                            nzShape="circle"
+                            nzType="default"
+                        >
+                            <i nz-icon nzType="close"> </i>
+                        </button>
+                    </td>
+                </tr>
+                <tr>
+                    <td colspan="3">
+                        CN Folders
+                        <input
+                            [(ngModel)]="item.ldapCNFolders"
+                            class="form-control input-sm"
+                            required
+                            type="text"
+                        />
+                    </td>
+                    <td>
+                        For Admin
+                        <nz-switch [(ngModel)]="item.adminEnabled"></nz-switch>
+                    </td>
+                </tr>
+                <tr>
+                    <td colspan="3">
+                        OU Folders
+                        <input
+                            [(ngModel)]="item.ldapOUFolders"
+                            class="form-control input-sm"
+                            required
+                            type="text"
+                        />
+                    </td>
+                    <td>
+                        For Office
+                        <nz-switch
+                            [(ngModel)]="item.desktopEnabled"
+                        ></nz-switch>
+                    </td>
+                </tr>
+                <tr>
+                    <td colspan="3">
+                        Groups
+                        <input
+                            [(ngModel)]="item.ldapGroups"
+                            class="form-control input-sm"
+                            required
+                            type="text"
+                        />
+                    </td>
+                    <td>
+                        For Field
+                        <nz-switch [(ngModel)]="item.mobileEnabled"></nz-switch>
+                    </td>
+                </tr>
+                <tr>
+                    <td colspan="3">
+                        Agent Host
+                        <input
+                            [(ngModel)]="item.agentHost"
+                            class="form-control input-sm"
+                            type="text"
+                        />
+                    </td>
+                </tr>
             </tbody>
         </table>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
-Edit Internal Groups
+Edit LDAP Settings
 click)="save()" class="btn btn-default btn-sm">Save
 click)="loader.load()" class="btn btn-default btn-sm"> Reset
 click)="addRow()" class="btn btn-default btn-sm">Add
+ngIf="(items?.length || 0) == 0"> There are no LDAP Settings, Please create one
+with the Add button
 Title                       URI                       Domain                       click)="removeRow(item)"
 (ngModel)]="item.ldapTitle" (ngModel)]="item.ldapUri" (ngModel)]="item.ldapDomain" [nzSize]="size" nz-button
 class="form-control input-  class="form-control       class="form-control input-   nzJustify="right"
 sm" required type="text" /> input-sm" required        sm" required type="text" />  nzShape="circle"
                             type="text" />                                         nzType="default" >
 CN Folders                                                                         For Admin
 (ngModel)]="item.ldapCNFolders" class="form-control input-sm" required type="text" (ngModel)]="item.adminEnabled">
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-ldap-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-setting-table/edit.component.html` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.html` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/logged-in-user/logged-in-user.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/InternalGroupTuple.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/InternalGroupTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/InternalUserTuple.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/InternalUserTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/InternalUserUpdatePasswordAction.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/InternalUserUpdatePasswordAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/LdapSettingTuple.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/LdapSettingTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/tuples/SettingPropertyTuple.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/tuples/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/user.component.html` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/user.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/admin-app/user.module.ts` & `peek-core-user-3.4.0/peek_core_user/_private/admin-app/user.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/agent/AgentEntryHook.py` & `peek-core-user-3.4.0/peek_core_user/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/agent/RpcForLogic.py` & `peek-core-user-3.4.0/peek_core_user/_private/agent/RpcForLogic.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/script.py.mako` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/script.py.mako`

 * *Files 4% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 
 from alembic import op
 import sqlalchemy as sa
 import geoalchemy2
 ${imports if imports else ""}
 
 def upgrade():
-${upgrades if upgrades else "pass"}
+    ${upgrades if upgrades else "pass"}
 
 
 def downgrade():
-${downgrades if downgrades else "pass"}
+    ${downgrades if downgrades else "pass"}
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/0498d92479c8_implemented_internal_directory.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/0498d92479c8_implemented_internal_directory.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/1176bc54abf3_added_foreign_key_to_user_logged_in.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/1176bc54abf3_added_foreign_key_to_user_logged_in.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/2209cf338e6d_added_ldap_table.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/2209cf338e6d_added_ldap_table.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/2c6728ebc562_separated_password.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/2c6728ebc562_separated_password.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/3a9cddaf05e5_added_settings_table.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/3a9cddaf05e5_added_settings_table.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/3fd59734e444_removed_string_limits.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/3fd59734e444_removed_string_limits.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/3fec57d8da58_initial.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/3fec57d8da58_initial.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/43df0e05c728_added_user_import_source.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/43df0e05c728_added_user_import_source.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/45c62f8acd87_added_vehical_to_loggedin.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/45c62f8acd87_added_vehical_to_loggedin.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/56d805072d2a_added_importhash.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/56d805072d2a_added_importhash.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/5e33c6b788fd_removed_unique_logged_in_user.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/5e33c6b788fd_removed_unique_logged_in_user.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/73d65f042834_removed_foreign_key_from_user_logged_in.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/73d65f042834_removed_foreign_key_from_user_logged_in.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/7e3f668edf0e_updated_settings.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/7e3f668edf0e_updated_settings.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/9b65be31926e_timezone_aware.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/9b65be31926e_timezone_aware.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/b09fe7b3b31b_add_userkey.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/b09fe7b3b31b_add_userkey.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/d79da9333e2a_drop_internaluser_rows_from_ldap_for_useruuid_change.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/d79da9333e2a_drop_internaluser_rows_from_ldap_for_useruuid_change.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/alembic/versions/eef485ef2e0e_added_agenturi_column_to_ldapsetting.py` & `peek-core-user-3.4.0/peek_core_user/_private/alembic/versions/eef485ef2e0e_added_agenturi_column_to_ldapsetting.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/plugin-user.module.ts` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/plugin-user.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/plugin-user.routes.ts` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/plugin-user.routes.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/scss/plugin-user.dweb.scss` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/scss/plugin-user.dweb.scss`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/scss/plugin-user.mweb.scss` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/scss/plugin-user.mweb.scss`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/tuples/UserLoginUiSettingTuple.ts` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/tuples/UserLoginUiSettingTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/user-login/user-login.component.dweb.html` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/user-login/user-login.component.dweb.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 <div class="plugin-user">
     <h4>Login to Peek</h4>
 
     <form (keyup.enter)="doLogin()" autocomplete="off" novalidate>
         <fieldset [disabled]="isAuthenticating$ | async">
             <div class="form-group">
                 <input
-                    [(ngModel)]="selectedUser.userName"
+                    [(ngModel)]="typedUserName"
                     class="form-control"
                     id="username"
-                    name="password"
+                    name="username"
                     placeholder="Username"
                     type="text"
                 />
             </div>
 
             <!-- Login with user input box -->
             <div class="form-group">
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/user-login/user-login.component.mweb.html` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/user-login/user-login.component.mweb.html`

 * *Files 7% similar despite different names*

```diff
@@ -55,18 +55,18 @@
                 >
                     <option *ngFor="let user of users" [value]="user.userId">
                         {{webDisplayText(user)}}
                     </option>
                 </select>
                 <input
                     *ngIf="!setting.showUsersAsList"
-                    [(ngModel)]="selectedUser.userName"
+                    [(ngModel)]="typedUserName"
                     class="form-control"
                     id="username"
-                    name="password"
+                    name="username"
                     type="text"
                 />
             </div>
 
             <!-- Login with user input box -->
             <div class="form-group">
                 <label class="user-message" for="password">Password :</label>
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/user-login/user-login.component.ts` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/user-login/user-login.component.ts`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,22 @@
             .pipe(filter((items) => items.length != 0))
             .subscribe((tuples: UserLoginUiSettingTuple[]) => {
                 this.setting = tuples[0];
                 if (this.setting.showUsersAsList) this.loadUsersList();
             });
     }
 
+    get typedUserName(): string {
+        return this.selectedUser.userName;
+    }
+
+    set typedUserName(value: string) {
+        this.selectedUser.userName = value.toLowerCase();
+    }
+
     get isAuthenticating(): boolean {
         return this.isAuthenticating$.getValue();
     }
 
     set isAuthenticating(value) {
         this.isAuthenticating$.next(value);
     }
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/user-logout/user-logout.component.dweb.html` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/user-logout/user-logout.component.dweb.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/user-logout/user-logout.component.mweb.html` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/user-logout/user-logout.component.mweb.html`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-app/user-logout/user-logout.component.ts` & `peek-core-user-3.4.0/peek_core_user/_private/both-app/user-logout/user-logout.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/both-assets/plugin_icon.png` & `peek-core-user-3.4.0/peek_core_user/_private/both-assets/plugin_icon.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/client/PluginClientEntryHook.py` & `peek-core-user-3.4.0/peek_core_user/_private/client/PluginClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/ldap_auth/ldap_auth.py` & `peek-core-user-3.4.0/peek_core_user/_private/ldap_auth/ldap_auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 {'objectClass': [b'top', b'person', b'organizationalPerson', b'user'], 'cn': [b'attest'],
- 'givenName': [b'attest'],‰
+ 'givenName': [b'attest'],
  'distinguishedName': [b'CN=attest,OU=testou,DC=synad,DC=synerty,DC=com'],
  'instanceType': [b'4'], 'whenCreated': [b'20170505160836.0Z'],
  'whenChanged': [b'20190606130621.0Z'], 'displayName': [b'attest'],
  'uSNCreated': [b'16498'],
  'memberOf': [b'CN=Domain Admins,CN=Users,DC=synad,DC=synerty,DC=com',
               b'CN=Enterprise Admins,CN=Users,DC=synad,DC=synerty,DC=com',
               b'CN=Administrators,CN=Builtin,DC=synad,DC=synerty,DC=com'],
@@ -27,18 +27,23 @@
 from typing import List
 from typing import Optional
 from typing import Tuple
 
 import ldap
 from twisted.cred.error import LoginFailed
 
+from peek_core_user._private.PluginNames import userPluginTuplePrefix
 from peek_core_user._private.storage import LdapSetting
+from peek_core_user._private.storage.InternalUserTuple import InternalUserTuple
 from peek_core_user._private.tuples.LdapLoggedInUserTuple import (
     LdapLoggedInUserTuple,
 )
+from peek_core_user.tuples.constants.UserAuthTargetEnum import (
+    UserAuthTargetEnum,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def checkLdapAuth(
     username: str,
     password: str,
@@ -52,29 +57,30 @@
         conn.set_option(ldap.OPT_REFERRALS, 0)
 
         # make the connection
         conn.simple_bind_s(
             "%s@%s" % (username.split("@")[0], ldapSetting.ldapDomain), password
         )
         logger.info(
-            "Connected to LDAP server %s for user %s",
-            ldapSetting.ldapDomain,
+            "User=%s, Connected to LDAP server %s",
             username,
+            ldapSetting.ldapDomain,
         )
 
         if userUuid:
             ldapFilter = (
                 "(&(objectCategory=person)(objectClass=user)(objectSid=%s))"
                 % userUuid
             )
         else:
             ldapFilter = (
                 "(&(objectCategory=person)(objectClass=user)(sAMAccountName=%s))"
                 % username.split("@")[0]
             )
+        logger.debug("User=%s, LDAP user query: %s", username, ldapFilter)
 
         dcParts = ",".join(
             ["DC=%s" % part for part in ldapSetting.ldapDomain.split(".")]
         )
 
         ldapBases = []
         if ldapSetting.ldapOUFolders:
@@ -83,46 +89,76 @@
             )
         if ldapSetting.ldapCNFolders:
             ldapBases += _makeLdapBase(
                 ldapSetting.ldapCNFolders, username, "CN"
             )
 
         if not ldapBases:
+            logger.debug(
+                "User=%s, LDAP OU and/or CN search paths must be set.", username
+            )
             raise LoginFailed(
                 "LDAPAuth: LDAP OU and/or CN search paths must be set."
             )
 
         userDetails = None
         for ldapBase in ldapBases:
             ldapBase = "%s,%s" % (ldapBase, dcParts)
-            logger.debug("LDAP Base: %s", ldapBase)
+            logger.debug(
+                "User=%s, Searching in LDAP Base: %s, for LDAP Filter: %s",
+                username,
+                ldapBase,
+                ldapFilter,
+            )
 
             try:
                 # Example Base: 'CN=atuser1,CN=Users,DC=synad,DC=synerty,DC=com'
                 userDetails = conn.search_st(
                     ldapBase, ldap.SCOPE_SUBTREE, ldapFilter, None, 0, 10
                 )
 
                 if userDetails:
                     break
 
+                logger.debug(
+                    "User=%s, Checking next, user was not found in: %s",
+                    username,
+                    ldapBase,
+                )
+
             except ldap.NO_SUCH_OBJECT:
-                logger.warning("CN or OU doesn't exist : %s", ldapBase)
+                logger.warning(
+                    "User=%s, CN or OU doesn't exist : %s", username, ldapBase
+                )
 
     except ldap.NO_SUCH_OBJECT:
+        logger.info(
+            "User=%s, was not found in any LDAP bases, NO_SUCH_OBJECT", username
+        )
         raise LoginFailed(
-            "LDAPAuth: An internal error occurred, ask admin to check "
-            "Attune logs"
+            "LDAPAuth: A user with username %s was not found, ask admin to "
+            "check Peek logs" % username
         )
 
     except ldap.INVALID_CREDENTIALS:
-        raise LoginFailed("LDAPAuth: Username or password is incorrect")
+        logger.info(
+            "User=%s, provided an incorrect username or password, INVALID_CREDENTIALS"
+        )
+        raise LoginFailed(
+            "LDAPAuth: Username or password is incorrect for %s" % username
+        )
 
     if not userDetails:
-        raise LoginFailed("LDAPAuth: User doesn't belong to the correct CN/OUs")
+        logger.info(
+            "User=%s, was not found in any LDAP bases, 'not userDetails'",
+            username,
+        )
+        raise LoginFailed(
+            "LDAPAuth: User %s doesn't belong to the correct CN/OUs" % username
+        )
 
     userDetails = userDetails[0][1]
 
     distinguishedName = userDetails.get("distinguishedName")[0].decode()
     primaryGroupId = userDetails.get("primaryGroupID")[0].decode()
     objectSid = userDetails.get("objectSid")[0]
     # python-ldap doesn't include key `memberOf` in search result
@@ -131,26 +167,32 @@
 
     decodedSid = _decodeSid(objectSid)
     primaryGroupSid = (
         "-".join(decodedSid.split("-")[:-1]) + "-" + primaryGroupId
     )
 
     ldapFilter = "(objectSid=%s)" % primaryGroupSid
+    logger.debug(
+        "User=%s, Primary group details LDAP filter: %s", username, ldapFilter
+    )
     primGroupDetails = conn.search_st(
         dcParts, ldap.SCOPE_SUBTREE, ldapFilter, None, 0, 10
     )
     memberOfSet.add(primGroupDetails[0][1].get("distinguishedName")[0])
 
     # find all it's groups and groups of those groups
     # The magic number in this filter allows us to fetch the groups of
     # a group.
     ldapFilter = (
         "(&(objectCategory=group)(member:1.2.840.113556.1.4.1941:=%s))"
         % (_escapeParensForLdapFilter(distinguishedName),)
     )
+    logger.debug(
+        "User=%s, Using recursive groups filter: %s", username, ldapFilter
+    )
     logger.info("Fetching groups from the LDAP server for user %s", username)
     groupDetails = conn.search_st(
         ",".join(distinguishedName.split(",")[1:]),
         ldap.SCOPE_SUBTREE,
         ldapFilter,
         None,
         0,
@@ -165,30 +207,49 @@
     groups = []
     for memberOf in memberOfSet:
         group = memberOf.decode().split(",")[0]
         if "=" in group:
             group = group.split("=")[1]
         groups.append(group)
 
+    logger.debug("User %s, is a member of groups: %s", username, groups)
+
     userTitle = None
-    if userDetails["displayName"]:
+    if userDetails.get("displayName"):
         userTitle = userDetails["displayName"][0].decode()
 
     email = None
-    if userDetails["userPrincipalName"]:
+    if userDetails.get("userPrincipalName"):
         email = userDetails["userPrincipalName"][0].decode()
 
     if not userUuid:
         userUuid = _decodeSid(objectSid)
 
     if ldapSetting.ldapGroups:
         ldapGroups = set([s.strip() for s in ldapSetting.ldapGroups.split(",")])
 
+        logger.debug(
+            "User=%s, Checking if user is a member of groups: %s",
+            username,
+            groups,
+        )
+
         if not ldapGroups & set(groups):
-            raise LoginFailed("User is not a member of an authorised group")
+            logger.info(
+                "User=%s, is not a member of any authorised group, 'not ldapGroups & set(groups)'",
+                username,
+            )
+            raise LoginFailed(
+                "User %s is not a member of an authorised group" % username
+            )
+
+        logger.debug(
+            "User=%s, is a member of specified groups. Proceeding with login",
+            username,
+        )
 
     ldapLoggedInUser = LdapLoggedInUserTuple(
         username=username,
         userTitle=userTitle,
         userUuid=userUuid,
         email=email,
         ldapName=ldapSetting.ldapTitle,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/AdminTupleDataObservable.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/AdminTupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/ClientTupleActionProcessor.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/ClientTupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/ClientTupleDataObservable.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/ClientTupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/PluginLogicEntryHook.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/PluginLogicEntryHook.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,18 @@
 
         loadStorageTuples()
 
         from peek_core_user.tuples import loadPublicTuples
 
         loadPublicTuples()
 
+        # ----------------
+        # Setup our API
+        self._userApi = UserApi()
+
         logger.debug("loaded")
 
     def start(self):
         """Start
 
         This will be called when the plugin is loaded, just after the db is migrated.
         Place any custom initialiastion steps here.
@@ -152,17 +156,17 @@
         # ----------------
         # Login / Logout Controller
         adminAuthController = AdminAuthController(self.dbSessionCreator)
         self._handlers.append(adminAuthController)
 
         # ----------------
         # Setup our API
-        self._userApi = UserApi(
-            deviceApi,
+        self._userApi.setStartValues(
             self.dbSessionCreator,
+            deviceApi,
             importController,
             loginLogoutController,
             adminAuthController,
         )
 
         # ----------------
         # Main Controller
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/InternalGroupTableHandler.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/InternalGroupTableHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/InternalUserTableHandler.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/InternalUserTableHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/LdapSettingsHandler.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/LdapSettingsHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/admin_backend/__init__.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/admin_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/admin_tuple_providers/LoggedInUserStatusTupleProvider.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/admin_tuple_providers/LoggedInUserStatusTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/api/UserAdminAuthApi.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/api/UserAdminAuthApi.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 )
 from peek_core_user.server.UserAdminAuthApiABC import UserAdminAuthApiABC
 
 logger = logging.getLogger(__name__)
 
 
 class UserAdminAuthApi(UserAdminAuthApiABC):
-    def __init__(self, adminAuthController: AdminAuthController):
+    def __init__(self):
+        self._adminAuthController = None
+
+    def setStartValues(self, adminAuthController: AdminAuthController):
         self._adminAuthController = adminAuthController
 
     def shutdown(self):
-        pass
+        self._adminAuthController = None
 
     def check(self, username: str, password: str) -> Deferred:
         return self._adminAuthController.check(username, password)
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/api/UserApi.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/api/UserApi.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,43 +5,55 @@
 from peek_core_user._private.server.api.UserFieldHookApi import UserFieldHookApi
 from peek_core_user._private.server.api.UserImportApi import UserImportApi
 from peek_core_user._private.server.api.UserInfoApi import UserInfoApi
 from peek_core_user._private.server.api.UserLoginApi import UserLoginApi
 from peek_core_user._private.server.controller.AdminAuthController import (
     AdminAuthController,
 )
-from peek_core_user._private.server.controller.ImportController import ImportController
+from peek_core_user._private.server.controller.ImportController import (
+    ImportController,
+)
 from peek_core_user._private.server.controller.LoginLogoutController import (
     LoginLogoutController,
 )
 from peek_core_user.server.UserApiABC import UserApiABC
 
 logger = logging.getLogger(__name__)
 
 
 class UserApi(UserApiABC):
-    def __init__(
+    def __init__(self):
+        self._hookApi = UserFieldHookApi()
+        self._importApi = UserImportApi()
+        self._infoApi = UserInfoApi()
+        self._loginApi = UserLoginApi()
+        self._adminAuthApi = UserAdminAuthApi()
+
+    def setStartValues(
         self,
-        deviceApi: DeviceApiABC,
         dbSessionCreator,
+        deviceApi: DeviceApiABC,
         importController: ImportController,
         loginLogoutController: LoginLogoutController,
         adminAuthController: AdminAuthController,
     ):
-        self._hookApi = UserFieldHookApi()
 
-        self._importApi = UserImportApi(importController=importController)
+        self._importApi.setStartValues(importController=importController)
 
-        self._infoApi = UserInfoApi(
+        self._infoApi.setStartValues(
             deviceApi=deviceApi, dbSessionCreator=dbSessionCreator
         )
 
-        self._loginApi = UserLoginApi(loginLogoutController=loginLogoutController)
+        self._loginApi.setStartValues(
+            loginLogoutController=loginLogoutController
+        )
 
-        self._adminAuthApi = UserAdminAuthApi(adminAuthController=adminAuthController)
+        self._adminAuthApi.setStartValues(
+            adminAuthController=adminAuthController
+        )
 
     def shutdown(self):
         self._loginApi.shutdown()
         self._importApi.shutdown()
         self._hookApi.shutdown()
         self._infoApi.shutdown()
         self._adminAuthApi.shutdown()
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/api/UserFieldHookApi.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/api/UserFieldHookApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/api/UserImportApi.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/api/UserImportApi.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import logging
 
 from twisted.internet.defer import Deferred
 
-from peek_core_user._private.server.controller.ImportController import ImportController
+from peek_core_user._private.server.controller.ImportController import (
+    ImportController,
+)
 from peek_core_user.server.UserImportApiABC import UserImportApiABC
 
 logger = logging.getLogger(__name__)
 
 
 class UserImportApi(UserImportApiABC):
-    def __init__(self, importController: ImportController):
+    def __init__(self):
+        self._importController = None
+
+    def setStartValues(self, importController: ImportController):
         self._importController = importController
 
     def shutdown(self):
-        pass
+        self._importController = None
 
     def importInternalUsers(
         self, importHash: str, usersEncodedPayload: bytes
     ) -> Deferred:
         return self._importController.importInternalUsers(
             importHash, usersEncodedPayload
         )
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/api/UserInfoApi.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/api/UserInfoApi.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,20 +34,25 @@
         InternalUserTuple.tupleFieldNames()
     )
 
     _groupCopyFields = set(GroupDetailTuple.tupleFieldNames()) & set(
         InternalGroupTuple.tupleFieldNames()
     )
 
-    def __init__(self, deviceApi: DeviceApiABC, dbSessionCreator):
+    def __init__(self):
+        self._deviceApi = None
+        self._dbSessionCreator = None
+
+    def setStartValues(self, deviceApi: DeviceApiABC, dbSessionCreator):
         self._deviceApi = deviceApi
         self._dbSessionCreator = dbSessionCreator
 
     def shutdown(self):
-        pass
+        self._deviceApi = None
+        self._dbSessionCreator = None
 
     @deferToThreadWrapWithLogger(logger)
     def user(self, userName: str):
         """
         :returns a Deferred firing with Optional[UserDetailTuple]]
         """
         return self.userBlocking(userName)
@@ -255,18 +260,23 @@
         except NoResultFound:
             return []
         finally:
             session.close()
 
     @deferToThreadWrapWithLogger(logger)
     def userLoggedInInfo(
-        self, userName: str, isFieldDevice: bool
+        self,
+        userName: Optional[str] = None,
+        isFieldDevice: Optional[bool] = None,
     ) -> List[UserLoggedIn]:
         session = self._dbSessionCreator()
         try:
-            query = session.query(UserLoggedIn).filter(
-                UserLoggedIn.isFieldLogin == isFieldDevice,
-                UserLoggedIn.userName == userName,
-            )
+            query = session.query(UserLoggedIn)
+            if userName:
+                query = query.filter(UserLoggedIn.userName == userName)
+
+            if isFieldDevice:
+                query = query.filter(UserLoggedIn.isFieldLogin == isFieldDevice)
+
             return [row.toTuple() for row in query.all()]
         finally:
             session.close()
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/api/UserLoginApi.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/api/UserLoginApi.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 logger = logging.getLogger(__name__)
 
 
 class UserLoginApi(UserLoginApiABC):
     #: A reference to the core device plugins API
     _deviceApi: DeviceApiABC
 
-    def __init__(self, loginLogoutController: LoginLogoutController):
+    def __init__(self):
+        self._loginLogoutController = None
+
+    def setStartValues(self, loginLogoutController: LoginLogoutController):
         self._loginLogoutController = loginLogoutController
 
     def shutdown(self):
-        pass
+        self._loginLogoutController = None
 
     def logout(self, logoutTuple: UserLogoutAction) -> Deferred:
         return self._loginLogoutController.logout(logoutTuple)
 
     def login(self, loginTuple: UserLoginAction) -> Deferred:
         return self._loginLogoutController.login(loginTuple)
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/auth_connectors/AuthABC.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/auth_connectors/AuthABC.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from abc import ABCMeta
 from abc import abstractmethod
 from typing import List
 from typing import Optional
 from typing import Tuple
 
+from sqlalchemy import func
 from sqlalchemy.orm.exc import NoResultFound
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 
 from peek_core_user._private.storage.InternalUserPassword import (
     InternalUserPassword,
 )
 from peek_core_user._private.storage.InternalUserTuple import InternalUserTuple
@@ -31,15 +32,14 @@
     ) -> Tuple[List[str], InternalUserTuple]:
         raise NotImplementedError()
 
     @deferToThreadWrapWithLogger(logger)
     def getInternalUser(
         self, userName, raiseNotLoggedInException=True
     ) -> Optional[InternalUserTuple]:
-
         session = self._dbSessionCreator()
         try:
             authenticatedUsers = (
                 session.query(InternalUserTuple)
                 .filter(InternalUserTuple.userName == userName)
                 .all()
             )
@@ -61,23 +61,24 @@
 
             # No commit needed, we only query
         finally:
             session.close()
 
     @deferToThreadWrapWithLogger(logger)
     def getInternalUserAndPassword(self, userName):
-
         session = self._dbSessionCreator()
         try:
             authenticatedUserPasswords = (
                 session.query(InternalUserTuple, InternalUserPassword)
                 .join(
                     InternalUserPassword, isouter=True
                 )  # effectively `LEFT JOIN`
-                .filter(InternalUserTuple.userName == userName)
+                .filter(
+                    func.lower(InternalUserTuple.userName) == userName.lower()
+                )
                 .all()
             )
             session.expunge_all()
 
             if len(authenticatedUserPasswords) == 0:
                 raise NoResultFound()
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/auth_connectors/InternalAuth.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/auth_connectors/InternalAuth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 
+from sqlalchemy.orm.exc import NoResultFound
 from twisted.cred.error import LoginFailed
 from twisted.internet.defer import inlineCallbacks
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 
 from peek_core_user._private.server.auth_connectors.AuthABC import AuthABC
 from peek_core_user._private.server.auth_connectors.LdapAuth import LdapAuth
 from peek_core_user._private.server.controller.PasswordUpdateController import (
@@ -30,17 +31,20 @@
 
 logger = logging.getLogger(__name__)
 
 
 class InternalAuth(AuthABC):
     @inlineCallbacks
     def checkPassAsync(self, userName, password, forService):
-        authenticatedUserPassword = yield self.getInternalUserAndPassword(
-            userName
-        )
+        try:
+            authenticatedUserPassword = yield self.getInternalUserAndPassword(
+                userName
+            )
+        except NoResultFound:
+            authenticatedUserPassword = None
 
         # if user not found
         if (
             not authenticatedUserPassword
             or not authenticatedUserPassword.InternalUserTuple
         ):
             raise UserNotFoundException(userName)
@@ -67,18 +71,16 @@
             yield self._checkInternalPass(
                 authenticatedUserPassword, password, forService
             )
         )
 
     @deferToThreadWrapWithLogger(logger)
     def _checkInternalPass(self, authenticatedUser, password, forService):
-
         dbSession = self._dbSessionCreator()
         try:
-
             passObj = authenticatedUser.InternalUserPassword
             if passObj.password != PasswordUpdateController.hashPass(password):
                 raise LoginFailed(
                     "Peek InternalAuth: Username or password is incorrect"
                 )
 
             groups = (
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/auth_connectors/LdapAuth.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/auth_connectors/LdapAuth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import logging
 from collections import namedtuple
 from typing import List
 
 from twisted.cred.error import LoginFailed
 from twisted.internet.defer import inlineCallbacks
 from vortex.DeferUtil import deferToThreadWrapWithLogger
-from vortex.VortexFactory import VortexFactory, NoVortexException
+from vortex.VortexFactory import NoVortexException
+from vortex.VortexFactory import VortexFactory
 
 from peek_core_user._private.PluginNames import userPluginTuplePrefix
 from peek_core_user._private.agent.RpcForLogic import RpcForLogic
 from peek_core_user._private.ldap_auth.ldap_auth import checkLdapAuth
 from peek_core_user._private.server.auth_connectors.AuthABC import AuthABC
 from peek_core_user._private.storage.InternalUserTuple import InternalUserTuple
 from peek_core_user._private.storage.LdapSetting import LdapSetting
 from peek_core_user._private.storage.Setting import LDAP_AUTH_ENABLED
+from peek_core_user._private.storage.Setting import LDAP_ENABLE_DOMAIN_SUPPORT
 from peek_core_user._private.storage.Setting import LDAP_VERIFY_SSL
 from peek_core_user._private.storage.Setting import globalSetting
 from peek_platform.file_config.PeekFileConfigABC import PEEK_AGENT_SERVICE
 
 __author__ = "synerty"
 
 from peek_core_user._private.tuples.LdapLoggedInUserTuple import (
@@ -33,15 +35,15 @@
 
 
 class LdapNotEnabledError(Exception):
     pass
 
 
 _LdapAuthSettings = namedtuple(
-    "_LdapAuthSettings", ["ldapSettings", "ldapVerifySsl"]
+    "_LdapAuthSettings", ["ldapSettings", "ldapVerifySsl", "ldapEnableDomain"]
 )
 
 
 class LdapAuth(AuthABC):
     @inlineCallbacks
     def checkPassAsync(self, userName, password, forService, userUuid=None):
         """Login User
@@ -57,14 +59,19 @@
             AuthABC.FOR_FIELD,
             AuthABC.FOR_OFFICE,
             AuthABC.FOR_ADMIN,
         ), "Unhandled authentication for service type"
 
         authSettings: _LdapAuthSettings = yield self._getSettings()
 
+        if not authSettings.ldapEnableDomain and "@" in userName:
+            raise Exception(
+                "Please login with a username, not an email address"
+            )
+
         if not authSettings.ldapVerifySsl:
             ldap.set_option(ldap.OPT_X_TLS_REQUIRE_CERT, ldap.OPT_X_TLS_NEVER)
 
         if not authSettings.ldapSettings:
             raise Exception("LDAPAuth: No LDAP servers configured.")
 
         firstException = None
@@ -169,15 +176,14 @@
                 .replace("twisted.cred.error.LoginFailed: LDAPAuth: ", "")
             )
 
     @deferToThreadWrapWithLogger(logger)
     def _getOrCreateInternalUserAsync(
         self, ldapLoggedInUser: LdapLoggedInUserTuple
     ) -> List[LdapSetting]:
-
         session = self._dbSessionCreator()
         try:
             internalUser = self._getOrCreateInternalUserBlocking(
                 session, ldapLoggedInUser
             )
             session.expunge_all()
             session.commit()
@@ -187,15 +193,14 @@
         finally:
             session.close()
 
     # noinspection PyMethodMayBeStatic
     def _getOrCreateInternalUserBlocking(
         self, dbSession, ldapLoggedInUser: LdapLoggedInUserTuple
     ) -> InternalUserTuple:
-
         internalUser = (
             dbSession.query(InternalUserTuple)
             .filter(InternalUserTuple.userUuid == ldapLoggedInUser.userUuid)
             .first()
         )
 
         # do no create, return the existing user
@@ -217,24 +222,24 @@
 
         userKey = "%s@%s" % (
             ldapLoggedInUser.username,
             ldapLoggedInUser.ldapDomain,
         )
         logger.info("Creating new internal user: %s", userKey)
         newInternalUser = InternalUserTuple(
-            userName=ldapLoggedInUser.username,
+            userName=ldapLoggedInUser.username.lower(),
             userKey=(
                 ldapLoggedInUser.username
                 if "@" in ldapLoggedInUser.username
                 else userKey
-            ),
+            ).lower(),
             userTitle="%s (%s)"
             % (ldapLoggedInUser.userTitle, ldapLoggedInUser.ldapName),
             userUuid=ldapLoggedInUser.userUuid,
-            email=ldapLoggedInUser.email,
+            email=ldapLoggedInUser.email.lower(),
             authenticationTarget=UserAuthTargetEnum.LDAP,
             importSource="LDAP",
             # importHash e.g. 'peek_core_user.LDAPAuth:<md5 hash>'
             importHash=f"{userPluginTuplePrefix}LDAPAuth:{ldapLoggedInUser.userUuid}",
         )
 
         try:
@@ -245,25 +250,29 @@
                 "Failed to create Internal User. Use the full name <username>@<ldap-domain> to login"
             )
         dbSession.commit()
         return newInternalUser
 
     @deferToThreadWrapWithLogger(logger)
     def _getSettings(self) -> _LdapAuthSettings:
-
         session = self._dbSessionCreator()
         try:
             # Check if the user is actually logged into this device.
             ldapSettings = session.query(LdapSetting).all()
             ldapVerifySsl = globalSetting(session, LDAP_VERIFY_SSL)
+            ldapEnableDomain = globalSetting(
+                session, LDAP_ENABLE_DOMAIN_SUPPORT
+            )
 
             session.expunge_all()
 
             return _LdapAuthSettings(
-                ldapSettings=ldapSettings, ldapVerifySsl=ldapVerifySsl
+                ldapSettings=ldapSettings,
+                ldapVerifySsl=ldapVerifySsl,
+                ldapEnableDomain=ldapEnableDomain,
             )
 
             # No commit needed, we only query
 
         finally:
             session.close()
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/controller/AdminAuthController.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/controller/AdminAuthController.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/controller/ImportController.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/controller/ImportController.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/controller/LoginLogoutController.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/controller/LoginLogoutController.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,15 +332,14 @@
         )
 
         userDetail = self._infoApi.userBlocking(userName)
 
         # check user group and user password
         ormSession = self._dbSessionCreator()
         try:
-
             if not userDetail:
                 responseTuple.setFailed()
                 return responseTuple
 
             userKey = userDetail.userKey
             userUuid = userDetail.userUuid
             loginTuple.userName = userDetail.userName
@@ -375,15 +374,14 @@
             )
 
             sameDevice = userLoggedIn and loggedInElsewhere is None
 
             # If the user is logged in, but not to this client device, raise exception
             if blockMultipleLogins and userLoggedIn and not sameDevice:
                 if USER_ALREADY_LOGGED_ON_KEY in acceptedWarningKeys:
-
                     forceLogouter = _ForceLogout(
                         userUuid, loggedInElsewhere.deviceToken
                     )
 
                     forceLogouter.forceDbLogout(ormSession)
 
                     userLoggedIn = False
@@ -457,16 +455,16 @@
                     )
 
                     return responseTuple
 
             # Create the user logged in entry
 
             newUser = UserLoggedIn(
-                userName=userName,
-                userKey=userKey,
+                userName=userName.lower(),
+                userKey=userKey.lower(),
                 userUuid=userUuid,
                 loggedInDateTime=datetime.now(pytz.utc),
                 deviceToken=deviceToken,
                 vehicle=vehicle,
                 isFieldLogin=isFieldService,
             )
             ormSession.add(newUser)
@@ -503,28 +501,28 @@
         # except DeviceAlreadyLoggedInError as e:
         #     pass
         #
         # except UserIsNotLoggedInToThisDeviceError as e:
         #     pass
 
         except Exception as e:
-
             # Log the user out again if the hooks fail
             logoutTuple = UserLogoutAction(
                 userName=loginTuple.userName, deviceToken=loginTuple.deviceToken
             )
 
             # Force logout, we don't care if it works or not.
             try:
                 yield self._logoutInDb(
                     logoutTuple, raiseNotLoggedInException=False
                 )
             except UserIsNotLoggedInToThisDeviceError:
                 pass
 
+            logger.debug(f"User login failed: {e}")
             raise e
 
         self._clientTupleObservable.notifyOfTupleUpdate(
             TupleSelector(
                 UserLoggedInTuple.tupleType(),
                 selector=dict(deviceToken=loginTuple.deviceToken),
             )
@@ -533,15 +531,14 @@
         self._adminTupleObservable.notifyOfTupleUpdateForTuple(
             LoggedInUserStatusTuple.tupleType()
         )
 
         return loginResponse
 
     def _forceLogout(self, ormSession, userUuid, deviceToken):
-
         ormSession.query(UserLoggedIn).filter(
             UserLoggedIn.userUuid == userUuid
         ).filter(UserLoggedIn.deviceToken == deviceToken).delete(
             synchronize_session=False
         )
 
         self._clientTupleObservable.notifyOfTupleUpdate(
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/controller/MainController.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/controller/PasswordUpdateController.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/controller/PasswordUpdateController.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+import hashlib
 import logging
 
-import hashlib
 from sqlalchemy.orm.exc import NoResultFound
 from twisted.internet.defer import Deferred
+from vortex.DeferUtil import deferToThreadWrapWithLogger
+from vortex.TupleAction import TupleActionABC
+from vortex.handler.TupleActionProcessor import TupleActionProcessorDelegateABC
 
-from peek_core_user._private.storage.InternalUserPassword import InternalUserPassword
-from peek_core_user._private.storage.InternalUserTuple import InternalUserTuple
+from peek_core_user._private.storage.InternalUserPassword import (
+    InternalUserPassword,
+)
 from peek_core_user._private.tuples.InternalUserUpdatePasswordAction import (
     InternalUserUpdatePasswordAction,
 )
-from vortex.DeferUtil import deferToThreadWrapWithLogger
-from vortex.TupleAction import TupleActionABC
-from vortex.handler.TupleActionProcessor import TupleActionProcessorDelegateABC
 
 logger = logging.getLogger(__name__)
 
 
 # This is the CRUD handler
 class PasswordUpdateController(TupleActionProcessorDelegateABC):
     def __init__(self, ormSessionCreator):
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/tuple_providers/GroupDetailTupleProvider.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/tuple_providers/GroupDetailTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/tuple_providers/UserListItemTupleProvider.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/tuple_providers/UserListItemTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/tuple_providers/UserLoggedInTupleProvider.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/tuple_providers/UserLoggedInTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/server/tuple_providers/UserLoginUiSettingTupleProvider.py` & `peek-core-user-3.4.0/peek_core_user/_private/server/tuple_providers/UserLoginUiSettingTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/storage/DeclarativeBase.py` & `peek-core-user-3.4.0/peek_core_user/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/storage/DirectoryTuple.py` & `peek-core-user-3.4.0/peek_core_user/_private/storage/DirectoryTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/storage/InternalGroupTuple.py` & `peek-core-user-3.4.0/peek_core_user/_private/storage/InternalGroupTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/storage/InternalUserGroupTuple.py` & `peek-core-user-3.4.0/peek_core_user/_private/storage/InternalUserGroupTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/storage/InternalUserPassword.py` & `peek-core-user-3.4.0/peek_core_user/_private/storage/InternalUserPassword.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/storage/InternalUserTuple.py` & `peek-core-user-3.4.0/peek_core_user/_private/storage/InternalUserTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/storage/LdapSetting.py` & `peek-core-user-3.4.0/peek_core_user/_private/storage/LdapSetting.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/storage/Setting.py` & `peek-core-user-3.4.0/peek_core_user/_private/storage/Setting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from peek_core_user._private.PluginNames import userPluginTuplePrefix
 from sqlalchemy.ext.associationproxy import association_proxy
 from sqlalchemy.orm import relationship
 from sqlalchemy.orm.collections import attribute_mapped_collection
-from sqlalchemy.schema import Column, ForeignKey
-from sqlalchemy.sql.expression import cast, null, case
+from sqlalchemy.schema import Column
+from sqlalchemy.schema import ForeignKey
+from sqlalchemy.sql.expression import case
+from sqlalchemy.sql.expression import cast
+from sqlalchemy.sql.expression import null
 from sqlalchemy.sql.schema import Index
-from sqlalchemy.types import Integer, String, Boolean
-from vortex.Tuple import Tuple, addTupleType
+from sqlalchemy.types import Boolean
+from sqlalchemy.types import Integer
+from sqlalchemy.types import String
+from vortex.Tuple import Tuple
+from vortex.Tuple import addTupleType
 
+from peek_core_user._private.PluginNames import userPluginTuplePrefix
 from .DeclarativeBase import DeclarativeBase
 
 """Mapping a polymorphic-valued vertical table as a dictionary.
 
 For any given properties row, the value of the 'type' column will point to the
 '_value' column active for that row.
 
@@ -228,15 +234,18 @@
     if needsCommit:
         ormSession.commit()
 
     if not key:
         return setting
 
     # Make sure the propery is defined for this setting
-    assert str(key) in propertyDict, "Key %s is not defined in setting %s" % (key, name)
+    assert str(key) in propertyDict, "Key %s is not defined in setting %s" % (
+        key,
+        name,
+    )
 
     if value is None:
         return setting[key]
 
     setting[key] = value
     ormSession.commit()
 
@@ -248,15 +257,17 @@
 # GLOBAL PROPERTIES
 # =============================================================================
 
 globalProperties = {}
 
 
 def globalSetting(ormSession, key=None, value=None):
-    return _getSetting(ormSession, "Global", globalProperties, key=key, value=value)
+    return _getSetting(
+        ormSession, "Global", globalProperties, key=key, value=value
+    )
 
 
 MOBILE_LOGIN_GROUP = PropertyKey(
     "Mobile Login Group", "peek-field-app-login", propertyDict=globalProperties
 )
 
 ADMIN_LOGIN_GROUP = PropertyKey(
@@ -290,7 +301,11 @@
 LDAP_AUTH_ENABLED = PropertyKey(
     "LDAP Auth Enabled", False, propertyDict=globalProperties
 )
 
 LDAP_VERIFY_SSL = PropertyKey(
     "LDAP Verify SSL Certificates", True, propertyDict=globalProperties
 )
+
+LDAP_ENABLE_DOMAIN_SUPPORT = PropertyKey(
+    "LDAP Enable @domain Support for Login", True, propertyDict=globalProperties
+)
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/storage/UserLoggedIn.py` & `peek-core-user-3.4.0/peek_core_user/_private/storage/UserLoggedIn.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/tuples/InternalGroupImportResultTuple.py` & `peek-core-user-3.4.0/peek_core_user/_private/tuples/InternalGroupImportResultTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/tuples/InternalUserImportResultTuple.py` & `peek-core-user-3.4.0/peek_core_user/_private/tuples/InternalUserImportResultTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/tuples/LdapLoggedInUserTuple.py` & `peek-core-user-3.4.0/peek_core_user/_private/tuples/LdapLoggedInUserTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/tuples/LoggedInUserStatusTuple.py` & `peek-core-user-3.4.0/peek_core_user/_private/tuples/LoggedInUserStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/tuples/UserLoggedInTuple.py` & `peek-core-user-3.4.0/peek_core_user/_private/tuples/UserLoggedInTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/worker/WorkerEntryHook.py` & `peek-core-user-3.4.0/peek_core_user/_private/worker/WorkerEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/worker/tasks/UserImportInternalGroupTask.py` & `peek-core-user-3.4.0/peek_core_user/_private/worker/tasks/UserImportInternalGroupTask.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from datetime import datetime
 from typing import List
 
 import pytz
 from txcelery.defer import DeferrableTask
 
 from peek_plugin_base.worker import CeleryDbConn
-from peek_core_user._private.storage.InternalGroupTuple import InternalGroupTuple
+from peek_core_user._private.storage.InternalGroupTuple import (
+    InternalGroupTuple,
+)
 from peek_core_user._private.tuples.InternalGroupImportResultTuple import (
     InternalGroupImportResultTuple,
 )
 from peek_plugin_base.worker.CeleryApp import celeryApp
 from peek_core_user.tuples.import_.ImportInternalGroupTuple import (
     ImportInternalGroupTuple,
 )
@@ -72,15 +74,17 @@
                 else:
                     sameCount += 1
 
             else:
                 newGroup = InternalGroupTuple()
 
                 for fieldName in ImportInternalGroupTuple.tupleFieldNames():
-                    setattr(newGroup, fieldName, getattr(importGroup, fieldName))
+                    setattr(
+                        newGroup, fieldName, getattr(importGroup, fieldName)
+                    )
 
                 session.add(newGroup)
                 inserts.append(newGroup)
 
         for oldGroup in existingGroupsByName.values():
             deleteIds.append(oldGroup.id)
             session.delete(oldGroup)
```

### Comparing `peek-core-user-3.3.3/peek_core_user/_private/worker/tasks/UserImportInternalUserTask.py` & `peek-core-user-3.4.0/peek_core_user/_private/worker/tasks/UserImportInternalUserTask.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,24 +67,32 @@
                 for g in session.query(InternalUserTuple)
                 .filter(InternalUserTuple.userUuid.in_(allUuids))
                 .filter(InternalUserTuple.importHash == importHash)
                 .options(subqueryload(InternalUserTuple.groups))
                 .all()
             }
 
-        groupsByName = {g.groupName: g for g in session.query(InternalGroupTuple).all()}
+        groupsByName = {
+            g.groupName: g for g in session.query(InternalGroupTuple).all()
+        }
 
         for importUser in importUsers:
             try:
-                existingUser = existingUsersByUuid.pop(importUser.userUuid, None)
+                existingUser = existingUsersByUuid.pop(
+                    importUser.userUuid, None
+                )
                 if existingUser:
-                    _updateUser(existingUser, groupsByName, importUser, same, updates)
+                    _updateUser(
+                        existingUser, groupsByName, importUser, same, updates
+                    )
 
                 else:
-                    _insertUser(session, groupsByName, importUser, importHash, inserts)
+                    _insertUser(
+                        session, groupsByName, importUser, importHash, inserts
+                    )
 
                 session.commit()
 
             except IntegrityError as e:
                 errors.append(str(e))
                 session.rollback()
 
@@ -134,14 +142,17 @@
 
     if importUser.groupKeys is not None:
         for groupKey in importUser.groupKeys:
             newUser.groups.append(groupsByName[groupKey])
 
     newUser.password = PasswordUpdateController.hashPass(str(uuid.uuid4()))
 
+    newUser.userKey = newUser.userKey.lower()
+    newUser.userName = newUser.userName.lower()
+
     session.add(newUser)
     inserts.append(newUser)
 
 
 def _updateUser(existingUser, groupsByName, importUser, same, updates):
     excludeFieldNames = ("groupKeys", "password", "userUuid")
 
@@ -152,26 +163,28 @@
 
     updated = False
     for fieldName in copyFields:
         newVal = getattr(importUser, fieldName)
         existingVal = getattr(existingUser, fieldName)
         if existingVal != newVal:
             if existingVal and not newVal:
-                """ Don't wipe out values if they already exist """
+                """Don't wipe out values if they already exist"""
 
             else:
                 setattr(existingUser, fieldName, newVal)
                 # update userKey as well when 'userName' changes
                 if fieldName == "userName":
                     setattr(existingUser, "userKey", newVal.lower())
                 updated = True
 
     # The password is an optional field
     if importUser.password is not None:
-        existingUser.password = PasswordUpdateController.hashPass(importUser.password)
+        existingUser.password = PasswordUpdateController.hashPass(
+            importUser.password
+        )
         updated = True
 
     # If there are NONE groups, then don't make any changes
     if importUser.groupKeys is not None:
         linkedGroupNames = set([g.groupName for g in existingUser.groups])
         addGroups = set(importUser.groupKeys) - linkedGroupNames
         removeGroups = linkedGroupNames - set(importUser.groupKeys)
```

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/add_group.png` & `peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/add_group.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/add_user.png` & `peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/add_user.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/configuration.rst` & `peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/configuration.rst`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/edit-internal-groups.png` & `peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/edit-internal-groups.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/edit-internal-user.png` & `peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/edit-internal-user.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/settings-general.png` & `peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/settings-general.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/configuration/settings-ldap.png` & `peek-core-user-3.4.0/peek_core_user/admin-doc/configuration/settings-ldap.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/logged_in/logged_in.rst` & `peek-core-user-3.4.0/peek_core_user/admin-doc/logged_in/logged_in.rst`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/logged_in/logout_user.png` & `peek-core-user-3.4.0/peek_core_user/admin-doc/logged_in/logout_user.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/logged_in/logout_yes.png` & `peek-core-user-3.4.0/peek_core_user/admin-doc/logged_in/logout_yes.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/logged_in/manage-logged-in-users.png` & `peek-core-user-3.4.0/peek_core_user/admin-doc/logged_in/manage-logged-in-users.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/admin-doc/overview.rst` & `peek-core-user-3.4.0/peek_core_user/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/both-doc/login.png` & `peek-core-user-3.4.0/peek_core_user/both-doc/login.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/both-doc/login_logout.png` & `peek-core-user-3.4.0/peek_core_user/both-doc/login_logout.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/both-doc/login_logout.rst` & `peek-core-user-3.4.0/peek_core_user/both-doc/login_logout.rst`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/both-doc/user_button.png` & `peek-core-user-3.4.0/peek_core_user/both-doc/user_button.png`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/_private/tuples/LoggedInUserStatusTuple.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/_private/tuples/LoggedInUserStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/_private/tuples/UserLoggedInTuple.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/_private/tuples/UserLoggedInTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/_private/user-tuple.service.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/_private/user-tuple.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/index.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/index.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/services/logged-in.guard.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/services/logged-in.guard.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/services/user.service.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/services/user.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/UserDetailTuple.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/UserDetailTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/UserListItemTuple.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/UserListItemTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/login/UserLoginAction.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/login/UserLoginAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/login/UserLoginResponseTuple.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/login/UserLoginResponseTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/login/UserLogoutAction.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/login/UserLogoutAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin-module/tuples/login/UserLogoutResponseTuple.ts` & `peek-core-user-3.4.0/peek_core_user/plugin-module/tuples/login/UserLogoutResponseTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/plugin_package.json` & `peek-core-user-3.4.0/peek_core_user/plugin_package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967532467532468%*

 * *Differences: {"'plugin'": "{'version': '3.4.0'}"}*

```diff
@@ -74,15 +74,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_core_user",
         "title": "Users",
-        "version": "3.3.3",
+        "version": "3.4.0",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "storage",
         "field",
         "office",
```

### Comparing `peek-core-user-3.3.3/peek_core_user/server/UserApiABC.py` & `peek-core-user-3.4.0/peek_core_user/server/UserApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/server/UserDbErrors.py` & `peek-core-user-3.4.0/peek_core_user/server/UserDbErrors.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/server/UserFieldHookApiABC.py` & `peek-core-user-3.4.0/peek_core_user/server/UserFieldHookApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/server/UserImportApiABC.py` & `peek-core-user-3.4.0/peek_core_user/server/UserImportApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/server/UserInfoApiABC.py` & `peek-core-user-3.4.0/peek_core_user/server/UserInfoApiABC.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,13 +106,18 @@
         # str]
         """Peek field device tokens with logged-in status
 
         :return: A list of string of device tokens
         """
 
     @abstractmethod
-    def userLoggedInInfo(self, userName: str, isFieldDevice: bool) -> Deferred:
+    def userLoggedInInfo(
+        self,
+        userName: Optional[str] = None,
+        isFieldDevice: Optional[bool] = None,
+    ) -> Deferred:
         """Peek logged-in field device info by userName
 
         :param userName: The username / userid of the user, EG C917
+        :param isFieldDevice:
         :return: A list of user LoggedIn Info
         """
```

### Comparing `peek-core-user-3.3.3/peek_core_user/server/UserLoginApiABC.py` & `peek-core-user-3.4.0/peek_core_user/server/UserLoginApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/tuples/DeviceWithUserDetails.py` & `peek-core-user-3.4.0/peek_core_user/tuples/DeviceWithUserDetails.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/tuples/UserDetailTuple.py` & `peek-core-user-3.4.0/peek_core_user/tuples/UserDetailTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/tuples/UserListItemTuple.py` & `peek-core-user-3.4.0/peek_core_user/tuples/UserListItemTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/tuples/UserLoggedInInfoTuple.py` & `peek-core-user-3.4.0/peek_core_user/tuples/UserLoggedInInfoTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/tuples/import_/ImportInternalUserTuple.py` & `peek-core-user-3.4.0/peek_core_user/tuples/import_/ImportInternalUserTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/tuples/login/UserLoginAction.py` & `peek-core-user-3.4.0/peek_core_user/tuples/login/UserLoginAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/tuples/login/UserLoginResponseTuple.py` & `peek-core-user-3.4.0/peek_core_user/tuples/login/UserLoginResponseTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/tuples/login/UserLogoutAction.py` & `peek-core-user-3.4.0/peek_core_user/tuples/login/UserLogoutAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user/tuples/login/UserLogoutResponseTuple.py` & `peek-core-user-3.4.0/peek_core_user/tuples/login/UserLogoutResponseTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-user-3.3.3/peek_core_user.egg-info/SOURCES.txt` & `peek-core-user-3.4.0/peek_core_user.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 peek_core_user/_private/alembic/versions/56d805072d2a_added_importhash.py
 peek_core_user/_private/alembic/versions/5e33c6b788fd_removed_unique_logged_in_user.py
 peek_core_user/_private/alembic/versions/73d65f042834_removed_foreign_key_from_user_logged_in.py
 peek_core_user/_private/alembic/versions/7e3f668edf0e_updated_settings.py
 peek_core_user/_private/alembic/versions/9b65be31926e_timezone_aware.py
 peek_core_user/_private/alembic/versions/__init__.py
 peek_core_user/_private/alembic/versions/b09fe7b3b31b_add_userkey.py
+peek_core_user/_private/alembic/versions/d03db0fcb600_convert_userkey_and_username_to_all_.py
 peek_core_user/_private/alembic/versions/d79da9333e2a_drop_internaluser_rows_from_ldap_for_useruuid_change.py
 peek_core_user/_private/alembic/versions/eef485ef2e0e_added_agenturi_column_to_ldapsetting.py
 peek_core_user/_private/both-app/__init__.py
 peek_core_user/_private/both-app/plugin-user.module.ts
 peek_core_user/_private/both-app/plugin-user.routes.ts
 peek_core_user/_private/both-app/plugin-user.text.ts
 peek_core_user/_private/both-app/scss/plugin-user.dweb.scss
```

### Comparing `peek-core-user-3.3.3/setup.py` & `peek-core-user-3.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_core_user"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.3.3"
+package_version = "3.4.0"
 description = "Peek Plugin ENAMC Email Incidents."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

