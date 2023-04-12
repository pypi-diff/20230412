# Comparing `tmp/pontos-23.4.1.tar.gz` & `tmp/pontos-23.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.4.1.tar", max compression
+gzip compressed data, was "pontos-23.4.2.tar", max compression
```

## Comparing `pontos-23.4.1.tar` & `pontos-23.4.2.tar`

### file list

```diff
@@ -1,248 +1,248 @@
--rw-r--r--   0        0        0    35149 2023-04-06 10:54:40.732158 pontos-23.4.1/LICENSE
--rw-r--r--   0        0        0     3349 2023-04-06 10:54:40.732158 pontos-23.4.1/README.md
--rw-r--r--   0        0        0    97720 2023-04-06 10:54:40.736158 pontos-23.4.1/poetry.lock
--rw-r--r--   0        0        0       32 2023-04-06 10:54:40.736158 pontos-23.4.1/poetry.toml
--rw-r--r--   0        0        0      791 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4427 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/git/__init__.py
--rw-r--r--   0        0        0    16117 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     6158 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-04-06 10:54:40.736158 pontos-23.4.1/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    10519 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/api/search.py
--rw-r--r--   0        0        0     5079 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7508 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/models/organization.py
--rw-r--r--   0        0        0    12937 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/models/search.py
--rw-r--r--   0        0        0     3922 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3400 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/release/main.py
--rw-r--r--   0        0        0     7440 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/release/parser.py
--rw-r--r--   0        0        0    12114 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/release/release.py
--rw-r--r--   0        0        0    12039 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-04-06 10:54:40.740158 pontos-23.4.1/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      749 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0      757 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0      737 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0      753 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0      757 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0      757 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      871 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0      737 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0      737 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      747 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0      709 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      741 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      741 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0      733 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0      733 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      793 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0      802 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0      781 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0      802 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0      802 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      915 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0      781 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0      781 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0      791 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0      751 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      783 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      783 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      727 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0      735 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0      715 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0      731 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0      735 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0      735 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      849 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0      715 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0      715 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      725 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0      687 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      720 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      720 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12050 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1416 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     7752 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6263 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     7786 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/errors.py
--rw-r--r--   0        0        0     2018 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13117 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2145 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    14501 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5241 2023-04-06 10:54:40.744158 pontos-23.4.1/pontos/version/version.py
--rw-r--r--   0        0        0     2890 2023-04-06 10:54:40.744158 pontos-23.4.1/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-04-06 10:54:40.744158 pontos-23.4.1/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-04-06 10:54:40.744158 pontos-23.4.1/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-04-06 10:54:40.744158 pontos-23.4.1/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-04-06 10:54:40.744158 pontos-23.4.1/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17750 2023-04-06 10:54:40.744158 pontos-23.4.1/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-04-06 10:54:40.744158 pontos-23.4.1/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/git/__init__.py
--rw-r--r--   0        0        0    27772 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     4385 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    52500 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_search.py
--rw-r--r--   0        0        0     7383 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-04-06 10:54:40.748158 pontos-23.4.1/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    76541 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6098 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/release/__init__.py
--rw-r--r--   0        0        0     3190 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/release/test_helper.py
--rw-r--r--   0        0        0     8223 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/release/test_parser.py
--rw-r--r--   0        0        0    59154 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/release/test_release.py
--rw-r--r--   0        0        0    21452 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/test_helper.py
--rw-r--r--   0        0        0     1373 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15227 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/commands/__init__.py
--rw-r--r--   0        0        0    11322 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    15371 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    22817 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    25027 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/test_errors.py
--rw-r--r--   0        0        0     3385 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-04-06 10:54:40.752158 pontos-23.4.1/tests/version/test_version.py
--rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 pontos-23.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-12 07:27:28.477329 pontos-23.4.2/LICENSE
+-rw-r--r--   0        0        0     3349 2023-04-12 07:27:28.477329 pontos-23.4.2/README.md
+-rw-r--r--   0        0        0    97724 2023-04-12 07:27:28.481329 pontos-23.4.2/poetry.lock
+-rw-r--r--   0        0        0       32 2023-04-12 07:27:28.481329 pontos-23.4.2/poetry.toml
+-rw-r--r--   0        0        0      791 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9914 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4427 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16117 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     6158 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    10519 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7508 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    12937 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-04-12 07:27:28.481329 pontos-23.4.2/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3400 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/main.py
+-rw-r--r--   0        0        0     7491 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/parser.py
+-rw-r--r--   0        0        0    12426 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/release.py
+-rw-r--r--   0        0        0    12039 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      749 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0      757 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0      737 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0      753 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0      757 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0      757 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      871 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0      737 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0      737 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      747 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0      709 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      741 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      741 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0      733 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0      733 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      793 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0      802 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0      781 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0      802 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0      802 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      915 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0      781 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0      781 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0      791 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0      751 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      783 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      783 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      727 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0      735 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0      715 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0      731 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0      735 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0      735 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      849 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0      715 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0      715 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      725 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0      687 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      720 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      720 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12050 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1416 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     7752 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6263 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     7786 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/errors.py
+-rw-r--r--   0        0        0     2018 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13117 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2145 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    14501 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5241 2023-04-12 07:27:28.485329 pontos-23.4.2/pontos/version/version.py
+-rw-r--r--   0        0        0     2890 2023-04-12 07:27:28.485329 pontos-23.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-04-12 07:27:28.485329 pontos-23.4.2/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17750 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/git/__init__.py
+-rw-r--r--   0        0        0    27772 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     4385 2023-04-12 07:27:28.485329 pontos-23.4.2/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    52500 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    76541 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6098 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/__init__.py
+-rw-r--r--   0        0        0     3190 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/test_helper.py
+-rw-r--r--   0        0        0     8223 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/test_parser.py
+-rw-r--r--   0        0        0    59154 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/test_release.py
+-rw-r--r--   0        0        0    21452 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-04-12 07:27:28.489329 pontos-23.4.2/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/test_helper.py
+-rw-r--r--   0        0        0     1373 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15227 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0    11322 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    15371 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    22817 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    25027 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_errors.py
+-rw-r--r--   0        0        0     3385 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-04-12 07:27:28.493329 pontos-23.4.2/tests/version/test_version.py
+-rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 pontos-23.4.2/PKG-INFO
```

### Comparing `pontos-23.4.1/LICENSE` & `pontos-23.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/README.md` & `pontos-23.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/poetry.lock` & `pontos-23.4.2/poetry.lock`

 * *Files 2% similar despite different names*

```diff
@@ -31,42 +31,42 @@
 [package.extras]
 doc = ["packaging", "sphinx-autodoc-typehints (>=1.2.0)", "sphinx-rtd-theme"]
 test = ["contextlib2", "coverage[toml] (>=4.5)", "hypothesis (>=4.0)", "mock (>=4)", "pytest (>=7.0)", "pytest-mock (>=3.6.1)", "trustme", "uvloop (<0.15)", "uvloop (>=0.15)"]
 trio = ["trio (>=0.16,<0.22)"]
 
 [[package]]
 name = "astroid"
