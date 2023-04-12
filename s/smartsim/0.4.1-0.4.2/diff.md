# Comparing `tmp/smartsim-0.4.1.tar.gz` & `tmp/smartsim-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartsim-0.4.1.tar", last modified: Sat Jun 25 00:32:45 2022, max compression
+gzip compressed data, was "smartsim-0.4.2.tar", last modified: Wed Apr 12 20:48:46 2023, max compression
```

## Comparing `smartsim-0.4.1.tar` & `smartsim-0.4.2.tar`

### file list

```diff
@@ -1,161 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1341 2022-06-25 00:32:42.000000 smartsim-0.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-06-25 00:32:42.000000 smartsim-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4164 2022-06-25 00:32:42.000000 smartsim-0.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    36144 2022-06-25 00:32:45.418562 smartsim-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    28775 2022-06-25 00:32:42.000000 smartsim-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      677 2022-06-25 00:32:42.000000 smartsim-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-25 00:32:42.000000 smartsim-0.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-06-25 00:32:45.418562 smartsim-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-06-25 00:32:42.000000 smartsim-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.406562 smartsim-0.4.1/smartsim/
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.410562 smartsim-0.4.1/smartsim/_core/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.410562 smartsim-0.4.1/smartsim/_core/_cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15393 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/_cli/clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1768 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.410562 smartsim-0.4.1/smartsim/_core/_install/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/_install/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.410562 smartsim-0.4.1/smartsim/_core/_install/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)    14637 2022-06-25 00:32:45.000000 smartsim-0.4.1/smartsim/_core/_install/__pycache__/buildenv.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (121)    11795 2022-06-25 00:32:45.000000 smartsim-0.4.1/smartsim/_core/_install/__pycache__/builder.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (121)    16264 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/_install/buildenv.py
--rw-r--r--   0 runner    (1001) docker     (121)    16462 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/_install/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.406562 smartsim-0.4.1/smartsim/_core/bin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.410562 smartsim-0.4.1/smartsim/_core/bin/modules/
--rw-r--r--   0 runner    (1001) docker     (121)    16407 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/bin/modules/FindTensorFlow.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.410562 smartsim-0.4.1/smartsim/_core/config/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6047 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/config/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    71337 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/config/keydb.conf
--rw-r--r--   0 runner    (1001) docker     (121)    85544 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/config/redis6.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.410562 smartsim-0.4.1/smartsim/_core/control/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24686 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/control/controller.py
--rw-r--r--   0 runner    (1001) docker     (121)     6323 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/control/job.py
--rw-r--r--   0 runner    (1001) docker     (121)    13273 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/control/jobmanager.py
--rw-r--r--   0 runner    (1001) docker     (121)     8985 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/control/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.410562 smartsim-0.4.1/smartsim/_core/entrypoints/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/entrypoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10775 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/entrypoints/colocated.py
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/entrypoints/ray.py
--rw-r--r--   0 runner    (1001) docker     (121)     3778 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/entrypoints/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.410562 smartsim-0.4.1/smartsim/_core/generation/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10008 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/generation/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6271 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/generation/modelwriter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.414562 smartsim-0.4.1/smartsim/_core/launcher/
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.414562 smartsim-0.4.1/smartsim/_core/launcher/cobalt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/cobalt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/cobalt/cobaltCommands.py
--rw-r--r--   0 runner    (1001) docker     (121)     6518 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/cobalt/cobaltLauncher.py
--rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/cobalt/cobaltParser.py
--rw-r--r--   0 runner    (1001) docker     (121)     7709 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/colocated.py
--rw-r--r--   0 runner    (1001) docker     (121)     6200 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.414562 smartsim-0.4.1/smartsim/_core/launcher/local/
--rw-r--r--   0 runner    (1001) docker     (121)     4691 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/local/local.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.414562 smartsim-0.4.1/smartsim/_core/launcher/lsf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/lsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/lsf/lsfCommands.py
--rw-r--r--   0 runner    (1001) docker     (121)     7098 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/lsf/lsfLauncher.py
--rw-r--r--   0 runner    (1001) docker     (121)     5226 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/lsf/lsfParser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.414562 smartsim-0.4.1/smartsim/_core/launcher/pbs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/pbs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2272 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/pbs/pbsCommands.py
--rw-r--r--   0 runner    (1001) docker     (121)     6323 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/pbs/pbsLauncher.py
--rw-r--r--   0 runner    (1001) docker     (121)     4638 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/pbs/pbsParser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.414562 smartsim-0.4.1/smartsim/_core/launcher/slurm/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3675 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/slurm/slurmCommands.py
--rw-r--r--   0 runner    (1001) docker     (121)     9471 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/slurm/slurmLauncher.py
--rw-r--r--   0 runner    (1001) docker     (121)     4983 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/slurm/slurmParser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.414562 smartsim-0.4.1/smartsim/_core/launcher/step/
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4865 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/step/alpsStep.py
--rw-r--r--   0 runner    (1001) docker     (121)     3840 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/step/cobaltStep.py
--rw-r--r--   0 runner    (1001) docker     (121)     2744 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/step/localStep.py
--rw-r--r--   0 runner    (1001) docker     (121)    10570 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/step/lsfStep.py
--rw-r--r--   0 runner    (1001) docker     (121)     5321 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/step/mpirunStep.py
--rw-r--r--   0 runner    (1001) docker     (121)     3580 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/step/pbsStep.py
--rw-r--r--   0 runner    (1001) docker     (121)     7389 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/step/slurmStep.py
--rw-r--r--   0 runner    (1001) docker     (121)     3849 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/step/step.py
--rw-r--r--   0 runner    (1001) docker     (121)    10049 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/stepInfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2776 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/stepMapping.py
--rw-r--r--   0 runner    (1001) docker     (121)    12350 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/taskManager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.414562 smartsim-0.4.1/smartsim/_core/launcher/util/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/util/launcherUtil.py
--rw-r--r--   0 runner    (1001) docker     (121)     3455 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/launcher/util/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.414562 smartsim-0.4.1/smartsim/_core/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7173 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3231 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (121)     7488 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/_core/utils/redis.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/smartsim/database/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40324 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/database/orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/smartsim/entity/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8687 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/entity/dbnode.py
--rw-r--r--   0 runner    (1001) docker     (121)     7857 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/entity/dbobject.py
--rw-r--r--   0 runner    (1001) docker     (121)    18310 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/entity/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/entity/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/entity/entityList.py
--rw-r--r--   0 runner    (1001) docker     (121)    11191 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/entity/files.py
--rw-r--r--   0 runner    (1001) docker     (121)    16894 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/entity/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/entity/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/smartsim/error/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3952 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/error/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.406562 smartsim-0.4.1/smartsim/exp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/smartsim/exp/ray/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/exp/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15565 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/exp/ray/raycluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    30472 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)     4461 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/smartsim/ml/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28191 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/ml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/smartsim/ml/tf/
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/ml/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2395 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/ml/tf/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2927 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/ml/tf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/smartsim/ml/torch/
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/ml/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/ml/torch/data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/smartsim/settings/
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8250 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/settings/alpsSettings.py
--rw-r--r--   0 runner    (1001) docker     (121)    20491 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5933 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/settings/cobaltSettings.py
--rw-r--r--   0 runner    (1001) docker     (121)     5313 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/settings/containers.py
--rw-r--r--   0 runner    (1001) docker     (121)    19566 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/settings/lsfSettings.py
--rw-r--r--   0 runner    (1001) docker     (121)    12471 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/settings/mpirunSettings.py
--rw-r--r--   0 runner    (1001) docker     (121)     7860 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/settings/pbsSettings.py
--rw-r--r--   0 runner    (1001) docker     (121)     6432 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    14686 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/settings/slurmSettings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/slurm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/smartsim/tf/
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/tf/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-25 00:32:45.000000 smartsim-0.4.1/smartsim/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.418562 smartsim-0.4.1/smartsim/wlm/
--rw-r--r--   0 runner    (1001) docker     (121)     4074 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/wlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3379 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/wlm/pbs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11235 2022-06-25 00:32:42.000000 smartsim-0.4.1/smartsim/wlm/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 00:32:45.406562 smartsim-0.4.1/smartsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    36144 2022-06-25 00:32:45.000000 smartsim-0.4.1/smartsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4127 2022-06-25 00:32:45.000000 smartsim-0.4.1/smartsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 00:32:45.000000 smartsim-0.4.1/smartsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-06-25 00:32:45.000000 smartsim-0.4.1/smartsim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 00:32:45.000000 smartsim-0.4.1/smartsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-06-25 00:32:45.000000 smartsim-0.4.1/smartsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-25 00:32:45.000000 smartsim-0.4.1/smartsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.143744 smartsim-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-12 20:48:40.000000 smartsim-0.4.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 20:48:40.000000 smartsim-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-12 20:48:40.000000 smartsim-0.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    33917 2023-04-12 20:48:46.147744 smartsim-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26929 2023-04-12 20:48:40.000000 smartsim-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-12 20:48:40.000000 smartsim-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-12 20:48:40.000000 smartsim-0.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 20:48:46.147744 smartsim-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-12 20:48:40.000000 smartsim-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.115744 smartsim-0.4.2/smartsim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim/_core/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16968 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim/_core/_install/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_install/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim/_core/_install/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)    16196 2023-04-12 20:48:45.000000 smartsim-0.4.2/smartsim/_core/_install/__pycache__/buildenv.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    12101 2023-04-12 20:48:45.000000 smartsim-0.4.2/smartsim/_core/_install/__pycache__/builder.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_install/buildenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18635 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/_install/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.111744 smartsim-0.4.2/smartsim/_core/bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim/_core/bin/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/bin/modules/FindTensorFlow.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.123744 smartsim-0.4.2/smartsim/_core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71337 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/config/keydb.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    85544 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/config/redis6.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.123744 smartsim-0.4.2/smartsim/_core/control/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25793 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/control/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/control/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/control/jobmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/control/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.123744 smartsim-0.4.2/smartsim/_core/entrypoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/entrypoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/entrypoints/colocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/entrypoints/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.123744 smartsim-0.4.2/smartsim/_core/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/generation/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/generation/modelwriter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.123744 smartsim-0.4.2/smartsim/_core/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.127744 smartsim-0.4.2/smartsim/_core/launcher/cobalt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/cobalt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8232 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/colocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.127744 smartsim-0.4.2/smartsim/_core/launcher/local/
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.127744 smartsim-0.4.2/smartsim/_core/launcher/lsf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/lsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7283 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfParser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.127744 smartsim-0.4.2/smartsim/_core/launcher/pbs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/pbs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6550 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsParser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.127744 smartsim-0.4.2/smartsim/_core/launcher/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmParser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.131744 smartsim-0.4.2/smartsim/_core/launcher/step/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/alpsStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/cobaltStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/localStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/lsfStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/mpiStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/pbsStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/slurmStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/step/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/stepInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/stepMapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/taskManager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.131744 smartsim-0.4.2/smartsim/_core/launcher/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/util/launcherUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/launcher/util/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.135744 smartsim-0.4.2/smartsim/_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/_core/utils/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.135744 smartsim-0.4.2/smartsim/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40661 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/database/orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.139744 smartsim-0.4.2/smartsim/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/dbnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/dbobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/entityList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11191 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20119 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/entity/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.139744 smartsim-0.4.2/smartsim/error/
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/error/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.139744 smartsim-0.4.2/smartsim/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18232 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.139744 smartsim-0.4.2/smartsim/ml/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/tf/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/tf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.139744 smartsim-0.4.2/smartsim/ml/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/ml/torch/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.143744 smartsim-0.4.2/smartsim/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/alpsSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20491 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/cobaltSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19558 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/lsfSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/mpiSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/mpirunSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/palsSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/pbsSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/settings/slurmSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.143744 smartsim-0.4.2/smartsim/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/tf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-12 20:48:45.000000 smartsim-0.4.2/smartsim/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.143744 smartsim-0.4.2/smartsim/wlm/
+-rw-r--r--   0 runner    (1001) docker     (123)     5461 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/wlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/wlm/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-04-12 20:48:40.000000 smartsim-0.4.2/smartsim/wlm/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:48:46.119744 smartsim-0.4.2/smartsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    33917 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 20:48:46.000000 smartsim-0.4.2/smartsim.egg-info/top_level.txt
```

### Comparing `smartsim-0.4.1/LICENSE.md` & `smartsim-0.4.2/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2021-2022, Hewlett Packard Enterprise
+Copyright (c) 2021-2023, Hewlett Packard Enterprise
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/PKG-INFO` & `smartsim-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsim
-Version: 0.4.1
+Version: 0.4.2
 Summary: AI Workflows for Science
 Home-page: https://github.com/CrayLabs/SmartSim
 Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
 Author-email: craylabs@hpe.com
 License: BSD 2-Clause License
 Project-URL: Source, https://github.com/CrayLabs/SmartSim
 Project-URL: Documentation, https://www.craylabs.org
@@ -22,25 +22,29 @@
             <a href="https://github.com/CrayLabs"><b>Cray Labs</b></a>&nbsp;&nbsp;&nbsp;
           </div>
             <br />
             <br />
         </div>
         
         
+        <div align="center">
+        
         [![License](https://img.shields.io/github/license/CrayLabs/SmartSim)](https://github.com/CrayLabs/SmartSim/blob/master/LICENSE.md)
         ![GitHub last commit](https://img.shields.io/github/last-commit/CrayLabs/SmartSim)
         ![GitHub deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/github-pages?label=doc%20build)
         ![PyPI - Wheel](https://img.shields.io/pypi/wheel/smartsim)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/smartsim)
         ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/CrayLabs/SmartSim)
         ![Language](https://img.shields.io/github/languages/top/CrayLabs/SmartSim)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![codecov](https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim)
         [![Downloads](https://static.pepy.tech/personalized-badge/smartsim?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/smartsim)
         
+        </div>
+        
         ------------
         
         # SmartSim
         
         SmartSim is made up of two parts
           1. SmartSim Infrastructure Library (This repository)
           2. [SmartRedis](https://github.com/CrayLabs/SmartRedis)
@@ -75,16 +79,14 @@
             - [Interactive Launch Example](#interactive-launch-example)
             - [Batch Launch Examples](#batch-launch-examples)
         - [Infrastructure Library Applications](#infrastructure-library-applications)
           - [Redis + RedisAI](#redis--redisai)
             - [Local Launch](#local-launch)
             - [Interactive Launch](#interactive-launch)
             - [Batch Launch](#batch-launch)
-          - [Ray](#ray)
-            - [Ray on HPC](#ray-on-hpc)
         - [SmartRedis](#smartredis)
           - [Tensors](#tensors)
           - [Datasets](#datasets)
         - [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-tutorials)
           - [Run the Tutorials](#run-the-tutorials)
           - [Online Analysis](#online-analysis)
               - [Lattice Boltzmann Simulation](#lattice-boltzmann-simulation)
@@ -103,16 +105,16 @@
         
         The documentation has a number of tutorials that make it easy to get used to SmartSim locally
         before using it on your system. Each tutorial is a Jupyter notebook that can be run through the
         [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
         which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
         
         ```bash
-        docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.1
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
+        docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.2
+        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
         # click on link to open jupyter lab
         ```
         
         # SmartSim Infrastructure Library
         
         The Infrastructure Library (IL), the ``smartsim`` python package,
         facilitates the launch of Machine Learning and simulation
@@ -290,15 +292,14 @@
         initialization. Local launching does not support batch workloads.
         
         
         --------
         
         # Infrastructure Library Applications
          - Orchestrator - In-memory data store and Machine Learning Inference (Redis + RedisAI)
-         - Ray - Distributed Reinforcement Learning (RL), Hyperparameter Optimization (HPO)
         
         ## Redis + RedisAI
         
         The ``Orchestrator`` is an in-memory database that utilizes Redis and RedisAI to provide
         a distributed database and access to ML runtimes from Fortran, C, C++ and Python.
         
         SmartSim provides classes that make it simple to launch the database in many
@@ -404,61 +405,14 @@
         exp.stop(db_cluster)
         ```
         
         ```bash
         python run_db_batch.py
         ```
         
-        -----
-        ## Ray
-        
-        Ray is a distributed computation framework that supports a number of applications
-         - RLlib - Distributed Reinforcement Learning (RL)
-         - RaySGD - Distributed Training
-         - Ray Tune - Hyperparameter Optimization (HPO)
-         - Ray Serve - ML/DL inference
-        As well as other integrations with frameworks like Modin, Mars, Dask, and Spark.
-        
-        Historically, Ray has not been well supported on HPC systems. A few examples exist,
-        but none are well maintained. Because SmartSim already has launchers for HPC systems,
-        launching Ray through SmartSim is a relatively simple task.
-        
-        ### Ray on HPC
-        
-        Below is an example of how to launch a Ray cluster on an HPC system and connect to it.
-        In this example, we set `batch=True`, which means that the cluster will be started
-        requesting an allocation through the scheduler (Slurm, PBS, etc). If this code
-        is run within a sufficiently large interactive allocation, setting `batch=False`
-        will spin the Ray cluster on the allocated nodes.
-        
-        ```Python
-        import ray
-        
-        from smartsim import Experiment
-        from smartsim.exp.ray import RayCluster
-        
-        exp = Experiment("ray-cluster", launcher='auto')
-        # 3 workers + 1 head node = 4 node-cluster
-        cluster = RayCluster(name="ray-cluster", run_args={},
-                             ray_args={"num-cpus": 24},
-                             launcher='auto', num_nodes=4, batch=True)
-        
-        exp.generate(cluster, overwrite=True)
-        exp.start(cluster, block=False, summary=True)
-        
-        # Connect to the Ray cluster
-        ctx = ray.init(f"ray://{cluster.get_head_address()}:10001")
-        
-        # <run Ray tune, RLlib, HPO...>
-        ```
-        
-        *New in 0.4.0* the auto argument enables the Ray Cluster to be launched
-        across scheduler types. Both batch launch and interactive launch commands
-        will be automatically detected and used by SmartSim.
-        
         ------
         # SmartRedis
         
         The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/SmartRedis))
         are implementations of Redis clients that implement the RedisAI
         API with additions specific to scientific workflows.
         
@@ -504,15 +458,15 @@
         
         Each tutorial is a Jupyter notebook that can be run through the
         [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
         which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
         
         ```bash
         docker pull ghcr.io/craylabs/smartsim-tutorials:v1
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
+        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
         ```
         Each of the following examples can be found in the
         [SmartSim documentation](https://www.craylabs.org/docs/tutorials/getting_started/getting_started.html).
         
         ## Online Analysis
         
         Using SmartSim, HPC applications can be monitored in real time by streaming data
@@ -689,25 +643,25 @@
               <th style="text-align:center">RedisAI Version</th>
               <th style="text-align:center">Libraries</th>
               <th style="text-align:center">Supported Version</th>
             </tr>
           </thead>
           <tbody style="text-align:center">
             <tr>
-              <td rowspan="3">1.2.3-1.2.4</td>
+              <td rowspan="3">1.2.7</td>
               <td>PyTorch</td>
-              <td>1.7.x</td>
+              <td>1.11.x</td>
             </tr>
             <tr>
               <td>TensorFlow\Keras</td>
-              <td>2.4.x-2.5.x</td>
+              <td>2.8.x</td>
             </tr>
             <tr>
               <td>ONNX</td>
-              <td>1.9.x</td>
+              <td>1.11.x</td>
             </tr>
               <td rowspan="3">1.2.5</td>
               <td>PyTorch</td>
               <td>1.9.x</td>
             </tr>
             <tr>
               <td>TensorFlow\Keras</td>
@@ -820,18 +774,17 @@
             author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E. Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins},
             keywords = {Deep learning, Numerical simulation, Climate modeling, High performance computing, SmartSim},
         }
         ```
         
 Keywords: scientific,ai,workflow,hpc,analysis
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ml
-Provides-Extra: ray
```

#### html2text {}

```diff
@@ -1,83 +1,83 @@
-Metadata-Version: 2.1 Name: smartsim Version: 0.4.1 Summary: AI Workflows for
+Metadata-Version: 2.1 Name: smartsim Version: 0.4.2 Summary: AI Workflows for
 Science Home-page: https://github.com/CrayLabs/SmartSim Author: CrayLabs, a
 Hewlett Packard Enterprise OSS Organization Author-email: craylabs@hpe.com
 License: BSD 2-Clause License Project-URL: Source, https://github.com/CrayLabs/
 SmartSim Project-URL: Documentation, https://www.craylabs.org Description:
     [https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/
                           SmartSim_Large.png][Image]
 
        Home    Install    Documentation    Slack_Invite    Cray_Labs   
 
 
 [![License](https://img.shields.io/github/license/CrayLabs/SmartSim)](https://
-github.com/CrayLabs/SmartSim/blob/master/LICENSE.md) ![GitHub last commit]
-(https://img.shields.io/github/last-commit/CrayLabs/SmartSim) ![GitHub
-deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/
-github-pages?label=doc%20build) ![PyPI - Wheel](https://img.shields.io/pypi/
-wheel/smartsim) ![PyPI - Python Version](https://img.shields.io/pypi/
-pyversions/smartsim) ![GitHub tag (latest by date)](https://img.shields.io/
-github/v/tag/CrayLabs/SmartSim) ![Language](https://img.shields.io/github/
+  github.com/CrayLabs/SmartSim/blob/master/LICENSE.md) ![GitHub last commit]
+    (https://img.shields.io/github/last-commit/CrayLabs/SmartSim) ![GitHub
+   deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/
+ github-pages?label=doc%20build) ![PyPI - Wheel](https://img.shields.io/pypi/
+     wheel/smartsim) ![PyPI - Python Version](https://img.shields.io/pypi/
+  pyversions/smartsim) ![GitHub tag (latest by date)](https://img.shields.io/
+  github/v/tag/CrayLabs/SmartSim) ![Language](https://img.shields.io/github/
 languages/top/CrayLabs/SmartSim) [![Code style: black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![codecov]
-(https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/
-badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim) [!
-[Downloads](https://static.pepy.tech/personalized-badge/
+        (https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/
+   badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim) [!
+           [Downloads](https://static.pepy.tech/personalized-badge/
 smartsim?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
-(https://pepy.tech/project/smartsim) ------------ # SmartSim SmartSim is made
-up of two parts 1. SmartSim Infrastructure Library (This repository) 2.
-[SmartRedis](https://github.com/CrayLabs/SmartRedis) The two library components
-are designed to work together, but can also be used independently. *SmartSim*
-is a workflow library that makes it easier to use common Machine Learning (ML)
-libraries, like PyTorch and TensorFlow, in High Performance Computing (HPC)
-simulations and applications. SmartSim launches ML infrastructure on HPC
-systems alongside user workloads. *SmartRedis* provides an API to connect HPC
-workloads, particularly (MPI + X) simulations, to the ML infrastructure, namely
-the The [Orchestrator database](https://www.craylabs.org/docs/
-orchestrator.html), launched by SmartSim. Applications integrated with the
-SmartRedis clients, written in Fortran, C, C++ and Python, can send data to and
-remotely request SmartSim infrastructure to execute ML models and scripts on
-GPU or CPU. The distributed Client-Server paradigm allows for data to be
-seamlessly exchanged between applications at runtime without the utilization of
-MPI. ---------- **Table of Contents** - [SmartSim](#smartsim) - [Quick Start]
-(#quick-start) - [SmartSim Infrastructure Library](#smartsim-infrastructure-
-library) - [Experiments](#experiments) - [Hello World](#hello-world) - [Hello
-World MPI](#hello-world-mpi) - [Experiments on HPC Systems](#experiments-on-
-hpc-systems) - [Interactive Launch Example](#interactive-launch-example) -
-[Batch Launch Examples](#batch-launch-examples) - [Infrastructure Library
-Applications](#infrastructure-library-applications) - [Redis + RedisAI](#redis-
--redisai) - [Local Launch](#local-launch) - [Interactive Launch](#interactive-
-launch) - [Batch Launch](#batch-launch) - [Ray](#ray) - [Ray on HPC](#ray-on-
-hpc) - [SmartRedis](#smartredis) - [Tensors](#tensors) - [Datasets](#datasets)
-- [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-tutorials) - [Run the
-Tutorials](#run-the-tutorials) - [Online Analysis](#online-analysis) - [Lattice
-Boltzmann Simulation](#lattice-boltzmann-simulation) - [Online Processing]
-(#online-processing) - [Singular Value Decomposition](#singular-value-
-decomposition) - [Online Inference](#online-inference) - [PyTorch CNN Example]
-(#pytorch-cnn-example) - [Publications](#publications) - [Cite](#cite) -
-[bibtex](#bibtex) ---- # Quick Start The documentation has a number of
-tutorials that make it easy to get used to SmartSim locally before using it on
-your system. Each tutorial is a Jupyter notebook that can be run through the
-[SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/
-packages?repo_name=SmartSim) which will run a jupyter lab with the tutorials,
-SmartSim, and SmartRedis installed. ```bash docker pull ghcr.io/craylabs/
-smartsim-tutorials:v0.4.1 docker run -p 8888:8888 ghcr.io/craylabs/smartsim-
-tutorials:v0.4.1 # click on link to open jupyter lab ``` # SmartSim
-Infrastructure Library The Infrastructure Library (IL), the ``smartsim`` python
-package, facilitates the launch of Machine Learning and simulation workflows.
-The Python interface of the IL creates, configures, launches and monitors
-applications. ## Experiments The [Experiment](https://www.craylabs.org/docs/
-api/smartsim_api.html#experiment) object is the main interface of SmartSim.
-Through the [Experiment](https://www.craylabs.org/docs/api/
-smartsim_api.html#experiment) users can create references to user applications
-called ``Models``. ### Hello World Below is a simple example of a workflow that
-uses the IL to launch hello world program using the local launcher which is
-designed for laptops and single nodes. ```python from smartsim import
-Experiment exp = Experiment("simple", launcher="local") settings =
-exp.create_run_settings("echo", exe_args="Hello World") model =
+                     (https://pepy.tech/project/smartsim)
+------------ # SmartSim SmartSim is made up of two parts 1. SmartSim
+Infrastructure Library (This repository) 2. [SmartRedis](https://github.com/
+CrayLabs/SmartRedis) The two library components are designed to work together,
+but can also be used independently. *SmartSim* is a workflow library that makes
+it easier to use common Machine Learning (ML) libraries, like PyTorch and
+TensorFlow, in High Performance Computing (HPC) simulations and applications.
+SmartSim launches ML infrastructure on HPC systems alongside user workloads.
+*SmartRedis* provides an API to connect HPC workloads, particularly (MPI + X)
+simulations, to the ML infrastructure, namely the The [Orchestrator database]
+(https://www.craylabs.org/docs/orchestrator.html), launched by SmartSim.
+Applications integrated with the SmartRedis clients, written in Fortran, C, C++
+and Python, can send data to and remotely request SmartSim infrastructure to
+execute ML models and scripts on GPU or CPU. The distributed Client-Server
+paradigm allows for data to be seamlessly exchanged between applications at
+runtime without the utilization of MPI. ---------- **Table of Contents** -
+[SmartSim](#smartsim) - [Quick Start](#quick-start) - [SmartSim Infrastructure
+Library](#smartsim-infrastructure-library) - [Experiments](#experiments) -
+[Hello World](#hello-world) - [Hello World MPI](#hello-world-mpi) -
+[Experiments on HPC Systems](#experiments-on-hpc-systems) - [Interactive Launch
+Example](#interactive-launch-example) - [Batch Launch Examples](#batch-launch-
+examples) - [Infrastructure Library Applications](#infrastructure-library-
+applications) - [Redis + RedisAI](#redis--redisai) - [Local Launch](#local-
+launch) - [Interactive Launch](#interactive-launch) - [Batch Launch](#batch-
+launch) - [SmartRedis](#smartredis) - [Tensors](#tensors) - [Datasets]
+(#datasets) - [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-
+tutorials) - [Run the Tutorials](#run-the-tutorials) - [Online Analysis]
+(#online-analysis) - [Lattice Boltzmann Simulation](#lattice-boltzmann-
+simulation) - [Online Processing](#online-processing) - [Singular Value
+Decomposition](#singular-value-decomposition) - [Online Inference](#online-
+inference) - [PyTorch CNN Example](#pytorch-cnn-example) - [Publications]
+(#publications) - [Cite](#cite) - [bibtex](#bibtex) ---- # Quick Start The
+documentation has a number of tutorials that make it easy to get used to
+SmartSim locally before using it on your system. Each tutorial is a Jupyter
+notebook that can be run through the [SmartSim Tutorials docker image](https://
+github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
+lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
+ghcr.io/craylabs/smartsim-tutorials:v0.4.2 docker run -p 8888:8888 ghcr.io/
+craylabs/smartsim-tutorials:v0.4.2 # click on link to open jupyter lab ``` #
+SmartSim Infrastructure Library The Infrastructure Library (IL), the
+``smartsim`` python package, facilitates the launch of Machine Learning and
+simulation workflows. The Python interface of the IL creates, configures,
+launches and monitors applications. ## Experiments The [Experiment](https://
+www.craylabs.org/docs/api/smartsim_api.html#experiment) object is the main
+interface of SmartSim. Through the [Experiment](https://www.craylabs.org/docs/
+api/smartsim_api.html#experiment) users can create references to user
+applications called ``Models``. ### Hello World Below is a simple example of a
+workflow that uses the IL to launch hello world program using the local
+launcher which is designed for laptops and single nodes. ```python from
+smartsim import Experiment exp = Experiment("simple", launcher="local")
+settings = exp.create_run_settings("echo", exe_args="Hello World") model =
 exp.create_model("hello_world", settings) exp.start(model, block=True) print
 (exp.get_status(model)) ``` ### Hello World MPI The
 [Experiment.create_run_settings](https://www.craylabs.org/docs/api/
 smartsim_api.html#smartsim.experiment.Experiment.create_run_settings) method
 returns a ``RunSettings`` object which defines how a model is launched. There
 are many types of ``RunSettings`` [supported by SmartSim](https://
 www.craylabs.org/docs/api/smartsim_api.html#settings). - ``RunSettings`` -
@@ -128,23 +128,22 @@
 replicas=4) exp.start(ensemble, block=True, summary=True) print(exp.get_status
 (ensemble)) ``` ```bash python hello_ensemble.py ``` Similar to the interactive
 example, this same script will run on a SLURM, PBS, LSF, or Cobalt system as
 the ``launcher`` is set to `auto` in the [Experiment](https://www.craylabs.org/
 docs/api/smartsim_api.html#experiment) initialization. Local launching does not
 support batch workloads. -------- # Infrastructure Library Applications -
 Orchestrator - In-memory data store and Machine Learning Inference (Redis +
-RedisAI) - Ray - Distributed Reinforcement Learning (RL), Hyperparameter
-Optimization (HPO) ## Redis + RedisAI The ``Orchestrator`` is an in-memory
-database that utilizes Redis and RedisAI to provide a distributed database and
-access to ML runtimes from Fortran, C, C++ and Python. SmartSim provides
-classes that make it simple to launch the database in many configurations and
-optionally form a distributed database cluster. The examples below will show
-how to launch the database. Later in this document we will show how to use the
-database to perform ML inference and processing. ### Local Launch The following
-script launches a single database using the local launcher.
+RedisAI) ## Redis + RedisAI The ``Orchestrator`` is an in-memory database that
+utilizes Redis and RedisAI to provide a distributed database and access to ML
+runtimes from Fortran, C, C++ and Python. SmartSim provides classes that make
+it simple to launch the database in many configurations and optionally form a
+distributed database cluster. The examples below will show how to launch the
+database. Later in this document we will show how to use the database to
+perform ML inference and processing. ### Local Launch The following script
+launches a single database using the local launcher.
 [Experiment.create_database](https://www.craylabs.org/docs/api/
 smartsim_api.html#smartsim.experiment.Experiment.create_database) will
 initialize an ``Orchestrator`` instance corresponding to the specified
 launcher. ```python # run_db_local.py from smartsim import Experiment exp =
 Experiment("local-db", launcher="local") db = exp.create_database(port=6780, #
 database port interface="lo") # network interface to use # by default, SmartSim
 never blocks execution after the database is launched. exp.start(db) # launch
@@ -170,81 +169,59 @@
 Users can hit CTRL-C to cancel the launch if needed. ```Python #
 run_db_batch.py from smartsim import Experiment exp = Experiment("batch-db-on-
 pbs", launcher="auto") db_cluster = exp.create_database(db_nodes=3,
 db_port=6780, batch=True, time="00:10:00", interface="ib0", account="12345-
 Cray", queue="cl40") exp.start(db_cluster) print(f"Orchestrator launched on
 nodes: {db_cluster.hosts}") # launch models, analysis, training, inference
 sessions, etc # that communicate with the database using the SmartRedis clients
-exp.stop(db_cluster) ``` ```bash python run_db_batch.py ``` ----- ## Ray Ray is
-a distributed computation framework that supports a number of applications -
-RLlib - Distributed Reinforcement Learning (RL) - RaySGD - Distributed Training
-- Ray Tune - Hyperparameter Optimization (HPO) - Ray Serve - ML/DL inference As
-well as other integrations with frameworks like Modin, Mars, Dask, and Spark.
-Historically, Ray has not been well supported on HPC systems. A few examples
-exist, but none are well maintained. Because SmartSim already has launchers for
-HPC systems, launching Ray through SmartSim is a relatively simple task. ###
-Ray on HPC Below is an example of how to launch a Ray cluster on an HPC system
-and connect to it. In this example, we set `batch=True`, which means that the
-cluster will be started requesting an allocation through the scheduler (Slurm,
-PBS, etc). If this code is run within a sufficiently large interactive
-allocation, setting `batch=False` will spin the Ray cluster on the allocated
-nodes. ```Python import ray from smartsim import Experiment from
-smartsim.exp.ray import RayCluster exp = Experiment("ray-cluster",
-launcher='auto') # 3 workers + 1 head node = 4 node-cluster cluster =
-RayCluster(name="ray-cluster", run_args={}, ray_args={"num-cpus": 24},
-launcher='auto', num_nodes=4, batch=True) exp.generate(cluster, overwrite=True)
-exp.start(cluster, block=False, summary=True) # Connect to the Ray cluster ctx
-= ray.init(f"ray://{cluster.get_head_address()}:10001") #
- RLlib, HPO...> ``` *New in 0.4.0* the auto argument enables the Ray Cluster to
-be launched across scheduler types. Both batch launch and interactive launch
-commands will be automatically detected and used by SmartSim. ------ #
-SmartRedis The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/
-SmartRedis)) are implementations of Redis clients that implement the RedisAI
-API with additions specific to scientific workflows. SmartRedis clients are
-available in Fortran, C, C++, and Python. Users can seamlessly pull and push
-data from the Orchestrator from different languages. ## Tensors Tensors are the
-fundamental data structure for the SmartRedis clients. The Clients use the
-native array format of the language. For example, in Python, a tensor is a
-NumPy array while the C/C++ clients accept nested and contiguous arrays. When
-stored in the database, all tensors are stored in the same format. Hence, any
-language can receive a tensor from the database no matter what supported
-language the array was sent from. This enables applications in different
-languages to communicate numerical data with each other at runtime. For more
-information on the tensor data structure, see [the documentation](https://
-www.craylabs.org/docs/sr_data_structures.html#tensor) ## Datasets Datasets are
-collections of Tensors and associated metadata. The ``Dataset`` class is a user
-space object that can be created, added to, sent to, and retrieved from the
-Orchestrator. For an example of how to use the ``Dataset`` class, see the
-[Online Analysis example](#online-analysis) For more information on the API,
-see the [API documentation](https://www.craylabs.org/docs/
-sr_data_structures.html#dataset) # SmartSim + SmartRedis Tutorials SmartSim and
-SmartRedis were designed to work together. When launched through SmartSim,
-applications using the SmartRedis clients are directly connected to any
-Orchestrator launched in the same [Experiment](https://www.craylabs.org/docs/
-api/smartsim_api.html#experiment). In this way, a SmartSim [Experiment](https:/
-/www.craylabs.org/docs/api/smartsim_api.html#experiment) becomes a driver for
-coupled ML and Simulation workflows. The following are simple examples of how
-to use SmartSim and SmartRedis together. ## Run the Tutorials Each tutorial is
-a Jupyter notebook that can be run through the [SmartSim Tutorials docker
-image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will
-run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
-```bash docker pull ghcr.io/craylabs/smartsim-tutorials:v1 docker run -p 8888:
-8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1 ``` Each of the following
-examples can be found in the [SmartSim documentation](https://www.craylabs.org/
-docs/tutorials/getting_started/getting_started.html). ## Online Analysis Using
-SmartSim, HPC applications can be monitored in real time by streaming data from
-the application to the database. SmartRedis clients can retrieve the data,
-process, analyze it, and finally store any updated data back to the database
-for use by other clients. The following is an example of how a user could
-monitor and analyze a simulation. The example here uses the Python client;
-however, SmartRedis clients are also available for C, C++, and Fortran. All
-SmartRedis clients implement the same API. The example will produce [this
-visualization](https://user-images.githubusercontent.com/13009163/127622717-
-2c9e4cfd-50f4-4d94-88c4-8c05fa2fa616.mp4) while the simulation is running. ####
-Lattice Boltzmann Simulation Using a [Lattice Boltzmann Simulation](https://
+exp.stop(db_cluster) ``` ```bash python run_db_batch.py ``` ------ # SmartRedis
+The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/SmartRedis))
+are implementations of Redis clients that implement the RedisAI API with
+additions specific to scientific workflows. SmartRedis clients are available in
+Fortran, C, C++, and Python. Users can seamlessly pull and push data from the
+Orchestrator from different languages. ## Tensors Tensors are the fundamental
+data structure for the SmartRedis clients. The Clients use the native array
+format of the language. For example, in Python, a tensor is a NumPy array while
+the C/C++ clients accept nested and contiguous arrays. When stored in the
+database, all tensors are stored in the same format. Hence, any language can
+receive a tensor from the database no matter what supported language the array
+was sent from. This enables applications in different languages to communicate
+numerical data with each other at runtime. For more information on the tensor
+data structure, see [the documentation](https://www.craylabs.org/docs/
+sr_data_structures.html#tensor) ## Datasets Datasets are collections of Tensors
+and associated metadata. The ``Dataset`` class is a user space object that can
+be created, added to, sent to, and retrieved from the Orchestrator. For an
+example of how to use the ``Dataset`` class, see the [Online Analysis example]
+(#online-analysis) For more information on the API, see the [API documentation]
+(https://www.craylabs.org/docs/sr_data_structures.html#dataset) # SmartSim +
+SmartRedis Tutorials SmartSim and SmartRedis were designed to work together.
+When launched through SmartSim, applications using the SmartRedis clients are
+directly connected to any Orchestrator launched in the same [Experiment](https:
+//www.craylabs.org/docs/api/smartsim_api.html#experiment). In this way, a
+SmartSim [Experiment](https://www.craylabs.org/docs/api/
+smartsim_api.html#experiment) becomes a driver for coupled ML and Simulation
+workflows. The following are simple examples of how to use SmartSim and
+SmartRedis together. ## Run the Tutorials Each tutorial is a Jupyter notebook
+that can be run through the [SmartSim Tutorials docker image](https://
+github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
+lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
+ghcr.io/craylabs/smartsim-tutorials:v1 docker run -p 8888:8888 ghcr.io/
+craylabs/smartsim-tutorials:v0.4.2 ``` Each of the following examples can be
+found in the [SmartSim documentation](https://www.craylabs.org/docs/tutorials/
+getting_started/getting_started.html). ## Online Analysis Using SmartSim, HPC
+applications can be monitored in real time by streaming data from the
+application to the database. SmartRedis clients can retrieve the data, process,
+analyze it, and finally store any updated data back to the database for use by
+other clients. The following is an example of how a user could monitor and
+analyze a simulation. The example here uses the Python client; however,
+SmartRedis clients are also available for C, C++, and Fortran. All SmartRedis
+clients implement the same API. The example will produce [this visualization]
+(https://user-images.githubusercontent.com/13009163/127622717-2c9e4cfd-50f4-
+4d94-88c4-8c05fa2fa616.mp4) while the simulation is running. #### Lattice
+Boltzmann Simulation Using a [Lattice Boltzmann Simulation](https://
 en.wikipedia.org/wiki/Lattice_Boltzmann_methods), this example demonstrates how
 to use the SmartRedis ``Dataset`` API to stream data over the Orchestrator
 deployed by SmartSim. The simulation will be composed of two parts: `fv_sim.py`
 which will generate data from the Simulation and store it in the Orchestrator,
 and `driver.py` which will launch the Orchestrator, start `fv_sim.py` and check
 for data posted to the Orchestrator to plot updates in real-time. The following
 code highlights the sections of `fv_sim.py` that are responsible for
@@ -305,17 +282,17 @@
 computational pipelines of functions, scripts, and models. See the full
 [TorchScript Language Reference](https://pytorch.org/docs/stable/
 jit.html#torchscript-language) documentation for more information on available
 methods, functions, and how to create your own. ## Online Inference SmartSim
 supports the following frameworks for querying Machine Learning models from C,
 C++, Fortran and Python with the SmartRedis Clients:
 RedisAI Version  Libraries        Supported Version
-                 PyTorch          1.7.x
-1.2.3-1.2.4      TensorFlow\Keras 2.4.x-2.5.x
-                 ONNX             1.9.x
+                 PyTorch          1.11.x
+1.2.7            TensorFlow\Keras 2.8.x
+                 ONNX             1.11.x
 TensorFlow\Keras 2.6.x
 ONNX             1.9.x
 A [number of other libraries](https://github.com/onnx/onnxmltools) are
 supported through ONNX, like [SciKit-Learn](https://github.com/onnx/sklearn-
 onnx/) and [XGBoost](https://github.com/onnx/onnxmltools/tree/master/tests/
 xgboost). **Note:** It's important to remember that SmartSim utilizes a client-
 server model. To run experiments that utilize the above frameworks, you must
@@ -357,13 +334,13 @@
 {Journal of Computational Science}, volume = {62}, pages = {101707}, year =
 {2022}, issn = {1877-7503}, doi = {https://doi.org/10.1016/j.jocs.2022.101707},
 url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
 author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E.
 Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins}, keywords =
 {Deep learning, Numerical simulation, Climate modeling, High performance
 computing, SmartSim}, } ``` Keywords: scientific,ai,workflow,hpc,analysis
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: License :: OSI Approved :: BSD License Classifier:
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: License :: OSI Approved :: BSD License Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: dev Provides-Extra: ml Provides-Extra: ray
+Engineering Requires-Python: <3.11,>=3.8 Description-Content-Type: text/
+markdown Provides-Extra: dev Provides-Extra: ml
```

### Comparing `smartsim-0.4.1/README.md` & `smartsim-0.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,25 +12,29 @@
     <a href="https://github.com/CrayLabs"><b>Cray Labs</b></a>&nbsp;&nbsp;&nbsp;
   </div>
     <br />
     <br />
 </div>
 
 
+<div align="center">
+
 [![License](https://img.shields.io/github/license/CrayLabs/SmartSim)](https://github.com/CrayLabs/SmartSim/blob/master/LICENSE.md)
 ![GitHub last commit](https://img.shields.io/github/last-commit/CrayLabs/SmartSim)
 ![GitHub deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/github-pages?label=doc%20build)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/smartsim)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/smartsim)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/CrayLabs/SmartSim)
 ![Language](https://img.shields.io/github/languages/top/CrayLabs/SmartSim)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![codecov](https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim)
 [![Downloads](https://static.pepy.tech/personalized-badge/smartsim?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/smartsim)
 
+</div>
+
 ------------
 
 # SmartSim
 
 SmartSim is made up of two parts
   1. SmartSim Infrastructure Library (This repository)
   2. [SmartRedis](https://github.com/CrayLabs/SmartRedis)
@@ -65,16 +69,14 @@
     - [Interactive Launch Example](#interactive-launch-example)
     - [Batch Launch Examples](#batch-launch-examples)
 - [Infrastructure Library Applications](#infrastructure-library-applications)
   - [Redis + RedisAI](#redis--redisai)
     - [Local Launch](#local-launch)
     - [Interactive Launch](#interactive-launch)
     - [Batch Launch](#batch-launch)
-  - [Ray](#ray)
-    - [Ray on HPC](#ray-on-hpc)
 - [SmartRedis](#smartredis)
   - [Tensors](#tensors)
   - [Datasets](#datasets)
 - [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-tutorials)
   - [Run the Tutorials](#run-the-tutorials)
   - [Online Analysis](#online-analysis)
       - [Lattice Boltzmann Simulation](#lattice-boltzmann-simulation)
@@ -93,16 +95,16 @@
 
 The documentation has a number of tutorials that make it easy to get used to SmartSim locally
 before using it on your system. Each tutorial is a Jupyter notebook that can be run through the
 [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
 which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
 
 ```bash
-docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.1
-docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
+docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.2
+docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
 # click on link to open jupyter lab
 ```
 
 # SmartSim Infrastructure Library
 
 The Infrastructure Library (IL), the ``smartsim`` python package,
 facilitates the launch of Machine Learning and simulation
@@ -280,15 +282,14 @@
 initialization. Local launching does not support batch workloads.
 
 
 --------
 
 # Infrastructure Library Applications
  - Orchestrator - In-memory data store and Machine Learning Inference (Redis + RedisAI)
- - Ray - Distributed Reinforcement Learning (RL), Hyperparameter Optimization (HPO)
 
 ## Redis + RedisAI
 
 The ``Orchestrator`` is an in-memory database that utilizes Redis and RedisAI to provide
 a distributed database and access to ML runtimes from Fortran, C, C++ and Python.
 
 SmartSim provides classes that make it simple to launch the database in many
@@ -394,61 +395,14 @@
 exp.stop(db_cluster)
 ```
 
 ```bash
 python run_db_batch.py
 ```
 
------
-## Ray
-
-Ray is a distributed computation framework that supports a number of applications
- - RLlib - Distributed Reinforcement Learning (RL)
- - RaySGD - Distributed Training
- - Ray Tune - Hyperparameter Optimization (HPO)
- - Ray Serve - ML/DL inference
-As well as other integrations with frameworks like Modin, Mars, Dask, and Spark.
-
-Historically, Ray has not been well supported on HPC systems. A few examples exist,
-but none are well maintained. Because SmartSim already has launchers for HPC systems,
-launching Ray through SmartSim is a relatively simple task.
-
-### Ray on HPC
-
-Below is an example of how to launch a Ray cluster on an HPC system and connect to it.
-In this example, we set `batch=True`, which means that the cluster will be started
-requesting an allocation through the scheduler (Slurm, PBS, etc). If this code
-is run within a sufficiently large interactive allocation, setting `batch=False`
-will spin the Ray cluster on the allocated nodes.
-
-```Python
-import ray
-
-from smartsim import Experiment
-from smartsim.exp.ray import RayCluster
-
-exp = Experiment("ray-cluster", launcher='auto')
-# 3 workers + 1 head node = 4 node-cluster
-cluster = RayCluster(name="ray-cluster", run_args={},
-                     ray_args={"num-cpus": 24},
-                     launcher='auto', num_nodes=4, batch=True)
-
-exp.generate(cluster, overwrite=True)
-exp.start(cluster, block=False, summary=True)
-
-# Connect to the Ray cluster
-ctx = ray.init(f"ray://{cluster.get_head_address()}:10001")
-
-# <run Ray tune, RLlib, HPO...>
-```
-
-*New in 0.4.0* the auto argument enables the Ray Cluster to be launched
-across scheduler types. Both batch launch and interactive launch commands
-will be automatically detected and used by SmartSim.
-
 ------
 # SmartRedis
 
 The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/SmartRedis))
 are implementations of Redis clients that implement the RedisAI
 API with additions specific to scientific workflows.
 
@@ -494,15 +448,15 @@
 
 Each tutorial is a Jupyter notebook that can be run through the
 [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
 which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
 
 ```bash
 docker pull ghcr.io/craylabs/smartsim-tutorials:v1
-docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
+docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
 ```
 Each of the following examples can be found in the
 [SmartSim documentation](https://www.craylabs.org/docs/tutorials/getting_started/getting_started.html).
 
 ## Online Analysis
 
 Using SmartSim, HPC applications can be monitored in real time by streaming data
@@ -679,25 +633,25 @@
       <th style="text-align:center">RedisAI Version</th>
       <th style="text-align:center">Libraries</th>
       <th style="text-align:center">Supported Version</th>
     </tr>
   </thead>
   <tbody style="text-align:center">
     <tr>
-      <td rowspan="3">1.2.3-1.2.4</td>
+      <td rowspan="3">1.2.7</td>
       <td>PyTorch</td>
-      <td>1.7.x</td>
+      <td>1.11.x</td>
     </tr>
     <tr>
       <td>TensorFlow\Keras</td>
-      <td>2.4.x-2.5.x</td>
+      <td>2.8.x</td>
     </tr>
     <tr>
       <td>ONNX</td>
-      <td>1.9.x</td>
+      <td>1.11.x</td>
     </tr>
       <td rowspan="3">1.2.5</td>
       <td>PyTorch</td>
       <td>1.9.x</td>
     </tr>
     <tr>
       <td>TensorFlow\Keras</td>
```

#### html2text {}

```diff
@@ -1,78 +1,78 @@
     [https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/
                           SmartSim_Large.png][Image]
 
        Home    Install    Documentation    Slack_Invite    Cray_Labs   
 
 
 [![License](https://img.shields.io/github/license/CrayLabs/SmartSim)](https://
-github.com/CrayLabs/SmartSim/blob/master/LICENSE.md) ![GitHub last commit]
-(https://img.shields.io/github/last-commit/CrayLabs/SmartSim) ![GitHub
-deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/
-github-pages?label=doc%20build) ![PyPI - Wheel](https://img.shields.io/pypi/
-wheel/smartsim) ![PyPI - Python Version](https://img.shields.io/pypi/
-pyversions/smartsim) ![GitHub tag (latest by date)](https://img.shields.io/
-github/v/tag/CrayLabs/SmartSim) ![Language](https://img.shields.io/github/
+  github.com/CrayLabs/SmartSim/blob/master/LICENSE.md) ![GitHub last commit]
+    (https://img.shields.io/github/last-commit/CrayLabs/SmartSim) ![GitHub
+   deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/
+ github-pages?label=doc%20build) ![PyPI - Wheel](https://img.shields.io/pypi/
+     wheel/smartsim) ![PyPI - Python Version](https://img.shields.io/pypi/
+  pyversions/smartsim) ![GitHub tag (latest by date)](https://img.shields.io/
+  github/v/tag/CrayLabs/SmartSim) ![Language](https://img.shields.io/github/
 languages/top/CrayLabs/SmartSim) [![Code style: black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![codecov]
-(https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/
-badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim) [!
-[Downloads](https://static.pepy.tech/personalized-badge/
+        (https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/
+   badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim) [!
+           [Downloads](https://static.pepy.tech/personalized-badge/
 smartsim?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
-(https://pepy.tech/project/smartsim) ------------ # SmartSim SmartSim is made
-up of two parts 1. SmartSim Infrastructure Library (This repository) 2.
-[SmartRedis](https://github.com/CrayLabs/SmartRedis) The two library components
-are designed to work together, but can also be used independently. *SmartSim*
-is a workflow library that makes it easier to use common Machine Learning (ML)
-libraries, like PyTorch and TensorFlow, in High Performance Computing (HPC)
-simulations and applications. SmartSim launches ML infrastructure on HPC
-systems alongside user workloads. *SmartRedis* provides an API to connect HPC
-workloads, particularly (MPI + X) simulations, to the ML infrastructure, namely
-the The [Orchestrator database](https://www.craylabs.org/docs/
-orchestrator.html), launched by SmartSim. Applications integrated with the
-SmartRedis clients, written in Fortran, C, C++ and Python, can send data to and
-remotely request SmartSim infrastructure to execute ML models and scripts on
-GPU or CPU. The distributed Client-Server paradigm allows for data to be
-seamlessly exchanged between applications at runtime without the utilization of
-MPI. ---------- **Table of Contents** - [SmartSim](#smartsim) - [Quick Start]
-(#quick-start) - [SmartSim Infrastructure Library](#smartsim-infrastructure-
-library) - [Experiments](#experiments) - [Hello World](#hello-world) - [Hello
-World MPI](#hello-world-mpi) - [Experiments on HPC Systems](#experiments-on-
-hpc-systems) - [Interactive Launch Example](#interactive-launch-example) -
-[Batch Launch Examples](#batch-launch-examples) - [Infrastructure Library
-Applications](#infrastructure-library-applications) - [Redis + RedisAI](#redis-
--redisai) - [Local Launch](#local-launch) - [Interactive Launch](#interactive-
-launch) - [Batch Launch](#batch-launch) - [Ray](#ray) - [Ray on HPC](#ray-on-
-hpc) - [SmartRedis](#smartredis) - [Tensors](#tensors) - [Datasets](#datasets)
-- [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-tutorials) - [Run the
-Tutorials](#run-the-tutorials) - [Online Analysis](#online-analysis) - [Lattice
-Boltzmann Simulation](#lattice-boltzmann-simulation) - [Online Processing]
-(#online-processing) - [Singular Value Decomposition](#singular-value-
-decomposition) - [Online Inference](#online-inference) - [PyTorch CNN Example]
-(#pytorch-cnn-example) - [Publications](#publications) - [Cite](#cite) -
-[bibtex](#bibtex) ---- # Quick Start The documentation has a number of
-tutorials that make it easy to get used to SmartSim locally before using it on
-your system. Each tutorial is a Jupyter notebook that can be run through the
-[SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/
-packages?repo_name=SmartSim) which will run a jupyter lab with the tutorials,
-SmartSim, and SmartRedis installed. ```bash docker pull ghcr.io/craylabs/
-smartsim-tutorials:v0.4.1 docker run -p 8888:8888 ghcr.io/craylabs/smartsim-
-tutorials:v0.4.1 # click on link to open jupyter lab ``` # SmartSim
-Infrastructure Library The Infrastructure Library (IL), the ``smartsim`` python
-package, facilitates the launch of Machine Learning and simulation workflows.
-The Python interface of the IL creates, configures, launches and monitors
-applications. ## Experiments The [Experiment](https://www.craylabs.org/docs/
-api/smartsim_api.html#experiment) object is the main interface of SmartSim.
-Through the [Experiment](https://www.craylabs.org/docs/api/
-smartsim_api.html#experiment) users can create references to user applications
-called ``Models``. ### Hello World Below is a simple example of a workflow that
-uses the IL to launch hello world program using the local launcher which is
-designed for laptops and single nodes. ```python from smartsim import
-Experiment exp = Experiment("simple", launcher="local") settings =
-exp.create_run_settings("echo", exe_args="Hello World") model =
+                     (https://pepy.tech/project/smartsim)
+------------ # SmartSim SmartSim is made up of two parts 1. SmartSim
+Infrastructure Library (This repository) 2. [SmartRedis](https://github.com/
+CrayLabs/SmartRedis) The two library components are designed to work together,
+but can also be used independently. *SmartSim* is a workflow library that makes
+it easier to use common Machine Learning (ML) libraries, like PyTorch and
+TensorFlow, in High Performance Computing (HPC) simulations and applications.
+SmartSim launches ML infrastructure on HPC systems alongside user workloads.
+*SmartRedis* provides an API to connect HPC workloads, particularly (MPI + X)
+simulations, to the ML infrastructure, namely the The [Orchestrator database]
+(https://www.craylabs.org/docs/orchestrator.html), launched by SmartSim.
+Applications integrated with the SmartRedis clients, written in Fortran, C, C++
+and Python, can send data to and remotely request SmartSim infrastructure to
+execute ML models and scripts on GPU or CPU. The distributed Client-Server
+paradigm allows for data to be seamlessly exchanged between applications at
+runtime without the utilization of MPI. ---------- **Table of Contents** -
+[SmartSim](#smartsim) - [Quick Start](#quick-start) - [SmartSim Infrastructure
+Library](#smartsim-infrastructure-library) - [Experiments](#experiments) -
+[Hello World](#hello-world) - [Hello World MPI](#hello-world-mpi) -
+[Experiments on HPC Systems](#experiments-on-hpc-systems) - [Interactive Launch
+Example](#interactive-launch-example) - [Batch Launch Examples](#batch-launch-
+examples) - [Infrastructure Library Applications](#infrastructure-library-
+applications) - [Redis + RedisAI](#redis--redisai) - [Local Launch](#local-
+launch) - [Interactive Launch](#interactive-launch) - [Batch Launch](#batch-
+launch) - [SmartRedis](#smartredis) - [Tensors](#tensors) - [Datasets]
+(#datasets) - [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-
+tutorials) - [Run the Tutorials](#run-the-tutorials) - [Online Analysis]
+(#online-analysis) - [Lattice Boltzmann Simulation](#lattice-boltzmann-
+simulation) - [Online Processing](#online-processing) - [Singular Value
+Decomposition](#singular-value-decomposition) - [Online Inference](#online-
+inference) - [PyTorch CNN Example](#pytorch-cnn-example) - [Publications]
+(#publications) - [Cite](#cite) - [bibtex](#bibtex) ---- # Quick Start The
+documentation has a number of tutorials that make it easy to get used to
+SmartSim locally before using it on your system. Each tutorial is a Jupyter
+notebook that can be run through the [SmartSim Tutorials docker image](https://
+github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
+lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
+ghcr.io/craylabs/smartsim-tutorials:v0.4.2 docker run -p 8888:8888 ghcr.io/
+craylabs/smartsim-tutorials:v0.4.2 # click on link to open jupyter lab ``` #
+SmartSim Infrastructure Library The Infrastructure Library (IL), the
+``smartsim`` python package, facilitates the launch of Machine Learning and
+simulation workflows. The Python interface of the IL creates, configures,
+launches and monitors applications. ## Experiments The [Experiment](https://
+www.craylabs.org/docs/api/smartsim_api.html#experiment) object is the main
+interface of SmartSim. Through the [Experiment](https://www.craylabs.org/docs/
+api/smartsim_api.html#experiment) users can create references to user
+applications called ``Models``. ### Hello World Below is a simple example of a
+workflow that uses the IL to launch hello world program using the local
+launcher which is designed for laptops and single nodes. ```python from
+smartsim import Experiment exp = Experiment("simple", launcher="local")
+settings = exp.create_run_settings("echo", exe_args="Hello World") model =
 exp.create_model("hello_world", settings) exp.start(model, block=True) print
 (exp.get_status(model)) ``` ### Hello World MPI The
 [Experiment.create_run_settings](https://www.craylabs.org/docs/api/
 smartsim_api.html#smartsim.experiment.Experiment.create_run_settings) method
 returns a ``RunSettings`` object which defines how a model is launched. There
 are many types of ``RunSettings`` [supported by SmartSim](https://
 www.craylabs.org/docs/api/smartsim_api.html#settings). - ``RunSettings`` -
@@ -123,23 +123,22 @@
 replicas=4) exp.start(ensemble, block=True, summary=True) print(exp.get_status
 (ensemble)) ``` ```bash python hello_ensemble.py ``` Similar to the interactive
 example, this same script will run on a SLURM, PBS, LSF, or Cobalt system as
 the ``launcher`` is set to `auto` in the [Experiment](https://www.craylabs.org/
 docs/api/smartsim_api.html#experiment) initialization. Local launching does not
 support batch workloads. -------- # Infrastructure Library Applications -
 Orchestrator - In-memory data store and Machine Learning Inference (Redis +
-RedisAI) - Ray - Distributed Reinforcement Learning (RL), Hyperparameter
-Optimization (HPO) ## Redis + RedisAI The ``Orchestrator`` is an in-memory
-database that utilizes Redis and RedisAI to provide a distributed database and
-access to ML runtimes from Fortran, C, C++ and Python. SmartSim provides
-classes that make it simple to launch the database in many configurations and
-optionally form a distributed database cluster. The examples below will show
-how to launch the database. Later in this document we will show how to use the
-database to perform ML inference and processing. ### Local Launch The following
-script launches a single database using the local launcher.
+RedisAI) ## Redis + RedisAI The ``Orchestrator`` is an in-memory database that
+utilizes Redis and RedisAI to provide a distributed database and access to ML
+runtimes from Fortran, C, C++ and Python. SmartSim provides classes that make
+it simple to launch the database in many configurations and optionally form a
+distributed database cluster. The examples below will show how to launch the
+database. Later in this document we will show how to use the database to
+perform ML inference and processing. ### Local Launch The following script
+launches a single database using the local launcher.
 [Experiment.create_database](https://www.craylabs.org/docs/api/
 smartsim_api.html#smartsim.experiment.Experiment.create_database) will
 initialize an ``Orchestrator`` instance corresponding to the specified
 launcher. ```python # run_db_local.py from smartsim import Experiment exp =
 Experiment("local-db", launcher="local") db = exp.create_database(port=6780, #
 database port interface="lo") # network interface to use # by default, SmartSim
 never blocks execution after the database is launched. exp.start(db) # launch
@@ -165,81 +164,59 @@
 Users can hit CTRL-C to cancel the launch if needed. ```Python #
 run_db_batch.py from smartsim import Experiment exp = Experiment("batch-db-on-
 pbs", launcher="auto") db_cluster = exp.create_database(db_nodes=3,
 db_port=6780, batch=True, time="00:10:00", interface="ib0", account="12345-
 Cray", queue="cl40") exp.start(db_cluster) print(f"Orchestrator launched on
 nodes: {db_cluster.hosts}") # launch models, analysis, training, inference
 sessions, etc # that communicate with the database using the SmartRedis clients
-exp.stop(db_cluster) ``` ```bash python run_db_batch.py ``` ----- ## Ray Ray is
-a distributed computation framework that supports a number of applications -
-RLlib - Distributed Reinforcement Learning (RL) - RaySGD - Distributed Training
-- Ray Tune - Hyperparameter Optimization (HPO) - Ray Serve - ML/DL inference As
-well as other integrations with frameworks like Modin, Mars, Dask, and Spark.
-Historically, Ray has not been well supported on HPC systems. A few examples
-exist, but none are well maintained. Because SmartSim already has launchers for
-HPC systems, launching Ray through SmartSim is a relatively simple task. ###
-Ray on HPC Below is an example of how to launch a Ray cluster on an HPC system
-and connect to it. In this example, we set `batch=True`, which means that the
-cluster will be started requesting an allocation through the scheduler (Slurm,
-PBS, etc). If this code is run within a sufficiently large interactive
-allocation, setting `batch=False` will spin the Ray cluster on the allocated
-nodes. ```Python import ray from smartsim import Experiment from
-smartsim.exp.ray import RayCluster exp = Experiment("ray-cluster",
-launcher='auto') # 3 workers + 1 head node = 4 node-cluster cluster =
-RayCluster(name="ray-cluster", run_args={}, ray_args={"num-cpus": 24},
-launcher='auto', num_nodes=4, batch=True) exp.generate(cluster, overwrite=True)
-exp.start(cluster, block=False, summary=True) # Connect to the Ray cluster ctx
-= ray.init(f"ray://{cluster.get_head_address()}:10001") #
- RLlib, HPO...> ``` *New in 0.4.0* the auto argument enables the Ray Cluster to
-be launched across scheduler types. Both batch launch and interactive launch
-commands will be automatically detected and used by SmartSim. ------ #
-SmartRedis The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/
-SmartRedis)) are implementations of Redis clients that implement the RedisAI
-API with additions specific to scientific workflows. SmartRedis clients are
-available in Fortran, C, C++, and Python. Users can seamlessly pull and push
-data from the Orchestrator from different languages. ## Tensors Tensors are the
-fundamental data structure for the SmartRedis clients. The Clients use the
-native array format of the language. For example, in Python, a tensor is a
-NumPy array while the C/C++ clients accept nested and contiguous arrays. When
-stored in the database, all tensors are stored in the same format. Hence, any
-language can receive a tensor from the database no matter what supported
-language the array was sent from. This enables applications in different
-languages to communicate numerical data with each other at runtime. For more
-information on the tensor data structure, see [the documentation](https://
-www.craylabs.org/docs/sr_data_structures.html#tensor) ## Datasets Datasets are
-collections of Tensors and associated metadata. The ``Dataset`` class is a user
-space object that can be created, added to, sent to, and retrieved from the
-Orchestrator. For an example of how to use the ``Dataset`` class, see the
-[Online Analysis example](#online-analysis) For more information on the API,
-see the [API documentation](https://www.craylabs.org/docs/
-sr_data_structures.html#dataset) # SmartSim + SmartRedis Tutorials SmartSim and
-SmartRedis were designed to work together. When launched through SmartSim,
-applications using the SmartRedis clients are directly connected to any
-Orchestrator launched in the same [Experiment](https://www.craylabs.org/docs/
-api/smartsim_api.html#experiment). In this way, a SmartSim [Experiment](https:/
-/www.craylabs.org/docs/api/smartsim_api.html#experiment) becomes a driver for
-coupled ML and Simulation workflows. The following are simple examples of how
-to use SmartSim and SmartRedis together. ## Run the Tutorials Each tutorial is
-a Jupyter notebook that can be run through the [SmartSim Tutorials docker
-image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will
-run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
-```bash docker pull ghcr.io/craylabs/smartsim-tutorials:v1 docker run -p 8888:
-8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1 ``` Each of the following
-examples can be found in the [SmartSim documentation](https://www.craylabs.org/
-docs/tutorials/getting_started/getting_started.html). ## Online Analysis Using
-SmartSim, HPC applications can be monitored in real time by streaming data from
-the application to the database. SmartRedis clients can retrieve the data,
-process, analyze it, and finally store any updated data back to the database
-for use by other clients. The following is an example of how a user could
-monitor and analyze a simulation. The example here uses the Python client;
-however, SmartRedis clients are also available for C, C++, and Fortran. All
-SmartRedis clients implement the same API. The example will produce [this
-visualization](https://user-images.githubusercontent.com/13009163/127622717-
-2c9e4cfd-50f4-4d94-88c4-8c05fa2fa616.mp4) while the simulation is running. ####
-Lattice Boltzmann Simulation Using a [Lattice Boltzmann Simulation](https://
+exp.stop(db_cluster) ``` ```bash python run_db_batch.py ``` ------ # SmartRedis
+The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/SmartRedis))
+are implementations of Redis clients that implement the RedisAI API with
+additions specific to scientific workflows. SmartRedis clients are available in
+Fortran, C, C++, and Python. Users can seamlessly pull and push data from the
+Orchestrator from different languages. ## Tensors Tensors are the fundamental
+data structure for the SmartRedis clients. The Clients use the native array
+format of the language. For example, in Python, a tensor is a NumPy array while
+the C/C++ clients accept nested and contiguous arrays. When stored in the
+database, all tensors are stored in the same format. Hence, any language can
+receive a tensor from the database no matter what supported language the array
+was sent from. This enables applications in different languages to communicate
+numerical data with each other at runtime. For more information on the tensor
+data structure, see [the documentation](https://www.craylabs.org/docs/
+sr_data_structures.html#tensor) ## Datasets Datasets are collections of Tensors
+and associated metadata. The ``Dataset`` class is a user space object that can
+be created, added to, sent to, and retrieved from the Orchestrator. For an
+example of how to use the ``Dataset`` class, see the [Online Analysis example]
+(#online-analysis) For more information on the API, see the [API documentation]
+(https://www.craylabs.org/docs/sr_data_structures.html#dataset) # SmartSim +
+SmartRedis Tutorials SmartSim and SmartRedis were designed to work together.
+When launched through SmartSim, applications using the SmartRedis clients are
+directly connected to any Orchestrator launched in the same [Experiment](https:
+//www.craylabs.org/docs/api/smartsim_api.html#experiment). In this way, a
+SmartSim [Experiment](https://www.craylabs.org/docs/api/
+smartsim_api.html#experiment) becomes a driver for coupled ML and Simulation
+workflows. The following are simple examples of how to use SmartSim and
+SmartRedis together. ## Run the Tutorials Each tutorial is a Jupyter notebook
+that can be run through the [SmartSim Tutorials docker image](https://
+github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
+lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
+ghcr.io/craylabs/smartsim-tutorials:v1 docker run -p 8888:8888 ghcr.io/
+craylabs/smartsim-tutorials:v0.4.2 ``` Each of the following examples can be
+found in the [SmartSim documentation](https://www.craylabs.org/docs/tutorials/
+getting_started/getting_started.html). ## Online Analysis Using SmartSim, HPC
+applications can be monitored in real time by streaming data from the
+application to the database. SmartRedis clients can retrieve the data, process,
+analyze it, and finally store any updated data back to the database for use by
+other clients. The following is an example of how a user could monitor and
+analyze a simulation. The example here uses the Python client; however,
+SmartRedis clients are also available for C, C++, and Fortran. All SmartRedis
+clients implement the same API. The example will produce [this visualization]
+(https://user-images.githubusercontent.com/13009163/127622717-2c9e4cfd-50f4-
+4d94-88c4-8c05fa2fa616.mp4) while the simulation is running. #### Lattice
+Boltzmann Simulation Using a [Lattice Boltzmann Simulation](https://
 en.wikipedia.org/wiki/Lattice_Boltzmann_methods), this example demonstrates how
 to use the SmartRedis ``Dataset`` API to stream data over the Orchestrator
 deployed by SmartSim. The simulation will be composed of two parts: `fv_sim.py`
 which will generate data from the Simulation and store it in the Orchestrator,
 and `driver.py` which will launch the Orchestrator, start `fv_sim.py` and check
 for data posted to the Orchestrator to plot updates in real-time. The following
 code highlights the sections of `fv_sim.py` that are responsible for
@@ -300,17 +277,17 @@
 computational pipelines of functions, scripts, and models. See the full
 [TorchScript Language Reference](https://pytorch.org/docs/stable/
 jit.html#torchscript-language) documentation for more information on available
 methods, functions, and how to create your own. ## Online Inference SmartSim
 supports the following frameworks for querying Machine Learning models from C,
 C++, Fortran and Python with the SmartRedis Clients:
 RedisAI Version  Libraries        Supported Version
-                 PyTorch          1.7.x
-1.2.3-1.2.4      TensorFlow\Keras 2.4.x-2.5.x
-                 ONNX             1.9.x
+                 PyTorch          1.11.x
+1.2.7            TensorFlow\Keras 2.8.x
+                 ONNX             1.11.x
 TensorFlow\Keras 2.6.x
 ONNX             1.9.x
 A [number of other libraries](https://github.com/onnx/onnxmltools) are
 supported through ONNX, like [SciKit-Learn](https://github.com/onnx/sklearn-
 onnx/) and [XGBoost](https://github.com/onnx/onnxmltools/tree/master/tests/
 xgboost). **Note:** It's important to remember that SmartSim utilizes a client-
 server model. To run experiments that utilize the above frameworks, you must
```

### Comparing `smartsim-0.4.1/setup.cfg` & `smartsim-0.4.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 author = CrayLabs, a Hewlett Packard Enterprise OSS Organization
 author_email = craylabs@hpe.com
 contact = CrayLabs, a Hewlett Packard Enterprise OSS Organization
 contact_email = craylabs@hpe.com
 license = BSD 2-Clause License
 keywords = scientific, ai, workflow, hpc, analysis
 classifiers = 
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	License :: OSI Approved :: BSD License
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 
 [options]
 packages = find:
 setup_requires = 
 	setuptools>=39.2
 	cmake>=3.13
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8,<3.11
 
 [options.packages.find]
 exclude = 
 	.third-party
 	tests
 	doc
 	smartredis
```

### Comparing `smartsim-0.4.1/setup.py` & `smartsim-0.4.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+# BSD 2-Clause License
+#
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+# 1. Redistributions of source code must retain the above copyright notice, this
+#    list of conditions and the following disclaimer.
+#
+# 2. Redistributions in binary form must reproduce the above copyright notice,
+#    this list of conditions and the following disclaimer in the documentation
+#    and/or other materials provided with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
 # Welcome to the SmartSim setup.py
 #
 # The following environment variables represent build time
 # options for SmartSim. These are only relevant to when a user
 # or CI is invoking the setup.py script.
 #
 #
@@ -97,15 +123,15 @@
 class BuildError(Exception):
     pass
 
 # Hacky workaround for solving CI build "purelib" issue
 # see https://github.com/google/or-tools/issues/616
 class InstallPlatlib(install):
     def finalize_options(self):
-        install.finalize_options(self)
+        super().finalize_options()
         if self.distribution.has_ext_modules():
             self.install_lib = self.install_platlib
 
 class SmartSimBuild(build_py):
 
     def run(self):
         database_builder = builder.DatabaseBuilder(build_env(),
@@ -114,15 +140,15 @@
         if not database_builder.is_built:
             database_builder.build_from_git(versions.REDIS_URL,
                                          versions.REDIS)
 
             database_builder.cleanup()
 
         # run original build_py command
-        build_py.run(self)
+        super().run()
 
 
 # Tested with wheel v0.29.0
 class BinaryDistribution(Distribution):
     """Distribution which always forces a binary package with platform name
 
        We use this because we want to pre-package Redis for certain
@@ -137,49 +163,48 @@
     "psutil>=5.7.2",
     "coloredlogs==10.0",
     "tabulate>=0.8.9",
     "redis-py-cluster==2.1.3",
     "redis==3.5.3",
     "tqdm>=4.50.2",
     "filelock>=3.4.2",
-    "protobuf==3.20"
+    "protobuf~=3.20",
 ]
 
 # Add SmartRedis at specific version
 deps.append("smartredis>={}".format(versions.SMARTREDIS))
 
 extras_require = {
     "dev": [
         "black>=20.8b1",
         "isort>=5.6.4",
         "pylint>=2.6.0",
         "pytest>=6.0.0",
-        "pytest-cov>=2.10.1"
+        "pytest-cov>=2.10.1",
         "click==8.0.2",
     ],
     # see smartsim/_core/_install/buildenv.py for more details
     "ml": versions.ml_extras_required(),
-    "ray": "ray>=1.6"
-    }
+}
 
 
 # rest in setup.cfg
 setup(
     version=smartsim_version,
     install_requires=deps,
     packages=["smartsim"],
     package_data={"smartsim": [
-        "_core/bin/*"
+        "_core/bin/*",
     ]},
     cmdclass={
         "build_py": SmartSimBuild,
-        "install": InstallPlatlib
+        "install": InstallPlatlib,
     },
     zip_safe=False,
     extras_require=extras_require,
     distclass=BinaryDistribution,
     entry_points={
         "console_scripts": [
-            "smart = smartsim._core._cli.__main__:main"
+            "smart = smartsim._core._cli.__main__:main",
         ]
     }
-)
+)
```

### Comparing `smartsim-0.4.1/smartsim/__init__.py` & `smartsim-0.4.2/smartsim/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -25,12 +25,12 @@
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import sys
 
 # -*- coding: utf-8 -*-
 from .version import __version__ as __version__
 
-if sys.version_info < (3, 7):  # pragma: no cover
-    sys.exit("Python 3.7 or greater must be used with SmartSim.")
+if sys.version_info < (3, 8):  # pragma: no cover
+    sys.exit("Python 3.8 or greater must be used with SmartSim.")
 
 # Main API module
 from .experiment import Experiment
```

### Comparing `smartsim-0.4.1/smartsim/_core/_cli/build.py` & `smartsim-0.4.2/smartsim/_core/_cli/build.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+# BSD 2-Clause License
+#
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+# 1. Redistributions of source code must retain the above copyright notice, this
+#    list of conditions and the following disclaimer.
+#
+# 2. Redistributions in binary form must reproduce the above copyright notice,
+#    this list of conditions and the following disclaimer in the documentation
+#    and/or other materials provided with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
 import argparse
 import os
 import sys
 from pathlib import Path
 
 import pkg_resources
 from tabulate import tabulate
@@ -19,26 +45,36 @@
 logger = get_logger("Smart", fmt=smart_logger_format)
 
 # NOTE: all smartsim modules need full paths as the smart cli
 #       may be installed into a different directory.
 
 
 def _install_torch_from_pip(versions, device="cpu", verbose=False):
+
     packages = []
     end_point = None
-    # if we are on linux cpu, use the torch without CUDA
-    if sys.platform == "linux" and device == "cpu":
-        packages.append(f"torch=={versions.TORCH}+cpu")
-        packages.append(f"torchvision=={versions.TORCHVISION}+cpu")
+
+    if sys.platform == "darwin":
+        if device == "gpu":
+            logger.warning("GPU support is not available on Mac OS X")
+        # The following is deliberately left blank as there is no
+        # alternative package available on Mac OS X
+        device_suffix = ""
+        end_point = None
+
+    # if we are on linux cpu, either CUDA or CPU must be installed
+    elif sys.platform == "linux":
         end_point = "https://download.pytorch.org/whl/torch_stable.html"
+        if device in ["gpu", "cuda"]:
+            device_suffix = versions.TORCH_CUDA_SUFFIX
+        elif device == "cpu":
+            device_suffix = versions.TORCH_CPU_SUFFIX
 
-    # otherwise just use the version downloaded by pip
-    else:
-        packages.append(f"torch=={versions.TORCH}")
-        packages.append(f"torchvision=={versions.TORCHVISION}")
+    packages.append(f"torch=={versions.TORCH}{device_suffix}")
+    packages.append(f"torchvision=={versions.TORCHVISION}{device_suffix}")
 
     pip_install(packages, end_point=end_point, verbose=verbose)
 
 
 class Build:
     def __init__(self):
         parser = argparse.ArgumentParser()
@@ -138,19 +174,14 @@
                     logger.info("Version Information:")
                     vers = self.versions.as_dict(db_name=db_name)
                     print(tabulate(vers, headers=vers.keys(), tablefmt="github"), "\n")
 
                 # REDIS/KeyDB
                 self.build_database()
 
-                if self.verbose:
-                    logger.info("Version Information:")
-                    vers = self.versions.as_dict()
-                    print(tabulate(vers, headers=vers.keys(), tablefmt="github"), "\n")
-
                 # REDISAI
                 self.build_redis_ai(
                     str(args.device),
                     pt,
                     tf,
                     onnx,
                     args.torch_dir,
@@ -162,15 +193,15 @@
                 ]
                 logger.info(
                     (", ".join(backends) if backends else "No") + " backend(s) built"
                 )
 
         except (SetupError, BuildError) as e:
             logger.error(str(e))
-            exit(1)
+            sys.exit(1)
 
         logger.info("SmartSim build complete!")
 
     def build_database(self):
         # check database installation
         database_name = "KeyDB" if self.keydb else "Redis"
         database_builder = builder.DatabaseBuilder(
@@ -187,55 +218,48 @@
         logger.info(f"{database_name} build complete!")
 
     def build_redis_ai(
         self, device, torch=True, tf=True, onnx=False, torch_dir=None, libtf_dir=None
     ):
 
         # make sure user isn't trying to do something silly on MacOS
-        if self.build_env.PLATFORM == "darwin":
-            if device == "gpu":
-                logger.error("SmartSim does not support GPU on MacOS")
-                exit(1)
-            if onnx and self.versions.REDISAI < "1.2.6":
-                logger.error("RedisAI < 1.2.6 does not support ONNX on MacOS")
-                exit(1)
-            if self.versions.REDISAI == "1.2.4" or self.versions.REDISAI == "1.2.5":
-                logger.error("RedisAI support for MacOS is broken in 1.2.4 and 1.2.5")
-                exit(1)
+        if self.build_env.PLATFORM == "darwin" and device == "gpu":
+            raise BuildError("SmartSim does not support GPU on MacOS")
 
         # decide which runtimes to build
         print("\nML Backends Requested")
-        print("-----------------------")
-        print(f"    PyTorch {self.versions.TORCH}: {color_bool(torch)}")
-        print(f"    TensorFlow {self.versions.TENSORFLOW}: {color_bool(tf)}")
-        print(f"    ONNX {self.versions.ONNX}: {color_bool(onnx)}\n")
+        backends_table = [
+            ["PyTorch", self.versions.TORCH, color_bool(torch)],
+            ["TensorFlow", self.versions.TENSORFLOW, color_bool(tf)],
+            ["ONNX", self.versions.ONNX or "Unavailable", color_bool(onnx)],
+        ]
+        print(tabulate(backends_table, tablefmt="fancy_outline"), end="\n\n")
         print(f"Building for GPU support: {color_bool(device == 'gpu')}\n")
 
         self.check_backends_install()
 
         # Check for onnx and tf in user python environemnt and prompt user
         # to download them if they are not installed. this should not break
         # the build however, as we use onnx and tf directly from RAI instead
         # of pip like we do PyTorch.
         if onnx:
             self.check_onnx_install()
         if tf:
             self.check_tf_install()
 
-        cmd = []
         # TORCH
         if torch:
             if torch_dir:
                 torch_dir = Path(torch_dir).resolve()
                 if not torch_dir.is_dir():
                     # we will always be able to find a torch version downloaded by
                     # pip so if we can't find it we know the user suggested a torch
                     # installation path that doesn't exist
                     logger.error("Could not find requested user Torch installation")
-                    exit(1)
+                    sys.exit(1)
             else:
                 # install pytorch wheel, and get the path to the cmake dir
                 # we will use in the RAI build
                 self.install_torch(device=device)
                 torch_dir = self.build_env.torch_cmake_path
 
         if tf:
@@ -327,14 +351,25 @@
                         + " Run `pip uninstall torch torchvision` and run `smart build` again"
                     )
                     logger.error(msg)  # error because this is usually fatal
             logger.info(f"Torch {self.versions.TORCH} installed in Python environment")
 
     def check_onnx_install(self):
         """Check Python environment for ONNX installation"""
+        if not self.versions.ONNX:
+            py_version = sys.version_info
+            msg = (
+                "An onnx wheel is not available for "
+                f"Python {py_version.major}.{py_version.minor}. "
+                "Instead consider using Python 3.8 or 3.9 with Onnx "
+            )
+            if sys.platform == "linux":
+                msg += "1.2.5 or "
+            msg += "1.2.7."
+            raise SetupError(msg)
         try:
             if not self.build_env.check_installed("onnx", self.versions.ONNX):
                 msg = (
                     f"ONNX {self.versions.ONNX} not installed in python environment. "
                     + f"Consider installing onnx=={self.versions.ONNX} with pip"
                 )
                 logger.warning(msg)
@@ -375,14 +410,14 @@
                 logger.error(
                     f"There is no need to build. Backends are already built and specified in the environment at 'RAI_PATH': {CONFIG.redisai}"
                 )
             else:
                 logger.error(
                     f"Before running 'smart build', unset your RAI_PATH environment variable with 'unset RAI_PATH'."
                 )
-            exit(1)
+            sys.exit(1)
         else:
             if installed_redisai_backends():
                 logger.error(
                     "If you wish to re-run `smart build`, you must first run `smart clean`."
                 )
-                exit(1)
+                sys.exit(1)
```

### Comparing `smartsim-0.4.1/smartsim/_core/_install/__pycache__/buildenv.cpython-38.pyc` & `smartsim-0.4.2/smartsim/_core/_install/__pycache__/buildenv.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 25 00:32:42 2022 UTC, .py size: 16264 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 aa57 b662 883f 0000  U........W.b.?..
+00000000: 550d 0d0a 0000 0000 2819 3764 d74c 0000  U.......(.7d.L..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 bc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6401 6c09 5a09 6400 6404 6c09 6d0a 5a0a  d.l.Z.d.d.l.m.Z.
@@ -56,15 +56,15 @@
 00000370: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
 00000380: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
 00000390: 635f 5fa9 0072 0b00 0000 720b 0000 00fa  c__..r....r.....
 000003a0: 472f 686f 6d65 2f72 756e 6e65 722f 776f  G/home/runner/wo
 000003b0: 726b 2f53 6d61 7274 5369 6d2f 536d 6172  rk/SmartSim/Smar
 000003c0: 7453 696d 2f73 6d61 7274 7369 6d2f 5f63  tSim/smartsim/_c
 000003d0: 6f72 652f 5f69 6e73 7461 6c6c 2f62 7569  ore/_install/bui
-000003e0: 6c64 656e 762e 7079 7206 0000 0015 0000  ldenv.pyr.......
+000003e0: 6c64 656e 762e 7079 7206 0000 002f 0000  ldenv.pyr..../..
 000003f0: 0073 0400 0000 0801 040d 7206 0000 0063  .s........r....c
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0300 0000 0000 0000 7388 0000 0065 005a  ........s....e.Z
 00000420: 0164 005a 0264 015a 0364 0264 0384 005a  .d.Z.d.Z.d.d...Z
 00000430: 0465 0564 0464 0584 0083 015a 0665 0564  .e.d.d.....Z.e.d
 00000440: 0664 0784 0083 015a 0765 0564 0864 0984  .d.....Z.e.d.d..
 00000450: 0083 015a 0865 0564 0a64 0b84 0083 015a  ...Z.e.d.d.....Z
@@ -90,826 +90,924 @@
 00000590: 0182 0164 0053 0029 044e da01 2e63 0100  ...d.S.).N...c..
 000005a0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
 000005b0: 0000 7300 0000 7316 0000 007c 005d 0e7d  ..s...s....|.].}
 000005c0: 0174 007c 0183 0156 0001 0071 0264 0053  .t.|...V...q.d.S
 000005d0: 00a9 014e 2901 da03 7374 7229 02da 022e  ...N)...str)....
 000005e0: 30da 0469 7465 6d72 0b00 0000 720b 0000  0..itemr....r...
 000005f0: 0072 0c00 0000 da09 3c67 656e 6578 7072  .r......<genexpr
-00000600: 3e32 0000 0073 0400 0000 0400 0200 7a2f  >2...s........z/
+00000600: 3e4c 0000 0073 0400 0000 0400 0200 7a2f  >L...s........z/
 00000610: 5665 7273 696f 6e5f 2e5f 636f 6e76 6572  Version_._conver
 00000620: 745f 746f 5f76 6572 7369 6f6e 2e3c 6c6f  t_to_version.<lo
 00000630: 6361 6c73 3e2e 3c67 656e 6578 7072 3e29  cals>.<genexpr>)
 00000640: 06da 0a69 7369 6e73 7461 6e63 65da 0756  ...isinstance..V
 00000650: 6572 7369 6f6e 7210 0000 0072 0400 0000  ersionr....r....
 00000660: da04 6a6f 696e da0e 496e 7661 6c69 6456  ..join..InvalidV
-00000670: 6572 7369 6f6e a902 da04 7365 6c66 da04  ersion....self..
+00000670: 6572 7369 6f6e 2902 da04 7365 6c66 da04  ersion)...self..
 00000680: 7665 7273 720b 0000 0072 0b00 0000 720c  versr....r....r.
 00000690: 0000 00da 135f 636f 6e76 6572 745f 746f  ....._convert_to
-000006a0: 5f76 6572 7369 6f6e 2c00 0000 730e 0000  _version,...s...
+000006a0: 5f76 6572 7369 6f6e 4600 0000 730e 0000  _versionF...s...
 000006b0: 0000 010a 0104 010a 0108 010a 0118 027a  ...............z
 000006c0: 1c56 6572 7369 6f6e 5f2e 5f63 6f6e 7665  .Version_._conve
 000006d0: 7274 5f74 6f5f 7665 7273 696f 6e63 0100  rt_to_versionc..
 000006e0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
 000006f0: 0000 4300 0000 731a 0000 0074 0074 01a0  ..C...s....t.t..
 00000700: 027c 00a1 016a 03a0 0464 01a1 0164 0219  .|...j...d...d..
 00000710: 0083 0153 0029 034e 720e 0000 0072 0100  ...S.).Nr....r..
 00000720: 0000 a905 da03 696e 74da 0d70 6b67 5f72  ......int..pkg_r
 00000730: 6573 6f75 7263 6573 da0d 7061 7273 655f  esources..parse_
 00000740: 7665 7273 696f 6eda 0c62 6173 655f 7665  version..base_ve
-00000750: 7273 696f 6eda 0573 706c 6974 a901 7219  rsion..split..r.
+00000750: 7273 696f 6eda 0573 706c 6974 a901 7218  rsion..split..r.
 00000760: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000770: 0000 da05 6d61 6a6f 7236 0000 0073 0200  ....major6...s..
+00000770: 0000 da05 6d61 6a6f 7250 0000 0073 0200  ....majorP...s..
 00000780: 0000 0004 7a0e 5665 7273 696f 6e5f 2e6d  ....z.Version_.m
 00000790: 616a 6f72 6301 0000 0000 0000 0000 0000  ajorc...........
 000007a0: 0001 0000 0004 0000 0043 0000 0073 1a00  .........C...s..
 000007b0: 0000 7400 7401 a002 7c00 a101 6a03 a004  ..t.t...|...j...
 000007c0: 6401 a101 6402 1900 8301 5300 2903 4e72  d...d.....S.).Nr
-000007d0: 0e00 0000 e901 0000 0072 1c00 0000 7222  .........r....r"
+000007d0: 0e00 0000 e901 0000 0072 1b00 0000 7221  .........r....r!
 000007e0: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-000007f0: 0000 da05 6d69 6e6f 723c 0000 0073 0200  ....minor<...s..
+000007f0: 0000 da05 6d69 6e6f 7256 0000 0073 0200  ....minorV...s..
 00000800: 0000 0002 7a0e 5665 7273 696f 6e5f 2e6d  ....z.Version_.m
 00000810: 696e 6f72 6301 0000 0000 0000 0000 0000  inorc...........
 00000820: 0001 0000 0004 0000 0043 0000 0073 1a00  .........C...s..
 00000830: 0000 7400 7401 a002 7c00 a101 6a03 a004  ..t.t...|...j...
 00000840: 6401 a101 6402 1900 8301 5300 a903 4e72  d...d.....S...Nr
-00000850: 0e00 0000 e902 0000 0072 1c00 0000 7222  .........r....r"
+00000850: 0e00 0000 e902 0000 0072 1b00 0000 7221  .........r....r!
 00000860: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000870: 0000 da05 6d69 6372 6f40 0000 0073 0200  ....micro@...s..
+00000870: 0000 da05 6d69 6372 6f5a 0000 0073 0200  ....microZ...s..
 00000880: 0000 0002 7a0e 5665 7273 696f 6e5f 2e6d  ....z.Version_.m
 00000890: 6963 726f 6301 0000 0000 0000 0000 0000  icroc...........
 000008a0: 0001 0000 0004 0000 0043 0000 0073 1800  .........C...s..
 000008b0: 0000 7400 7401 a002 7c00 a101 8301 a003  ..t.t...|.......
-000008c0: 6401 a101 6402 1900 5300 7226 0000 0029  d...d...S.r&...)
-000008d0: 0472 1000 0000 721e 0000 0072 1f00 0000  .r....r....r....
-000008e0: 7221 0000 0072 2200 0000 720b 0000 0072  r!...r"...r....r
+000008c0: 6401 a101 6402 1900 5300 7225 0000 0029  d...d...S.r%...)
+000008d0: 0472 1000 0000 721d 0000 0072 1e00 0000  .r....r....r....
+000008e0: 7220 0000 0072 2100 0000 720b 0000 0072  r ...r!...r....r
 000008f0: 0b00 0000 720c 0000 00da 0570 6174 6368  ....r......patch
-00000900: 4400 0000 7302 0000 0000 037a 0e56 6572  D...s......z.Ver
+00000900: 5e00 0000 7302 0000 0000 037a 0e56 6572  ^...s......z.Ver
 00000910: 7369 6f6e 5f2e 7061 7463 6863 0200 0000  sion_.patchc....
 00000920: 0000 0000 0000 0000 0200 0000 0800 0000  ................
 00000930: 0300 0000 733c 0000 007a 1674 007c 0083  ....s<...z.t.|..
 00000940: 01a0 017c 00a0 027c 01a1 01a1 0157 0053  ...|...|.....W.S
 00000950: 0004 0074 036b 0a72 3601 0001 0001 0074  ...t.k.r6......t
 00000960: 0483 00a0 017c 01a1 0106 0059 0053 0058  .....|.....Y.S.X
 00000970: 0064 0053 0072 0f00 0000 2905 7215 0000  .d.S.r....).r...
-00000980: 00da 065f 5f67 745f 5f72 1b00 0000 7217  ...__gt__r....r.
-00000990: 0000 00da 0573 7570 6572 a902 7219 0000  .....super..r...
+00000980: 00da 065f 5f67 745f 5f72 1a00 0000 7217  ...__gt__r....r.
+00000990: 0000 00da 0573 7570 6572 a902 7218 0000  .....super..r...
 000009a0: 005a 0363 6d70 a901 da09 5f5f 636c 6173  .Z.cmp....__clas
-000009b0: 735f 5f72 0b00 0000 720c 0000 0072 2a00  s__r....r....r*.
-000009c0: 0000 4900 0000 7308 0000 0000 0102 0116  ..I...s.........
+000009b0: 735f 5f72 0b00 0000 720c 0000 0072 2900  s__r....r....r).
+000009c0: 0000 6300 0000 7308 0000 0000 0102 0116  ..c...s.........
 000009d0: 010e 017a 0f56 6572 7369 6f6e 5f2e 5f5f  ...z.Version_.__
 000009e0: 6774 5f5f 6302 0000 0000 0000 0000 0000  gt__c...........
 000009f0: 0002 0000 0008 0000 0003 0000 0073 3c00  .............s<.
 00000a00: 0000 7a16 7400 7c00 8301 a001 7c00 a002  ..z.t.|.....|...
 00000a10: 7c01 a101 a101 5700 5300 0400 7403 6b0a  |.....W.S...t.k.
 00000a20: 7236 0100 0100 0100 7404 8300 a001 7c01  r6......t.....|.
 00000a30: a101 0600 5900 5300 5800 6400 5300 720f  ....Y.S.X.d.S.r.
 00000a40: 0000 0029 0572 1500 0000 da06 5f5f 6c74  ...).r......__lt
-00000a50: 5f5f 721b 0000 0072 1700 0000 722b 0000  __r....r....r+..
-00000a60: 0072 2c00 0000 722d 0000 0072 0b00 0000  .r,...r-...r....
-00000a70: 720c 0000 0072 2f00 0000 4f00 0000 7308  r....r/...O...s.
+00000a50: 5f5f 721a 0000 0072 1700 0000 722a 0000  __r....r....r*..
+00000a60: 0072 2b00 0000 722c 0000 0072 0b00 0000  .r+...r,...r....
+00000a70: 720c 0000 0072 2e00 0000 6900 0000 7308  r....r....i...s.
 00000a80: 0000 0000 0102 0116 010e 017a 0f56 6572  ...........z.Ver
 00000a90: 7369 6f6e 5f2e 5f5f 6c74 5f5f 6302 0000  sion_.__lt__c...
 00000aa0: 0000 0000 0000 0000 0002 0000 0008 0000  ................
 00000ab0: 0003 0000 0073 3c00 0000 7a16 7400 7c00  .....s<...z.t.|.
 00000ac0: 8301 a001 7c00 a002 7c01 a101 a101 5700  ....|...|.....W.
 00000ad0: 5300 0400 7403 6b0a 7236 0100 0100 0100  S...t.k.r6......
 00000ae0: 7404 8300 a001 7c01 a101 0600 5900 5300  t.....|.....Y.S.
 00000af0: 5800 6400 5300 720f 0000 0029 0572 1500  X.d.S.r....).r..
-00000b00: 0000 da06 5f5f 6571 5f5f 721b 0000 0072  ....__eq__r....r
-00000b10: 1700 0000 722b 0000 0072 2c00 0000 722d  ....r+...r,...r-
-00000b20: 0000 0072 0b00 0000 720c 0000 0072 3000  ...r....r....r0.
-00000b30: 0000 5500 0000 7308 0000 0000 0102 0116  ..U...s.........
+00000b00: 0000 da06 5f5f 6571 5f5f 721a 0000 0072  ....__eq__r....r
+00000b10: 1700 0000 722a 0000 0072 2b00 0000 722c  ....r*...r+...r,
+00000b20: 0000 0072 0b00 0000 720c 0000 0072 2f00  ...r....r....r/.
+00000b30: 0000 6f00 0000 7308 0000 0000 0102 0116  ..o...s.........
 00000b40: 010e 017a 0f56 6572 7369 6f6e 5f2e 5f5f  ...z.Version_.__
 00000b50: 6571 5f5f 6302 0000 0000 0000 0000 0000  eq__c...........
 00000b60: 0002 0000 0008 0000 0003 0000 0073 3c00  .............s<.
 00000b70: 0000 7a16 7400 7c00 8301 a001 7c00 a002  ..z.t.|.....|...
 00000b80: 7c01 a101 a101 5700 5300 0400 7403 6b0a  |.....W.S...t.k.
 00000b90: 7236 0100 0100 0100 7404 8300 a001 7c01  r6......t.....|.
 00000ba0: a101 0600 5900 5300 5800 6400 5300 720f  ....Y.S.X.d.S.r.
 00000bb0: 0000 0029 0572 1500 0000 da06 5f5f 6765  ...).r......__ge
-00000bc0: 5f5f 721b 0000 0072 1700 0000 722b 0000  __r....r....r+..
-00000bd0: 0072 2c00 0000 722d 0000 0072 0b00 0000  .r,...r-...r....
-00000be0: 720c 0000 0072 3100 0000 5b00 0000 7308  r....r1...[...s.
+00000bc0: 5f5f 721a 0000 0072 1700 0000 722a 0000  __r....r....r*..
+00000bd0: 0072 2b00 0000 722c 0000 0072 0b00 0000  .r+...r,...r....
+00000be0: 720c 0000 0072 3000 0000 7500 0000 7308  r....r0...u...s.
 00000bf0: 0000 0000 0102 0116 010e 017a 0f56 6572  ...........z.Ver
 00000c00: 7369 6f6e 5f2e 5f5f 6765 5f5f 6302 0000  sion_.__ge__c...
 00000c10: 0000 0000 0000 0000 0002 0000 0008 0000  ................
 00000c20: 0003 0000 0073 3c00 0000 7a16 7400 7c00  .....s<...z.t.|.
 00000c30: 8301 a001 7c00 a002 7c01 a101 a101 5700  ....|...|.....W.
 00000c40: 5300 0400 7403 6b0a 7236 0100 0100 0100  S...t.k.r6......
 00000c50: 7404 8300 a001 7c01 a101 0600 5900 5300  t.....|.....Y.S.
 00000c60: 5800 6400 5300 720f 0000 0029 0572 1500  X.d.S.r....).r..
-00000c70: 0000 da06 5f5f 6c65 5f5f 721b 0000 0072  ....__le__r....r
-00000c80: 1700 0000 722b 0000 0072 2c00 0000 722d  ....r+...r,...r-
-00000c90: 0000 0072 0b00 0000 720c 0000 0072 3200  ...r....r....r2.
-00000ca0: 0000 6100 0000 7308 0000 0000 0102 0116  ..a...s.........
+00000c70: 0000 da06 5f5f 6c65 5f5f 721a 0000 0072  ....__le__r....r
+00000c80: 1700 0000 722a 0000 0072 2b00 0000 722c  ....r*...r+...r,
+00000c90: 0000 0072 0b00 0000 720c 0000 0072 3100  ...r....r....r1.
+00000ca0: 0000 7b00 0000 7308 0000 0000 0102 0116  ..{...s.........
 00000cb0: 010e 017a 0f56 6572 7369 6f6e 5f2e 5f5f  ...z.Version_.__
 00000cc0: 6c65 5f5f 2910 7207 0000 0072 0800 0000  le__).r....r....
-00000cd0: 7209 0000 0072 0a00 0000 721b 0000 00da  r....r....r.....
-00000ce0: 0870 726f 7065 7274 7972 2300 0000 7225  .propertyr#...r%
-00000cf0: 0000 0072 2800 0000 7229 0000 0072 2a00  ...r(...r)...r*.
-00000d00: 0000 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
-00000d10: 0072 3200 0000 da0d 5f5f 636c 6173 7363  .r2.....__classc
+00000cd0: 7209 0000 0072 0a00 0000 721a 0000 00da  r....r....r.....
+00000ce0: 0870 726f 7065 7274 7972 2200 0000 7224  .propertyr"...r$
+00000cf0: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
+00000d00: 0000 722e 0000 0072 2f00 0000 7230 0000  ..r....r/...r0..
+00000d10: 0072 3100 0000 da0d 5f5f 636c 6173 7363  .r1.....__classc
 00000d20: 656c 6c5f 5f72 0b00 0000 720b 0000 0072  ell__r....r....r
-00000d30: 2d00 0000 720c 0000 0072 0d00 0000 2700  -...r....r....'.
+00000d30: 2c00 0000 720c 0000 0072 0d00 0000 4100  ,...r....r....A.
 00000d40: 0000 731e 0000 0008 0104 0408 0a02 010a  ..s.............
 00000d50: 0502 010a 0302 010a 0302 010a 040c 060c  ................
 00000d60: 060c 060c 0672 0d00 0000 6302 0000 0000  .....r....c.....
 00000d70: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
 00000d80: 0000 0073 0e00 0000 7400 6a01 a002 7c00  ...s....t.j...|.
 00000d90: 7c01 a102 5300 720f 0000 0029 03da 026f  |...S.r....)...o
 00000da0: 73da 0765 6e76 6972 6f6e da03 6765 7429  s..environ..get)
 00000db0: 02da 0376 6172 da07 6465 6661 756c 7472  ...var..defaultr
 00000dc0: 0b00 0000 720b 0000 0072 0c00 0000 da07  ....r....r......
-00000dd0: 6765 745f 656e 7668 0000 0073 0200 0000  get_envh...s....
-00000de0: 0001 723a 0000 0063 0000 0000 0000 0000  ..r:...c........
-00000df0: 0000 0000 0000 0000 0900 0000 4000 0000  ............@...
-00000e00: 735e 0000 0065 005a 0164 005a 0264 015a  s^...e.Z.d.Z.d.Z
+00000dd0: 6765 745f 656e 7682 0000 0073 0200 0000  get_env....s....
+00000de0: 0001 7239 0000 0063 0000 0000 0000 0000  ..r9...c........
+00000df0: 0000 0000 0000 0000 0b00 0000 4000 0000  ............@...
+00000e00: 73bc 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
 00000e10: 0364 0264 0364 0464 0564 0664 0764 0864  .d.d.d.d.d.d.d.d
-00000e20: 099c 0764 0a64 0364 0464 0564 0664 0b64  ...d.d.d.d.d.d.d
-00000e30: 0c64 099c 0764 0d9c 025a 0465 0464 0e19  .d...d...Z.e.d..
-00000e40: 0065 0464 0f3c 0064 1064 1184 005a 0564  .e.d.<.d.d...Z.d
-00000e50: 1264 1384 005a 0664 1464 1584 005a 0764  .d...Z.d.d...Z.d
-00000e60: 1653 0029 17da 0e52 6564 6973 4149 5665  .S.)...RedisAIVe
-00000e70: 7273 696f 6e61 9501 0000 4120 7375 6263  rsiona....A subc
-00000e80: 6c61 7373 206f 6620 5665 7273 696f 6e5f  lass of Version_
-00000e90: 2074 6861 7420 686f 6c64 7320 7468 6520   that holds the 
-00000ea0: 6465 7065 6e64 656e 6379 2073 6574 7320  dependency sets 
-00000eb0: 666f 7220 5265 6469 7341 490a 0a20 2020  for RedisAI..   
-00000ec0: 2074 6869 7320 636c 6173 7320 7365 7276   this class serv
-00000ed0: 6573 2074 776f 2070 7572 706f 7365 733a  es two purposes:
-00000ee0: 0a0a 2020 2020 312e 2049 7420 6973 2075  ..    1. It is u
-00000ef0: 7365 6420 746f 2070 6f70 756c 6174 6520  sed to populate 
-00000f00: 7468 6520 5b6d 6c5d 2060 6065 7874 7261  the [ml] ``extra
-00000f10: 735f 7265 7175 6972 6560 6020 6f66 2074  s_require`` of t
-00000f20: 6865 2073 6574 7570 2e70 792e 0a20 2020  he setup.py..   
-00000f30: 2054 6869 7320 6973 2062 6563 6175 7365   This is because
-00000f40: 2074 6865 2052 6564 6973 4149 2076 6572   the RedisAI ver
-00000f50: 7369 6f6e 2077 696c 6c20 6465 7465 726d  sion will determ
-00000f60: 696e 6520 7768 6963 6820 4d4c 2062 6173  ine which ML bas
-00000f70: 6564 0a20 2020 2064 6570 656e 6465 6e63  ed.    dependenc
-00000f80: 6965 7320 6172 6520 7265 7175 6972 6564  ies are required
-00000f90: 2e0a 0a20 2020 2032 2e20 5573 6564 2074  ...    2. Used t
-00000fa0: 6f20 7365 7420 7468 6520 6465 6661 756c  o set the defaul
-00000fb0: 7420 7661 6c75 6573 2066 6f72 2050 7954  t values for PyT
-00000fc0: 6f72 6368 2c20 5446 2c20 616e 6420 4f4e  orch, TF, and ON
-00000fd0: 4e58 0a20 2020 2067 6976 656e 2074 6865  NX.    given the
-00000fe0: 2053 4d41 5254 5349 4d5f 5245 4449 5341   SMARTSIM_REDISA
-00000ff0: 4920 656e 7620 7661 7220 7365 7420 6279  I env var set by
-00001000: 2074 6865 2075 7365 722e 0a20 2020 207a   the user..    z
-00001010: 0532 2e35 2e32 7a05 312e 392e 307a 0631  .2.5.2z.1.9.0z.1
-00001020: 2e31 302e 337a 0631 2e31 302e 307a 0531  .10.3z.1.10.0z.1
-00001030: 2e30 2e32 7a05 312e 372e 317a 0530 2e38  .0.2z.1.7.1z.0.8
-00001040: 2e32 2907 da0a 7465 6e73 6f72 666c 6f77  .2)...tensorflow
-00001050: da04 6f6e 6e78 5a08 736b 6c32 6f6e 6e78  ..onnxZ.skl2onnx
-00001060: 5a0b 6f6e 6e78 6d6c 746f 6f6c 737a 0c73  Z.onnxmltoolsz.s
-00001070: 6369 6b69 742d 6c65 6172 6eda 0574 6f72  cikit-learn..tor
-00001080: 6368 da0b 746f 7263 6876 6973 696f 6e7a  ch..torchvisionz
-00001090: 0532 2e36 2e32 7a05 312e 392e 317a 0630  .2.6.2z.1.9.1z.0
-000010a0: 2e31 302e 3129 02fa 0531 2e32 2e33 fa05  .10.1)...1.2.3..
-000010b0: 312e 322e 3572 4000 0000 7a05 312e 322e  1.2.5r@...z.1.2.
-000010c0: 3463 0200 0000 0000 0000 0000 0000 0200  4c..............
-000010d0: 0000 0600 0000 4300 0000 7342 0000 007c  ......C...sB...|
-000010e0: 017c 006a 006b 0772 387c 01a0 0164 01a1  .|.j.k.r8|...d..
-000010f0: 0172 1c64 027c 005f 0271 3e74 0364 037c  .r.d.|._.q>t.d.|
-00001100: 019b 0064 047c 006a 00a0 04a1 009b 009d  ...d.|.j........
-00001110: 0483 0182 016e 067c 017c 005f 0264 0053  .....n.|.|._.d.S
-00001120: 0029 054e 7a03 312e 3272 4100 0000 7a18  .).Nz.1.2rA...z.
-00001130: 496e 7661 6c69 6420 5265 6469 7341 4920  Invalid RedisAI 
-00001140: 7665 7273 696f 6e20 7a0e 2e20 4f70 7469  version z.. Opti
-00001150: 6f6e 7320 6172 6520 2905 da08 6465 6661  ons are )...defa
-00001160: 756c 7473 da0a 7374 6172 7473 7769 7468  ults..startswith
-00001170: da07 7665 7273 696f 6e72 0600 0000 da04  ..versionr......
-00001180: 6b65 7973 7218 0000 0072 0b00 0000 720b  keysr....r....r.
-00001190: 0000 0072 0c00 0000 da08 5f5f 696e 6974  ...r......__init
-000011a0: 5f5f 9000 0000 730e 0000 0000 010a 010a  __....s.........
-000011b0: 0308 0202 0114 ff06 047a 1752 6564 6973  .........z.Redis
-000011c0: 4149 5665 7273 696f 6e2e 5f5f 696e 6974  AIVersion.__init
-000011d0: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
-000011e0: 0000 0002 0000 0043 0000 0073 1000 0000  .......C...s....
-000011f0: 7c00 6a00 7c00 6a01 1900 7c01 1900 5300  |.j.|.j...|...S.
-00001200: 720f 0000 00a9 0272 4200 0000 7244 0000  r......rB...rD..
-00001210: 0029 0272 1900 0000 da04 6e61 6d65 720b  .).r......namer.
-00001220: 0000 0072 0b00 0000 720c 0000 00da 0b5f  ...r....r......_
-00001230: 5f67 6574 6174 7472 5f5f 9d00 0000 7302  _getattr__....s.
-00001240: 0000 0000 017a 1a52 6564 6973 4149 5665  .....z.RedisAIVe
-00001250: 7273 696f 6e2e 5f5f 6765 7461 7474 725f  rsion.__getattr_
-00001260: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-00001270: 0000 0200 0000 4300 0000 730c 0000 007c  ......C...s....|
-00001280: 006a 007c 006a 0119 0053 0072 0f00 0000  .j.|.j...S.r....
-00001290: 7247 0000 0072 2200 0000 720b 0000 0072  rG...r"...r....r
-000012a0: 0b00 0000 720c 0000 00da 0c67 6574 5f64  ....r......get_d
-000012b0: 6566 6175 6c74 73a0 0000 0073 0200 0000  efaults....s....
-000012c0: 0001 7a1b 5265 6469 7341 4956 6572 7369  ..z.RedisAIVersi
-000012d0: 6f6e 2e67 6574 5f64 6566 6175 6c74 734e  on.get_defaultsN
-000012e0: 2908 7207 0000 0072 0800 0000 7209 0000  ).r....r....r...
-000012f0: 0072 0a00 0000 7242 0000 0072 4600 0000  .r....rB...rF...
-00001300: 7249 0000 0072 4a00 0000 720b 0000 0072  rI...rJ...r....r
-00001310: 0b00 0000 720b 0000 0072 0c00 0000 723b  ....r....r....r;
-00001320: 0000 006c 0000 0073 2c00 0000 0801 040e  ...l...s,.......
-00001330: 0201 0201 0201 0201 0201 0201 02f9 040a  ................
-00001340: 0201 0201 0201 0201 0201 0201 02f9 04f6  ................
-00001350: 0615 0c02 080d 0803 723b 0000 0063 0000  ........r;...c..
-00001360: 0000 0000 0000 0000 0000 0000 0000 0400  ................
-00001370: 0000 4000 0000 73e4 0000 0065 005a 0164  ..@...s....e.Z.d
-00001380: 005a 0264 015a 0365 0464 0283 015a 0565  .Z.d.Z.e.d...Z.e
-00001390: 0465 0664 0364 0483 0283 015a 0765 0465  .e.d.d.....Z.e.e
-000013a0: 0664 0564 0683 0283 015a 0865 0664 0764  .d.d.....Z.e.d.d
-000013b0: 0883 025a 0965 0465 0664 0964 0a83 0283  ...Z.e.e.d.d....
-000013c0: 015a 0a65 0664 0b64 0c83 025a 0b65 0664  .Z.e.d.d...Z.e.d
-000013d0: 0d65 0a83 025a 0c65 0d65 0664 0e64 0f83  .e...Z.e.e.d.d..
-000013e0: 0283 015a 0e65 0664 1064 1183 025a 0f65  ...Z.e.d.d...Z.e
-000013f0: 0664 1264 1365 0e9b 009d 0283 025a 1065  .d.d.e.......Z.e
-00001400: 0465 0664 1465 0e6a 1183 0283 015a 1265  .e.d.e.j.....Z.e
-00001410: 0465 0664 1565 0e6a 1383 0283 015a 1465  .e.d.e.j.....Z.e
-00001420: 0465 0e6a 1583 015a 1665 0465 0e6a 1783  .e.j...Z.e.e.j..
-00001430: 015a 1864 2164 1764 1884 015a 1964 1964  .Z.d!d.d...Z.d.d
-00001440: 1a84 005a 1a65 1b64 1b9c 0164 1c64 1d84  ...Z.e.d...d.d..
-00001450: 045a 1c64 1e64 1f84 005a 1d64 2053 0029  .Z.d.d...Z.d S.)
-00001460: 22da 0956 6572 7369 6f6e 6572 61a6 0200  "..Versionera...
-00001470: 0056 6572 7369 6f6e 6572 2069 7320 7265  .Versioner is re
-00001480: 7370 6f6e 7369 626c 6520 666f 206d 616e  sponsible fo man
-00001490: 6167 696e 6720 616c 6c20 7468 6520 7665  aging all the ve
-000014a0: 7273 696f 6e73 0a20 2020 2077 6974 6869  rsions.    withi
-000014b0: 6e20 536d 6172 7453 696d 2069 6e63 6c75  n SmartSim inclu
-000014c0: 6469 6e67 2053 6d61 7274 5369 6d20 6974  ding SmartSim it
-000014d0: 7365 6c66 2e0a 0a20 2020 2053 6d61 7274  self...    Smart
-000014e0: 5369 6d27 7320 7665 7273 696f 6e20 6973  Sim's version is
-000014f0: 2077 7269 7474 656e 2069 6e74 6f20 7665   written into ve
-00001500: 7273 696f 6e2e 7079 2075 706f 6e20 7069  rsion.py upon pi
-00001510: 7020 696e 7374 616c 6c0a 2020 2020 6279  p install.    by
-00001520: 2075 7369 6e67 2074 6869 7320 636c 6173   using this clas
-00001530: 7320 696e 2073 6574 7570 2e70 792e 2042  s in setup.py. B
-00001540: 7920 7365 7474 696e 6720 534d 4152 5453  y setting SMARTS
-00001550: 494d 5f53 5546 4649 582c 0a20 2020 2074  IM_SUFFIX,.    t
-00001560: 6865 2076 6572 7369 6f6e 2077 696c 6c20  he version will 
-00001570: 6265 2077 7269 7474 656e 2061 7320 6120  be written as a 
-00001580: 2264 6972 7479 2220 7665 7273 696f 6e20  "dirty" version 
-00001590: 7769 7468 2074 6865 0a20 2020 2067 6974  with the.    git
-000015a0: 2d73 6861 2061 7070 656e 6465 642e 0a20  -sha appended.. 
-000015b0: 2020 2069 2e65 2e0a 2020 2020 2020 2020     i.e..        
-000015c0: 6578 706f 7274 2053 4d41 5254 5349 4d5f  export SMARTSIM_
-000015d0: 5355 4646 4958 3d6e 6967 6874 6c79 0a20  SUFFIX=nightly. 
-000015e0: 2020 2020 2020 2070 6970 2069 6e73 7461         pip insta
-000015f0: 6c6c 202d 6520 2e0a 2020 2020 2020 2020  ll -e ..        
-00001600: 736d 6172 7473 696d 2e5f 5f76 6572 7369  smartsim.__versi
-00001610: 6f6e 5f5f 203d 3d20 302e 332e 322b 6e69  on__ == 0.3.2+ni
-00001620: 6768 746c 792d 3366 6532 3366 660a 0a20  ghtly-3fe23ff.. 
-00001630: 2020 2056 6572 7369 6f6e 6572 206d 616e     Versioner man
-00001640: 6167 6573 2074 6869 7264 2070 6172 7479  ages third party
-00001650: 2064 6570 656e 6465 6e63 6965 7320 616e   dependencies an
-00001660: 6420 7468 6569 7220 7665 7273 696f 6e73  d their versions
-00001670: 0a20 2020 2061 7320 7765 6c6c 2e20 5468  .    as well. Th
-00001680: 6573 6520 7665 7273 696f 6e73 2061 7265  ese versions are
-00001690: 2075 7365 6420 6279 2074 6865 2060 6073   used by the ``s
-000016a0: 6d61 7274 6060 2063 6c69 2069 6e20 7468  mart`` cli in th
-000016b0: 650a 2020 2020 6060 736d 6172 7420 6275  e.    ``smart bu
-000016c0: 696c 6460 6020 636f 6d6d 616e 6420 746f  ild`` command to
-000016d0: 2064 6574 6572 6d69 6e65 2077 6869 6368   determine which
-000016e0: 2064 6570 656e 6465 6e63 7920 7665 7273   dependency vers
-000016f0: 696f 6e73 0a20 2020 2074 6f20 6c6f 6f6b  ions.    to look
-00001700: 2066 6f72 2061 6e64 2064 6f77 6e6c 6f61   for and downloa
-00001710: 642e 0a20 2020 207a 0533 2e37 2e30 5a10  d..    z.3.7.0Z.
-00001720: 534d 4152 5453 494d 5f56 4552 5349 4f4e  SMARTSIM_VERSION
-00001730: 7a05 302e 342e 315a 1253 4d41 5254 5245  z.0.4.1Z.SMARTRE
-00001740: 4449 535f 5645 5253 494f 4e7a 0530 2e33  DIS_VERSIONz.0.3
-00001750: 2e31 da0f 534d 4152 5453 494d 5f53 5546  .1..SMARTSIM_SUF
-00001760: 4649 58da 005a 0e53 4d41 5254 5349 4d5f  FIX..Z.SMARTSIM_
-00001770: 5245 4449 537a 0536 2e30 2e38 5a12 534d  REDISz.6.0.8Z.SM
-00001780: 4152 5453 494d 5f52 4544 4953 5f55 524c  ARTSIM_REDIS_URL
-00001790: 7a23 6874 7470 733a 2f2f 6769 7468 7562  z#https://github
-000017a0: 2e63 6f6d 2f72 6564 6973 2f72 6564 6973  .com/redis/redis
-000017b0: 2e67 6974 2f5a 1553 4d41 5254 5349 4d5f  .git/Z.SMARTSIM_
-000017c0: 5245 4449 535f 4252 414e 4348 5a10 534d  REDIS_BRANCHZ.SM
-000017d0: 4152 5453 494d 5f52 4544 4953 4149 7240  ARTSIM_REDISAIr@
-000017e0: 0000 005a 1453 4d41 5254 5349 4d5f 5245  ...Z.SMARTSIM_RE
-000017f0: 4449 5341 495f 5552 4c7a 2768 7474 7073  DISAI_URLz'https
-00001800: 3a2f 2f67 6974 6875 622e 636f 6d2f 5265  ://github.com/Re
-00001810: 6469 7341 492f 5265 6469 7341 492e 6769  disAI/RedisAI.gi
-00001820: 742f 5a17 534d 4152 5453 494d 5f52 4544  t/Z.SMARTSIM_RED
-00001830: 4953 4149 5f42 5241 4e43 48da 0176 5a0e  ISAI_BRANCH..vZ.
-00001840: 534d 4152 5453 494d 5f54 4f52 4348 5a11  SMARTSIM_TORCHZ.
-00001850: 534d 4152 5453 494d 5f54 4f52 4348 5649  SMARTSIM_TORCHVI
-00001860: 53da 0552 4544 4953 6302 0000 0000 0000  S..REDISc.......
-00001870: 0000 0000 0005 0000 0007 0000 0043 0000  .............C..
-00001880: 0073 4000 0000 6401 6402 7c01 6403 6404  .s@...d.d.|.d.d.
-00001890: 6405 6406 6707 7d02 7c00 6a00 7c00 6a01  d.d.g.}.|.j.|.j.
-000018a0: 7c00 6a02 7c00 6a03 7c00 6a04 7c00 6a05  |.j.|.j.|.j.|.j.
-000018b0: 7c00 6a06 6707 7d03 7c02 7c03 6407 9c02  |.j.g.}.|.|.d...
-000018c0: 7d04 7c04 5300 2908 4eda 0853 4d41 5254  }.|.S.).N..SMART
-000018d0: 5349 4dda 0a53 4d41 5254 5245 4449 53da  SIM..SMARTREDIS.
-000018e0: 0752 4544 4953 4149 da05 544f 5243 48da  .REDISAI..TORCH.
-000018f0: 0a54 454e 534f 5246 4c4f 57da 044f 4e4e  .TENSORFLOW..ONN
-00001900: 5829 025a 0850 6163 6b61 6765 735a 0856  X).Z.PackagesZ.V
-00001910: 6572 7369 6f6e 7329 0772 5000 0000 7251  ersions).rP...rQ
-00001920: 0000 0072 4f00 0000 7252 0000 0072 5300  ...rO...rR...rS.
-00001930: 0000 7254 0000 0072 5500 0000 2905 7219  ..rT...rU...).r.
-00001940: 0000 005a 0764 625f 6e61 6d65 da08 7061  ...Z.db_name..pa
-00001950: 636b 6167 6573 da08 7665 7273 696f 6e73  ckages..versions
-00001960: 721a 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
-00001970: 0c00 0000 da07 6173 5f64 6963 74d5 0000  ......as_dict...
-00001980: 0073 2400 0000 0002 0201 0201 0201 0201  .s$.............
-00001990: 0201 0201 02f9 040a 0401 0401 0401 0401  ................
-000019a0: 0401 0401 04f9 0409 0a01 7a11 5665 7273  ..........z.Vers
-000019b0: 696f 6e65 722e 6173 5f64 6963 7463 0100  ioner.as_dictc..
-000019c0: 0000 0000 0000 0000 0000 0500 0000 0600  ................
-000019d0: 0000 4300 0000 7344 0000 0067 007d 017c  ..C...sD...g.}.|
-000019e0: 006a 00a0 01a1 007d 027c 0264 013d 007c  .j.....}.|.d.=.|
-000019f0: 0264 023d 007c 02a0 02a1 0044 005d 1c5c  .d.=.|.....D.].\
-00001a00: 027d 037d 047c 01a0 037c 039b 0064 037c  .}.}.|...|...d.|
-00001a10: 049b 009d 03a1 0101 0071 227c 0153 0029  .........q"|.S.)
-00001a20: 047a 744f 7074 696f 6e61 6c20 4d4c 2f44  .ztOptional ML/D
-00001a30: 4c20 6465 7065 6e64 656e 6369 6573 2077  L dependencies w
-00001a40: 6520 7375 6767 6573 7420 666f 7220 7468  e suggest for th
-00001a50: 6520 7573 6572 2e0a 0a20 2020 2020 2020  e user...       
-00001a60: 2054 6865 2064 6566 6175 6c74 7320 6172   The defaults ar
-00001a70: 6520 6261 7365 6420 6f6e 2074 6865 2052  e based on the R
-00001a80: 6564 6973 4149 2076 6572 7369 6f6e 0a20  edisAI version. 
-00001a90: 2020 2020 2020 2072 3e00 0000 723f 0000         r>...r?..
-00001aa0: 007a 023d 3d29 0472 5200 0000 724a 0000  .z.==).rR...rJ..
-00001ab0: 00da 0569 7465 6d73 da06 6170 7065 6e64  ...items..append
-00001ac0: 2905 7219 0000 005a 096d 6c5f 6578 7472  ).r....Z.ml_extr
-00001ad0: 6173 5a0b 6d6c 5f64 6566 6175 6c74 73da  asZ.ml_defaults.
-00001ae0: 036c 6962 721a 0000 0072 0b00 0000 720b  .libr....r....r.
-00001af0: 0000 0072 0c00 0000 da12 6d6c 5f65 7874  ...r......ml_ext
-00001b00: 7261 735f 7265 7175 6972 6564 eb00 0000  ras_required....
-00001b10: 730e 0000 0000 0504 010a 0606 0106 0210  s...............
-00001b20: 0116 017a 1c56 6572 7369 6f6e 6572 2e6d  ...z.Versioner.m
-00001b30: 6c5f 6578 7472 6173 5f72 6571 7569 7265  l_extras_require
-00001b40: 6429 01da 0672 6574 7572 6e63 0200 0000  d)...returnc....
-00001b50: 0000 0000 0000 0000 0300 0000 0800 0000  ................
-00001b60: 4300 0000 7348 0000 007a 2c74 006a 0164  C...sH...z,t.j.d
-00001b70: 0164 0264 0367 037c 0164 048d 02a0 0264  .d.d.g.|.d.....d
-00001b80: 05a1 01a0 03a1 007d 027c 0264 0664 0785  .......}.|.d.d..
-00001b90: 0219 0057 0053 0004 0074 046b 0a72 4201  ...W.S...t.k.rB.
-00001ba0: 0001 0001 0059 0064 0853 0058 0064 0653  .....Y.d.S.X.d.S
-00001bb0: 0029 097a 2547 6574 2074 6865 2067 6974  .).z%Get the git
-00001bc0: 2073 6861 206f 6620 7468 6520 6375 7272   sha of the curr
-00001bd0: 656e 7420 6272 616e 6368 da03 6769 747a  ent branch..gitz
-00001be0: 0972 6576 2d70 6172 7365 5a04 4845 4144  .rev-parseZ.HEAD
-00001bf0: 2901 da03 6377 64da 0561 7363 6969 4ee9  )...cwd..asciiN.
-00001c00: 0700 0000 724d 0000 0029 05da 0a73 7562  ....rM...)...sub
-00001c10: 7072 6f63 6573 73da 0c63 6865 636b 5f6f  process..check_o
-00001c20: 7574 7075 74da 0664 6563 6f64 65da 0573  utput..decode..s
-00001c30: 7472 6970 da09 4578 6365 7074 696f 6e29  trip..Exception)
-00001c40: 0372 1900 0000 da0c 7365 7475 705f 7079  .r......setup_py
-00001c50: 5f64 6972 5a03 7368 6172 0b00 0000 720b  _dirZ.shar....r.
-00001c60: 0000 0072 0c00 0000 da07 6765 745f 7368  ...r......get_sh
-00001c70: 61fe 0000 0073 1000 0000 0002 0202 1401  a....s..........
-00001c80: 02ff 06ff 0205 0e01 0e02 7a11 5665 7273  ..........z.Vers
-00001c90: 696f 6e65 722e 6765 745f 7368 6163 0200  ioner.get_shac..
-00001ca0: 0000 0000 0000 0000 0000 0600 0000 0900  ................
-00001cb0: 0000 4300 0000 738e 0000 007c 006a 007d  ..C...s....|.j.}
-00001cc0: 027c 006a 0172 427c 00a0 027c 01a1 017d  .|.j.rB|...|...}
-00001cd0: 037c 0372 327c 029b 0064 017c 006a 019b  .|.r2|...d.|.j..
-00001ce0: 0064 027c 039b 009d 057d 026e 107c 029b  .d.|.....}.n.|..
-00001cf0: 0064 017c 006a 019b 009d 037d 027c 0164  .d.|.j.....}.|.d
-00001d00: 031b 0064 041b 007d 0474 037c 0464 0583  ...d...}.t.|.d..
-00001d10: 028f 2c7d 057c 05a0 0464 06a1 0101 007c  ..,}.|...d.....|
-00001d20: 05a0 0464 07a1 0101 007c 05a0 0464 087c  ...d.....|...d.|
-00001d30: 029b 0064 099d 03a1 0101 0057 0035 0051  ...d.......W.5.Q
-00001d40: 0052 0058 007c 0253 0029 0a7a 830a 2020  .R.X.|.S.).z..  
-00001d50: 2020 2020 2020 5772 6974 6520 7665 7273        Write vers
-00001d60: 696f 6e20 696e 666f 2074 6f20 7665 7273  ion info to vers
-00001d70: 696f 6e2e 7079 0a0a 2020 2020 2020 2020  ion.py..        
-00001d80: 5573 6520 6769 745f 7368 6120 696e 2074  Use git_sha in t
-00001d90: 6865 2063 6173 6520 7768 6572 6520 736d  he case where sm
-00001da0: 6172 7473 696d 2073 7566 6669 7820 6973  artsim suffix is
-00001db0: 2073 6574 2069 6e20 7468 6520 656e 7669   set in the envi
-00001dc0: 726f 6e6d 656e 740a 2020 2020 2020 2020  ronment.        
-00001dd0: fa01 2b72 0e00 0000 da08 736d 6172 7473  ..+r......smarts
-00001de0: 696d 7a0a 7665 7273 696f 6e2e 7079 da01  imz.version.py..
-00001df0: 777a 3323 2054 6869 7320 6669 6c65 2069  wz3# This file i
-00001e00: 7320 6175 746f 6d61 7469 6361 6c6c 7920  s automatically 
-00001e10: 6765 6e65 7261 7465 6420 6279 2073 6574  generated by set
-00001e20: 7570 2e70 790a 7a23 2320 646f 206e 6f74  up.py.z## do not
-00001e30: 2065 6469 7420 7468 6973 2066 696c 6520   edit this file 
-00001e40: 6d61 6e75 616c 6c79 2e0a 0a7a 0f5f 5f76  manually...z.__v
-00001e50: 6572 7369 6f6e 5f5f 203d 2027 7a02 270a  ersion__ = 'z.'.
-00001e60: 2905 7250 0000 0072 4c00 0000 7268 0000  ).rP...rL...rh..
-00001e70: 00da 046f 7065 6eda 0577 7269 7465 2906  ...open..write).
-00001e80: 7219 0000 0072 6700 0000 7244 0000 005a  r....rg...rD...Z
-00001e90: 0767 6974 5f73 6861 5a0c 7665 7273 696f  .git_shaZ.versio
-00001ea0: 6e5f 6669 6c65 da01 6672 0b00 0000 720b  n_file..fr....r.
-00001eb0: 0000 0072 0c00 0000 da0d 7772 6974 655f  ...r......write_
-00001ec0: 7665 7273 696f 6e0b 0100 0073 1800 0000  version....s....
-00001ed0: 0006 0601 0601 0a01 0401 1803 1002 0c01  ................
-00001ee0: 0c01 0a01 0a02 1c01 7a17 5665 7273 696f  ........z.Versio
-00001ef0: 6e65 722e 7772 6974 655f 7665 7273 696f  ner.write_versio
-00001f00: 6e4e 2901 724f 0000 0029 1e72 0700 0000  nN).rO...).r....
-00001f10: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
-00001f20: 0d00 0000 da0a 5059 5448 4f4e 5f4d 494e  ......PYTHON_MIN
-00001f30: 723a 0000 0072 5000 0000 7251 0000 0072  r:...rP...rQ...r
-00001f40: 4c00 0000 724f 0000 00da 0952 4544 4953  L...rO.....REDIS
-00001f50: 5f55 524c 5a0c 5245 4449 535f 4252 414e  _URLZ.REDIS_BRAN
-00001f60: 4348 723b 0000 0072 5200 0000 5a0b 5245  CHr;...rR...Z.RE
-00001f70: 4449 5341 495f 5552 4c5a 0e52 4544 4953  DISAI_URLZ.REDIS
-00001f80: 4149 5f42 5241 4e43 4872 3e00 0000 7253  AI_BRANCHr>...rS
-00001f90: 0000 0072 3f00 0000 5a0b 544f 5243 4856  ...r?...Z.TORCHV
-00001fa0: 4953 494f 4e72 3c00 0000 7254 0000 0072  ISIONr<...rT...r
-00001fb0: 3d00 0000 7255 0000 0072 5800 0000 725c  =...rU...rX...r\
-00001fc0: 0000 0072 1000 0000 7268 0000 0072 6f00  ...r....rh...ro.
-00001fd0: 0000 720b 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00001fe0: 0072 0c00 0000 724b 0000 00a4 0000 0073  .r....rK.......s
-00001ff0: 2c00 0000 0801 0413 0803 0e01 0e01 0a03  ,...............
-00002000: 0e01 0a01 0a03 0e01 0201 0200 02ff 0403  ................
-00002010: 1004 1001 1004 0a01 0a02 0a16 0813 0e0d  ................
-00002020: 724b 0000 0063 0000 0000 0000 0000 0000  rK...c..........
-00002030: 0000 0000 0000 0500 0000 4000 0000 73f0  ..........@...s.
-00002040: 0000 0065 005a 0164 005a 0264 015a 0365  ...e.Z.d.Z.d.Z.e
-00002050: 046a 05a0 0664 0264 03a1 025a 0765 046a  .j...d.d...Z.e.j
-00002060: 05a0 0664 0464 05a1 025a 0865 046a 05a0  ...d.d...Z.e.j..
-00002070: 0664 0664 07a1 025a 0965 046a 05a0 0664  .d.d...Z.e.j...d
-00002080: 0864 07a1 025a 0a65 046a 05a0 0664 0964  .d...Z.e.j...d.d
-00002090: 0aa1 025a 0b65 046a 05a0 0664 0b64 0ca1  ...Z.e.j...d.d..
-000020a0: 025a 0c65 0d65 046a 05a0 0664 0d64 0ea1  .Z.e.e.j...d.d..
-000020b0: 0283 015a 0e65 0f6a 105a 1164 2964 1064  ...Z.e.j.Z.d)d.d
-000020c0: 1184 015a 1264 1264 1384 005a 1364 1464  ...Z.d.d...Z.d.d
-000020d0: 1584 005a 1464 1664 1784 005a 1565 1664  ...Z.d.d...Z.e.d
-000020e0: 1864 1984 0083 015a 1764 1a64 1b84 005a  .d.....Z.d.d...Z
-000020f0: 1864 1c64 1d84 005a 1964 1e64 1f84 005a  .d.d...Z.d.d...Z
-00002100: 1a65 1664 2064 2184 0083 015a 1b65 1c64  .e.d d!....Z.e.d
-00002110: 2264 2384 0083 015a 1d64 2464 2584 005a  "d#....Z.d$d%..Z
-00002120: 1e65 1c64 2a64 2764 2884 0183 015a 1f64  .e.d*d'd(....Z.d
-00002130: 2653 0029 2bda 0842 7569 6c64 456e 7661  &S.)+..BuildEnva
-00002140: 3702 0000 456e 7669 726f 6e6d 656e 7420  7...Environment 
-00002150: 666f 7220 6275 696c 6469 6e67 2074 6869  for building thi
-00002160: 7264 2d70 6172 7479 2064 6570 656e 6465  rd-party depende
-00002170: 6e63 6965 730a 0a20 2020 2042 7569 6c64  ncies..    Build
-00002180: 456e 7620 7072 6f76 6964 6573 2061 206d  Env provides a m
-00002190: 6574 686f 6420 666f 7220 636f 6e66 6967  ethod for config
-000021a0: 7572 696e 6720 686f 7720 7468 6520 7468  uring how the th
-000021b0: 6972 642d 7061 7274 790a 2020 2020 6465  ird-party.    de
-000021c0: 7065 6e64 656e 6369 6573 2077 6974 6869  pendencies withi
-000021d0: 6e20 536d 6172 7453 696d 2061 7265 2062  n SmartSim are b
-000021e0: 7569 6c74 2c20 6e61 6d65 6c79 2052 6564  uilt, namely Red
-000021f0: 6973 2f4b 6579 4442 0a20 2020 2061 6e64  is/KeyDB.    and
-00002200: 2052 6564 6973 4149 2e0a 0a20 2020 2054   RedisAI...    T
-00002210: 6865 2065 6e76 6972 6f6e 6d65 6e74 2076  he environment v
-00002220: 6172 6961 626c 6573 206c 6973 7465 6420  ariables listed 
-00002230: 6865 7265 2063 616e 2062 6520 7365 7420  here can be set 
-00002240: 746f 2063 6f6e 7472 6f6c 2074 6865 0a20  to control the. 
-00002250: 2020 2052 6564 6973 2062 7569 6c64 2069     Redis build i
-00002260: 6e20 7468 6520 7069 7020 7768 6565 6c20  n the pip wheel 
-00002270: 6275 696c 6420 6173 2077 656c 6c20 6173  build as well as
-00002280: 2074 6865 2052 6564 6973 2061 6e64 2052   the Redis and R
-00002290: 6564 6973 4149 0a20 2020 2062 7569 6c64  edisAI.    build
-000022a0: 2065 7865 6375 7465 6420 6279 2074 6865   executed by the
-000022b0: 2043 4c49 2e0a 0a20 2020 2042 7569 6c64   CLI...    Build
-000022c0: 2074 6f6f 6c73 2061 7265 2061 6c73 6f20   tools are also 
-000022d0: 6368 6563 6b65 6420 666f 7220 6865 7265  checked for here
-000022e0: 2061 6e64 2069 6620 7468 6579 2061 7265   and if they are
-000022f0: 206e 6f74 2066 6f75 6e64 0a20 2020 2074   not found.    t
-00002300: 6865 6e20 6120 5365 7475 7045 7272 6f72  hen a SetupError
-00002310: 2069 7320 7261 6973 6564 2e0a 0a20 2020   is raised...   
-00002320: 2041 6464 696e 6720 7468 6520 2d76 2066   Adding the -v f
-00002330: 6c61 6720 746f 2060 6073 6d61 7274 2062  lag to ``smart b
-00002340: 7569 6c64 6060 2077 696c 6c20 7368 6f77  uild`` will show
-00002350: 2074 6865 2062 7569 6c64 2065 6e76 6972   the build envir
-00002360: 6f6e 6d65 6e74 0a20 2020 2062 6569 6e67  onment.    being
-00002370: 2075 7365 642e 0a20 2020 20da 0243 435a   used..    ..CCZ
-00002380: 0367 6363 da03 4358 587a 0367 2b2b da06  .gcc..CXXz.g++..
-00002390: 4346 4c41 4753 724d 0000 00da 0843 5858  CFLAGSrM.....CXX
-000023a0: 464c 4147 53da 064d 414c 4c4f 43da 046c  FLAGS..MALLOC..l
-000023b0: 6962 635a 0a42 5549 4c44 5f4a 4f42 5372  ibcZ.BUILD_JOBSr
-000023c0: 2400 0000 5a09 4e4f 5f43 4845 434b 5372  $...Z.NO_CHECKSr
-000023d0: 0100 0000 5463 0200 0000 0000 0000 0000  ....Tc..........
-000023e0: 0000 0200 0000 0200 0000 4300 0000 7310  ..........C...s.
-000023f0: 0000 007c 0172 0c7c 00a0 00a1 0001 0064  ...|.r.|.......d
-00002400: 0053 0072 0f00 0000 2901 da12 6368 6563  .S.r....)...chec
-00002410: 6b5f 6465 7065 6e64 656e 6369 6573 2902  k_dependencies).
-00002420: 7219 0000 00da 0663 6865 636b 7372 0b00  r......checksr..
-00002430: 0000 720b 0000 0072 0c00 0000 7246 0000  ..r....r....rF..
-00002440: 0043 0100 0073 0400 0000 0001 0401 7a11  .C...s........z.
-00002450: 4275 696c 6445 6e76 2e5f 5f69 6e69 745f  BuildEnv.__init_
-00002460: 5f63 0100 0000 0000 0000 0000 0000 0300  _c..............
-00002470: 0000 0700 0000 4300 0000 733c 0000 0064  ......C...s<...d
-00002480: 0164 0264 0364 0464 057c 006a 007c 006a  .d.d.d.d.|.j.|.j
-00002490: 0167 077d 0174 027c 006a 0383 0164 066b  .g.}.t.|.j...d.k
-000024a0: 0272 387c 0144 005d 0e7d 027c 00a0 047c  .r8|.D.].}.|...|
-000024b0: 02a1 0101 0071 2864 0053 0029 074e 725e  .....q(d.S.).Nr^
-000024c0: 0000 007a 0767 6974 2d6c 6673 da04 6d61  ...z.git-lfs..ma
-000024d0: 6b65 5a04 7767 6574 5a05 636d 616b 6572  keZ.wgetZ.cmaker
-000024e0: 0100 0000 2905 7273 0000 0072 7400 0000  ....).rs...rt...
-000024f0: 721d 0000 00da 0643 4845 434b 53da 1663  r......CHECKS..c
-00002500: 6865 636b 5f62 7569 6c64 5f64 6570 656e  heck_build_depen
-00002510: 6465 6e63 7929 0372 1900 0000 da04 6465  dency).r......de
-00002520: 7073 da03 6465 7072 0b00 0000 720b 0000  ps..depr....r...
-00002530: 0072 0c00 0000 7279 0000 0047 0100 0073  .r....ry...G...s
-00002540: 0800 0000 0001 1601 0e01 0801 7a1b 4275  ............z.Bu
-00002550: 696c 6445 6e76 2e63 6865 636b 5f64 6570  ildEnv.check_dep
-00002560: 656e 6465 6e63 6965 7363 0100 0000 0000  endenciesc......
-00002570: 0000 0000 0000 0200 0000 0700 0000 4300  ..............C.
-00002580: 0000 732a 0000 0074 006a 01a0 02a1 007d  ..s*...t.j.....}
-00002590: 017c 01a0 037c 006a 047c 006a 057c 006a  .|...|.j.|.j.|.j
-000025a0: 067c 006a 0764 019c 04a1 0101 007c 0153  .|.j.d.......|.S
-000025b0: 0029 024e 2904 7273 0000 0072 7400 0000  .).N).rs...rt...
-000025c0: 7275 0000 0072 7600 0000 2908 7235 0000  ru...rv...).r5..
-000025d0: 0072 3600 0000 da04 636f 7079 da06 7570  .r6.....copy..up
-000025e0: 6461 7465 7273 0000 0072 7400 0000 7275  daters...rt...ru
-000025f0: 0000 0072 7600 0000 2902 7219 0000 00da  ...rv...).r.....
-00002600: 0365 6e76 720b 0000 0072 0b00 0000 720c  .envr....r....r.
-00002610: 0000 00da 085f 5f63 616c 6c5f 5f4d 0100  .....__call__M..
-00002620: 0073 1200 0000 0002 0a01 0402 0401 0401  .s..............
-00002630: 0401 04fc 04ff 0408 7a11 4275 696c 6445  ........z.BuildE
-00002640: 6e76 2e5f 5f63 616c 6c5f 5f63 0100 0000  nv.__call__c....
-00002650: 0000 0000 0000 0000 0400 0000 0800 0000  ................
-00002660: 4300 0000 7346 0000 0064 0164 0264 0364  C...sF...d.d.d.d
-00002670: 0464 0564 0664 0764 0867 087d 017c 006a  .d.d.d.d.g.}.|.j
-00002680: 007c 006a 017c 006a 027c 006a 037c 006a  .|.j.|.j.|.j.|.j
-00002690: 047c 006a 057c 006a 067c 006a 0767 087d  .|.j.|.j.|.j.g.}
-000026a0: 027c 017c 0264 099c 027d 037c 0353 0029  .|.|.d...}.|.S.)
-000026b0: 0a4e 7273 0000 0072 7400 0000 7275 0000  .Nrs...rt...ru..
-000026c0: 0072 7600 0000 7277 0000 00da 044a 4f42  .rv...rw.....JOB
-000026d0: 535a 0e50 5954 484f 4e5f 5645 5253 494f  SZ.PYTHON_VERSIO
-000026e0: 4eda 0850 4c41 5446 4f52 4d29 02da 0b45  N..PLATFORM)...E
-000026f0: 6e76 6972 6f6e 6d65 6e74 5a06 5661 6c75  nvironmentZ.Valu
-00002700: 6573 2908 7273 0000 0072 7400 0000 7275  es).rs...rt...ru
-00002710: 0000 0072 7600 0000 7277 0000 0072 8400  ...rv...rw...r..
-00002720: 0000 da0e 7079 7468 6f6e 5f76 6572 7369  ....python_versi
-00002730: 6f6e 7285 0000 0029 0472 1900 0000 da09  onr....).r......
-00002740: 7661 7269 6162 6c65 73da 0676 616c 7565  variables..value
-00002750: 7372 8200 0000 720b 0000 0072 0b00 0000  sr....r....r....
-00002760: 720c 0000 0072 5800 0000 5a01 0000 7328  r....rX...Z...s(
-00002770: 0000 0000 0202 0102 0102 0102 0102 0102  ................
-00002780: 0102 0102 f804 0b04 0104 0104 0104 0104  ................
-00002790: 0104 0104 0104 f804 0a0a 017a 1042 7569  ...........z.Bui
-000027a0: 6c64 456e 762e 6173 5f64 6963 7463 0100  ldEnv.as_dictc..
-000027b0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000027c0: 0000 4300 0000 7308 0000 0074 00a0 01a1  ..C...s....t....
-000027d0: 0053 0072 0f00 0000 2902 da08 706c 6174  .S.r....)...plat
-000027e0: 666f 726d 7287 0000 0072 2200 0000 720b  formr....r"...r.
-000027f0: 0000 0072 0b00 0000 720c 0000 0072 8700  ...r....r....r..
-00002800: 0000 7201 0000 7302 0000 0000 027a 1742  ..r...s......z.B
-00002810: 7569 6c64 456e 762e 7079 7468 6f6e 5f76  uildEnv.python_v
-00002820: 6572 7369 6f6e 6302 0000 0000 0000 0000  ersionc.........
-00002830: 0000 0004 0000 0006 0000 0043 0000 0073  ...........C...s
-00002840: 2c00 0000 7400 6a01 7d02 7402 7c02 6a03  ,...t.j.}.t.|.j.
-00002850: 9b00 6401 7c02 6a04 9b00 6401 7c02 6a05  ..d.|.j...d.|.j.
-00002860: 9b00 9d05 8301 7d03 7c03 7c01 6b04 5300  ......}.|.|.k.S.
-00002870: 2902 7a22 4465 7465 6374 2069 6620 7379  ).z"Detect if sy
-00002880: 7374 656d 2050 7974 686f 6e20 6973 2074  stem Python is t
-00002890: 6f6f 206f 6c64 720e 0000 0029 06da 0373  oo oldr....)...s
-000028a0: 7973 da0c 7665 7273 696f 6e5f 696e 666f  ys..version_info
-000028b0: 720d 0000 0072 2300 0000 7225 0000 0072  r....r#...r%...r
-000028c0: 2800 0000 2904 7219 0000 005a 0a70 7974  (...).r....Z.pyt
-000028d0: 686f 6e5f 6d69 6e5a 0673 7973 5f70 795a  hon_minZ.sys_pyZ
-000028e0: 0d73 7973 7465 6d5f 7079 7468 6f6e 720b  .system_pythonr.
-000028f0: 0000 0072 0b00 0000 720c 0000 00da 1469  ...r....r......i
-00002900: 735f 636f 6d70 6174 6962 6c65 5f70 7974  s_compatible_pyt
-00002910: 686f 6e76 0100 0073 0600 0000 0002 0601  honv...s........
-00002920: 1e01 7a1d 4275 696c 6445 6e76 2e69 735f  ..z.BuildEnv.is_
-00002930: 636f 6d70 6174 6962 6c65 5f70 7974 686f  compatible_pytho
-00002940: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
-00002950: 0000 0200 0000 4300 0000 730a 0000 007c  ......C...s....|
-00002960: 006a 0064 016b 0653 0029 024e 2903 da05  .j.d.k.S.).N)...
-00002970: 7769 6e33 32da 0663 7967 7769 6e5a 046d  win32..cygwinZ.m
-00002980: 7379 73a9 0172 8500 0000 7222 0000 0072  sys..r....r"...r
-00002990: 0b00 0000 720b 0000 0072 0c00 0000 da0a  ....r....r......
-000029a0: 6973 5f77 696e 646f 7773 7c01 0000 7302  is_windows|...s.
-000029b0: 0000 0000 017a 1342 7569 6c64 456e 762e  .....z.BuildEnv.
-000029c0: 6973 5f77 696e 646f 7773 6301 0000 0000  is_windowsc.....
-000029d0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-000029e0: 0000 0073 0a00 0000 7c00 6a00 6401 6b02  ...s....|.j.d.k.
-000029f0: 5300 2902 4eda 0664 6172 7769 6e72 9000  S.).N..darwinr..
-00002a00: 0000 7222 0000 0072 0b00 0000 720b 0000  ..r"...r....r...
-00002a10: 0072 0c00 0000 da08 6973 5f6d 6163 6f73  .r......is_macos
-00002a20: 7f01 0000 7302 0000 0000 017a 1142 7569  ....s......z.Bui
-00002a30: 6c64 456e 762e 6973 5f6d 6163 6f73 6301  ldEnv.is_macosc.
-00002a40: 0000 0000 0000 0000 0000 0004 0000 0002  ................
-00002a50: 0000 0043 0000 0073 3400 0000 6401 6402  ...C...s4...d.d.
-00002a60: 8400 7d01 6403 6404 8400 7d02 7c01 8300  ..}.d.d...}.|...
-00002a70: 7d03 7c03 7320 7c02 8300 7d03 7c03 732c  }.|.s |...}.|.s,
-00002a80: 7400 6405 8301 8201 7401 7c03 8301 5300  t.d.....t.|...S.
-00002a90: 2906 7a53 4669 6e64 2074 6865 2070 6174  ).zSFind the pat
-00002aa0: 6820 746f 2074 6865 2063 6d61 6b65 2064  h to the cmake d
-00002ab0: 6972 6563 746f 7279 2077 6974 6869 6e20  irectory within 
-00002ac0: 610a 2020 2020 2020 2020 7069 7020 696e  a.        pip in
-00002ad0: 7374 616c 6c65 6420 7079 746f 7263 6820  stalled pytorch 
-00002ae0: 7061 636b 6167 6563 0000 0000 0000 0000  packagec........
-00002af0: 0000 0000 0400 0000 0800 0000 5300 0000  ............S...
-00002b00: 735e 0000 007a 4264 0164 026c 007d 0064  s^...zBd.d.l.}.d
-00002b10: 0364 0484 007c 006a 0144 0083 017d 017c  .d...|.j.D...}.|
-00002b20: 0144 005d 1e7d 027c 0264 051b 007d 037c  .D.].}.|.d...}.|
-00002b30: 03a0 02a1 0072 1e7c 0302 0001 0057 0053  .....r.|.....W.S
-00002b40: 0071 1e57 0064 0253 0004 0074 036b 0a72  .q.W.d.S...t.k.r
-00002b50: 5801 0001 0001 0059 0064 0253 0058 0064  X......Y.d.S.X.d
-00002b60: 0253 0029 067a 1c46 696e 6420 7468 726f  .S.).z.Find thro
-00002b70: 7567 6820 696d 706f 7274 696e 6720 746f  ugh importing to
-00002b80: 7263 6872 0100 0000 4e63 0100 0000 0000  rchr....Nc......
-00002b90: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00002ba0: 0000 7314 0000 0067 007c 005d 0c7d 0174  ..s....g.|.].}.t
-00002bb0: 007c 0183 0191 0271 0453 0072 0b00 0000  .|.....q.S.r....
-00002bc0: 7202 0000 00a9 0272 1100 0000 da01 7072  r......r......pr
-00002bd0: 0b00 0000 720b 0000 0072 0c00 0000 da0a  ....r....r......
-00002be0: 3c6c 6973 7463 6f6d 703e 8c01 0000 7304  <listcomp>....s.
-00002bf0: 0000 0006 0002 007a 4942 7569 6c64 456e  .......zIBuildEn
-00002c00: 762e 746f 7263 685f 636d 616b 655f 7061  v.torch_cmake_pa
-00002c10: 7468 2e3c 6c6f 6361 6c73 3e2e 5f74 6f72  th.<locals>._tor
-00002c20: 6368 5f69 6d70 6f72 745f 7061 7468 2e3c  ch_import_path.<
-00002c30: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00002c40: 703e 7a11 7368 6172 652f 636d 616b 652f  p>z.share/cmake/
-00002c50: 546f 7263 6829 0472 3e00 0000 da08 5f5f  Torch).r>.....__
-00002c60: 7061 7468 5f5f da06 6973 5f64 6972 da13  path__..is_dir..
-00002c70: 4d6f 6475 6c65 4e6f 7446 6f75 6e64 4572  ModuleNotFoundEr
-00002c80: 726f 7229 04da 0174 5a0b 746f 7263 685f  ror)...tZ.torch_
-00002c90: 7061 7468 73da 055f 7061 7468 da0a 746f  paths.._path..to
-00002ca0: 7263 685f 7061 7468 720b 0000 0072 0b00  rch_pathr....r..
-00002cb0: 0000 720c 0000 00da 125f 746f 7263 685f  ..r......_torch_
-00002cc0: 696d 706f 7274 5f70 6174 6887 0100 0073  import_path....s
-00002cd0: 1400 0000 0002 0201 0802 1001 0801 0801  ................
-00002ce0: 0801 0c01 0601 0e01 7a35 4275 696c 6445  ........z5BuildE
-00002cf0: 6e76 2e74 6f72 6368 5f63 6d61 6b65 5f70  nv.torch_cmake_p
-00002d00: 6174 682e 3c6c 6f63 616c 733e 2e5f 746f  ath.<locals>._to
-00002d10: 7263 685f 696d 706f 7274 5f70 6174 6863  rch_import_pathc
-00002d20: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00002d30: 0400 0000 5300 0000 7356 0000 0064 0164  ....S...sV...d.d
-00002d40: 0284 0074 00a0 01a1 0044 0083 017d 0074  ...t.....D...}.t
-00002d50: 0274 006a 0383 01a0 04a1 0072 307c 00a0  .t.j.......r0|..
-00002d60: 0574 0274 006a 0383 01a1 0101 007c 0044  .t.t.j.......|.D
-00002d70: 005d 1c7d 017c 0164 031b 007d 027c 02a0  .].}.|.d...}.|..
-00002d80: 04a1 0072 347c 0202 0001 0053 0071 3464  ...r4|.....S.q4d
-00002d90: 0453 0029 057a 2066 696e 6420 746f 7263  .S.).z find torc
-00002da0: 6820 7468 726f 7567 6820 7369 7465 2070  h through site p
-00002db0: 6163 6b61 6765 7363 0100 0000 0000 0000  ackagesc........
-00002dc0: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00002dd0: 7314 0000 0067 007c 005d 0c7d 0174 007c  s....g.|.].}.t.|
-00002de0: 0183 0191 0271 0453 0072 0b00 0000 7202  .....q.S.r....r.
-00002df0: 0000 0072 9400 0000 720b 0000 0072 0b00  ...r....r....r..
-00002e00: 0000 720c 0000 0072 9600 0000 9701 0000  ..r....r........
-00002e10: 7304 0000 0006 0002 007a 4742 7569 6c64  s........zGBuild
-00002e20: 456e 762e 746f 7263 685f 636d 616b 655f  Env.torch_cmake_
-00002e30: 7061 7468 2e3c 6c6f 6361 6c73 3e2e 5f74  path.<locals>._t
-00002e40: 6f72 6368 5f73 6974 655f 7061 7468 2e3c  orch_site_path.<
-00002e50: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00002e60: 703e 7a17 746f 7263 682f 7368 6172 652f  p>z.torch/share/
-00002e70: 636d 616b 652f 546f 7263 684e 2906 da04  cmake/TorchN)...
-00002e80: 7369 7465 da0f 6765 7473 6974 6570 6163  site..getsitepac
-00002e90: 6b61 6765 7372 0300 0000 da09 5553 4552  kagesr......USER
-00002ea0: 5f53 4954 4572 9800 0000 725a 0000 0029  _SITEr....rZ...)
-00002eb0: 035a 0a73 6974 655f 7061 7468 7372 9b00  .Z.site_pathsr..
-00002ec0: 0000 729c 0000 0072 0b00 0000 720b 0000  ..r....r....r...
-00002ed0: 0072 0c00 0000 da10 5f74 6f72 6368 5f73  .r......_torch_s
-00002ee0: 6974 655f 7061 7468 9501 0000 7310 0000  ite_path....s...
-00002ef0: 0000 0212 030e 0110 0208 0108 0108 010a  ................
-00002f00: 017a 3342 7569 6c64 456e 762e 746f 7263  .z3BuildEnv.torc
-00002f10: 685f 636d 616b 655f 7061 7468 2e3c 6c6f  h_cmake_path.<lo
-00002f20: 6361 6c73 3e2e 5f74 6f72 6368 5f73 6974  cals>._torch_sit
-00002f30: 655f 7061 7468 7a21 436f 756c 6420 6e6f  e_pathz!Could no
-00002f40: 7420 6c6f 6361 7465 2074 6f72 6368 2063  t locate torch c
-00002f50: 6d61 6b65 2070 6174 6829 0272 0600 0000  make path).r....
-00002f60: 7210 0000 0029 0472 1900 0000 729d 0000  r....).r....r...
-00002f70: 0072 a100 0000 729c 0000 0072 0b00 0000  .r....r....r....
-00002f80: 720b 0000 0072 0c00 0000 da10 746f 7263  r....r......torc
-00002f90: 685f 636d 616b 655f 7061 7468 8201 0000  h_cmake_path....
-00002fa0: 7310 0000 0000 0508 0e08 0e06 0104 0106  s...............
-00002fb0: 0104 0108 017a 1942 7569 6c64 456e 762e  .....z.BuildEnv.
-00002fc0: 746f 7263 685f 636d 616b 655f 7061 7468  torch_cmake_path
-00002fd0: 6300 0000 0000 0000 0000 0000 0005 0000  c...............
-00002fe0: 0007 0000 0043 0000 0073 bc00 0000 7400  .....C...s....t.
-00002ff0: 6a01 a002 6401 6402 a102 7400 6a01 a002  j...d.d...t.j...
-00003000: 6403 6402 a102 7400 6a01 a002 6404 6402  d.d...t.j...d.d.
-00003010: a102 7400 6a01 a002 6405 6402 a102 6406  ..t.j...d.d...d.
-00003020: 9c04 7d00 6401 6403 6702 7d01 6405 6404  ..}.d.d.g.}.d.d.
-00003030: 6702 7d02 7403 6407 6408 8400 7c01 4400  g.}.t.d.d...|.D.
-00003040: 8301 8301 7d03 7403 6409 6408 8400 7c02  ....}.t.d.d...|.
-00003050: 4400 8301 8301 7d04 7c03 7376 7c04 7376  D.....}.|.sv|.sv
-00003060: 6402 5300 7c03 7298 7c04 7398 7c00 6403  d.S.|.r.|.s.|.d.
-00003070: 1900 7c00 6405 3c00 7c00 6401 1900 7c00  ..|.d.<.|.d...|.
-00003080: 6404 3c00 6e20 7c04 72b8 7c03 73b8 7c00  d.<.n |.r.|.s.|.
-00003090: 6405 1900 7c00 6403 3c00 7c00 6404 1900  d...|.d.<.|.d...
-000030a0: 7c00 6401 3c00 7c00 5300 290a 612f 0100  |.d.<.|.S.).a/..
-000030b0: 0043 6f6c 6c65 6374 2074 6865 2065 6e76  .Collect the env
-000030c0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-000030d0: 6573 206e 6565 6465 6420 666f 7220 4361  es needed for Ca
-000030e0: 6666 6520 2850 7974 6f72 6368 290a 2020  ffe (Pytorch).  
-000030f0: 2020 2020 2020 616e 6420 7468 726f 7720        and throw 
-00003100: 616e 2065 7272 6f72 2069 6620 7468 6579  an error if they
-00003110: 2061 7265 206e 6f74 2066 6f75 6e64 0a0a   are not found..
-00003120: 2020 2020 2020 2020 5370 6563 6966 6963          Specific
-00003130: 616c 6c79 206d 616b 6520 7375 7265 2074  ally make sure t
-00003140: 6f20 7365 7420 6174 206c 6561 7374 206f  o set at least o
-00003150: 6e65 2073 6574 206f 663a 0a20 2020 2020  ne set of:.     
-00003160: 2020 2020 2020 202d 2043 5544 4e4e 5f4c         - CUDNN_L
-00003170: 4942 5241 5259 2061 6e64 2043 5544 4e4e  IBRARY and CUDNN
-00003180: 5f49 4e43 4c55 4445 5f44 4952 0a20 2020  _INCLUDE_DIR.   
-00003190: 2020 2020 2020 2020 2020 2020 206f 720a               or.
-000031a0: 2020 2020 2020 2020 2020 2020 2d20 4355              - CU
-000031b0: 444e 4e5f 4c49 4252 4152 595f 5041 5448  DNN_LIBRARY_PATH
-000031c0: 2061 6e64 2043 5544 4e4e 5f49 4e43 4c55   and CUDNN_INCLU
-000031d0: 4445 5f50 4154 480a 2020 2020 2020 2020  DE_PATH.        
-000031e0: da0d 4355 444e 4e5f 4c49 4252 4152 594e  ..CUDNN_LIBRARYN
-000031f0: da11 4355 444e 4e5f 494e 434c 5544 455f  ..CUDNN_INCLUDE_
-00003200: 4449 52da 1243 5544 4e4e 5f4c 4942 5241  DIR..CUDNN_LIBRA
-00003210: 5259 5f50 4154 48da 1243 5544 4e4e 5f49  RY_PATH..CUDNN_I
-00003220: 4e43 4c55 4445 5f50 4154 4829 0472 a300  NCLUDE_PATH).r..
-00003230: 0000 72a4 0000 0072 a500 0000 72a6 0000  ..r....r....r...
-00003240: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00003250: 0000 0400 0000 5300 0000 7316 0000 0067  ......S...s....g
-00003260: 007c 005d 0e7d 017c 0174 006a 016b 0691  .|.].}.|.t.j.k..
-00003270: 0271 0453 0072 0b00 0000 a902 7235 0000  .q.S.r......r5..
-00003280: 0072 3600 0000 a902 7211 0000 0072 3800  .r6.....r....r8.
-00003290: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-000032a0: 0072 9600 0000 bd01 0000 7304 0000 0006  .r........s.....
-000032b0: 0002 007a 2a42 7569 6c64 456e 762e 6765  ...z*BuildEnv.ge
-000032c0: 745f 6375 646e 6e5f 656e 762e 3c6c 6f63  t_cudnn_env.<loc
-000032d0: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
-000032e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000032f0: 0400 0000 5300 0000 7316 0000 0067 007c  ....S...s....g.|
-00003300: 005d 0e7d 017c 0174 006a 016b 0691 0271  .].}.|.t.j.k...q
-00003310: 0453 0072 0b00 0000 72a7 0000 0072 a800  .S.r....r....r..
-00003320: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
-00003330: 0072 9600 0000 be01 0000 7304 0000 0006  .r........s.....
-00003340: 0002 0029 0472 3500 0000 7236 0000 0072  ...).r5...r6...r
-00003350: 3700 0000 da03 616c 6c29 0572 8200 0000  7.....all).r....
-00003360: 5a10 746f 7263 685f 6375 646e 6e5f 7661  Z.torch_cudnn_va
-00003370: 7273 5a10 6361 6666 655f 6375 646e 6e5f  rsZ.caffe_cudnn_
-00003380: 7661 7273 5a09 746f 7263 685f 7365 745a  varsZ.torch_setZ
-00003390: 0963 6166 6665 5f73 6574 720b 0000 0072  .caffe_setr....r
-000033a0: 0b00 0000 720c 0000 00da 0d67 6574 5f63  ....r......get_c
-000033b0: 7564 6e6e 5f65 6e76 aa01 0000 7324 0000  udnn_env....s$..
-000033c0: 0000 0b0c 010c 010c 010c fc06 0608 0108  ................
-000033d0: 0212 0112 0408 0104 0108 010c 010e 0108  ................
-000033e0: 010c 010c 017a 1642 7569 6c64 456e 762e  .....z.BuildEnv.
-000033f0: 6765 745f 6375 646e 6e5f 656e 7663 0200  get_cudnn_envc..
-00003400: 0000 0000 0000 0000 0000 0300 0000 0800  ................
-00003410: 0000 4300 0000 7346 0000 007a 1c74 006a  ..C...sF...z.t.j
-00003420: 017c 0164 0167 0274 006a 0274 006a 0264  .|.d.g.t.j.t.j.d
-00003430: 028d 037d 0257 006e 2404 0074 036b 0a72  ...}.W.n$..t.k.r
-00003440: 4001 0001 0001 0074 047c 019b 0064 039d  @......t.|...d..
-00003450: 0283 0164 0082 0259 006e 0258 0064 0053  ...d...Y.n.X.d.S
-00003460: 0029 044e 7a09 2d2d 7665 7273 696f 6e29  .).Nz.--version)
-00003470: 02da 0673 7464 6f75 74da 0673 7464 6572  ...stdout..stder
-00003480: 727a 2420 6d75 7374 2062 6520 696e 7374  rz$ must be inst
-00003490: 616c 6c65 6420 746f 2062 7569 6c64 2053  alled to build S
-000034a0: 6d61 7274 5369 6d29 0572 6200 0000 da0a  martSim).rb.....
-000034b0: 6368 6563 6b5f 6361 6c6c da07 4445 564e  check_call..DEVN
-000034c0: 554c 4cda 074f 5345 7272 6f72 7206 0000  ULL..OSErrorr...
-000034d0: 0029 0372 1900 0000 da07 636f 6d6d 616e  .).r......comman
-000034e0: 64da 036f 7574 720b 0000 0072 0b00 0000  d..outr....r....
-000034f0: 720c 0000 0072 7d00 0000 cc01 0000 7310  r....r}.......s.
-00003500: 0000 0000 0202 0104 0106 0104 0104 fd0a  ................
-00003510: 050e 017a 1f42 7569 6c64 456e 762e 6368  ...z.BuildEnv.ch
-00003520: 6563 6b5f 6275 696c 645f 6465 7065 6e64  eck_build_depend
-00003530: 656e 6379 4e63 0200 0000 0000 0000 0000  encyNc..........
-00003540: 0000 0400 0000 0900 0000 4300 0000 7380  ..........C...s.
-00003550: 0000 007a 6274 0074 01a0 027c 00a1 016a  ...zbt.t...|...j
-00003560: 0383 017d 027c 0172 5e7c 026a 047c 016a  ...}.|.r^|.j.|.j
-00003570: 046b 0373 2e7c 026a 057c 016a 056b 0372  .k.s.|.j.|.j.k.r
-00003580: 5e64 017c 009b 0064 029d 037c 009b 0064  ^d.|...d...|...d
-00003590: 037c 019b 0064 047c 009b 0064 037c 029b  .|...d.|...d.|..
-000035a0: 0064 059d 0817 007d 0374 067c 0383 0182  .d.....}.t.|....
-000035b0: 0157 0064 0653 0004 0074 016a 076b 0a72  .W.d.S...t.j.k.r
-000035c0: 7a01 0001 0001 0059 0064 0753 0058 0064  z......Y.d.S.X.d
-000035d0: 0853 0029 097a 7f43 6865 636b 2069 6620  .S.).z.Check if 
-000035e0: 6120 7061 636b 6167 6520 6973 2069 6e73  a package is ins
-000035f0: 7461 6c6c 6564 2e20 4966 2076 6572 7369  talled. If versi
-00003600: 6f6e 2069 7320 7072 6f76 6964 6564 2c20  on is provided, 
-00003610: 6368 6563 6b20 6966 0a20 2020 2020 2020  check if.       
-00003620: 2069 7427 7320 6120 636f 6d70 6174 6962   it's a compatib
-00003630: 6c65 2076 6572 7369 6f6e 2e20 286d 616a  le version. (maj
-00003640: 6f72 2061 6e64 206d 696e 6f72 2074 6865  or and minor the
-00003650: 2073 616d 6529 7a19 496e 636f 6d70 6174   same)z.Incompat
-00003660: 6962 6c65 2076 6572 7369 6f6e 2066 6f72  ible version for
-00003670: 207a 0b20 6465 7465 6374 6564 2e0a fa01   z. detected....
-00003680: 207a 0f20 7265 7175 6573 7465 6420 6275   z. requested bu
-00003690: 7420 7a0b 2069 6e73 7461 6c6c 6564 2e54  t z. installed.T
-000036a0: 464e 2908 720d 0000 0072 1e00 0000 da10  FN).r....r......
-000036b0: 6765 745f 6469 7374 7269 6275 7469 6f6e  get_distribution
-000036c0: 7244 0000 0072 2300 0000 7225 0000 0072  rD...r#...r%...r
-000036d0: 0600 0000 da14 4469 7374 7269 6275 7469  ......Distributi
-000036e0: 6f6e 4e6f 7446 6f75 6e64 2904 da07 7061  onNotFound)...pa
-000036f0: 636b 6167 6572 4400 0000 5a09 696e 7374  ckagerD...Z.inst
-00003700: 616c 6c65 64da 036d 7367 720b 0000 0072  alled..msgr....r
-00003710: 0b00 0000 720c 0000 00da 0f63 6865 636b  ....r......check
-00003720: 5f69 6e73 7461 6c6c 6564 d701 0000 7318  _installed....s.
-00003730: 0000 0000 0402 0110 0104 0218 020a 011a  ................
-00003740: ff02 ff02 0408 0106 0110 017a 1842 7569  ...........z.Bui
-00003750: 6c64 456e 762e 6368 6563 6b5f 696e 7374  ldEnv.check_inst
-00003760: 616c 6c65 6429 0154 2901 4e29 2072 0700  alled).T).N) r..
-00003770: 0000 7208 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00003780: 0072 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
-00003790: 7273 0000 0072 7400 0000 7275 0000 0072  rs...rt...ru...r
-000037a0: 7600 0000 7277 0000 0072 8400 0000 721d  v...rw...r....r.
-000037b0: 0000 0072 7c00 0000 728b 0000 0072 8a00  ...r|...r....r..
-000037c0: 0000 7285 0000 0072 4600 0000 7279 0000  ..r....rF...ry..
-000037d0: 0072 8300 0000 7258 0000 0072 3300 0000  .r....rX...r3...
-000037e0: 7287 0000 0072 8d00 0000 7291 0000 0072  r....r....r....r
-000037f0: 9300 0000 72a2 0000 00da 0c73 7461 7469  ....r......stati
-00003800: 636d 6574 686f 6472 aa00 0000 727d 0000  cmethodr....r}..
-00003810: 0072 b700 0000 720b 0000 0072 0b00 0000  .r....r....r....
-00003820: 720b 0000 0072 0c00 0000 7272 0000 0023  r....r....rr...#
-00003830: 0100 0073 3200 0000 0801 0412 0e01 0e01  ...s2...........
-00003840: 0e01 0e03 0e01 0e03 1201 0602 0a04 0806  ................
-00003850: 080d 0818 0201 0a03 0806 0803 0803 0201  ................
-00003860: 0a27 0201 0a21 080b 0201 7272 0000 0029  .'...!....rr...)
-00003870: 1672 3500 0000 728a 0000 0072 9e00 0000  .r5...r....r....
-00003880: 7262 0000 0072 8b00 0000 da07 7061 7468  rb...r......path
-00003890: 6c69 6272 0300 0000 da06 7479 7069 6e67  libr......typing
-000038a0: 7204 0000 0072 1e00 0000 7205 0000 0072  r....r....r....r
-000038b0: 4400 0000 7215 0000 0072 1700 0000 7266  D...r....r....rf
-000038c0: 0000 0072 0600 0000 7210 0000 0072 0d00  ...r....r....r..
-000038d0: 0000 723a 0000 0072 3b00 0000 724b 0000  ..r:...r;...rK..
-000038e0: 0072 7200 0000 720b 0000 0072 0b00 0000  .rr...r....r....
-000038f0: 720b 0000 0072 0c00 0000 da08 3c6d 6f64  r....r......<mod
-00003900: 756c 653e 0100 0000 7320 0000 0008 0108  ule>....s ......
-00003910: 0108 0108 0108 010c 010c 0208 010c 0208  ................
-00003920: 0108 0810 1210 4108 0410 380e 7f         ......A...8..
+00000e20: 0964 0a64 0b9c 0964 0c64 0d64 0e64 0e64  .d.d...d.d.d.d.d
+00000e30: 0f64 0d64 0864 1064 1164 0b9c 0964 129c  .d.d.d.d.d...d..
+00000e40: 025a 0465 056a 0664 136b 0572 8a65 04a0  .Z.e.j.d.k.r.e..
+00000e50: 0764 14a1 0101 0065 0464 1519 00a0 0764  .d.....e.d.....d
+00000e60: 16a1 0101 0065 0464 1519 00a0 0764 17a1  .....e.d.....d..
+00000e70: 0101 0065 0464 1519 00a0 0764 18a1 0101  ...e.d.....d....
+00000e80: 0065 0464 1519 00a0 0764 19a1 0101 0065  .e.d.....d.....e
+00000e90: 056a 0864 1a6b 0272 a065 04a0 0764 1464  .j.d.k.r.e...d.d
+00000ea0: 1ba1 0201 0064 1c64 1d84 005a 0964 1e64  .....d.d...Z.d.d
+00000eb0: 1f84 005a 0a64 2064 2184 005a 0b64 1b53  ...Z.d d!..Z.d.S
+00000ec0: 0029 22da 0e52 6564 6973 4149 5665 7273  .)"..RedisAIVers
+00000ed0: 696f 6e61 ff01 0000 4120 7375 6263 6c61  iona....A subcla
+00000ee0: 7373 206f 6620 5665 7273 696f 6e5f 2074  ss of Version_ t
+00000ef0: 6861 7420 686f 6c64 7320 7468 6520 6465  hat holds the de
+00000f00: 7065 6e64 656e 6379 2073 6574 7320 666f  pendency sets fo
+00000f10: 7220 5265 6469 7341 490a 0a20 2020 2074  r RedisAI..    t
+00000f20: 6869 7320 636c 6173 7320 7365 7276 6573  his class serves
+00000f30: 2074 776f 2070 7572 706f 7365 733a 0a0a   two purposes:..
+00000f40: 2020 2020 312e 2049 7420 6973 2075 7365      1. It is use
+00000f50: 6420 746f 2070 6f70 756c 6174 6520 7468  d to populate th
+00000f60: 6520 5b6d 6c5d 2060 6065 7874 7261 735f  e [ml] ``extras_
+00000f70: 7265 7175 6972 6560 6020 6f66 2074 6865  require`` of the
+00000f80: 2073 6574 7570 2e70 792e 0a20 2020 2054   setup.py..    T
+00000f90: 6869 7320 6973 2062 6563 6175 7365 2074  his is because t
+00000fa0: 6865 2052 6564 6973 4149 2076 6572 7369  he RedisAI versi
+00000fb0: 6f6e 2077 696c 6c20 6465 7465 726d 696e  on will determin
+00000fc0: 6520 7768 6963 6820 4d4c 2062 6173 6564  e which ML based
+00000fd0: 0a20 2020 2064 6570 656e 6465 6e63 6965  .    dependencie
+00000fe0: 7320 6172 6520 7265 7175 6972 6564 2e0a  s are required..
+00000ff0: 0a20 2020 2032 2e20 5573 6564 2074 6f20  .    2. Used to 
+00001000: 7365 7420 7468 6520 6465 6661 756c 7420  set the default 
+00001010: 7661 6c75 6573 2066 6f72 2050 7954 6f72  values for PyTor
+00001020: 6368 2c20 5446 2c20 616e 6420 4f4e 4e58  ch, TF, and ONNX
+00001030: 0a20 2020 2067 6976 656e 2074 6865 2053  .    given the S
+00001040: 4d41 5254 5349 4d5f 5245 4449 5341 4920  MARTSIM_REDISAI 
+00001050: 656e 7620 7661 7220 7365 7420 6279 2074  env var set by t
+00001060: 6865 2075 7365 722e 0a0a 2020 2020 4e4f  he user...    NO
+00001070: 5445 3a20 546f 7263 6820 7265 7175 6972  TE: Torch requir
+00001080: 6573 2061 6464 6974 696f 6e61 6c20 696e  es additional in
+00001090: 666f 726d 6174 696f 6e20 6465 7065 6e64  formation depend
+000010a0: 696e 6720 6f6e 2077 6865 7468 6572 0a20  ing on whether. 
+000010b0: 2020 2043 5055 206f 7220 4750 5520 7375     CPU or GPU su
+000010c0: 7070 6f72 7420 6973 2072 6571 7565 7374  pport is request
+000010d0: 6564 0a20 2020 207a 0532 2e36 2e32 7a05  ed.    z.2.6.2z.
+000010e0: 312e 392e 307a 0631 2e31 302e 337a 0631  1.9.0z.1.10.3z.1
+000010f0: 2e31 302e 307a 0531 2e30 2e32 7a05 312e  .10.0z.1.0.2z.1.
+00001100: 392e 317a 042b 6370 757a 062b 6375 3131  9.1z.+cpuz.+cu11
+00001110: 317a 0630 2e31 302e 3129 09da 0a74 656e  1z.0.10.1)...ten
+00001120: 736f 7266 6c6f 77da 046f 6e6e 78da 0873  sorflow..onnx..s
+00001130: 6b6c 326f 6e6e 78da 0b6f 6e6e 786d 6c74  kl2onnx..onnxmlt
+00001140: 6f6f 6c73 fa0c 7363 696b 6974 2d6c 6561  ools..scikit-lea
+00001150: 726e da05 746f 7263 68da 1074 6f72 6368  rn..torch..torch
+00001160: 5f63 7075 5f73 7566 6669 78da 1174 6f72  _cpu_suffix..tor
+00001170: 6368 5f63 7564 615f 7375 6666 6978 da0b  ch_cuda_suffix..
+00001180: 746f 7263 6876 6973 696f 6e7a 0532 2e38  torchvisionz.2.8
+00001190: 2e30 7a06 312e 3131 2e30 7a06 312e 3131  .0z.1.11.0z.1.11
+000011a0: 2e31 7a05 312e 312e 317a 062b 6375 3131  .1z.1.1.1z.+cu11
+000011b0: 337a 0630 2e31 322e 3029 02fa 0531 2e32  3z.0.12.0)...1.2
+000011c0: 2e35 fa05 312e 322e 3729 02e9 0300 0000  .5..1.2.7)......
+000011d0: e90a 0000 0072 4400 0000 7245 0000 0072  .....rD...rE...r
+000011e0: 3c00 0000 723d 0000 0072 3e00 0000 723f  <...r=...r>...r?
+000011f0: 0000 00da 0664 6172 7769 6e4e 6302 0000  .....darwinNc...
+00001200: 0000 0000 0000 0000 0003 0000 0006 0000  ................
+00001210: 0043 0000 0073 6c00 0000 7400 6401 6402  .C...sl...t.d.d.
+00001220: 8400 7c00 6a01 4400 8301 8301 7d02 7c02  ..|.j.D.....}.|.
+00001230: 7c01 6b04 722a 7402 6403 7c02 9b00 9d02  |.k.r*t.d.|.....
+00001240: 8301 8201 7c01 7c00 6a01 6b07 7262 7c01  ....|.|.j.k.rb|.
+00001250: a003 6404 a101 7246 6405 7c00 5f04 7168  ..d...rFd.|._.qh
+00001260: 7402 6406 7c01 9b00 6407 7c00 6a01 a005  t.d.|...d.|.j...
+00001270: a100 9b00 9d04 8301 8201 6e06 7c01 7c00  ..........n.|.|.
+00001280: 5f04 6400 5300 2908 4e63 0100 0000 0000  _.d.S.).Nc......
+00001290: 0000 0000 0000 0200 0000 0300 0000 7300  ..............s.
+000012a0: 0000 7316 0000 007c 005d 0e7d 0174 007c  ..s....|.].}.t.|
+000012b0: 0183 0156 0001 0071 0264 0053 0072 0f00  ...V...q.d.S.r..
+000012c0: 0000 2901 720d 0000 0029 0272 1100 0000  ..).r....).r....
+000012d0: da03 7665 7272 0b00 0000 720b 0000 0072  ..verr....r....r
+000012e0: 0c00 0000 7213 0000 00ba 0000 0073 0400  ....r........s..
+000012f0: 0000 0400 0200 7a2a 5265 6469 7341 4956  ......z*RedisAIV
+00001300: 6572 7369 6f6e 2e5f 5f69 6e69 745f 5f2e  ersion.__init__.
+00001310: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00001320: 723e 7a31 5265 6469 7341 4920 7665 7273  r>z1RedisAI vers
+00001330: 696f 6e20 6d75 7374 2062 6520 6772 6561  ion must be grea
+00001340: 7465 7220 7468 616e 206f 7220 6571 7561  ter than or equa
+00001350: 6c20 746f 207a 0331 2e32 7245 0000 007a  l to z.1.2rE...z
+00001360: 1849 6e76 616c 6964 2052 6564 6973 4149  .Invalid RedisAI
+00001370: 2076 6572 7369 6f6e 207a 0e2e 204f 7074   version z.. Opt
+00001380: 696f 6e73 2061 7265 2029 06da 036d 696e  ions are )...min
+00001390: da08 6465 6661 756c 7473 7206 0000 00da  ..defaultsr.....
+000013a0: 0a73 7461 7274 7377 6974 68da 0776 6572  .startswith..ver
+000013b0: 7369 6f6e da04 6b65 7973 2903 7218 0000  sion..keys).r...
+000013c0: 0072 1900 0000 5a0f 6d69 6e5f 7261 695f  .r....Z.min_rai_
+000013d0: 7665 7273 696f 6e72 0b00 0000 720b 0000  versionr....r...
+000013e0: 0072 0c00 0000 da08 5f5f 696e 6974 5f5f  .r......__init__
+000013f0: b900 0000 7318 0000 0000 0114 0108 0102  ....s...........
+00001400: 0108 ff04 030a 010a 0308 0202 0114 ff06  ................
+00001410: 047a 1752 6564 6973 4149 5665 7273 696f  .z.RedisAIVersio
+00001420: 6e2e 5f5f 696e 6974 5f5f 6302 0000 0000  n.__init__c.....
+00001430: 0000 0000 0000 0002 0000 0009 0000 0043  ...............C
+00001440: 0000 0073 4a00 0000 7a12 7c00 6a00 7c00  ...sJ...z.|.j.|.
+00001450: 6a01 1900 7c01 1900 5700 5300 0400 7402  j...|...W.S...t.
+00001460: 6b0a 7244 0100 0100 0100 7403 6401 7404  k.rD......t.d.t.
+00001470: 7c00 8301 6a05 9b00 6402 7c01 9b00 6403  |...j...d.|...d.
+00001480: 9d05 8301 6400 8202 5900 6e02 5800 6400  ....d...Y.n.X.d.
+00001490: 5300 2904 4efa 0127 7a1b 2720 6f62 6a65  S.).N..'z.' obje
+000014a0: 6374 2068 6173 206e 6f20 6174 7472 6962  ct has no attrib
+000014b0: 7574 6520 277a e427 0a0a 5468 6973 2069  ute 'z.'..This i
+000014c0: 7320 6c69 6b65 6c79 2061 2070 726f 626c  s likely a probl
+000014d0: 656d 2077 6974 6820 7468 6520 536d 6172  em with the Smar
+000014e0: 7453 696d 2062 7569 6c64 2070 726f 6365  tSim build proce
+000014f0: 7373 3b69 6620 7468 6973 2070 726f 626c  ss;if this probl
+00001500: 656d 2070 6572 7369 7374 7320 706c 6561  em persists plea
+00001510: 7365 206c 6f67 2061 206e 6577 2069 7373  se log a new iss
+00001520: 7565 2061 7420 6874 7470 733a 2f2f 6769  ue at https://gi
+00001530: 7468 7562 2e63 6f6d 2f43 7261 794c 6162  thub.com/CrayLab
+00001540: 732f 536d 6172 7453 696d 2f69 7373 7565  s/SmartSim/issue
+00001550: 7320 6f72 2067 6574 2069 6e20 636f 6e74  s or get in cont
+00001560: 6163 7420 7769 7468 2075 7320 6174 2068  act with us at h
+00001570: 7474 7073 3a2f 2f77 7777 2e63 7261 796c  ttps://www.crayl
+00001580: 6162 732e 6f72 672f 646f 6373 2f63 6f6d  abs.org/docs/com
+00001590: 6d75 6e69 7479 2e68 746d 6c29 0672 4b00  munity.html).rK.
+000015a0: 0000 724d 0000 00da 084b 6579 4572 726f  ..rM.....KeyErro
+000015b0: 72da 0e41 7474 7269 6275 7465 4572 726f  r..AttributeErro
+000015c0: 72da 0474 7970 6572 0700 0000 2902 7218  r..typer....).r.
+000015d0: 0000 00da 046e 616d 6572 0b00 0000 720b  .....namer....r.
+000015e0: 0000 0072 0c00 0000 da0b 5f5f 6765 7461  ...r......__geta
+000015f0: 7474 725f 5fcb 0000 0073 1000 0000 0001  ttr__....s......
+00001600: 0201 1201 0e01 0201 16ff 0207 02f9 7a1a  ..............z.
+00001610: 5265 6469 7341 4956 6572 7369 6f6e 2e5f  RedisAIVersion._
+00001620: 5f67 6574 6174 7472 5f5f 6301 0000 0000  _getattr__c.....
+00001630: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00001640: 0000 0073 1000 0000 7c00 6a00 7c00 6a01  ...s....|.j.|.j.
+00001650: 1900 a002 a100 5300 720f 0000 0029 0372  ......S.r....).r
+00001660: 4b00 0000 724d 0000 00da 0463 6f70 7972  K...rM.....copyr
+00001670: 2100 0000 720b 0000 0072 0b00 0000 720c  !...r....r....r.
+00001680: 0000 00da 0c67 6574 5f64 6566 6175 6c74  .....get_default
+00001690: 73d8 0000 0073 0200 0000 0001 7a1b 5265  s....s......z.Re
+000016a0: 6469 7341 4956 6572 7369 6f6e 2e67 6574  disAIVersion.get
+000016b0: 5f64 6566 6175 6c74 7329 0c72 0700 0000  _defaults).r....
+000016c0: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+000016d0: 4b00 0000 da03 7379 73da 0c76 6572 7369  K.....sys..versi
+000016e0: 6f6e 5f69 6e66 6fda 0370 6f70 da08 706c  on_info..pop..pl
+000016f0: 6174 666f 726d 724f 0000 0072 5500 0000  atformrO...rU...
+00001700: 7257 0000 0072 0b00 0000 720b 0000 0072  rW...r....r....r
+00001710: 0b00 0000 720c 0000 0072 3a00 0000 8600  ....r....r:.....
+00001720: 0000 7342 0000 0008 0104 1102 0102 0102  ..sB............
+00001730: 0102 0102 0102 0102 0102 0102 f704 0c02  ................
+00001740: 0102 0102 0102 0102 0102 0102 0102 0102  ................
+00001750: f704 f406 190a 010a 010e 010e 010e 010e  ................
+00001760: 020a 010c 0208 1208 0d72 3a00 0000 6300  .........r:...c.
+00001770: 0000 0000 0000 0000 0000 0000 0000 0008  ................
+00001780: 0000 0040 0000 0073 2201 0000 6500 5a01  ...@...s"...e.Z.
+00001790: 6400 5a02 6401 5a03 6504 6402 8301 5a05  d.Z.d.Z.e.d...Z.
+000017a0: 6504 6506 6403 6404 8302 8301 5a07 6504  e.e.d.d.....Z.e.
+000017b0: 6506 6405 6406 8302 8301 5a08 6506 6407  e.d.d.....Z.e.d.
+000017c0: 6408 8302 5a09 6504 6506 6409 640a 8302  d...Z.e.e.d.d...
+000017d0: 8301 5a0a 6506 640b 640c 8302 5a0b 6506  ..Z.e.d.d...Z.e.
+000017e0: 640d 650a 8302 5a0c 650d 6506 640e 640f  d.e...Z.e.e.d.d.
+000017f0: 8302 8301 5a0e 6506 6410 6411 8302 5a0f  ....Z.e.d.d...Z.
+00001800: 6506 6412 6413 650e 9b00 9d02 8302 5a10  e.d.d.e.......Z.
+00001810: 6504 6506 6414 650e 6a11 8302 8301 5a12  e.e.d.e.j.....Z.
+00001820: 6504 6506 6415 650e 6a13 8302 8301 5a14  e.e.d.e.j.....Z.
+00001830: 6504 6506 6416 650e 6a15 8302 8301 5a16  e.e.d.e.j.....Z.
+00001840: 6504 6506 6417 650e 6a17 8302 8301 5a18  e.e.d.e.j.....Z.
+00001850: 6504 650e 6a19 8301 5a1a 7a0e 6504 650e  e.e.j...Z.z.e.e.
+00001860: 6a1b 8301 5a1c 5700 6e18 0400 651d 6b0a  j...Z.W.n...e.k.
+00001870: 72f4 0100 0100 0100 6418 5a1c 5900 6e02  r.......d.Z.Y.n.
+00001880: 5800 6423 641a 641b 8401 5a1e 641c 641d  X.d#d.d...Z.d.d.
+00001890: 8400 5a1f 6520 641e 9c01 641f 6420 8404  ..Z.e d...d.d ..
+000018a0: 5a21 6421 6422 8400 5a22 6418 5300 2924  Z!d!d"..Z"d.S.)$
+000018b0: da09 5665 7273 696f 6e65 7261 6c03 0000  ..Versioneral...
+000018c0: 5665 7273 696f 6e65 7220 6973 2072 6573  Versioner is res
+000018d0: 706f 6e73 6962 6c65 2066 6f72 206d 616e  ponsible for man
+000018e0: 6167 696e 6720 616c 6c20 7468 6520 7665  aging all the ve
+000018f0: 7273 696f 6e73 0a20 2020 2077 6974 6869  rsions.    withi
+00001900: 6e20 536d 6172 7453 696d 2069 6e63 6c75  n SmartSim inclu
+00001910: 6469 6e67 2053 6d61 7274 5369 6d20 6974  ding SmartSim it
+00001920: 7365 6c66 2e0a 0a20 2020 2053 6d61 7274  self...    Smart
+00001930: 5369 6d27 7320 7665 7273 696f 6e20 6973  Sim's version is
+00001940: 2077 7269 7474 656e 2069 6e74 6f20 7665   written into ve
+00001950: 7273 696f 6e2e 7079 2075 706f 6e20 7069  rsion.py upon pi
+00001960: 7020 696e 7374 616c 6c0a 2020 2020 6279  p install.    by
+00001970: 2075 7369 6e67 2074 6869 7320 636c 6173   using this clas
+00001980: 7320 696e 2073 6574 7570 2e70 792e 2042  s in setup.py. B
+00001990: 7920 7365 7474 696e 6720 534d 4152 5453  y setting SMARTS
+000019a0: 494d 5f53 5546 4649 582c 0a20 2020 2074  IM_SUFFIX,.    t
+000019b0: 6865 2076 6572 7369 6f6e 2077 696c 6c20  he version will 
+000019c0: 6265 2077 7269 7474 656e 2061 7320 6120  be written as a 
+000019d0: 2264 6972 7479 2220 7665 7273 696f 6e20  "dirty" version 
+000019e0: 7769 7468 2074 6865 0a20 2020 2067 6974  with the.    git
+000019f0: 2d73 6861 2061 7070 656e 6465 642e 0a20  -sha appended.. 
+00001a00: 2020 2069 2e65 2e0a 2020 2020 2020 2020     i.e..        
+00001a10: 6578 706f 7274 2053 4d41 5254 5349 4d5f  export SMARTSIM_
+00001a20: 5355 4646 4958 3d6e 6967 6874 6c79 0a20  SUFFIX=nightly. 
+00001a30: 2020 2020 2020 2070 6970 2069 6e73 7461         pip insta
+00001a40: 6c6c 202d 6520 2e0a 2020 2020 2020 2020  ll -e ..        
+00001a50: 736d 6172 7473 696d 2e5f 5f76 6572 7369  smartsim.__versi
+00001a60: 6f6e 5f5f 203d 3d20 302e 332e 322b 6e69  on__ == 0.3.2+ni
+00001a70: 6768 746c 792d 3366 6532 3366 660a 0a20  ghtly-3fe23ff.. 
+00001a80: 2020 2056 6572 7369 6f6e 6572 206d 616e     Versioner man
+00001a90: 6167 6573 2074 6869 7264 2070 6172 7479  ages third party
+00001aa0: 2064 6570 656e 6465 6e63 6965 7320 616e   dependencies an
+00001ab0: 6420 7468 6569 7220 7665 7273 696f 6e73  d their versions
+00001ac0: 0a20 2020 2061 7320 7765 6c6c 2e20 5468  .    as well. Th
+00001ad0: 6573 6520 7665 7273 696f 6e73 2061 7265  ese versions are
+00001ae0: 2075 7365 6420 6279 2074 6865 2060 6073   used by the ``s
+00001af0: 6d61 7274 6060 2063 6c69 2069 6e20 7468  mart`` cli in th
+00001b00: 650a 2020 2020 6060 736d 6172 7420 6275  e.    ``smart bu
+00001b10: 696c 6460 6020 636f 6d6d 616e 6420 746f  ild`` command to
+00001b20: 2064 6574 6572 6d69 6e65 2077 6869 6368   determine which
+00001b30: 2064 6570 656e 6465 6e63 7920 7665 7273   dependency vers
+00001b40: 696f 6e73 0a20 2020 2074 6f20 6c6f 6f6b  ions.    to look
+00001b50: 2066 6f72 2061 6e64 2064 6f77 6e6c 6f61   for and downloa
+00001b60: 642e 0a0a 2020 2020 4465 6661 756c 7420  d...    Default 
+00001b70: 7665 7273 696f 6e73 2066 6f72 2053 6d61  versions for Sma
+00001b80: 7274 5369 6d2c 2053 6d61 7274 5265 6469  rtSim, SmartRedi
+00001b90: 732c 2052 6564 6973 2c20 616e 6420 5265  s, Redis, and Re
+00001ba0: 6469 7341 4920 6172 650a 2020 2020 616c  disAI are.    al
+00001bb0: 6c20 7365 7420 6865 7265 2e20 5365 7474  l set here. Sett
+00001bc0: 696e 6720 6120 6465 6661 756c 7420 7665  ing a default ve
+00001bd0: 7273 696f 6e20 666f 7220 5265 6469 7341  rsion for RedisA
+00001be0: 4920 616c 736f 2064 6963 7461 7465 730a  I also dictates.
+00001bf0: 2020 2020 6465 6661 756c 7420 7665 7273      default vers
+00001c00: 696f 6e73 206f 6620 7468 6520 6d61 6368  ions of the mach
+00001c10: 696e 6520 6c65 6172 6e69 6e67 206c 6962  ine learning lib
+00001c20: 7261 7269 6573 2e0a 2020 2020 7a05 332e  raries..    z.3.
+00001c30: 382e 305a 1053 4d41 5254 5349 4d5f 5645  8.0Z.SMARTSIM_VE
+00001c40: 5253 494f 4e7a 0530 2e34 2e32 5a12 534d  RSIONz.0.4.2Z.SM
+00001c50: 4152 5452 4544 4953 5f56 4552 5349 4f4e  ARTREDIS_VERSION
+00001c60: 7a05 302e 342e 30da 0f53 4d41 5254 5349  z.0.4.0..SMARTSI
+00001c70: 4d5f 5355 4646 4958 da00 5a0e 534d 4152  M_SUFFIX..Z.SMAR
+00001c80: 5453 494d 5f52 4544 4953 7a05 372e 302e  TSIM_REDISz.7.0.
+00001c90: 355a 1253 4d41 5254 5349 4d5f 5245 4449  5Z.SMARTSIM_REDI
+00001ca0: 535f 5552 4c7a 2368 7474 7073 3a2f 2f67  S_URLz#https://g
+00001cb0: 6974 6875 622e 636f 6d2f 7265 6469 732f  ithub.com/redis/
+00001cc0: 7265 6469 732e 6769 742f 5a15 534d 4152  redis.git/Z.SMAR
+00001cd0: 5453 494d 5f52 4544 4953 5f42 5241 4e43  TSIM_REDIS_BRANC
+00001ce0: 485a 1053 4d41 5254 5349 4d5f 5245 4449  HZ.SMARTSIM_REDI
+00001cf0: 5341 4972 4500 0000 5a14 534d 4152 5453  SAIrE...Z.SMARTS
+00001d00: 494d 5f52 4544 4953 4149 5f55 524c 7a27  IM_REDISAI_URLz'
+00001d10: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001d20: 6f6d 2f52 6564 6973 4149 2f52 6564 6973  om/RedisAI/Redis
+00001d30: 4149 2e67 6974 2f5a 1753 4d41 5254 5349  AI.git/Z.SMARTSI
+00001d40: 4d5f 5245 4449 5341 495f 4252 414e 4348  M_REDISAI_BRANCH
+00001d50: da01 765a 0e53 4d41 5254 5349 4d5f 544f  ..vZ.SMARTSIM_TO
+00001d60: 5243 485a 1153 4d41 5254 5349 4d5f 544f  RCHZ.SMARTSIM_TO
+00001d70: 5243 4856 4953 da10 544f 5243 485f 4350  RCHVIS..TORCH_CP
+00001d80: 555f 5355 4646 4958 da11 544f 5243 485f  U_SUFFIX..TORCH_
+00001d90: 4355 4441 5f53 5546 4649 584e da05 5245  CUDA_SUFFIXN..RE
+00001da0: 4449 5363 0200 0000 0000 0000 0000 0000  DISc............
+00001db0: 0500 0000 0600 0000 4300 0000 7356 0000  ........C...sV..
+00001dc0: 0064 0164 027c 0164 0364 0464 0567 067d  .d.d.|.d.d.d.g.}
+00001dd0: 027c 006a 007c 006a 017c 006a 027c 006a  .|.j.|.j.|.j.|.j
+00001de0: 037c 006a 047c 006a 0567 067d 037c 006a  .|.j.|.j.g.}.|.j
+00001df0: 0672 487c 02a0 0764 06a1 0101 007c 03a0  .rH|...d.....|..
+00001e00: 077c 006a 06a1 0101 007c 027c 0364 079c  .|.j.....|.|.d..
+00001e10: 027d 047c 0453 0029 084e da08 534d 4152  .}.|.S.).N..SMAR
+00001e20: 5453 494d da0a 534d 4152 5452 4544 4953  TSIM..SMARTREDIS
+00001e30: da07 5245 4449 5341 49da 0554 4f52 4348  ..REDISAI..TORCH
+00001e40: da0a 5445 4e53 4f52 464c 4f57 da04 4f4e  ..TENSORFLOW..ON
+00001e50: 4e58 2902 5a08 5061 636b 6167 6573 5a08  NX).Z.PackagesZ.
+00001e60: 5665 7273 696f 6e73 2908 7263 0000 0072  Versions).rc...r
+00001e70: 6400 0000 7262 0000 0072 6500 0000 7266  d...rb...re...rf
+00001e80: 0000 0072 6700 0000 7268 0000 00da 0661  ...rg...rh.....a
+00001e90: 7070 656e 6429 0572 1800 0000 5a07 6462  ppend).r....Z.db
+00001ea0: 5f6e 616d 65da 0870 6163 6b61 6765 73da  _name..packages.
+00001eb0: 0876 6572 7369 6f6e 7372 1900 0000 720b  .versionsr....r.
+00001ec0: 0000 0072 0b00 0000 720c 0000 00da 0761  ...r....r......a
+00001ed0: 735f 6469 6374 1801 0000 7326 0000 0000  s_dict....s&....
+00001ee0: 0202 0102 0102 0102 0102 0102 fa04 0904  ................
+00001ef0: 0104 0104 0104 0104 0104 fa04 0806 010a  ................
+00001f00: 010c 010a 017a 1156 6572 7369 6f6e 6572  .....z.Versioner
+00001f10: 2e61 735f 6469 6374 6301 0000 0000 0000  .as_dictc.......
+00001f20: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+00001f30: 0073 3c00 0000 7c00 6a00 a001 a100 7d01  .s<...|.j.....}.
+00001f40: 6401 6402 6403 6404 6704 7d02 7c02 4400  d.d.d.d.g.}.|.D.
+00001f50: 5d0e 7d03 7c01 a002 7c03 a101 0100 711a  ].}.|...|.....q.
+00001f60: 6405 6406 8400 7c01 a003 a100 4400 8301  d.d...|.....D...
+00001f70: 5300 2907 7a74 4f70 7469 6f6e 616c 204d  S.).ztOptional M
+00001f80: 4c2f 444c 2064 6570 656e 6465 6e63 6965  L/DL dependencie
+00001f90: 7320 7765 2073 7567 6765 7374 2066 6f72  s we suggest for
+00001fa0: 2074 6865 2075 7365 722e 0a0a 2020 2020   the user...    
+00001fb0: 2020 2020 5468 6520 6465 6661 756c 7473      The defaults
+00001fc0: 2061 7265 2062 6173 6564 206f 6e20 7468   are based on th
+00001fd0: 6520 5265 6469 7341 4920 7665 7273 696f  e RedisAI versio
+00001fe0: 6e0a 2020 2020 2020 2020 7240 0000 0072  n.        r@...r
+00001ff0: 4300 0000 7241 0000 0072 4200 0000 6301  C...rA...rB...c.
+00002000: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+00002010: 0000 0053 0000 0073 1e00 0000 6700 7c00  ...S...s....g.|.
+00002020: 5d16 5c02 7d01 7d02 7c01 9b00 6400 7c02  ].\.}.}.|...d.|.
+00002030: 9b00 9d03 9102 7104 5300 2901 7a02 3d3d  ......q.S.).z.==
+00002040: 720b 0000 0029 0372 1100 0000 da03 6c69  r....).r......li
+00002050: 6272 1900 0000 720b 0000 0072 0b00 0000  br....r....r....
+00002060: 720c 0000 00da 0a3c 6c69 7374 636f 6d70  r......<listcomp
+00002070: 3e44 0100 0073 0400 0000 0600 0600 7a30  >D...s........z0
+00002080: 5665 7273 696f 6e65 722e 6d6c 5f65 7874  Versioner.ml_ext
+00002090: 7261 735f 7265 7175 6972 6564 2e3c 6c6f  ras_required.<lo
+000020a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000020b0: 2904 7265 0000 0072 5700 0000 725a 0000  ).re...rW...rZ..
+000020c0: 00da 0569 7465 6d73 2904 7218 0000 005a  ...items).r....Z
+000020d0: 0b6d 6c5f 6465 6661 756c 7473 5a0d 5f74  .ml_defaultsZ._t
+000020e0: 6f72 6368 5f66 6965 6c64 73da 0566 6965  orch_fields..fie
+000020f0: 6c64 720b 0000 0072 0b00 0000 720c 0000  ldr....r....r...
+00002100: 00da 126d 6c5f 6578 7472 6173 5f72 6571  ...ml_extras_req
+00002110: 7569 7265 642f 0100 0073 1200 0000 0005  uired/...s......
+00002120: 0a08 0201 0201 0201 02fc 0406 0801 0c02  ................
+00002130: 7a1c 5665 7273 696f 6e65 722e 6d6c 5f65  z.Versioner.ml_e
+00002140: 7874 7261 735f 7265 7175 6972 6564 2901  xtras_required).
+00002150: da06 7265 7475 726e 6302 0000 0000 0000  ..returnc.......
+00002160: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
+00002170: 0073 4800 0000 7a2c 7400 6a01 6401 6402  .sH...z,t.j.d.d.
+00002180: 6403 6703 7c01 6404 8d02 a002 6405 a101  d.g.|.d.....d...
+00002190: a003 a100 7d02 7c02 6406 6407 8502 1900  ....}.|.d.d.....
+000021a0: 5700 5300 0400 7404 6b0a 7242 0100 0100  W.S...t.k.rB....
+000021b0: 0100 5900 6408 5300 5800 6406 5300 2909  ..Y.d.S.X.d.S.).
+000021c0: 7a25 4765 7420 7468 6520 6769 7420 7368  z%Get the git sh
+000021d0: 6120 6f66 2074 6865 2063 7572 7265 6e74  a of the current
+000021e0: 2062 7261 6e63 68da 0367 6974 7a09 7265   branch..gitz.re
+000021f0: 762d 7061 7273 655a 0448 4541 4429 01da  v-parseZ.HEAD)..
+00002200: 0363 7764 da05 6173 6369 694e e907 0000  .cwd..asciiN....
+00002210: 0072 5e00 0000 2905 da0a 7375 6270 726f  .r^...)...subpro
+00002220: 6365 7373 da0c 6368 6563 6b5f 6f75 7470  cess..check_outp
+00002230: 7574 da06 6465 636f 6465 da05 7374 7269  ut..decode..stri
+00002240: 70da 0945 7863 6570 7469 6f6e 2903 7218  p..Exception).r.
+00002250: 0000 00da 0c73 6574 7570 5f70 795f 6469  .....setup_py_di
+00002260: 725a 0373 6861 720b 0000 0072 0b00 0000  rZ.shar....r....
+00002270: 720c 0000 00da 0767 6574 5f73 6861 4601  r......get_shaF.
+00002280: 0000 7310 0000 0000 0202 0214 0102 ff06  ..s.............
+00002290: ff02 050e 010e 027a 1156 6572 7369 6f6e  .......z.Version
+000022a0: 6572 2e67 6574 5f73 6861 6302 0000 0000  er.get_shac.....
+000022b0: 0000 0000 0000 0006 0000 0009 0000 0043  ...............C
+000022c0: 0000 0073 8e00 0000 7c00 6a00 7d02 7c00  ...s....|.j.}.|.
+000022d0: 6a01 7242 7c00 a002 7c01 a101 7d03 7c03  j.rB|...|...}.|.
+000022e0: 7232 7c02 9b00 6401 7c00 6a01 9b00 6402  r2|...d.|.j...d.
+000022f0: 7c03 9b00 9d05 7d02 6e10 7c02 9b00 6401  |.....}.n.|...d.
+00002300: 7c00 6a01 9b00 9d03 7d02 7c01 6403 1b00  |.j.....}.|.d...
+00002310: 6404 1b00 7d04 7403 7c04 6405 8302 8f2c  d...}.t.|.d....,
+00002320: 7d05 7c05 a004 6406 a101 0100 7c05 a004  }.|...d.....|...
+00002330: 6407 a101 0100 7c05 a004 6408 7c02 9b00  d.....|...d.|...
+00002340: 6409 9d03 a101 0100 5700 3500 5100 5200  d.......W.5.Q.R.
+00002350: 5800 7c02 5300 290a 7a83 0a20 2020 2020  X.|.S.).z..     
+00002360: 2020 2057 7269 7465 2076 6572 7369 6f6e     Write version
+00002370: 2069 6e66 6f20 746f 2076 6572 7369 6f6e   info to version
+00002380: 2e70 790a 0a20 2020 2020 2020 2055 7365  .py..        Use
+00002390: 2067 6974 5f73 6861 2069 6e20 7468 6520   git_sha in the 
+000023a0: 6361 7365 2077 6865 7265 2073 6d61 7274  case where smart
+000023b0: 7369 6d20 7375 6666 6978 2069 7320 7365  sim suffix is se
+000023c0: 7420 696e 2074 6865 2065 6e76 6972 6f6e  t in the environ
+000023d0: 6d65 6e74 0a20 2020 2020 2020 20fa 012b  ment.        ..+
+000023e0: 720e 0000 00da 0873 6d61 7274 7369 6d7a  r......smartsimz
+000023f0: 0a76 6572 7369 6f6e 2e70 79da 0177 7a33  .version.py..wz3
+00002400: 2320 5468 6973 2066 696c 6520 6973 2061  # This file is a
+00002410: 7574 6f6d 6174 6963 616c 6c79 2067 656e  utomatically gen
+00002420: 6572 6174 6564 2062 7920 7365 7475 702e  erated by setup.
+00002430: 7079 0a7a 2323 2064 6f20 6e6f 7420 6564  py.z## do not ed
+00002440: 6974 2074 6869 7320 6669 6c65 206d 616e  it this file man
+00002450: 7561 6c6c 792e 0a0a 7a0f 5f5f 7665 7273  ually...z.__vers
+00002460: 696f 6e5f 5f20 3d20 277a 0227 0a29 0572  ion__ = 'z.'.).r
+00002470: 6300 0000 725d 0000 0072 7d00 0000 da04  c...r]...r}.....
+00002480: 6f70 656e da05 7772 6974 6529 0672 1800  open..write).r..
+00002490: 0000 727c 0000 0072 4d00 0000 5a07 6769  ..r|...rM...Z.gi
+000024a0: 745f 7368 615a 0c76 6572 7369 6f6e 5f66  t_shaZ.version_f
+000024b0: 696c 65da 0166 720b 0000 0072 0b00 0000  ile..fr....r....
+000024c0: 720c 0000 00da 0d77 7269 7465 5f76 6572  r......write_ver
+000024d0: 7369 6f6e 5301 0000 7318 0000 0000 0606  sionS...s.......
+000024e0: 0106 010a 0104 0118 0310 020c 010c 010a  ................
+000024f0: 010a 021c 017a 1756 6572 7369 6f6e 6572  .....z.Versioner
+00002500: 2e77 7269 7465 5f76 6572 7369 6f6e 2901  .write_version).
+00002510: 7262 0000 0029 2372 0700 0000 7208 0000  rb...)#r....r...
+00002520: 0072 0900 0000 720a 0000 0072 0d00 0000  .r....r....r....
+00002530: da0a 5059 5448 4f4e 5f4d 494e 7239 0000  ..PYTHON_MINr9..
+00002540: 0072 6300 0000 7264 0000 0072 5d00 0000  .rc...rd...r]...
+00002550: 7262 0000 00da 0952 4544 4953 5f55 524c  rb.....REDIS_URL
+00002560: 5a0c 5245 4449 535f 4252 414e 4348 723a  Z.REDIS_BRANCHr:
+00002570: 0000 0072 6500 0000 5a0b 5245 4449 5341  ...re...Z.REDISA
+00002580: 495f 5552 4c5a 0e52 4544 4953 4149 5f42  I_URLZ.REDISAI_B
+00002590: 5241 4e43 4872 4000 0000 7266 0000 0072  RANCHr@...rf...r
+000025a0: 4300 0000 5a0b 544f 5243 4856 4953 494f  C...Z.TORCHVISIO
+000025b0: 4e72 4100 0000 7260 0000 0072 4200 0000  NrA...r`...rB...
+000025c0: 7261 0000 0072 3b00 0000 7267 0000 0072  ra...r;...rg...r
+000025d0: 3c00 0000 7268 0000 0072 5200 0000 726c  <...rh...rR...rl
+000025e0: 0000 0072 7100 0000 7210 0000 0072 7d00  ...rq...r....r}.
+000025f0: 0000 7284 0000 0072 0b00 0000 720b 0000  ..r....r....r...
+00002600: 0072 0b00 0000 720c 0000 0072 5c00 0000  .r....r....r\...
+00002610: dc00 0000 733a 0000 0008 0104 1708 030e  ....s:..........
+00002620: 010e 010a 030e 010a 010a 030e 0102 0102  ................
+00002630: 0002 ff04 0310 0410 0110 0110 0102 010a  ................
+00002640: ff04 060a 0102 010e 010e 010a 020a 1708  ................
+00002650: 170e 0d72 5c00 0000 6300 0000 0000 0000  ...r\...c.......
+00002660: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
+00002670: 0073 f000 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+00002680: 5a03 6504 6a05 a006 6402 6403 a102 5a07  Z.e.j...d.d...Z.
+00002690: 6504 6a05 a006 6404 6405 a102 5a08 6504  e.j...d.d...Z.e.
+000026a0: 6a05 a006 6406 6407 a102 5a09 6504 6a05  j...d.d...Z.e.j.
+000026b0: a006 6408 6407 a102 5a0a 6504 6a05 a006  ..d.d...Z.e.j...
+000026c0: 6409 640a a102 5a0b 6504 6a05 a006 640b  d.d...Z.e.j...d.
+000026d0: 640c a102 5a0c 650d 6504 6a05 a006 640d  d...Z.e.e.j...d.
+000026e0: 640e a102 8301 5a0e 650f 6a10 5a11 6429  d.....Z.e.j.Z.d)
+000026f0: 6410 6411 8401 5a12 6412 6413 8400 5a13  d.d...Z.d.d...Z.
+00002700: 6414 6415 8400 5a14 6416 6417 8400 5a15  d.d...Z.d.d...Z.
+00002710: 6516 6418 6419 8400 8301 5a17 641a 641b  e.d.d.....Z.d.d.
+00002720: 8400 5a18 641c 641d 8400 5a19 641e 641f  ..Z.d.d...Z.d.d.
+00002730: 8400 5a1a 6516 6420 6421 8400 8301 5a1b  ..Z.e.d d!....Z.
+00002740: 651c 6422 6423 8400 8301 5a1d 6424 6425  e.d"d#....Z.d$d%
+00002750: 8400 5a1e 651c 642a 6427 6428 8401 8301  ..Z.e.d*d'd(....
+00002760: 5a1f 6426 5300 292b da08 4275 696c 6445  Z.d&S.)+..BuildE
+00002770: 6e76 6137 0200 0045 6e76 6972 6f6e 6d65  nva7...Environme
+00002780: 6e74 2066 6f72 2062 7569 6c64 696e 6720  nt for building 
+00002790: 7468 6972 642d 7061 7274 7920 6465 7065  third-party depe
+000027a0: 6e64 656e 6369 6573 0a0a 2020 2020 4275  ndencies..    Bu
+000027b0: 696c 6445 6e76 2070 726f 7669 6465 7320  ildEnv provides 
+000027c0: 6120 6d65 7468 6f64 2066 6f72 2063 6f6e  a method for con
+000027d0: 6669 6775 7269 6e67 2068 6f77 2074 6865  figuring how the
+000027e0: 2074 6869 7264 2d70 6172 7479 0a20 2020   third-party.   
+000027f0: 2064 6570 656e 6465 6e63 6965 7320 7769   dependencies wi
+00002800: 7468 696e 2053 6d61 7274 5369 6d20 6172  thin SmartSim ar
+00002810: 6520 6275 696c 742c 206e 616d 656c 7920  e built, namely 
+00002820: 5265 6469 732f 4b65 7944 420a 2020 2020  Redis/KeyDB.    
+00002830: 616e 6420 5265 6469 7341 492e 0a0a 2020  and RedisAI...  
+00002840: 2020 5468 6520 656e 7669 726f 6e6d 656e    The environmen
+00002850: 7420 7661 7269 6162 6c65 7320 6c69 7374  t variables list
+00002860: 6564 2068 6572 6520 6361 6e20 6265 2073  ed here can be s
+00002870: 6574 2074 6f20 636f 6e74 726f 6c20 7468  et to control th
+00002880: 650a 2020 2020 5265 6469 7320 6275 696c  e.    Redis buil
+00002890: 6420 696e 2074 6865 2070 6970 2077 6865  d in the pip whe
+000028a0: 656c 2062 7569 6c64 2061 7320 7765 6c6c  el build as well
+000028b0: 2061 7320 7468 6520 5265 6469 7320 616e   as the Redis an
+000028c0: 6420 5265 6469 7341 490a 2020 2020 6275  d RedisAI.    bu
+000028d0: 696c 6420 6578 6563 7574 6564 2062 7920  ild executed by 
+000028e0: 7468 6520 434c 492e 0a0a 2020 2020 4275  the CLI...    Bu
+000028f0: 696c 6420 746f 6f6c 7320 6172 6520 616c  ild tools are al
+00002900: 736f 2063 6865 636b 6564 2066 6f72 2068  so checked for h
+00002910: 6572 6520 616e 6420 6966 2074 6865 7920  ere and if they 
+00002920: 6172 6520 6e6f 7420 666f 756e 640a 2020  are not found.  
+00002930: 2020 7468 656e 2061 2053 6574 7570 4572    then a SetupEr
+00002940: 726f 7220 6973 2072 6169 7365 642e 0a0a  ror is raised...
+00002950: 2020 2020 4164 6469 6e67 2074 6865 202d      Adding the -
+00002960: 7620 666c 6167 2074 6f20 6060 736d 6172  v flag to ``smar
+00002970: 7420 6275 696c 6460 6020 7769 6c6c 2073  t build`` will s
+00002980: 686f 7720 7468 6520 6275 696c 6420 656e  how the build en
+00002990: 7669 726f 6e6d 656e 740a 2020 2020 6265  vironment.    be
+000029a0: 696e 6720 7573 6564 2e0a 2020 2020 da02  ing used..    ..
+000029b0: 4343 5a03 6763 63da 0343 5858 7a03 672b  CCZ.gcc..CXXz.g+
+000029c0: 2bda 0643 464c 4147 5372 5e00 0000 da08  +..CFLAGSr^.....
+000029d0: 4358 5846 4c41 4753 da06 4d41 4c4c 4f43  CXXFLAGS..MALLOC
+000029e0: da04 6c69 6263 5a0a 4255 494c 445f 4a4f  ..libcZ.BUILD_JO
+000029f0: 4253 7223 0000 005a 094e 4f5f 4348 4543  BSr#...Z.NO_CHEC
+00002a00: 4b53 7201 0000 0054 6302 0000 0000 0000  KSr....Tc.......
+00002a10: 0000 0000 0002 0000 0002 0000 0043 0000  .............C..
+00002a20: 0073 1000 0000 7c01 720c 7c00 a000 a100  .s....|.r.|.....
+00002a30: 0100 6400 5300 720f 0000 0029 01da 1263  ..d.S.r....)...c
+00002a40: 6865 636b 5f64 6570 656e 6465 6e63 6965  heck_dependencie
+00002a50: 7329 0272 1800 0000 da06 6368 6563 6b73  s).r......checks
+00002a60: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00002a70: 4f00 0000 8b01 0000 7304 0000 0000 0104  O.......s.......
+00002a80: 017a 1142 7569 6c64 456e 762e 5f5f 696e  .z.BuildEnv.__in
+00002a90: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+00002aa0: 0003 0000 0007 0000 0043 0000 0073 3c00  .........C...s<.
+00002ab0: 0000 6401 6402 6403 6404 6405 7c00 6a00  ..d.d.d.d.d.|.j.
+00002ac0: 7c00 6a01 6707 7d01 7402 7c00 6a03 8301  |.j.g.}.t.|.j...
+00002ad0: 6406 6b02 7238 7c01 4400 5d0e 7d02 7c00  d.k.r8|.D.].}.|.
+00002ae0: a004 7c02 a101 0100 7128 6400 5300 2907  ..|.....q(d.S.).
+00002af0: 4e72 7300 0000 7a07 6769 742d 6c66 73da  Nrs...z.git-lfs.
+00002b00: 046d 616b 655a 0477 6765 745a 0563 6d61  .makeZ.wgetZ.cma
+00002b10: 6b65 7201 0000 0029 0572 8800 0000 7289  ker....).r....r.
+00002b20: 0000 0072 1c00 0000 da06 4348 4543 4b53  ...r......CHECKS
+00002b30: da16 6368 6563 6b5f 6275 696c 645f 6465  ..check_build_de
+00002b40: 7065 6e64 656e 6379 2903 7218 0000 00da  pendency).r.....
+00002b50: 0464 6570 73da 0364 6570 720b 0000 0072  .deps..depr....r
+00002b60: 0b00 0000 720c 0000 0072 8e00 0000 8f01  ....r....r......
+00002b70: 0000 7308 0000 0000 0116 010e 0108 017a  ..s............z
+00002b80: 1b42 7569 6c64 456e 762e 6368 6563 6b5f  .BuildEnv.check_
+00002b90: 6465 7065 6e64 656e 6369 6573 6301 0000  dependenciesc...
+00002ba0: 0000 0000 0000 0000 0002 0000 0007 0000  ................
+00002bb0: 0043 0000 0073 2a00 0000 7400 6a01 a002  .C...s*...t.j...
+00002bc0: a100 7d01 7c01 a003 7c00 6a04 7c00 6a05  ..}.|...|.j.|.j.
+00002bd0: 7c00 6a06 7c00 6a07 6401 9c04 a101 0100  |.j.|.j.d.......
+00002be0: 7c01 5300 2902 4e29 0472 8800 0000 7289  |.S.).N).r....r.
+00002bf0: 0000 0072 8a00 0000 728b 0000 0029 0872  ...r....r....).r
+00002c00: 3400 0000 7235 0000 0072 5600 0000 da06  4...r5...rV.....
+00002c10: 7570 6461 7465 7288 0000 0072 8900 0000  updater....r....
+00002c20: 728a 0000 0072 8b00 0000 2902 7218 0000  r....r....).r...
+00002c30: 00da 0365 6e76 720b 0000 0072 0b00 0000  ...envr....r....
+00002c40: 720c 0000 00da 085f 5f63 616c 6c5f 5f95  r......__call__.
+00002c50: 0100 0073 1200 0000 0002 0a01 0402 0401  ...s............
+00002c60: 0401 0401 04fc 04ff 0408 7a11 4275 696c  ..........z.Buil
+00002c70: 6445 6e76 2e5f 5f63 616c 6c5f 5f63 0100  dEnv.__call__c..
+00002c80: 0000 0000 0000 0000 0000 0400 0000 0800  ................
+00002c90: 0000 4300 0000 7346 0000 0064 0164 0264  ..C...sF...d.d.d
+00002ca0: 0364 0464 0564 0664 0764 0867 087d 017c  .d.d.d.d.d.g.}.|
+00002cb0: 006a 007c 006a 017c 006a 027c 006a 037c  .j.|.j.|.j.|.j.|
+00002cc0: 006a 047c 006a 057c 006a 067c 006a 0767  .j.|.j.|.j.|.j.g
+00002cd0: 087d 027c 017c 0264 099c 027d 037c 0353  .}.|.|.d...}.|.S
+00002ce0: 0029 0a4e 7288 0000 0072 8900 0000 728a  .).Nr....r....r.
+00002cf0: 0000 0072 8b00 0000 728c 0000 00da 044a  ...r....r......J
+00002d00: 4f42 535a 0e50 5954 484f 4e5f 5645 5253  OBSZ.PYTHON_VERS
+00002d10: 494f 4eda 0850 4c41 5446 4f52 4d29 02da  ION..PLATFORM)..
+00002d20: 0b45 6e76 6972 6f6e 6d65 6e74 5a06 5661  .EnvironmentZ.Va
+00002d30: 6c75 6573 2908 7288 0000 0072 8900 0000  lues).r....r....
+00002d40: 728a 0000 0072 8b00 0000 728c 0000 0072  r....r....r....r
+00002d50: 9800 0000 da0e 7079 7468 6f6e 5f76 6572  ......python_ver
+00002d60: 7369 6f6e 7299 0000 0029 0472 1800 0000  sionr....).r....
+00002d70: da09 7661 7269 6162 6c65 73da 0676 616c  ..variables..val
+00002d80: 7565 7372 9600 0000 720b 0000 0072 0b00  uesr....r....r..
+00002d90: 0000 720c 0000 0072 6c00 0000 a201 0000  ..r....rl.......
+00002da0: 7328 0000 0000 0202 0102 0102 0102 0102  s(..............
+00002db0: 0102 0102 0102 f804 0b04 0104 0104 0104  ................
+00002dc0: 0104 0104 0104 0104 f804 0a0a 017a 1042  .............z.B
+00002dd0: 7569 6c64 456e 762e 6173 5f64 6963 7463  uildEnv.as_dictc
+00002de0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00002df0: 0200 0000 4300 0000 7308 0000 0074 00a0  ....C...s....t..
+00002e00: 01a1 0053 0072 0f00 0000 2902 725b 0000  ...S.r....).r[..
+00002e10: 0072 9b00 0000 7221 0000 0072 0b00 0000  .r....r!...r....
+00002e20: 720b 0000 0072 0c00 0000 729b 0000 00ba  r....r....r.....
+00002e30: 0100 0073 0200 0000 0002 7a17 4275 696c  ...s......z.Buil
+00002e40: 6445 6e76 2e70 7974 686f 6e5f 7665 7273  dEnv.python_vers
+00002e50: 696f 6e63 0200 0000 0000 0000 0000 0000  ionc............
+00002e60: 0400 0000 0600 0000 4300 0000 732c 0000  ........C...s,..
+00002e70: 0074 006a 017d 0274 027c 026a 039b 0064  .t.j.}.t.|.j...d
+00002e80: 017c 026a 049b 0064 017c 026a 059b 009d  .|.j...d.|.j....
+00002e90: 0583 017d 037c 037c 016b 0453 0029 027a  ...}.|.|.k.S.).z
+00002ea0: 2244 6574 6563 7420 6966 2073 7973 7465  "Detect if syste
+00002eb0: 6d20 5079 7468 6f6e 2069 7320 746f 6f20  m Python is too 
+00002ec0: 6f6c 6472 0e00 0000 2906 7258 0000 0072  oldr....).rX...r
+00002ed0: 5900 0000 720d 0000 0072 2200 0000 7224  Y...r....r"...r$
+00002ee0: 0000 0072 2700 0000 2904 7218 0000 005a  ...r'...).r....Z
+00002ef0: 0a70 7974 686f 6e5f 6d69 6e5a 0673 7973  .python_minZ.sys
+00002f00: 5f70 795a 0d73 7973 7465 6d5f 7079 7468  _pyZ.system_pyth
+00002f10: 6f6e 720b 0000 0072 0b00 0000 720c 0000  onr....r....r...
+00002f20: 00da 1469 735f 636f 6d70 6174 6962 6c65  ...is_compatible
+00002f30: 5f70 7974 686f 6ebe 0100 0073 0600 0000  _python....s....
+00002f40: 0002 0601 1e01 7a1d 4275 696c 6445 6e76  ......z.BuildEnv
+00002f50: 2e69 735f 636f 6d70 6174 6962 6c65 5f70  .is_compatible_p
+00002f60: 7974 686f 6e63 0100 0000 0000 0000 0000  ythonc..........
+00002f70: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
+00002f80: 0000 007c 006a 0064 016b 0653 0029 024e  ...|.j.d.k.S.).N
+00002f90: 2903 da05 7769 6e33 32da 0663 7967 7769  )...win32..cygwi
+00002fa0: 6e5a 046d 7379 73a9 0172 9900 0000 7221  nZ.msys..r....r!
+00002fb0: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
+00002fc0: 0000 da0a 6973 5f77 696e 646f 7773 c401  ....is_windows..
+00002fd0: 0000 7302 0000 0000 017a 1342 7569 6c64  ..s......z.Build
+00002fe0: 456e 762e 6973 5f77 696e 646f 7773 6301  Env.is_windowsc.
+00002ff0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00003000: 0000 0043 0000 0073 0a00 0000 7c00 6a00  ...C...s....|.j.
+00003010: 6401 6b02 5300 2902 4e72 4800 0000 72a1  d.k.S.).NrH...r.
+00003020: 0000 0072 2100 0000 720b 0000 0072 0b00  ...r!...r....r..
+00003030: 0000 720c 0000 00da 0869 735f 6d61 636f  ..r......is_maco
+00003040: 73c7 0100 0073 0200 0000 0001 7a11 4275  s....s......z.Bu
+00003050: 696c 6445 6e76 2e69 735f 6d61 636f 7363  ildEnv.is_macosc
+00003060: 0100 0000 0000 0000 0000 0000 0400 0000  ................
+00003070: 0200 0000 4300 0000 7334 0000 0064 0164  ....C...s4...d.d
+00003080: 0284 007d 0164 0364 0484 007d 027c 0183  ...}.d.d...}.|..
+00003090: 007d 037c 0373 207c 0283 007d 037c 0373  .}.|.s |...}.|.s
+000030a0: 2c74 0064 0583 0182 0174 017c 0383 0153  ,t.d.....t.|...S
+000030b0: 0029 067a 5346 696e 6420 7468 6520 7061  .).zSFind the pa
+000030c0: 7468 2074 6f20 7468 6520 636d 616b 6520  th to the cmake 
+000030d0: 6469 7265 6374 6f72 7920 7769 7468 696e  directory within
+000030e0: 2061 0a20 2020 2020 2020 2070 6970 2069   a.        pip i
+000030f0: 6e73 7461 6c6c 6564 2070 7974 6f72 6368  nstalled pytorch
+00003100: 2070 6163 6b61 6765 6300 0000 0000 0000   packagec.......
+00003110: 0000 0000 0004 0000 0008 0000 0053 0000  .............S..
+00003120: 0073 5e00 0000 7a42 6401 6402 6c00 7d00  .s^...zBd.d.l.}.
+00003130: 6403 6404 8400 7c00 6a01 4400 8301 7d01  d.d...|.j.D...}.
+00003140: 7c01 4400 5d1e 7d02 7c02 6405 1b00 7d03  |.D.].}.|.d...}.
+00003150: 7c03 a002 a100 721e 7c03 0200 0100 5700  |.....r.|.....W.
+00003160: 5300 711e 5700 6402 5300 0400 7403 6b0a  S.q.W.d.S...t.k.
+00003170: 7258 0100 0100 0100 5900 6402 5300 5800  rX......Y.d.S.X.
+00003180: 6402 5300 2906 7a1c 4669 6e64 2074 6872  d.S.).z.Find thr
+00003190: 6f75 6768 2069 6d70 6f72 7469 6e67 2074  ough importing t
+000031a0: 6f72 6368 7201 0000 004e 6301 0000 0000  orchr....Nc.....
+000031b0: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+000031c0: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
+000031d0: 7400 7c01 8301 9102 7104 5300 720b 0000  t.|.....q.S.r...
+000031e0: 0072 0200 0000 a902 7211 0000 00da 0170  .r......r......p
+000031f0: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00003200: 6e00 0000 d401 0000 7304 0000 0006 0002  n.......s.......
+00003210: 007a 4942 7569 6c64 456e 762e 746f 7263  .zIBuildEnv.torc
+00003220: 685f 636d 616b 655f 7061 7468 2e3c 6c6f  h_cmake_path.<lo
+00003230: 6361 6c73 3e2e 5f74 6f72 6368 5f69 6d70  cals>._torch_imp
+00003240: 6f72 745f 7061 7468 2e3c 6c6f 6361 6c73  ort_path.<locals
+00003250: 3e2e 3c6c 6973 7463 6f6d 703e 7a11 7368  >.<listcomp>z.sh
+00003260: 6172 652f 636d 616b 652f 546f 7263 6829  are/cmake/Torch)
+00003270: 0472 4000 0000 da08 5f5f 7061 7468 5f5f  .r@.....__path__
+00003280: da06 6973 5f64 6972 da13 4d6f 6475 6c65  ..is_dir..Module
+00003290: 4e6f 7446 6f75 6e64 4572 726f 7229 04da  NotFoundError)..
+000032a0: 0174 5a0b 746f 7263 685f 7061 7468 73da  .tZ.torch_paths.
+000032b0: 055f 7061 7468 da0a 746f 7263 685f 7061  ._path..torch_pa
+000032c0: 7468 720b 0000 0072 0b00 0000 720c 0000  thr....r....r...
+000032d0: 00da 125f 746f 7263 685f 696d 706f 7274  ..._torch_import
+000032e0: 5f70 6174 68cf 0100 0073 1400 0000 0002  _path....s......
+000032f0: 0201 0802 1001 0801 0801 0801 0c01 0601  ................
+00003300: 0e01 7a35 4275 696c 6445 6e76 2e74 6f72  ..z5BuildEnv.tor
+00003310: 6368 5f63 6d61 6b65 5f70 6174 682e 3c6c  ch_cmake_path.<l
+00003320: 6f63 616c 733e 2e5f 746f 7263 685f 696d  ocals>._torch_im
+00003330: 706f 7274 5f70 6174 6863 0000 0000 0000  port_pathc......
+00003340: 0000 0000 0000 0300 0000 0400 0000 5300  ..............S.
+00003350: 0000 7356 0000 0064 0164 0284 0074 00a0  ..sV...d.d...t..
+00003360: 01a1 0044 0083 017d 0074 0274 006a 0383  ...D...}.t.t.j..
+00003370: 01a0 04a1 0072 307c 00a0 0574 0274 006a  .....r0|...t.t.j
+00003380: 0383 01a1 0101 007c 0044 005d 1c7d 017c  .......|.D.].}.|
+00003390: 0164 031b 007d 027c 02a0 04a1 0072 347c  .d...}.|.....r4|
+000033a0: 0202 0001 0053 0071 3464 0453 0029 057a  .....S.q4d.S.).z
+000033b0: 2066 696e 6420 746f 7263 6820 7468 726f   find torch thro
+000033c0: 7567 6820 7369 7465 2070 6163 6b61 6765  ugh site package
+000033d0: 7363 0100 0000 0000 0000 0000 0000 0200  sc..............
+000033e0: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+000033f0: 007c 005d 0c7d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
+00003400: 0453 0072 0b00 0000 7202 0000 0072 a400  .S.r....r....r..
+00003410: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+00003420: 0072 6e00 0000 df01 0000 7304 0000 0006  .rn.......s.....
+00003430: 0002 007a 4742 7569 6c64 456e 762e 746f  ...zGBuildEnv.to
+00003440: 7263 685f 636d 616b 655f 7061 7468 2e3c  rch_cmake_path.<
+00003450: 6c6f 6361 6c73 3e2e 5f74 6f72 6368 5f73  locals>._torch_s
+00003460: 6974 655f 7061 7468 2e3c 6c6f 6361 6c73  ite_path.<locals
+00003470: 3e2e 3c6c 6973 7463 6f6d 703e 7a17 746f  >.<listcomp>z.to
+00003480: 7263 682f 7368 6172 652f 636d 616b 652f  rch/share/cmake/
+00003490: 546f 7263 684e 2906 da04 7369 7465 da0f  TorchN)...site..
+000034a0: 6765 7473 6974 6570 6163 6b61 6765 7372  getsitepackagesr
+000034b0: 0300 0000 da09 5553 4552 5f53 4954 4572  ......USER_SITEr
+000034c0: a700 0000 7269 0000 0029 035a 0a73 6974  ....ri...).Z.sit
+000034d0: 655f 7061 7468 7372 aa00 0000 72ab 0000  e_pathsr....r...
+000034e0: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
+000034f0: da10 5f74 6f72 6368 5f73 6974 655f 7061  .._torch_site_pa
+00003500: 7468 dd01 0000 7310 0000 0000 0212 030e  th....s.........
+00003510: 0110 0208 0108 0108 010a 017a 3342 7569  ...........z3Bui
+00003520: 6c64 456e 762e 746f 7263 685f 636d 616b  ldEnv.torch_cmak
+00003530: 655f 7061 7468 2e3c 6c6f 6361 6c73 3e2e  e_path.<locals>.
+00003540: 5f74 6f72 6368 5f73 6974 655f 7061 7468  _torch_site_path
+00003550: 7a21 436f 756c 6420 6e6f 7420 6c6f 6361  z!Could not loca
+00003560: 7465 2074 6f72 6368 2063 6d61 6b65 2070  te torch cmake p
+00003570: 6174 6829 0272 0600 0000 7210 0000 0029  ath).r....r....)
+00003580: 0472 1800 0000 72ac 0000 0072 b000 0000  .r....r....r....
+00003590: 72ab 0000 0072 0b00 0000 720b 0000 0072  r....r....r....r
+000035a0: 0c00 0000 da10 746f 7263 685f 636d 616b  ......torch_cmak
+000035b0: 655f 7061 7468 ca01 0000 7310 0000 0000  e_path....s.....
+000035c0: 0508 0e08 0e06 0104 0106 0104 0108 017a  ...............z
+000035d0: 1942 7569 6c64 456e 762e 746f 7263 685f  .BuildEnv.torch_
+000035e0: 636d 616b 655f 7061 7468 6300 0000 0000  cmake_pathc.....
+000035f0: 0000 0000 0000 0005 0000 0007 0000 0043  ...............C
+00003600: 0000 0073 bc00 0000 7400 6a01 a002 6401  ...s....t.j...d.
+00003610: 6402 a102 7400 6a01 a002 6403 6402 a102  d...t.j...d.d...
+00003620: 7400 6a01 a002 6404 6402 a102 7400 6a01  t.j...d.d...t.j.
+00003630: a002 6405 6402 a102 6406 9c04 7d00 6401  ..d.d...d...}.d.
+00003640: 6403 6702 7d01 6405 6404 6702 7d02 7403  d.g.}.d.d.g.}.t.
+00003650: 6407 6408 8400 7c01 4400 8301 8301 7d03  d.d...|.D.....}.
+00003660: 7403 6409 6408 8400 7c02 4400 8301 8301  t.d.d...|.D.....
+00003670: 7d04 7c03 7376 7c04 7376 6402 5300 7c03  }.|.sv|.svd.S.|.
+00003680: 7298 7c04 7398 7c00 6403 1900 7c00 6405  r.|.s.|.d...|.d.
+00003690: 3c00 7c00 6401 1900 7c00 6404 3c00 6e20  <.|.d...|.d.<.n 
+000036a0: 7c04 72b8 7c03 73b8 7c00 6405 1900 7c00  |.r.|.s.|.d...|.
+000036b0: 6403 3c00 7c00 6404 1900 7c00 6401 3c00  d.<.|.d...|.d.<.
+000036c0: 7c00 5300 290a 612f 0100 0043 6f6c 6c65  |.S.).a/...Colle
+000036d0: 6374 2074 6865 2065 6e76 6972 6f6e 6d65  ct the environme
+000036e0: 6e74 2076 6172 6961 626c 6573 206e 6565  nt variables nee
+000036f0: 6465 6420 666f 7220 4361 6666 6520 2850  ded for Caffe (P
+00003700: 7974 6f72 6368 290a 2020 2020 2020 2020  ytorch).        
+00003710: 616e 6420 7468 726f 7720 616e 2065 7272  and throw an err
+00003720: 6f72 2069 6620 7468 6579 2061 7265 206e  or if they are n
+00003730: 6f74 2066 6f75 6e64 0a0a 2020 2020 2020  ot found..      
+00003740: 2020 5370 6563 6966 6963 616c 6c79 206d    Specifically m
+00003750: 616b 6520 7375 7265 2074 6f20 7365 7420  ake sure to set 
+00003760: 6174 206c 6561 7374 206f 6e65 2073 6574  at least one set
+00003770: 206f 663a 0a20 2020 2020 2020 2020 2020   of:.           
+00003780: 202d 2043 5544 4e4e 5f4c 4942 5241 5259   - CUDNN_LIBRARY
+00003790: 2061 6e64 2043 5544 4e4e 5f49 4e43 4c55   and CUDNN_INCLU
+000037a0: 4445 5f44 4952 0a20 2020 2020 2020 2020  DE_DIR.         
+000037b0: 2020 2020 2020 206f 720a 2020 2020 2020         or.      
+000037c0: 2020 2020 2020 2d20 4355 444e 4e5f 4c49        - CUDNN_LI
+000037d0: 4252 4152 595f 5041 5448 2061 6e64 2043  BRARY_PATH and C
+000037e0: 5544 4e4e 5f49 4e43 4c55 4445 5f50 4154  UDNN_INCLUDE_PAT
+000037f0: 480a 2020 2020 2020 2020 da0d 4355 444e  H.        ..CUDN
+00003800: 4e5f 4c49 4252 4152 594e da11 4355 444e  N_LIBRARYN..CUDN
+00003810: 4e5f 494e 434c 5544 455f 4449 52da 1243  N_INCLUDE_DIR..C
+00003820: 5544 4e4e 5f4c 4942 5241 5259 5f50 4154  UDNN_LIBRARY_PAT
+00003830: 48da 1243 5544 4e4e 5f49 4e43 4c55 4445  H..CUDNN_INCLUDE
+00003840: 5f50 4154 4829 0472 b200 0000 72b3 0000  _PATH).r....r...
+00003850: 0072 b400 0000 72b5 0000 0063 0100 0000  .r....r....c....
+00003860: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00003870: 5300 0000 7316 0000 0067 007c 005d 0e7d  S...s....g.|.].}
+00003880: 017c 0174 006a 016b 0691 0271 0453 0072  .|.t.j.k...q.S.r
+00003890: 0b00 0000 a902 7234 0000 0072 3500 0000  ......r4...r5...
+000038a0: a902 7211 0000 0072 3700 0000 720b 0000  ..r....r7...r...
+000038b0: 0072 0b00 0000 720c 0000 0072 6e00 0000  .r....r....rn...
+000038c0: 0502 0000 7304 0000 0006 0002 007a 2a42  ....s........z*B
+000038d0: 7569 6c64 456e 762e 6765 745f 6375 646e  uildEnv.get_cudn
+000038e0: 6e5f 656e 762e 3c6c 6f63 616c 733e 2e3c  n_env.<locals>.<
+000038f0: 6c69 7374 636f 6d70 3e63 0100 0000 0000  listcomp>c......
+00003900: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
+00003910: 0000 7316 0000 0067 007c 005d 0e7d 017c  ..s....g.|.].}.|
+00003920: 0174 006a 016b 0691 0271 0453 0072 0b00  .t.j.k...q.S.r..
+00003930: 0000 72b6 0000 0072 b700 0000 720b 0000  ..r....r....r...
+00003940: 0072 0b00 0000 720c 0000 0072 6e00 0000  .r....r....rn...
+00003950: 0602 0000 7304 0000 0006 0002 0029 0472  ....s........).r
+00003960: 3400 0000 7235 0000 0072 3600 0000 da03  4...r5...r6.....
+00003970: 616c 6c29 0572 9600 0000 5a10 746f 7263  all).r....Z.torc
+00003980: 685f 6375 646e 6e5f 7661 7273 5a10 6361  h_cudnn_varsZ.ca
+00003990: 6666 655f 6375 646e 6e5f 7661 7273 5a09  ffe_cudnn_varsZ.
+000039a0: 746f 7263 685f 7365 745a 0963 6166 6665  torch_setZ.caffe
+000039b0: 5f73 6574 720b 0000 0072 0b00 0000 720c  _setr....r....r.
+000039c0: 0000 00da 0d67 6574 5f63 7564 6e6e 5f65  .....get_cudnn_e
+000039d0: 6e76 f201 0000 7324 0000 0000 0b0c 010c  nv....s$........
+000039e0: 010c 010c fc06 0608 0108 0212 0112 0408  ................
+000039f0: 0104 0108 010c 010e 0108 010c 010c 017a  ...............z
+00003a00: 1642 7569 6c64 456e 762e 6765 745f 6375  .BuildEnv.get_cu
+00003a10: 646e 6e5f 656e 7663 0200 0000 0000 0000  dnn_envc........
+00003a20: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
+00003a30: 7346 0000 007a 1c74 006a 017c 0164 0167  sF...z.t.j.|.d.g
+00003a40: 0274 006a 0274 006a 0264 028d 0301 0057  .t.j.t.j.d.....W
+00003a50: 006e 2404 0074 036b 0a72 4001 0001 0001  .n$..t.k.r@.....
+00003a60: 0074 047c 019b 0064 039d 0283 0164 0082  .t.|...d.....d..
+00003a70: 0259 006e 0258 0064 0053 0029 044e 7a09  .Y.n.X.d.S.).Nz.
+00003a80: 2d2d 7665 7273 696f 6e29 02da 0673 7464  --version)...std
+00003a90: 6f75 74da 0673 7464 6572 727a 2420 6d75  out..stderrz$ mu
+00003aa0: 7374 2062 6520 696e 7374 616c 6c65 6420  st be installed 
+00003ab0: 746f 2062 7569 6c64 2053 6d61 7274 5369  to build SmartSi
+00003ac0: 6d29 0572 7700 0000 da0a 6368 6563 6b5f  m).rw.....check_
+00003ad0: 6361 6c6c da07 4445 564e 554c 4cda 074f  call..DEVNULL..O
+00003ae0: 5345 7272 6f72 7206 0000 0029 0272 1800  SErrorr....).r..
+00003af0: 0000 da07 636f 6d6d 616e 6472 0b00 0000  ....commandr....
+00003b00: 720b 0000 0072 0c00 0000 7292 0000 0014  r....r....r.....
+00003b10: 0200 0073 1000 0000 0002 0201 0401 0601  ...s............
+00003b20: 0401 04fd 0a05 0e01 7a1f 4275 696c 6445  ........z.BuildE
+00003b30: 6e76 2e63 6865 636b 5f62 7569 6c64 5f64  nv.check_build_d
+00003b40: 6570 656e 6465 6e63 794e 6302 0000 0000  ependencyNc.....
+00003b50: 0000 0000 0000 0004 0000 0009 0000 0043  ...............C
+00003b60: 0000 0073 8000 0000 7a62 7400 7401 a002  ...s....zbt.t...
+00003b70: 7c00 a101 6a03 8301 7d02 7c01 725e 7c02  |...j...}.|.r^|.
+00003b80: 6a04 7c01 6a04 6b03 732e 7c02 6a05 7c01  j.|.j.k.s.|.j.|.
+00003b90: 6a05 6b03 725e 6401 7c00 9b00 6402 9d03  j.k.r^d.|...d...
+00003ba0: 7c00 9b00 6403 7c01 9b00 6404 7c00 9b00  |...d.|...d.|...
+00003bb0: 6403 7c02 9b00 6405 9d08 1700 7d03 7406  d.|...d.....}.t.
+00003bc0: 7c03 8301 8201 5700 6406 5300 0400 7401  |.....W.d.S...t.
+00003bd0: 6a07 6b0a 727a 0100 0100 0100 5900 6407  j.k.rz......Y.d.
+00003be0: 5300 5800 6408 5300 2909 7a7f 4368 6563  S.X.d.S.).z.Chec
+00003bf0: 6b20 6966 2061 2070 6163 6b61 6765 2069  k if a package i
+00003c00: 7320 696e 7374 616c 6c65 642e 2049 6620  s installed. If 
+00003c10: 7665 7273 696f 6e20 6973 2070 726f 7669  version is provi
+00003c20: 6465 642c 2063 6865 636b 2069 660a 2020  ded, check if.  
+00003c30: 2020 2020 2020 6974 2773 2061 2063 6f6d        it's a com
+00003c40: 7061 7469 626c 6520 7665 7273 696f 6e2e  patible version.
+00003c50: 2028 6d61 6a6f 7220 616e 6420 6d69 6e6f   (major and mino
+00003c60: 7220 7468 6520 7361 6d65 297a 1949 6e63  r the same)z.Inc
+00003c70: 6f6d 7061 7469 626c 6520 7665 7273 696f  ompatible versio
+00003c80: 6e20 666f 7220 7a0b 2064 6574 6563 7465  n for z. detecte
+00003c90: 642e 0afa 0120 7a0f 2072 6571 7565 7374  d.... z. request
+00003ca0: 6564 2062 7574 207a 0b20 696e 7374 616c  ed but z. instal
+00003cb0: 6c65 642e 5446 4e29 0872 0d00 0000 721d  led.TFN).r....r.
+00003cc0: 0000 00da 1067 6574 5f64 6973 7472 6962  .....get_distrib
+00003cd0: 7574 696f 6e72 4d00 0000 7222 0000 0072  utionrM...r"...r
+00003ce0: 2400 0000 7206 0000 00da 1444 6973 7472  $...r......Distr
+00003cf0: 6962 7574 696f 6e4e 6f74 466f 756e 6429  ibutionNotFound)
+00003d00: 04da 0770 6163 6b61 6765 724d 0000 005a  ...packagerM...Z
+00003d10: 0969 6e73 7461 6c6c 6564 da03 6d73 6772  .installed..msgr
+00003d20: 0b00 0000 720b 0000 0072 0c00 0000 da0f  ....r....r......
+00003d30: 6368 6563 6b5f 696e 7374 616c 6c65 641f  check_installed.
+00003d40: 0200 0073 1800 0000 0004 0201 1001 0402  ...s............
+00003d50: 1802 0a01 1aff 02ff 0204 0801 0601 1001  ................
+00003d60: 7a18 4275 696c 6445 6e76 2e63 6865 636b  z.BuildEnv.check
+00003d70: 5f69 6e73 7461 6c6c 6564 2901 5429 014e  _installed).T).N
+00003d80: 2920 7207 0000 0072 0800 0000 7209 0000  ) r....r....r...
+00003d90: 0072 0a00 0000 7234 0000 0072 3500 0000  .r....r4...r5...
+00003da0: 7236 0000 0072 8800 0000 7289 0000 0072  r6...r....r....r
+00003db0: 8a00 0000 728b 0000 0072 8c00 0000 7298  ....r....r....r.
+00003dc0: 0000 0072 1c00 0000 7291 0000 0072 5800  ...r....r....rX.
+00003dd0: 0000 725b 0000 0072 9900 0000 724f 0000  ..r[...r....rO..
+00003de0: 0072 8e00 0000 7297 0000 0072 6c00 0000  .r....r....rl...
+00003df0: 7232 0000 0072 9b00 0000 729e 0000 0072  r2...r....r....r
+00003e00: a200 0000 72a3 0000 0072 b100 0000 da0c  ....r....r......
+00003e10: 7374 6174 6963 6d65 7468 6f64 72b9 0000  staticmethodr...
+00003e20: 0072 9200 0000 72c5 0000 0072 0b00 0000  .r....r....r....
+00003e30: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00003e40: 8700 0000 6b01 0000 7332 0000 0008 0104  ....k...s2......
+00003e50: 120e 010e 010e 010e 030e 010e 0312 0106  ................
+00003e60: 020a 0408 0608 0d08 1802 010a 0308 0608  ................
+00003e70: 0308 0302 010a 2702 010a 2108 0b02 0172  ......'...!....r
+00003e80: 8700 0000 2916 7234 0000 0072 5b00 0000  ....).r4...r[...
+00003e90: 72ad 0000 0072 7700 0000 7258 0000 00da  r....rw...rX....
+00003ea0: 0770 6174 686c 6962 7203 0000 00da 0674  .pathlibr......t
+00003eb0: 7970 696e 6772 0400 0000 721d 0000 0072  ypingr....r....r
+00003ec0: 0500 0000 724d 0000 0072 1500 0000 7217  ....rM...r....r.
+00003ed0: 0000 0072 7b00 0000 7206 0000 0072 1000  ...r{...r....r..
+00003ee0: 0000 720d 0000 0072 3900 0000 723a 0000  ..r....r9...r:..
+00003ef0: 0072 5c00 0000 7287 0000 0072 0b00 0000  .r\...r....r....
+00003f00: 720b 0000 0072 0b00 0000 720c 0000 00da  r....r....r.....
+00003f10: 083c 6d6f 6475 6c65 3e1b 0000 0073 2200  .<module>....s".
+00003f20: 0000 0801 0801 0801 0801 0801 0c01 0c02  ................
+00003f30: 0801 0c02 0801 0808 1012 1041 0804 1056  ...........A...V
+00003f40: 0e7f 0010                                ....
```

### Comparing `smartsim-0.4.1/smartsim/_core/_install/__pycache__/builder.cpython-38.pyc` & `smartsim-0.4.2/smartsim/_core/_install/__pycache__/builder.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Sat Jun 25 00:32:42 2022 UTC, .py size: 16462 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-00000000: 550d 0d0a 0000 0000 aa57 b662 4e40 0000  U........W.bN@..
+00000000: 550d 0d0a 0000 0000 2819 3764 cb48 0000  U.......(.7d.H..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
-00000060: 6402 6c06 6d07 5a07 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
-00000070: 6d08 5a08 0100 6400 6404 6c02 6d09 5a09  m.Z...d.d.l.m.Z.
+00000060: 6402 6c06 6d07 5a07 0100 6400 6403 6c02  d.l.m.Z...d.d.l.
+00000070: 6d08 5a08 0100 6400 6404 6c04 6d09 5a09  m.Z...d.d.l.m.Z.
 00000080: 0100 6405 6406 8400 5a0a 4700 6407 6408  ..d.d...Z.G.d.d.
 00000090: 8400 6408 650b 8303 5a0c 4700 6409 640a  ..d.e...Z.G.d.d.
 000000a0: 8400 640a 8302 5a0d 4700 640b 640c 8400  ..d...Z.G.d.d...
 000000b0: 640c 650d 8303 5a0e 4700 640d 640e 8400  d.e...Z.G.d.d...
 000000c0: 640e 650d 8303 5a0f 6401 5300 290f e900  d.e...Z.d.S.)...
-000000d0: 0000 004e 2901 da04 5061 7468 2901 da0f  ...N)...Path)...
-000000e0: 5375 6270 726f 6365 7373 4572 726f 7229  SubprocessError)
-000000f0: 01da 0577 6869 6368 6301 0000 0000 0000  ...whichc.......
+000000d0: 0000 004e 2901 da04 5061 7468 2901 da05  ...N)...Path)...
+000000e0: 7768 6963 6829 01da 0f53 7562 7072 6f63  which)...Subproc
+000000f0: 6573 7345 7272 6f72 6301 0000 0000 0000  essErrorc.......
 00000100: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
 00000110: 0073 7600 0000 7400 7c00 8301 7d01 7c01  .sv...t.|...}.|.
 00000120: 736a 7401 6a02 a003 7c00 a101 7232 7401  sjt.j...|...r2t.
 00000130: a004 7c00 7401 6a05 a102 7232 7401 6a02  ..|.t.j...r2t.j.
 00000140: a006 7c00 a101 5300 7401 6a02 a003 7c00  ..|...S.t.j...|.
 00000150: a101 725c 7401 a004 7c00 7401 6a05 a102  ..r\t...|.t.j...
 00000160: 735c 7407 6401 7c00 9b00 6402 9d03 8301  s\t.d.|...d.....
@@ -37,36 +37,36 @@
 00000240: 3a72 6169 7365 7320 4669 6c65 4e6f 7446  :raises FileNotF
 00000250: 6f75 6e64 4572 726f 723a 2069 6620 6578  oundError: if ex
 00000260: 6563 7574 6162 6c65 2063 616e 6e6f 7420  ecutable cannot 
 00000270: 6265 2066 6f75 6e64 0a20 2020 207a 0646  be found.    z.F
 00000280: 696c 652c 207a 162c 2069 7320 6e6f 7420  ile, z., is not 
 00000290: 616e 2065 7865 6375 7461 626c 657a 1c43  an executablez.C
 000002a0: 6f75 6c64 206e 6f74 206c 6f63 6174 6520  ould not locate 
-000002b0: 6578 6563 7574 6162 6c65 2029 0972 0400  executable ).r..
+000002b0: 6578 6563 7574 6162 6c65 2029 0972 0300  executable ).r..
 000002c0: 0000 da02 6f73 da04 7061 7468 da06 6973  ....os..path..is
 000002d0: 6669 6c65 da06 6163 6365 7373 da04 585f  file..access..X_
 000002e0: 4f4b da07 6162 7370 6174 68da 0954 7970  OK..abspath..Typ
 000002f0: 6545 7272 6f72 da11 4669 6c65 4e6f 7446  eError..FileNotF
 00000300: 6f75 6e64 4572 726f 7229 025a 0365 7865  oundError).Z.exe
 00000310: 5a07 696e 5f70 6174 68a9 0072 0d00 0000  Z.in_path..r....
 00000320: fa46 2f68 6f6d 652f 7275 6e6e 6572 2f77  .F/home/runner/w
 00000330: 6f72 6b2f 536d 6172 7453 696d 2f53 6d61  ork/SmartSim/Sma
 00000340: 7274 5369 6d2f 736d 6172 7473 696d 2f5f  rtSim/smartsim/_
 00000350: 636f 7265 2f5f 696e 7374 616c 6c2f 6275  core/_install/bu
 00000360: 696c 6465 722e 7079 da0f 6578 7061 6e64  ilder.py..expand
-00000370: 5f65 7865 5f70 6174 6813 0000 0073 1000  _exe_path....s..
+00000370: 5f65 7865 5f70 6174 682d 0000 0073 1000  _exe_path-...s..
 00000380: 0000 000a 0801 0401 1a01 0c01 1a01 1001  ................
 00000390: 0e01 720f 0000 0063 0000 0000 0000 0000  ..r....c........
 000003a0: 0000 0000 0000 0000 0100 0000 4000 0000  ............@...
 000003b0: 730c 0000 0065 005a 0164 005a 0264 0153  s....e.Z.d.Z.d.S
 000003c0: 0029 02da 0a42 7569 6c64 4572 726f 724e  .)...BuildErrorN
 000003d0: 2903 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000003e0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
 000003f0: 6e61 6d65 5f5f 720d 0000 0072 0d00 0000  name__r....r....
-00000400: 720d 0000 0072 0e00 0000 7210 0000 0026  r....r....r....&
+00000400: 720d 0000 0072 0e00 0000 7210 0000 0041  r....r....r....A
 00000410: 0000 0073 0200 0000 0801 7210 0000 0063  ...s......r....c
 00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000430: 0400 0000 4000 0000 7372 0000 0065 005a  ....@...sr...e.Z
 00000440: 0164 005a 0264 015a 0365 04a0 0564 0265  .d.Z.d.Z.e...d.e
 00000450: 046a 06a1 025a 0764 1864 0564 0684 015a  .j...Z.d.d.d...Z
 00000460: 0865 0964 0764 0884 0083 015a 0a64 0964  .e.d.d.....Z.d.d
 00000470: 0a84 005a 0b64 0b64 0c84 005a 0c64 1964  ...Z.d.d...Z.d.d
@@ -114,59 +114,59 @@
 00000710: 554c 4cda 036f 7574 da07 7665 7262 6f73  ULL..out..verbos
 00000720: 65da 0669 735f 6469 72da 056d 6b64 6972  e..is_dir..mkdir
 00000730: da04 6a6f 6273 2906 da04 7365 6c66 7218  ..jobs)...selfr.
 00000740: 0000 0072 2600 0000 7223 0000 005a 095f  ...r&...r#...Z._
 00000750: 636f 7265 5f64 6972 da0f 6465 7065 6e64  core_dir..depend
 00000760: 656e 6379 5f70 6174 6872 0d00 0000 720d  ency_pathr....r.
 00000770: 0000 0072 0e00 0000 da08 5f5f 696e 6974  ...r......__init
-00000780: 5f5f 3700 0000 7328 0000 0000 0306 0314  __7...s(........
+00000780: 5f5f 5200 0000 7328 0000 0000 0306 0314  __R...s(........
 00000790: 0204 010a 010e 020a 020a 010a 0308 0106  ................
 000007a0: 0106 0106 030a 010a 0108 010a 010a 010a  ................
 000007b0: 010a 027a 1042 7569 6c64 6572 2e5f 5f69  ...z.Builder.__i
 000007c0: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
 000007d0: 0000 0100 0000 0100 0000 4300 0000 7308  ..........C...s.
 000007e0: 0000 0074 0082 0164 0053 00a9 014e a901  ...t...d.S...N..
 000007f0: da13 4e6f 7449 6d70 6c65 6d65 6e74 6564  ..NotImplemented
 00000800: 4572 726f 72a9 0172 2700 0000 720d 0000  Error..r'...r...
 00000810: 0072 0d00 0000 720e 0000 00da 0869 735f  .r....r......is_
-00000820: 6275 696c 745a 0000 0073 0200 0000 0002  builtZ...s......
+00000820: 6275 696c 7475 0000 0073 0200 0000 0002  builtu...s......
 00000830: 7a10 4275 696c 6465 722e 6973 5f62 7569  z.Builder.is_bui
 00000840: 6c74 6301 0000 0000 0000 0000 0000 0001  ltc.............
 00000850: 0000 0001 0000 0043 0000 0073 0800 0000  .......C...s....
 00000860: 7400 8201 6400 5300 722a 0000 0072 2b00  t...d.S.r*...r+.
 00000870: 0000 722d 0000 0072 0d00 0000 720d 0000  ..r-...r....r...
 00000880: 0072 0e00 0000 da0e 6275 696c 645f 6672  .r......build_fr
-00000890: 6f6d 5f67 6974 5e00 0000 7302 0000 0000  om_git^...s.....
+00000890: 6f6d 5f67 6974 7900 0000 7302 0000 0000  om_gity...s.....
 000008a0: 017a 1642 7569 6c64 6572 2e62 7569 6c64  .z.Builder.build
 000008b0: 5f66 726f 6d5f 6769 7463 0200 0000 0000  _from_gitc......
 000008c0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
 000008d0: 0000 7324 0000 0074 00a0 017c 01a1 017d  ..s$...t...|...}
 000008e0: 027c 0272 127c 0253 0074 027c 019b 0064  .|.r.|.S.t.|...d
 000008f0: 019d 0283 0182 0164 0053 0029 024e 7a12  .......d.S.).Nz.
 00000900: 206e 6f74 2066 6f75 6e64 2069 6e20 5041   not found in PA
-00000910: 5448 2903 da06 7368 7574 696c 7204 0000  TH)...shutilr...
+00000910: 5448 2903 da06 7368 7574 696c 7203 0000  TH)...shutilr...
 00000920: 0072 1000 0000 2903 7227 0000 00da 0662  .r....).r'.....b
 00000930: 696e 6172 795a 0762 696e 6172 795f 720d  inaryZ.binary_r.
 00000940: 0000 0072 0d00 0000 720e 0000 00da 0b62  ...r....r......b
-00000950: 696e 6172 795f 7061 7468 6100 0000 7308  inary_patha...s.
+00000950: 696e 6172 795f 7061 7468 7c00 0000 7308  inary_path|...s.
 00000960: 0000 0000 010a 0104 0104 017a 1342 7569  ...........z.Bui
 00000970: 6c64 6572 2e62 696e 6172 795f 7061 7468  lder.binary_path
 00000980: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
 00000990: 0004 0000 0043 0000 0073 3000 0000 7400  .....C...s0...t.
 000009a0: a001 7c01 7c02 a102 0100 7c03 722c 7402  ..|.|.....|.r,t.
 000009b0: 7c02 8301 a003 7404 6a05 7404 6a06 4200  |.....t.j.t.j.B.
 000009c0: 7404 6a07 4200 a101 0100 6400 5300 722a  t.j.B.....d.S.r*
 000009d0: 0000 0029 0872 3000 0000 da08 636f 7079  ...).r0.....copy
 000009e0: 6669 6c65 7202 0000 00da 0563 686d 6f64  filer......chmod
 000009f0: da04 7374 6174 da07 535f 4958 5553 52da  ..stat..S_IXUSR.
 00000a00: 0753 5f49 5755 5352 da07 535f 4952 5553  .S_IWUSR..S_IRUS
 00000a10: 5229 0472 2700 0000 da03 7372 63da 0364  R).r'.....src..d
 00000a20: 7374 da07 7365 745f 6578 6572 0d00 0000  st..set_exer....
 00000a30: 720d 0000 0072 0e00 0000 da09 636f 7079  r....r......copy
-00000a40: 5f66 696c 6567 0000 0073 0600 0000 0001  _fileg...s......
+00000a40: 5f66 696c 6582 0000 0073 0600 0000 0001  _file....s......
 00000a50: 0c01 0401 7a11 4275 696c 6465 722e 636f  ....z.Builder.co
 00000a60: 7079 5f66 696c 6563 0400 0000 0000 0000  py_filec........
 00000a70: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
 00000a80: 7366 0000 0074 007c 0183 017d 0174 007c  sf...t.|...}.t.|
 00000a90: 0283 017d 027c 026a 0164 0164 028d 0101  ...}.|.j.d.d....
 00000aa0: 007c 01a0 0264 03a1 0144 005d 3a7d 047c  .|...d...D.]:}.|
 00000ab0: 04a0 03a1 0072 4a7c 006a 047c 047c 027c  .....rJ|.j.|.|.|
@@ -176,35 +176,35 @@
 00000af0: 01da 0865 7869 7374 5f6f 6bda 012a a901  ...exist_ok..*..
 00000b00: 723b 0000 0029 0772 0200 0000 7225 0000  r;...).r....r%..
 00000b10: 00da 0467 6c6f 6272 2400 0000 da08 636f  ...globr$.....co
 00000b20: 7079 5f64 6972 da04 6e61 6d65 723c 0000  py_dir..namer<..
 00000b30: 0029 0572 2700 0000 7239 0000 0072 3a00  .).r'...r9...r:.
 00000b40: 0000 723b 0000 00da 0763 6f6e 7465 6e74  ..r;.....content
 00000b50: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
-00000b60: 4100 0000 6c00 0000 730e 0000 0000 0108  A...l...s.......
+00000b60: 4100 0000 8700 0000 730e 0000 0000 0108  A.......s.......
 00000b70: 0108 010c 020e 0108 0118 027a 1042 7569  ...........z.Bui
 00000b80: 6c64 6572 2e63 6f70 795f 6469 7263 0200  lder.copy_dirc..
 00000b90: 0000 0000 0000 0000 0000 0200 0000 0400  ................
 00000ba0: 0000 4300 0000 7312 0000 0074 00a0 017c  ..C...s....t...|
 00000bb0: 006a 027c 01a1 0264 006b 0953 0072 2a00  .j.|...d.k.S.r*.
 00000bc0: 0000 2903 da02 7265 da05 6d61 7463 68da  ..)...re..match.
 00000bd0: 0975 726c 5f72 6567 6578 2902 7227 0000  .url_regex).r'..
 00000be0: 00da 0375 726c 720d 0000 0072 0d00 0000  ...urlr....r....
 00000bf0: 720e 0000 00da 0c69 735f 7661 6c69 645f  r......is_valid_
-00000c00: 7572 6c77 0000 0073 0200 0000 0001 7a14  urlw...s......z.
+00000c00: 7572 6c92 0000 0073 0200 0000 0001 7a14  url....s......z.
 00000c10: 4275 696c 6465 722e 6973 5f76 616c 6964  Builder.is_valid
 00000c20: 5f75 726c 6301 0000 0000 0000 0000 0000  _urlc...........
 00000c30: 0001 0000 0004 0000 0043 0000 0073 1e00  .........C...s..
 00000c40: 0000 7c00 6a00 a001 a100 721a 7402 a003  ..|.j.....r.t...
 00000c50: 7404 7c00 6a00 8301 a101 0100 6400 5300  t.|.j.......d.S.
 00000c60: 722a 0000 0029 0572 1d00 0000 7224 0000  r*...).r....r$..
 00000c70: 0072 3000 0000 da06 726d 7472 6565 da03  .r0.....rmtree..
 00000c80: 7374 7272 2d00 0000 720d 0000 0072 0d00  strr-...r....r..
 00000c90: 0000 720e 0000 00da 0763 6c65 616e 7570  ..r......cleanup
-00000ca0: 7a00 0000 7304 0000 0000 010a 017a 0f42  z...s........z.B
+00000ca0: 9500 0000 7304 0000 0000 010a 017a 0f42  ....s........z.B
 00000cb0: 7569 6c64 6572 2e63 6c65 616e 7570 4e63  uilder.cleanupNc
 00000cc0: 0500 0000 0000 0000 0000 0000 0800 0000  ................
 00000cd0: 0a00 0000 4300 0000 7380 0000 007c 0373  ....C...s....|.s
 00000ce0: 0a7c 006a 007d 037a 4274 016a 027c 0174  .|.j.}.zBt.j.|.t
 00000cf0: 016a 037c 037c 047c 027c 006a 0464 018d  .j.|.|.|.|.j.d..
 00000d00: 067d 057c 05a0 05a1 0064 0219 00a0 0664  .}.|.....d.....d
 00000d10: 03a1 017d 067c 056a 0764 046b 0372 4a74  ...}.|.j.d.k.rJt
@@ -216,33 +216,33 @@
 00000d70: 7574 da03 6377 64da 0573 6865 6c6c 7218  ut..cwd..shellr.
 00000d80: 0000 0072 1500 0000 7a05 7574 662d 3872  ...r....z.utf-8r
 00000d90: 0100 0000 290b 7222 0000 0072 2000 0000  ....).r"...r ...
 00000da0: da05 506f 7065 6eda 0450 4950 4572 1800  ..Popen..PIPEr..
 00000db0: 0000 da0b 636f 6d6d 756e 6963 6174 65da  ....communicate.
 00000dc0: 0664 6563 6f64 65da 0a72 6574 7572 6e63  .decode..returnc
 00000dd0: 6f64 6572 1000 0000 da07 4f53 4572 726f  oder......OSErro
-00000de0: 7272 0300 0000 2908 7227 0000 00da 0363  rr....).r'.....c
+00000de0: 7272 0400 0000 2908 7227 0000 00da 0363  rr....).r'.....c
 00000df0: 6d64 724f 0000 0072 2200 0000 724e 0000  mdrO...r"...rN..
 00000e00: 00da 0470 726f 63da 0565 7272 6f72 da01  ...proc..error..
 00000e10: 6572 0d00 0000 720d 0000 0072 0e00 0000  er....r....r....
-00000e20: da0b 7275 6e5f 636f 6d6d 616e 647e 0000  ..run_command~..
+00000e20: da0b 7275 6e5f 636f 6d6d 616e 6499 0000  ..run_command...
 00000e30: 0073 2000 0000 0002 0401 0601 0201 0401  .s .............
 00000e40: 0201 0401 0201 0201 0201 04fa 0608 1201  ................
 00000e50: 0a01 0c01 1401 7a13 4275 696c 6465 722e  ......z.Builder.
 00000e60: 7275 6e5f 636f 6d6d 616e 6429 0272 1500  run_command).r..
 00000e70: 0000 4629 0146 2901 4629 0346 4e4e 2912  ..F).F).F).FNN).
 00000e80: 7211 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
 00000e90: 075f 5f64 6f63 5f5f 7244 0000 00da 0763  .__doc__rD.....c
 00000ea0: 6f6d 7069 6c65 da0a 4947 4e4f 5245 4341  ompile..IGNORECA
 00000eb0: 5345 7246 0000 0072 2900 0000 da08 7072  SErF...r).....pr
 00000ec0: 6f70 6572 7479 722e 0000 0072 2f00 0000  opertyr....r/...
 00000ed0: 7232 0000 0072 3c00 0000 7241 0000 0072  r2...r<...rA...r
 00000ee0: 4800 0000 724b 0000 0072 5a00 0000 720d  H...rK...rZ...r.
 00000ef0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000f00: 0000 7214 0000 002a 0000 0073 1e00 0000  ..r....*...s....
+00000f00: 0000 7214 0000 0045 0000 0073 1e00 0000  ..r....E...s....
 00000f10: 0801 0402 0401 0206 04f9 040a 0a23 0201  .............#..
 00000f20: 0a03 0803 0806 0a05 0a0b 0803 0804 7214  ..............r.
 00000f30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 00000f40: 0000 0000 0400 0000 0000 0000 733e 0000  ............s>..
 00000f50: 0065 005a 0164 005a 0264 015a 0369 0064  .e.Z.d.Z.d.Z.i.d
 00000f60: 0264 0364 0466 0487 0066 0164 0564 0684  .d.d.f...f.d.d..
 00000f70: 095a 0465 0564 0764 0884 0083 015a 0664  .Z.e.d.d.....Z.d
@@ -265,15 +265,15 @@
 00001080: 017c 037c 0464 018d 0301 007c 027c 005f  .|.|.d.....|.|._
 00001090: 0264 0053 0029 024e a902 7226 0000 0072  .d.S.).N..r&...r
 000010a0: 2300 0000 2903 da05 7375 7065 7272 2900  #...)...superr).
 000010b0: 0000 da06 6d61 6c6c 6f63 2905 7227 0000  ....malloc).r'..
 000010c0: 00da 0962 7569 6c64 5f65 6e76 7263 0000  ...build_envrc..
 000010d0: 0072 2600 0000 7223 0000 00a9 01da 095f  .r&...r#......._
 000010e0: 5f63 6c61 7373 5f5f 720d 0000 0072 0e00  _class__r....r..
-000010f0: 0000 7229 0000 009a 0000 0073 0400 0000  ..r).......s....
+000010f0: 0000 7229 0000 00b5 0000 0073 0400 0000  ..r).......s....
 00001100: 0001 1201 7a18 4461 7461 6261 7365 4275  ....z.DatabaseBu
 00001110: 696c 6465 722e 5f5f 696e 6974 5f5f 6301  ilder.__init__c.
 00001120: 0000 0000 0000 0000 0000 0004 0000 0003  ................
 00001130: 0000 0043 0000 0073 3800 0000 6401 6402  ...C...s8...d.d.
 00001140: 8400 7c00 6a00 a001 a100 4400 8301 7d01  ..|.j.....D...}.
 00001150: 6403 6404 6802 7d02 6405 6406 6802 7d03  d.d.h.}.d.d.h.}.
 00001160: 7c02 a002 7c01 a101 7036 7c03 a002 7c01  |...|...p6|...|.
@@ -281,28 +281,28 @@
 00001180: 2052 6564 6973 206f 7220 4b65 7944 4220   Redis or KeyDB 
 00001190: 6973 2062 7569 6c74 6301 0000 0000 0000  is builtc.......
 000011a0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
 000011b0: 0073 1200 0000 6800 7c00 5d0a 7d01 7c01  .s....h.|.].}.|.
 000011c0: 6a00 9202 7104 5300 720d 0000 0029 0172  j...q.S.r....).r
 000011d0: 4200 0000 2902 da02 2e30 da04 6669 6c65  B...)....0..file
 000011e0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
-000011f0: 093c 7365 7463 6f6d 703e a100 0000 7304  .<setcomp>....s.
+000011f0: 093c 7365 7463 6f6d 703e bc00 0000 7304  .<setcomp>....s.
 00001200: 0000 0006 0002 007a 2b44 6174 6162 6173  .......z+Databas
 00001210: 6542 7569 6c64 6572 2e69 735f 6275 696c  eBuilder.is_buil
 00001220: 742e 3c6c 6f63 616c 733e 2e3c 7365 7463  t.<locals>.<setc
 00001230: 6f6d 703e 7a0c 7265 6469 732d 7365 7276  omp>z.redis-serv
 00001240: 6572 7a09 7265 6469 732d 636c 697a 0c6b  erz.redis-cliz.k
 00001250: 6579 6462 2d73 6572 7665 727a 096b 6579  eydb-serverz.key
 00001260: 6462 2d63 6c69 2903 721e 0000 00da 0769  db-cli).r......i
 00001270: 7465 7264 6972 da08 6973 7375 6273 6574  terdir..issubset
 00001280: 2904 7227 0000 005a 0962 696e 5f66 696c  ).r'...Z.bin_fil
 00001290: 6573 5a0b 7265 6469 735f 6669 6c65 735a  esZ.redis_filesZ
 000012a0: 0b6b 6579 6462 5f66 696c 6573 720d 0000  .keydb_filesr...
 000012b0: 0072 0d00 0000 720e 0000 0072 2e00 0000  .r....r....r....
-000012c0: 9e00 0000 7308 0000 0000 0314 0108 0108  ....s...........
+000012c0: b900 0000 7308 0000 0000 0314 0108 0108  ....s...........
 000012d0: 017a 1844 6174 6162 6173 6542 7569 6c64  .z.DatabaseBuild
 000012e0: 6572 2e69 735f 6275 696c 7463 0300 0000  er.is_builtc....
 000012f0: 0000 0000 0000 0000 1700 0000 0a00 0000  ................
 00001300: 4300 0000 734e 0200 0064 017c 016b 0672  C...sN...d.|.k.r
 00001310: 0c64 026e 0264 037d 0374 007c 006a 017c  .d.n.d.}.t.|.j.|
 00001320: 03a0 02a1 0083 027d 0474 007c 006a 0164  .......}.t.|.j.d
 00001330: 0383 027d 0574 007c 006a 0164 0283 027d  ...}.t.|.j.d...}
@@ -327,21 +327,21 @@
 00001460: 016a 136a 137d 0e74 0f6a 14a0 1564 147c  .j.j.}.t.j...d.|
 00001470: 0ea1 027d 0f74 007c 0f64 1583 02a0 16a1  ...}.t.|.d......
 00001480: 007d 107a 3474 177c 10a0 1864 16a1 0183  .}.z4t.|...d....
 00001490: 017d 1174 0074 0f6a 14a0 1564 177c 11a1  .}.t.t.j...d.|..
 000014a0: 0283 01a0 16a1 007d 1274 1974 067c 1283  .......}.t.t.|..
 000014b0: 0183 017d 1357 006e 3204 0074 1a74 1b66  ...}.W.n2..t.t.f
 000014c0: 026b 0a90 0172 e001 007d 1401 007a 0e74  .k...r...}...z.t
-000014d0: 1c64 1883 017c 1482 0257 0035 0064 197d  .d...|...W.5.d.}
+000014d0: 0864 1883 017c 1482 0257 0035 0064 197d  .d...|...W.5.d.}
 000014e0: 147e 1458 0059 006e 0258 007a 3474 177c  .~.X.Y.n.X.z4t.|
 000014f0: 10a0 1864 1aa1 0183 017d 1574 0074 0f6a  ...d.....}.t.t.j
 00001500: 14a0 1564 1b7c 15a1 0283 01a0 16a1 007d  ...d.|.........}
 00001510: 1674 1974 067c 1683 0183 017d 1357 006e  .t.t.|.....}.W.n
 00001520: 3204 0074 1a74 1b66 026b 0a90 0272 4801  2..t.t.f.k...rH.
-00001530: 007d 1401 007a 0e74 1c64 1c83 017c 1482  .}...z.t.d...|..
+00001530: 007d 1401 007a 0e74 0864 1c83 017c 1482  .}...z.t.d...|..
 00001540: 0257 0035 0064 197d 147e 1458 0059 006e  .W.5.d.}.~.X.Y.n
 00001550: 0258 0064 1953 0029 1d7a b542 7569 6c64  .X.d.S.).z.Build
 00001560: 2052 6564 6973 2066 726f 6d20 6769 740a   Redis from git.
 00001570: 2020 2020 2020 2020 3a70 6172 616d 2067          :param g
 00001580: 6974 5f75 726c 3a20 7572 6c20 6672 6f6d  it_url: url from
 00001590: 2077 6869 6368 2074 6f20 7265 7472 6965   which to retrie
 000015a0: 7665 2052 6564 6973 0a20 2020 2020 2020  ve Redis.       
@@ -364,375 +364,394 @@
 000016b0: 082a 2d73 6572 7665 725a 0a52 4544 4953  .*-serverZ.REDIS
 000016c0: 5f50 4154 487a 2449 6e73 7461 6c6c 6174  _PATHz$Installat
 000016d0: 696f 6e20 6f66 2072 6564 6973 2d73 6572  ion of redis-ser
 000016e0: 7665 7220 6661 696c 6564 214e 7a05 2a2d  ver failed!Nz.*-
 000016f0: 636c 695a 0e52 4544 4953 5f43 4c49 5f50  cliZ.REDIS_CLI_P
 00001700: 4154 487a 2149 6e73 7461 6c6c 6174 696f  ATHz!Installatio
 00001710: 6e20 6f66 2072 6564 6973 2d63 6c69 2066  n of redis-cli f
-00001720: 6169 6c65 6421 291d 7202 0000 0072 1d00  ailed!).r....r..
+00001720: 6169 6c65 6421 291c 7202 0000 0072 1d00  ailed!).r....r..
 00001730: 0000 da05 6c6f 7765 7272 2400 0000 7230  ....lowerr$...r0
 00001740: 0000 0072 4900 0000 724a 0000 0072 4800  ...rI...rJ...rH.
 00001750: 0000 7210 0000 0072 3200 0000 725a 0000  ..r....r2...rZ..
 00001760: 0072 2600 0000 7263 0000 0072 1e00 0000  .r&...rc...r....
 00001770: 723c 0000 0072 0500 0000 7206 0000 0072  r<...r....r....r
 00001780: 0a00 0000 7219 0000 0072 1a00 0000 721c  ....r....r....r.
 00001790: 0000 00da 0367 6574 da07 7265 736f 6c76  .....get..resolv
 000017a0: 65da 046e 6578 7472 4000 0000 720f 0000  e..nextr@...r...
-000017b0: 0072 0b00 0000 720c 0000 005a 0d53 5343  .r....r....Z.SSC
-000017c0: 6f6e 6669 6745 7272 6f72 2917 7227 0000  onfigError).r'..
-000017d0: 00da 0767 6974 5f75 726c da06 6272 616e  ...git_url..bran
-000017e0: 6368 5a0d 6461 7461 6261 7365 5f6e 616d  chZ.database_nam
-000017f0: 655a 1364 6174 6162 6173 655f 6275 696c  eZ.database_buil
-00001800: 645f 7061 7468 5a10 7265 6469 735f 6275  d_pathZ.redis_bu
-00001810: 696c 645f 7061 7468 5a10 6b65 7964 625f  ild_pathZ.keydb_
-00001820: 6275 696c 645f 7061 7468 da09 636c 6f6e  build_path..clon
-00001830: 655f 636d 64da 0962 7569 6c64 5f63 6d64  e_cmd..build_cmd
-00001840: 5a10 6461 7461 6261 7365 5f73 7263 5f64  Z.database_src_d
-00001850: 6972 5a0d 7365 7276 6572 5f73 6f75 7263  irZ.server_sourc
-00001860: 655a 1273 6572 7665 725f 6465 7374 696e  eZ.server_destin
-00001870: 6174 696f 6e5a 0a63 6c69 5f73 6f75 7263  ationZ.cli_sourc
-00001880: 655a 0f63 6c69 5f64 6573 7469 6e61 7469  eZ.cli_destinati
-00001890: 6f6e 5a09 636f 7265 5f70 6174 6872 2800  onZ.core_pathr(.
-000018a0: 0000 721e 0000 005a 0c64 6174 6162 6173  ..r....Z.databas
-000018b0: 655f 6578 655a 0864 6174 6162 6173 65da  e_exeZ.database.
-000018c0: 015f 7259 0000 005a 0d72 6564 6973 5f63  ._rY...Z.redis_c
-000018d0: 6c69 5f65 7865 5a09 7265 6469 735f 636c  li_exeZ.redis_cl
-000018e0: 6972 0d00 0000 720d 0000 0072 0e00 0000  ir....r....r....
-000018f0: 722f 0000 00a6 0000 0073 6000 0000 0007  r/.......s`.....
-00001900: 1001 1004 0c01 0c01 0801 0e01 0801 0e03  ................
-00001910: 0a01 1404 0801 0201 0201 0201 0201 0201  ................
-00001920: 0201 02f8 040a 1004 0801 0201 0801 0afc  ................
-00001930: 0406 1203 0801 1001 1201 1001 1201 1001  ................
-00001940: 1003 1401 0e01 0e01 0201 0e01 1601 1001  ................
-00001950: 1601 1c03 0201 0e01 1601 1001 1601 7a1e  ..............z.
-00001960: 4461 7461 6261 7365 4275 696c 6465 722e  DatabaseBuilder.
-00001970: 6275 696c 645f 6672 6f6d 5f67 6974 2909  build_from_git).
-00001980: 7211 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-00001990: 5b00 0000 7229 0000 0072 5e00 0000 722e  [...r)...r^...r.
-000019a0: 0000 0072 2f00 0000 da0d 5f5f 636c 6173  ...r/.....__clas
-000019b0: 7363 656c 6c5f 5f72 0d00 0000 720d 0000  scell__r....r...
-000019c0: 0072 6500 0000 720e 0000 0072 5f00 0000  .re...r....r_...
-000019d0: 9200 0000 730a 0000 0008 0104 0716 0402  ....s...........
-000019e0: 010a 0772 5f00 0000 6300 0000 0000 0000  ...r_...c.......
-000019f0: 0000 0000 0000 0000 0008 0000 0000 0000  ................
-00001a00: 0073 6600 0000 6500 5a01 6400 5a02 6401  .sf...e.Z.d.Z.d.
-00001a10: 5a03 6900 6402 6402 6403 6403 6404 6405  Z.i.d.d.d.d.d.d.
-00001a20: 6404 6608 8700 6601 6406 6407 8409 5a04  d.f...f.d.d...Z.
-00001a30: 6505 6408 6409 8400 8301 5a06 640a 640b  e.d.d.....Z.d.d.
-00001a40: 8400 5a07 640c 640d 8400 5a08 640e 640f  ..Z.d.d...Z.d.d.
-00001a50: 8400 5a09 6410 6411 8400 5a0a 6412 6413  ..Z.d.d...Z.d.d.
-00001a60: 8400 5a0b 8700 0400 5a0c 5300 2914 da0e  ..Z.....Z.S.)...
-00001a70: 5265 6469 7341 4942 7569 6c64 6572 7aa3  RedisAIBuilderz.
-00001a80: 436c 6173 7320 746f 2062 7569 6c64 2052  Class to build R
-00001a90: 6564 6973 4149 2066 726f 6d20 536f 7572  edisAI from Sour
-00001aa0: 6365 0a20 2020 2053 7570 706f 7274 6564  ce.    Supported
-00001ab0: 2062 7569 6c64 206d 6574 686f 643a 0a20   build method:. 
-00001ac0: 2020 2020 2d20 6672 6f6d 2067 6974 0a20      - from git. 
-00001ad0: 2020 2053 6565 2062 7569 6c64 656e 762e     See buildenv.
-00001ae0: 7079 2066 6f72 2062 7569 6c64 7469 6d65  py for buildtime
-00001af0: 2063 6f6e 6669 6775 7261 7469 6f6e 206f   configuration o
-00001b00: 6620 5265 6469 7341 490a 2020 2020 7665  f RedisAI.    ve
-00001b10: 7273 696f 6e20 616e 6420 7572 6c2e 0a20  rsion and url.. 
-00001b20: 2020 20da 0054 464e 6309 0000 0000 0000     ..TFNc.......
-00001b30: 0000 0000 0009 0000 0005 0000 0003 0000  ................
-00001b40: 0073 5a00 0000 7400 8300 6a01 7c01 7c07  .sZ...t...j.|.|.
-00001b50: 7c08 6401 8d03 0100 7402 7c00 6a03 6402  |.d.....t.|.j.d.
-00001b60: 8302 7c00 5f04 7c04 7228 6403 6e02 6404  ..|._.|.r(d.n.d.
-00001b70: 7c00 5f05 7c05 7236 6403 6e02 6404 7c00  |._.|.r6d.n.d.|.
-00001b80: 5f06 7c06 7244 6403 6e02 6404 7c00 5f07  _.|.rDd.n.d.|._.
-00001b90: 7c03 7c00 5f08 7c02 7c00 5f09 6400 5300  |.|._.|.|._.d.S.
-00001ba0: 2905 4e72 6100 0000 da07 5265 6469 7341  ).Nra.....RedisA
-00001bb0: 4972 1500 0000 7201 0000 0029 0a72 6200  Ir....r....).rb.
-00001bc0: 0000 7229 0000 0072 0200 0000 721d 0000  ..r)...r....r...
-00001bd0: 00da 0e72 6169 5f62 7569 6c64 5f70 6174  ...rai_build_pat
-00001be0: 68da 0574 6f72 6368 da02 7466 da04 6f6e  h..torch..tf..on
-00001bf0: 6e78 da09 6c69 6274 665f 6469 72da 0974  nx..libtf_dir..t
-00001c00: 6f72 6368 5f64 6972 2909 7227 0000 0072  orch_dir).r'...r
-00001c10: 6400 0000 7285 0000 0072 8400 0000 5a0b  d...r....r....Z.
-00001c20: 6275 696c 645f 746f 7263 685a 0862 7569  build_torchZ.bui
-00001c30: 6c64 5f74 665a 0a62 7569 6c64 5f6f 6e6e  ld_tfZ.build_onn
-00001c40: 7872 2600 0000 7223 0000 0072 6500 0000  xr&...r#...re...
-00001c50: 720d 0000 0072 0e00 0000 7229 0000 00f7  r....r....r)....
-00001c60: 0000 0073 0e00 0000 000b 1201 0e03 0e01  ...s............
-00001c70: 0e01 0e01 0601 7a17 5265 6469 7341 4942  ......z.RedisAIB
-00001c80: 7569 6c64 6572 2e5f 5f69 6e69 745f 5f63  uilder.__init__c
-00001c90: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00001ca0: 0300 0000 4300 0000 7328 0000 007c 006a  ....C...s(...|.j
-00001cb0: 00a0 0164 01a1 01a0 02a1 007d 017c 006a  ...d.......}.|.j
-00001cc0: 00a0 0164 02a1 01a0 03a1 007d 027c 016f  ...d.......}.|.o
-00001cd0: 267c 0253 0029 034e da08 6261 636b 656e  &|.S.).N..backen
-00001ce0: 6473 fa0a 7265 6469 7361 692e 736f 2904  ds..redisai.so).
-00001cf0: 721f 0000 00da 086a 6f69 6e70 6174 6872  r......joinpathr
-00001d00: 2400 0000 da07 6973 5f66 696c 6529 0372  $.....is_file).r
-00001d10: 2700 0000 da06 7365 7276 6572 da03 636c  '.....server..cl
-00001d20: 6972 0d00 0000 720d 0000 0072 0e00 0000  ir....r....r....
-00001d30: 722e 0000 000c 0100 0073 0600 0000 0002  r........s......
-00001d40: 1001 1001 7a17 5265 6469 7341 4942 7569  ....z.RedisAIBui
-00001d50: 6c64 6572 2e69 735f 6275 696c 7463 0100  lder.is_builtc..
-00001d60: 0000 0000 0000 0000 0000 0200 0000 0500  ................
-00001d70: 0000 4300 0000 733c 0000 007c 006a 0064  ..C...s<...|.j.d
-00001d80: 011b 007d 017c 01a0 01a1 0001 007c 01a0  ...}.|.......|..
-00001d90: 02a1 0072 387c 01a0 03a1 0001 007c 006a  ...r8|.......|.j
-00001da0: 047c 006a 0564 021b 007c 0164 0364 048d  .|.j.d...|.d.d..
-00001db0: 0301 0064 0553 0029 067a be43 6f70 7920  ...d.S.).z.Copy 
-00001dc0: 7468 6520 4669 6e64 5465 6e73 6f72 466c  the FindTensorFl
-00001dd0: 6f77 2e63 6d61 6b65 2066 696c 6520 746f  ow.cmake file to
-00001de0: 2074 6865 2062 7569 6c64 2064 6972 6563   the build direc
-00001df0: 746f 7279 0a20 2020 2020 2020 2061 7320  tory.        as 
-00001e00: 7468 6520 7665 7273 696f 6e20 696e 636c  the version incl
-00001e10: 7564 6564 2069 6e20 5265 6469 7341 4920  uded in RedisAI 
-00001e20: 6973 206f 7574 206f 6620 6461 7465 2066  is out of date f
-00001e30: 6f72 2075 732e 0a20 2020 2020 2020 204e  or us..        N
-00001e40: 6f74 653a 206f 7074 2f63 6d61 6b65 2f6d  ote: opt/cmake/m
-00001e50: 6f64 756c 6573 2072 656d 6f76 6564 2069  odules removed i
-00001e60: 6e20 5265 6469 7341 4920 7631 2e32 2e35  n RedisAI v1.2.5
-00001e70: 0a20 2020 2020 2020 207a 266f 7074 2f63  .        z&opt/c
-00001e80: 6d61 6b65 2f6d 6f64 756c 6573 2f46 696e  make/modules/Fin
-00001e90: 6454 656e 736f 7246 6c6f 772e 636d 616b  dTensorFlow.cmak
-00001ea0: 657a 1c6d 6f64 756c 6573 2f46 696e 6454  ez.modules/FindT
-00001eb0: 656e 736f 7246 6c6f 772e 636d 616b 6546  ensorFlow.cmakeF
-00001ec0: 723f 0000 004e 2906 7280 0000 0072 7500  r?...N).r....ru.
-00001ed0: 0000 7289 0000 00da 0675 6e6c 696e 6b72  ..r......unlinkr
-00001ee0: 3c00 0000 721e 0000 0029 0272 2700 0000  <...r....).r'...
-00001ef0: 5a08 7466 5f63 6d61 6b65 720d 0000 0072  Z.tf_cmaker....r
-00001f00: 0d00 0000 720e 0000 00da 0d63 6f70 795f  ....r......copy_
-00001f10: 7466 5f63 6d61 6b65 1201 0000 7312 0000  tf_cmake....s...
-00001f20: 0000 060a 0108 0108 0108 0204 0108 0002  ................
-00001f30: 0002 ff7a 1c52 6564 6973 4149 4275 696c  ...z.RedisAIBuil
-00001f40: 6465 722e 636f 7079 5f74 665f 636d 616b  der.copy_tf_cmak
-00001f50: 6563 0200 0000 0000 0000 0000 0000 0b00  ec..............
-00001f60: 0000 0900 0000 4300 0000 732e 0100 0074  ......C...s....t
-00001f70: 007c 006a 01a0 0274 036a 04a0 0564 0164  .|.j...t.j...d.d
-00001f80: 027c 019b 0064 029d 03a1 02a1 0183 017d  .|...d.........}
-00001f90: 027c 0273 2e74 0664 0383 0182 017c 0264  .|.s.t.d.....|.d
-00001fa0: 0419 0064 051b 007d 037c 03a0 07a1 0001  ...d...}.|......
-00001fb0: 007c 03a0 08a1 0072 5474 09a0 0a7c 03a1  .|.....rTt...|..
-00001fc0: 0101 0074 03a0 0b7c 03a1 0101 0074 0c7c  ...t...|.....t.|
-00001fd0: 006a 0d83 01a0 07a1 007d 047c 0464 061b  .j.......}.|.d..
-00001fe0: 007d 057c 05a0 0ea1 0073 8a74 0664 077c  .}.|.....s.t.d.|
-00001ff0: 049b 009d 0283 0182 0174 03a0 0f7c 057c  .........t...|.|
-00002000: 0364 061b 00a1 0201 007c 0364 081b 007d  .d.......|.d...}
-00002010: 0674 03a0 0b7c 06a1 0101 007c 0464 081b  .t...|.....|.d..
-00002020: 007d 077c 07a0 08a1 0072 de74 007c 07a0  .}.|.....r.t.|..
-00002030: 0264 02a1 0183 017d 087c 0873 fe74 0664  .d.....}.|.s.t.d
-00002040: 097c 079b 009d 0283 0182 016e 2074 007c  .|.........n t.|
-00002050: 04a0 0264 0aa1 0183 017d 087c 0873 fe74  ...d.....}.|.s.t
-00002060: 0664 097c 049b 009d 0283 0182 017c 0844  .d.|.........|.D
-00002070: 005d 267d 097c 067c 096a 101b 007d 0a7c  .]&}.|.|.j...}.|
-00002080: 0aa0 11a1 0090 0173 0274 03a0 0f7c 097c  .......s.t...|.|
-00002090: 0aa1 0201 0090 0171 0264 0b53 0029 0c7a  .......q.d.S.).z
-000020a0: 8341 6464 2073 796d 626f 6c69 6320 6c69  .Add symbolic li
-000020b0: 6e6b 2074 6f20 6176 6169 6c61 626c 6520  nk to available 
-000020c0: 6c69 6274 656e 736f 7266 6c6f 7720 696e  libtensorflow in
-000020d0: 2052 6564 6973 4149 2064 6570 732e 0a0a   RedisAI deps...
-000020e0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-000020f0: 6576 6963 653a 2063 7075 206f 7220 6770  evice: cpu or gp
-00002100: 750a 2020 2020 2020 2020 3a74 7970 6520  u.        :type 
-00002110: 6465 7669 6365 3a20 7374 720a 2020 2020  device: str.    
-00002120: 2020 2020 da04 6465 7073 723e 0000 007a      ..depsr>...z
-00002130: 2743 6f75 6c64 206e 6f74 2066 696e 6420  'Could not find 
-00002140: 5265 6469 7341 4920 2764 6570 7327 2064  RedisAI 'deps' d
-00002150: 6972 6563 746f 7279 7201 0000 005a 0d6c  irectoryr....Z.l
-00002160: 6962 7465 6e73 6f72 666c 6f77 da07 696e  ibtensorflow..in
-00002170: 636c 7564 657a 2443 6f75 6c64 206e 6f74  cludez$Could not
-00002180: 2066 696e 6420 696e 636c 7564 6520 6469   find include di
-00002190: 7265 6374 6f72 7920 696e 2072 1700 0000  rectory in r....
-000021a0: 7a2e 436f 756c 6420 6e6f 7420 6669 6e64  z.Could not find
-000021b0: 206c 6962 7465 6e73 6f72 666c 6f77 206c   libtensorflow l
-000021c0: 6962 7261 7279 2066 696c 6573 2069 6e20  ibrary files in 
-000021d0: 7a08 6c69 622a 2e73 6f2a 4e29 12da 0673  z.lib*.so*N)...s
-000021e0: 6f72 7465 6472 8000 0000 7240 0000 0072  ortedr....r@...r
-000021f0: 0500 0000 7206 0000 00da 046a 6f69 6e72  ....r......joinr
-00002200: 0c00 0000 7275 0000 0072 2400 0000 7230  ....ru...r$...r0
-00002210: 0000 0072 4900 0000 da08 6d61 6b65 6469  ...rI.....makedi
-00002220: 7273 7202 0000 0072 8400 0000 da06 6578  rsr....r......ex
-00002230: 6973 7473 da07 7379 6d6c 696e 6b72 4200  ists..symlinkrB.
-00002240: 0000 7289 0000 0029 0b72 2700 0000 da06  ..r....).r'.....
-00002250: 6465 7669 6365 5a0d 7261 695f 6465 7073  deviceZ.rai_deps
-00002260: 5f70 6174 685a 0e72 6169 5f6c 6962 7466  _pathZ.rai_libtf
-00002270: 5f70 6174 685a 0a6c 6962 7466 5f70 6174  _pathZ.libtf_pat
-00002280: 685a 1069 6e63 6c75 6465 5f73 7263 5f70  hZ.include_src_p
-00002290: 6174 685a 1172 6169 5f6c 6962 7466 5f6c  athZ.rai_libtf_l
-000022a0: 6962 5f64 6972 5a11 7372 635f 6c69 6274  ib_dirZ.src_libt
-000022b0: 665f 6c69 625f 6469 725a 0d6c 6962 7261  f_lib_dirZ.libra
-000022c0: 7279 5f66 696c 6573 5a08 7372 635f 6669  ry_filesZ.src_fi
-000022d0: 6c65 5a08 6473 745f 6669 6c65 720d 0000  leZ.dst_filer...
-000022e0: 0072 0d00 0000 720e 0000 00da 0d73 796d  .r....r......sym
-000022f0: 6c69 6e6b 5f6c 6962 7466 2101 0000 7342  link_libtf!...sB
-00002300: 0000 0000 0602 011c ff04 0304 0108 050c  ................
-00002310: 0108 0108 010a 020a 010e 0308 0108 010e  ................
-00002320: 0110 0408 010a 0108 0408 010e 0104 0102  ................
-00002330: 0108 ff06 040e 0104 0102 0108 ff04 0408  ................
-00002340: 010a 010a 017a 1c52 6564 6973 4149 4275  .....z.RedisAIBu
-00002350: 696c 6465 722e 7379 6d6c 696e 6b5f 6c69  ilder.symlink_li
-00002360: 6274 6663 0400 0000 0000 0000 0000 0000  btfc............
-00002370: 0700 0000 0a00 0000 4300 0000 7398 0100  ........C...s...
-00002380: 007c 006a 00a0 01a1 0072 1674 02a0 037c  .|.j.....r.t...|
-00002390: 006a 00a1 0101 007c 00a0 047c 01a1 0173  .j.....|...|...s
-000023a0: 2e74 0564 017c 019b 009d 0283 0182 017c  .t.d.|.........|
-000023b0: 00a0 0664 02a1 0164 0364 0464 0564 067c  ...d...d.d.d.d.|
-000023c0: 0164 077c 0264 0864 0967 0a7d 047c 006a  .d.|.d.d.g.}.|.j
-000023d0: 077c 0474 086a 097c 006a 0a64 0a8d 0301  .|.t.j.|.j.d....
-000023e0: 007c 00a0 0ba1 0001 007c 00a0 0664 02a1  .|.......|...d..
-000023f0: 0164 0b64 0c7c 006a 0c72 847c 006a 0d73  .d.d.|.j.r.|.j.s
-00002400: 8464 0d6e 0264 0e9b 009d 0264 0f64 107c  .d.n.d.....d.d.|
-00002410: 006a 0e9b 009d 0264 117c 00a0 0664 12a1  .j.....d.|...d..
-00002420: 017c 006a 0064 131b 007c 0367 097d 057c  .|.j.d...|.g.}.|
-00002430: 006a 077c 0574 086a 097c 006a 0064 0a8d  .j.|.t.j.|.j.d..
-00002440: 0301 007c 006a 0d72 d27c 00a0 0f7c 03a1  ...|.j.r.|...|..
-00002450: 0101 007c 00a0 0664 02a1 0164 147c 006a  ...|...d...d.|.j
-00002460: 109b 009d 0264 0c7c 006a 0c9b 009d 0264  .....d.|.j.....d
-00002470: 0f64 107c 006a 0e9b 009d 0264 1567 067d  .d.|.j.....d.g.}
-00002480: 067c 0364 166b 0290 0172 167c 06a0 1164  .|.d.k...r.|...d
-00002490: 17a1 0101 006e 0a7c 06a0 1164 18a1 0101  .....n.|...d....
-000024a0: 007c 006a 1290 0172 3874 137c 006a 1283  .|.j...r8t.|.j..
-000024b0: 017c 006a 1464 193c 007c 06a0 157c 00a0  .|.j.d.<.|...|..
-000024c0: 0664 1aa1 0164 1b74 137c 006a 0064 1c1b  .d...d.t.|.j.d..
-000024d0: 0083 0164 1d7c 006a 169b 0064 1e67 06a1  ...d.|.j...d.g..
-000024e0: 0101 007c 006a 077c 067c 006a 0064 1f8d  ...|.j.|.|.j.d..
-000024f0: 0201 007c 00a0 177c 03a1 0101 007c 006a  ...|...|.....|.j
-00002500: 1090 0172 8c7c 00a0 18a1 0001 007c 00a0  ...r.|.......|..
-00002510: 19a1 0001 0064 2053 0029 217a f542 7569  .....d S.)!z.Bui
-00002520: 6c64 2052 6564 6973 4149 2066 726f 6d20  ld RedisAI from 
-00002530: 6769 740a 2020 2020 2020 2020 3a70 6172  git.        :par
-00002540: 616d 2067 6974 5f75 726c 3a20 7572 6c20  am git_url: url 
-00002550: 6672 6f6d 2077 6869 6368 2074 6f20 7265  from which to re
-00002560: 7472 6965 7665 2052 6564 6973 4149 0a20  trieve RedisAI. 
-00002570: 2020 2020 2020 203a 7479 7065 2067 6974         :type git
-00002580: 5f75 726c 3a20 7374 720a 2020 2020 2020  _url: str.      
-00002590: 2020 3a70 6172 616d 2062 7261 6e63 683a    :param branch:
-000025a0: 2062 7261 6e63 6820 746f 2063 6865 636b   branch to check
-000025b0: 6f75 740a 2020 2020 2020 2020 3a74 7970  out.        :typ
-000025c0: 6520 6272 616e 6368 3a20 7374 720a 2020  e branch: str.  
-000025d0: 2020 2020 2020 3a70 6172 616d 2064 6576        :param dev
-000025e0: 6963 653a 2063 7075 206f 7220 6770 750a  ice: cpu or gpu.
-000025f0: 2020 2020 2020 2020 3a74 7970 6520 6465          :type de
-00002600: 7669 6365 3a20 7374 720a 2020 2020 2020  vice: str.      
-00002610: 2020 7a17 4d61 6c66 6f72 6d65 6420 5265    z.Malformed Re
-00002620: 6469 7341 4920 5552 4c3a 2072 1800 0000  disAI URL: r....
-00002630: 7a15 4749 545f 4c46 535f 534b 4950 5f53  z.GIT_LFS_SKIP_S
-00002640: 4d55 4447 453d 3172 6c00 0000 726d 0000  MUDGE=1rl...rm..
-00002650: 007a 0b2d 2d72 6563 7572 7369 7665 726e  .z.--recursivern
-00002660: 0000 007a 092d 2d64 6570 7468 3d31 727f  ...z.--depth=1r.
-00002670: 0000 0029 0272 2200 0000 724e 0000 007a  ...).r"...rN...z
-00002680: 0957 4954 485f 5054 3d30 7a08 5749 5448  .WITH_PT=0z.WITH
-00002690: 5f54 463d 7215 0000 0072 0100 0000 7a0d  _TF=r....r....z.
-000026a0: 5749 5448 5f54 464c 4954 453d 307a 0957  WITH_TFLITE=0z.W
-000026b0: 4954 485f 4f52 543d 7a09 5645 5242 4f53  ITH_ORT=z.VERBOS
-000026c0: 453d 315a 0462 6173 687a 0b67 6574 5f64  E=1Z.bashz.get_d
-000026d0: 6570 732e 7368 7a08 5749 5448 5f50 543d  eps.shz.WITH_PT=
-000026e0: 7a11 5749 5448 5f55 4e49 545f 5445 5354  z.WITH_UNIT_TEST
-000026f0: 533d 305a 0367 7075 7a05 4750 553d 317a  S=0Z.gpuz.GPU=1z
-00002700: 0547 5055 3d30 5a09 546f 7263 685f 4449  .GPU=0Z.Torch_DI
-00002710: 5272 7100 0000 7a02 2d43 da03 6f70 7472  Rrq...z.-C..optr
-00002720: 7200 0000 da05 6275 696c 6472 7000 0000  r.....buildrp...
-00002730: 4e29 1a72 8000 0000 7224 0000 0072 3000  N).r....r$...r0.
-00002740: 0000 7249 0000 0072 4800 0000 7210 0000  ..rI...rH...r...
-00002750: 0072 3200 0000 725a 0000 0072 2000 0000  .r2...rZ...r ...
-00002760: 7221 0000 0072 1d00 0000 728d 0000 0072  r!...r....r....r
-00002770: 8200 0000 7284 0000 0072 8300 0000 7296  ....r....r....r.
-00002780: 0000 0072 8100 0000 da06 6170 7065 6e64  ...r......append
-00002790: 7285 0000 0072 4a00 0000 7218 0000 00da  r....rJ...r.....
-000027a0: 0665 7874 656e 6472 2600 0000 da11 5f69  .extendr&....._i
-000027b0: 6e73 7461 6c6c 5f62 6163 6b65 6e64 73da  nstall_backends.
-000027c0: 105f 6d6f 7665 5f74 6f72 6368 5f6c 6962  ._move_torch_lib
-000027d0: 7372 4b00 0000 2907 7227 0000 0072 7700  srK...).r'...rw.
-000027e0: 0000 7278 0000 0072 9500 0000 7279 0000  ..rx...r....ry..
-000027f0: 005a 0764 6570 5f63 6d64 727a 0000 0072  .Z.dep_cmdrz...r
-00002800: 0d00 0000 720d 0000 0072 0e00 0000 722f  ....r....r....r/
-00002810: 0000 0058 0100 0073 7800 0000 000b 0a01  ...X...sx.......
-00002820: 0c03 0a01 0e04 0801 0201 0201 0201 0201  ................
-00002830: 0201 0201 0201 0201 02f6 040c 1403 0804  ................
-00002840: 0801 0201 1801 0201 0a01 0201 0801 0801  ................
-00002850: 02f7 040c 0401 0201 0401 04fd 0606 0601  ................
-00002860: 0a03 0801 0a01 0a01 0201 0a01 02fa 0409  ................
-00002870: 0a01 0c02 0a02 0801 1002 0402 0801 0201  ................
-00002880: 0c01 0201 0601 02fa 02ff 040a 1002 0a01  ................
-00002890: 0801 0801 7a1d 5265 6469 7341 4942 7569  ....z.RedisAIBui
-000028a0: 6c64 6572 2e62 7569 6c64 5f66 726f 6d5f  lder.build_from_
-000028b0: 6769 7463 0200 0000 0000 0000 0000 0000  gitc............
-000028c0: 0400 0000 0500 0000 4300 0000 736c 0000  ........C...sl..
-000028d0: 007c 006a 00a0 0164 017c 019b 009d 02a1  .|.j...d.|......
-000028e0: 01a0 02a1 007c 005f 037c 006a 0364 021b  .....|._.|.j.d..
-000028f0: 007d 027c 006a 0364 031b 007d 037c 02a0  .}.|.j.d...}.|..
-00002900: 04a1 0072 687c 03a0 05a1 0072 687c 006a  ...rh|.....rh|.j
-00002910: 067c 037c 006a 0764 031b 0064 0464 058d  .|.|.j.d...d.d..
-00002920: 0301 007c 006a 087c 027c 006a 0764 021b  ...|.j.|.|.j.d..
-00002930: 0064 0464 058d 0301 0064 0653 0029 077a  .d.d.....d.S.).z
-00002940: 724d 6f76 6520 6261 636b 656e 6420 6c69  rMove backend li
-00002950: 6272 6172 6965 7320 746f 2073 6d61 7274  braries to smart
-00002960: 7369 6d2f 5f63 6f72 652f 6c69 622f 0a20  sim/_core/lib/. 
-00002970: 2020 2020 2020 203a 7061 7261 6d20 6465         :param de
-00002980: 7669 6365 3a20 6370 7520 6f72 2063 7075  vice: cpu or cpu
-00002990: 0a20 2020 2020 2020 203a 7479 7065 2064  .        :type d
-000029a0: 6576 6963 653a 2073 7472 0a20 2020 2020  evice: str.     
-000029b0: 2020 207a 0869 6e73 7461 6c6c 2d72 8700     z.install-r..
-000029c0: 0000 7286 0000 0054 723f 0000 004e 2909  ..r....Tr?...N).
-000029d0: 7280 0000 0072 8800 0000 7275 0000 005a  r....r....ru...Z
-000029e0: 1072 6169 5f69 6e73 7461 6c6c 5f70 6174  .rai_install_pat
-000029f0: 6872 8900 0000 7224 0000 0072 4100 0000  hr....r$...rA...
-00002a00: 721f 0000 0072 3c00 0000 2904 7227 0000  r....r<...).r'..
-00002a10: 0072 9500 0000 5a07 7261 695f 6c69 625a  .r....Z.rai_libZ
-00002a20: 0c72 6169 5f62 6163 6b65 6e64 7372 0d00  .rai_backendsr..
-00002a30: 0000 720d 0000 0072 0e00 0000 729b 0000  ..r....r....r...
-00002a40: 00b4 0100 0073 1000 0000 0005 0601 08ff  .....s..........
-00002a50: 0a03 0a01 0a02 1001 1601 7a20 5265 6469  ..........z Redi
-00002a60: 7341 4942 7569 6c64 6572 2e5f 696e 7374  sAIBuilder._inst
-00002a70: 616c 6c5f 6261 636b 656e 6473 6301 0000  all_backendsc...
-00002a80: 0000 0000 0000 0000 0006 0000 0005 0000  ................
-00002a90: 0043 0000 0073 6800 0000 7c00 6a00 6401  .C...sh...|.j.d.
-00002aa0: 1b00 6402 1b00 7d01 7c01 6403 1b00 7d02  ..d...}.|.d...}.
-00002ab0: 7401 7c00 6a02 8301 6a03 6a03 6a03 7d03  t.|.j...j.j.j.}.
-00002ac0: 7c03 6403 1b00 7d04 7c00 6a04 7c04 7c02  |.d...}.|.j.|.|.
-00002ad0: 6404 6405 8d03 0100 7405 6a06 6406 6b02  d.d.....t.j.d.k.
-00002ae0: 7264 7c03 6407 1b00 7d05 7c00 6a04 7c05  rd|.d...}.|.j.|.
-00002af0: 7c01 6407 1b00 6404 6405 8d03 0100 6408  |.d...d.d.....d.
-00002b00: 5300 2909 7ade 4d6f 7665 2070 6970 2069  S.).z.Move pip i
-00002b10: 6e73 7461 6c6c 2074 6f72 6368 206c 6962  nstall torch lib
-00002b20: 7261 7269 6573 0a20 2020 2020 2020 2053  raries.        S
-00002b30: 696e 6365 2077 6520 7573 6520 7069 7020  ince we use pip 
-00002b40: 696e 7374 616c 6c65 6420 746f 7263 6820  installed torch 
-00002b50: 6c69 6272 6172 6965 7320 666f 7220 6275  libraries for bu
-00002b60: 696c 6469 6e67 0a20 2020 2020 2020 2052  ilding.        R
-00002b70: 6564 6973 4149 2c20 7765 206e 6565 6420  edisAI, we need 
-00002b80: 746f 206d 6f76 6520 7468 656d 2069 6e74  to move them int
-00002b90: 6f20 7468 6520 4c44 5f72 756e 7061 7468  o the LD_runpath
-00002ba0: 206f 6620 7265 6469 7361 692e 736f 0a20   of redisai.so. 
-00002bb0: 2020 2020 2020 2069 6e20 7468 6520 736d         in the sm
-00002bc0: 6172 7473 696d 2f5f 636f 7265 2f6c 6962  artsim/_core/lib
-00002bd0: 2064 6972 6563 746f 7279 2e0a 2020 2020   directory..    
-00002be0: 2020 2020 7286 0000 005a 0d72 6564 6973      r....Z.redis
-00002bf0: 6169 5f74 6f72 6368 7217 0000 0054 723f  ai_torchr....Tr?
-00002c00: 0000 00da 0664 6172 7769 6e7a 072e 6479  .....darwinz..dy
-00002c10: 6c69 6273 4e29 0772 1f00 0000 7202 0000  libsN).r....r...
-00002c20: 0072 8500 0000 721a 0000 0072 4100 0000  .r....r....rA...
-00002c30: da03 7379 73da 0870 6c61 7466 6f72 6d29  ..sys..platform)
-00002c40: 0672 2700 0000 5a11 7373 5f72 6169 5f74  .r'...Z.ss_rai_t
-00002c50: 6f72 6368 5f70 6174 685a 1573 735f 7261  orch_pathZ.ss_ra
-00002c60: 695f 746f 7263 685f 6c69 625f 7061 7468  i_torch_lib_path
-00002c70: 5a0e 7069 705f 746f 7263 685f 7061 7468  Z.pip_torch_path
-00002c80: 5a12 7069 705f 746f 7263 685f 6c69 625f  Z.pip_torch_lib_
-00002c90: 7061 7468 5a06 6479 6c69 6273 720d 0000  pathZ.dylibsr...
-00002ca0: 0072 0d00 0000 720e 0000 0072 9c00 0000  .r....r....r....
-00002cb0: c301 0000 7310 0000 0000 070e 0108 0610  ....s...........
-00002cc0: 0108 0210 030a 0108 017a 1f52 6564 6973  .........z.Redis
-00002cd0: 4149 4275 696c 6465 722e 5f6d 6f76 655f  AIBuilder._move_
-00002ce0: 746f 7263 685f 6c69 6273 290d 7211 0000  torch_libs).r...
-00002cf0: 0072 1200 0000 7213 0000 0072 5b00 0000  .r....r....r[...
-00002d00: 7229 0000 0072 5e00 0000 722e 0000 0072  r)...r^...r....r
-00002d10: 8d00 0000 7296 0000 0072 2f00 0000 729b  ....r....r/...r.
-00002d20: 0000 0072 9c00 0000 727c 0000 0072 0d00  ...r....r|...r..
-00002d30: 0000 720d 0000 0072 6500 0000 720e 0000  ..r....re...r...
-00002d40: 0072 7d00 0000 ef00 0000 7322 0000 0008  .r}.......s"....
-00002d50: 0104 0902 0102 0102 0102 0102 0102 0102  ................
-00002d60: 0102 f70e 1502 010a 0508 0f08 3708 5c08  ............7.\.
-00002d70: 0f72 7d00 0000 2910 7205 0000 0072 4400  .r}...).r....rD.
-00002d80: 0000 7230 0000 0072 3500 0000 7220 0000  ..r0...r5...r ..
-00002d90: 0072 9e00 0000 da07 7061 7468 6c69 6272  .r......pathlibr
-00002da0: 0200 0000 7203 0000 0072 0400 0000 720f  ....r....r....r.
-00002db0: 0000 00da 0945 7863 6570 7469 6f6e 7210  .....Exceptionr.
-00002dc0: 0000 0072 1400 0000 725f 0000 0072 7d00  ...r....r_...r}.
-00002dd0: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00002de0: 0072 0e00 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00002df0: 0100 0000 731a 0000 0008 0108 0108 0108  ....s...........
-00002e00: 0108 0108 010c 010c 010c 0a08 1310 040e  ................
-00002e10: 6810 5d                                  h.]
+000017b0: 0072 0b00 0000 720c 0000 0029 1772 2700  .r....r....).r'.
+000017c0: 0000 da07 6769 745f 7572 6cda 0662 7261  ....git_url..bra
+000017d0: 6e63 685a 0d64 6174 6162 6173 655f 6e61  nchZ.database_na
+000017e0: 6d65 5a13 6461 7461 6261 7365 5f62 7569  meZ.database_bui
+000017f0: 6c64 5f70 6174 685a 1072 6564 6973 5f62  ld_pathZ.redis_b
+00001800: 7569 6c64 5f70 6174 685a 106b 6579 6462  uild_pathZ.keydb
+00001810: 5f62 7569 6c64 5f70 6174 68da 0963 6c6f  _build_path..clo
+00001820: 6e65 5f63 6d64 da09 6275 696c 645f 636d  ne_cmd..build_cm
+00001830: 645a 1064 6174 6162 6173 655f 7372 635f  dZ.database_src_
+00001840: 6469 725a 0d73 6572 7665 725f 736f 7572  dirZ.server_sour
+00001850: 6365 5a12 7365 7276 6572 5f64 6573 7469  ceZ.server_desti
+00001860: 6e61 7469 6f6e 5a0a 636c 695f 736f 7572  nationZ.cli_sour
+00001870: 6365 5a0f 636c 695f 6465 7374 696e 6174  ceZ.cli_destinat
+00001880: 696f 6e5a 0963 6f72 655f 7061 7468 7228  ionZ.core_pathr(
+00001890: 0000 0072 1e00 0000 5a0c 6461 7461 6261  ...r....Z.databa
+000018a0: 7365 5f65 7865 5a08 6461 7461 6261 7365  se_exeZ.database
+000018b0: da01 5f72 5900 0000 5a0d 7265 6469 735f  .._rY...Z.redis_
+000018c0: 636c 695f 6578 655a 0972 6564 6973 5f63  cli_exeZ.redis_c
+000018d0: 6c69 720d 0000 0072 0d00 0000 720e 0000  lir....r....r...
+000018e0: 0072 2f00 0000 c100 0000 7360 0000 0000  .r/.......s`....
+000018f0: 0710 0110 040c 010c 0108 010e 0108 010e  ................
+00001900: 030a 0114 0408 0102 0102 0102 0102 0102  ................
+00001910: 0102 0102 f804 0a10 0408 0102 0108 010a  ................
+00001920: fc04 0612 0308 0110 0112 0110 0112 0110  ................
+00001930: 0110 0314 010e 010e 0102 010e 0116 0110  ................
+00001940: 0116 011c 0302 010e 0116 0110 0116 017a  ...............z
+00001950: 1e44 6174 6162 6173 6542 7569 6c64 6572  .DatabaseBuilder
+00001960: 2e62 7569 6c64 5f66 726f 6d5f 6769 7429  .build_from_git)
+00001970: 0972 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00001980: 725b 0000 0072 2900 0000 725e 0000 0072  r[...r)...r^...r
+00001990: 2e00 0000 722f 0000 00da 0d5f 5f63 6c61  ....r/.....__cla
+000019a0: 7373 6365 6c6c 5f5f 720d 0000 0072 0d00  sscell__r....r..
+000019b0: 0000 7265 0000 0072 0e00 0000 725f 0000  ..re...r....r_..
+000019c0: 00ad 0000 0073 0a00 0000 0801 0407 1604  .....s..........
+000019d0: 0201 0a07 725f 0000 0063 0000 0000 0000  ....r_...c......
+000019e0: 0000 0000 0000 0000 0000 0800 0000 0000  ................
+000019f0: 0000 7372 0000 0065 005a 0164 005a 0264  ..sr...e.Z.d.Z.d
+00001a00: 015a 0369 0064 0264 0264 0364 0364 0464  .Z.i.d.d.d.d.d.d
+00001a10: 0564 0466 0887 0066 0164 0664 0784 095a  .d.f...f.d.d...Z
+00001a20: 0465 0564 0864 0984 0083 015a 0665 0564  .e.d.d.....Z.e.d
+00001a30: 0a64 0b84 0083 015a 0764 0c64 0d84 005a  .d.....Z.d.d...Z
+00001a40: 0864 0e64 0f84 005a 0964 1064 1184 005a  .d.d...Z.d.d...Z
+00001a50: 0a64 1264 1384 005a 0b64 1464 1584 005a  .d.d...Z.d.d...Z
+00001a60: 0c87 0004 005a 0d53 0029 16da 0e52 6564  .....Z.S.)...Red
+00001a70: 6973 4149 4275 696c 6465 727a a343 6c61  isAIBuilderz.Cla
+00001a80: 7373 2074 6f20 6275 696c 6420 5265 6469  ss to build Redi
+00001a90: 7341 4920 6672 6f6d 2053 6f75 7263 650a  sAI from Source.
+00001aa0: 2020 2020 5375 7070 6f72 7465 6420 6275      Supported bu
+00001ab0: 696c 6420 6d65 7468 6f64 3a0a 2020 2020  ild method:.    
+00001ac0: 202d 2066 726f 6d20 6769 740a 2020 2020   - from git.    
+00001ad0: 5365 6520 6275 696c 6465 6e76 2e70 7920  See buildenv.py 
+00001ae0: 666f 7220 6275 696c 6474 696d 6520 636f  for buildtime co
+00001af0: 6e66 6967 7572 6174 696f 6e20 6f66 2052  nfiguration of R
+00001b00: 6564 6973 4149 0a20 2020 2076 6572 7369  edisAI.    versi
+00001b10: 6f6e 2061 6e64 2075 726c 2e0a 2020 2020  on and url..    
+00001b20: da00 5446 4e63 0900 0000 0000 0000 0000  ..TFNc..........
+00001b30: 0000 0900 0000 0500 0000 0300 0000 734c  ..............sL
+00001b40: 0000 0074 0083 006a 017c 017c 077c 0864  ...t...j.|.|.|.d
+00001b50: 018d 0301 007c 0472 1a64 026e 0264 037c  .....|.r.d.n.d.|
+00001b60: 005f 027c 0572 2864 026e 0264 037c 005f  ._.|.r(d.n.d.|._
+00001b70: 037c 0672 3664 026e 0264 037c 005f 047c  .|.r6d.n.d.|._.|
+00001b80: 037c 005f 057c 027c 005f 0664 0053 0029  .|._.|.|._.d.S.)
+00001b90: 044e 7261 0000 0072 1500 0000 7201 0000  .Nra...r....r...
+00001ba0: 0029 0772 6200 0000 7229 0000 00da 0574  .).rb...r).....t
+00001bb0: 6f72 6368 da02 7466 da04 6f6e 6e78 da09  orch..tf..onnx..
+00001bc0: 6c69 6274 665f 6469 72da 0974 6f72 6368  libtf_dir..torch
+00001bd0: 5f64 6972 2909 7227 0000 0072 6400 0000  _dir).r'...rd...
+00001be0: 7283 0000 0072 8200 0000 5a0b 6275 696c  r....r....Z.buil
+00001bf0: 645f 746f 7263 685a 0862 7569 6c64 5f74  d_torchZ.build_t
+00001c00: 665a 0a62 7569 6c64 5f6f 6e6e 7872 2600  fZ.build_onnxr&.
+00001c10: 0000 7223 0000 0072 6500 0000 720d 0000  ..r#...re...r...
+00001c20: 0072 0e00 0000 7229 0000 0013 0100 0073  .r....r).......s
+00001c30: 0c00 0000 000b 1203 0e01 0e01 0e01 0601  ................
+00001c40: 7a17 5265 6469 7341 4942 7569 6c64 6572  z.RedisAIBuilder
+00001c50: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
+00001c60: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+00001c70: 0000 730c 0000 0074 007c 006a 0164 0183  ..s....t.|.j.d..
+00001c80: 0253 0029 024e da07 5265 6469 7341 4929  .S.).N..RedisAI)
+00001c90: 0272 0200 0000 721d 0000 0072 2d00 0000  .r....r....r-...
+00001ca0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+00001cb0: 0e72 6169 5f62 7569 6c64 5f70 6174 6827  .rai_build_path'
+00001cc0: 0100 0073 0200 0000 0002 7a1d 5265 6469  ...s......z.Redi
+00001cd0: 7341 4942 7569 6c64 6572 2e72 6169 5f62  sAIBuilder.rai_b
+00001ce0: 7569 6c64 5f70 6174 6863 0100 0000 0000  uild_pathc......
+00001cf0: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+00001d00: 0000 7328 0000 007c 006a 00a0 0164 01a1  ..s(...|.j...d..
+00001d10: 01a0 02a1 007d 017c 006a 00a0 0164 02a1  .....}.|.j...d..
+00001d20: 01a0 03a1 007d 027c 016f 267c 0253 0029  .....}.|.o&|.S.)
+00001d30: 034e da08 6261 636b 656e 6473 fa0a 7265  .N..backends..re
+00001d40: 6469 7361 692e 736f 2904 721f 0000 00da  disai.so).r.....
+00001d50: 086a 6f69 6e70 6174 6872 2400 0000 da07  .joinpathr$.....
+00001d60: 6973 5f66 696c 6529 0372 2700 0000 da06  is_file).r'.....
+00001d70: 7365 7276 6572 da03 636c 6972 0d00 0000  server..clir....
+00001d80: 720d 0000 0072 0e00 0000 722e 0000 002b  r....r....r....+
+00001d90: 0100 0073 0600 0000 0002 1001 1001 7a17  ...s..........z.
+00001da0: 5265 6469 7341 4942 7569 6c64 6572 2e69  RedisAIBuilder.i
+00001db0: 735f 6275 696c 7463 0100 0000 0000 0000  s_builtc........
+00001dc0: 0000 0000 0200 0000 0500 0000 4300 0000  ............C...
+00001dd0: 733c 0000 007c 006a 0064 011b 007d 017c  s<...|.j.d...}.|
+00001de0: 01a0 01a1 0001 007c 01a0 02a1 0072 387c  .......|.....r8|
+00001df0: 01a0 03a1 0001 007c 006a 047c 006a 0564  .......|.j.|.j.d
+00001e00: 021b 007c 0164 0364 048d 0301 0064 0553  ...|.d.d.....d.S
+00001e10: 0029 067a be43 6f70 7920 7468 6520 4669  .).z.Copy the Fi
+00001e20: 6e64 5465 6e73 6f72 466c 6f77 2e63 6d61  ndTensorFlow.cma
+00001e30: 6b65 2066 696c 6520 746f 2074 6865 2062  ke file to the b
+00001e40: 7569 6c64 2064 6972 6563 746f 7279 0a20  uild directory. 
+00001e50: 2020 2020 2020 2061 7320 7468 6520 7665         as the ve
+00001e60: 7273 696f 6e20 696e 636c 7564 6564 2069  rsion included i
+00001e70: 6e20 5265 6469 7341 4920 6973 206f 7574  n RedisAI is out
+00001e80: 206f 6620 6461 7465 2066 6f72 2075 732e   of date for us.
+00001e90: 0a20 2020 2020 2020 204e 6f74 653a 206f  .        Note: o
+00001ea0: 7074 2f63 6d61 6b65 2f6d 6f64 756c 6573  pt/cmake/modules
+00001eb0: 2072 656d 6f76 6564 2069 6e20 5265 6469   removed in Redi
+00001ec0: 7341 4920 7631 2e32 2e35 0a20 2020 2020  sAI v1.2.5.     
+00001ed0: 2020 207a 266f 7074 2f63 6d61 6b65 2f6d     z&opt/cmake/m
+00001ee0: 6f64 756c 6573 2f46 696e 6454 656e 736f  odules/FindTenso
+00001ef0: 7246 6c6f 772e 636d 616b 657a 1c6d 6f64  rFlow.cmakez.mod
+00001f00: 756c 6573 2f46 696e 6454 656e 736f 7246  ules/FindTensorF
+00001f10: 6c6f 772e 636d 616b 6546 723f 0000 004e  low.cmakeFr?...N
+00001f20: 2906 7285 0000 0072 7500 0000 7289 0000  ).r....ru...r...
+00001f30: 00da 0675 6e6c 696e 6b72 3c00 0000 721e  ...unlinkr<...r.
+00001f40: 0000 0029 0272 2700 0000 5a08 7466 5f63  ...).r'...Z.tf_c
+00001f50: 6d61 6b65 720d 0000 0072 0d00 0000 720e  maker....r....r.
+00001f60: 0000 00da 0d63 6f70 795f 7466 5f63 6d61  .....copy_tf_cma
+00001f70: 6b65 3101 0000 7312 0000 0000 060a 0108  ke1...s.........
+00001f80: 0108 0108 0204 0108 0002 0002 ff7a 1c52  .............z.R
+00001f90: 6564 6973 4149 4275 696c 6465 722e 636f  edisAIBuilder.co
+00001fa0: 7079 5f74 665f 636d 616b 6563 0200 0000  py_tf_cmakec....
+00001fb0: 0000 0000 0000 0000 0b00 0000 0900 0000  ................
+00001fc0: 4300 0000 732e 0100 0074 007c 006a 01a0  C...s....t.|.j..
+00001fd0: 0274 036a 04a0 0564 0164 027c 019b 0064  .t.j...d.d.|...d
+00001fe0: 029d 03a1 02a1 0183 017d 027c 0273 2e74  .........}.|.s.t
+00001ff0: 0664 0383 0182 017c 0264 0419 0064 051b  .d.....|.d...d..
+00002000: 007d 037c 03a0 07a1 0001 007c 03a0 08a1  .}.|.......|....
+00002010: 0072 5474 09a0 0a7c 03a1 0101 0074 03a0  .rTt...|.....t..
+00002020: 0b7c 03a1 0101 0074 0c7c 006a 0d83 01a0  .|.....t.|.j....
+00002030: 07a1 007d 047c 0464 061b 007d 057c 05a0  ...}.|.d...}.|..
+00002040: 0ea1 0073 8a74 0664 077c 049b 009d 0283  ...s.t.d.|......
+00002050: 0182 0174 03a0 0f7c 057c 0364 061b 00a1  ...t...|.|.d....
+00002060: 0201 007c 0364 081b 007d 0674 03a0 0b7c  ...|.d...}.t...|
+00002070: 06a1 0101 007c 0464 081b 007d 077c 07a0  .....|.d...}.|..
+00002080: 08a1 0072 de74 007c 07a0 0264 02a1 0183  ...r.t.|...d....
+00002090: 017d 087c 0873 fe74 0664 097c 079b 009d  .}.|.s.t.d.|....
+000020a0: 0283 0182 016e 2074 007c 04a0 0264 0aa1  .....n t.|...d..
+000020b0: 0183 017d 087c 0873 fe74 0664 097c 049b  ...}.|.s.t.d.|..
+000020c0: 009d 0283 0182 017c 0844 005d 267d 097c  .......|.D.]&}.|
+000020d0: 067c 096a 101b 007d 0a7c 0aa0 11a1 0090  .|.j...}.|......
+000020e0: 0173 0274 03a0 0f7c 097c 0aa1 0201 0090  .s.t...|.|......
+000020f0: 0171 0264 0b53 0029 0c7a 8341 6464 2073  .q.d.S.).z.Add s
+00002100: 796d 626f 6c69 6320 6c69 6e6b 2074 6f20  ymbolic link to 
+00002110: 6176 6169 6c61 626c 6520 6c69 6274 656e  available libten
+00002120: 736f 7266 6c6f 7720 696e 2052 6564 6973  sorflow in Redis
+00002130: 4149 2064 6570 732e 0a0a 2020 2020 2020  AI deps...      
+00002140: 2020 3a70 6172 616d 2064 6576 6963 653a    :param device:
+00002150: 2063 7075 206f 7220 6770 750a 2020 2020   cpu or gpu.    
+00002160: 2020 2020 3a74 7970 6520 6465 7669 6365      :type device
+00002170: 3a20 7374 720a 2020 2020 2020 2020 da04  : str.        ..
+00002180: 6465 7073 723e 0000 007a 2743 6f75 6c64  depsr>...z'Could
+00002190: 206e 6f74 2066 696e 6420 5265 6469 7341   not find RedisA
+000021a0: 4920 2764 6570 7327 2064 6972 6563 746f  I 'deps' directo
+000021b0: 7279 7201 0000 005a 0d6c 6962 7465 6e73  ryr....Z.libtens
+000021c0: 6f72 666c 6f77 da07 696e 636c 7564 657a  orflow..includez
+000021d0: 2443 6f75 6c64 206e 6f74 2066 696e 6420  $Could not find 
+000021e0: 696e 636c 7564 6520 6469 7265 6374 6f72  include director
+000021f0: 7920 696e 2072 1700 0000 7a2e 436f 756c  y in r....z.Coul
+00002200: 6420 6e6f 7420 6669 6e64 206c 6962 7465  d not find libte
+00002210: 6e73 6f72 666c 6f77 206c 6962 7261 7279  nsorflow library
+00002220: 2066 696c 6573 2069 6e20 7a08 6c69 622a   files in z.lib*
+00002230: 2e73 6f2a 4e29 12da 0673 6f72 7465 6472  .so*N)...sortedr
+00002240: 8500 0000 7240 0000 0072 0500 0000 7206  ....r@...r....r.
+00002250: 0000 00da 046a 6f69 6e72 0c00 0000 7275  .....joinr....ru
+00002260: 0000 0072 2400 0000 7230 0000 0072 4900  ...r$...r0...rI.
+00002270: 0000 da08 6d61 6b65 6469 7273 7202 0000  ....makedirsr...
+00002280: 0072 8200 0000 da06 6578 6973 7473 da07  .r......exists..
+00002290: 7379 6d6c 696e 6b72 4200 0000 7289 0000  symlinkrB...r...
+000022a0: 0029 0b72 2700 0000 da06 6465 7669 6365  .).r'.....device
+000022b0: 5a0d 7261 695f 6465 7073 5f70 6174 685a  Z.rai_deps_pathZ
+000022c0: 0e72 6169 5f6c 6962 7466 5f70 6174 685a  .rai_libtf_pathZ
+000022d0: 0a6c 6962 7466 5f70 6174 685a 1069 6e63  .libtf_pathZ.inc
+000022e0: 6c75 6465 5f73 7263 5f70 6174 685a 1172  lude_src_pathZ.r
+000022f0: 6169 5f6c 6962 7466 5f6c 6962 5f64 6972  ai_libtf_lib_dir
+00002300: 5a11 7372 635f 6c69 6274 665f 6c69 625f  Z.src_libtf_lib_
+00002310: 6469 725a 0d6c 6962 7261 7279 5f66 696c  dirZ.library_fil
+00002320: 6573 5a08 7372 635f 6669 6c65 5a08 6473  esZ.src_fileZ.ds
+00002330: 745f 6669 6c65 720d 0000 0072 0d00 0000  t_filer....r....
+00002340: 720e 0000 00da 0d73 796d 6c69 6e6b 5f6c  r......symlink_l
+00002350: 6962 7466 4001 0000 7342 0000 0000 0602  ibtf@...sB......
+00002360: 011c ff04 0304 0108 050c 0108 0108 010a  ................
+00002370: 020a 010e 0308 0108 010e 0110 0408 010a  ................
+00002380: 0108 0408 010e 0104 0102 0108 ff06 040e  ................
+00002390: 0104 0102 0108 ff04 0408 010a 010a 017a  ...............z
+000023a0: 1c52 6564 6973 4149 4275 696c 6465 722e  .RedisAIBuilder.
+000023b0: 7379 6d6c 696e 6b5f 6c69 6274 6663 0400  symlink_libtfc..
+000023c0: 0000 0000 0000 0000 0000 0800 0000 0900  ................
+000023d0: 0000 4300 0000 73ec 0100 007c 006a 00a0  ..C...s....|.j..
+000023e0: 01a1 0072 1674 02a0 037c 006a 00a1 0101  ...r.t...|.j....
+000023f0: 007c 00a0 047c 01a1 0173 2e74 0564 017c  .|...|...s.t.d.|
+00002400: 019b 009d 0283 0182 017c 00a0 0664 02a1  .........|...d..
+00002410: 0164 0364 0464 0564 067c 0167 067d 0474  .d.d.d.d.|.g.}.t
+00002420: 076a 0864 076b 0272 727c 0264 086b 0272  .j.d.k.rr|.d.k.r
+00002430: 727c 006a 0972 727c 0464 0967 0137 007d  r|.j.rr|.d.g.7.}
+00002440: 0464 0464 0a64 0b67 037d 056e 147c 0464  .d.d.d.g.}.n.|.d
+00002450: 0c7c 0264 0d64 0967 0437 007d 0467 007d  .|.d.d.g.7.}.g.}
+00002460: 057c 006a 0a7c 0474 0b6a 0c7c 006a 0d64  .|.j.|.t.j.|.j.d
+00002470: 0e8d 0301 007c 0572 b27c 006a 0a7c 0574  .....|.r.|.j.|.t
+00002480: 0b6a 0c7c 006a 0064 0e8d 0301 007c 00a0  .j.|.j.d.....|..
+00002490: 0ea1 0001 007c 00a0 0664 02a1 0164 0f64  .....|...d...d.d
+000024a0: 107c 006a 0f72 d67c 006a 1073 d664 116e  .|.j.r.|.j.s.d.n
+000024b0: 0264 129b 009d 0264 1364 147c 006a 099b  .d.....d.d.|.j..
+000024c0: 009d 0264 157c 00a0 0664 16a1 017c 006a  ...d.|...d...|.j
+000024d0: 0064 171b 007c 0367 097d 067c 006a 0a7c  .d...|.g.}.|.j.|
+000024e0: 0674 0b6a 0c7c 006a 0064 0e8d 0301 007c  .t.j.|.j.d.....|
+000024f0: 006a 1090 0172 267c 00a0 117c 03a1 0101  .j...r&|...|....
+00002500: 007c 00a0 0664 02a1 0164 187c 006a 129b  .|...d...d.|.j..
+00002510: 009d 0264 107c 006a 0f9b 009d 0264 1364  ...d.|.j.....d.d
+00002520: 147c 006a 099b 009d 0264 1967 067d 077c  .|.j.....d.g.}.|
+00002530: 0364 1a6b 0290 0172 6a7c 07a0 1364 1ba1  .d.k...rj|...d..
+00002540: 0101 006e 0a7c 07a0 1364 1ca1 0101 007c  ...n.|...d.....|
+00002550: 006a 1490 0172 8c74 157c 006a 1483 017c  .j...r.t.|.j...|
+00002560: 006a 1664 1d3c 007c 07a0 177c 00a0 0664  .j.d.<.|...|...d
+00002570: 1ea1 0164 1f74 157c 006a 0064 201b 0083  ...d.t.|.j.d ...
+00002580: 0164 217c 006a 189b 0064 2267 06a1 0101  .d!|.j...d"g....
+00002590: 007c 006a 0a7c 077c 006a 0064 238d 0201  .|.j.|.|.j.d#...
+000025a0: 007c 00a0 197c 03a1 0101 007c 006a 1290  .|...|.....|.j..
+000025b0: 0172 e07c 00a0 1aa1 0001 007c 00a0 1ba1  .r.|.......|....
+000025c0: 0001 0064 2453 0029 257a f542 7569 6c64  ...d$S.)%z.Build
+000025d0: 2052 6564 6973 4149 2066 726f 6d20 6769   RedisAI from gi
+000025e0: 740a 2020 2020 2020 2020 3a70 6172 616d  t.        :param
+000025f0: 2067 6974 5f75 726c 3a20 7572 6c20 6672   git_url: url fr
+00002600: 6f6d 2077 6869 6368 2074 6f20 7265 7472  om which to retr
+00002610: 6965 7665 2052 6564 6973 4149 0a20 2020  ieve RedisAI.   
+00002620: 2020 2020 203a 7479 7065 2067 6974 5f75       :type git_u
+00002630: 726c 3a20 7374 720a 2020 2020 2020 2020  rl: str.        
+00002640: 3a70 6172 616d 2062 7261 6e63 683a 2062  :param branch: b
+00002650: 7261 6e63 6820 746f 2063 6865 636b 6f75  ranch to checkou
+00002660: 740a 2020 2020 2020 2020 3a74 7970 6520  t.        :type 
+00002670: 6272 616e 6368 3a20 7374 720a 2020 2020  branch: str.    
+00002680: 2020 2020 3a70 6172 616d 2064 6576 6963      :param devic
+00002690: 653a 2063 7075 206f 7220 6770 750a 2020  e: cpu or gpu.  
+000026a0: 2020 2020 2020 3a74 7970 6520 6465 7669        :type devi
+000026b0: 6365 3a20 7374 720a 2020 2020 2020 2020  ce: str.        
+000026c0: 7a17 4d61 6c66 6f72 6d65 6420 5265 6469  z.Malformed Redi
+000026d0: 7341 4920 5552 4c3a 2072 1800 0000 7a15  sAI URL: r....z.
+000026e0: 4749 545f 4c46 535f 534b 4950 5f53 4d55  GIT_LFS_SKIP_SMU
+000026f0: 4447 453d 3172 6c00 0000 726d 0000 007a  DGE=1rl...rm...z
+00002700: 0b2d 2d72 6563 7572 7369 7665 da06 6461  .--recursive..da
+00002710: 7277 696e 7a06 7631 2e32 2e37 7284 0000  rwinz.v1.2.7r...
+00002720: 005a 0863 6865 636b 6f75 745a 2836 3334  .Z.checkoutZ(634
+00002730: 3931 3663 3732 3265 3731 3863 6336 6561  916c722e718cc6ea
+00002740: 3366 6164 3436 6536 3366 3764 3739 3866  3fad46e63f7d798f
+00002750: 3961 6463 3272 6e00 0000 7a09 2d2d 6465  9adc2rn...z.--de
+00002760: 7074 683d 3129 0272 2200 0000 724e 0000  pth=1).r"...rN..
+00002770: 007a 0957 4954 485f 5054 3d30 7a08 5749  .z.WITH_PT=0z.WI
+00002780: 5448 5f54 463d 7215 0000 0072 0100 0000  TH_TF=r....r....
+00002790: 7a0d 5749 5448 5f54 464c 4954 453d 307a  z.WITH_TFLITE=0z
+000027a0: 0957 4954 485f 4f52 543d 7a09 5645 5242  .WITH_ORT=z.VERB
+000027b0: 4f53 453d 315a 0462 6173 687a 0b67 6574  OSE=1Z.bashz.get
+000027c0: 5f64 6570 732e 7368 7a08 5749 5448 5f50  _deps.shz.WITH_P
+000027d0: 543d 7a11 5749 5448 5f55 4e49 545f 5445  T=z.WITH_UNIT_TE
+000027e0: 5354 533d 305a 0367 7075 7a05 4750 553d  STS=0Z.gpuz.GPU=
+000027f0: 317a 0547 5055 3d30 5a09 546f 7263 685f  1z.GPU=0Z.Torch_
+00002800: 4449 5272 7100 0000 7a02 2d43 da03 6f70  DIRrq...z.-C..op
+00002810: 7472 7200 0000 da05 6275 696c 6472 7000  trr.....buildrp.
+00002820: 0000 4e29 1c72 8500 0000 7224 0000 0072  ..N).r....r$...r
+00002830: 3000 0000 7249 0000 0072 4800 0000 7210  0...rI...rH...r.
+00002840: 0000 0072 3200 0000 da03 7379 73da 0870  ...r2.....sys..p
+00002850: 6c61 7466 6f72 6d72 8100 0000 725a 0000  latformr....rZ..
+00002860: 0072 2000 0000 7221 0000 0072 1d00 0000  .r ...r!...r....
+00002870: 728d 0000 0072 8000 0000 7282 0000 0072  r....r....r....r
+00002880: 9600 0000 727f 0000 00da 0661 7070 656e  ....r......appen
+00002890: 6472 8300 0000 724a 0000 0072 1800 0000  dr....rJ...r....
+000028a0: da06 6578 7465 6e64 7226 0000 00da 115f  ..extendr&....._
+000028b0: 696e 7374 616c 6c5f 6261 636b 656e 6473  install_backends
+000028c0: da10 5f6d 6f76 655f 746f 7263 685f 6c69  .._move_torch_li
+000028d0: 6273 724b 0000 0029 0872 2700 0000 7277  bsrK...).r'...rw
+000028e0: 0000 0072 7800 0000 7295 0000 0072 7900  ...rx...r....ry.
+000028f0: 0000 5a10 6368 6563 6b6f 7574 5f6f 7378  ..Z.checkout_osx
+00002900: 5f66 6978 5a07 6465 705f 636d 6472 7a00  _fixZ.dep_cmdrz.
+00002910: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00002920: 0072 2f00 0000 7701 0000 7396 0000 0000  .r/...w...s.....
+00002930: 0a0a 010c 030a 010e 0408 0102 0102 0102  ................
+00002940: 0102 0102 fa04 0a18 020a 0202 0102 0102  ................
+00002950: fd06 0702 0102 0102 0102 0102 fc06 0604  ................
+00002960: 0214 0104 0104 0102 0004 0004 ff06 0508  ................
+00002970: 0408 0102 0118 0102 010a 0102 0108 0108  ................
+00002980: 0102 f704 0c04 0102 0104 0104 fd06 0608  ................
+00002990: 010a 0308 010a 010a 0102 010a 0102 fa04  ................
+000029a0: 090a 010c 020a 0208 0110 0204 0208 0102  ................
+000029b0: 010c 0102 0106 0102 fa02 ff04 0a10 020a  ................
+000029c0: 0108 0108 017a 1d52 6564 6973 4149 4275  .....z.RedisAIBu
+000029d0: 696c 6465 722e 6275 696c 645f 6672 6f6d  ilder.build_from
+000029e0: 5f67 6974 6302 0000 0000 0000 0000 0000  _gitc...........
+000029f0: 0004 0000 0005 0000 0043 0000 0073 6c00  .........C...sl.
+00002a00: 0000 7c00 6a00 a001 6401 7c01 9b00 9d02  ..|.j...d.|.....
+00002a10: a101 a002 a100 7c00 5f03 7c00 6a03 6402  ......|._.|.j.d.
+00002a20: 1b00 7d02 7c00 6a03 6403 1b00 7d03 7c02  ..}.|.j.d...}.|.
+00002a30: a004 a100 7268 7c03 a005 a100 7268 7c00  ....rh|.....rh|.
+00002a40: 6a06 7c03 7c00 6a07 6403 1b00 6404 6405  j.|.|.j.d...d.d.
+00002a50: 8d03 0100 7c00 6a08 7c02 7c00 6a07 6402  ....|.j.|.|.j.d.
+00002a60: 1b00 6404 6405 8d03 0100 6406 5300 2907  ..d.d.....d.S.).
+00002a70: 7a72 4d6f 7665 2062 6163 6b65 6e64 206c  zrMove backend l
+00002a80: 6962 7261 7269 6573 2074 6f20 736d 6172  ibraries to smar
+00002a90: 7473 696d 2f5f 636f 7265 2f6c 6962 2f0a  tsim/_core/lib/.
+00002aa0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+00002ab0: 6576 6963 653a 2063 7075 206f 7220 6370  evice: cpu or cp
+00002ac0: 750a 2020 2020 2020 2020 3a74 7970 6520  u.        :type 
+00002ad0: 6465 7669 6365 3a20 7374 720a 2020 2020  device: str.    
+00002ae0: 2020 2020 7a08 696e 7374 616c 6c2d 7287      z.install-r.
+00002af0: 0000 0072 8600 0000 5472 3f00 0000 4e29  ...r....Tr?...N)
+00002b00: 0972 8500 0000 7288 0000 0072 7500 0000  .r....r....ru...
+00002b10: 5a10 7261 695f 696e 7374 616c 6c5f 7061  Z.rai_install_pa
+00002b20: 7468 7289 0000 0072 2400 0000 7241 0000  thr....r$...rA..
+00002b30: 0072 1f00 0000 723c 0000 0029 0472 2700  .r....r<...).r'.
+00002b40: 0000 7295 0000 005a 0772 6169 5f6c 6962  ..r....Z.rai_lib
+00002b50: 5a0c 7261 695f 6261 636b 656e 6473 720d  Z.rai_backendsr.
+00002b60: 0000 0072 0d00 0000 720e 0000 0072 9e00  ...r....r....r..
+00002b70: 0000 e601 0000 7310 0000 0000 0506 0108  ......s.........
+00002b80: ff0a 030a 010a 0210 0116 017a 2052 6564  ...........z Red
+00002b90: 6973 4149 4275 696c 6465 722e 5f69 6e73  isAIBuilder._ins
+00002ba0: 7461 6c6c 5f62 6163 6b65 6e64 7363 0100  tall_backendsc..
+00002bb0: 0000 0000 0000 0000 0000 0600 0000 0500  ................
+00002bc0: 0000 4300 0000 7368 0000 007c 006a 0064  ..C...sh...|.j.d
+00002bd0: 011b 0064 021b 007d 017c 0164 031b 007d  ...d...}.|.d...}
+00002be0: 0274 017c 006a 0283 016a 036a 036a 037d  .t.|.j...j.j.j.}
+00002bf0: 037c 0364 031b 007d 047c 006a 047c 047c  .|.d...}.|.j.|.|
+00002c00: 0264 0464 058d 0301 0074 056a 0664 066b  .d.d.....t.j.d.k
+00002c10: 0272 647c 0364 071b 007d 057c 006a 047c  .rd|.d...}.|.j.|
+00002c20: 057c 0164 071b 0064 0464 058d 0301 0064  .|.d...d.d.....d
+00002c30: 0853 0029 097a de4d 6f76 6520 7069 7020  .S.).z.Move pip 
+00002c40: 696e 7374 616c 6c20 746f 7263 6820 6c69  install torch li
+00002c50: 6272 6172 6965 730a 2020 2020 2020 2020  braries.        
+00002c60: 5369 6e63 6520 7765 2075 7365 2070 6970  Since we use pip
+00002c70: 2069 6e73 7461 6c6c 6564 2074 6f72 6368   installed torch
+00002c80: 206c 6962 7261 7269 6573 2066 6f72 2062   libraries for b
+00002c90: 7569 6c64 696e 670a 2020 2020 2020 2020  uilding.        
+00002ca0: 5265 6469 7341 492c 2077 6520 6e65 6564  RedisAI, we need
+00002cb0: 2074 6f20 6d6f 7665 2074 6865 6d20 696e   to move them in
+00002cc0: 746f 2074 6865 204c 445f 7275 6e70 6174  to the LD_runpat
+00002cd0: 6820 6f66 2072 6564 6973 6169 2e73 6f0a  h of redisai.so.
+00002ce0: 2020 2020 2020 2020 696e 2074 6865 2073          in the s
+00002cf0: 6d61 7274 7369 6d2f 5f63 6f72 652f 6c69  martsim/_core/li
+00002d00: 6220 6469 7265 6374 6f72 792e 0a20 2020  b directory..   
+00002d10: 2020 2020 2072 8600 0000 5a0d 7265 6469       r....Z.redi
+00002d20: 7361 695f 746f 7263 6872 1700 0000 5472  sai_torchr....Tr
+00002d30: 3f00 0000 7297 0000 007a 072e 6479 6c69  ?...r....z..dyli
+00002d40: 6273 4e29 0772 1f00 0000 7202 0000 0072  bsN).r....r....r
+00002d50: 8300 0000 721a 0000 0072 4100 0000 729a  ....r....rA...r.
+00002d60: 0000 0072 9b00 0000 2906 7227 0000 005a  ...r....).r'...Z
+00002d70: 1173 735f 7261 695f 746f 7263 685f 7061  .ss_rai_torch_pa
+00002d80: 7468 5a15 7373 5f72 6169 5f74 6f72 6368  thZ.ss_rai_torch
+00002d90: 5f6c 6962 5f70 6174 685a 0e70 6970 5f74  _lib_pathZ.pip_t
+00002da0: 6f72 6368 5f70 6174 685a 1270 6970 5f74  orch_pathZ.pip_t
+00002db0: 6f72 6368 5f6c 6962 5f70 6174 685a 0664  orch_lib_pathZ.d
+00002dc0: 796c 6962 7372 0d00 0000 720d 0000 0072  ylibsr....r....r
+00002dd0: 0e00 0000 729f 0000 00f5 0100 0073 1000  ....r........s..
+00002de0: 0000 0007 0e01 0806 1001 0802 1003 0a01  ................
+00002df0: 0801 7a1f 5265 6469 7341 4942 7569 6c64  ..z.RedisAIBuild
+00002e00: 6572 2e5f 6d6f 7665 5f74 6f72 6368 5f6c  er._move_torch_l
+00002e10: 6962 7329 0e72 1100 0000 7212 0000 0072  ibs).r....r....r
+00002e20: 1300 0000 725b 0000 0072 2900 0000 725e  ....r[...r)...r^
+00002e30: 0000 0072 8500 0000 722e 0000 0072 8d00  ...r....r....r..
+00002e40: 0000 7296 0000 0072 2f00 0000 729e 0000  ..r....r/...r...
+00002e50: 0072 9f00 0000 727c 0000 0072 0d00 0000  .r....r|...r....
+00002e60: 720d 0000 0072 6500 0000 720e 0000 0072  r....re...r....r
+00002e70: 7d00 0000 0b01 0000 7326 0000 0008 0104  }.......s&......
+00002e80: 0902 0102 0102 0102 0102 0102 0102 0102  ................
+00002e90: f70e 1402 010a 0302 010a 0508 0f08 3708  ..............7.
+00002ea0: 6f08 0f72 7d00 0000 2910 7205 0000 0072  o..r}...).r....r
+00002eb0: 4400 0000 7230 0000 0072 3500 0000 7220  D...r0...r5...r 
+00002ec0: 0000 0072 9a00 0000 da07 7061 7468 6c69  ...r......pathli
+00002ed0: 6272 0200 0000 7203 0000 0072 0400 0000  br....r....r....
+00002ee0: 720f 0000 00da 0945 7863 6570 7469 6f6e  r......Exception
+00002ef0: 7210 0000 0072 1400 0000 725f 0000 0072  r....r....r_...r
+00002f00: 7d00 0000 720d 0000 0072 0d00 0000 720d  }...r....r....r.
+00002f10: 0000 0072 0e00 0000 da08 3c6d 6f64 756c  ...r......<modul
+00002f20: 653e 1b00 0000 731a 0000 0008 0108 0108  e>....s.........
+00002f30: 0108 0108 0108 010c 010c 010c 0a08 1410  ................
+00002f40: 040e 6810 5e                             ..h.^
```

### Comparing `smartsim-0.4.1/smartsim/_core/_install/buildenv.py` & `smartsim-0.4.2/smartsim/_core/_install/buildenv.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+# BSD 2-Clause License
+#
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+# 1. Redistributions of source code must retain the above copyright notice, this
+#    list of conditions and the following disclaimer.
+#
+# 2. Redistributions in binary form must reproduce the above copyright notice,
+#    this list of conditions and the following disclaimer in the documentation
+#    and/or other materials provided with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
 import os
 import platform
 import site
 import subprocess
 import sys
 from pathlib import Path
 from typing import Iterable
@@ -112,61 +138,91 @@
 
     1. It is used to populate the [ml] ``extras_require`` of the setup.py.
     This is because the RedisAI version will determine which ML based
     dependencies are required.
 
     2. Used to set the default values for PyTorch, TF, and ONNX
     given the SMARTSIM_REDISAI env var set by the user.
+
+    NOTE: Torch requires additional information depending on whether
+    CPU or GPU support is requested
     """
 
     defaults = {
-        "1.2.3": {
-            "tensorflow": "2.5.2",
-            "onnx": "1.9.0",
-            "skl2onnx": "1.10.3",
-            "onnxmltools": "1.10.0",
-            "scikit-learn": "1.0.2",
-            "torch": "1.7.1",
-            "torchvision": "0.8.2",
-        },
         "1.2.5": {
             "tensorflow": "2.6.2",
             "onnx": "1.9.0",
             "skl2onnx": "1.10.3",
             "onnxmltools": "1.10.0",
             "scikit-learn": "1.0.2",
             "torch": "1.9.1",
+            "torch_cpu_suffix": "+cpu",
+            "torch_cuda_suffix": "+cu111",
             "torchvision": "0.10.1",
         },
+        "1.2.7": {
+            "tensorflow": "2.8.0",
+            "onnx": "1.11.0",
+            "skl2onnx": "1.11.1",
+            "onnxmltools": "1.11.1",
+            "scikit-learn": "1.1.1",
+            "torch": "1.11.0",
+            "torch_cpu_suffix": "+cpu",
+            "torch_cuda_suffix": "+cu113",
+            "torchvision": "0.12.0",
+        },
     }
-    # deps are the same between the following versions
-    defaults["1.2.4"] = defaults["1.2.3"]
+    # Remove options with unsported wheels for python>=3.10
+    if sys.version_info >= (3, 10):
+        defaults.pop("1.2.5")
+        defaults["1.2.7"].pop("onnx")
+        defaults["1.2.7"].pop("skl2onnx")
+        defaults["1.2.7"].pop("onnxmltools")
+        defaults["1.2.7"].pop("scikit-learn")
+    # Remove incompatible RAI versions for OSX
+    if sys.platform == "darwin":
+        defaults.pop("1.2.5", None)
 
     def __init__(self, vers):
+        min_rai_version = min(Version_(ver) for ver in self.defaults)
+        if min_rai_version > vers:
+            raise SetupError(
+                f"RedisAI version must be greater than or equal to {min_rai_version}"
+            )
         if vers not in self.defaults:
             if vers.startswith("1.2"):
                 # resolve to latest version for 1.2.x
                 # the str representation will still be 1.2.x
-                self.version = "1.2.5"
+                self.version = "1.2.7"
             else:
                 raise SetupError(
                     f"Invalid RedisAI version {vers}. Options are {self.defaults.keys()}"
                 )
         else:
             self.version = vers
 
     def __getattr__(self, name):
-        return self.defaults[self.version][name]
+        try:
+            return self.defaults[self.version][name]
+        except KeyError:
+            raise AttributeError(
+                f"'{type(self).__name__}' object has no attribute '{name}'\n\n"
+                "This is likely a problem with the SmartSim build process;"
+                "if this problem persists please log a new issue at "
+                "https://github.com/CrayLabs/SmartSim/issues "
+                "or get in contact with us at "
+                "https://www.craylabs.org/docs/community.html"
+            ) from None
 
     def get_defaults(self):
-        return self.defaults[self.version]
+        return self.defaults[self.version].copy()
 
 
 class Versioner:
-    """Versioner is responsible fo managing all the versions
+    """Versioner is responsible for managing all the versions
     within SmartSim including SmartSim itself.
 
     SmartSim's version is written into version.py upon pip install
     by using this class in setup.py. By setting SMARTSIM_SUFFIX,
     the version will be written as a "dirty" version with the
     git-sha appended.
     i.e.
@@ -174,86 +230,102 @@
         pip install -e .
         smartsim.__version__ == 0.3.2+nightly-3fe23ff
 
     Versioner manages third party dependencies and their versions
     as well. These versions are used by the ``smart`` cli in the
     ``smart build`` command to determine which dependency versions
     to look for and download.
+
+    Default versions for SmartSim, SmartRedis, Redis, and RedisAI are
+    all set here. Setting a default version for RedisAI also dictates
+    default versions of the machine learning libraries.
     """
 
     # compatible Python version
-    PYTHON_MIN = Version_("3.7.0")
+    PYTHON_MIN = Version_("3.8.0")
 
     # Versions
-    SMARTSIM = Version_(get_env("SMARTSIM_VERSION", "0.4.1"))
-    SMARTREDIS = Version_(get_env("SMARTREDIS_VERSION", "0.3.1"))
+    SMARTSIM = Version_(get_env("SMARTSIM_VERSION", "0.4.2"))
+    SMARTREDIS = Version_(get_env("SMARTREDIS_VERSION", "0.4.0"))
     SMARTSIM_SUFFIX = get_env("SMARTSIM_SUFFIX", "")
 
     # Redis
-    REDIS = Version_(get_env("SMARTSIM_REDIS", "6.0.8"))
+    REDIS = Version_(get_env("SMARTSIM_REDIS", "7.0.5"))
     REDIS_URL = get_env("SMARTSIM_REDIS_URL", "https://github.com/redis/redis.git/")
     REDIS_BRANCH = get_env("SMARTSIM_REDIS_BRANCH", REDIS)
 
     # RedisAI
-    REDISAI = RedisAIVersion(get_env("SMARTSIM_REDISAI", "1.2.3"))
+    REDISAI = RedisAIVersion(get_env("SMARTSIM_REDISAI", "1.2.7"))
     REDISAI_URL = get_env(
         "SMARTSIM_REDISAI_URL", "https://github.com/RedisAI/RedisAI.git/"
     )
     REDISAI_BRANCH = get_env("SMARTSIM_REDISAI_BRANCH", f"v{REDISAI}")
 
     # ML/DL (based on RedisAI version defaults)
     # torch can be set by the user because we download that for them
     TORCH = Version_(get_env("SMARTSIM_TORCH", REDISAI.torch))
     TORCHVISION = Version_(get_env("SMARTSIM_TORCHVIS", REDISAI.torchvision))
+    TORCH_CPU_SUFFIX = Version_(get_env("TORCH_CPU_SUFFIX", REDISAI.torch_cpu_suffix))
+    TORCH_CUDA_SUFFIX = Version_(
+        get_env("TORCH_CUDA_SUFFIX", REDISAI.torch_cuda_suffix)
+    )
 
     # TensorFlow and ONNX only use the defaults, but these are not built into
     # the RedisAI package and therefore the user is free to pick other versions.
     TENSORFLOW = Version_(REDISAI.tensorflow)
-    ONNX = Version_(REDISAI.onnx)
+    try:
+        ONNX = Version_(REDISAI.onnx)
+    except AttributeError:
+        ONNX = None
 
     def as_dict(self, db_name="REDIS"):
         packages = [
             "SMARTSIM",
             "SMARTREDIS",
             db_name,
             "REDISAI",
             "TORCH",
             "TENSORFLOW",
-            "ONNX",
         ]
         versions = [
             self.SMARTSIM,
             self.SMARTREDIS,
             self.REDIS,
             self.REDISAI,
             self.TORCH,
             self.TENSORFLOW,
-            self.ONNX,
         ]
+        if self.ONNX:
+            packages.append("ONNX")
+            versions.append(self.ONNX)
         vers = {"Packages": packages, "Versions": versions}
         return vers
 
     def ml_extras_required(self):
         """Optional ML/DL dependencies we suggest for the user.
 
         The defaults are based on the RedisAI version
         """
-        ml_extras = []
         ml_defaults = self.REDISAI.get_defaults()
 
-        # remove torch and torch vision as they will be installed
+        # remove torch-related fields as they will be installed
         # by the cli process for use in the RAI build. We don't install
         # them here as the user needs to decide between GPU/CPU. All other
-        # libraries work on both devices
-        del ml_defaults["torch"]
-        del ml_defaults["torchvision"]
-
-        for lib, vers in ml_defaults.items():
-            ml_extras.append(f"{lib}=={vers}")
-        return ml_extras
+        # libraries work on both devices. The correct versions and suffixes
+        # were scraped from https://pytorch.org/get-started/previous-versions/
+        _torch_fields = [
+            "torch",
+            "torchvision",
+            "torch_cpu_suffix",
+            "torch_cuda_suffix",
+        ]
+        for field in _torch_fields:
+            ml_defaults.pop(field)
+
+        return [f"{lib}=={vers}" for lib, vers in ml_defaults.items()]
 
     def get_sha(self, setup_py_dir) -> str:
         """Get the git sha of the current branch"""
         try:
             sha = (
                 subprocess.check_output(["git", "rev-parse", "HEAD"], cwd=setup_py_dir)
                 .decode("ascii")
@@ -456,15 +528,15 @@
             env["CUDNN_INCLUDE_DIR"] = env["CUDNN_INCLUDE_PATH"]
             env["CUDNN_LIBRARY"] = env["CUDNN_LIBRARY_PATH"]
         return env
 
     def check_build_dependency(self, command):
         # TODO expand this to parse and check versions.
         try:
-            out = subprocess.check_call(
+            subprocess.check_call(
                 [command, "--version"],
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
             )
         except OSError:
             raise SetupError(f"{command} must be installed to build SmartSim") from None
```

### Comparing `smartsim-0.4.1/smartsim/_core/_install/builder.py` & `smartsim-0.4.2/smartsim/_core/_install/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,42 @@
+# BSD 2-Clause License
+#
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+# 1. Redistributions of source code must retain the above copyright notice, this
+#    list of conditions and the following disclaimer.
+#
+# 2. Redistributions in binary form must reproduce the above copyright notice,
+#    this list of conditions and the following disclaimer in the documentation
+#    and/or other materials provided with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
 import os
 import re
 import shutil
 import stat
 import subprocess
 import sys
 from pathlib import Path
-from subprocess import SubprocessError
 from shutil import which
+from subprocess import SubprocessError
 
 # NOTE: This will be imported by setup.py and hence no
 #       smartsim related items should be imported into
 #       this file.
 
 # TODO:
 #   - check cmake version and use system if possible to avoid conflicts
@@ -31,14 +57,15 @@
         if os.path.isfile(exe) and os.access(exe, os.X_OK):
             return os.path.abspath(exe)
         if os.path.isfile(exe) and not os.access(exe, os.X_OK):
             raise TypeError(f"File, {exe}, is not an executable")
         raise FileNotFoundError(f"Could not locate executable {exe}")
     return os.path.abspath(in_path)
 
+
 class BuildError(Exception):
     pass
 
 
 class Builder:
     """Base class for building third-party libraries"""
 
@@ -222,23 +249,24 @@
         dependency_path = os.environ.get("SMARTSIM_DEP_INSTALL_PATH", core_path)
         bin_path = Path(dependency_path, "bin").resolve()
         try:
             database_exe = next(bin_path.glob("*-server"))
             database = Path(os.environ.get("REDIS_PATH", database_exe)).resolve()
             _ = expand_exe_path(str(database))
         except (TypeError, FileNotFoundError) as e:
-            raise SSConfigError("Installation of redis-server failed!") from e
+            raise BuildError("Installation of redis-server failed!") from e
 
         # validate install -- redis-cli
         try:
             redis_cli_exe = next(bin_path.glob("*-cli"))
             redis_cli = Path(os.environ.get("REDIS_CLI_PATH", redis_cli_exe)).resolve()
             _ = expand_exe_path(str(redis_cli))
         except (TypeError, FileNotFoundError) as e:
-            raise SSConfigError("Installation of redis-cli failed!") from e
+            raise BuildError("Installation of redis-cli failed!") from e
+
 
 class RedisAIBuilder(Builder):
     """Class to build RedisAI from Source
     Supported build method:
      - from git
     See buildenv.py for buildtime configuration of RedisAI
     version and url.
@@ -252,24 +280,27 @@
         build_torch=True,
         build_tf=True,
         build_onnx=False,
         jobs=None,
         verbose=False,
     ):
         super().__init__(build_env, jobs=jobs, verbose=verbose)
-        self.rai_build_path = Path(self.build_dir, "RedisAI")
 
         # convert to int for RAI build script
         self.torch = 1 if build_torch else 0
         self.tf = 1 if build_tf else 0
         self.onnx = 1 if build_onnx else 0
         self.libtf_dir = libtf_dir
         self.torch_dir = torch_dir
 
     @property
+    def rai_build_path(self):
+        return Path(self.build_dir, "RedisAI")
+
+    @property
     def is_built(self):
         server = self.lib_path.joinpath("backends").is_dir()
         cli = self.lib_path.joinpath("redisai.so").is_file()
         return server and cli
 
     def copy_tf_cmake(self):
         """Copy the FindTensorFlow.cmake file to the build directory
@@ -346,15 +377,14 @@
         :param git_url: url from which to retrieve RedisAI
         :type git_url: str
         :param branch: branch to checkout
         :type branch: str
         :param device: cpu or gpu
         :type device: str
         """
-
         # delete previous build dir (should never be there)
         if self.rai_build_path.is_dir():
             shutil.rmtree(self.rai_build_path)
 
         # Check RedisAI URL
         if not self.is_valid_url(git_url):
             raise BuildError(f"Malformed RedisAI URL: {git_url}")
@@ -363,20 +393,40 @@
         clone_cmd = [
             self.binary_path("env"),
             "GIT_LFS_SKIP_SMUDGE=1",
             "git",
             "clone",
             "--recursive",
             git_url,
-            "--branch",
-            branch,
-            "--depth=1",
-            "RedisAI",
         ]
+        # Circumvent a bad `get_deps.sh` script from RAI on 1.2.7 with ONNX
+        # TODO: Look for a better way to do this or wait for RAI patch
+        if sys.platform == "darwin" and branch == "v1.2.7" and self.onnx:
+            # Clone RAI patch commit for OSX
+            clone_cmd += ["RedisAI"]
+            checkout_osx_fix = [
+                "git",
+                "checkout",
+                "634916c722e718cc6ea3fad46e63f7d798f9adc2",
+            ]
+        else:
+            # Clone RAI release commit
+            clone_cmd += [
+                "--branch",
+                branch,
+                "--depth=1",
+                "RedisAI",
+            ]
+            checkout_osx_fix = []
+
         self.run_command(clone_cmd, out=subprocess.DEVNULL, cwd=self.build_dir)
+        if checkout_osx_fix:
+            self.run_command(
+                checkout_osx_fix, out=subprocess.DEVNULL, cwd=self.rai_build_path
+            )
 
         # copy FindTensorFlow.cmake to RAI cmake dir
         self.copy_tf_cmake()
 
         # get RedisAI dependencies
         dep_cmd = [
             self.binary_path("env"),
```

### Comparing `smartsim-0.4.1/smartsim/_core/bin/modules/FindTensorFlow.cmake` & `smartsim-0.4.2/smartsim/_core/bin/modules/FindTensorFlow.cmake`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.1/smartsim/_core/config/config.py` & `smartsim-0.4.2/smartsim/_core/config/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -142,14 +142,18 @@
         return os.environ.get("SMARTSIM_LOG_LEVEL", "info")
 
     @property
     def jm_interval(self) -> int:
         return int(os.environ.get("SMARTSIM_JM_INTERVAL", 10))
 
     @property
+    def wlm_trials(self) -> int:
+        return int(os.environ.get("SMARTSIM_WLM_TRIALS", 10))
+
+    @property
     def test_launcher(self) -> str:
         return os.environ.get("SMARTSIM_TEST_LAUNCHER", "local")
 
     @property
     def test_device(self) -> str:
         return os.environ.get("SMARTSIM_TEST_DEVICE", "CPU")
```

### Comparing `smartsim-0.4.1/smartsim/_core/config/keydb.conf` & `smartsim-0.4.2/smartsim/_core/config/keydb.conf`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.1/smartsim/_core/config/redis6.conf` & `smartsim-0.4.2/smartsim/_core/config/redis6.conf`

 * *Files identical despite different names*

### Comparing `smartsim-0.4.1/smartsim/_core/control/controller.py` & `smartsim-0.4.2/smartsim/_core/control/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -286,40 +286,46 @@
                 )
             if self.orchestrator_active:
                 msg = "Attempted to launch a second Orchestrator instance. "
                 msg += "Only 1 Orchestrator can be active at a time"
                 raise SmartSimError(msg)
             self._launch_orchestrator(orchestrator)
 
-        for rc in manifest.ray_clusters:  # cov-wlm
-            rc._update_workers()
-
         if self.orchestrator_active:
             self._set_dbobjects(manifest)
 
         # create all steps prior to launch
         steps = []
-        all_entity_lists = manifest.ensembles + manifest.ray_clusters
+        all_entity_lists = manifest.ensembles
         for elist in all_entity_lists:
             if elist.batch:
                 batch_step = self._create_batch_job_step(elist)
                 steps.append((batch_step, elist))
             else:
                 # if ensemble is to be run as separate job steps, aka not in a batch
                 job_steps = [(self._create_job_step(e), e) for e in elist.entities]
                 steps.extend(job_steps)
 
-        # models themselves cannot be batch steps
+        # models themselves cannot be batch steps. If batch settings are
+        # attached, wrap them in an anonymous batch job step
         for model in manifest.models:
-            job_step = self._create_job_step(model)
-            steps.append((job_step, model))
+            if model.batch_settings:
+                anon_entity_list = _AnonymousBatchJob(
+                    model.name, model.path, model.batch_settings
+                )
+                anon_entity_list.entities.append(model)
+                batch_step = self._create_batch_job_step(anon_entity_list)
+                steps.append((batch_step, model))
+            else:
+                job_step = self._create_job_step(model)
+                steps.append((job_step, model))
 
         # launch steps
-        for job_step in steps:
-            self._launch_step(*job_step)
+        for step, entity in steps:
+            self._launch_step(step, entity)
 
     def _launch_orchestrator(self, orchestrator):
         """Launch an Orchestrator instance
 
         This function will launch the Orchestrator instance and
         if on WLM, find the nodes where it was launched and
         set them in the JobManager
@@ -377,15 +383,14 @@
 
         :param job_step: a job step instance
         :type job_step: Step
         :param entity: entity instance
         :type entity: SmartSimEntity
         :raises SmartSimError: if launch fails
         """
-
         try:
             job_id = self._launcher.run(job_step)
         except LauncherError as e:
             msg = f"An error occurred when launching {entity.name} \n"
             msg += "Check error and output files for details.\n"
             msg += f"{entity}"
             logger.error(msg)
@@ -456,18 +461,29 @@
                 client_env["SSKEYIN"] = ",".join(
                     [in_entity.name for in_entity in entity.incoming_entities]
                 )
             if entity.query_key_prefixing():
                 client_env["SSKEYOUT"] = entity.name
 
         # Set address to local if it's a colocated model
-        if hasattr(entity, "colocated"):
-            if entity.colocated:
-                port = entity.run_settings.colocated_db_settings["port"]
+        if hasattr(entity, "colocated") and entity.colocated:
+            port = entity.run_settings.colocated_db_settings.get("port", None)
+            socket = entity.run_settings.colocated_db_settings.get("unix_socket", None)
+            if socket and port:
+                raise SSInternalError(
+                    "Co-located was configured for both TCP/IP and UDS"
+                )
+            if port:
                 client_env["SSDB"] = f"127.0.0.1:{str(port)}"
+            elif socket:
+                client_env["SSDB"] = f"unix://{socket}"
+            else:
+                raise SSInternalError(
+                    "Colocated database was not configured for either TCP or UDS"
+                )
         entity.run_settings.update_env(client_env)
 
     def _save_orchestrator(self, orchestrator):
         """Save the orchestrator object via pickle
 
         This function saves the orchestrator information to a pickle
         file that can be imported by subsequent experiments to reconnect
@@ -626,7 +642,16 @@
                     # but avoid duplicates
                     for db_model in entity._db_models:
                         if db_model not in ensemble._db_models:
                             set_ml_model(db_model, client)
                     for db_script in entity._db_scripts:
                         if db_script not in ensemble._db_scripts:
                             set_script(db_script, client)
+
+
+class _AnonymousBatchJob(EntityList):
+    def __init__(self, name, path, batch_settings, **kwargs):
+        super().__init__(name, path)
+        self.batch_settings = batch_settings
+
+    def _initialize_entities(self, **kwargs):
+        ...
```

### Comparing `smartsim-0.4.1/smartsim/_core/control/job.py` & `smartsim-0.4.2/smartsim/_core/control/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/control/jobmanager.py` & `smartsim-0.4.2/smartsim/_core/control/jobmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/control/manifest.py` & `smartsim-0.4.2/smartsim/_core/control/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -23,21 +23,20 @@
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from ...database import Orchestrator
 from ...entity import EntityList, SmartSimEntity
 from ...error import SmartSimError
-from ...exp.ray import RayCluster
 from ..utils.helpers import fmt_dict
 
 # List of types derived from EntityList which require specific behavior
 # A corresponding property needs to exist (like db for Orchestrator),
 # otherwise they will not be accessible
-entity_list_exception_types = [Orchestrator, RayCluster]
+entity_list_exception_types = [Orchestrator]
 
 
 class Manifest:
     """This class is used to keep track of all deployables generated by an experiment.
     Different types of deployables (i.e. different `SmartSimEntity`-derived objects
     or `EntityList`-derived objects) can be accessed by using the corresponding accessor.
 
@@ -98,35 +97,22 @@
                         is_exceptional_type |= True
                 if not is_exceptional_type:
                     _ensembles.append(deployable)
 
         return _ensembles
 
     @property
-    def ray_clusters(self):
-        """Return all RayCluster instances in Manifest
-
-        :return: list of RayCluster instances
-        :rtype: List[RayCluster]
-        """
-        _ray_cluster = []
-        for deployable in self._deployables:
-            if isinstance(deployable, RayCluster):
-                _ray_cluster.append(deployable)
-        return _ray_cluster
-
-    @property
     def all_entity_lists(self):
         """All entity lists, including ensembles and
-        exceptional ones like Orchestrator and RayCluster
+        exceptional ones like Orchestrator
 
         :return: list of entity lists
         :rtype: List[EntityList]
         """
-        _all_entity_lists = self.ray_clusters + self.ensembles
+        _all_entity_lists = self.ensembles
         db = self.db
         if db is not None:
             _all_entity_lists.append(db)
 
         return _all_entity_lists
 
     def _check_names(self, deployables):
@@ -160,28 +146,30 @@
         s = ""
         e_header = "=== Ensembles ===\n"
         m_header = "=== Models ===\n"
         db_header = "=== Database ===\n"
         if self.ensembles:
             s += e_header
 
-            # include ray clusters as an ensemble while still in experimental API
-            all_ensembles = self.ensembles + self.ray_clusters
+            all_ensembles = self.ensembles
             for ensemble in all_ensembles:
                 s += f"{ensemble.name}\n"
                 s += f"Members: {len(ensemble)}\n"
                 s += f"Batch Launch: {ensemble.batch}\n"
                 if ensemble.batch:
                     s += f"{str(ensemble.batch_settings)}\n"
             s += "\n"
+
         if self.models:
             s += m_header
             for model in self.models:
                 s += f"{model.name}\n"
-                s += f"{str(model.run_settings)}\n"
+                if model.batch_settings:
+                    s += f"{model.batch_settings}\n"
+                s += f"{model.run_settings}\n"
                 if model.params:
                     s += f"Parameters: \n{fmt_dict(model.params)}\n"
             s += "\n"
 
         if self.db:
             s += db_header
             s += f"Shards: {self.db.num_shards}\n"
```

### Comparing `smartsim-0.4.1/smartsim/_core/entrypoints/colocated.py` & `smartsim-0.4.2/smartsim/_core/entrypoints/colocated.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023 Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -77,14 +77,17 @@
     parser.add_argument("--inputs", nargs="+", default=None)
     parser.add_argument("--outputs", nargs="+", default=None)
 
     # Unused if we use SmartRedis
     parser.add_argument("--min_batch_timeout", type=int, default=None)
     args = parser.parse_args(db_model)
 
+    inputs = None
+    outputs = None
+
     if args.inputs:
         inputs = list(args.inputs)
     if args.outputs:
         outputs = list(args.outputs)
 
     if args.devices_per_node == 1:
         client.set_model_from_file(
@@ -159,15 +162,17 @@
     command: List[str],
     db_models: List[List[str]],
     db_scripts: List[List[str]],
 ):
     global DBPID
 
     try:
-        ip_address = current_ip(network_interface)
+        ip_address = None
+        if network_interface:
+            ip_address = current_ip(network_interface)
         lo_address = current_ip("lo")
     except ValueError as e:
         logger.warning(e)
         ip_address = None
 
     if lo_address == ip_address or not ip_address:
         cmd = command + [f"--bind {lo_address}"]
@@ -262,15 +267,15 @@
 
 if __name__ == "__main__":
     try:
         parser = argparse.ArgumentParser(
             prefix_chars="+", description="SmartSim Process Launcher"
         )
         parser.add_argument(
-            "+ifname", type=str, help="Network Interface name", default="lo"
+            "+ifname", type=str, help="Network Interface name", default=""
         )
         parser.add_argument(
             "+lockfile", type=str, help="Filename to create for single proc per host"
         )
         parser.add_argument(
             "+db_cpus", type=int, default=2, help="Number of CPUs to use for DB"
         )
@@ -307,8 +312,8 @@
 
         main(args.ifname, args.db_cpus, args.command, args.db_model, args.db_script)
 
     # gracefully exit the processes in the distributed application that
     # we do not want to have start a colocated process. Only one process
     # per node should be running.
     except filelock.Timeout:
-        exit(0)
+        sys.exit(0)
```

### Comparing `smartsim-0.4.1/smartsim/_core/entrypoints/redis.py` & `smartsim-0.4.2/smartsim/_core/entrypoints/redis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023 Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/generation/generator.py` & `smartsim-0.4.2/smartsim/_core/generation/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -82,15 +82,14 @@
 
         """
         generator_manifest = Manifest(*args)
         self._gen_exp_dir()
         self._gen_orc_dir(generator_manifest.db)
         self._gen_entity_list_dir(generator_manifest.ensembles)
         self._gen_entity_dirs(generator_manifest.models)
-        self._gen_entity_list_dir(generator_manifest.ray_clusters)
 
     def set_tag(self, tag, regex=None):
         """Set the tag used for tagging input files
 
         Set a tag or a regular expression for the
         generator to look for when configuring new models.
```

### Comparing `smartsim-0.4.1/smartsim/_core/generation/modelwriter.py` & `smartsim-0.4.2/smartsim/_core/generation/modelwriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/cobalt/cobaltCommands.py` & `smartsim-0.4.2/smartsim/_core/control/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -19,7 +19,10 @@
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+from .controller import Controller
+from .manifest import Manifest
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/cobalt/cobaltLauncher.py` & `smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltLauncher.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -28,17 +28,25 @@
 
 import psutil
 
 from ....error import LauncherError
 from ....log import get_logger
 from ....settings import *
 from ....status import STATUS_CANCELLED, STATUS_COMPLETED
+from ...config import CONFIG
 from ..launcher import WLMLauncher
 from ..pbs.pbsCommands import qdel, qstat
-from ..step import AprunStep, CobaltBatchStep, LocalStep, MpirunStep
+from ..step import (
+    AprunStep,
+    CobaltBatchStep,
+    LocalStep,
+    MpiexecStep,
+    MpirunStep,
+    OrterunStep,
+)
 from ..stepInfo import CobaltStepInfo
 from .cobaltParser import parse_cobalt_step_id, parse_cobalt_step_status, parse_qsub_out
 
 logger = get_logger(__name__)
 
 
 class CobaltLauncher(WLMLauncher):
@@ -57,14 +65,16 @@
         self.user = psutil.Process().username()
 
     # RunSettings types supported by this launcher
     supported_rs = {
         AprunSettings: AprunStep,
         CobaltBatchSettings: CobaltBatchStep,
         MpirunSettings: MpirunStep,
+        MpiexecSettings: MpiexecStep,
+        OrterunSettings: OrterunStep,
         RunSettings: LocalStep,
     }
 
     def run(self, step):
         """Run a job step through Cobalt
 
         :param step: a job step instance
@@ -122,20 +132,21 @@
         else:
             self.task_manager.remove_task(stepmap.task_id)
 
         _, step_info = self.get_step_update([step_name])[0]
         step_info.status = STATUS_CANCELLED  # set status to cancelled instead of failed
         return step_info
 
-    def _get_cobalt_step_id(self, step, interval=4, trials=5):
+    def _get_cobalt_step_id(self, step, interval=2):
         """Get the step_id of a step from qstat (rarely used)
 
         Parses cobalt qstat output by looking for the step name
         """
         step_id = None
+        trials = CONFIG.wlm_trials
         while trials > 0:
             output, _ = qstat(["--header", "JobName:JobId", "-u", self.user])
             step_id = parse_cobalt_step_id(output, step.name)
             if step_id:
                 break
             else:
                 time.sleep(interval)
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/cobalt/cobaltParser.py` & `smartsim-0.4.2/smartsim/_core/launcher/cobalt/cobaltParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/colocated.py` & `smartsim-0.4.2/smartsim/_core/launcher/colocated.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023 Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -22,15 +22,15 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import sys
 
-from ...error import SSUnsupportedError
+from ...error import SSInternalError, SSUnsupportedError
 from ..config import CONFIG
 from ..utils.helpers import create_lockfile_name
 
 
 def write_colocated_launch_script(file_name, db_log, colocated_settings):
     """Write the colocated launch script
 
@@ -41,15 +41,15 @@
     :type file_name: str
     :param db_log: log file for the db
     :type db_log: str
     :param colocated_settings: db settings from entity run_settings
     :type colocated_settings: dict[str, Any]
     """
 
-    colocated_cmd = _build_colocated_wrapper_cmd(**colocated_settings, db_log=db_log)
+    colocated_cmd = _build_colocated_wrapper_cmd(db_log, **colocated_settings)
 
     with open(file_name, "w") as f:
         f.write("#!/bin/bash\n")
         f.write("set -e\n\n")
 
         f.write("Cleanup () {\n")
         f.write("if ps -p $DBPID > /dev/null; then\n")
@@ -71,30 +71,26 @@
             cpus = colocated_settings["cpus"]
             f.write(f"taskset -c 0-$(nproc --ignore={str(cpus+1)}) $@\n\n")
         else:
             f.write(f"$@\n\n")
 
 
 def _build_colocated_wrapper_cmd(
-    port=6780,
+    db_log,
     cpus=1,
-    interface="lo",
     rai_args=None,
     extra_db_args=None,
-    db_log=None,
+    port=6780,
+    ifname=None,
     **kwargs,
 ):
     """Build the command use to run a colocated db application
 
-    :param port: db port, defaults to 6780
-    :type port: int, optional
     :param cpus: db cpus, defaults to 1
     :type cpus: int, optional
-    :param interface: network interface, defaults to "lo"
-    :type interface: str, optional
     :param rai_args: redisai args, defaults to None
     :type rai_args: dict[str, str], optional
     :param extra_db_args: extra redis args, defaults to None
     :type extra_db_args: dict[str, str], optional
     :return: the command to run
     :rtype: str
     """
@@ -109,34 +105,56 @@
     # create the command that will be used to launch the
     # database with the python entrypoint for starting
     # up the backgrounded db process
     cmd = [
         sys.executable,
         "-m",
         "smartsim._core.entrypoints.colocated",
-        "+ifname",
-        interface,
         "+lockfile",
         lockfile,
         "+db_cpus",
         str(cpus),
-        "+command",
     ]
-
+    # Add in the interface if using TCP/IP
+    if ifname:
+        cmd.extend(["+ifname", ifname])
+    cmd.append("+command")
     # collect DB binaries and libraries from the config
     db_cmd = [CONFIG.database_exe, CONFIG.database_conf, "--loadmodule", CONFIG.redisai]
+
     # add extra redisAI configurations
     for arg, value in rai_args.items():
         if value:
             # RAI wants arguments for inference in all caps
             # ex. THREADS_PER_QUEUE=1
             db_cmd.append(f"{arg.upper()} {str(value)}")
 
-    # add port and log information
-    db_cmd.extend(["--port", str(port), "--logfile", db_log])  # usually /dev/null
+    db_cmd.extend(["--port", str(port)])
+
+    # Add socket and permissions for UDS
+    unix_socket = kwargs.get("unix_socket", None)
+    socket_permissions = kwargs.get("socket_permissions", None)
+
+    if unix_socket and socket_permissions:
+        db_cmd.extend(
+            [
+                "--unixsocket",
+                str(unix_socket),
+                "--unixsocketperm",
+                str(socket_permissions),
+            ]
+        )
+    elif bool(unix_socket) ^ bool(socket_permissions):
+        raise SSInternalError(
+            "`unix_socket` and `socket_permissions` must both be defined or undefined."
+        )
+
+    db_cmd.extend(
+        ["--logfile", db_log]
+    )  # usually /dev/null, unless debug was specified
     for db_arg, value in extra_db_args.items():
         # replace "_" with "-" in the db_arg because we use kwargs
         # for the extra configurations and Python doesn't allow a hyphen
         # in a variable name. All redis and KeyDB configuration options
         # use hyphens in their names.
         db_arg = db_arg.replace("_", "-")
         db_cmd.extend([f"--{db_arg}", value])
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/launcher.py` & `smartsim-0.4.2/smartsim/_core/launcher/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/local/local.py` & `smartsim-0.4.2/smartsim/_core/launcher/local/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/lsf/lsfCommands.py` & `smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfCommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/lsf/lsfLauncher.py` & `smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfLauncher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -26,16 +26,24 @@
 
 import time
 
 from ....error import LauncherError
 from ....log import get_logger
 from ....settings import *
 from ....status import STATUS_CANCELLED, STATUS_COMPLETED
+from ...config import CONFIG
 from ..launcher import WLMLauncher
-from ..step import BsubBatchStep, JsrunStep, LocalStep, MpirunStep
+from ..step import (
+    BsubBatchStep,
+    JsrunStep,
+    LocalStep,
+    MpiexecStep,
+    MpirunStep,
+    OrterunStep,
+)
 from ..stepInfo import LSFBatchStepInfo, LSFJsrunStepInfo
 from .lsfCommands import bjobs, bkill, jskill, jslist
 from .lsfParser import (
     parse_bjobs_jobid,
     parse_bsub,
     parse_jslist_stepid,
     parse_max_step_id_from_jslist,
@@ -58,14 +66,16 @@
     # init in WLMLauncher, launcher.py
 
     # RunSettings types supported by this launcher
     supported_rs = {
         JsrunSettings: JsrunStep,
         BsubBatchSettings: BsubBatchStep,
         MpirunSettings: MpirunStep,
+        MpiexecSettings: MpiexecStep,
+        OrterunSettings: OrterunStep,
         RunSettings: LocalStep,
     }
 
     def run(self, step):
         """Run a job step through LSF
 
         :param step: a job step instance
@@ -126,18 +136,19 @@
         else:
             self.task_manager.remove_task(stepmap.task_id)
 
         _, step_info = self.get_step_update([step_name])[0]
         step_info.status = STATUS_CANCELLED  # set status to cancelled instead of failed
         return step_info
 
-    def _get_lsf_step_id(self, step, interval=2, trials=5):
+    def _get_lsf_step_id(self, step, interval=2):
         """Get the step_id of last launched step from jslist"""
         time.sleep(interval)
         step_id = "unassigned"
+        trials = CONFIG.wlm_trials
         while trials > 0:
             output, _ = jslist([])
             step_id = parse_max_step_id_from_jslist(output)
             if step_id:
                 break
             else:
                 time.sleep(interval)
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/lsf/lsfParser.py` & `smartsim-0.4.2/smartsim/_core/launcher/lsf/lsfParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/pbs/pbsCommands.py` & `smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsCommands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/pbs/pbsLauncher.py` & `smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsLauncher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -26,16 +26,24 @@
 
 import time
 
 from ....error import LauncherError
 from ....log import get_logger
 from ....settings import *
 from ....status import STATUS_CANCELLED, STATUS_COMPLETED
+from ...config import CONFIG
 from ..launcher import WLMLauncher
-from ..step import AprunStep, LocalStep, MpirunStep, QsubBatchStep
+from ..step import (
+    AprunStep,
+    LocalStep,
+    MpiexecStep,
+    MpirunStep,
+    OrterunStep,
+    QsubBatchStep,
+)
 from ..stepInfo import PBSStepInfo
 from .pbsCommands import qdel, qstat
 from .pbsParser import parse_qstat_jobid, parse_step_id_from_qstat
 
 logger = get_logger(__name__)
 
 
@@ -52,16 +60,19 @@
 
     # init in WLMLauncher, launcher.py
 
     # RunSettings types supported by this launcher
     supported_rs = {
         AprunSettings: AprunStep,
         QsubBatchSettings: QsubBatchStep,
+        MpiexecSettings: MpiexecStep,
         MpirunSettings: MpirunStep,
+        OrterunSettings: OrterunStep,
         RunSettings: LocalStep,
+        PalsMpiexecSettings: MpiexecStep,
     }
 
     def run(self, step):
         """Run a job step through PBSPro
 
         :param step: a job step instance
         :type step: Step
@@ -117,22 +128,23 @@
         else:
             self.task_manager.remove_task(stepmap.task_id)
 
         _, step_info = self.get_step_update([step_name])[0]
         step_info.status = STATUS_CANCELLED  # set status to cancelled instead of failed
         return step_info
 
-    def _get_pbs_step_id(self, step, interval=2, trials=5):
+    def _get_pbs_step_id(self, step, interval=2):
         """Get the step_id of a step from qstat (rarely used)
 
         Parses qstat JSON output by looking for the step name
         TODO: change this to use ``qstat -a -u user``
         """
         time.sleep(interval)
         step_id = "unassigned"
+        trials = CONFIG.wlm_trials
         while trials > 0:
             output, _ = qstat(["-f", "-F", "json"])
             step_id = parse_step_id_from_qstat(output, step.name)
             if step_id:
                 break
             else:
                 time.sleep(interval)
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/pbs/pbsParser.py` & `smartsim-0.4.2/smartsim/_core/launcher/pbs/pbsParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/slurm/slurmCommands.py` & `smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmCommands.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/slurm/slurmLauncher.py` & `smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmLauncher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -27,16 +27,17 @@
 import time
 from shutil import which
 
 from ....error import LauncherError
 from ....log import get_logger
 from ....settings import *
 from ....status import STATUS_CANCELLED
+from ...config import CONFIG
 from ..launcher import WLMLauncher
-from ..step import LocalStep, MpirunStep, SbatchStep, SrunStep
+from ..step import LocalStep, MpiexecStep, MpirunStep, OrterunStep, SbatchStep, SrunStep
 from ..stepInfo import SlurmStepInfo
 from .slurmCommands import sacct, scancel, sstat
 from .slurmParser import parse_sacct, parse_sstat_nodes, parse_step_id_from_sacct
 
 logger = get_logger(__name__)
 
 
@@ -54,14 +55,16 @@
     # init in launcher.py (WLMLauncher)
 
     # RunSettings types supported by this launcher
     supported_rs = {
         SrunSettings: SrunStep,
         SbatchSettings: SbatchStep,
         MpirunSettings: MpirunStep,
+        MpiexecSettings: MpiexecStep,
+        OrterunSettings: OrterunStep,
         RunSettings: LocalStep,
     }
 
     def get_step_nodes(self, step_names):
         """Return the compute nodes of a specific job or allocation
 
         This function returns the compute nodes of a specific job or allocation
@@ -171,27 +174,28 @@
         else:
             self.task_manager.remove_task(stepmap.task_id)
 
         _, step_info = self.get_step_update([step_name])[0]
         step_info.status = STATUS_CANCELLED  # set status to cancelled instead of failed
         return step_info
 
-    def _get_slurm_step_id(self, step, interval=2, trials=5):
+    def _get_slurm_step_id(self, step, interval=2):
         """Get the step_id of a step from sacct
 
         Parses sacct output by looking for the step name
         e.g. the following
 
         SmartSim|119225|
         extern|119225.extern|
         m1-119225.0|119225.0|
         m2-119225.1|119225.1|
         """
         time.sleep(interval)
         step_id = "unassigned"
+        trials = CONFIG.wlm_trials
         while trials > 0:
             output, _ = sacct(["--noheader", "-p", "--format=jobname,jobid"])
             step_id = parse_step_id_from_sacct(output, step.name)
             if step_id:
                 break
             else:
                 time.sleep(interval)
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/slurm/slurmParser.py` & `smartsim-0.4.2/smartsim/_core/launcher/slurm/slurmParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/step/alpsStep.py` & `smartsim-0.4.2/smartsim/_core/launcher/step/alpsStep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/step/cobaltStep.py` & `smartsim-0.4.2/smartsim/_core/launcher/step/cobaltStep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/step/localStep.py` & `smartsim-0.4.2/smartsim/_core/launcher/step/localStep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/step/lsfStep.py` & `smartsim-0.4.2/smartsim/_core/launcher/step/lsfStep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/step/pbsStep.py` & `smartsim-0.4.2/smartsim/_core/launcher/step/pbsStep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/step/slurmStep.py` & `smartsim-0.4.2/smartsim/_core/launcher/step/slurmStep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -125,29 +125,30 @@
         :return: launch command
         :rtype: list[str]
         """
         srun = self.run_settings.run_command
         output, error = self.get_output_files()
 
         srun_cmd = [srun, "--output", output, "--error", error, "--job-name", self.name]
+        compound_env = set()
 
         if self.alloc:
             srun_cmd += ["--jobid", str(self.alloc)]
 
         if self.run_settings.env_vars:
             (
                 env_var_str,
                 comma_separated_env_vars,
             ) = self.run_settings.format_comma_sep_env_vars()
 
             if len(env_var_str) > 0:
-                srun_cmd += ["--export", env_var_str]
+                srun_cmd += ["--export", f"ALL,{env_var_str}"]
 
             if comma_separated_env_vars:
-                srun_cmd = ["env"] + comma_separated_env_vars + srun_cmd
+                compound_env = compound_env.union(comma_separated_env_vars)
 
         srun_cmd += self.run_settings.format_run_args()
 
         if self.run_settings.colocated_db_settings:
             # disable cpu binding as the entrypoint will set that
             # for the application and database process now
             srun_cmd.append("--cpu-bind=none")
@@ -156,15 +157,19 @@
             bash = shutil.which("bash")
             launch_script_path = self.get_colocated_launch_script()
             srun_cmd += [bash, launch_script_path]
 
         if self.run_settings.container:
             srun_cmd += self.run_settings.container._container_cmds(self.cwd)
 
+        if compound_env:
+            srun_cmd = ["env"] + list(compound_env) + srun_cmd
+
         srun_cmd += self._build_exe()
+
         return srun_cmd
 
     def _set_alloc(self):
         """Set the id of the allocation
 
         :raises AllocationError: allocation not listed or found
         """
@@ -195,19 +200,24 @@
             return exe + args
 
     def _make_mpmd(self):
         """Build Slurm multi-prog (MPMD) executable"""
         exe = self.run_settings.exe
         args = self.run_settings.exe_args
         cmd = exe + args
+
+        compound_env_vars = []
         for mpmd in self.run_settings.mpmd:
             cmd += [" : "]
             cmd += mpmd.format_run_args()
             cmd += ["--job-name", self.name]
-            (env_var_str, _) = mpmd.format_comma_sep_env_vars()
+
+            (env_var_str, csv_env_vars) = mpmd.format_comma_sep_env_vars()
             if len(env_var_str) > 0:
-                cmd += ["--export", env_var_str]
+                cmd += ["--export", f"ALL,{env_var_str}"]
+            if csv_env_vars:
+                compound_env_vars.extend(csv_env_vars)
             cmd += mpmd.exe
             cmd += mpmd.exe_args
 
         cmd = sh_split(" ".join(cmd))
         return cmd
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/step/step.py` & `smartsim-0.4.2/smartsim/_core/launcher/step/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/stepInfo.py` & `smartsim-0.4.2/smartsim/_core/launcher/stepInfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/stepMapping.py` & `smartsim-0.4.2/smartsim/_core/launcher/stepMapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/launcher/taskManager.py` & `smartsim-0.4.2/smartsim/_core/launcher/taskManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/utils/helpers.py` & `smartsim-0.4.2/smartsim/_core/utils/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/utils/network.py` & `smartsim-0.4.2/smartsim/_core/utils/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023 Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/_core/utils/redis.py` & `smartsim-0.4.2/smartsim/_core/utils/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/constants.py` & `smartsim-0.4.2/smartsim/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/database/orchestrator.py` & `smartsim-0.4.2/smartsim/database/orchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -41,15 +41,18 @@
 from ..error import SmartSimError, SSConfigError, SSUnsupportedError
 from ..log import get_logger
 from ..settings import (
     AprunSettings,
     BsubBatchSettings,
     CobaltBatchSettings,
     JsrunSettings,
+    MpiexecSettings,
     MpirunSettings,
+    OrterunSettings,
+    PalsMpiexecSettings,
     QsubBatchSettings,
     SbatchSettings,
     SrunSettings,
 )
 from ..settings.settings import create_batch_settings, create_run_settings
 from ..wlm import detect_launcher
 
@@ -97,17 +100,17 @@
         :type intra_op_threads: int, optional
         """
 
         if launcher == "auto":
             launcher = detect_launcher()
 
         by_launcher = {
-            "slurm": ["srun", "mpirun"],
-            "pbs": ["aprun", "mpirun"],
-            "cobalt": ["aprun", "mpirun"],
+            "slurm": ["srun", "mpirun", "mpiexec"],
+            "pbs": ["aprun", "mpirun", "mpiexec"],
+            "cobalt": ["aprun", "mpirun", "mpiexec"],
             "lsf": ["jsrun"],
             "local": [None],
         }
 
         def _detect_command(launcher):
             if launcher in by_launcher:
                 for cmd in by_launcher[launcher]:
@@ -715,24 +718,32 @@
                 f"{self._interface} is not a valid network interface on this node. \n"
                 "This could be because the head node doesn't have the same networks, if so, ignore this."
             )
             logger.warning(f"Found network interfaces are: {available}")
 
     def _fill_reserved(self):
         """Fill the reserved batch and run arguments dictionaries"""
-        self._reserved_run_args[MpirunSettings] = [
-            "np",
-            "N",
-            "c",
-            "output-filename",
-            "n",
-            "wdir",
-            "wd",
-            "host",
+
+        mpi_like_settings = [
+            MpirunSettings,
+            MpiexecSettings,
+            OrterunSettings,
+            PalsMpiexecSettings,
         ]
+        for settings in mpi_like_settings:
+            self._reserved_run_args[settings] = [
+                "np",
+                "N",
+                "c",
+                "output-filename",
+                "n",
+                "wdir",
+                "wd",
+                "host",
+            ]
         self._reserved_run_args[SrunSettings] = [
             "nodes",
             "N",
             "ntasks",
             "n",
             "ntasks-per-node",
             "output",
```

### Comparing `smartsim-0.4.1/smartsim/entity/dbnode.py` & `smartsim-0.4.2/smartsim/entity/dbnode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/entity/dbobject.py` & `smartsim-0.4.2/smartsim/entity/dbobject.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,57 @@
+# BSD 2-Clause License
+#
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+# 1. Redistributions of source code must retain the above copyright notice, this
+#    list of conditions and the following disclaimer.
+#
+# 2. Redistributions in binary form must reproduce the above copyright notice,
+#    this list of conditions and the following disclaimer in the documentation
+#    and/or other materials provided with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
 from pathlib import Path
 
 from .._core.utils.helpers import init_default
 
 __all__ = ["DBObject", "DBModel", "DBScript"]
 
 
 class DBObject:
     """Base class for ML objects residing on DB. Should not
     be instantiated.
     """
+
     def __init__(self, name, func, file_path, device, devices_per_node):
         self.name = name
         self.func = func
         if file_path:
             self.file = self._check_filepath(file_path)
         else:
             # Need to have this explicitly to check on it
             self.file = None
         self.device = self._check_device(device)
         self.devices_per_node = devices_per_node
 
-
     @property
     def is_file(self):
         if self.func:
             return False
         return True
 
     @staticmethod
```

### Comparing `smartsim-0.4.1/smartsim/entity/ensemble.py` & `smartsim-0.4.2/smartsim/entity/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/entity/entity.py` & `smartsim-0.4.2/smartsim/entity/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/entity/entityList.py` & `smartsim-0.4.2/smartsim/entity/entityList.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/entity/files.py` & `smartsim-0.4.2/smartsim/entity/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/entity/model.py` & `smartsim-0.4.2/smartsim/entity/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -21,23 +21,27 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
+import warnings
+
 from .._core.utils.helpers import cat_arg_and_value, init_default
 from ..error import EntityExistsError, SSUnsupportedError
 from .dbobject import DBModel, DBScript
 from .entity import SmartSimEntity
 from .files import EntityFiles
 
 
 class Model(SmartSimEntity):
-    def __init__(self, name, params, path, run_settings, params_as_args=None):
+    def __init__(
+        self, name, params, path, run_settings, params_as_args=None, batch_settings=None
+    ):
         """Initialize a ``Model``
 
         :param name: name of the model
         :type name: str
         :param params: model parameters for writing into configuration files or
                        to be passed as command line arguments to executable.
         :type params: dict
@@ -45,30 +49,32 @@
         :type path: str
         :param run_settings: launcher settings specified in the experiment
         :type run_settings: RunSettings
         :param params_as_args: list of parameters which have to be
                                interpreted as command line arguments to
                                be added to run_settings
         :type params_as_args: list[str]
+        :param batch_settings: Launcher settings for running the individual
+                               model as a batch job, defaults to None
+        :type batch_settings: BatchSettings | None
         """
         super().__init__(name, path, run_settings)
         self.params = params
         self.params_as_args = params_as_args
         self.incoming_entities = []
         self._key_prefixing_enabled = False
+        self.batch_settings = batch_settings
         self._db_models = []
         self._db_scripts = []
         self.files = None
 
     @property
     def colocated(self):
         """Return True if this Model will run with a colocated Orchestrator"""
-        if self.run_settings.colocated_db_settings:
-            return True
-        return False
+        return bool(self.run_settings.colocated_db_settings)
 
     def register_incoming_entity(self, incoming_entity):
         """Register future communication between entities.
 
         Registers the named data sources that this entity
         has access to by storing the key_prefix associated
         with that entity
@@ -124,29 +130,96 @@
         :type to_configure: list, optional
         """
         to_copy = init_default([], to_copy, (list, str))
         to_symlink = init_default([], to_symlink, (list, str))
         to_configure = init_default([], to_configure, (list, str))
         self.files = EntityFiles(to_configure, to_copy, to_symlink)
 
-    def colocate_db(
+    def colocate_db(self, *args, **kwargs):
+        """An alias for ``Model.colocate_db_tcp``"""
+        warnings.warn(
+            (
+                "`colocate_db` has been deprecated and will be removed in a \n"
+                "future release. Please use `colocate_db_tcp` or `colocate_db_uds`."
+            ),
+            category=DeprecationWarning,
+        )
+        self.colocate_db_tcp(*args, **kwargs)
+
+    def colocate_db_uds(
         self,
-        port=6379,
+        unix_socket="/tmp/redis.socket",
+        socket_permissions=755,
         db_cpus=1,
         limit_app_cpus=True,
+        debug=False,
+        **kwargs,
+    ):
+        """Colocate an Orchestrator instance with this Model over UDS.
+
+        This method will initialize settings which add an unsharded
+        database to this Model instance. Only this Model will be able to communicate
+        with this colocated database by using Unix Domain sockets.
+
+        Extra parameters for the db can be passed through kwargs. This includes
+        many performance, caching and inference settings.
+
+        .. highlight:: python
+        .. code-block:: python
+
+            example_kwargs = {
+                "maxclients": 100000,
+                "threads_per_queue": 1,
+                "inter_op_threads": 1,
+                "intra_op_threads": 1,
+                "server_threads": 2 # keydb only
+            }
+
+        Generally these don't need to be changed.
+
+        :param unix_socket: path to where the socket file will be created
+        :type unix_socket: str, optional
+        :param socket_permissions: permissions for the socketfile
+        :type socket_permissions: int, optional
+        :param db_cpus: number of cpus to use for orchestrator, defaults to 1
+        :type db_cpus: int, optional
+        :param limit_app_cpus: whether to limit the number of cpus used by the app, defaults to True
+        :type limit_app_cpus: bool, optional
+        :param debug: launch Model with extra debug information about the co-located db
+        :type debug: bool, optional
+        :param kwargs: additional keyword arguments to pass to the orchestrator database
+        :type kwargs: dict, optional
+        """
+
+        uds_options = {
+            "unix_socket": unix_socket,
+            "socket_permissions": socket_permissions,
+            "port": 0,  # This is hardcoded to 0 as recommended by redis for UDS
+        }
+        common_options = {
+            "cpus": db_cpus,
+            "limit_app_cpus": limit_app_cpus,
+            "debug": debug,
+        }
+        self._set_colocated_db_settings(uds_options, common_options, **kwargs)
+
+    def colocate_db_tcp(
+        self,
+        port=6379,
         ifname="lo",
+        db_cpus=1,
+        limit_app_cpus=True,
         debug=False,
         **kwargs,
     ):
-        """Colocate an Orchestrator instance with this Model at runtime.
+        """Colocate an Orchestrator instance with this Model over TCP/IP.
 
-        This method will initialize settings which add an unsharded (not connected)
+        This method will initialize settings which add an unsharded
         database to this Model instance. Only this Model will be able to communicate
-        with this colocated database by using the loopback TCP interface or Unix
-        Domain sockets (UDS coming soon).
+        with this colocated database by using the loopback TCP interface.
 
         Extra parameters for the db can be passed through kwargs. This includes
         many performance, caching and inference settings.
 
         .. highlight:: python
         .. code-block:: python
 
@@ -158,47 +231,58 @@
                 server_threads: 2 # keydb only
             }
 
         Generally these don't need to be changed.
 
         :param port: port to use for orchestrator database, defaults to 6379
         :type port: int, optional
+        :param ifname: interface to use for orchestrator, defaults to "lo"
+        :type ifname: str, optional
         :param db_cpus: number of cpus to use for orchestrator, defaults to 1
         :type db_cpus: int, optional
         :param limit_app_cpus: whether to limit the number of cpus used by the app, defaults to True
         :type limit_app_cpus: bool, optional
-        :param ifname: interface to use for orchestrator, defaults to "lo"
-        :type ifname: str, optional
         :param debug: launch Model with extra debug information about the co-located db
         :type debug: bool, optional
         :param kwargs: additional keyword arguments to pass to the orchestrator database
         :type kwargs: dict, optional
 
         """
+
+        tcp_options = {"port": port, "ifname": ifname}
+        common_options = {
+            "cpus": db_cpus,
+            "limit_app_cpus": limit_app_cpus,
+            "debug": debug,
+        }
+        self._set_colocated_db_settings(tcp_options, common_options, **kwargs)
+
+    def _set_colocated_db_settings(self, connection_options, common_options, **kwargs):
+        """
+        Ingest the connection-specific options (UDS/TCP) and set the final settings
+        for the co-located database
+        """
+
         if hasattr(self.run_settings, "mpmd") and len(self.run_settings.mpmd) > 0:
             raise SSUnsupportedError(
                 "Models co-located with databases cannot be run as a mpmd workload"
             )
 
         if hasattr(self.run_settings, "_prep_colocated_db"):
-            self.run_settings._prep_colocated_db(db_cpus)
+            self.run_settings._prep_colocated_db(common_options["cpus"])
 
         # TODO list which db settings can be extras
-        colo_db_config = {
-            "port": int(port),
-            "cpus": int(db_cpus),
-            "interface": ifname,
-            "limit_app_cpus": limit_app_cpus,
-            "debug": debug,
-            # redisai arguments for inference settings
-            "rai_args": {
-                "threads_per_queue": kwargs.get("threads_per_queue", None),
-                "inter_op_parallelism": kwargs.get("inter_op_parallelism", None),
-                "intra_op_parallelism": kwargs.get("intra_op_parallelism", None),
-            },
+        colo_db_config = {}
+        colo_db_config.update(connection_options)
+        colo_db_config.update(common_options)
+        # redisai arguments for inference settings
+        colo_db_config["rai_args"] = {
+            "threads_per_queue": kwargs.get("threads_per_queue", None),
+            "inter_op_parallelism": kwargs.get("inter_op_parallelism", None),
+            "intra_op_parallelism": kwargs.get("intra_op_parallelism", None),
         }
         colo_db_config["extra_db_args"] = dict(
             [
                 (k, str(v))
                 for k, v in kwargs.items()
                 if k not in colo_db_config["rai_args"]
             ]
```

### Comparing `smartsim-0.4.1/smartsim/entity/strategies.py` & `smartsim-0.4.2/smartsim/entity/strategies.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/error/errors.py` & `smartsim-0.4.2/smartsim/error/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/exp/ray/raycluster.py` & `smartsim-0.4.2/smartsim/settings/slurmSettings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -20,448 +20,449 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import datetime
 import os
-import re
-import sys
-import time as _time
-import uuid
-
-from ..._core.utils import init_default
-from ..._core.utils.helpers import expand_exe_path
-from ...entity import EntityList, SmartSimEntity
-from ...error import SmartSimError, SSUnsupportedError
-from ...log import get_logger
-from ...settings import settings
+from typing import List, Tuple
 
-logger = get_logger(__name__)
+from ..error import SSUnsupportedError
+from ..log import get_logger
+from .base import BatchSettings, RunSettings
 
+logger = get_logger(__name__)
 
-class RayCluster(EntityList):
-    """Entity used to run a Ray cluster on a given number of hosts. One Ray node is
-    launched on each host, and the first host is used to launch the head node.
-
-    :param name: The name of the entity.
-    :type name: str
-    :param path: Path to output, error, and configuration files
-    :type path: str
-    :param ray_port: Port at which the head node will be running.
-    :type ray_port: int
-    :param ray_args: Arguments to be passed to Ray executable.
-    :type ray_args: dict[str,str]
-    :param num_nodes: Number of hosts, includes 1 head node and all worker nodes.
-    :type num_nodes: int
-    :param run_args: Arguments to pass to launcher to specify details such as partition or time.
-    :type run_args: dict[str,str]
-    :param batch_args: Additional batch arguments passed to launcher when running batch jobs.
-    :type batch_args: dict[str,str]
-    :param launcher: Name of launcher to use for starting the cluster.
-    :type launcher: str
-    :param interface: Name of network interface the cluster nodes should bind to.
-    :type interface: str
-    :param alloc: ID of allocation to run on, if obtained with ``smartsim.slurm.get_allocation``
-    :type alloc: int
-    :param batch: Whether cluster should be launched as batch file, ignored when ``launcher`` is `local`
-    :type batch: bool
-    :param time: The walltime the cluster will be running for
-    :type time: str
-    :param run_command: Specify launch binary, defaults to automatic selection.
-    :type run_command: str
-    :param hosts: Specify hosts to launch on, defaults to None. Optional if not launching with OpenMPI.
-    :type hosts: str, list[str]
-    :param password: Password to use for Redis server, which is passed as `--redis_password` to `ray start`.
-                     Can be set to
-                     - `auto`: a strong password will be generated internally
-                     - a string: it will be used as password
-                     - `None`: the default Ray password will be used.
-                     Defaults to `auto`
-    :type password: str
-    """
 
+class SrunSettings(RunSettings):
     def __init__(
-        self,
-        name,
-        path=os.getcwd(),
-        ray_port=6789,
-        ray_args=None,
-        num_nodes=1,
-        run_args=None,
-        batch_args=None,
-        launcher="local",
-        batch=False,
-        time="01:00:00",
-        interface="ipogif0",
-        alloc=None,
-        run_command=None,
-        host_list=None,
-        password="auto",
-        **kwargs,
+        self, exe, exe_args=None, run_args=None, env_vars=None, alloc=None, **kwargs
     ):
-        launcher = launcher.lower()
-        supported_launchers = ["slurm", "pbs", "cobalt"]
-        if launcher not in supported_launchers:
-            raise SSUnsupportedError(
-                "The supported launchers for RayCluster are",
-                *[f"{launcher_name}," for launcher_name in supported_launchers],
-                f"but {launcher} was provided.",
-            )
-
-        if password:
-            if password == "auto":
-                self._ray_password = str(uuid.uuid4())
-            else:
-                self._ray_password = password
-        else:
-            self._ray_password = None
-
-        if num_nodes < 1:
-            raise ValueError("Number of nodes must be larger than 0.")
+        """Initialize run parameters for a slurm job with ``srun``
 
-        self.alloc = None
-        self.batch_settings = None
-        self._hosts = None
+        ``SrunSettings`` should only be used on Slurm based systems.
 
-        run_args = init_default({}, run_args, dict)
-        batch_args = init_default({}, batch_args, dict)
-        ray_args = init_default({}, ray_args, dict)
+        If an allocation is specified, the instance receiving these run
+        parameters will launch on that allocation.
 
-        self._ray_args = ray_args
+        :param exe: executable to run
+        :type exe: str
+        :param exe_args: executable arguments, defaults to None
+        :type exe_args: list[str] | str, optional
+        :param run_args: srun arguments without dashes, defaults to None
+        :type run_args: dict[str, str | None], optional
+        :param env_vars: environment variables for job, defaults to None
+        :type env_vars: dict[str, str], optional
+        :param alloc: allocation ID if running on existing alloc, defaults to None
+        :type alloc: str, optional
+        """
         super().__init__(
-            name=name,
-            path=path,
-            ray_args=ray_args,
+            exe,
+            exe_args,
+            run_command="srun",
             run_args=run_args,
-            ray_port=ray_port,
-            launcher=launcher,
-            interface=interface,
-            alloc=alloc,
-            num_nodes=num_nodes,
-            run_command=run_command if run_command else "auto",
-            host_list=host_list,
+            env_vars=env_vars,
             **kwargs,
         )
-        if batch:
-            self.batch_settings = settings.create_batch_settings(
-                launcher=launcher,
-                nodes=num_nodes,
-                time=time,
-                batch_args=batch_args,
-                **kwargs,
+        self.alloc = alloc
+        self.mpmd = []
+
+    reserved_run_args = {"chdir", "D"}
+
+    def set_nodes(self, nodes):
+        """Set the number of nodes
+
+        Effectively this is setting: ``srun --nodes <num_nodes>``
+
+        :param nodes: number of nodes to run with
+        :type nodes: int
+        """
+        self.run_args["nodes"] = int(nodes)
+
+    def make_mpmd(self, srun_settings):
+        """Make a mpmd workload by combining two ``srun`` commands
+
+        This connects the two settings to be executed with a single
+        Model instance
+
+        :param srun_settings: SrunSettings instance
+        :type srun_settings: SrunSettings
+        """
+        if self.colocated_db_settings:
+            raise SSUnsupportedError(
+                "Colocated models cannot be run as a mpmd workload"
             )
-        self.ray_head_address = None
+        if self.container:
+            raise SSUnsupportedError(
+                "Containerized MPMD workloads are not yet supported."
+            )
+        self.mpmd.append(srun_settings)
 
-        if host_list:
-            self.set_hosts(host_list=host_list, launcher=launcher)
+    def set_hostlist(self, host_list):
+        """Specify the hostlist for this job
 
-    @property
-    def batch(self):
-        try:
-            if self.batch_settings:
-                return True
-            return False
-        except AttributeError:
-            return False
-
-    def set_hosts(self, host_list, launcher):
-        """Specify the hosts for the ``RayCluster`` to launch on. This is
-        optional, unless ``run_command`` is `mpirun`.
+        This sets ``--nodelist``
 
-        :param host_list: list of hosts (compute node names)
+        :param host_list: hosts to launch on
         :type host_list: str | list[str]
-        :raises TypeError: if wrong type
+        :raises TypeError: if not str or list of str
         """
         if isinstance(host_list, str):
             host_list = [host_list.strip()]
         if not isinstance(host_list, list):
             raise TypeError("host_list argument must be a list of strings")
         if not all([isinstance(host, str) for host in host_list]):
             raise TypeError("host_list argument must be list of strings")
-        # TODO check length
-        if self.batch:
-            self.batch_settings.set_hostlist(host_list)
-        for host, node in zip(host_list, self.entities):
-            # Aprun doesn't like settings hosts in batch launch
-            if launcher == "pbs" or launcher == "cobalt":
-                if not self.batch:
-                    node.run_settings.set_hostlist([host])
-            else:
-                node.run_settings.set_hostlist([host])
+        self.run_args["nodelist"] = ",".join(host_list)
+
+    def set_hostlist_from_file(self, file_path):
+        """Use the contents of a file to set the node list
+
+        This sets ``--nodefile``
+
+        :param file_path: Path to the hostlist file
+        :type file_path: str
+        """
+        self.run_args["nodefile"] = str(file_path)
+
+    def set_excluded_hosts(self, host_list):
+        """Specify a list of hosts to exclude for launching this job
+
+        :param host_list: hosts to exclude
+        :type host_list: list[str]
+        :raises TypeError:
+        """
+        if isinstance(host_list, str):
+            host_list = [host_list.strip()]
+        if not isinstance(host_list, list):
+            raise TypeError("host_list argument must be a list of strings")
+        if not all([isinstance(host, str) for host in host_list]):
+            raise TypeError("host_list argument must be list of strings")
+        self.run_args["exclude"] = ",".join(host_list)
+
+    def set_cpus_per_task(self, cpus_per_task):
+        """Set the number of cpus to use per task
+
+        This sets ``--cpus-per-task``
+
+        :param num_cpus: number of cpus to use per task
+        :type num_cpus: int
+        """
+        self.run_args["cpus-per-task"] = int(cpus_per_task)
+
+    def set_tasks(self, tasks):
+        """Set the number of tasks for this job
+
+        This sets ``--ntasks``
+
+        :param tasks: number of tasks
+        :type tasks: int
+        """
+        self.run_args["ntasks"] = int(tasks)
+
+    def set_tasks_per_node(self, tasks_per_node):
+        """Set the number of tasks for this job
 
-    def _initialize_entities(self, **kwargs):
+        This sets ``--ntasks-per-node``
 
-        ray_port = kwargs.get("ray_port", 6789)
-        launcher = kwargs.get("launcher", "slurm")
-        ray_args = kwargs.get("ray_args", None)
-        run_args = kwargs.get("run_args", None)
-        interface = kwargs.get("interface", "ipogif0")
-        num_nodes = kwargs.get("num_nodes", 0)
-        alloc = kwargs.get("alloc", None)
-        run_command = kwargs.get("run_command", None)
-
-        ray_head = RayHead(
-            name="ray_head",
-            path=self.path,
-            ray_password=self._ray_password,
-            ray_port=ray_port,
-            launcher=launcher,
-            run_args=run_args.copy(),
-            ray_args=ray_args.copy(),
-            interface=interface,
-            run_command=run_command,
-            alloc=alloc,
+        :param tasks_per_node: number of tasks per node
+        :type tasks_per_node: int
+        """
+        self.run_args["ntasks-per-node"] = int(tasks_per_node)
+
+    def set_cpu_bindings(self, bindings):
+        """Bind by setting CPU masks on tasks
+
+        This sets ``--cpu-bind`` using the ``map_cpu:<list>`` option
+
+        :param bindings: List specifing the cores to which MPI processes are bound
+        :type bindings: list[int] | int
+        """
+        if isinstance(bindings, int):
+            bindings = [bindings]
+        self.run_args["cpu_bind"] = "map_cpu:" + ",".join(
+            str(int(num)) for num in bindings
         )
 
-        self.entities.append(ray_head)
+    def set_memory_per_node(self, memory_per_node):
+        """Specify the real memory required per node
 
-        for worker_id in range(num_nodes - 1):
-            worker_model = RayWorker(
-                name=f"ray_worker_{worker_id}",
-                path=self.path,
-                run_args=run_args.copy(),
-                ray_port=ray_port,
-                ray_password=self._ray_password,
-                ray_args=ray_args.copy(),
-                interface=interface,
-                run_command=run_command,
-                launcher=launcher,
-                alloc=alloc,
-            )
-            self.entities.append(worker_model)
+        This sets ``--mem`` in megabytes
+
+        :param memory_per_node: Amount of memory per node in megabytes
+        :type memory_per_node: int
+        """
+        self.run_args["mem"] = f"{int(memory_per_node)}M"
 
-    def get_head_address(self):
-        """Return address of head node
+    def set_verbose_launch(self, verbose):
+        """Set the job to run in verbose mode
 
-        If address has not been initialized, returns None
+        This sets ``--verbose``
 
-        :returns: Address of head node
-        :rtype: str
+        :param verbose: Whether the job should be run verbosely
+        :type verbose: bool
         """
-        if not self.ray_head_address:
-            self.ray_head_address = parse_ray_head_node_address(
-                os.path.join(self.entities[0].path, self.entities[0].name + ".out")
-            )
-        return self.ray_head_address
+        if verbose:
+            self.run_args["verbose"] = None
+        else:
+            self.run_args.pop("verbose", None)
 
-    def get_dashboard_address(self):
-        """Returns dashboard address
+    def set_quiet_launch(self, quiet):
+        """Set the job to run in quiet mode
 
-        The format is <head_ip>:<dashboard_port>
+        This sets ``--quiet``
 
-        :returns: Dashboard address
-        :rtype: str
+        :param quiet: Whether the job should be run quietly
+        :type quiet: bool
         """
-        return self.get_head_address() + ":" + str(self.entities[0].dashboard_port)
+        if quiet:
+            self.run_args["quiet"] = None
+        else:
+            self.run_args.pop("quiet", None)
 
-    def _update_workers(self):
-        """Update worker args before launching them."""
-        for worker in range(1, len(self.entities)):
-            self.entities[worker].set_head_log(
-                f"{os.path.join(self.entities[0].path, self.entities[0].name)}.out"
-            )
+    def set_broadcast(self, dest_path=None):
+        """Copy executable file to allocated compute nodes
 
+        This sets ``--bcast``
 
-def find_ray_exe():
-    """Find ray executable in current path."""
-    # TODO add this to CONFIG?
-    try:
-        return expand_exe_path("ray")
-    except (TypeError, FileNotFoundError):
-        raise SmartSimError("Could not find ray executable")
-
-
-def parse_ray_head_node_address(head_log):
-    """Get the ray head node host address from the log file produced
-    by the head process.
-
-    :param head_log: full path to log file of head node
-    :return: address of the head host
-    :rtype: str
-    """
-
-    max_attempts = 24
-    attempts = 0
-    while not os.path.isfile(head_log):
-        _time.sleep(5)
-        attempts += 1
-        if attempts == max_attempts:
-            raise RuntimeError(f"Could not find Ray cluster head log file {head_log}")
-
-    attempts = 0
-    head_ip = None
-    while head_ip is None:
-        _time.sleep(5)
-        with open(head_log) as fp:
-            line = fp.readline()
-            while line:
-                plain_line = re.sub("\033\\[([0-9]+)(;[0-9]+)*m", "", line)
-                if "Local node IP:" in plain_line:
-                    matches = re.search(r"(?<=Local node IP: ).*", plain_line)
-                    head_ip = matches.group()
-                    break
-                line = fp.readline()
-        attempts += 1
-        if attempts == max_attempts:
-            raise RuntimeError(
-                f"Could not find Ray cluster head address in log file {head_log}."
-            )
+        :param dest_path: Path to copy an executable file
+        :type dest_path: str | None
+        """
+        self.run_args["bcast"] = dest_path
 
-    return head_ip
+    def _fmt_walltime(self, hours, minutes, seconds):
+        """Convert hours, minutes, and seconds into valid walltime format
 
+        Converts time to format HH:MM:SS
 
-class RayHead(SmartSimEntity):
-    def __init__(
-        self,
-        name,
-        path,
-        ray_password,
-        ray_port=6789,
-        run_args=None,
-        ray_args=None,
-        launcher="slurm",
-        interface="ipogif0",
-        run_command=None,
-        alloc=None,
-        dash_port=8265,
-        **kwargs,
-    ):
-        self.dashboard_port = dash_port
-        self.batch_settings = None
-        self.files = None
+        :param hours: number of hours to run job
+        :type hours: int
+        :param minutes: number of minutes to run job
+        :type minutes: int
+        :param seconds: number of seconds to run job
+        :type seconds: int
+        :returns: Formatted walltime
+        :rtype
+        """
+        delta = datetime.timedelta(hours=hours, minutes=minutes, seconds=seconds)
+        fmt_str = str(delta)
+        if delta.seconds // 3600 < 10:
+            fmt_str = "0" + fmt_str
+        return fmt_str
 
-        run_args = init_default({}, run_args, dict)
-        ray_args = init_default({}, ray_args, dict)
+    def set_walltime(self, walltime):
+        """Set the walltime of the job
 
-        ray_exe_args = self._build_ray_exe_args(
-            ray_port, ray_password, interface, ray_args
-        )
+        format = "HH:MM:SS"
 
-        run_settings = settings.create_run_settings(
-            launcher=launcher,
-            exe="python",
-            exe_args=ray_exe_args,
-            run_args=run_args,
-            run_command=run_command if run_command else "auto",
-            alloc=alloc,
-            **kwargs,
-        )
+        :param walltime: wall time
+        :type walltime: str
+        """
+        self.run_args["time"] = str(walltime)
 
-        run_settings.set_tasks_per_node(1)
-        run_settings.set_tasks(1)
+    def format_run_args(self):
+        """Return a list of slurm formatted run arguments
 
-        super().__init__(name, path, run_settings)
+        :return: list of slurm arguments for these settings
+        :rtype: list[str]
+        """
+        # add additional slurm arguments based on key length
+        opts = []
+        for opt, value in self.run_args.items():
+            short_arg = bool(len(str(opt)) == 1)
+            prefix = "-" if short_arg else "--"
+            if not value:
+                opts += [prefix + opt]
+            else:
+                if short_arg:
+                    opts += [prefix + opt, str(value)]
+                else:
+                    opts += ["=".join((prefix + opt, str(value)))]
+        return opts
 
-    def _build_ray_exe_args(self, ray_port, ray_password, interface, ray_args):
+    def check_env_vars(self):
+        """Warn a user trying to set a variable which is set in the environment
 
-        # python script that launches ray head node
-        ray_starter_args = [
-            "-m",
-            "smartsim._core.entrypoints.ray",
-            f"+port={ray_port}",
-            f"+ifname={interface}",
-            f"+ray-exe={find_ray_exe()}",
-            f"+head",
-        ]
+        Given Slurm's env var precedence, trying to export a variable which is already
+        present in the environment will not work.
+        """
+        for k, v in self.env_vars.items():
+            if "," not in str(v):
+                # If a variable is defined, it will take precedence over --export
+                # we warn the user
+                preexisting_var = os.environ.get(k, None)
+                if preexisting_var is not None:
+                    msg = f"Variable {k} is set to {preexisting_var} in current environment. "
+                    msg += f"If the job is running in an interactive allocation, the value {v} will not be set. "
+                    msg += "Please consider removing the variable from the environment and re-run the experiment."
+                    logger.warning(msg)
 
-        if ray_password:
-            ray_starter_args += [f"+redis-password={ray_password}"]
+    def format_env_vars(self):
+        """Build bash compatible environment variable string for Slurm
 
-        if "dashboard-port" in ray_args:
-            self.dashboard_port = int(ray_args["dashboard-port"])
-        ray_starter_args += [f"+dashboard-port={self.dashboard_port}"]
+        :returns: the formatted string of environment variables
+        :rtype: list[str]
+        """
+        self.check_env_vars()
+        return [f"{k}={v}" for k, v in self.env_vars.items() if "," not in str(v)]
 
-        used = ["block", "redis-password", "start", "head", "port", "dashboard-port"]
-        extra_ray_args = []
-        for key, value in ray_args.items():
-            if key not in used:
-                extra_ray_args += [f"+ray-args=--{key}={value}"]
-        ray_starter_args += extra_ray_args
+    def format_comma_sep_env_vars(self) -> Tuple[str, List[str]]:
+        """Build environment variable string for Slurm
 
-        return " ".join(ray_starter_args)
+        Slurm takes exports in comma separated lists
+        the list starts with all as to not disturb the rest of the environment
+        for more information on this, see the slurm documentation for srun
 
+        :returns: the formatted string of environment variables
+        :rtype: tuple[str, list[str]]
+        """
+        self.check_env_vars()
+        exportable_env, compound_env, key_only = [], [], []
 
-class RayWorker(SmartSimEntity):
-    def __init__(
-        self,
-        name,
-        path,
-        ray_password,
-        ray_port,
-        run_args=None,
-        ray_args=None,
-        interface="ipogif0",
-        launcher="slurm",
-        run_command=None,
-        alloc=None,
-        **kwargs,
-    ):
+        for k, v in self.env_vars.items():
+            kvp = f"{k}={v}"
 
-        self.batch_settings = None
-        self.files = None
+            if "," in str(v):
+                key_only.append(k)
+                compound_env.append(kvp)
+            else:
+                exportable_env.append(kvp)
 
-        run_args = init_default({}, run_args, dict)
-        ray_args = init_default({}, ray_args, dict)
+        # Append keys to exportable KVPs, e.g. `--export x1=v1,KO1,KO2`
+        fmt_exported_env = ",".join(v for v in exportable_env + key_only)
 
-        ray_exe_args = self._build_ray_exe_args(
-            ray_password, ray_args, ray_port, interface
-        )
+        for mpmd in self.mpmd:
+            compound_mpmd_env = {k: v for k, v in mpmd.env_vars.items() if "," in v}
+            compound_mpmd_fmt = {f"{k}={v}" for k, v in compound_mpmd_env.items()}
+            compound_env.extend(compound_mpmd_fmt)
 
-        run_settings = settings.create_run_settings(
-            launcher=launcher,
-            exe=sys.executable,
-            exe_args=ray_exe_args,
-            run_args=run_args,
-            run_command=run_command,
-            alloc=alloc,
+        return fmt_exported_env, compound_env
+
+
+class SbatchSettings(BatchSettings):
+    def __init__(self, nodes=None, time="", account=None, batch_args=None, **kwargs):
+        """Specify run parameters for a Slurm batch job
+
+        Slurm `sbatch` arguments can be written into ``batch_args``
+        as a dictionary. e.g. {'ntasks': 1}
+
+        If the argument doesn't have a parameter, put `None`
+        as the value. e.g. {'exclusive': None}
+
+        Initialization values provided (nodes, time, account)
+        will overwrite the same arguments in ``batch_args`` if present
+
+        :param nodes: number of nodes, defaults to None
+        :type nodes: int, optional
+        :param time: walltime for job, e.g. "10:00:00" for 10 hours
+        :type time: str, optional
+        :param account: account for job, defaults to None
+        :type account: str, optional
+        :param batch_args: extra batch arguments, defaults to None
+        :type batch_args: dict[str, str], optional
+        """
+        super().__init__(
+            "sbatch",
+            batch_args=batch_args,
+            nodes=nodes,
+            account=account,
+            time=time,
             **kwargs,
         )
 
-        run_settings.set_tasks_per_node(1)
-        run_settings.set_tasks(1)
+    def set_walltime(self, walltime):
+        """Set the walltime of the job
+
+        format = "HH:MM:SS"
+
+        :param walltime: wall time
+        :type walltime: str
+        """
+        # TODO check for formatting here
+        if walltime:
+            self.batch_args["time"] = walltime
+
+    def set_nodes(self, num_nodes):
+        """Set the number of nodes for this batch job
+
+        :param num_nodes: number of nodes
+        :type num_nodes: int
+        """
+        if num_nodes:
+            self.batch_args["nodes"] = int(num_nodes)
+
+    def set_account(self, account):
+        """Set the account for this batch job
 
-        super().__init__(name, path, run_settings)
+        :param account: account id
+        :type account: str
+        """
+        if account:
+            self.batch_args["account"] = account
+
+    def set_partition(self, partition):
+        """Set the partition for the batch job
+
+        :param partition: partition name
+        :type partition: str
+        """
+        self.batch_args["partition"] = str(partition)
 
-    @property
-    def batch(self):
-        return False
-
-    def set_head_log(self, head_log):
-        """Set head log file (with full path)
-
-        The head log file is used by the worker to discover
-        the head IP address. This function is called by
-        RayCluster before the cluster is launched.
-        """
-        self.run_settings.add_exe_args([f"+head-log={head_log}"])
-
-    def _build_ray_exe_args(self, ray_password, ray_args, ray_port, interface):
-
-        # python script that launches ray  node
-        ray_starter_args = [
-            "-m",
-            "smartsim._core.entrypoints.ray",
-            f"+ray-exe={find_ray_exe()}",
-            f"+port={ray_port}",
-            f"+ifname={interface}",
-        ]
-        if ray_password:
-            ray_starter_args += [f"+redis-password={ray_password}"]
-
-        used = [
-            "block",
-            "redis-password",
-            "start",
-            "head",
-            "port",
-            "dashboard-port",
-            "dashboard-host",
-        ]
-        extra_ray_args = []
-        for key, value in ray_args.items():
-            if key not in used:
-                extra_ray_args += [f"+ray-args=--{key}={value}"]
-        ray_starter_args += extra_ray_args
+    def set_queue(self, queue):
+        """alias for set_partition
+
+        Sets the partition for the slurm batch job
+
+        :param queue: the partition to run the batch job on
+        :type queue: str
+        """
+        if queue:
+            self.set_partition(queue)
+
+    def set_cpus_per_task(self, cpus_per_task):
+        """Set the number of cpus to use per task
+
+        This sets ``--cpus-per-task``
+
+        :param num_cpus: number of cpus to use per task
+        :type num_cpus: int
+        """
+        self.batch_args["cpus-per-task"] = int(cpus_per_task)
 
-        return " ".join(ray_starter_args)
+    def set_hostlist(self, host_list):
+        """Specify the hostlist for this job
+
+        :param host_list: hosts to launch on
+        :type host_list: str | list[str]
+        :raises TypeError: if not str or list of str
+        """
+        if isinstance(host_list, str):
+            host_list = [host_list.strip()]
+        if not isinstance(host_list, list):
+            raise TypeError("host_list argument must be a list of strings")
+        if not all([isinstance(host, str) for host in host_list]):
+            raise TypeError("host_list argument must be list of strings")
+        self.batch_args["nodelist"] = ",".join(host_list)
+
+    def format_batch_args(self):
+        """Get the formatted batch arguments for a preview
+
+        :return: batch arguments for Sbatch
+        :rtype: list[str]
+        """
+        opts = []
+        # TODO add restricted here
+        for opt, value in self.batch_args.items():
+            # attach "-" prefix if argument is 1 character otherwise "--"
+            short_arg = bool(len(str(opt)) == 1)
+            prefix = "-" if short_arg else "--"
+
+            if not value:
+                opts += [prefix + opt]
+            else:
+                if short_arg:
+                    opts += [prefix + opt, str(value)]
+                else:
+                    opts += ["=".join((prefix + opt, str(value)))]
+        return opts
```

### Comparing `smartsim-0.4.1/smartsim/experiment.py` & `smartsim-0.4.2/smartsim/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -423,25 +423,42 @@
             )
             return new_ensemble
         except SmartSimError as e:
             logger.error(e)
             raise
 
     def create_model(
-        self, name, run_settings, params=None, path=None, enable_key_prefixing=False
+        self,
+        name,
+        run_settings,
+        params=None,
+        path=None,
+        enable_key_prefixing=False,
+        batch_settings=None,
     ):
         """Create a general purpose ``Model``
 
         The ``Model`` class is the most general encapsulation of
         executable code in SmartSim. ``Model`` instances are named
         references to pieces of a workflow that can be parameterized,
         and executed.
 
-        ``Model`` instances can be launched sequentially or as a batch
-        by adding them into an ``Ensemble``.
+        ``Model`` instances can be launched sequentially, as a batch job,
+        or as a group by adding them into an ``Ensemble``.
+
+        All models require a reference to run settings to specify which
+        executable to launch as well provide options for how to launch
+        the executable with the underlying WLM. Furthermore, batch a
+        reference to a batch settings can be added to launch the model
+        as a batch job through ``Experiment.start``. If a model with
+        a reference to a set of batch settings is added to a larger
+        entity with its own set of batch settings (for e.g. an
+        ``Ensemble``) the batch settings of the larger entity will take
+        precedence and the batch setting of the model will be
+        strategically ignored.
 
         Parameters supplied in the `params` argument can be written into
         configuration files supplied at runtime to the model through
         ``Model.attach_generator_files``. `params` can also be turned
         into executable arguments by calling ``Model.params_to_args``
 
         By default, ``Model`` instances will be executed in the
@@ -473,35 +490,47 @@
         New in 0.4.0, ``Model`` instances can be co-located with an
         Orchestrator database shard through ``Model.colocate_db``. This
         will launch a single ``Orchestrator`` instance on each compute
         host used by the (possibly distributed) application. This is
         useful for performant online inference or processing
         at runtime.
 
+        New in 0.4.2, ``Model`` instances can now be co-located with
+        an Orchestrator database over either TCP or UDS using the
+        ``Model.colocate_db_tcp`` or ``Model.colocate_db_uds`` method
+        respectively. The original ``Model.colocate_db`` method is now
+        deprecated, but remains as an alias for ``Model.colocate_db_tcp``
+        for backward compatibility.
+
         :param name: name of the model
         :type name: str
         :param run_settings: defines how ``Model`` should be run
         :type run_settings: RunSettings
         :param params: model parameters for writing into configuration files
         :type params: dict, optional
         :param path: path to where the model should be executed at runtime
         :type path: str, optional
         :param enable_key_prefixing: If True, data sent to the Orchestrator
                                      using SmartRedis from this ``Model`` will
                                      be prefixed with the ``Model`` name.
                                      Default is True.
         :type enable_key_prefixing: bool, optional
+        :param batch_settings: Settings to run model individually as a batch job,
+                               defaults to None
+        :type batch_settings: BatchSettings | None
         :raises SmartSimError: if initialization fails
         :return: the created ``Model``
         :rtype: Model
         """
         path = init_default(getcwd(), path, str)
         params = init_default({}, params, dict)
         try:
-            new_model = Model(name, params, path, run_settings)
+            new_model = Model(
+                name, params, path, run_settings, batch_settings=batch_settings
+            )
             if enable_key_prefixing:
                 new_model.enable_key_prefixing()
             return new_model
         except SmartSimError as e:
             logger.error(e)
             raise
 
@@ -541,15 +570,15 @@
         :param run_command: command to run the executable
         :type run_command: str
         :param exe: executable to run
         :type exe: str
         :param exe_args: arguments to pass to the executable
         :type exe_args: list[str], optional
         :param run_args: arguments to pass to the ``run_command``
-        :type run_args: list[str], optional
+        :type run_args: dict[str, str], optional
         :param env_vars: environment variables to pass to the executable
         :type env_vars: dict[str, str], optional
         :return: the created ``RunSettings``
         :rtype: RunSettings
         """
         try:
             return settings.create_run_settings(
@@ -741,39 +770,40 @@
             for run in range(job.history.runs + 1):
                 values.append(
                     [
                         job.entity.name,
                         job.entity.type,
                         job.history.jids[run],
                         run,
-                        job.history.job_times[run],
+                        f"{job.history.job_times[run]:.4f}",
                         job.history.statuses[run],
                         job.history.returns[run],
                     ]
                 )
         else:
             return tabulate(
-                values, headers, showindex=True, tablefmt=format, missingval="None"
+                values,
+                headers,
+                showindex=True,
+                tablefmt=format,
+                missingval="None",
+                disable_numparse=True,
             )
 
     def _launch_summary(self, manifest):
         """Experiment pre-launch summary of entities that will be launched
 
         :param manifest: Manifest of deployables.
         :type manifest: Manifest
         """
 
         summary = "\n\n=== Launch Summary ===\n"
         summary += f"Experiment: {self.name}\n"
         summary += f"Experiment Path: {self.exp_path}\n"
         summary += f"Launcher: {self._launcher}\n"
-        if manifest.ensembles or manifest.ray_clusters:
-            summary += (
-                f"Ensembles: {len(manifest.ensembles) + len(manifest.ray_clusters)}\n"
-            )
         if manifest.models:
             summary += f"Models: {len(manifest.models)}\n"
 
         if self._control.orchestrator_active:
             summary += f"Database Status: active\n"
         elif manifest.db:
             summary += f"Database Status: launching\n"
```

### Comparing `smartsim-0.4.1/smartsim/log.py` & `smartsim-0.4.2/smartsim/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/ml/data.py` & `smartsim-0.4.2/smartsim/ml/data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,707 +1,493 @@
+# BSD 2-Clause License
+#
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without
+# modification, are permitted provided that the following conditions are met:
+#
+# 1. Redistributions of source code must retain the above copyright notice, this
+#    list of conditions and the following disclaimer.
+#
+# 2. Redistributions in binary form must reproduce the above copyright notice,
+#    this list of conditions and the following disclaimer in the documentation
+#    and/or other materials provided with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+# FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+# OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+# OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
 import time
 from os import environ
 
 import numpy as np
 from smartredis import Client, Dataset
+from smartredis.error import RedisReplyError
 
-from ..error import SmartSimError
+from ..error import SSInternalError
 from ..log import get_logger
 
 logger = get_logger(__name__)
 
 
 def form_name(*args):
     return "_".join(str(arg) for arg in args if arg is not None)
 
 
+class DataInfo:
+    """A class holding all relevant information to download datasets from aggregation lists
+
+    This class can be passed as argument to SmartSim's ML data loaders, as it wraps the
+    information about the aggregation list holding the training datasets.
+
+    Each training dataset will store batches of samples and (optionally) labels or targets in the
+    form of tensors. The tensors must always have the same names, which can be accessed
+    in ``DataInfo.sample_name`` and ``DataInfo.target_name``.
+
+    :param list_name: Name of the aggregation list used for sample datasets
+    :type list_name: str
+    :param sample_name: Name of tensor holding training samples in stored datasets.
+    :type sample_name: str
+    :param target_name: Name of tensor holding targets or labels in stored datasets.
+    :type target_name: str
+    :num_classes: Number of classes (for categorical data).
+    :type num_classes: int | None
+    """
+
+    def __init__(
+        self, list_name, sample_name="samples", target_name="targets", num_classes=None
+    ):
+        self.list_name = list_name
+        self.sample_name = sample_name
+        self.target_name = target_name
+        self.num_classes = num_classes
+        self._ds_name = form_name(self.list_name, "info")
+
+    def publish(self, client: Client):
+        """Upload DataInfo information to Orchestrator
+
+        The information is put on the DB as a DataSet, with strings
+        stored as metastrings and integers stored as metascalars.
+
+        :param client: Client to connect to Database
+        :type client: SmartRedis.Client
+        """
+        info_ds = Dataset(self._ds_name)
+        info_ds.add_meta_string("sample_name", self.sample_name)
+        if self.target_name:
+            info_ds.add_meta_string("target_name", self.target_name)
+        if self.num_classes:
+            info_ds.add_meta_scalar("num_classes", self.num_classes)
+        client.put_dataset(info_ds)
+
+    def download(self, client: Client):
+        """Download DataInfo information from Orchestrator
+
+        The information retrieved from the DB is used to populate
+        this object's members. If the information is not available
+        on the DB, the object members are not modified.
+
+        :param client: Client to connect to Database
+        :type client: SmartRedis.Client
+        """
+        try:
+            info_ds = client.get_dataset(self._ds_name)
+        except RedisReplyError:
+            # If the info was not published, proceed with default parameters
+            logger.warning(
+                f"Could not retrieve data for DataInfo object, the following values will be kept."
+            )
+            logger.warning(str(self))
+            return
+        self.sample_name = info_ds.get_meta_strings("sample_name")[0]
+        field_names = info_ds.get_metadata_field_names()
+        if "target_name" in field_names:
+            self.target_name = info_ds.get_meta_strings("target_name")[0]
+        if "num_classes" in field_names:
+            self.num_classes = info_ds.get_meta_scalars("num_classes")[0]
+
+    def __repr__(self):
+        strings = ["DataInfo object"]
+        strings += [f"Aggregation list name: {self.list_name}"]
+        strings += [f"Sample tensor name: {self.sample_name}"]
+        if self.target_name:
+            strings += [f"Target tensor name: {self.target_name}"]
+        if self.num_classes:
+            strings += [f"Number of classes: {self.num_classes}"]
+        return "\n".join(strings)
+
+
 class TrainingDataUploader:
     """A class to simplify uploading batches of samples to train a model.
 
     This class can be used to upload samples following a simple convention
     for naming. Once created, the function `publish_info` can be used
     to put all details about the data set on the Orchestrator. A training
     process can thus access them and get all relevant information to download
     the batches which are uploaded.
 
     Each time a new batch is available, it is sufficient to call `put_batch`,
     and the data will be stored following the naming convention specified
     by the attributes of this class.
 
-    :param name: Name of the dataset as stored on the Orchestrator
-    :type name: str
-    :param sample_prefix: Prefix of samples batches
-    :type sample_prefix: str
-    :param target_prefix: Prefix of target batches (if needed)
-    :type target_prefix: str
+    :param list_name: Name of the dataset as stored on the Orchestrator
+    :type list_name: str
+    :param sample_name: Name of samples tensor in uploaded Datasets
+    :type sample_name: str
+    :param target_name: Name of targets tensor (if needed) in uploaded Datasets
+    :type target_name: str
     :param num_classes: Number of classes of targets, if categorical
     :type num_classes: int
-    :param producer_prefixes: Prefixes of processes which will be producing batches.
-                              This can be useful in case the consumer processes also
-                              have other incoming entities.
-    :type producer_prefixes: str or list[str]
     :param cluster: Whether the SmartSim Orchestrator is being run as a cluster
     :type cluster: bool
     :param address: Address of Redis DB as <ip_address>:<port>
     :type address: str
-    :param num_ranks: Number of processes (e.g. MPI ranks) of application using
-                      DataUploader.
-    :type num_ranks: int
     :param rank: Rank of DataUploader in multi-process application (e.g. MPI rank).
     :type rank: int
     :param verbose: If output should be logged to screen.
     :type verbose: bool
 
     """
 
     def __init__(
         self,
-        name="training_data",
-        sample_prefix="samples",
-        target_prefix="targets",
+        list_name="training_data",
+        sample_name="samples",
+        target_name="targets",
         num_classes=None,
-        producer_prefixes=None,
         cluster=True,
         address=None,
-        num_ranks=None,
         rank=None,
         verbose=False,
     ):
-        if not name:
+        if not list_name:
             raise ValueError("Name can not be empty")
-        if not sample_prefix:
-            raise ValueError("Sample prefix can not be empty")
-
-        self.name = name
-        self.sample_prefix = sample_prefix
-        self.target_prefix = target_prefix
-        if isinstance(producer_prefixes, str):
-            producer_prefixes = [producer_prefixes]
-        self.producer_prefixes = producer_prefixes
-        self.num_classes = num_classes
-        if num_ranks is None:
-            self.num_ranks = None
-        else:
-            self.num_ranks = int(num_ranks)
-        self.rank = rank
+        if not sample_name:
+            raise ValueError("Sample name can not be empty")
 
         self.client = Client(address=address, cluster=cluster)
-        self.batch_idx = 0
         self.verbose = verbose
+        self.batch_idx = 0
+        self.rank = rank
+        self._info = DataInfo(list_name, sample_name, target_name, num_classes)
+
+    @property
+    def list_name(self):
+        return self._info.list_name
+
+    @property
+    def sample_name(self):
+        return self._info.sample_name
+
+    @property
+    def target_name(self):
+        return self._info.target_name
+
+    @property
+    def num_classes(self):
+        return self._info.num_classes
 
     def publish_info(self):
-        info_ds = Dataset(form_name(self.name, "info"))
-        info_ds.add_meta_string("sample_prefix", self.sample_prefix)
-        if self.target_prefix:
-            info_ds.add_meta_string("target_prefix", self.target_prefix)
-        if self.producer_prefixes:
-            for producer_prefix in self.producer_prefixes:
-                info_ds.add_meta_string("producer_prefixes", producer_prefix)
-        if self.num_classes:
-            info_ds.add_meta_scalar("num_classes", self.num_classes)
-        if self.num_ranks:
-            info_ds.add_meta_scalar("num_ranks", self.num_ranks)
-        self.client.put_dataset(info_ds)
+        self._info.publish(self.client)
 
     def put_batch(self, samples, targets=None):
-        batch_key = form_name(self.sample_prefix, self.batch_idx, self.rank)
-        self.client.put_tensor(batch_key, samples)
-        if self.verbose:
-            logger.info(f"Put batch {batch_key}")
-
+        batch_ds_name = form_name("training_samples", self.rank, self.batch_idx)
+        batch_ds = Dataset(batch_ds_name)
+        batch_ds.add_tensor(self.sample_name, samples)
         if (
             targets is not None
-            and self.target_prefix
-            and (self.target_prefix != self.sample_prefix)
+            and self.target_name
+            and (self.target_name != self.sample_name)
         ):
-            labels_key = form_name(self.target_prefix, self.batch_idx, self.rank)
-            self.client.put_tensor(labels_key, targets)
+            batch_ds.add_tensor(self.target_name, targets)
+            if self.verbose:
+                logger.info(f"Putting dataset {batch_ds_name} with samples and targets")
+        else:
+            if self.verbose:
+                logger.info(f"Putting dataset {batch_ds_name} with samples")
+
+        self.client.put_dataset(batch_ds)
+        self.client.append_to_list(self.list_name, batch_ds)
+        if self.verbose:
+            logger.info(f"Added dataset to list {self.list_name}")
+            logger.info(f"List length {self.client.get_list_length(self.list_name)}")
 
         self.batch_idx += 1
 
 
-class StaticDataDownloader:
+class DataDownloader:
     """A class to download a dataset from the DB.
 
-    By default, the StaticDataDownloader has to be created in a process
+    By default, the DataDownloader has to be created in a process
     launched through SmartSim, with sample producers listed as incoming
     entities.
 
-    All details about the batches must be defined in
-    the constructor; two mechanisms are available, `manual` and
-    `auto`.
-
-     - When specifying `auto`, the user must also specify
-      `uploader_name`. StaticDataDownloader will get all needed information
-      from the database (this expects a Dataset like the one created
-      by TrainingDataUploader to be available and stored as `uploader_name`
-      on the DB).
-
-     - When specifying `manual`, the user must also specify details
-       of batch naming. Specifically, for each incoming entity with
-       a name starting with an element of `producer_prefixes`,
-       StaticDataDownloader will query the DB
-       for all batches named <sample_prefix>_<sub_index> for all indices
-       in `sub_indexes` if supplied, and, if
-       `target_prefix` is supplied, it will also query for all targets
-       named <target_prefix>.<sub_index>. If `producer_prefixes` is
-       None, then all incoming entities will be treated as producers,
-       and for each one, the corresponding batches will be downloaded.
+    Information about the uploaded datasets can be defined in two ways:
 
-    The flag `init_samples` defines whether sources (the list of batches
-    to be fetched) and samples (the actual data) should automatically
+     - By supplying a DataInfo object as value of ``data_info_or_list_name``
+
+     - By supplying a string as value of ``data_info_or_list_name``.
+       in this case, an attempt is made to download information from the
+       DB, where a Dataset called ``<data_info_or_list_name>_info`` should be available
+       and have the information normally stored by DataInfo.publish()
+
+    The flag `init_samples` defines whether samples should automatically
     be set up in the costructor.
 
-    If the user needs to modify the list of sources, then `init_samples=False`
-    has to be set. In that case, to set up a `BatchDownlaoder`, the user has to call
-    `init_sources()` (which initializes the list of sources and the SmartRedis client)
-    and `init_samples()`.  After `init_sources()` is called,
-    a list of data sources is populated, representing the batches which
-    will be downloaded.
-
-    Each source is represented as a tuple `(producer_name, sub_index)`.
-    Before `init_samples()` is called, the user can modify the list.
-    Once `init_samples()` is called, all data is downloaded and batches
-    can be obtained with iter().
-
-    After initialization, samples and targets will not be updated. The data can
-    be shuffled by calling `update_data()`, if `shuffle` is set to ``True`` at
-    initialization.
+    If the user needs to modify the `DataDownloader` object before starting
+    the training, then `init_samples=False` has to be set.
+    In that case, to set up a `DataDownloader`, the user has to call
+    `init_samples()`.
+
+    Calling `update_data()`
+     - check if new batches are available and download them, if `dynamic` is set to `True`
+     - shuffle the dataset if `shuffle` is set to ``True``.
 
     :param batch_size: Size of batches obtained with __iter__
     :type batch_size: int
+    :param dynamic: Whether new batches should be donwnloaded when ``update_data`` is called.
+    :type dtnamic: bool
     :param shuffle: whether order of samples has to be shuffled when calling `update_data`
     :type shuffle: bool
-    :param uploader_info: Set to `auto` uploader information has to be downloaded from DB,
-                          or to `manual` if it is provided by the user
-    :type uploader_info: str
-    :param uploader_name: Name of uploader info dataset, only used if `uploader_info` is `auto`
-    :type uploader_name: str
-    :param sample_prefix: prefix of keys representing batches
-    :type sample_prefix: str
-    :param target_prefix: prefix of keys representing targets
-    :type target_prefix: str
-    :param uploader_ranks: Number of processes every uploader runs on (e.g, if each
-                           rank in an MPI simulation is uploading its own batches,
-                           this will be the MPI comm world size of the simulation).
-    :type uploader_ranks: int
-    :param num_classes: Number of classes of targets, if categorical
-    :type num_classes: int
-    :param producer_prefixes: Prefixes of names of which will be producing batches.
-                              These can be e.g. prefixes of SmartSim entity names in
-                              an ensemble.
-    :type producer_prefixes: str
+    :param data_info_or_list_name: DataInfo object with details about dataset to download, if a string is passed,
+                      it is used to download DataInfo data from DB, assuming it was stored with
+                      ``list_name=data_info_or_list_name``
+    :type data_info_or_list_name: DataInfo | str
+    :param list_name: Name of aggregation list used to upload data
+    :type list_name: str
     :param cluster: Whether the Orchestrator will be run as a cluster
     :type cluster: bool
     :param address: Address of Redis client as <ip_address>:<port>
     :type address: str
     :param replica_rank: When StaticDataDownloader is used distributedly, indicates
                          the rank of this object
     :type replica_rank: int
     :param num_replicas: When BatchDownlaoder is used distributedly, indicates
                          the total number of ranks
     :type num_replicas: int
     :param verbose: Whether log messages should be printed
     :type verbose: bool
     :param init_samples: whether samples should be initialized in the constructor
     :type init_samples: bool
+    :param max_fetch_trials: maximum number of attempts to initialize data
+    :type max_fetch_trials: int
     """
 
     def __init__(
         self,
+        data_info_or_list_name,
         batch_size=32,
+        dynamic=True,
         shuffle=True,
-        uploader_info="auto",
-        uploader_name="training_data",
-        sample_prefix="samples",
-        target_prefix="targets",
-        uploader_ranks=None,
-        num_classes=None,
-        producer_prefixes=None,
         cluster=True,
         address=None,
         replica_rank=0,
         num_replicas=1,
         verbose=False,
         init_samples=True,
-        **kwargs,
+        max_fetch_trials=-1,
     ):
-        self.replica_rank = replica_rank
-        self.num_replicas = num_replicas
         self.address = address
         self.cluster = cluster
-        self.uploader_info = uploader_info
-        self.uploader_name = uploader_name
         self.verbose = verbose
         self.samples = None
         self.targets = None
         self.num_samples = 0
         self.indices = np.arange(0)
         self.shuffle = shuffle
+        self.dynamic = dynamic
         self.batch_size = batch_size
-        if uploader_info == "manual":
-            self.sample_prefix = sample_prefix
-            self.target_prefix = target_prefix
-            if uploader_ranks is not None:
-                self.sub_indices = [str(rank) for rank in range(uploader_ranks)]
-            else:
-                self.sub_indices = None
-            if producer_prefixes:
-                self.producer_prefixes = list(producer_prefixes)
-            else:
-                producer_prefixes = [""]
-            self.num_classes = num_classes
-        elif self.uploader_info == "auto":
-            pass
+        if isinstance(data_info_or_list_name, DataInfo):
+            self._info = data_info_or_list_name
+        elif isinstance(data_info_or_list_name, str):
+            self._info = DataInfo(list_name=data_info_or_list_name)
+            client = Client(self.address, self.cluster)
+            self._info.download(client)
         else:
-            raise ValueError(
-                f"uploader_info must be one of 'auto' or 'manual', but was {self.uploader_info}"
-            )
+            raise TypeError("data_info_or_list_name must be either DataInfo or str")
+        self.client = None
+        sskeyin = environ.get("SSKEYIN", "")
+        self.uploader_keys = sskeyin.split(",")
+
+        self.set_replica_parameters(replica_rank, num_replicas)
 
         if init_samples:
-            self.init_sources()
-            self.init_samples()
-        else:
-            self.client = Client(self.address, self.cluster)
-            if self.uploader_info == "auto":
-                if not self.uploader_name:
-                    raise ValueError(
-                        "uploader_name can not be empty if uploader_info is 'auto'"
-                    )
-                self._get_uploader_info(self.uploader_name)
-            # This avoids problems with Pytorch
-            self.client = None
+            self.init_samples(max_fetch_trials)
 
     def log(self, message):
         if self.verbose:
             logger.info(message)
 
-    def _list_all_sources(self):
-        uploaders = environ["SSKEYIN"].split(",")
-        sources = []
-        for uploader in uploaders:
-            if any(
-                [
-                    uploader.startswith(producer_prefix)
-                    for producer_prefix in self.producer_prefixes
-                ]
-            ):
-                if self.sub_indices:
-                    sources.extend(
-                        [[uploader, sub_index] for sub_index in self.sub_indices]
-                    )
-                else:
-                    sources.append([uploader, None])
-
-        per_replica = len(sources) // self.num_replicas
-        if per_replica > 0:
-            if self.replica_rank < self.num_replicas - 1:
-                sources = sources[
-                    self.replica_rank
-                    * per_replica : (self.replica_rank + 1)
-                    * per_replica
-                ]
-            else:
-                sources = sources[self.replica_rank * per_replica :]
-        else:
-            self.log(
-                "Number of loader replicas is higher than number of sources, automatic split cannot be performed, "
-                "all replicas will have the same dataset. If this is not intended, then implement a distribution strategy "
-                "and modify `sources`."
-            )
-
-        return sources
+    def set_replica_parameters(self, replica_rank, num_replicas):
+        self.replica_rank = replica_rank
+        self.num_replicas = num_replicas
+        self.next_indices = [self.replica_rank] * max(1, len(self.uploader_keys))
 
-    def init_sources(self):
-        """Initalize list of data sources based on incoming entitites and self.sub_indices.
+    @property
+    def autoencoding(self):
+        return self.sample_name == self.target_name
 
+    @property
+    def list_name(self):
+        return self._info.list_name
 
-        Each source is represented as a tuple `(producer_name, sub_index)`.
-        Before `init_samples()` is called, the user can modify the list.
-        Once `init_samples()` is called, all data is downloaded and batches
-        can be obtained with iter(). The list of all sources is stored as `self.sources`.
+    @property
+    def sample_name(self):
+        return self._info.sample_name
 
-        :raises ValueError: If self.uploader_info is set to `auto` but no `uploader_name` is specified.
-        :raises ValueError: If self.uploader_info is not set to `auto` or `manual`.
-        """
-        self.client = Client(self.address, self.cluster)
-        if self.uploader_info == "auto":
-            if not self.uploader_name:
-                raise ValueError(
-                    "uploader_name can not be empty if uploader_info is 'auto'"
-                )
-            self._get_uploader_info(self.uploader_name)
-        elif self.uploader_info == "manual":
-            pass
-        else:
-            raise ValueError(
-                f"uploader_info must be one of 'auto' or 'manual', but was {self.uploader_info}"
-            )
+    @property
+    def target_name(self):
+        return self._info.target_name
 
-        self.sources = self._list_all_sources()
+    @property
+    def num_classes(self):
+        return self._info.num_classes
 
     @property
     def need_targets(self):
         """Compute if targets have to be downloaded.
 
         :return: Whether targets (or labels) should be downloaded
         :rtype: bool
         """
-        return self.target_prefix and not self.autoencoding
+        return self.target_name and not self.autoencoding
 
     def __len__(self):
         length = int(np.floor(self.num_samples / self.batch_size))
         return length
 
     def __iter__(self):
 
-        if self.sources:
-            self.update_data()
-            # Generate data
-            if len(self) < 1:
-                msg = "Not enough samples in generator for one batch. "
-                msg += "Please run init_samples() or initialize generator with init_samples=True"
-                raise ValueError(msg)
-
-            for index in range(len(self)):
-                indices = self.indices[
-                    index * self.batch_size : (index + 1) * self.batch_size
-                ]
-
-                x, y = self.__data_generation(indices)
+        self.update_data()
+        # Generate data
+        if len(self) < 1:
+            msg = "Not enough samples in generator for one batch. "
+            msg += "Please run init_samples() or initialize generator with init_samples=True"
+            raise ValueError(msg)
+
+        _calc_indices = lambda index: self.indices[
+            index * self.batch_size : (index + 1) * self.batch_size
+        ]
+        yield from (
+            self._data_generation(_calc_indices(idx)) for idx in range(len(self))
+        )
 
-                if y is not None:
-                    yield x, y
-                else:
-                    yield x
-
-    def init_samples(self, sources=None):
+    def init_samples(self, init_trials=-1):
         """Initialize samples (and targets, if needed).
 
-        This function will not return until samples have been downloaded
-        from all sources.
-
-        :param sources: List of sources as defined in `init_sources`, defaults to None,
-                        in which case sources will be initialized, unless `self.sources`
-                        is already set
-        :type sources: list[tuple], optional
+        A new attempt to download samples will be made every ten seconds, for ``init_trials``
+        times.
+        :param init_trials: maximum number of attempts to fetch data
+        :type init_trials: int
         """
-        self.autoencoding = self.sample_prefix == self.target_prefix
-
-        if sources is not None:
-            self.sources = sources
-
-        if self.sources is None:
-            self.sources = self._list_all_sources()
+        self.client = Client(self.address, self.cluster)
 
-        self.log("Generator initialization complete")
+        num_trials = 0
+        max_trials = init_trials or -1
+        while not len(self) and num_trials != max_trials:
+            self._update_samples_and_targets()
+            self.log(
+                "DataLoader could not download samples, will try again in 10 seconds"
+            )
+            time.sleep(10)
+            num_trials += 1
 
-        self._update_samples_and_targets()
+        if not len(self):
+            raise SSInternalError(
+                "Could not download samples in given number of trials"
+            )
         if self.shuffle:
             np.random.shuffle(self.indices)
 
     def _data_exists(self, batch_name, target_name):
 
         if self.need_targets:
             return self.client.tensor_exists(batch_name) and self.client.tensor_exists(
                 target_name
             )
         else:
             return self.client.tensor_exists(batch_name)
 
-    def _add_samples(self, batch_name, target_name):
+    def _add_samples(self, indices):
+
+        if self.num_replicas == 1:
+            datasets: list[Dataset] = self.client.get_dataset_list_range(
+                self.list_name, start_index=indices[0], end_index=indices[-1]
+            )
+        else:
+            datasets: list[Dataset] = []
+            for idx in indices:
+                datasets += self.client.get_dataset_list_range(
+                    self.list_name, start_index=idx, end_index=idx
+                )
+
         if self.samples is None:
-            self.samples = self.client.get_tensor(batch_name)
+            self.samples = datasets[0].get_tensor(self.sample_name)
             if self.need_targets:
-                self.targets = self.client.get_tensor(target_name)
-        else:
+                self.targets = datasets[0].get_tensor(self.target_name)
+
+            if len(datasets) > 1:
+                datasets = datasets[1:]
+
+        for dataset in datasets:
             self.samples = np.concatenate(
-                (self.samples, self.client.get_tensor(batch_name))
+                (self.samples, dataset.get_tensor(self.sample_name))
             )
             if self.need_targets:
                 self.targets = np.concatenate(
-                    (self.targets, self.client.get_tensor(target_name))
+                    (self.targets, dataset.get_tensor(self.target_name))
                 )
 
         self.num_samples = self.samples.shape[0]
         self.indices = np.arange(self.num_samples)
-        self.log("Success!")
         self.log(f"New dataset size: {self.num_samples}, batches: {len(self)}")
 
-    def _get_uploader_info(self, uploader_name):
-        dataset_name = form_name(uploader_name, "info")
-        self.log(f"Uploader dataset name: {dataset_name}")
-
-        ds_exists = False
-        try:
-            ds_exists = self.client.dataset_exists(dataset_name)
-        # As long as required SmartRedis version is not 0.3 we
-        # need a workaround for the missing function
-        except AttributeError:
-            try:
-                uploaders = environ["SSKEYIN"].split(",")
-                for uploader in uploaders:
-                    if self.client.key_exists(uploader + "." + dataset_name):
-                        ds_exists = True
-            except KeyError:
-                msg = "Uploader must be launched with SmartSim and added to incoming entity, "
-                msg += "when setting uploader_info to 'auto'"
-                raise SmartSimError(msg)
-
-        trials = 6
-        while not ds_exists:
-            trials -= 1
-            if trials == 0:
-                raise SmartSimError("Could not find uploader dataset")
-            time.sleep(5)
-            try:
-                ds_exists = self.client.dataset_exists(dataset_name)
-            except AttributeError:
-                try:
-                    uploaders = environ["SSKEYIN"].split(",")
-                    for uploader in uploaders:
-                        if self.client.key_exists(uploader + "." + dataset_name):
-                            ds_exists = True
-                except KeyError:
-                    msg = "Uploader must be launched with SmartSim and added to incoming entity, "
-                    msg += "when setting uploader_info to 'auto'"
-                    raise SmartSimError(msg)
-
-        uploader_info = self.client.get_dataset(dataset_name)
-        self.sample_prefix = uploader_info.get_meta_strings("sample_prefix")[0]
-        self.log(f"Uploader sample prefix: {self.sample_prefix}")
-
-        try:
-            self.target_prefix = uploader_info.get_meta_strings("target_prefix")[0]
-        except:
-            self.target_prefix = None
-        self.log(f"Uploader target prefix: {self.target_prefix}")
-
-        try:
-            self.producer_prefixes = uploader_info.get_meta_strings("producer_prefixes")
-        except:
-            self.producer_prefixes = [""]
-        self.log(f"Uploader producer prefixes: {self.producer_prefixes}")
-
-        try:
-            self.num_classes = uploader_info.get_meta_scalars("num_classes")[0]
-        except:
-            self.num_classes = None
-        self.log(f"Uploader num classes: {self.num_classes}")
-
-        try:
-            num_ranks = uploader_info.get_meta_scalars("num_ranks")[0]
-            self.sub_indices = [str(rank) for rank in range(num_ranks)]
-        except:
-            self.sub_indices = None
-        self.log(f"Uploader sub-indices: {self.sub_indices}")
-
     def _update_samples_and_targets(self):
-        for source in self.sources:
-            entity = source[0]
-            sub_index = source[1]
-            self.client.set_data_source(entity)
-            batch_name = form_name(self.sample_prefix, sub_index)
-            if self.need_targets:
-                target_name = form_name(self.target_prefix, sub_index)
-            else:
-                target_name = None
-
-            self.log(f"Retrieving {batch_name} from {entity}")
-            trials = 6
-            while not self._data_exists(batch_name, target_name):
-                trials -= 1
-                if trials == 0:
-                    raise SmartSimError(
-                        f"Could not retrieve batch {batch_name} from entity {entity}"
-                    )
-                time.sleep(5)
+        if not self.client:
+            self.client = Client(self.address, self.cluster)
+            
+        self.log(f"Rank {self.replica_rank} out of {self.num_replicas} replicas")
 
-            self._add_samples(batch_name, target_name)
+        for uploader_idx, uploader_key in enumerate(self.uploader_keys):
+            if uploader_key:
+                self.client.use_list_ensemble_prefix(True)
+                self.client.set_data_source(uploader_key)
+
+            list_length = self.client.get_list_length(self.list_name)
+
+            # Strictly greater, because next_index is 0-based
+            if list_length > self.next_indices[uploader_idx]:
+                indices = [
+                    idx
+                    for idx in range(
+                        self.next_indices[uploader_idx], list_length, self.num_replicas
+                    )
+                ]
+                self._add_samples(indices)
+                self.next_indices[uploader_idx] = indices[-1] + self.num_replicas
 
     def update_data(self):
-        self._update_samples_and_targets()
+        if self.dynamic:
+            self._update_samples_and_targets()
+        if self.shuffle:
+            np.random.shuffle(self.indices)
 
-    def __data_generation(self, indices):
+    def _data_generation(self, indices):
         # Initialization
         x = self.samples[indices]
 
         if self.need_targets:
             y = self.targets[indices]
-
         elif self.autoencoding:
             y = x
         else:
-            y = None
+            return x
 
         return x, y
-
-    def __len__(self):
-        length = int(np.floor(self.num_samples / self.batch_size))
-        return length
-
-
-class DynamicDataDownloader(StaticDataDownloader):
-    """A class to download batches from the DB as they are produced.
-
-    By default, the DynamicDataDownloader has to be created in a process
-    launched through SmartSim, with sample producers listed as incoming
-    entities.
-
-    All details about the batches must be defined in
-    the constructor; two mechanisms are available, `manual` and
-    `auto`.
-
-     - When specifying `auto`, the user must also specify
-      `uploader_name`. DynamicDataDownloader will get all needed information
-      from the database (this expects a Dataset like the one created
-      by TrainingDataUploader to be available and stored as `uploader_name`
-      on the DB).
-
-     - When specifying `manual`, the user must also specify details
-       of batch naming. Specifically, for each incoming entity with
-       a name starting with an element of `producer_prefixes`,
-       DynamicDataDownloader will query the DB
-       for all batches named <sample_prefix>_<sub_index>_<iteration> for all indices
-       in `sub_indices` if supplied, and, if
-       `target_prefix` is supplied, it will also query for all targets
-       named <target_prefix>.<sub_index>.<iteration>. If `producer_prefixes` is
-       None, then all incoming entities will be treated as producers,
-       and for each one, the corresponding batches will be downloaded.
-
-    The flag `init_samples` defines whether sources (the list of batches
-    to be fetched) and samples (the actual data) should automatically
-    be set up in the costructor.
-
-    If the user needs to modify the list of sources, then `init_samples=False`
-    has to be set. In that case, to set up a `DynamicDataDownloader`, the user has to call
-    `init_sources()` (which initializes the list of sources and the SmartRedis client)
-    and `init_samples()`.  After `init_sources()` is called,
-    a list of data sources is populated, representing the batches which
-    will be downloaded. See `init_sources()`
-
-    Each source is represented as a tuple `(producer_name, sub_index, iteration)`.
-    Before `init_samples()` is called, the user can modify the list.
-    Once `init_samples()` is called, all data is downloaded and batches
-    can be obtained with iter().
-
-    After initialization, samples and targets can be updated calling `update_data()`,
-    which shuffles the available samples, if `shuffle` is set to ``True`` at initialization.
-
-    :param batch_size: Size of batches obtained with __iter__
-    :type batch_size: int
-    :param shuffle: whether order of samples has to be shuffled when calling `update_data`
-    :type shuffle: bool
-    :param uploader_info: Set to `auto` uploader information has to be downloaded from DB,
-                          or to `manual` if it is provided by the user
-    :type uploader_info: str
-    :param uploader_name: Name of uploader info dataset, only used if `uploader_info` is `auto`
-    :type uploader_name: str
-    :param sample_prefix: prefix of keys representing batches
-    :type sample_prefix: str
-    :param target_prefix: prefix of keys representing targets
-    :type target_prefix: str
-    :param uploader_ranks: Number of processes every uploader runs on (e.g, if each
-                           rank in an MPI simulation is uploading its own batches,
-                           this will be the MPI comm world size of the simulation).
-    :type uploader_ranks: int
-    :param num_classes: Number of classes of targets, if categorical
-    :type num_classes: int
-    :param producer_prefixes: Prefixes of processes which will be producing batches.
-                              This can be useful in case the consumer processes also
-                              have other incoming entities.
-    :type producer_prefixes: str
-    :param cluster: Whether the Orchestrator is being run as a cluster
-    :type cluster: bool
-    :param address: Address of Redis DB as <ip_address>:<port>
-    :type address: str
-    :param replica_rank: When StaticDataDownloader is used in a distributed setting, indicates
-                         the rank of this replica
-    :type replica_rank: int
-    :param num_replicas: When ContinuousBatchDownlaoder is used in a distributed setting,
-                         indicates the total number of replicas (ranks)
-    :type num_replicas: int
-    :param verbose: Whether log messages should be printed
-    :type verbose: bool
-    :param init_samples: whether samples should be initialized in the constructor
-    :type init_samples: bool
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def _list_all_sources(self):
-        sources = super()._list_all_sources()
-        # Append the batch index to each source
-        for source in sources:
-            source.append(0)
-        return sources
-
-    def _update_samples_and_targets(self):
-        for source in self.sources:
-            entity = source[0]
-            sub_index = source[1]
-            index = source[2]
-            self.client.set_data_source(entity)
-            batch_name = form_name(self.sample_prefix, index, sub_index)
-            if self.need_targets:
-                target_name = form_name(self.target_prefix, index, sub_index)
-            else:
-                target_name = None
-
-            self.log(f"Retrieving {batch_name} from {entity}")
-            # Poll next batch based on index, if available: retrieve it, update index and loop
-            while self._data_exists(batch_name, target_name):
-                self._add_samples(batch_name, target_name)
-                source[2] += 1
-                index = source[2]
-                batch_name = form_name(self.sample_prefix, index, sub_index)
-                if self.need_targets:
-                    target_name = form_name(self.target_prefix, index, sub_index)
-
-                self.log(f"Retrieving {batch_name}...")
-
-    def update_data(self):
-        """Update data.
-
-        Fetch new batches (if available) from the DB. Also shuffle
-        list of samples if `self.shuffle` is set to ``True``.
-        """
-        self._update_samples_and_targets()
-        if self.shuffle:
-            np.random.shuffle(self.indices)
-
-    def init_samples(self, sources=None):
-        """Initialize samples (and targets, if needed).
-
-        This function will not return until at least one batch worth of data
-        has been downloaded.
-
-        :param sources: List of sources as defined in `init_sources`, defaults to None,
-                        in which case sources will be initialized, unless `self.sources`
-                        is already set
-        :type sources: list[tuple], optional
-        """
-        self.autoencoding = self.sample_prefix == self.target_prefix
-
-        if sources is not None:
-            self.sources = sources
-
-        if self.sources is None:
-            self.sources = self._list_all_sources()
-
-        if self.sources:
-
-            while len(self) < 1:
-                self._update_samples_and_targets()
-                trials = 6
-                if len(self) < 1:
-                    trials -= 1
-                    if trials == 0:
-                        raise SmartSimError("Could not find samples")
-                    time.sleep(5)
-            self.log("Generator initialization complete")
-        else:
-            self.log(
-                "Generator has no associated sources, this can happen if the number of "
-                "loader workers is larger than the number of available sources."
-            )
```

### Comparing `smartsim-0.4.1/smartsim/settings/alpsSettings.py` & `smartsim-0.4.2/smartsim/settings/alpsSettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/settings/base.py` & `smartsim-0.4.2/smartsim/settings/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # BSD 2-Clause License #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/settings/cobaltSettings.py` & `smartsim-0.4.2/smartsim/settings/cobaltSettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/settings/lsfSettings.py` & `smartsim-0.4.2/smartsim/settings/lsfSettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -81,15 +81,15 @@
         """Set the number of cpus to use per resource set
 
         This sets ``--cpu_per_rs``
 
         :param cpus_per_rs: number of cpus to use per resource set or ALL_CPUS
         :type cpus_per_rs: int or str
         """
-        if self.colocated_db_settings == True:
+        if self.colocated_db_settings:
             db_cpus = self.colocated_db_settings["db_cpus"]
             if cpus_per_rs < db_cpus:
                 raise ValueError(
                     f"Cannot set cpus_per_rs ({cpus_per_rs}) to less than db_cpus ({db_cpus})"
                 )
         if isinstance(cpus_per_rs, str):
             self.run_args["cpu_per_rs"] = cpus_per_rs
```

### Comparing `smartsim-0.4.1/smartsim/settings/mpirunSettings.py` & `smartsim-0.4.2/smartsim/settings/mpiSettings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -20,31 +20,38 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import shutil
 import subprocess
-import re
 
-from ..error import SSUnsupportedError
+from ..error import LauncherError, SSUnsupportedError
 from ..log import get_logger
 from .base import RunSettings
 
 logger = get_logger(__name__)
 
 
-class _OpenMPISettings(RunSettings):
-    """Base class for all common arguments of OpenMPI run commands"""
+class _BaseMPISettings(RunSettings):
+    """Base class for all common arguments of MPI-standard run commands"""
 
     def __init__(
-        self, exe, exe_args=None, run_command="", run_args=None, env_vars=None, **kwargs
+        self,
+        exe,
+        exe_args=None,
+        run_command="mpiexec",
+        run_args=None,
+        env_vars=None,
+        fail_if_missing_exec=True,
+        **kwargs,
     ):
-        """Settings to format run job with an OpenMPI binary
+        """Settings to format run job with an MPI-standard binary
 
         Note that environment variables can be passed with a None
         value to signify that they should be exported from the current
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
         command line arguments and prefixed with ``--``. Values of
@@ -54,25 +61,38 @@
         :type exe: str
         :param exe_args: executable arguments, defaults to None
         :type exe_args: str | list[str], optional
         :param run_args: arguments for run command, defaults to None
         :type run_args: dict[str, str], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
+        :param fail_if_missing_exec: Throw an exception of the MPI command
+                                     is missing. Otherwise, throw a warning
+        :type fail_if_missing_exec: bool, optional
         """
         super().__init__(
             exe,
             exe_args,
             run_command=run_command,
             run_args=run_args,
             env_vars=env_vars,
             **kwargs,
         )
         self.mpmd = []
 
+        if not shutil.which(self._run_command):
+            msg = (
+                f"Cannot find {self._run_command}. Try passing the "
+                "full path via run_command."
+            )
+            if fail_if_missing_exec:
+                raise LauncherError(msg)
+            else:
+                logger.warning(msg)
+
     reserved_run_args = {"wd", "wdir"}
 
     def make_mpmd(self, mpirun_settings):
         """Make a mpmd workload by combining two ``mpirun`` commands
 
         This connects the two settings to be executed with a single
         Model instance
@@ -97,36 +117,46 @@
         :type task_mapping: str
         """
         self.run_args["map-by"] = str(task_mapping)
 
     def set_cpus_per_task(self, cpus_per_task):
         """Set the number of tasks for this job
 
-        This sets ``--cpus-per-proc``
+        This sets ``--cpus-per-proc`` for MPI compliant implementations
 
         note: this option has been deprecated in openMPI 4.0+
         and will soon be replaced.
 
         :param cpus_per_task: number of tasks
         :type cpus_per_task: int
         """
         self.run_args["cpus-per-proc"] = int(cpus_per_task)
 
+    def set_cpu_binding_type(self, bind_type):
+        """Specifies the cores to which MPI processes are bound
+
+        This sets ``--bind-to`` for MPI compliant implementations
+
+        :param bind_type: binding type
+        :type bind_type: str
+        """
+        self.run_args["bind-to"] = str(bind_type)
+
     def set_tasks_per_node(self, tasks_per_node):
         """Set the number of tasks per node
 
         :param tasks_per_node: number of tasks to launch per node
         :type tasks_per_node: int
         """
         self.run_args["npernode"] = int(tasks_per_node)
 
     def set_tasks(self, tasks):
         """Set the number of tasks for this job
 
-        This sets ``--n``
+        This sets ``-n`` for MPI compliant implementations
 
         :param tasks: number of tasks
         :type tasks: int
         """
         self.run_args["n"] = int(tasks)
 
     def set_hostlist(self, host_list):
@@ -206,17 +236,17 @@
 
         :param walltime: number like string of seconds that a job will run in secs
         :type walltime: str
         """
         self.run_args["timeout"] = str(walltime)
 
     def format_run_args(self):
-        """Return a list of OpenMPI formatted run arguments
+        """Return a list of MPI-standard formatted run arguments
 
-        :return: list of OpenMPI arguments for these settings
+        :return: list of MPI-standard arguments for these settings
         :rtype: list[str]
         """
         # args launcher uses
         args = []
         restricted = ["wdir", "wd"]
 
         for opt, value in self.run_args.items():
@@ -231,27 +261,28 @@
     def format_env_vars(self):
         """Format the environment variables for mpirun
 
         :return: list of env vars
         :rtype: list[str]
         """
         formatted = []
+        env_string = "-x"
 
         if self.env_vars:
             for name, value in self.env_vars.items():
                 if value:
-                    formatted += ["-x", "=".join((name, str(value)))]
+                    formatted += [env_string, "=".join((name, str(value)))]
                 else:
-                    formatted += ["-x", name]
+                    formatted += [env_string, name]
         return formatted
 
 
-class MpirunSettings(_OpenMPISettings):
+class MpirunSettings(_BaseMPISettings):
     def __init__(self, exe, exe_args=None, run_args=None, env_vars=None, **kwargs):
-        """Settings to run job with ``mpirun`` command (OpenMPI)
+        """Settings to run job with ``mpirun`` command (MPI-standard)
 
         Note that environment variables can be passed with a None
         value to signify that they should be exported from the current
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
         into ``mpirun`` arguments and prefixed with ``--``. Values of
@@ -264,26 +295,18 @@
         :param run_args: arguments for run command, defaults to None
         :type run_args: dict[str, str], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
         """
         super().__init__(exe, exe_args, "mpirun", run_args, env_vars, **kwargs)
 
-        completed_process = subprocess.run(
-            [self.run_command, "-V"], capture_output=True
-        )  # type: subprocess.CompletedProcess
-        version_statement = completed_process.stdout.decode()
-
-        if not re.match(r"mpirun\s\(Open MPI\)\s4.\d+.\d+", version_statement):
-            logger.warning("Non-OpenMPI implementation of `mpirun` detected")
 
-
-class MpiexecSettings(_OpenMPISettings):
+class MpiexecSettings(_BaseMPISettings):
     def __init__(self, exe, exe_args=None, run_args=None, env_vars=None, **kwargs):
-        """Settings to run job with ``mpiexec`` command (OpenMPI)
+        """Settings to run job with ``mpiexec`` command (MPI-standard)
 
         Note that environment variables can be passed with a None
         value to signify that they should be exported from the current
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
         into ``mpiexec`` arguments and prefixed with ``--``. Values of
@@ -297,25 +320,26 @@
         :type run_args: dict[str, str], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
         """
         super().__init__(exe, exe_args, "mpiexec", run_args, env_vars, **kwargs)
 
         completed_process = subprocess.run(
-            [self.run_command, "-V"], capture_output=True
-        )  # type: subprocess.CompletedProcess
-        version_statement = completed_process.stdout.decode()
-
-        if not re.match(r"mpiexec\s\(OpenRTE\)\s4.\d+.\d+", version_statement):
-            logger.warning("Non-OpenMPI implementation of `mpiexec` detected")
+            [self._run_command, "--help"], capture_output=True
+        )
+        help_statement = completed_process.stdout.decode()
+        if "mpiexec.slurm" in help_statement:
+            raise SSUnsupportedError(
+                "Slurm's wrapper for mpiexec is unsupported. Use slurmSettings instead"
+            )
 
 
-class OrterunSettings(_OpenMPISettings):
+class OrterunSettings(_BaseMPISettings):
     def __init__(self, exe, exe_args=None, run_args=None, env_vars=None, **kwargs):
-        """Settings to run job with ``orterun`` command (OpenMPI)
+        """Settings to run job with ``orterun`` command (MPI-standard)
 
         Note that environment variables can be passed with a None
         value to signify that they should be exported from the current
         environment
 
         Any arguments passed in the ``run_args`` dict will be converted
         into ``orterun`` arguments and prefixed with ``--``. Values of
@@ -327,15 +351,7 @@
         :type exe_args: str | list[str], optional
         :param run_args: arguments for run command, defaults to None
         :type run_args: dict[str, str], optional
         :param env_vars: environment vars to launch job with, defaults to None
         :type env_vars: dict[str, str], optional
         """
         super().__init__(exe, exe_args, "orterun", run_args, env_vars, **kwargs)
-
-        completed_process = subprocess.run(
-            [self.run_command, "-V"], capture_output=True
-        )  # type: subprocess.CompletedProcess
-        version_statement = completed_process.stdout.decode()
-
-        if not re.match(r"orterun\s\(OpenRTE\)\s4.\d+.\d+", version_statement):
-            logger.warning("Non-OpenMPI implementation of `orterun` detected")
```

### Comparing `smartsim-0.4.1/smartsim/settings/pbsSettings.py` & `smartsim-0.4.2/smartsim/settings/pbsSettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/settings/settings.py` & `smartsim-0.4.2/smartsim/settings/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -160,13 +160,17 @@
         if launcher == "local":
             run_command = None
         else:
             run_command = _detect_command(launcher)
 
     # if user specified and supported or auto detection worked
     if run_command and run_command in supported:
-        return supported[run_command](exe, exe_args, run_args, env_vars, container=container, **kwargs)
+        return supported[run_command](
+            exe, exe_args, run_args, env_vars, container=container, **kwargs
+        )
 
     # 1) user specified and not implementation in SmartSim
     # 2) user supplied run_command=None
     # 3) local launcher being used and default of "auto" was passed.
-    return RunSettings(exe, exe_args, run_command, run_args, env_vars, container=container)
+    return RunSettings(
+        exe, exe_args, run_command, run_args, env_vars, container=container
+    )
```

### Comparing `smartsim-0.4.1/smartsim/slurm.py` & `smartsim-0.4.2/smartsim/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/status.py` & `smartsim-0.4.2/smartsim/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim/wlm/slurm.py` & `smartsim-0.4.2/smartsim/wlm/slurm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 2-Clause License
 #
-# Copyright (c) 2021-2022, Hewlett Packard Enterprise
+# Copyright (c) 2021-2023, Hewlett Packard Enterprise
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # 1. Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
```

### Comparing `smartsim-0.4.1/smartsim.egg-info/PKG-INFO` & `smartsim-0.4.2/smartsim.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsim
-Version: 0.4.1
+Version: 0.4.2
 Summary: AI Workflows for Science
 Home-page: https://github.com/CrayLabs/SmartSim
 Author: CrayLabs, a Hewlett Packard Enterprise OSS Organization
 Author-email: craylabs@hpe.com
 License: BSD 2-Clause License
 Project-URL: Source, https://github.com/CrayLabs/SmartSim
 Project-URL: Documentation, https://www.craylabs.org
@@ -22,25 +22,29 @@
             <a href="https://github.com/CrayLabs"><b>Cray Labs</b></a>&nbsp;&nbsp;&nbsp;
           </div>
             <br />
             <br />
         </div>
         
         
+        <div align="center">
+        
         [![License](https://img.shields.io/github/license/CrayLabs/SmartSim)](https://github.com/CrayLabs/SmartSim/blob/master/LICENSE.md)
         ![GitHub last commit](https://img.shields.io/github/last-commit/CrayLabs/SmartSim)
         ![GitHub deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/github-pages?label=doc%20build)
         ![PyPI - Wheel](https://img.shields.io/pypi/wheel/smartsim)
         ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/smartsim)
         ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/CrayLabs/SmartSim)
         ![Language](https://img.shields.io/github/languages/top/CrayLabs/SmartSim)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![codecov](https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim)
         [![Downloads](https://static.pepy.tech/personalized-badge/smartsim?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/smartsim)
         
+        </div>
+        
         ------------
         
         # SmartSim
         
         SmartSim is made up of two parts
           1. SmartSim Infrastructure Library (This repository)
           2. [SmartRedis](https://github.com/CrayLabs/SmartRedis)
@@ -75,16 +79,14 @@
             - [Interactive Launch Example](#interactive-launch-example)
             - [Batch Launch Examples](#batch-launch-examples)
         - [Infrastructure Library Applications](#infrastructure-library-applications)
           - [Redis + RedisAI](#redis--redisai)
             - [Local Launch](#local-launch)
             - [Interactive Launch](#interactive-launch)
             - [Batch Launch](#batch-launch)
-          - [Ray](#ray)
-            - [Ray on HPC](#ray-on-hpc)
         - [SmartRedis](#smartredis)
           - [Tensors](#tensors)
           - [Datasets](#datasets)
         - [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-tutorials)
           - [Run the Tutorials](#run-the-tutorials)
           - [Online Analysis](#online-analysis)
               - [Lattice Boltzmann Simulation](#lattice-boltzmann-simulation)
@@ -103,16 +105,16 @@
         
         The documentation has a number of tutorials that make it easy to get used to SmartSim locally
         before using it on your system. Each tutorial is a Jupyter notebook that can be run through the
         [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
         which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
         
         ```bash
-        docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.1
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
+        docker pull ghcr.io/craylabs/smartsim-tutorials:v0.4.2
+        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
         # click on link to open jupyter lab
         ```
         
         # SmartSim Infrastructure Library
         
         The Infrastructure Library (IL), the ``smartsim`` python package,
         facilitates the launch of Machine Learning and simulation
@@ -290,15 +292,14 @@
         initialization. Local launching does not support batch workloads.
         
         
         --------
         
         # Infrastructure Library Applications
          - Orchestrator - In-memory data store and Machine Learning Inference (Redis + RedisAI)
-         - Ray - Distributed Reinforcement Learning (RL), Hyperparameter Optimization (HPO)
         
         ## Redis + RedisAI
         
         The ``Orchestrator`` is an in-memory database that utilizes Redis and RedisAI to provide
         a distributed database and access to ML runtimes from Fortran, C, C++ and Python.
         
         SmartSim provides classes that make it simple to launch the database in many
@@ -404,61 +405,14 @@
         exp.stop(db_cluster)
         ```
         
         ```bash
         python run_db_batch.py
         ```
         
-        -----
-        ## Ray
-        
-        Ray is a distributed computation framework that supports a number of applications
-         - RLlib - Distributed Reinforcement Learning (RL)
-         - RaySGD - Distributed Training
-         - Ray Tune - Hyperparameter Optimization (HPO)
-         - Ray Serve - ML/DL inference
-        As well as other integrations with frameworks like Modin, Mars, Dask, and Spark.
-        
-        Historically, Ray has not been well supported on HPC systems. A few examples exist,
-        but none are well maintained. Because SmartSim already has launchers for HPC systems,
-        launching Ray through SmartSim is a relatively simple task.
-        
-        ### Ray on HPC
-        
-        Below is an example of how to launch a Ray cluster on an HPC system and connect to it.
-        In this example, we set `batch=True`, which means that the cluster will be started
-        requesting an allocation through the scheduler (Slurm, PBS, etc). If this code
-        is run within a sufficiently large interactive allocation, setting `batch=False`
-        will spin the Ray cluster on the allocated nodes.
-        
-        ```Python
-        import ray
-        
-        from smartsim import Experiment
-        from smartsim.exp.ray import RayCluster
-        
-        exp = Experiment("ray-cluster", launcher='auto')
-        # 3 workers + 1 head node = 4 node-cluster
-        cluster = RayCluster(name="ray-cluster", run_args={},
-                             ray_args={"num-cpus": 24},
-                             launcher='auto', num_nodes=4, batch=True)
-        
-        exp.generate(cluster, overwrite=True)
-        exp.start(cluster, block=False, summary=True)
-        
-        # Connect to the Ray cluster
-        ctx = ray.init(f"ray://{cluster.get_head_address()}:10001")
-        
-        # <run Ray tune, RLlib, HPO...>
-        ```
-        
-        *New in 0.4.0* the auto argument enables the Ray Cluster to be launched
-        across scheduler types. Both batch launch and interactive launch commands
-        will be automatically detected and used by SmartSim.
-        
         ------
         # SmartRedis
         
         The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/SmartRedis))
         are implementations of Redis clients that implement the RedisAI
         API with additions specific to scientific workflows.
         
@@ -504,15 +458,15 @@
         
         Each tutorial is a Jupyter notebook that can be run through the
         [SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim)
         which will run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
         
         ```bash
         docker pull ghcr.io/craylabs/smartsim-tutorials:v1
-        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1
+        docker run -p 8888:8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.2
         ```
         Each of the following examples can be found in the
         [SmartSim documentation](https://www.craylabs.org/docs/tutorials/getting_started/getting_started.html).
         
         ## Online Analysis
         
         Using SmartSim, HPC applications can be monitored in real time by streaming data
@@ -689,25 +643,25 @@
               <th style="text-align:center">RedisAI Version</th>
               <th style="text-align:center">Libraries</th>
               <th style="text-align:center">Supported Version</th>
             </tr>
           </thead>
           <tbody style="text-align:center">
             <tr>
-              <td rowspan="3">1.2.3-1.2.4</td>
+              <td rowspan="3">1.2.7</td>
               <td>PyTorch</td>
-              <td>1.7.x</td>
+              <td>1.11.x</td>
             </tr>
             <tr>
               <td>TensorFlow\Keras</td>
-              <td>2.4.x-2.5.x</td>
+              <td>2.8.x</td>
             </tr>
             <tr>
               <td>ONNX</td>
-              <td>1.9.x</td>
+              <td>1.11.x</td>
             </tr>
               <td rowspan="3">1.2.5</td>
               <td>PyTorch</td>
               <td>1.9.x</td>
             </tr>
             <tr>
               <td>TensorFlow\Keras</td>
@@ -820,18 +774,17 @@
             author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E. Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins},
             keywords = {Deep learning, Numerical simulation, Climate modeling, High performance computing, SmartSim},
         }
         ```
         
 Keywords: scientific,ai,workflow,hpc,analysis
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ml
-Provides-Extra: ray
```

#### html2text {}

```diff
@@ -1,83 +1,83 @@
-Metadata-Version: 2.1 Name: smartsim Version: 0.4.1 Summary: AI Workflows for
+Metadata-Version: 2.1 Name: smartsim Version: 0.4.2 Summary: AI Workflows for
 Science Home-page: https://github.com/CrayLabs/SmartSim Author: CrayLabs, a
 Hewlett Packard Enterprise OSS Organization Author-email: craylabs@hpe.com
 License: BSD 2-Clause License Project-URL: Source, https://github.com/CrayLabs/
 SmartSim Project-URL: Documentation, https://www.craylabs.org Description:
     [https://raw.githubusercontent.com/CrayLabs/SmartSim/master/doc/images/
                           SmartSim_Large.png][Image]
 
        Home    Install    Documentation    Slack_Invite    Cray_Labs   
 
 
 [![License](https://img.shields.io/github/license/CrayLabs/SmartSim)](https://
-github.com/CrayLabs/SmartSim/blob/master/LICENSE.md) ![GitHub last commit]
-(https://img.shields.io/github/last-commit/CrayLabs/SmartSim) ![GitHub
-deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/
-github-pages?label=doc%20build) ![PyPI - Wheel](https://img.shields.io/pypi/
-wheel/smartsim) ![PyPI - Python Version](https://img.shields.io/pypi/
-pyversions/smartsim) ![GitHub tag (latest by date)](https://img.shields.io/
-github/v/tag/CrayLabs/SmartSim) ![Language](https://img.shields.io/github/
+  github.com/CrayLabs/SmartSim/blob/master/LICENSE.md) ![GitHub last commit]
+    (https://img.shields.io/github/last-commit/CrayLabs/SmartSim) ![GitHub
+   deployments](https://img.shields.io/github/deployments/CrayLabs/SmartSim/
+ github-pages?label=doc%20build) ![PyPI - Wheel](https://img.shields.io/pypi/
+     wheel/smartsim) ![PyPI - Python Version](https://img.shields.io/pypi/
+  pyversions/smartsim) ![GitHub tag (latest by date)](https://img.shields.io/
+  github/v/tag/CrayLabs/SmartSim) ![Language](https://img.shields.io/github/
 languages/top/CrayLabs/SmartSim) [![Code style: black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![codecov]
-(https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/
-badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim) [!
-[Downloads](https://static.pepy.tech/personalized-badge/
+        (https://codecov.io/gh/CrayLabs/SmartSim/branch/develop/graph/
+   badge.svg?token=96HFI2F45E)](https://codecov.io/gh/CrayLabs/SmartSim) [!
+           [Downloads](https://static.pepy.tech/personalized-badge/
 smartsim?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)]
-(https://pepy.tech/project/smartsim) ------------ # SmartSim SmartSim is made
-up of two parts 1. SmartSim Infrastructure Library (This repository) 2.
-[SmartRedis](https://github.com/CrayLabs/SmartRedis) The two library components
-are designed to work together, but can also be used independently. *SmartSim*
-is a workflow library that makes it easier to use common Machine Learning (ML)
-libraries, like PyTorch and TensorFlow, in High Performance Computing (HPC)
-simulations and applications. SmartSim launches ML infrastructure on HPC
-systems alongside user workloads. *SmartRedis* provides an API to connect HPC
-workloads, particularly (MPI + X) simulations, to the ML infrastructure, namely
-the The [Orchestrator database](https://www.craylabs.org/docs/
-orchestrator.html), launched by SmartSim. Applications integrated with the
-SmartRedis clients, written in Fortran, C, C++ and Python, can send data to and
-remotely request SmartSim infrastructure to execute ML models and scripts on
-GPU or CPU. The distributed Client-Server paradigm allows for data to be
-seamlessly exchanged between applications at runtime without the utilization of
-MPI. ---------- **Table of Contents** - [SmartSim](#smartsim) - [Quick Start]
-(#quick-start) - [SmartSim Infrastructure Library](#smartsim-infrastructure-
-library) - [Experiments](#experiments) - [Hello World](#hello-world) - [Hello
-World MPI](#hello-world-mpi) - [Experiments on HPC Systems](#experiments-on-
-hpc-systems) - [Interactive Launch Example](#interactive-launch-example) -
-[Batch Launch Examples](#batch-launch-examples) - [Infrastructure Library
-Applications](#infrastructure-library-applications) - [Redis + RedisAI](#redis-
--redisai) - [Local Launch](#local-launch) - [Interactive Launch](#interactive-
-launch) - [Batch Launch](#batch-launch) - [Ray](#ray) - [Ray on HPC](#ray-on-
-hpc) - [SmartRedis](#smartredis) - [Tensors](#tensors) - [Datasets](#datasets)
-- [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-tutorials) - [Run the
-Tutorials](#run-the-tutorials) - [Online Analysis](#online-analysis) - [Lattice
-Boltzmann Simulation](#lattice-boltzmann-simulation) - [Online Processing]
-(#online-processing) - [Singular Value Decomposition](#singular-value-
-decomposition) - [Online Inference](#online-inference) - [PyTorch CNN Example]
-(#pytorch-cnn-example) - [Publications](#publications) - [Cite](#cite) -
-[bibtex](#bibtex) ---- # Quick Start The documentation has a number of
-tutorials that make it easy to get used to SmartSim locally before using it on
-your system. Each tutorial is a Jupyter notebook that can be run through the
-[SmartSim Tutorials docker image](https://github.com/orgs/CrayLabs/
-packages?repo_name=SmartSim) which will run a jupyter lab with the tutorials,
-SmartSim, and SmartRedis installed. ```bash docker pull ghcr.io/craylabs/
-smartsim-tutorials:v0.4.1 docker run -p 8888:8888 ghcr.io/craylabs/smartsim-
-tutorials:v0.4.1 # click on link to open jupyter lab ``` # SmartSim
-Infrastructure Library The Infrastructure Library (IL), the ``smartsim`` python
-package, facilitates the launch of Machine Learning and simulation workflows.
-The Python interface of the IL creates, configures, launches and monitors
-applications. ## Experiments The [Experiment](https://www.craylabs.org/docs/
-api/smartsim_api.html#experiment) object is the main interface of SmartSim.
-Through the [Experiment](https://www.craylabs.org/docs/api/
-smartsim_api.html#experiment) users can create references to user applications
-called ``Models``. ### Hello World Below is a simple example of a workflow that
-uses the IL to launch hello world program using the local launcher which is
-designed for laptops and single nodes. ```python from smartsim import
-Experiment exp = Experiment("simple", launcher="local") settings =
-exp.create_run_settings("echo", exe_args="Hello World") model =
+                     (https://pepy.tech/project/smartsim)
+------------ # SmartSim SmartSim is made up of two parts 1. SmartSim
+Infrastructure Library (This repository) 2. [SmartRedis](https://github.com/
+CrayLabs/SmartRedis) The two library components are designed to work together,
+but can also be used independently. *SmartSim* is a workflow library that makes
+it easier to use common Machine Learning (ML) libraries, like PyTorch and
+TensorFlow, in High Performance Computing (HPC) simulations and applications.
+SmartSim launches ML infrastructure on HPC systems alongside user workloads.
+*SmartRedis* provides an API to connect HPC workloads, particularly (MPI + X)
+simulations, to the ML infrastructure, namely the The [Orchestrator database]
+(https://www.craylabs.org/docs/orchestrator.html), launched by SmartSim.
+Applications integrated with the SmartRedis clients, written in Fortran, C, C++
+and Python, can send data to and remotely request SmartSim infrastructure to
+execute ML models and scripts on GPU or CPU. The distributed Client-Server
+paradigm allows for data to be seamlessly exchanged between applications at
+runtime without the utilization of MPI. ---------- **Table of Contents** -
+[SmartSim](#smartsim) - [Quick Start](#quick-start) - [SmartSim Infrastructure
+Library](#smartsim-infrastructure-library) - [Experiments](#experiments) -
+[Hello World](#hello-world) - [Hello World MPI](#hello-world-mpi) -
+[Experiments on HPC Systems](#experiments-on-hpc-systems) - [Interactive Launch
+Example](#interactive-launch-example) - [Batch Launch Examples](#batch-launch-
+examples) - [Infrastructure Library Applications](#infrastructure-library-
+applications) - [Redis + RedisAI](#redis--redisai) - [Local Launch](#local-
+launch) - [Interactive Launch](#interactive-launch) - [Batch Launch](#batch-
+launch) - [SmartRedis](#smartredis) - [Tensors](#tensors) - [Datasets]
+(#datasets) - [SmartSim + SmartRedis Tutorials](#smartsim--smartredis-
+tutorials) - [Run the Tutorials](#run-the-tutorials) - [Online Analysis]
+(#online-analysis) - [Lattice Boltzmann Simulation](#lattice-boltzmann-
+simulation) - [Online Processing](#online-processing) - [Singular Value
+Decomposition](#singular-value-decomposition) - [Online Inference](#online-
+inference) - [PyTorch CNN Example](#pytorch-cnn-example) - [Publications]
+(#publications) - [Cite](#cite) - [bibtex](#bibtex) ---- # Quick Start The
+documentation has a number of tutorials that make it easy to get used to
+SmartSim locally before using it on your system. Each tutorial is a Jupyter
+notebook that can be run through the [SmartSim Tutorials docker image](https://
+github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
+lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
+ghcr.io/craylabs/smartsim-tutorials:v0.4.2 docker run -p 8888:8888 ghcr.io/
+craylabs/smartsim-tutorials:v0.4.2 # click on link to open jupyter lab ``` #
+SmartSim Infrastructure Library The Infrastructure Library (IL), the
+``smartsim`` python package, facilitates the launch of Machine Learning and
+simulation workflows. The Python interface of the IL creates, configures,
+launches and monitors applications. ## Experiments The [Experiment](https://
+www.craylabs.org/docs/api/smartsim_api.html#experiment) object is the main
+interface of SmartSim. Through the [Experiment](https://www.craylabs.org/docs/
+api/smartsim_api.html#experiment) users can create references to user
+applications called ``Models``. ### Hello World Below is a simple example of a
+workflow that uses the IL to launch hello world program using the local
+launcher which is designed for laptops and single nodes. ```python from
+smartsim import Experiment exp = Experiment("simple", launcher="local")
+settings = exp.create_run_settings("echo", exe_args="Hello World") model =
 exp.create_model("hello_world", settings) exp.start(model, block=True) print
 (exp.get_status(model)) ``` ### Hello World MPI The
 [Experiment.create_run_settings](https://www.craylabs.org/docs/api/
 smartsim_api.html#smartsim.experiment.Experiment.create_run_settings) method
 returns a ``RunSettings`` object which defines how a model is launched. There
 are many types of ``RunSettings`` [supported by SmartSim](https://
 www.craylabs.org/docs/api/smartsim_api.html#settings). - ``RunSettings`` -
@@ -128,23 +128,22 @@
 replicas=4) exp.start(ensemble, block=True, summary=True) print(exp.get_status
 (ensemble)) ``` ```bash python hello_ensemble.py ``` Similar to the interactive
 example, this same script will run on a SLURM, PBS, LSF, or Cobalt system as
 the ``launcher`` is set to `auto` in the [Experiment](https://www.craylabs.org/
 docs/api/smartsim_api.html#experiment) initialization. Local launching does not
 support batch workloads. -------- # Infrastructure Library Applications -
 Orchestrator - In-memory data store and Machine Learning Inference (Redis +
-RedisAI) - Ray - Distributed Reinforcement Learning (RL), Hyperparameter
-Optimization (HPO) ## Redis + RedisAI The ``Orchestrator`` is an in-memory
-database that utilizes Redis and RedisAI to provide a distributed database and
-access to ML runtimes from Fortran, C, C++ and Python. SmartSim provides
-classes that make it simple to launch the database in many configurations and
-optionally form a distributed database cluster. The examples below will show
-how to launch the database. Later in this document we will show how to use the
-database to perform ML inference and processing. ### Local Launch The following
-script launches a single database using the local launcher.
+RedisAI) ## Redis + RedisAI The ``Orchestrator`` is an in-memory database that
+utilizes Redis and RedisAI to provide a distributed database and access to ML
+runtimes from Fortran, C, C++ and Python. SmartSim provides classes that make
+it simple to launch the database in many configurations and optionally form a
+distributed database cluster. The examples below will show how to launch the
+database. Later in this document we will show how to use the database to
+perform ML inference and processing. ### Local Launch The following script
+launches a single database using the local launcher.
 [Experiment.create_database](https://www.craylabs.org/docs/api/
 smartsim_api.html#smartsim.experiment.Experiment.create_database) will
 initialize an ``Orchestrator`` instance corresponding to the specified
 launcher. ```python # run_db_local.py from smartsim import Experiment exp =
 Experiment("local-db", launcher="local") db = exp.create_database(port=6780, #
 database port interface="lo") # network interface to use # by default, SmartSim
 never blocks execution after the database is launched. exp.start(db) # launch
@@ -170,81 +169,59 @@
 Users can hit CTRL-C to cancel the launch if needed. ```Python #
 run_db_batch.py from smartsim import Experiment exp = Experiment("batch-db-on-
 pbs", launcher="auto") db_cluster = exp.create_database(db_nodes=3,
 db_port=6780, batch=True, time="00:10:00", interface="ib0", account="12345-
 Cray", queue="cl40") exp.start(db_cluster) print(f"Orchestrator launched on
 nodes: {db_cluster.hosts}") # launch models, analysis, training, inference
 sessions, etc # that communicate with the database using the SmartRedis clients
-exp.stop(db_cluster) ``` ```bash python run_db_batch.py ``` ----- ## Ray Ray is
-a distributed computation framework that supports a number of applications -
-RLlib - Distributed Reinforcement Learning (RL) - RaySGD - Distributed Training
-- Ray Tune - Hyperparameter Optimization (HPO) - Ray Serve - ML/DL inference As
-well as other integrations with frameworks like Modin, Mars, Dask, and Spark.
-Historically, Ray has not been well supported on HPC systems. A few examples
-exist, but none are well maintained. Because SmartSim already has launchers for
-HPC systems, launching Ray through SmartSim is a relatively simple task. ###
-Ray on HPC Below is an example of how to launch a Ray cluster on an HPC system
-and connect to it. In this example, we set `batch=True`, which means that the
-cluster will be started requesting an allocation through the scheduler (Slurm,
-PBS, etc). If this code is run within a sufficiently large interactive
-allocation, setting `batch=False` will spin the Ray cluster on the allocated
-nodes. ```Python import ray from smartsim import Experiment from
-smartsim.exp.ray import RayCluster exp = Experiment("ray-cluster",
-launcher='auto') # 3 workers + 1 head node = 4 node-cluster cluster =
-RayCluster(name="ray-cluster", run_args={}, ray_args={"num-cpus": 24},
-launcher='auto', num_nodes=4, batch=True) exp.generate(cluster, overwrite=True)
-exp.start(cluster, block=False, summary=True) # Connect to the Ray cluster ctx
-= ray.init(f"ray://{cluster.get_head_address()}:10001") #
- RLlib, HPO...> ``` *New in 0.4.0* the auto argument enables the Ray Cluster to
-be launched across scheduler types. Both batch launch and interactive launch
-commands will be automatically detected and used by SmartSim. ------ #
-SmartRedis The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/
-SmartRedis)) are implementations of Redis clients that implement the RedisAI
-API with additions specific to scientific workflows. SmartRedis clients are
-available in Fortran, C, C++, and Python. Users can seamlessly pull and push
-data from the Orchestrator from different languages. ## Tensors Tensors are the
-fundamental data structure for the SmartRedis clients. The Clients use the
-native array format of the language. For example, in Python, a tensor is a
-NumPy array while the C/C++ clients accept nested and contiguous arrays. When
-stored in the database, all tensors are stored in the same format. Hence, any
-language can receive a tensor from the database no matter what supported
-language the array was sent from. This enables applications in different
-languages to communicate numerical data with each other at runtime. For more
-information on the tensor data structure, see [the documentation](https://
-www.craylabs.org/docs/sr_data_structures.html#tensor) ## Datasets Datasets are
-collections of Tensors and associated metadata. The ``Dataset`` class is a user
-space object that can be created, added to, sent to, and retrieved from the
-Orchestrator. For an example of how to use the ``Dataset`` class, see the
-[Online Analysis example](#online-analysis) For more information on the API,
-see the [API documentation](https://www.craylabs.org/docs/
-sr_data_structures.html#dataset) # SmartSim + SmartRedis Tutorials SmartSim and
-SmartRedis were designed to work together. When launched through SmartSim,
-applications using the SmartRedis clients are directly connected to any
-Orchestrator launched in the same [Experiment](https://www.craylabs.org/docs/
-api/smartsim_api.html#experiment). In this way, a SmartSim [Experiment](https:/
-/www.craylabs.org/docs/api/smartsim_api.html#experiment) becomes a driver for
-coupled ML and Simulation workflows. The following are simple examples of how
-to use SmartSim and SmartRedis together. ## Run the Tutorials Each tutorial is
-a Jupyter notebook that can be run through the [SmartSim Tutorials docker
-image](https://github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will
-run a jupyter lab with the tutorials, SmartSim, and SmartRedis installed.
-```bash docker pull ghcr.io/craylabs/smartsim-tutorials:v1 docker run -p 8888:
-8888 ghcr.io/craylabs/smartsim-tutorials:v0.4.1 ``` Each of the following
-examples can be found in the [SmartSim documentation](https://www.craylabs.org/
-docs/tutorials/getting_started/getting_started.html). ## Online Analysis Using
-SmartSim, HPC applications can be monitored in real time by streaming data from
-the application to the database. SmartRedis clients can retrieve the data,
-process, analyze it, and finally store any updated data back to the database
-for use by other clients. The following is an example of how a user could
-monitor and analyze a simulation. The example here uses the Python client;
-however, SmartRedis clients are also available for C, C++, and Fortran. All
-SmartRedis clients implement the same API. The example will produce [this
-visualization](https://user-images.githubusercontent.com/13009163/127622717-
-2c9e4cfd-50f4-4d94-88c4-8c05fa2fa616.mp4) while the simulation is running. ####
-Lattice Boltzmann Simulation Using a [Lattice Boltzmann Simulation](https://
+exp.stop(db_cluster) ``` ```bash python run_db_batch.py ``` ------ # SmartRedis
+The SmartSim IL Clients ([SmartRedis](https://github.com/CrayLabs/SmartRedis))
+are implementations of Redis clients that implement the RedisAI API with
+additions specific to scientific workflows. SmartRedis clients are available in
+Fortran, C, C++, and Python. Users can seamlessly pull and push data from the
+Orchestrator from different languages. ## Tensors Tensors are the fundamental
+data structure for the SmartRedis clients. The Clients use the native array
+format of the language. For example, in Python, a tensor is a NumPy array while
+the C/C++ clients accept nested and contiguous arrays. When stored in the
+database, all tensors are stored in the same format. Hence, any language can
+receive a tensor from the database no matter what supported language the array
+was sent from. This enables applications in different languages to communicate
+numerical data with each other at runtime. For more information on the tensor
+data structure, see [the documentation](https://www.craylabs.org/docs/
+sr_data_structures.html#tensor) ## Datasets Datasets are collections of Tensors
+and associated metadata. The ``Dataset`` class is a user space object that can
+be created, added to, sent to, and retrieved from the Orchestrator. For an
+example of how to use the ``Dataset`` class, see the [Online Analysis example]
+(#online-analysis) For more information on the API, see the [API documentation]
+(https://www.craylabs.org/docs/sr_data_structures.html#dataset) # SmartSim +
+SmartRedis Tutorials SmartSim and SmartRedis were designed to work together.
+When launched through SmartSim, applications using the SmartRedis clients are
+directly connected to any Orchestrator launched in the same [Experiment](https:
+//www.craylabs.org/docs/api/smartsim_api.html#experiment). In this way, a
+SmartSim [Experiment](https://www.craylabs.org/docs/api/
+smartsim_api.html#experiment) becomes a driver for coupled ML and Simulation
+workflows. The following are simple examples of how to use SmartSim and
+SmartRedis together. ## Run the Tutorials Each tutorial is a Jupyter notebook
+that can be run through the [SmartSim Tutorials docker image](https://
+github.com/orgs/CrayLabs/packages?repo_name=SmartSim) which will run a jupyter
+lab with the tutorials, SmartSim, and SmartRedis installed. ```bash docker pull
+ghcr.io/craylabs/smartsim-tutorials:v1 docker run -p 8888:8888 ghcr.io/
+craylabs/smartsim-tutorials:v0.4.2 ``` Each of the following examples can be
+found in the [SmartSim documentation](https://www.craylabs.org/docs/tutorials/
+getting_started/getting_started.html). ## Online Analysis Using SmartSim, HPC
+applications can be monitored in real time by streaming data from the
+application to the database. SmartRedis clients can retrieve the data, process,
+analyze it, and finally store any updated data back to the database for use by
+other clients. The following is an example of how a user could monitor and
+analyze a simulation. The example here uses the Python client; however,
+SmartRedis clients are also available for C, C++, and Fortran. All SmartRedis
+clients implement the same API. The example will produce [this visualization]
+(https://user-images.githubusercontent.com/13009163/127622717-2c9e4cfd-50f4-
+4d94-88c4-8c05fa2fa616.mp4) while the simulation is running. #### Lattice
+Boltzmann Simulation Using a [Lattice Boltzmann Simulation](https://
 en.wikipedia.org/wiki/Lattice_Boltzmann_methods), this example demonstrates how
 to use the SmartRedis ``Dataset`` API to stream data over the Orchestrator
 deployed by SmartSim. The simulation will be composed of two parts: `fv_sim.py`
 which will generate data from the Simulation and store it in the Orchestrator,
 and `driver.py` which will launch the Orchestrator, start `fv_sim.py` and check
 for data posted to the Orchestrator to plot updates in real-time. The following
 code highlights the sections of `fv_sim.py` that are responsible for
@@ -305,17 +282,17 @@
 computational pipelines of functions, scripts, and models. See the full
 [TorchScript Language Reference](https://pytorch.org/docs/stable/
 jit.html#torchscript-language) documentation for more information on available
 methods, functions, and how to create your own. ## Online Inference SmartSim
 supports the following frameworks for querying Machine Learning models from C,
 C++, Fortran and Python with the SmartRedis Clients:
 RedisAI Version  Libraries        Supported Version
-                 PyTorch          1.7.x
-1.2.3-1.2.4      TensorFlow\Keras 2.4.x-2.5.x
-                 ONNX             1.9.x
+                 PyTorch          1.11.x
+1.2.7            TensorFlow\Keras 2.8.x
+                 ONNX             1.11.x
 TensorFlow\Keras 2.6.x
 ONNX             1.9.x
 A [number of other libraries](https://github.com/onnx/onnxmltools) are
 supported through ONNX, like [SciKit-Learn](https://github.com/onnx/sklearn-
 onnx/) and [XGBoost](https://github.com/onnx/onnxmltools/tree/master/tests/
 xgboost). **Note:** It's important to remember that SmartSim utilizes a client-
 server model. To run experiments that utilize the above frameworks, you must
@@ -357,13 +334,13 @@
 {Journal of Computational Science}, volume = {62}, pages = {101707}, year =
 {2022}, issn = {1877-7503}, doi = {https://doi.org/10.1016/j.jocs.2022.101707},
 url = {https://www.sciencedirect.com/science/article/pii/S1877750322001065},
 author = {Sam Partee and Matthew Ellis and Alessandro Rigazzi and Andrew E.
 Shao and Scott Bachman and Gustavo Marques and Benjamin Robbins}, keywords =
 {Deep learning, Numerical simulation, Climate modeling, High performance
 computing, SmartSim}, } ``` Keywords: scientific,ai,workflow,hpc,analysis
-Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: License :: OSI Approved :: BSD License Classifier:
+Platform: UNKNOWN Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: License :: OSI Approved :: BSD License Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
-Engineering Requires-Python: >=3.7 Description-Content-Type: text/markdown
-Provides-Extra: dev Provides-Extra: ml Provides-Extra: ray
+Engineering Requires-Python: <3.11,>=3.8 Description-Content-Type: text/
+markdown Provides-Extra: dev Provides-Extra: ml
```

### Comparing `smartsim-0.4.1/smartsim.egg-info/SOURCES.txt` & `smartsim-0.4.2/smartsim.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 smartsim/_core/control/__init__.py
 smartsim/_core/control/controller.py
 smartsim/_core/control/job.py
 smartsim/_core/control/jobmanager.py
 smartsim/_core/control/manifest.py
 smartsim/_core/entrypoints/__init__.py
 smartsim/_core/entrypoints/colocated.py
-smartsim/_core/entrypoints/ray.py
 smartsim/_core/entrypoints/redis.py
 smartsim/_core/generation/__init__.py
 smartsim/_core/generation/generator.py
 smartsim/_core/generation/modelwriter.py
 smartsim/_core/launcher/__init__.py
 smartsim/_core/launcher/colocated.py
 smartsim/_core/launcher/launcher.py
@@ -73,15 +72,15 @@
 smartsim/_core/launcher/slurm/slurmLauncher.py
 smartsim/_core/launcher/slurm/slurmParser.py
 smartsim/_core/launcher/step/__init__.py
 smartsim/_core/launcher/step/alpsStep.py
 smartsim/_core/launcher/step/cobaltStep.py
 smartsim/_core/launcher/step/localStep.py
 smartsim/_core/launcher/step/lsfStep.py
-smartsim/_core/launcher/step/mpirunStep.py
+smartsim/_core/launcher/step/mpiStep.py
 smartsim/_core/launcher/step/pbsStep.py
 smartsim/_core/launcher/step/slurmStep.py
 smartsim/_core/launcher/step/step.py
 smartsim/_core/launcher/util/__init__.py
 smartsim/_core/launcher/util/launcherUtil.py
 smartsim/_core/launcher/util/shell.py
 smartsim/_core/utils/__init__.py
@@ -97,30 +96,30 @@
 smartsim/entity/entity.py
 smartsim/entity/entityList.py
 smartsim/entity/files.py
 smartsim/entity/model.py
 smartsim/entity/strategies.py
 smartsim/error/__init__.py
 smartsim/error/errors.py
-smartsim/exp/ray/__init__.py
-smartsim/exp/ray/raycluster.py
 smartsim/ml/__init__.py
 smartsim/ml/data.py
 smartsim/ml/tf/__init__.py
 smartsim/ml/tf/data.py
 smartsim/ml/tf/utils.py
 smartsim/ml/torch/__init__.py
 smartsim/ml/torch/data.py
 smartsim/settings/__init__.py
 smartsim/settings/alpsSettings.py
 smartsim/settings/base.py
 smartsim/settings/cobaltSettings.py
 smartsim/settings/containers.py
 smartsim/settings/lsfSettings.py
+smartsim/settings/mpiSettings.py
 smartsim/settings/mpirunSettings.py
+smartsim/settings/palsSettings.py
 smartsim/settings/pbsSettings.py
 smartsim/settings/settings.py
 smartsim/settings/slurmSettings.py
 smartsim/tf/__init__.py
 smartsim/tf/utils.py
 smartsim/wlm/__init__.py
 smartsim/wlm/pbs.py
```