-version = "2.15.1"
+version = "2.15.2"
 description = "An abstract syntax tree for Python with inference support."
 category = "dev"
 optional = false
 python-versions = ">=3.7.2"
 files = [
-    {file = "astroid-2.15.1-py3-none-any.whl", hash = "sha256:89860bda98fe2bbd1f5d262229be7629d778ce280de68d95d4a73d1f592ad268"},
-    {file = "astroid-2.15.1.tar.gz", hash = "sha256:af4e0aff46e2868218502789898269ed95b663fba49e65d91c1e09c966266c34"},
+    {file = "astroid-2.15.2-py3-none-any.whl", hash = "sha256:dea89d9f99f491c66ac9c04ebddf91e4acf8bd711722175fe6245c0725cc19bb"},
+    {file = "astroid-2.15.2.tar.gz", hash = "sha256:6e61b85c891ec53b07471aec5878f4ac6446a41e590ede0f2ce095f39f7d49dd"},
 ]
 
 [package.dependencies]
 lazy-object-proxy = ">=1.4.0"
 typing-extensions = {version = ">=4.0.0", markers = "python_version < \"3.11\""}
 wrapt = [
     {version = ">=1.11,<2", markers = "python_version < \"3.11\""},
     {version = ">=1.14,<2", markers = "python_version >= \"3.11\""},
 ]
 
 [[package]]
 name = "autohooks"
-version = "23.1.0"
+version = "23.4.0"
 description = "Library for managing git hooks"
 category = "dev"
 optional = false
-python-versions = ">=3.7,<4.0"
+python-versions = ">=3.7.2,<4.0.0"
 files = [
-    {file = "autohooks-23.1.0-py3-none-any.whl", hash = "sha256:bff89af36bc2a442a4d6198b7dbf4c6cc204b1b35c4a8d51e3c30e6bd12224bd"},
-    {file = "autohooks-23.1.0.tar.gz", hash = "sha256:bf9da5e9155676edde49c795b7ad4bf3b4322da3ee9c9358811a2b497eb811c7"},
+    {file = "autohooks-23.4.0-py3-none-any.whl", hash = "sha256:2c3b8506890565ad8c9b690db9b70a9b65068ff9f1c2a2d601d2914ad576cfff"},
+    {file = "autohooks-23.4.0.tar.gz", hash = "sha256:6880ad263f0aaab607bbfc1d42afc407de6234320fcff10d75d4e89f4e711ccd"},
 ]
 
 [package.dependencies]
 pontos = ">=22.8.0"
 rich = ">=12.5.1"
 tomlkit = ">=0.5.11"
 
@@ -130,22 +130,22 @@
 files = [
     {file = "Babel-2.12.1-py3-none-any.whl", hash = "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610"},
     {file = "Babel-2.12.1.tar.gz", hash = "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"},
 ]
 
 [[package]]
 name = "beautifulsoup4"
-version = "4.12.0"
+version = "4.12.2"
 description = "Screen-scraping library"
 category = "dev"
 optional = false
 python-versions = ">=3.6.0"
 files = [
-    {file = "beautifulsoup4-4.12.0-py3-none-any.whl", hash = "sha256:2130a5ad7f513200fae61a17abb5e338ca980fa28c439c0571014bc0217e9591"},
-    {file = "beautifulsoup4-4.12.0.tar.gz", hash = "sha256:c5fceeaec29d09c84970e47c65f2f0efe57872f7cff494c9691a26ec0ff13234"},
+    {file = "beautifulsoup4-4.12.2-py3-none-any.whl", hash = "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"},
+    {file = "beautifulsoup4-4.12.2.tar.gz", hash = "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da"},
 ]
 
 [package.dependencies]
 soupsieve = ">1.2"
 
 [package.extras]
 html5lib = ["html5lib"]
@@ -338,71 +338,71 @@
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
 
 [[package]]
 name = "coverage"
-version = "7.2.2"
+version = "7.2.3"
 description = "Code coverage measurement for Python"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "coverage-7.2.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7"},
-    {file = "coverage-7.2.2-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d"},
-    {file = "coverage-7.2.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5"},
-    {file = "coverage-7.2.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"},
-    {file = "coverage-7.2.2-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6"},
-    {file = "coverage-7.2.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137"},
-    {file = "coverage-7.2.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90"},
-    {file = "coverage-7.2.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2"},
-    {file = "coverage-7.2.2-cp310-cp310-win32.whl", hash = "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292"},
-    {file = "coverage-7.2.2-cp310-cp310-win_amd64.whl", hash = "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab"},
-    {file = "coverage-7.2.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b"},
-    {file = "coverage-7.2.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5"},
-    {file = "coverage-7.2.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731"},
-    {file = "coverage-7.2.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd"},
-    {file = "coverage-7.2.2-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d"},
-    {file = "coverage-7.2.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212"},
-    {file = "coverage-7.2.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54"},
-    {file = "coverage-7.2.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57"},
-    {file = "coverage-7.2.2-cp311-cp311-win32.whl", hash = "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d"},
-    {file = "coverage-7.2.2-cp311-cp311-win_amd64.whl", hash = "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512"},
-    {file = "coverage-7.2.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9"},
-    {file = "coverage-7.2.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e"},
-    {file = "coverage-7.2.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69"},
-    {file = "coverage-7.2.2-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0"},
-    {file = "coverage-7.2.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f"},
-    {file = "coverage-7.2.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67"},
-    {file = "coverage-7.2.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9"},
-    {file = "coverage-7.2.2-cp37-cp37m-win32.whl", hash = "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8"},
-    {file = "coverage-7.2.2-cp37-cp37m-win_amd64.whl", hash = "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25"},
-    {file = "coverage-7.2.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6"},
-    {file = "coverage-7.2.2-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5"},
-    {file = "coverage-7.2.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4"},
-    {file = "coverage-7.2.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd"},
-    {file = "coverage-7.2.2-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84"},
-    {file = "coverage-7.2.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540"},
-    {file = "coverage-7.2.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88"},
-    {file = "coverage-7.2.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2"},
-    {file = "coverage-7.2.2-cp38-cp38-win32.whl", hash = "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3"},
-    {file = "coverage-7.2.2-cp38-cp38-win_amd64.whl", hash = "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8"},
-    {file = "coverage-7.2.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d"},
-    {file = "coverage-7.2.2-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005"},
-    {file = "coverage-7.2.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988"},
-    {file = "coverage-7.2.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149"},
-    {file = "coverage-7.2.2-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8"},
-    {file = "coverage-7.2.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140"},
-    {file = "coverage-7.2.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016"},
-    {file = "coverage-7.2.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be"},
-    {file = "coverage-7.2.2-cp39-cp39-win32.whl", hash = "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc"},
-    {file = "coverage-7.2.2-cp39-cp39-win_amd64.whl", hash = "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef"},
-    {file = "coverage-7.2.2-pp37.pp38.pp39-none-any.whl", hash = "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968"},
-    {file = "coverage-7.2.2.tar.gz", hash = "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2"},
+    {file = "coverage-7.2.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5"},
+    {file = "coverage-7.2.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4"},
+    {file = "coverage-7.2.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2"},
+    {file = "coverage-7.2.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013"},
+    {file = "coverage-7.2.3-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa"},
+    {file = "coverage-7.2.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b"},
+    {file = "coverage-7.2.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257"},
+    {file = "coverage-7.2.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535"},
+    {file = "coverage-7.2.3-cp310-cp310-win32.whl", hash = "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91"},
+    {file = "coverage-7.2.3-cp310-cp310-win_amd64.whl", hash = "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e"},
+    {file = "coverage-7.2.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79"},
+    {file = "coverage-7.2.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc"},
+    {file = "coverage-7.2.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df"},
+    {file = "coverage-7.2.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623"},
+    {file = "coverage-7.2.3-cp311-cp311-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d"},
+    {file = "coverage-7.2.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93"},
+    {file = "coverage-7.2.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"},
+    {file = "coverage-7.2.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4"},
+    {file = "coverage-7.2.3-cp311-cp311-win32.whl", hash = "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925"},
+    {file = "coverage-7.2.3-cp311-cp311-win_amd64.whl", hash = "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910"},
+    {file = "coverage-7.2.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c"},
+    {file = "coverage-7.2.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9"},
+    {file = "coverage-7.2.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1"},
+    {file = "coverage-7.2.3-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1"},
+    {file = "coverage-7.2.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21"},
+    {file = "coverage-7.2.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841"},
+    {file = "coverage-7.2.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48"},
+    {file = "coverage-7.2.3-cp37-cp37m-win32.whl", hash = "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1"},
+    {file = "coverage-7.2.3-cp37-cp37m-win_amd64.whl", hash = "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f"},
+    {file = "coverage-7.2.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab"},
+    {file = "coverage-7.2.3-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040"},
+    {file = "coverage-7.2.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1"},
+    {file = "coverage-7.2.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911"},
+    {file = "coverage-7.2.3-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462"},
+    {file = "coverage-7.2.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c"},
+    {file = "coverage-7.2.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd"},
+    {file = "coverage-7.2.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152"},
+    {file = "coverage-7.2.3-cp38-cp38-win32.whl", hash = "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22"},
+    {file = "coverage-7.2.3-cp38-cp38-win_amd64.whl", hash = "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367"},
+    {file = "coverage-7.2.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235"},
+    {file = "coverage-7.2.3-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21"},
+    {file = "coverage-7.2.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934"},
+    {file = "coverage-7.2.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859"},
+    {file = "coverage-7.2.3-cp39-cp39-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9"},
+    {file = "coverage-7.2.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539"},
+    {file = "coverage-7.2.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe"},
+    {file = "coverage-7.2.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4"},
+    {file = "coverage-7.2.3-cp39-cp39-win32.whl", hash = "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30"},
+    {file = "coverage-7.2.3-cp39-cp39-win_amd64.whl", hash = "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a"},
+    {file = "coverage-7.2.3-pp37.pp38.pp39-none-any.whl", hash = "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0"},
+    {file = "coverage-7.2.3.tar.gz", hash = "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259"},
 ]
 
 [package.extras]
 toml = ["tomli"]
 
 [[package]]
 name = "dill"
@@ -570,22 +570,22 @@
 files = [
     {file = "imagesize-1.4.1-py2.py3-none-any.whl", hash = "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b"},
     {file = "imagesize-1.4.1.tar.gz", hash = "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"},
 ]
 
 [[package]]
 name = "importlib-metadata"
-version = "6.1.0"
+version = "6.3.0"
 description = "Read metadata from Python packages"
 category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "importlib_metadata-6.1.0-py3-none-any.whl", hash = "sha256:ff80f3b5394912eb1b108fcfd444dc78b7f1f3e16b16188054bd01cb9cb86f09"},
-    {file = "importlib_metadata-6.1.0.tar.gz", hash = "sha256:43ce9281e097583d758c2c708c4376371261a02c34682491a8e98352365aad20"},
+    {file = "importlib_metadata-6.3.0-py3-none-any.whl", hash = "sha256:8f8bd2af397cf33bd344d35cfe7f489219b7d14fc79a3f854b75b8417e9226b0"},
+    {file = "importlib_metadata-6.3.0.tar.gz", hash = "sha256:23c2bcae4762dfb0bbe072d358faec24957901d75b6c4ab11172c0c982532402"},
 ]
 
 [package.dependencies]
 zipp = ">=0.5"
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
@@ -911,26 +911,26 @@
 ]
 
 [package.extras]
 plugins = ["importlib-metadata"]
 
 [[package]]
 name = "pylint"
-version = "2.17.1"
+version = "2.17.2"
 description = "python code static checker"
 category = "dev"
 optional = false
 python-versions = ">=3.7.2"
 files = [
-    {file = "pylint-2.17.1-py3-none-any.whl", hash = "sha256:8660a54e3f696243d644fca98f79013a959c03f979992c1ab59c24d3f4ec2700"},
-    {file = "pylint-2.17.1.tar.gz", hash = "sha256:d4d009b0116e16845533bc2163493d6681846ac725eab8ca8014afb520178ddd"},
+    {file = "pylint-2.17.2-py3-none-any.whl", hash = "sha256:001cc91366a7df2970941d7e6bbefcbf98694e00102c1f121c531a814ddc2ea8"},
+    {file = "pylint-2.17.2.tar.gz", hash = "sha256:1b647da5249e7c279118f657ca28b6aaebb299f86bf92affc632acf199f7adbb"},
 ]
 
 [package.dependencies]
-astroid = ">=2.15.0,<=2.17.0-dev0"
+astroid = ">=2.15.2,<=2.17.0-dev0"
 colorama = {version = ">=0.4.5", markers = "sys_platform == \"win32\""}
 dill = [
     {version = ">=0.2", markers = "python_version < \"3.11\""},
     {version = ">=0.3.6", markers = "python_version >= \"3.11\""},
 ]
 isort = ">=4.2.5,<6"
 mccabe = ">=0.6,<0.8"
```

### Comparing `pontos-23.4.1/pontos/__init__.py` & `pontos-23.4.2/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/changelog/__init__.py` & `pontos-23.4.2/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/changelog/conventional_commits.py` & `pontos-23.4.2/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/changelog/errors.py` & `pontos-23.4.2/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/changelog/main.py` & `pontos-23.4.2/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/errors.py` & `pontos-23.4.2/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/git/__init__.py` & `pontos-23.4.2/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/git/git.py` & `pontos-23.4.2/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/git/status.py` & `pontos-23.4.2/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/__init__.py` & `pontos-23.4.2/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/actions/__init__.py` & `pontos-23.4.2/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/actions/argparser.py` & `pontos-23.4.2/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/actions/cmds.py` & `pontos-23.4.2/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/actions/core.py` & `pontos-23.4.2/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/actions/env.py` & `pontos-23.4.2/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/actions/errors.py` & `pontos-23.4.2/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/actions/event.py` & `pontos-23.4.2/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/actions/main.py` & `pontos-23.4.2/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/__init__.py` & `pontos-23.4.2/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/api.py` & `pontos-23.4.2/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/artifacts.py` & `pontos-23.4.2/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/branch.py` & `pontos-23.4.2/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/client.py` & `pontos-23.4.2/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/contents.py` & `pontos-23.4.2/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/errors.py` & `pontos-23.4.2/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/helper.py` & `pontos-23.4.2/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/labels.py` & `pontos-23.4.2/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/organizations.py` & `pontos-23.4.2/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/pull_requests.py` & `pontos-23.4.2/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/release.py` & `pontos-23.4.2/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/repositories.py` & `pontos-23.4.2/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/search.py` & `pontos-23.4.2/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/tags.py` & `pontos-23.4.2/pontos/github/api/tags.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from datetime import datetime
-from typing import Any, Dict, Optional, Union
+from typing import Any, AsyncIterator, Dict, Optional, Union
 
 from pontos.github.api.client import GitHubAsyncREST
-from pontos.github.models.tag import GitObjectType, Tag
+from pontos.github.models.tag import GitObjectType, RepositoryTag, Tag
 from pontos.helper import enum_or_value
 
 
 class GitHubAsyncRESTTags(GitHubAsyncREST):
     async def create(
         self,
         repo: str,
@@ -150,14 +150,43 @@
 
         Example:
             .. code-block:: python
 
                 from pontos.github.api import GitHubAsyncRESTApi
 
                 async with GitHubAsyncRESTApi(token) as api:
-                    tag = await api.tags.get("foo/bar", e746420)
+                    tag = await api.tags.get("foo/bar", "e746420")
                     print(tag)
         """
         api = f"/repos/{repo}/git/tags/{tag_sha}"
         response = await self._client.get(api)
         response.raise_for_status()
         return Tag.from_dict(response.json())
+
+    async def get_all(self, repo: str) -> AsyncIterator[RepositoryTag]:
+        """
+        Get information about all git tags
+
+        Args:
+            repo: GitHub repository (owner/name) to use
+
+        Raises:
+            HTTPStatusError: If the request was invalid
+
+        Example:
+            .. code-block:: python
+
+                from pontos.github.api import GitHubAsyncRESTApi
+
+                async with GitHubAsyncRESTApi(token) as api:
+                    async for tag in api.tags.get_all(
+                        "foo/bar"
+                    ):
+                        print(tag)
+        """
+        api = f"/repos/{repo}/git/tags"
+        params = {"per_page": "100"}
+
+        async for response in self._client.get_all(api, params=params):
+            response.raise_for_status()
+            for tag in response.json():
+                yield RepositoryTag.from_dict(tag)
```

### Comparing `pontos-23.4.1/pontos/github/api/teams.py` & `pontos-23.4.2/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/api/workflows.py` & `pontos-23.4.2/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/argparser.py` & `pontos-23.4.2/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/cmds.py` & `pontos-23.4.2/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/main.py` & `pontos-23.4.2/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/models/__init__.py` & `pontos-23.4.2/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/models/artifact.py` & `pontos-23.4.2/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/models/base.py` & `pontos-23.4.2/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/models/branch.py` & `pontos-23.4.2/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/models/organization.py` & `pontos-23.4.2/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/models/pull_request.py` & `pontos-23.4.2/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/models/release.py` & `pontos-23.4.2/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/models/search.py` & `pontos-23.4.2/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/models/tag.py` & `pontos-23.4.2/pontos/github/models/tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,7 +151,41 @@
     tag: str
     sha: str
     url: str
     message: str
     tagger: Tagger
     object: GitObject
     verification: Optional[Verification] = None
+
+
+@dataclass
+class Commit(GitHubModel):
+    """
+    A GitHub commit model, storing URL and SHA of a commit
+
+    Attributes:
+        sha: Commits SHA hash
+        url: Commits URL
+    """
+
+    sha: str
+    url: str
+
+
+@dataclass
+class RepositoryTag(GitHubModel):
+    """
+    A GitHub tag model, when accessing all tags of a repository
+
+    Attributes:
+        node_id: Node ID of the tag
+        name: The tag name
+        zipball_url: Link to the tags zip ball content
+        tarball_url: Link to the tags tar ball content
+        commit: SHA and URL to the commit the tag points to
+    """
+
+    node_id: str
+    name: str
+    zipball_url: str
+    tarball_url: str
+    commit: Commit
```

### Comparing `pontos-23.4.1/pontos/github/models/workflow.py` & `pontos-23.4.2/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/pr_template.md` & `pontos-23.4.2/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/script/__init__.py` & `pontos-23.4.2/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/script/errors.py` & `pontos-23.4.2/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/script/load.py` & `pontos-23.4.2/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/github/script/parser.py` & `pontos-23.4.2/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/helper.py` & `pontos-23.4.2/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/models/__init__.py` & `pontos-23.4.2/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/__init__.py` & `pontos-23.4.2/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/api.py` & `pontos-23.4.2/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/cpe/__init__.py` & `pontos-23.4.2/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/cpe/api.py` & `pontos-23.4.2/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/cve/__init__.py` & `pontos-23.4.2/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/cve/api.py` & `pontos-23.4.2/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/models/__init__.py` & `pontos-23.4.2/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/models/cpe.py` & `pontos-23.4.2/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/models/cve.py` & `pontos-23.4.2/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/models/cvss_v2.py` & `pontos-23.4.2/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/nvd/models/cvss_v3.py` & `pontos-23.4.2/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/pontos.py` & `pontos-23.4.2/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/release/__init__.py` & `pontos-23.4.2/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/release/helper.py` & `pontos-23.4.2/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/release/main.py` & `pontos-23.4.2/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/release/parser.py` & `pontos-23.4.2/pontos/release/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         "--git-tag-prefix",
         default="v",
         help="Prefix for git tag versions. Default: %(default)s",
     )
     release_parser.add_argument(
         "--git-signing-key",
         help="The key to sign the commits and tag for a release",
+        default=os.environ.get("GPG_SIGNING_KEY"),
     )
     release_parser.add_argument(
         "--project",
         help="The github project",
     )
     release_parser.add_argument(
         "--space",
```

### Comparing `pontos-23.4.1/pontos/release/release.py` & `pontos-23.4.2/pontos/release/release.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,16 @@
 
         try:
             project = Project(versioning_scheme)
         except PontosError as e:
             self.terminal.error(f"Unable to determine project settings. {e}")
             return ReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
 
+        self.terminal.info(f"Using versioning scheme {versioning_scheme}")
+
         calculator = versioning_scheme.calculator()
 
         try:
             current_version = project.get_current_version()
 
             self.terminal.info(f"Current version is {current_version}")
 
@@ -250,18 +252,24 @@
         last_release_version = get_last_release_version(
             calculator.version_from_string,
             git_tag_prefix=self.git_tag_prefix,
             ignore_pre_releases=not release_version.is_pre_release,
             tag_name=tag_name,
         )
 
-        self.terminal.info(
-            f"Creating changelog for {release_version} since "
-            f"{last_release_version}"
-        )
+        if not last_release_version:
+            self.terminal.info(
+                f"No last release found. Creating changelog for the initial "
+                f"release {release_version}"
+            )
+        else:
+            self.terminal.info(
+                f"Creating changelog for {release_version} since "
+                f"{last_release_version}"
+            )
 
         release_text = self._create_changelog(
             release_version, last_release_version, cc_config
         )
 
         self.terminal.info("Committing changes")
```

### Comparing `pontos-23.4.1/pontos/release/sign.py` & `pontos-23.4.2/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/terminal/__init__.py` & `pontos-23.4.2/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/terminal/null.py` & `pontos-23.4.2/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/terminal/rich.py` & `pontos-23.4.2/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/terminal/terminal.py` & `pontos-23.4.2/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/testing/__init__.py` & `pontos-23.4.2/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/__init__.py` & `pontos-23.4.2/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/__main__.py` & `pontos-23.4.2/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.c` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.c`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.go` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.go`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.h` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.h`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.js` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.js`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.po` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.po`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.py` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl` & `pontos-23.4.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-only/template.c` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-only/template.c`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-only/template.h` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-only/template.h`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.bash` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.bash`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.c` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.c`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.h` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.h`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.js` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.js`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.po` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.po`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.py` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.sh` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.sh`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.txt` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.txt`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xml` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xml`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl` & `pontos-23.4.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.bash` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.bash`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.c` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.c`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.go` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.go`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.h` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.h`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.js` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.js`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.po` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.po`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.py` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.sh` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.sh`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.txt` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.txt`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xml` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xml`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl` & `pontos-23.4.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/updateheader/updateheader.py` & `pontos-23.4.2/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/__init__.py` & `pontos-23.4.2/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/__main__.py` & `pontos-23.4.2/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/_calculator.py` & `pontos-23.4.2/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/commands/__init__.py` & `pontos-23.4.2/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/commands/_cmake.py` & `pontos-23.4.2/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/commands/_command.py` & `pontos-23.4.2/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/commands/_go.py` & `pontos-23.4.2/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/commands/_javascript.py` & `pontos-23.4.2/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/commands/_python.py` & `pontos-23.4.2/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/errors.py` & `pontos-23.4.2/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/helper.py` & `pontos-23.4.2/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/main.py` & `pontos-23.4.2/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/parser.py` & `pontos-23.4.2/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/project.py` & `pontos-23.4.2/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/schemes/__init__.py` & `pontos-23.4.2/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/schemes/_pep440.py` & `pontos-23.4.2/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/schemes/_scheme.py` & `pontos-23.4.2/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/schemes/_semantic.py` & `pontos-23.4.2/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pontos/version/version.py` & `pontos-23.4.2/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/pyproject.toml` & `pontos-23.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.4.1"
+version = "23.4.2"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
```

### Comparing `pontos-23.4.1/scripts/github/artifacts-download.py` & `pontos-23.4.2/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/artifacts.py` & `pontos-23.4.2/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/branchprotection.py` & `pontos-23.4.2/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/create-repository.py` & `pontos-23.4.2/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/enforce-admins.py` & `pontos-23.4.2/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/lock-branch.py` & `pontos-23.4.2/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/members.py` & `pontos-23.4.2/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/release-assets-download.py` & `pontos-23.4.2/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/repositories.py` & `pontos-23.4.2/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/search-repositories.py` & `pontos-23.4.2/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/team-repositories.py` & `pontos-23.4.2/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/teams.py` & `pontos-23.4.2/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/scripts/github/workflow-runs.py` & `pontos-23.4.2/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/__init__.py` & `pontos-23.4.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/changelog/__init__.py` & `pontos-23.4.2/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/changelog/test_conventional_commits.py` & `pontos-23.4.2/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/changelog/test_parser.py` & `pontos-23.4.2/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/git/__init__.py` & `pontos-23.4.2/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/git/test_git.py` & `pontos-23.4.2/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/git/test_status.py` & `pontos-23.4.2/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/__init__.py` & `pontos-23.4.2/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/actions/__init__.py` & `pontos-23.4.2/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/actions/test-pull-request-event.json` & `pontos-23.4.2/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/actions/test_core.py` & `pontos-23.4.2/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/actions/test_env.py` & `pontos-23.4.2/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/actions/test_event.py` & `pontos-23.4.2/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/__init__.py` & `pontos-23.4.2/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/pr-files.json` & `pontos-23.4.2/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/release-response.json` & `pontos-23.4.2/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_artifacts.py` & `pontos-23.4.2/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_branch.py` & `pontos-23.4.2/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_client.py` & `pontos-23.4.2/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_contents.py` & `pontos-23.4.2/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_labels.py` & `pontos-23.4.2/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_organizations.py` & `pontos-23.4.2/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_pull_requests.py` & `pontos-23.4.2/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_release.py` & `pontos-23.4.2/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_repositories.py` & `pontos-23.4.2/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_search.py` & `pontos-23.4.2/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_tags.py` & `pontos-23.4.2/tests/github/api/test_tags.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-# pylint: disable=line-too-long
+# pylint: disable=too-many-lines, redefined-builtin, line-too-long
 
 from datetime import datetime, timezone
 from unittest.mock import MagicMock
 
 import httpx
 
 from pontos.github.api.tags import GitHubAsyncRESTTags
 from pontos.github.models.tag import GitObjectType, Tag, VerificationReason
+from tests import AsyncIteratorMock, aiter, anext
 from tests.github.api import GitHubAsyncRESTTestCase, create_response
 
 TAG_JSON = {
     "node_id": "MDM6VGFnOTQwYmQzMzYyNDhlZmFlMGY5ZWU1YmM3YjJkNWM5ODU4ODdiMTZhYw==",
     "tag": "v0.0.1",
     "sha": "940bd336248efae0f9ee5bc7b2d5c985887b16ac",
     "url": "https://api.github.com/repos/octocat/Hello-World/git/tags/940bd336248efae0f9ee5bc7b2d5c985887b16ac",
@@ -47,14 +48,38 @@
         "reason": "unsigned",
         "signature": None,
         "payload": None,
     },
 }
 
 
+TAGS_JSON = [
+    {
+        "name": "v0.1.0",
+        "zipball_url": "https://api.github.com/repos/foo/ui/zipball/refs/tags/v0.1.0",
+        "tarball_url": "https://api.github.com/repos/foo/ui/tarball/refs/tags/v0.1.0",
+        "commit": {
+            "sha": "b55408280162c20cf0ffef155618270d26fe7352",
+            "url": "https://api.github.com/repos/foo/ui/commits/b55408280162c20cf0ffef155618270d26fe7352",
+        },
+        "node_id": "REF_kwDOHeuT1rByZWZzL3RhZ3MvdjAuMS4w",
+    },
+    {
+        "name": "0.0.72",
+        "zipball_url": "https://api.github.com/repos/foo/ui/zipball/refs/tags/0.0.72",
+        "tarball_url": "https://api.github.com/repos/foo/ui/tarball/refs/tags/0.0.72",
+        "commit": {
+            "sha": "fd54097278df75332917d9d1a2d940083513a6b2",
+            "url": "https://api.github.com/repos/foo/ui/commits/fd54097278df75332917d9d1a2d940083513a6b2",
+        },
+        "node_id": "REF_kwDOHeuT1rByZWZzL3RhZ3MvMC4wLjcy",
+    },
+]
+
+
 class GitHubAsyncRESTTagsTestCase(GitHubAsyncRESTTestCase):
     api_cls = GitHubAsyncRESTTags
 
     def assertTag(self, tag: Tag):  # pylint: disable=invalid-name
         self.assertEqual(
             tag.node_id,
             "MDM6VGFnOTQwYmQzMzYyNDhlZmFlMGY5ZWU1YmM3YjJkNWM5ODU4ODdiMTZhYw==",
@@ -206,7 +231,35 @@
 
         with self.assertRaises(httpx.HTTPStatusError):
             await self.api.get("octocat/Hello-World", "v0.0.1")
 
         self.client.get.assert_awaited_once_with(
             "/repos/octocat/Hello-World/git/tags/v0.0.1"
         )
+
+    async def test_get_all(self):
+        response = create_response()
+        response.json.return_value = TAGS_JSON
+        self.client.get_all.return_value = AsyncIteratorMock([response])
+
+        async_it = aiter(self.api.get_all("foo"))
+
+        tag = await anext(async_it)
+        self.assertEqual(tag.name, "v0.1.0")
+        self.assertEqual(
+            tag.commit.sha, "b55408280162c20cf0ffef155618270d26fe7352"
+        )
+        self.assertEqual(
+            tag.commit.url,
+            "https://api.github.com/repos/foo/ui/commits/b55408280162c20cf0ffef155618270d26fe7352",
+        )
+        self.assertEqual(
+            tag.zipball_url,
+            "https://api.github.com/repos/foo/ui/zipball/refs/tags/v0.1.0",
+        )
+        self.assertEqual(
+            tag.tarball_url,
+            "https://api.github.com/repos/foo/ui/tarball/refs/tags/v0.1.0",
+        )
+        self.assertEqual(tag.node_id, "REF_kwDOHeuT1rByZWZzL3RhZ3MvdjAuMS4w")
+        tag2 = await anext(async_it)
+        self.assertEqual(tag2.name, "0.0.72")
```

### Comparing `pontos-23.4.1/tests/github/api/test_teams.py` & `pontos-23.4.2/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/api/test_workflows.py` & `pontos-23.4.2/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/models/__init__.py` & `pontos-23.4.2/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/models/test_artifact.py` & `pontos-23.4.2/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/models/test_base.py` & `pontos-23.4.2/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/models/test_branch.py` & `pontos-23.4.2/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/models/test_organization.py` & `pontos-23.4.2/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/models/test_pull_request.py` & `pontos-23.4.2/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/models/test_release.py` & `pontos-23.4.2/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/models/test_search.py` & `pontos-23.4.2/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/models/test_tag.py` & `pontos-23.4.2/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/models/test_workflow.py` & `pontos-23.4.2/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/script/__init__.py` & `pontos-23.4.2/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/script/test_load.py` & `pontos-23.4.2/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/script/test_parser.py` & `pontos-23.4.2/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/test_argparser.py` & `pontos-23.4.2/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/github/test_cmds.py` & `pontos-23.4.2/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/models/__init__.py` & `pontos-23.4.2/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/models/test_models.py` & `pontos-23.4.2/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/nvd/__init__.py` & `pontos-23.4.2/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/nvd/cpe/__init__.py` & `pontos-23.4.2/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/nvd/cpe/test_api.py` & `pontos-23.4.2/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/nvd/cve/__init__.py` & `pontos-23.4.2/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/nvd/cve/test_api.py` & `pontos-23.4.2/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/nvd/models/__init__.py` & `pontos-23.4.2/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/nvd/models/test_cpe.py` & `pontos-23.4.2/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/nvd/models/test_cve.py` & `pontos-23.4.2/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/nvd/test_api.py` & `pontos-23.4.2/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/release/__init__.py` & `pontos-23.4.2/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/release/test_helper.py` & `pontos-23.4.2/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/release/test_parser.py` & `pontos-23.4.2/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/release/test_release.py` & `pontos-23.4.2/tests/release/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/release/test_sign.py` & `pontos-23.4.2/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/terminal/__init__.py` & `pontos-23.4.2/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/terminal/test_terminal.py` & `pontos-23.4.2/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/test_helper.py` & `pontos-23.4.2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/test_pontos.py` & `pontos-23.4.2/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/testing/__init__.py` & `pontos-23.4.2/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/testing/test_testing.py` & `pontos-23.4.2/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/updateheader/__init__.py` & `pontos-23.4.2/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/updateheader/test_header.py` & `pontos-23.4.2/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/__init__.py` & `pontos-23.4.2/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/commands/__init__.py` & `pontos-23.4.2/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/commands/test_cmake.py` & `pontos-23.4.2/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/commands/test_go.py` & `pontos-23.4.2/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/commands/test_javascript.py` & `pontos-23.4.2/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/commands/test_python.py` & `pontos-23.4.2/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/schemes/__init__.py` & `pontos-23.4.2/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/schemes/test_pep440.py` & `pontos-23.4.2/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/schemes/test_semantic.py` & `pontos-23.4.2/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/test_commands.py` & `pontos-23.4.2/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/test_errors.py` & `pontos-23.4.2/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/test_helper.py` & `pontos-23.4.2/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/test_main.py` & `pontos-23.4.2/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/test_parser.py` & `pontos-23.4.2/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/test_project.py` & `pontos-23.4.2/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/tests/version/test_version.py` & `pontos-23.4.2/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.1/PKG-INFO` & `pontos-23.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.4.1
+Version: 23.4.2
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

