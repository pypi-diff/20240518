# Comparing `tmp/zettel_org-0.7.2.tar.gz` & `tmp/zettel_org-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zettel_org-0.7.2.tar", last modified: Sun May  5 20:46:54 2024, max compression
+gzip compressed data, was "zettel_org-0.7.3.tar", last modified: Sat May 18 01:59:35 2024, max compression
```

## Comparing `zettel_org-0.7.2.tar` & `zettel_org-0.7.3.tar`

### file list

```diff
@@ -1,194 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.732855 zettel_org-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.708855 zettel_org-0.7.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-05 20:46:46.000000 zettel_org-0.7.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-05 20:46:46.000000 zettel_org-0.7.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-05 20:46:46.000000 zettel_org-0.7.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-05 20:46:46.000000 zettel_org-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-05 20:46:46.000000 zettel_org-0.7.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-05 20:46:46.000000 zettel_org-0.7.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-05-05 20:46:54.732855 zettel_org-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-05-05 20:46:46.000000 zettel_org-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3093 2024-05-05 20:46:46.000000 zettel_org-0.7.2/bin/build_zorg_grammars
--rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-05-05 20:46:46.000000 zettel_org-0.7.2/bin/check_cc
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-05 20:46:46.000000 zettel_org-0.7.2/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-05-05 20:46:46.000000 zettel_org-0.7.2/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-05-05 20:46:46.000000 zettel_org-0.7.2/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/docs/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.712855 zettel_org-0.7.2/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-05 20:46:46.000000 zettel_org-0.7.2/docs/source/zorg.rst
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-05 20:46:46.000000 zettel_org-0.7.2/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.704855 zettel_org-0.7.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/examples/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/20240323.zo
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/basic.zo
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/multiblocks.zo
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/priority.zo
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/property.zo
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/scrambled_prj_notes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/subnotes.zo
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/subsections.zo
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_file/tags_and_ids.zo
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/examples/zorg_query/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_query/all_contexts.zoq
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 20:46:46.000000 zettel_org-0.7.2/examples/zorg_query/open_projects.zoq
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-05 20:46:46.000000 zettel_org-0.7.2/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-05 20:46:46.000000 zettel_org-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-05 20:46:46.000000 zettel_org-0.7.2/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-05 20:46:46.000000 zettel_org-0.7.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-05 20:46:46.000000 zettel_org-0.7.2/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-05 20:46:46.000000 zettel_org-0.7.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-05 20:46:46.000000 zettel_org-0.7.2/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-05 20:46:54.732855 zettel_org-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-05 20:46:46.000000 zettel_org-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.704855 zettel_org-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.732855 zettel_org-0.7.2/src/zettel_org.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11588 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:46:50.000000 zettel_org-0.7.2/src/zettel_org.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-05 20:46:54.000000 zettel_org-0.7.2/src/zettel_org.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/src/zorg/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.716855 zettel_org-0.7.2/src/zorg/app/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.720855 zettel_org-0.7.2/src/zorg/app/runners/
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/app/runners/_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.720855 zettel_org-0.7.2/src/zorg/domain/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.720855 zettel_org-0.7.2/src/zorg/domain/messages/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/messages/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/messages/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.720855 zettel_org-0.7.2/src/zorg/domain/models/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/models/_zorg_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/models/_zorg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/domain/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.720855 zettel_org-0.7.2/src/zorg/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/CommonLexerRules.g4
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/ZorgFile.g4
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/ZorgQuery.g4
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/grammar/zorg_file/
--rw-r--r--   0 runner    (1001) docker     (127)    16154 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFile.interp
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFile.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileListener.py
--rw-r--r--   0 runner    (1001) docker     (127)   120709 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/grammar/zorg_query/
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQuery.interp
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQuery.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
--rw-r--r--   0 runner    (1001) docker     (127)     9816 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryLexer.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryListener.py
--rw-r--r--   0 runner    (1001) docker     (127)    65908 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/grammar/zorg_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/service/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/service/compiler/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/compiler/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/compiler/_file_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/compiler/_query_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/messagebus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/service/swog/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/swog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/swog/_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/service/zid_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.724855 zettel_org-0.7.2/src/zorg/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.728855 zettel_org-0.7.2/src/zorg/storage/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10129 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-05 20:46:46.000000 zettel_org-0.7.2/src/zorg/storage/sql/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-05 20:46:46.000000 zettel_org-0.7.2/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.728855 zettel_org-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.728855 zettel_org-0.7.2/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    71784 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__snapshots__/test_run_compile.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__snapshots__/test_run_db.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__snapshots__/test_run_edit.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    23947 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__snapshots__/test_run_query.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/__snapshots__/test_run_template.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:46:54.732855 zettel_org-0.7.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/data/day_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/data/done_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/data/habit_log.zot
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/data/hello.zot
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/data/links.zo
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_file_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_action_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tests/test_run_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-05 20:46:46.000000 zettel_org-0.7.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.728771 zettel_org-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-18 01:59:27.000000 zettel_org-0.7.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-05-18 01:59:27.000000 zettel_org-0.7.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-18 01:59:27.000000 zettel_org-0.7.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-05-18 01:59:27.000000 zettel_org-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-18 01:59:27.000000 zettel_org-0.7.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-18 01:59:27.000000 zettel_org-0.7.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-18 01:59:35.728771 zettel_org-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-18 01:59:27.000000 zettel_org-0.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3093 2024-05-18 01:59:27.000000 zettel_org-0.7.3/bin/build_zorg_grammars
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-05-18 01:59:27.000000 zettel_org-0.7.3/bin/check_cc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-18 01:59:27.000000 zettel_org-0.7.3/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-05-18 01:59:27.000000 zettel_org-0.7.3/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-05-18 01:59:27.000000 zettel_org-0.7.3/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.708770 zettel_org-0.7.3/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/design/design.template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-18 01:59:27.000000 zettel_org-0.7.3/docs/source/zorg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 01:59:27.000000 zettel_org-0.7.3/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.700770 zettel_org-0.7.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/examples/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/20240323.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/basic.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/multiblocks.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/priority.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/property.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/scrambled_prj_notes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/subnotes.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/subsections.zo
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_file/tags_and_ids.zo
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/examples/zorg_query/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_query/all_contexts.zoq
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-18 01:59:27.000000 zettel_org-0.7.3/examples/zorg_query/open_projects.zoq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-05-18 01:59:27.000000 zettel_org-0.7.3/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-18 01:59:27.000000 zettel_org-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-18 01:59:27.000000 zettel_org-0.7.3/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-05-18 01:59:27.000000 zettel_org-0.7.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-18 01:59:27.000000 zettel_org-0.7.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-18 01:59:27.000000 zettel_org-0.7.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.712770 zettel_org-0.7.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-18 01:59:27.000000 zettel_org-0.7.3/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-18 01:59:35.732771 zettel_org-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-18 01:59:27.000000 zettel_org-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.700770 zettel_org-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.728771 zettel_org-0.7.3/src/zettel_org.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 01:59:31.000000 zettel_org-0.7.3/src/zettel_org.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-18 01:59:35.000000 zettel_org-0.7.3/src/zettel_org.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.716771 zettel_org-0.7.3/src/zorg/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.716771 zettel_org-0.7.3/src/zorg/app/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.716771 zettel_org-0.7.3/src/zorg/app/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/app/runners/_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.716771 zettel_org-0.7.3/src/zorg/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.716771 zettel_org-0.7.3/src/zorg/domain/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/messages/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/messages/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.720771 zettel_org-0.7.3/src/zorg/domain/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/models/_zorg_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/models/_zorg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/domain/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.720771 zettel_org-0.7.3/src/zorg/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/CommonLexerRules.g4
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/ZorgFile.g4
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/ZorgQuery.g4
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.720771 zettel_org-0.7.3/src/zorg/grammar/zorg_file/
+-rw-r--r--   0 runner    (1001) docker     (127)    16243 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFile.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFile.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)     9817 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121459 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.720771 zettel_org-0.7.3/src/zorg/grammar/zorg_query/
+-rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQuery.interp
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQuery.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    12504 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryLexer.interp
+-rw-r--r--   0 runner    (1001) docker     (127)    12969 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryLexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryListener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92723 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/grammar/zorg_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.724771 zettel_org-0.7.3/src/zorg/service/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.724771 zettel_org-0.7.3/src/zorg/service/compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/compiler/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16269 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/compiler/_file_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12306 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/compiler/_query_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12846 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/messagebus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.724771 zettel_org-0.7.3/src/zorg/service/swog/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/swog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/swog/_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/service/zid_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.724771 zettel_org-0.7.3/src/zorg/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.724771 zettel_org-0.7.3/src/zorg/storage/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15674 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-18 01:59:27.000000 zettel_org-0.7.3/src/zorg/storage/sql/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-05-18 01:59:27.000000 zettel_org-0.7.3/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.728771 zettel_org-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.728771 zettel_org-0.7.3/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_action_open.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    62043 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_compile.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_db.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_edit.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    29656 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_query.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/__snapshots__/test_run_template.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:59:35.728771 zettel_org-0.7.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/data/day_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/data/done_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/data/habit_log.zot
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/data/hello.zot
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/data/links.zo
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_file_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_action_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tests/test_run_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-18 01:59:27.000000 zettel_org-0.7.3/tox.ini
```

### Comparing `zettel_org-0.7.2/.cruft.json` & `zettel_org-0.7.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/.github/labels.yml` & `zettel_org-0.7.3/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/.github/workflows/ci.yml` & `zettel_org-0.7.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/.gitignore` & `zettel_org-0.7.3/.gitignore`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/.pylintrc` & `zettel_org-0.7.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/.readthedocs.yml` & `zettel_org-0.7.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/CHANGELOG.md` & `zettel_org-0.7.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,23 @@
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
 
-## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.7.2...HEAD)
+## [Unreleased](https://github.com/bbugyi200/zorg/compare/0.7.3...HEAD)
+
+
+## [0.7.3](https://github.com/bbugyi200/zorg/compare/0.7.2...0.7.3) - 2024-05-17
+
+### Added
+
+* Add support for the various new WHERE filters and new GROUP BY dimensions.
+* Add ORDER BY support to zorg queries.
 
 
 ## [0.7.2](https://github.com/bbugyi200/zorg/compare/0.7.1...0.7.2) - 2024-05-05
 
 ### Added
 
 * Implement basic functionality for `zorg query`. We can now SELECT notes with
```

### Comparing `zettel_org-0.7.2/CONTRIBUTING.md` & `zettel_org-0.7.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/Dockerfile` & `zettel_org-0.7.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/Makefile` & `zettel_org-0.7.3/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/PKG-INFO` & `zettel_org-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.7.2
+Version: 0.7.3
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -98,14 +98,15 @@
     "db",
     "db create",
     "db reindex",
     "edit",
     "query",
     "template",
     "template init",
+    "template list",
     "template render",
 ]:
     popen = subprocess.Popen(["zorg"] + cmd.split() + ["--help"], stdout=subprocess.PIPE)
     stdout, _ = popen.communicate()
     print(f"\n### `zorg {cmd} --help`\n")
     print("```", stdout.decode().strip(), "```", sep="\n")
 ]]]]] -->
@@ -167,21 +168,23 @@
   {open}
     open      Open a zettel link if one exists on the provided zorg file line.
 ```
 
 ### `zorg action open --help`
 
 ```
-usage: zorg action open [-h] zo_path line_number
+usage: zorg action open [-h] zo_path line_number [option_idx]
 
 Open a zettel link if one exists on the provided zorg file line.
 
 positional arguments:
   line_number  The line number that your editor cursor is currently located
                on.
+  option_idx   Used on a second 'action open' run to indicate which option was
+               selected.
   zo_path      The file that your editor currently has open.
 
 options:
   -h, --help   show this help message and exit
 ```
 
 ### `zorg compile --help`
@@ -267,25 +270,24 @@
 options:
   -h, --help  show this help message and exit
 ```
 
 ### `zorg template --help`
 
 ```
-usage: zorg template [-h] {render,init} ...
+usage: zorg template render [-h] template [variables ...]
 
-Commands for managing .zot templates.
+Render a new .zo file using a .zot template.
 
-options:
-  -h, --help     show this help message and exit
+positional arguments:
+  template    Path to the .zot template.
+  variables   A list of variable specs of the form of key=value.
 
-subcommands:
-  {render,init}
-    render       Render a new .zo file using a .zot template.
-    init         Initialize a new file using a zorg template.
+options:
+  -h, --help  show this help message and exit
 ```
 
 ### `zorg template init --help`
 
 ```
 usage: zorg template init [-h] [-t TEMPLATE] new_path [variables ...]
 
@@ -299,14 +301,25 @@
   -h, --help            show this help message and exit
   -t TEMPLATE, --template TEMPLATE
                         Optional path to the .zot template. If a template is
                         not provided, we will infer what template to use based
                         off of the new file's name.
 ```
 
+### `zorg template list --help`
+
+```
+usage: zorg template list [-h]
+
+List all zorg template files.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ### `zorg template render --help`
 
 ```
 usage: zorg template render [-h] template [variables ...]
 
 Render a new .zo file using a .zot template.
```

### Comparing `zettel_org-0.7.2/README.md` & `zettel_org-0.7.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     "db",
     "db create",
     "db reindex",
     "edit",
     "query",
     "template",
     "template init",
+    "template list",
     "template render",
 ]:
     popen = subprocess.Popen(["zorg"] + cmd.split() + ["--help"], stdout=subprocess.PIPE)
     stdout, _ = popen.communicate()
     print(f"\n### `zorg {cmd} --help`\n")
     print("```", stdout.decode().strip(), "```", sep="\n")
 ]]]]] -->
@@ -137,21 +138,23 @@
   {open}
     open      Open a zettel link if one exists on the provided zorg file line.
 ```
 
 ### `zorg action open --help`
 
 ```
-usage: zorg action open [-h] zo_path line_number
+usage: zorg action open [-h] zo_path line_number [option_idx]
 
 Open a zettel link if one exists on the provided zorg file line.
 
 positional arguments:
   line_number  The line number that your editor cursor is currently located
                on.
+  option_idx   Used on a second 'action open' run to indicate which option was
+               selected.
   zo_path      The file that your editor currently has open.
 
 options:
   -h, --help   show this help message and exit
 ```
 
 ### `zorg compile --help`
@@ -237,25 +240,24 @@
 options:
   -h, --help  show this help message and exit
 ```
 
 ### `zorg template --help`
 
 ```
-usage: zorg template [-h] {render,init} ...
+usage: zorg template render [-h] template [variables ...]
 
-Commands for managing .zot templates.
+Render a new .zo file using a .zot template.
 
-options:
-  -h, --help     show this help message and exit
+positional arguments:
+  template    Path to the .zot template.
+  variables   A list of variable specs of the form of key=value.
 
-subcommands:
-  {render,init}
-    render       Render a new .zo file using a .zot template.
-    init         Initialize a new file using a zorg template.
+options:
+  -h, --help  show this help message and exit
 ```
 
 ### `zorg template init --help`
 
 ```
 usage: zorg template init [-h] [-t TEMPLATE] new_path [variables ...]
 
@@ -269,14 +271,25 @@
   -h, --help            show this help message and exit
   -t TEMPLATE, --template TEMPLATE
                         Optional path to the .zot template. If a template is
                         not provided, we will infer what template to use based
                         off of the new file's name.
 ```
 
+### `zorg template list --help`
+
+```
+usage: zorg template list [-h]
+
+List all zorg template files.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ### `zorg template render --help`
 
 ```
 usage: zorg template render [-h] template [variables ...]
 
 Render a new .zo file using a .zot template.
```

### Comparing `zettel_org-0.7.2/bin/build_zorg_grammars` & `zettel_org-0.7.3/bin/build_zorg_grammars`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/bin/check_cc` & `zettel_org-0.7.3/bin/check_cc`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/bin/publish_docs` & `zettel_org-0.7.3/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/bin/quick-lints` & `zettel_org-0.7.3/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/bin/render_all_cogs` & `zettel_org-0.7.3/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/docs/Makefile` & `zettel_org-0.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/docs/make.bat` & `zettel_org-0.7.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/docs/source/conf.py` & `zettel_org-0.7.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/lib/bugyi.sh` & `zettel_org-0.7.3/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/requirements-dev.in` & `zettel_org-0.7.3/requirements-dev.in`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/requirements-dev.txt` & `zettel_org-0.7.3/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     # via
     #   -r requirements.in
     #   zettel-org
 antlr4-tools==0.2.1
     # via -r requirements-dev.in
 arrow==1.3.0
     # via cookiecutter
-astroid==3.1.0
+astroid==3.2.1
     # via pylint
 babel==2.15.0
     # via sphinx
 binaryornot==0.4.4
     # via cookiecutter
 black==24.4.2
     # via -r requirements-dev.in
@@ -94,15 +94,15 @@
     # via pytest
 filelock==3.14.0
     # via
     #   tox
     #   virtualenv
 flake8==7.0.0
     # via -r requirements-dev.in
-freezegun==1.5.0
+freezegun==1.5.1
     # via -r requirements-dev.in
 gitdb==4.0.11
     # via gitpython
 gitpython==3.1.43
     # via cruft
 greenlet==3.0.3
     # via sqlalchemy
@@ -114,15 +114,15 @@
     # via pytest
 install-jdk==1.1.0
     # via antlr4-tools
 isort==5.13.2
     # via
     #   -r requirements-dev.in
     #   pylint
-jinja2==3.1.3
+jinja2==3.1.4
     # via
     #   -r requirements.in
     #   cookiecutter
     #   sphinx
     #   zettel-org
 m2r2==0.3.3.post2
     # via -r requirements-dev.in
@@ -152,15 +152,15 @@
     #   setuptools-scm
     #   sphinx
     #   tox
 pathspec==0.12.1
     # via black
 pip-tools==7.4.1
     # via -r requirements-dev.in
-platformdirs==4.2.1
+platformdirs==4.2.2
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.5.0
     # via
     #   pytest
@@ -182,15 +182,15 @@
     # via -r requirements-dev.in
 pyflakes==3.2.0
     # via flake8
 pygments==2.18.0
     # via
     #   rich
     #   sphinx
-pylint==3.1.0
+pylint==3.2.0
     # via -r requirements-dev.in
 pyproject-hooks==1.1.0
     # via
     #   build
     #   pip-tools
 pytest==7.4.4
     # via
@@ -220,15 +220,15 @@
     #   sphinx
 rich==13.7.1
     # via
     #   -r requirements.in
     #   cookiecutter
     #   typer
     #   zettel-org
-setuptools-scm==8.0.4
+setuptools-scm==8.1.0
     # via -r requirements-dev.in
 shellingham==1.5.4
     # via typer
 six==1.16.0
     # via
     #   python-dateutil
     #   tox
@@ -258,15 +258,15 @@
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-sqlalchemy==2.0.29
+sqlalchemy==2.0.30
     # via sqlmodel
 sqlmodel==0.0.18
     # via
     #   -r requirements.in
     #   zettel-org
 structlog==24.1.0
     # via bolton-logrus
@@ -285,15 +285,15 @@
     #   pip-tools
     #   pydocstyle
     #   pylint
     #   pytest
     #   setuptools-scm
     #   sphinx
     #   tox
-tomlkit==0.12.4
+tomlkit==0.12.5
     # via pylint
 tox==3.28.0
     # via
     #   -r requirements-dev.in
     #   tox-pyenv
 tox-pyenv==1.1.0
     # via -r requirements-dev.in
@@ -310,24 +310,23 @@
 typing-extensions==4.11.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pydantic-core
-    #   setuptools-scm
     #   sqlalchemy
     #   typer
 urllib3==2.2.1
     # via requests
 vimala==0.2.0
     # via
     #   -r requirements.in
     #   zettel-org
-virtualenv==20.26.1
+virtualenv==20.26.2
     # via tox
 wheel==0.43.0
     # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 pip==24.0
     # via pip-tools
```

### Comparing `zettel_org-0.7.2/requirements.txt` & `zettel_org-0.7.3/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # via
     #   -r requirements.in
     #   bolton-clack
     #   bolton-eris
     #   vimala
 greenlet==3.0.3
     # via sqlalchemy
-jinja2==3.1.3
+jinja2==3.1.4
     # via -r requirements.in
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
@@ -56,15 +56,15 @@
     # via rich
 python-dotenv==1.0.1
     # via pydantic-settings
 pyyaml==6.0.1
     # via bolton-clack
 rich==13.7.1
     # via -r requirements.in
-sqlalchemy==2.0.29
+sqlalchemy==2.0.30
     # via sqlmodel
 sqlmodel==0.0.18
     # via -r requirements.in
 structlog==24.1.0
     # via bolton-logrus
 tqdm==4.66.4
     # via -r requirements.in
```

### Comparing `zettel_org-0.7.2/setup.cfg` & `zettel_org-0.7.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/setup.py` & `zettel_org-0.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 DESCRIPTION = "The zettel note manager of the future."
 SUPPORTED_PYTHON_VERSIONS = [
     (3, 9),
     (3, 10),
     (3, 11),
     (3, 12),
 ]
-USE_SCM_VERSION = {"fallback_version": "0.7.2"}
+USE_SCM_VERSION = {"fallback_version": "0.7.3"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
```

### Comparing `zettel_org-0.7.2/src/zettel_org.egg-info/PKG-INFO` & `zettel_org-0.7.3/src/zettel_org.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zettel-org
-Version: 0.7.2
+Version: 0.7.3
 Summary: The zettel note manager of the future.
 Home-page: https://github.com/bbugyi200/zorg
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -98,14 +98,15 @@
     "db",
     "db create",
     "db reindex",
     "edit",
     "query",
     "template",
     "template init",
+    "template list",
     "template render",
 ]:
     popen = subprocess.Popen(["zorg"] + cmd.split() + ["--help"], stdout=subprocess.PIPE)
     stdout, _ = popen.communicate()
     print(f"\n### `zorg {cmd} --help`\n")
     print("```", stdout.decode().strip(), "```", sep="\n")
 ]]]]] -->
@@ -167,21 +168,23 @@
   {open}
     open      Open a zettel link if one exists on the provided zorg file line.
 ```
 
 ### `zorg action open --help`
 
 ```
-usage: zorg action open [-h] zo_path line_number
+usage: zorg action open [-h] zo_path line_number [option_idx]
 
 Open a zettel link if one exists on the provided zorg file line.
 
 positional arguments:
   line_number  The line number that your editor cursor is currently located
                on.
+  option_idx   Used on a second 'action open' run to indicate which option was
+               selected.
   zo_path      The file that your editor currently has open.
 
 options:
   -h, --help   show this help message and exit
 ```
 
 ### `zorg compile --help`
@@ -267,25 +270,24 @@
 options:
   -h, --help  show this help message and exit
 ```
 
 ### `zorg template --help`
 
 ```
-usage: zorg template [-h] {render,init} ...
+usage: zorg template render [-h] template [variables ...]
 
-Commands for managing .zot templates.
+Render a new .zo file using a .zot template.
 
-options:
-  -h, --help     show this help message and exit
+positional arguments:
+  template    Path to the .zot template.
+  variables   A list of variable specs of the form of key=value.
 
-subcommands:
-  {render,init}
-    render       Render a new .zo file using a .zot template.
-    init         Initialize a new file using a zorg template.
+options:
+  -h, --help  show this help message and exit
 ```
 
 ### `zorg template init --help`
 
 ```
 usage: zorg template init [-h] [-t TEMPLATE] new_path [variables ...]
 
@@ -299,14 +301,25 @@
   -h, --help            show this help message and exit
   -t TEMPLATE, --template TEMPLATE
                         Optional path to the .zot template. If a template is
                         not provided, we will infer what template to use based
                         off of the new file's name.
 ```
 
+### `zorg template list --help`
+
+```
+usage: zorg template list [-h]
+
+List all zorg template files.
+
+options:
+  -h, --help  show this help message and exit
+```
+
 ### `zorg template render --help`
 
 ```
 usage: zorg template render [-h] template [variables ...]
 
 Render a new .zo file using a .zot template.
```

### Comparing `zettel_org-0.7.2/src/zettel_org.egg-info/SOURCES.txt` & `zettel_org-0.7.3/src/zettel_org.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
 src/zorg/grammar/zorg_query/ZorgQueryLexer.py
 src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens
 src/zorg/grammar/zorg_query/ZorgQueryListener.py
 src/zorg/grammar/zorg_query/ZorgQueryParser.py
 src/zorg/grammar/zorg_query/__init__.py
 src/zorg/service/__init__.py
 src/zorg/service/common.py
+src/zorg/service/dates.py
 src/zorg/service/file_groups.py
 src/zorg/service/handlers.py
 src/zorg/service/messagebus.py
 src/zorg/service/templates.py
 src/zorg/service/zid_manager.py
 src/zorg/service/compiler/__init__.py
 src/zorg/service/compiler/_api.py
@@ -143,14 +144,15 @@
 tests/test_file_groups.py
 tests/test_run_action_open.py
 tests/test_run_compile.py
 tests/test_run_db.py
 tests/test_run_edit.py
 tests/test_run_query.py
 tests/test_run_template.py
+tests/__snapshots__/test_run_action_open.ambr
 tests/__snapshots__/test_run_compile.ambr
 tests/__snapshots__/test_run_db.ambr
 tests/__snapshots__/test_run_edit.ambr
 tests/__snapshots__/test_run_query.ambr
 tests/__snapshots__/test_run_template.ambr
 tests/data/day_log.zot
 tests/data/done_log.zot
```

### Comparing `zettel_org-0.7.2/src/zorg/app/config.py` & `zettel_org-0.7.3/src/zorg/app/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,22 +4,31 @@
 
 import itertools as it
 from pathlib import Path
 from typing import Any, Final, Literal, Optional, Sequence
 
 import clack
 from logrus import Logger
+from typist import literal_to_list
 
 from .. import APP_NAME
 from ..domain.types import FileGroupMapType, TemplatePatternMapType, VarMapType
 from ..service import common
 
 
 Command = Literal[
-    "compile", "create", "edit", "init", "open", "query", "reindex", "render"
+    "compile",
+    "create",
+    "edit",
+    "init",
+    "list",
+    "open",
+    "query",
+    "reindex",
+    "render",
 ]
 
 _LOGGER = Logger(__name__)
 
 _DEFAULT_ZETTEL_DIR: Final[Path] = Path.home() / "org"
 
 
@@ -36,24 +45,14 @@
     zettel_dir: Path = _DEFAULT_ZETTEL_DIR
 
     # ----- CONFIG
     database_url: str = _get_default_database_url(_DEFAULT_ZETTEL_DIR)
     template_pattern_map: TemplatePatternMapType = {}
 
 
-class OpenActionConfig(Config):
-    """Clack config for the 'action' command."""
-
-    command: Literal["open"]
-
-    # ----- ARGUMENTS
-    zo_path: Path
-    line_number: int
-
-
 class CompileConfig(Config):
     """Clack config for the 'compile' command."""
 
     command: Literal["compile"]
 
     # ----- ARGUMENTS
     zo_path: Path
@@ -84,23 +83,40 @@
 
     # ----- CONFIG
     file_group_map: FileGroupMapType = {}
     keep_alive_file: Path = Path("/tmp/zorg_keep_alive")
     vim_commands: list[str] = []
 
 
+class OpenActionConfig(Config):
+    """Clack config for the 'action open' command."""
+
+    command: Literal["open"]
+
+    # ----- ARGUMENTS
+    zo_path: Path
+    line_number: int
+    option_idx: Optional[int] = None
+
+
 class QueryConfig(Config):
     """Clack config for the 'query' command."""
 
     command: Literal["query"]
 
     # ----- ARGUMENTS
     query: str
 
 
+class TemplateListConfig(Config):
+    """Clack config for the 'template' command."""
+
+    command: Literal["list"]
+
+
 class TemplateRenderConfig(Config):
     """Clack config for the 'template' command."""
 
     command: Literal["render"]
 
     # ----- ARGUMENTS
     template: Path
@@ -116,29 +132,47 @@
     new_path: Path
     template: Optional[Path] = None
     var_map: Optional[VarMapType] = None
 
 
 def clack_parser(argv: Sequence[str]) -> dict[str, Any]:
     """Parser we pass to the `main_factory()` `parser` kwarg."""
-    # HACK: Make 'edit' the default sub-command.
+    # HACK: These make the command-line arguments more conveniant:
+    #
+    # * Make 'edit' the default sub-command.
+    # * Make 'render' the default sub-sub-command for the 'template'
+    #   sub-command.
+    argv_before_opts = [argv[0]] + list(
+        it.takewhile(lambda x: x.startswith("-"), argv[1:])
+    )
     argv_after_opts = list(it.dropwhile(lambda x: x.startswith("-"), argv[1:]))
     if not argv_after_opts:
         _LOGGER.debug(
             "Inferring 'edit' command since no subcommand was specified."
         )
         argv = list(argv) + ["edit"]
     elif argv_after_opts[0].startswith("@"):
-        argv_opts = list(it.takewhile(lambda x: x.startswith("-"), argv[1:]))
-        argv = [argv[0]] + argv_opts + ["edit"] + argv_after_opts
+        argv = argv_before_opts + ["edit"] + argv_after_opts
         _LOGGER.debug(
             "Inferring 'edit' command since we found a file group name.",
             file_group_name=argv_after_opts[0],
             new_args=argv[1:],
         )
+    elif (
+        argv_after_opts[0] == "template"
+        and len(argv_after_opts) > 1
+        and argv_after_opts[1] not in literal_to_list(Command)
+    ):
+        argv = (
+            argv_before_opts
+            + [argv_after_opts[0], "render"]
+            + argv_after_opts[1:]
+        )
+    elif argv_after_opts[0] == "template" and len(argv_after_opts) == 1:
+        argv = argv_before_opts + [argv_after_opts[0], "render", ""]
 
     parser = clack.Parser(description="The zettel note manager of the future.")
     # --- Global Options
     parser.add_argument(
         "-d",
         "--dir",
         dest="zettel_dir",
@@ -169,14 +203,22 @@
     action_open_parser.add_argument(
         "line_number",
         type=int,
         help=(
             "The line number that your editor cursor is currently located on."
         ),
     )
+    action_open_parser.add_argument(
+        "option_idx",
+        nargs="?",
+        help=(
+            "Used on a second 'action open' run to indicate which option was"
+            " selected."
+        ),
+    )
 
     # --- 'compile' command
     compile_parser = new_command(
         "compile", help="Compiles zorg (*.zo) files into zorc (*.zoc) files."
     )
     compile_parser.add_argument(
         "zo_path", help="Path to the zorg file you want to compile."
@@ -229,26 +271,14 @@
     query_parser.add_argument("query", help="The zorg query we will run.")
 
     # --- 'template' command
     template_parser = new_command(
         "template", help="Commands for managing .zot templates."
     )
     new_template_command = clack.new_command_factory(template_parser)
-    # --- 'template render' command
-    template_render_parser = new_template_command(
-        "render", help="Render a new .zo file using a .zot template."
-    )
-    template_render_parser.add_argument(
-        "template", type=Path, help="Path to the .zot template."
-    )
-    template_render_parser.add_argument(
-        "variables",
-        nargs="*",
-        help="A list of variable specs of the form of key=value.",
-    )
     # --- 'template init' command
     template_init_parser = new_template_command(
         "init", help="Initialize a new file using a zorg template."
     )
     template_init_parser.add_argument(
         "new_path",
         type=Path,
@@ -266,14 +296,28 @@
         ),
     )
     template_init_parser.add_argument(
         "variables",
         nargs="*",
         help="A list of variable specs of the form of key=value.",
     )
+    # --- 'template list' command
+    new_template_command("list", help="List all zorg template files.")
+    # --- 'template render' command
+    template_render_parser = new_template_command(
+        "render", help="Render a new .zo file using a .zot template."
+    )
+    template_render_parser.add_argument(
+        "template", type=Path, help="Path to the .zot template."
+    )
+    template_render_parser.add_argument(
+        "variables",
+        nargs="*",
+        help="A list of variable specs of the form of key=value.",
+    )
 
     args = parser.parse_args(argv[1:])
     kwargs = clack.filter_cli_args(args)
 
     _convert_variables_to_var_map(kwargs)
     _process_zo_paths(kwargs)
     _process_query(kwargs)
@@ -310,7 +354,9 @@
         var_map = {}
         for var_spec in kwargs["variables"]:
             k, v = var_spec.split("=")
             var_map[k] = v
         var_map = common.process_var_map(var_map)
         kwargs["var_map"] = var_map
         del kwargs["variables"]
+    elif kwargs["command"] == "render":
+        kwargs["var_map"] = {}
```

### Comparing `zettel_org-0.7.2/src/zorg/app/runners/__init__.py` & `zettel_org-0.7.3/src/zorg/app/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/src/zorg/app/runners/_run_compile.py` & `zettel_org-0.7.3/src/zorg/app/runners/_run_compile.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/src/zorg/app/runners/_run_db.py` & `zettel_org-0.7.3/src/zorg/app/runners/_run_db.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/src/zorg/app/runners/_run_edit.py` & `zettel_org-0.7.3/src/zorg/app/runners/_run_edit.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/src/zorg/domain/messages/commands.py` & `zettel_org-0.7.3/src/zorg/domain/messages/commands.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/src/zorg/domain/messages/events.py` & `zettel_org-0.7.3/src/zorg/domain/messages/events.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,11 +26,20 @@
 
     zettel_dir: Path
     zorg_file_path: Path
     new_notes: list[Note]
 
 
 @dataclass(frozen=True)
+class ModifiedZorgNotesEvent(Event):
+    """Broadcast when zorg notes should have their modify date updated."""
+
+    zettel_dir: Path
+    zorg_file_path: Path
+    modified_notes: list[Note]
+
+
+@dataclass(frozen=True)
 class DBModifiedEvent(Event):
     """Broadcast when the zorg database is done being initialized."""
 
     zettel_dir: Path
```

### Comparing `zettel_org-0.7.2/src/zorg/domain/models/_zorg_file.py` & `zettel_org-0.7.3/src/zorg/domain/models/_zorg_file.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,40 +12,44 @@
     from ..messages.events import Event
 
 
 @dataclass(frozen=True)
 class TodoPayload:
     """Extra fields that are added to ZorgNotes that are todos."""
 
-    priority: TodoPriorityType = "C"
+    priority: TodoPriorityType = "P2"
     status: NoteType = NoteType.OPEN_TODO
 
 
 @dataclass
 class Note:
     """A Zorg note."""
 
     body: str
 
     areas: list[str] = field(default_factory=lambda: [])
-    child_note_ids: list[int] = field(default_factory=lambda: [])
     contexts: list[str] = field(default_factory=lambda: [])
     create_date: dt.date = field(default_factory=dt.date.today)
     file_path: Optional[Path] = None
     line_no: Optional[int] = None
     links: list[str] = field(default_factory=lambda: [])
-    next_note_id: Optional[int] = None
-    parent_note_id: Optional[int] = None
+    modify_date: dt.date = field(default_factory=dt.date.today)
     people: list[str] = field(default_factory=lambda: [])
-    prev_note_id: Optional[int] = None
     projects: list[str] = field(default_factory=lambda: [])
     properties: dict[str, str] = field(default_factory=lambda: {})
     todo_payload: Optional[TodoPayload] = None
     zid: Optional[str] = None
 
+    def __eq__(self, other: object) -> bool:  # noqa: D105
+        return (
+            isinstance(other, Note)
+            and self.body == other.body
+            and self.todo_payload == other.todo_payload
+        )
+
 
 @dataclass
 class File:
     """A Zorg (i.e. *.zo) file."""
 
     path: Path
     has_errors: bool = False
```

### Comparing `zettel_org-0.7.2/src/zorg/domain/models/_zorg_query.py` & `zettel_org-0.7.3/src/zorg/domain/models/_zorg_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 class PropertyFilter:
     """Represents a single property filter (e.g. 'due:<=0d' or '!recur:*')."""
 
     key: str
     value: str = ""
     op: PropertyOperator = PropertyOperator.EXISTS
     value_type: PropertyValueType = PropertyValueType.STRING
+    negated: bool = False
 
 
 @dataclass(frozen=True)
 class DateRange:
     """Represents a range of dates."""
 
     start: dt.date
@@ -89,10 +90,11 @@
     """
 
     select: SelectType = field(default=SelectType.NOTE)
     where: Optional[WhereOrFilter] = None
     order_by: tuple[OrderByType, ...] = (
         OrderByType.NOTE_TYPE,
         OrderByType.PRIORITY,
-        OrderByType.DATE,
+        OrderByType.MODIFY_DATE,
+        OrderByType.CREATE_DATE,
     )
     group_by: tuple[GroupByType, ...] = tuple()
```

### Comparing `zettel_org-0.7.2/src/zorg/domain/types.py` & `zettel_org-0.7.3/src/zorg/domain/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,44 @@
 """Custom types used by zorg."""
 
 import abc
+import datetime as dt
 import enum
 from pathlib import Path
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    Final,
     Generic,
     Literal,
     Mapping,
     Optional,
     Pattern,
     Protocol,
     Sequence,
     TypeVar,
 )
 
 from sqlalchemy.future import Engine
-from typist import Comparable, assert_never
+from typist import assert_never
 
 
 if TYPE_CHECKING:
     from .models import Note, TodoPayload
 
 
 E = TypeVar("E")
 T = TypeVar("T")
 
 
-KeyFunc = Callable[["Note"], Comparable]
+KeyFunc = Callable[["Note"], str]
 FileGroupMapType = Mapping[str, Sequence[str]]
 TodoPriorityType = Literal[
-    "A",
-    "B",
-    "C",
-    "D",
-    "E",
-    "F",
-    "G",
-    "H",
-    "I",
-    "J",
-    "K",
-    "L",
-    "M",
-    "N",
-    "O",
-    "P",
-    "Q",
-    "R",
-    "S",
-    "T",
-    "U",
-    "V",
-    "W",
-    "X",
-    "Y",
-    "Z",
+    "P0", "P1", "P2", "P3", "P4", "P5", "P6", "P7", "P8", "P9"
 ]
 TemplatePatternMapType = Mapping[Pattern, Path]
 VarMapType = Mapping[str, Any]
 TodoStatusPrefixChar = Literal["o", "x", "~", "<", ">"]
 
 
 class NoteType(enum.Enum):
@@ -72,26 +49,27 @@
     CLOSED_TODO = enum.auto()  # x
     CANCELED_TODO = enum.auto()  # ~
     BLOCKED_TODO = enum.auto()  # <
     PARENT_TODO = enum.auto()  # >
 
     def to_header_label(self) -> str:
         """Converts to a header label that can be used by GROUP BY."""
+        open_todos_label: Final = "1 | OPEN TODOS"
         if self is NoteType.BASIC:
-            return "Notes"
+            return "4 | NOTES"
         elif self is NoteType.OPEN_TODO:
-            return "Open Todos"
+            return open_todos_label
         elif self is NoteType.CLOSED_TODO:
-            return "Done Todos"
+            return "2 | DONE TODOS"
         elif self is NoteType.CANCELED_TODO:
-            return "Canceled Todos"
+            return "3 | CANCELED TODOS"
         elif self is NoteType.BLOCKED_TODO:
-            return "Blocked Todos"
+            return open_todos_label
         elif self is NoteType.PARENT_TODO:
-            return "Parent Todos"
+            return open_todos_label
         else:
             assert_never(self)
 
     def to_prefix_char(self) -> str:  # pyright: reportGeneralTypeIssues=false
         """Converts a note's type to its corresponding prefix character."""
         if self is NoteType.BASIC:
             return "-"
@@ -149,64 +127,85 @@
     """Represents a single GROUP BY field for zorg queries."""
 
     AREA = enum.auto()
     CONTEXT = enum.auto()
     FILE = enum.auto()
     NOTE_TYPE = enum.auto()
     PERSON = enum.auto()
+    PRIORITY = enum.auto()
     PROJECT = enum.auto()
 
     @property
     def keyfunc(self) -> KeyFunc:
-        """Returns a callable that can be used to group/sort notes."""
+        """Returns a callable that can be used to group notes."""
         if self is GroupByType.AREA:
-            return _tag_keyfunc_factory("areas", "#")
+            return _to_comparable_tag_factory("areas", "#")
         elif self is GroupByType.CONTEXT:
-            return _tag_keyfunc_factory("contexts", "@")
+            return _to_comparable_tag_factory("contexts", "@")
         elif self is GroupByType.FILE:
             return lambda note: _to_comparable_file(note.file_path)
         elif self is GroupByType.NOTE_TYPE:
             return lambda note: _to_comparable_note_type(note.todo_payload)
         elif self is GroupByType.PERSON:
-            return _tag_keyfunc_factory("people", "%")
+            return _to_comparable_tag_factory("people", "%")
         elif self is GroupByType.PROJECT:
-            return _tag_keyfunc_factory("projects", "+")
+            return _to_comparable_tag_factory("projects", "+")
+        elif self is GroupByType.PRIORITY:
+            return lambda note: _to_comparable_priority(note.todo_payload)
         else:
             assert_never(self)
 
 
 class OrderByType(enum.Enum):
     """Represents a single ORDER BY field for zorg queries."""
 
-    DATE = enum.auto()
+    CREATE_DATE = enum.auto()
+    MODIFY_DATE = enum.auto()
     NOTE_TYPE = enum.auto()
     PRIORITY = enum.auto()
 
+    @property
+    def keyfunc(self) -> KeyFunc:
+        """Returns a callable that can be used sort notes."""
+        if self is OrderByType.CREATE_DATE:
+            return lambda note: _to_comparable_date(note.create_date)
+        elif self is OrderByType.MODIFY_DATE:
+            return lambda note: _to_comparable_date(note.modify_date)
+        elif self is OrderByType.NOTE_TYPE:
+            return lambda note: _to_comparable_note_type(note.todo_payload)
+        elif self is OrderByType.PRIORITY:
+            return lambda note: _to_comparable_priority(note.todo_payload)
+        else:
+            assert_never(self)
+
 
 class SelectType(enum.Enum):
     """A zorg query (S)ELECT."""
 
-    AREA = enum.auto()
-    CONTEXT = enum.auto()
+    # Select all notes in block.
+    BLOCK = enum.auto()
+
+    # Select file paths.
     FILE = enum.auto()
+
+    # Select a note.
     NOTE = enum.auto()
+
+    # Select tags.
+    AREA = enum.auto()
+    CONTEXT = enum.auto()
     PERSON = enum.auto()
     PROJECT = enum.auto()
 
 
 class PropertyOperator(enum.Enum):
-    """Used to determine what kind of metatag constraint has been specified."""
+    """Used to determine what kind of property constraint has been specified."""
 
-    # exists / not exists
     EXISTS = enum.auto()
-    NOT_EXISTS = enum.auto()
-
-    # comparison operators
     EQ = enum.auto()
-    NE = enum.auto()
     LT = enum.auto()
     LE = enum.auto()
     GT = enum.auto()
     GE = enum.auto()
 
 
 class PropertyValueType(enum.Enum):
@@ -232,20 +231,33 @@
 def _to_comparable_note_type(todo_payload: Optional["TodoPayload"]) -> str:
     if todo_payload is None:
         return NoteType.BASIC.to_header_label()
     else:
         return todo_payload.status.to_header_label()
 
 
+def _to_comparable_priority(
+    todo_payload: Optional["TodoPayload"],
+) -> TodoPriorityType:
+    if todo_payload is None:
+        return "P9"
+    else:
+        return todo_payload.priority
+
+
 def _to_comparable_file(file_path: Optional[Path]) -> str:
     assert file_path is not None
     link_name = str(file_path).replace(".zo", "")
     return f"[[{link_name}]]"
 
 
-def _tag_keyfunc_factory(attr: str, tag_symbol: str) -> KeyFunc:
+def _to_comparable_date(date: dt.date) -> str:
+    return date.strftime("%Y%m%d")
+
+
+def _to_comparable_tag_factory(attr: str, tag_symbol: str) -> KeyFunc:
     def _keyfunc(note: "Note") -> str:
-        return " ".join(
+        return " | ".join(
             f"{tag_symbol}{tag}" for tag in sorted(getattr(note, attr))
         )
 
     return _keyfunc
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/CommonLexerRules.g4` & `zettel_org-0.7.3/src/zorg/grammar/CommonLexerRules.g4`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 lexer grammar CommonLexerRules;
 
 //// lexer rules
-NL : '\r'? '\n' ;
-LOWER_O : 'o' ;
-LOWER_X : 'x' ;
-DATE : '2' NUM NUM NUM DASH FIRST_M_NUM NUM DASH FIRST_D_NUM NUM ;
-TIME : ('0' | '1' | '2') NUM ('0' | '1' | '2' | '3' | '4' | '5') NUM ;
-ID : ALPHANUM (ALPHANUM|UNDERSCORE)* ;
-ZID : NUM NUM FIRST_M_NUM NUM FIRST_D_NUM NUM HASH ZID_CHAR ZID_CHAR ZID_CHAR? ;
-NUM_ID : NUM (ALPHANUM|UNDERSCORE)* ;
-TWO_SPACE_DASH : '  -' ;
-FOUR_SPACE_DASH : '    -' ;
-SYMBOL : [^[\],?!;|=\\`{}$&] ;
-DASH : '-' ;
-DOT : '.' ;
-FSLASH : '/' ;
-UNDERSCORE : '_' ;
-COLON : ':' ;
-SPACE : ' ' ;
-LPAREN : '(' ;
-RPAREN : ')' ;
-HASH : '#' ;
-AT_SIGN : '@' ;
-PLUS : '+' ;
-PERCENT : '%' ;
-SQUOTE : '\'' ;
-DQUOTE : '"' ;
-TILDE : '~' ;
-STAR : '*' ;
-LANGLE : '<' ;
-RANGLE : '>' ;
+NL                : '\r'? '\n' ;
+LOWER_O           : 'o' ;
+LOWER_X           : 'x' ;
+DATE              : '2' NUM NUM NUM DASH FIRST_M_NUM NUM DASH FIRST_D_NUM NUM ;
+TIME              : ('0' | '1' | '2') NUM ('0' | '1' | '2' | '3' | '4' | '5') NUM ;
+CREATE_RANGE_HEAD : HAT SHORT_DATE ;
+MODIFY_RANGE_HEAD : DOLLAR SHORT_DATE ;
+DATE_RANGE_TAIL   : COLON SHORT_DATE ;
+PRIORITY          : 'P' NUM ;
+ID                : ALPHANUM (ALPHANUM|UNDERSCORE)* ;
+ZID               : SHORT_DATE HASH ZID_CHAR ZID_CHAR ZID_CHAR? ;
+SHORT_DATE        : NUM NUM FIRST_M_NUM NUM FIRST_D_NUM NUM ;
+NUM_ID            : NUM (ALPHANUM|UNDERSCORE)* ;
+TWO_SPACE_DASH    : '  -' ;
+FOUR_SPACE_DASH   : '    -' ;
+SYMBOL            : [[\],?!;|=\\`{}&] ;
+DOLLAR            : '$' ;
+HAT               : '^' ;
+DASH              : '-' ;
+DOT               : '.' ;
+FSLASH            : '/' ;
+UNDERSCORE        : '_' ;
+SPACE             : ' ' ;
+LPAREN            : '(' ;
+RPAREN            : ')' ;
+HASH              : '#' ;
+AT_SIGN           : '@' ;
+PLUS              : '+' ;
+PERCENT           : '%' ;
+SQUOTE            : '\'' ;
+DQUOTE            : '"' ;
+TILDE             : '~' ;
+STAR              : '*' ;
+LANGLE            : '<' ;
+RANGLE            : '>' ;
+COLON             : ':' ;
 
 //// fragments
+//
+// ZID_CHAR is any digit OR any letter NOT in ('I', 'O', 'j', 'l')
 fragment UPPER_LETTER : 'A'..'Z' ;
 fragment LOWER_LETTER : 'a'..'z' ;
-// ZID_CHAR: Any digit OR any letter NOT in ('I', 'O', 'j', 'l')
-fragment ZID_CHAR : NUM | 'A'..'H' | 'J'..'N' | 'P'..'Z' | 'a'..'i' | 'k' | 'm'..'z' ;
+fragment ZID_CHAR     : NUM | 'A'..'H' | 'J'..'N' | 'P'..'Z' | 'a'..'i' | 'k' | 'm'..'z' ;
 fragment NUM          : '0'..'9' ;
-fragment FIRST_D_NUM : '0' | '1' | '2' | '3' ;
-fragment FIRST_M_NUM : '0' | '1' ;
+fragment FIRST_D_NUM  : '0' | '1' | '2' | '3' ;
+fragment FIRST_M_NUM  : '0' | '1' ;
 fragment ALPHA        : UPPER_LETTER | LOWER_LETTER ;
 fragment ALPHANUM     : ALPHA | NUM ;
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/ZorgFile.g4` & `zettel_org-0.7.3/src/zorg/grammar/ZorgFile.g4`

 * *Files 10% similar despite different names*

```diff
@@ -2,65 +2,65 @@
 
 import CommonLexerRules;
 
 //// parser rules
 prog : head body? EOF ;
 
 // header and body
-head       : comment+ ;
-comment    : HASH space_atoms? NL ;
-body : NL+ block* h2_section* h1_section* ;
+head    : comment+ ;
+comment : HASH space_atoms? NL ;
+body    : NL+ block* h2_section* h1_section* ;
 
 // blocks
 block       : item+ NL* ;
 item        : todo | note | footnote | comment ;
 footnote    : ref COLON space_atoms NL ;
 
 // notes
-note        : DASH base_note subnote* ;
-base_note   : id_note_body NL ;
-id_note_body : (SPACE zid)? note_body ;
-note_body   : space_atoms (NL SPACE+ space_atoms)* ;
-subnote     : TWO_SPACE_DASH base_note subsubnote*;
-subsubnote  : FOUR_SPACE_DASH base_note ;
+note         : DASH base_note subnote* ;
+base_note    : id_note_body NL ;
+id_note_body : note_body ;
+note_body    : space_atoms (NL SPACE+ space_atoms)* ;
+subnote      : TWO_SPACE_DASH base_note subsubnote*;
+subsubnote   : FOUR_SPACE_DASH base_note ;
 
 // todos
 todo        : base_todo subnote* ;
 base_todo   : todo_prefix (SPACE priority)? id_note_body NL ;
 todo_prefix : (LOWER_O | x_or_tilde | LANGLE | RANGLE) ;
 x_or_tilde  : (LOWER_X | TILDE) (COLON time)? ;
-priority    : '[' HASH ID ']' ;
-
-// Zorg YYMMDD#XX IDs
-zid : ZID ;
+priority    : PRIORITY ;
 
 // atoms
 space_atoms : space_atom+ ;
 space_atom  : SPACE (SQUOTE non_tag_symbol)? (non_tag_symbol | DQUOTE)* (atom | quoted)? (any_symbol (any_symbol | id)*)? ref? ;
-atom        : tag_symbol | tag | link | property | id_group | ref | zid | priority ;
+atom        : tag_symbol | tag | link | property | id_group | ref | priority ;
+
+// Zorg YYMMDD#XX IDs
+zid : ZID  ;
 
 // property
 property    : ID COLON COLON id_group ;
 id_group    : id (id_symbol+ id)* ;
-id          : ID | NUM_ID | date | time | LOWER_O | LOWER_X ;
+id          : ID | NUM_ID | DATE_RANGE_TAIL | PRIORITY | date | time | zid | LOWER_O | LOWER_X ;
 date        : DATE ;
 time        : TIME ;
 
 // symbols
-any_symbol     : SQUOTE | DQUOTE | non_tag_symbol | tag_symbol | id_symbol ;
+any_symbol     : SQUOTE | DQUOTE | HAT | DOLLAR | non_tag_symbol | tag_symbol | id_symbol ;
 non_tag_symbol : LANGLE | RANGLE | STAR | TILDE | SYMBOL | LPAREN | RPAREN | UNDERSCORE ;
 id_symbol      : DASH | DOT | FSLASH | COLON ;
 tag_symbol     : HASH | AT_SIGN | PERCENT | PLUS ;
 
 // tag
-tag        : area | context | person | project ;
-area       : HASH ID ;
-context    : AT_SIGN ID ;
-person     : PERCENT ID ;
-project    : PLUS ID ;
+tag     : area | context | person | project ;
+area    : HASH ID ;
+context : AT_SIGN ID ;
+person  : PERCENT ID ;
+project : PLUS ID ;
 
 // quotes and links
 quoted     : (SQUOTE (atom | priority | '[[' | ']]')+ SQUOTE | DQUOTE atom+ DQUOTE) ;
 link       : '[[' id_group ']]' ;
 ref        : '[' id_group ']' ;
 
 // sections
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFile.interp` & `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFile.interp`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,96 @@
 token literal names:
 null
-'['
-']'
 '[['
 ']]'
+'['
+']'
 '======='
 '*****'
 null
 'o'
 'x'
 null
 null
 null
 null
 null
+null
+null
+null
+null
+null
 '  -'
 '    -'
 null
+'$'
+'^'
 '-'
 '.'
 '/'
 '_'
-':'
 ' '
 '('
 ')'
 '#'
 '@'
 '+'
 '%'
 '\''
 '"'
 '~'
 '*'
 '<'
 '>'
+':'
 
 token symbolic names:
 null
 null
 null
 null
 null
 null
 null
 NL
 LOWER_O
 LOWER_X
 DATE
 TIME
+CREATE_RANGE_HEAD
+MODIFY_RANGE_HEAD
+DATE_RANGE_TAIL
+PRIORITY
 ID
 ZID
+SHORT_DATE
 NUM_ID
 TWO_SPACE_DASH
 FOUR_SPACE_DASH
 SYMBOL
+DOLLAR
+HAT
 DASH
 DOT
 FSLASH
 UNDERSCORE
-COLON
 SPACE
 LPAREN
 RPAREN
 HASH
 AT_SIGN
 PLUS
 PERCENT
 SQUOTE
 DQUOTE
 TILDE
 STAR
 LANGLE
 RANGLE
+COLON
 
 rule names:
 prog
 head
 comment
 body
 block
@@ -89,18 +103,18 @@
 subnote
 subsubnote
 todo
 base_todo
 todo_prefix
 x_or_tilde
 priority
-zid
 space_atoms
 space_atom
 atom
+zid
 property
 id_group
 id
 date
 time
 any_symbol
 non_tag_symbol
@@ -122,8 +136,8 @@
 h2_header
 h3_header
 h4_header
 eol
 
 
 atn:
-[4, 1, 35, 473, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 2, 47, 7, 47, 1, 0, 1, 0, 3, 0, 99, 8, 0, 1, 0, 1, 0, 1, 1, 4, 1, 104, 8, 1, 11, 1, 12, 1, 105, 1, 2, 1, 2, 3, 2, 110, 8, 2, 1, 2, 1, 2, 1, 3, 4, 3, 115, 8, 3, 11, 3, 12, 3, 116, 1, 3, 5, 3, 120, 8, 3, 10, 3, 12, 3, 123, 9, 3, 1, 3, 5, 3, 126, 8, 3, 10, 3, 12, 3, 129, 9, 3, 1, 3, 5, 3, 132, 8, 3, 10, 3, 12, 3, 135, 9, 3, 1, 4, 4, 4, 138, 8, 4, 11, 4, 12, 4, 139, 1, 4, 5, 4, 143, 8, 4, 10, 4, 12, 4, 146, 9, 4, 1, 5, 1, 5, 1, 5, 1, 5, 3, 5, 152, 8, 5, 1, 6, 1, 6, 1, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 7, 5, 7, 162, 8, 7, 10, 7, 12, 7, 165, 9, 7, 1, 8, 1, 8, 1, 8, 1, 9, 1, 9, 3, 9, 172, 8, 9, 1, 9, 1, 9, 1, 10, 1, 10, 1, 10, 4, 10, 179, 8, 10, 11, 10, 12, 10, 180, 1, 10, 5, 10, 184, 8, 10, 10, 10, 12, 10, 187, 9, 10, 1, 11, 1, 11, 1, 11, 5, 11, 192, 8, 11, 10, 11, 12, 11, 195, 9, 11, 1, 12, 1, 12, 1, 12, 1, 13, 1, 13, 5, 13, 202, 8, 13, 10, 13, 12, 13, 205, 9, 13, 1, 14, 1, 14, 1, 14, 3, 14, 210, 8, 14, 1, 14, 1, 14, 1, 14, 1, 15, 1, 15, 1, 15, 1, 15, 3, 15, 219, 8, 15, 1, 16, 1, 16, 1, 16, 3, 16, 224, 8, 16, 1, 17, 1, 17, 1, 17, 1, 17, 1, 17, 1, 18, 1, 18, 1, 19, 4, 19, 234, 8, 19, 11, 19, 12, 19, 235, 1, 20, 1, 20, 1, 20, 3, 20, 241, 8, 20, 1, 20, 1, 20, 5, 20, 245, 8, 20, 10, 20, 12, 20, 248, 9, 20, 1, 20, 1, 20, 3, 20, 252, 8, 20, 1, 20, 1, 20, 1, 20, 5, 20, 257, 8, 20, 10, 20, 12, 20, 260, 9, 20, 3, 20, 262, 8, 20, 1, 20, 3, 20, 265, 8, 20, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 1, 21, 3, 21, 275, 8, 21, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 23, 1, 23, 4, 23, 284, 8, 23, 11, 23, 12, 23, 285, 1, 23, 1, 23, 5, 23, 290, 8, 23, 10, 23, 12, 23, 293, 9, 23, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 3, 24, 301, 8, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 3, 27, 312, 8, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 31, 1, 31, 3, 31, 324, 8, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 1, 35, 1, 35, 1, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 36, 4, 36, 343, 8, 36, 11, 36, 12, 36, 344, 1, 36, 1, 36, 1, 36, 4, 36, 350, 8, 36, 11, 36, 12, 36, 351, 1, 36, 1, 36, 3, 36, 356, 8, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 1, 38, 1, 38, 1, 39, 1, 39, 5, 39, 368, 8, 39, 10, 39, 12, 39, 371, 9, 39, 1, 39, 5, 39, 374, 8, 39, 10, 39, 12, 39, 377, 9, 39, 1, 39, 3, 39, 380, 8, 39, 1, 39, 5, 39, 383, 8, 39, 10, 39, 12, 39, 386, 9, 39, 1, 40, 1, 40, 5, 40, 390, 8, 40, 10, 40, 12, 40, 393, 9, 40, 1, 40, 5, 40, 396, 8, 40, 10, 40, 12, 40, 399, 9, 40, 1, 40, 3, 40, 402, 8, 40, 1, 40, 5, 40, 405, 8, 40, 10, 40, 12, 40, 408, 9, 40, 1, 41, 1, 41, 5, 41, 412, 8, 41, 10, 41, 12, 41, 415, 9, 41, 1, 41, 5, 41, 418, 8, 41, 10, 41, 12, 41, 421, 9, 41, 1, 41, 3, 41, 424, 8, 41, 1, 41, 5, 41, 427, 8, 41, 10, 41, 12, 41, 430, 9, 41, 1, 42, 1, 42, 5, 42, 434, 8, 42, 10, 42, 12, 42, 437, 9, 42, 1, 42, 5, 42, 440, 8, 42, 10, 42, 12, 42, 443, 9, 42, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 44, 1, 44, 1, 44, 1, 44, 1, 45, 1, 45, 1, 45, 1, 45, 1, 46, 1, 46, 1, 46, 1, 46, 1, 46, 1, 46, 1, 47, 1, 47, 1, 47, 0, 0, 48, 0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 94, 0, 5, 2, 0, 9, 9, 32, 32, 4, 0, 17, 17, 21, 21, 24, 25, 32, 35, 2, 0, 18, 20, 22, 22, 1, 0, 26, 29, 1, 1, 7, 7, 498, 0, 96, 1, 0, 0, 0, 2, 103, 1, 0, 0, 0, 4, 107, 1, 0, 0, 0, 6, 114, 1, 0, 0, 0, 8, 137, 1, 0, 0, 0, 10, 151, 1, 0, 0, 0, 12, 153, 1, 0, 0, 0, 14, 158, 1, 0, 0, 0, 16, 166, 1, 0, 0, 0, 18, 171, 1, 0, 0, 0, 20, 175, 1, 0, 0, 0, 22, 188, 1, 0, 0, 0, 24, 196, 1, 0, 0, 0, 26, 199, 1, 0, 0, 0, 28, 206, 1, 0, 0, 0, 30, 218, 1, 0, 0, 0, 32, 220, 1, 0, 0, 0, 34, 225, 1, 0, 0, 0, 36, 230, 1, 0, 0, 0, 38, 233, 1, 0, 0, 0, 40, 237, 1, 0, 0, 0, 42, 274, 1, 0, 0, 0, 44, 276, 1, 0, 0, 0, 46, 281, 1, 0, 0, 0, 48, 300, 1, 0, 0, 0, 50, 302, 1, 0, 0, 0, 52, 304, 1, 0, 0, 0, 54, 311, 1, 0, 0, 0, 56, 313, 1, 0, 0, 0, 58, 315, 1, 0, 0, 0, 60, 317, 1, 0, 0, 0, 62, 323, 1, 0, 0, 0, 64, 325, 1, 0, 0, 0, 66, 328, 1, 0, 0, 0, 68, 331, 1, 0, 0, 0, 70, 334, 1, 0, 0, 0, 72, 355, 1, 0, 0, 0, 74, 357, 1, 0, 0, 0, 76, 361, 1, 0, 0, 0, 78, 365, 1, 0, 0, 0, 80, 387, 1, 0, 0, 0, 82, 409, 1, 0, 0, 0, 84, 431, 1, 0, 0, 0, 86, 444, 1, 0, 0, 0, 88, 456, 1, 0, 0, 0, 90, 460, 1, 0, 0, 0, 92, 464, 1, 0, 0, 0, 94, 470, 1, 0, 0, 0, 96, 98, 3, 2, 1, 0, 97, 99, 3, 6, 3, 0, 98, 97, 1, 0, 0, 0, 98, 99, 1, 0, 0, 0, 99, 100, 1, 0, 0, 0, 100, 101, 5, 0, 0, 1, 101, 1, 1, 0, 0, 0, 102, 104, 3, 4, 2, 0, 103, 102, 1, 0, 0, 0, 104, 105, 1, 0, 0, 0, 105, 103, 1, 0, 0, 0, 105, 106, 1, 0, 0, 0, 106, 3, 1, 0, 0, 0, 107, 109, 5, 26, 0, 0, 108, 110, 3, 38, 19, 0, 109, 108, 1, 0, 0, 0, 109, 110, 1, 0, 0, 0, 110, 111, 1, 0, 0, 0, 111, 112, 5, 7, 0, 0, 112, 5, 1, 0, 0, 0, 113, 115, 5, 7, 0, 0, 114, 113, 1, 0, 0, 0, 115, 116, 1, 0, 0, 0, 116, 114, 1, 0, 0, 0, 116, 117, 1, 0, 0, 0, 117, 121, 1, 0, 0, 0, 118, 120, 3, 8, 4, 0, 119, 118, 1, 0, 0, 0, 120, 123, 1, 0, 0, 0, 121, 119, 1, 0, 0, 0, 121, 122, 1, 0, 0, 0, 122, 127, 1, 0, 0, 0, 123, 121, 1, 0, 0, 0, 124, 126, 3, 80, 40, 0, 125, 124, 1, 0, 0, 0, 126, 129, 1, 0, 0, 0, 127, 125, 1, 0, 0, 0, 127, 128, 1, 0, 0, 0, 128, 133, 1, 0, 0, 0, 129, 127, 1, 0, 0, 0, 130, 132, 3, 78, 39, 0, 131, 130, 1, 0, 0, 0, 132, 135, 1, 0, 0, 0, 133, 131, 1, 0, 0, 0, 133, 134, 1, 0, 0, 0, 134, 7, 1, 0, 0, 0, 135, 133, 1, 0, 0, 0, 136, 138, 3, 10, 5, 0, 137, 136, 1, 0, 0, 0, 138, 139, 1, 0, 0, 0, 139, 137, 1, 0, 0, 0, 139, 140, 1, 0, 0, 0, 140, 144, 1, 0, 0, 0, 141, 143, 5, 7, 0, 0, 142, 141, 1, 0, 0, 0, 143, 146, 1, 0, 0, 0, 144, 142, 1, 0, 0, 0, 144, 145, 1, 0, 0, 0, 145, 9, 1, 0, 0, 0, 146, 144, 1, 0, 0, 0, 147, 152, 3, 26, 13, 0, 148, 152, 3, 14, 7, 0, 149, 152, 3, 12, 6, 0, 150, 152, 3, 4, 2, 0, 151, 147, 1, 0, 0, 0, 151, 148, 1, 0, 0, 0, 151, 149, 1, 0, 0, 0, 151, 150, 1, 0, 0, 0, 152, 11, 1, 0, 0, 0, 153, 154, 3, 76, 38, 0, 154, 155, 5, 22, 0, 0, 155, 156, 3, 38, 19, 0, 156, 157, 5, 7, 0, 0, 157, 13, 1, 0, 0, 0, 158, 159, 5, 18, 0, 0, 159, 163, 3, 16, 8, 0, 160, 162, 3, 22, 11, 0, 161, 160, 1, 0, 0, 0, 162, 165, 1, 0, 0, 0, 163, 161, 1, 0, 0, 0, 163, 164, 1, 0, 0, 0, 164, 15, 1, 0, 0, 0, 165, 163, 1, 0, 0, 0, 166, 167, 3, 18, 9, 0, 167, 168, 5, 7, 0, 0, 168, 17, 1, 0, 0, 0, 169, 170, 5, 23, 0, 0, 170, 172, 3, 36, 18, 0, 171, 169, 1, 0, 0, 0, 171, 172, 1, 0, 0, 0, 172, 173, 1, 0, 0, 0, 173, 174, 3, 20, 10, 0, 174, 19, 1, 0, 0, 0, 175, 185, 3, 38, 19, 0, 176, 178, 5, 7, 0, 0, 177, 179, 5, 23, 0, 0, 178, 177, 1, 0, 0, 0, 179, 180, 1, 0, 0, 0, 180, 178, 1, 0, 0, 0, 180, 181, 1, 0, 0, 0, 181, 182, 1, 0, 0, 0, 182, 184, 3, 38, 19, 0, 183, 176, 1, 0, 0, 0, 184, 187, 1, 0, 0, 0, 185, 183, 1, 0, 0, 0, 185, 186, 1, 0, 0, 0, 186, 21, 1, 0, 0, 0, 187, 185, 1, 0, 0, 0, 188, 189, 5, 15, 0, 0, 189, 193, 3, 16, 8, 0, 190, 192, 3, 24, 12, 0, 191, 190, 1, 0, 0, 0, 192, 195, 1, 0, 0, 0, 193, 191, 1, 0, 0, 0, 193, 194, 1, 0, 0, 0, 194, 23, 1, 0, 0, 0, 195, 193, 1, 0, 0, 0, 196, 197, 5, 16, 0, 0, 197, 198, 3, 16, 8, 0, 198, 25, 1, 0, 0, 0, 199, 203, 3, 28, 14, 0, 200, 202, 3, 22, 11, 0, 201, 200, 1, 0, 0, 0, 202, 205, 1, 0, 0, 0, 203, 201, 1, 0, 0, 0, 203, 204, 1, 0, 0, 0, 204, 27, 1, 0, 0, 0, 205, 203, 1, 0, 0, 0, 206, 209, 3, 30, 15, 0, 207, 208, 5, 23, 0, 0, 208, 210, 3, 34, 17, 0, 209, 207, 1, 0, 0, 0, 209, 210, 1, 0, 0, 0, 210, 211, 1, 0, 0, 0, 211, 212, 3, 18, 9, 0, 212, 213, 5, 7, 0, 0, 213, 29, 1, 0, 0, 0, 214, 219, 5, 8, 0, 0, 215, 219, 3, 32, 16, 0, 216, 219, 5, 34, 0, 0, 217, 219, 5, 35, 0, 0, 218, 214, 1, 0, 0, 0, 218, 215, 1, 0, 0, 0, 218, 216, 1, 0, 0, 0, 218, 217, 1, 0, 0, 0, 219, 31, 1, 0, 0, 0, 220, 223, 7, 0, 0, 0, 221, 222, 5, 22, 0, 0, 222, 224, 3, 52, 26, 0, 223, 221, 1, 0, 0, 0, 223, 224, 1, 0, 0, 0, 224, 33, 1, 0, 0, 0, 225, 226, 5, 1, 0, 0, 226, 227, 5, 26, 0, 0, 227, 228, 5, 12, 0, 0, 228, 229, 5, 2, 0, 0, 229, 35, 1, 0, 0, 0, 230, 231, 5, 13, 0, 0, 231, 37, 1, 0, 0, 0, 232, 234, 3, 40, 20, 0, 233, 232, 1, 0, 0, 0, 234, 235, 1, 0, 0, 0, 235, 233, 1, 0, 0, 0, 235, 236, 1, 0, 0, 0, 236, 39, 1, 0, 0, 0, 237, 240, 5, 23, 0, 0, 238, 239, 5, 30, 0, 0, 239, 241, 3, 56, 28, 0, 240, 238, 1, 0, 0, 0, 240, 241, 1, 0, 0, 0, 241, 246, 1, 0, 0, 0, 242, 245, 3, 56, 28, 0, 243, 245, 5, 31, 0, 0, 244, 242, 1, 0, 0, 0, 244, 243, 1, 0, 0, 0, 245, 248, 1, 0, 0, 0, 246, 244, 1, 0, 0, 0, 246, 247, 1, 0, 0, 0, 247, 251, 1, 0, 0, 0, 248, 246, 1, 0, 0, 0, 249, 252, 3, 42, 21, 0, 250, 252, 3, 72, 36, 0, 251, 249, 1, 0, 0, 0, 251, 250, 1, 0, 0, 0, 251, 252, 1, 0, 0, 0, 252, 261, 1, 0, 0, 0, 253, 258, 3, 54, 27, 0, 254, 257, 3, 54, 27, 0, 255, 257, 3, 48, 24, 0, 256, 254, 1, 0, 0, 0, 256, 255, 1, 0, 0, 0, 257, 260, 1, 0, 0, 0, 258, 256, 1, 0, 0, 0, 258, 259, 1, 0, 0, 0, 259, 262, 1, 0, 0, 0, 260, 258, 1, 0, 0, 0, 261, 253, 1, 0, 0, 0, 261, 262, 1, 0, 0, 0, 262, 264, 1, 0, 0, 0, 263, 265, 3, 76, 38, 0, 264, 263, 1, 0, 0, 0, 264, 265, 1, 0, 0, 0, 265, 41, 1, 0, 0, 0, 266, 275, 3, 60, 30, 0, 267, 275, 3, 62, 31, 0, 268, 275, 3, 74, 37, 0, 269, 275, 3, 44, 22, 0, 270, 275, 3, 46, 23, 0, 271, 275, 3, 76, 38, 0, 272, 275, 3, 36, 18, 0, 273, 275, 3, 34, 17, 0, 274, 266, 1, 0, 0, 0, 274, 267, 1, 0, 0, 0, 274, 268, 1, 0, 0, 0, 274, 269, 1, 0, 0, 0, 274, 270, 1, 0, 0, 0, 274, 271, 1, 0, 0, 0, 274, 272, 1, 0, 0, 0, 274, 273, 1, 0, 0, 0, 275, 43, 1, 0, 0, 0, 276, 277, 5, 12, 0, 0, 277, 278, 5, 22, 0, 0, 278, 279, 5, 22, 0, 0, 279, 280, 3, 46, 23, 0, 280, 45, 1, 0, 0, 0, 281, 291, 3, 48, 24, 0, 282, 284, 3, 58, 29, 0, 283, 282, 1, 0, 0, 0, 284, 285, 1, 0, 0, 0, 285, 283, 1, 0, 0, 0, 285, 286, 1, 0, 0, 0, 286, 287, 1, 0, 0, 0, 287, 288, 3, 48, 24, 0, 288, 290, 1, 0, 0, 0, 289, 283, 1, 0, 0, 0, 290, 293, 1, 0, 0, 0, 291, 289, 1, 0, 0, 0, 291, 292, 1, 0, 0, 0, 292, 47, 1, 0, 0, 0, 293, 291, 1, 0, 0, 0, 294, 301, 5, 12, 0, 0, 295, 301, 5, 14, 0, 0, 296, 301, 3, 50, 25, 0, 297, 301, 3, 52, 26, 0, 298, 301, 5, 8, 0, 0, 299, 301, 5, 9, 0, 0, 300, 294, 1, 0, 0, 0, 300, 295, 1, 0, 0, 0, 300, 296, 1, 0, 0, 0, 300, 297, 1, 0, 0, 0, 300, 298, 1, 0, 0, 0, 300, 299, 1, 0, 0, 0, 301, 49, 1, 0, 0, 0, 302, 303, 5, 10, 0, 0, 303, 51, 1, 0, 0, 0, 304, 305, 5, 11, 0, 0, 305, 53, 1, 0, 0, 0, 306, 312, 5, 30, 0, 0, 307, 312, 5, 31, 0, 0, 308, 312, 3, 56, 28, 0, 309, 312, 3, 60, 30, 0, 310, 312, 3, 58, 29, 0, 311, 306, 1, 0, 0, 0, 311, 307, 1, 0, 0, 0, 311, 308, 1, 0, 0, 0, 311, 309, 1, 0, 0, 0, 311, 310, 1, 0, 0, 0, 312, 55, 1, 0, 0, 0, 313, 314, 7, 1, 0, 0, 314, 57, 1, 0, 0, 0, 315, 316, 7, 2, 0, 0, 316, 59, 1, 0, 0, 0, 317, 318, 7, 3, 0, 0, 318, 61, 1, 0, 0, 0, 319, 324, 3, 64, 32, 0, 320, 324, 3, 66, 33, 0, 321, 324, 3, 68, 34, 0, 322, 324, 3, 70, 35, 0, 323, 319, 1, 0, 0, 0, 323, 320, 1, 0, 0, 0, 323, 321, 1, 0, 0, 0, 323, 322, 1, 0, 0, 0, 324, 63, 1, 0, 0, 0, 325, 326, 5, 26, 0, 0, 326, 327, 5, 12, 0, 0, 327, 65, 1, 0, 0, 0, 328, 329, 5, 27, 0, 0, 329, 330, 5, 12, 0, 0, 330, 67, 1, 0, 0, 0, 331, 332, 5, 29, 0, 0, 332, 333, 5, 12, 0, 0, 333, 69, 1, 0, 0, 0, 334, 335, 5, 28, 0, 0, 335, 336, 5, 12, 0, 0, 336, 71, 1, 0, 0, 0, 337, 342, 5, 30, 0, 0, 338, 343, 3, 42, 21, 0, 339, 343, 3, 34, 17, 0, 340, 343, 5, 3, 0, 0, 341, 343, 5, 4, 0, 0, 342, 338, 1, 0, 0, 0, 342, 339, 1, 0, 0, 0, 342, 340, 1, 0, 0, 0, 342, 341, 1, 0, 0, 0, 343, 344, 1, 0, 0, 0, 344, 342, 1, 0, 0, 0, 344, 345, 1, 0, 0, 0, 345, 346, 1, 0, 0, 0, 346, 356, 5, 30, 0, 0, 347, 349, 5, 31, 0, 0, 348, 350, 3, 42, 21, 0, 349, 348, 1, 0, 0, 0, 350, 351, 1, 0, 0, 0, 351, 349, 1, 0, 0, 0, 351, 352, 1, 0, 0, 0, 352, 353, 1, 0, 0, 0, 353, 354, 5, 31, 0, 0, 354, 356, 1, 0, 0, 0, 355, 337, 1, 0, 0, 0, 355, 347, 1, 0, 0, 0, 356, 73, 1, 0, 0, 0, 357, 358, 5, 3, 0, 0, 358, 359, 3, 46, 23, 0, 359, 360, 5, 4, 0, 0, 360, 75, 1, 0, 0, 0, 361, 362, 5, 1, 0, 0, 362, 363, 3, 46, 23, 0, 363, 364, 5, 2, 0, 0, 364, 77, 1, 0, 0, 0, 365, 369, 3, 86, 43, 0, 366, 368, 5, 7, 0, 0, 367, 366, 1, 0, 0, 0, 368, 371, 1, 0, 0, 0, 369, 367, 1, 0, 0, 0, 369, 370, 1, 0, 0, 0, 370, 375, 1, 0, 0, 0, 371, 369, 1, 0, 0, 0, 372, 374, 3, 8, 4, 0, 373, 372, 1, 0, 0, 0, 374, 377, 1, 0, 0, 0, 375, 373, 1, 0, 0, 0, 375, 376, 1, 0, 0, 0, 376, 384, 1, 0, 0, 0, 377, 375, 1, 0, 0, 0, 378, 380, 5, 7, 0, 0, 379, 378, 1, 0, 0, 0, 379, 380, 1, 0, 0, 0, 380, 381, 1, 0, 0, 0, 381, 383, 3, 80, 40, 0, 382, 379, 1, 0, 0, 0, 383, 386, 1, 0, 0, 0, 384, 382, 1, 0, 0, 0, 384, 385, 1, 0, 0, 0, 385, 79, 1, 0, 0, 0, 386, 384, 1, 0, 0, 0, 387, 391, 3, 88, 44, 0, 388, 390, 5, 7, 0, 0, 389, 388, 1, 0, 0, 0, 390, 393, 1, 0, 0, 0, 391, 389, 1, 0, 0, 0, 391, 392, 1, 0, 0, 0, 392, 397, 1, 0, 0, 0, 393, 391, 1, 0, 0, 0, 394, 396, 3, 8, 4, 0, 395, 394, 1, 0, 0, 0, 396, 399, 1, 0, 0, 0, 397, 395, 1, 0, 0, 0, 397, 398, 1, 0, 0, 0, 398, 406, 1, 0, 0, 0, 399, 397, 1, 0, 0, 0, 400, 402, 5, 7, 0, 0, 401, 400, 1, 0, 0, 0, 401, 402, 1, 0, 0, 0, 402, 403, 1, 0, 0, 0, 403, 405, 3, 82, 41, 0, 404, 401, 1, 0, 0, 0, 405, 408, 1, 0, 0, 0, 406, 404, 1, 0, 0, 0, 406, 407, 1, 0, 0, 0, 407, 81, 1, 0, 0, 0, 408, 406, 1, 0, 0, 0, 409, 413, 3, 90, 45, 0, 410, 412, 5, 7, 0, 0, 411, 410, 1, 0, 0, 0, 412, 415, 1, 0, 0, 0, 413, 411, 1, 0, 0, 0, 413, 414, 1, 0, 0, 0, 414, 419, 1, 0, 0, 0, 415, 413, 1, 0, 0, 0, 416, 418, 3, 8, 4, 0, 417, 416, 1, 0, 0, 0, 418, 421, 1, 0, 0, 0, 419, 417, 1, 0, 0, 0, 419, 420, 1, 0, 0, 0, 420, 428, 1, 0, 0, 0, 421, 419, 1, 0, 0, 0, 422, 424, 5, 7, 0, 0, 423, 422, 1, 0, 0, 0, 423, 424, 1, 0, 0, 0, 424, 425, 1, 0, 0, 0, 425, 427, 3, 84, 42, 0, 426, 423, 1, 0, 0, 0, 427, 430, 1, 0, 0, 0, 428, 426, 1, 0, 0, 0, 428, 429, 1, 0, 0, 0, 429, 83, 1, 0, 0, 0, 430, 428, 1, 0, 0, 0, 431, 435, 3, 92, 46, 0, 432, 434, 5, 7, 0, 0, 433, 432, 1, 0, 0, 0, 434, 437, 1, 0, 0, 0, 435, 433, 1, 0, 0, 0, 435, 436, 1, 0, 0, 0, 436, 441, 1, 0, 0, 0, 437, 435, 1, 0, 0, 0, 438, 440, 3, 8, 4, 0, 439, 438, 1, 0, 0, 0, 440, 443, 1, 0, 0, 0, 441, 439, 1, 0, 0, 0, 441, 442, 1, 0, 0, 0, 442, 85, 1, 0, 0, 0, 443, 441, 1, 0, 0, 0, 444, 445, 5, 26, 0, 0, 445, 446, 5, 26, 0, 0, 446, 447, 5, 26, 0, 0, 447, 448, 5, 26, 0, 0, 448, 449, 5, 26, 0, 0, 449, 450, 5, 26, 0, 0, 450, 451, 5, 26, 0, 0, 451, 452, 5, 26, 0, 0, 452, 453, 5, 26, 0, 0, 453, 454, 3, 38, 19, 0, 454, 455, 3, 94, 47, 0, 455, 87, 1, 0, 0, 0, 456, 457, 5, 5, 0, 0, 457, 458, 3, 38, 19, 0, 458, 459, 3, 94, 47, 0, 459, 89, 1, 0, 0, 0, 460, 461, 5, 6, 0, 0, 461, 462, 3, 38, 19, 0, 462, 463, 3, 94, 47, 0, 463, 91, 1, 0, 0, 0, 464, 465, 5, 18, 0, 0, 465, 466, 5, 18, 0, 0, 466, 467, 5, 18, 0, 0, 467, 468, 3, 38, 19, 0, 468, 469, 3, 94, 47, 0, 469, 93, 1, 0, 0, 0, 470, 471, 7, 4, 0, 0, 471, 95, 1, 0, 0, 0, 52, 98, 105, 109, 116, 121, 127, 133, 139, 144, 151, 163, 171, 180, 185, 193, 203, 209, 218, 223, 235, 240, 244, 246, 251, 256, 258, 261, 264, 274, 285, 291, 300, 311, 323, 342, 344, 351, 355, 369, 375, 379, 384, 391, 397, 401, 406, 413, 419, 423, 428, 435, 441]
+[4, 1, 42, 470, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 2, 47, 7, 47, 1, 0, 1, 0, 3, 0, 99, 8, 0, 1, 0, 1, 0, 1, 1, 4, 1, 104, 8, 1, 11, 1, 12, 1, 105, 1, 2, 1, 2, 3, 2, 110, 8, 2, 1, 2, 1, 2, 1, 3, 4, 3, 115, 8, 3, 11, 3, 12, 3, 116, 1, 3, 5, 3, 120, 8, 3, 10, 3, 12, 3, 123, 9, 3, 1, 3, 5, 3, 126, 8, 3, 10, 3, 12, 3, 129, 9, 3, 1, 3, 5, 3, 132, 8, 3, 10, 3, 12, 3, 135, 9, 3, 1, 4, 4, 4, 138, 8, 4, 11, 4, 12, 4, 139, 1, 4, 5, 4, 143, 8, 4, 10, 4, 12, 4, 146, 9, 4, 1, 5, 1, 5, 1, 5, 1, 5, 3, 5, 152, 8, 5, 1, 6, 1, 6, 1, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 7, 5, 7, 162, 8, 7, 10, 7, 12, 7, 165, 9, 7, 1, 8, 1, 8, 1, 8, 1, 9, 1, 9, 1, 10, 1, 10, 1, 10, 4, 10, 175, 8, 10, 11, 10, 12, 10, 176, 1, 10, 5, 10, 180, 8, 10, 10, 10, 12, 10, 183, 9, 10, 1, 11, 1, 11, 1, 11, 5, 11, 188, 8, 11, 10, 11, 12, 11, 191, 9, 11, 1, 12, 1, 12, 1, 12, 1, 13, 1, 13, 5, 13, 198, 8, 13, 10, 13, 12, 13, 201, 9, 13, 1, 14, 1, 14, 1, 14, 3, 14, 206, 8, 14, 1, 14, 1, 14, 1, 14, 1, 15, 1, 15, 1, 15, 1, 15, 3, 15, 215, 8, 15, 1, 16, 1, 16, 1, 16, 3, 16, 220, 8, 16, 1, 17, 1, 17, 1, 18, 4, 18, 225, 8, 18, 11, 18, 12, 18, 226, 1, 19, 1, 19, 1, 19, 3, 19, 232, 8, 19, 1, 19, 1, 19, 5, 19, 236, 8, 19, 10, 19, 12, 19, 239, 9, 19, 1, 19, 1, 19, 3, 19, 243, 8, 19, 1, 19, 1, 19, 1, 19, 5, 19, 248, 8, 19, 10, 19, 12, 19, 251, 9, 19, 3, 19, 253, 8, 19, 1, 19, 3, 19, 256, 8, 19, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 3, 20, 265, 8, 20, 1, 21, 1, 21, 1, 22, 1, 22, 1, 22, 1, 22, 1, 22, 1, 23, 1, 23, 4, 23, 276, 8, 23, 11, 23, 12, 23, 277, 1, 23, 1, 23, 5, 23, 282, 8, 23, 10, 23, 12, 23, 285, 9, 23, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 1, 24, 3, 24, 296, 8, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 1, 27, 3, 27, 309, 8, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 31, 1, 31, 3, 31, 321, 8, 31, 1, 32, 1, 32, 1, 32, 1, 33, 1, 33, 1, 33, 1, 34, 1, 34, 1, 34, 1, 35, 1, 35, 1, 35, 1, 36, 1, 36, 1, 36, 1, 36, 1, 36, 4, 36, 340, 8, 36, 11, 36, 12, 36, 341, 1, 36, 1, 36, 1, 36, 4, 36, 347, 8, 36, 11, 36, 12, 36, 348, 1, 36, 1, 36, 3, 36, 353, 8, 36, 1, 37, 1, 37, 1, 37, 1, 37, 1, 38, 1, 38, 1, 38, 1, 38, 1, 39, 1, 39, 5, 39, 365, 8, 39, 10, 39, 12, 39, 368, 9, 39, 1, 39, 5, 39, 371, 8, 39, 10, 39, 12, 39, 374, 9, 39, 1, 39, 3, 39, 377, 8, 39, 1, 39, 5, 39, 380, 8, 39, 10, 39, 12, 39, 383, 9, 39, 1, 40, 1, 40, 5, 40, 387, 8, 40, 10, 40, 12, 40, 390, 9, 40, 1, 40, 5, 40, 393, 8, 40, 10, 40, 12, 40, 396, 9, 40, 1, 40, 3, 40, 399, 8, 40, 1, 40, 5, 40, 402, 8, 40, 10, 40, 12, 40, 405, 9, 40, 1, 41, 1, 41, 5, 41, 409, 8, 41, 10, 41, 12, 41, 412, 9, 41, 1, 41, 5, 41, 415, 8, 41, 10, 41, 12, 41, 418, 9, 41, 1, 41, 3, 41, 421, 8, 41, 1, 41, 5, 41, 424, 8, 41, 10, 41, 12, 41, 427, 9, 41, 1, 42, 1, 42, 5, 42, 431, 8, 42, 10, 42, 12, 42, 434, 9, 42, 1, 42, 5, 42, 437, 8, 42, 10, 42, 12, 42, 440, 9, 42, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 43, 1, 44, 1, 44, 1, 44, 1, 44, 1, 45, 1, 45, 1, 45, 1, 45, 1, 46, 1, 46, 1, 46, 1, 46, 1, 46, 1, 46, 1, 47, 1, 47, 1, 47, 0, 0, 48, 0, 2, 4, 6, 8, 10, 12, 14, 16, 18, 20, 22, 24, 26, 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56, 58, 60, 62, 64, 66, 68, 70, 72, 74, 76, 78, 80, 82, 84, 86, 88, 90, 92, 94, 0, 5, 2, 0, 9, 9, 38, 38, 4, 0, 22, 22, 28, 28, 30, 31, 38, 41, 2, 0, 25, 27, 42, 42, 1, 0, 32, 35, 1, 1, 7, 7, 498, 0, 96, 1, 0, 0, 0, 2, 103, 1, 0, 0, 0, 4, 107, 1, 0, 0, 0, 6, 114, 1, 0, 0, 0, 8, 137, 1, 0, 0, 0, 10, 151, 1, 0, 0, 0, 12, 153, 1, 0, 0, 0, 14, 158, 1, 0, 0, 0, 16, 166, 1, 0, 0, 0, 18, 169, 1, 0, 0, 0, 20, 171, 1, 0, 0, 0, 22, 184, 1, 0, 0, 0, 24, 192, 1, 0, 0, 0, 26, 195, 1, 0, 0, 0, 28, 202, 1, 0, 0, 0, 30, 214, 1, 0, 0, 0, 32, 216, 1, 0, 0, 0, 34, 221, 1, 0, 0, 0, 36, 224, 1, 0, 0, 0, 38, 228, 1, 0, 0, 0, 40, 264, 1, 0, 0, 0, 42, 266, 1, 0, 0, 0, 44, 268, 1, 0, 0, 0, 46, 273, 1, 0, 0, 0, 48, 295, 1, 0, 0, 0, 50, 297, 1, 0, 0, 0, 52, 299, 1, 0, 0, 0, 54, 308, 1, 0, 0, 0, 56, 310, 1, 0, 0, 0, 58, 312, 1, 0, 0, 0, 60, 314, 1, 0, 0, 0, 62, 320, 1, 0, 0, 0, 64, 322, 1, 0, 0, 0, 66, 325, 1, 0, 0, 0, 68, 328, 1, 0, 0, 0, 70, 331, 1, 0, 0, 0, 72, 352, 1, 0, 0, 0, 74, 354, 1, 0, 0, 0, 76, 358, 1, 0, 0, 0, 78, 362, 1, 0, 0, 0, 80, 384, 1, 0, 0, 0, 82, 406, 1, 0, 0, 0, 84, 428, 1, 0, 0, 0, 86, 441, 1, 0, 0, 0, 88, 453, 1, 0, 0, 0, 90, 457, 1, 0, 0, 0, 92, 461, 1, 0, 0, 0, 94, 467, 1, 0, 0, 0, 96, 98, 3, 2, 1, 0, 97, 99, 3, 6, 3, 0, 98, 97, 1, 0, 0, 0, 98, 99, 1, 0, 0, 0, 99, 100, 1, 0, 0, 0, 100, 101, 5, 0, 0, 1, 101, 1, 1, 0, 0, 0, 102, 104, 3, 4, 2, 0, 103, 102, 1, 0, 0, 0, 104, 105, 1, 0, 0, 0, 105, 103, 1, 0, 0, 0, 105, 106, 1, 0, 0, 0, 106, 3, 1, 0, 0, 0, 107, 109, 5, 32, 0, 0, 108, 110, 3, 36, 18, 0, 109, 108, 1, 0, 0, 0, 109, 110, 1, 0, 0, 0, 110, 111, 1, 0, 0, 0, 111, 112, 5, 7, 0, 0, 112, 5, 1, 0, 0, 0, 113, 115, 5, 7, 0, 0, 114, 113, 1, 0, 0, 0, 115, 116, 1, 0, 0, 0, 116, 114, 1, 0, 0, 0, 116, 117, 1, 0, 0, 0, 117, 121, 1, 0, 0, 0, 118, 120, 3, 8, 4, 0, 119, 118, 1, 0, 0, 0, 120, 123, 1, 0, 0, 0, 121, 119, 1, 0, 0, 0, 121, 122, 1, 0, 0, 0, 122, 127, 1, 0, 0, 0, 123, 121, 1, 0, 0, 0, 124, 126, 3, 80, 40, 0, 125, 124, 1, 0, 0, 0, 126, 129, 1, 0, 0, 0, 127, 125, 1, 0, 0, 0, 127, 128, 1, 0, 0, 0, 128, 133, 1, 0, 0, 0, 129, 127, 1, 0, 0, 0, 130, 132, 3, 78, 39, 0, 131, 130, 1, 0, 0, 0, 132, 135, 1, 0, 0, 0, 133, 131, 1, 0, 0, 0, 133, 134, 1, 0, 0, 0, 134, 7, 1, 0, 0, 0, 135, 133, 1, 0, 0, 0, 136, 138, 3, 10, 5, 0, 137, 136, 1, 0, 0, 0, 138, 139, 1, 0, 0, 0, 139, 137, 1, 0, 0, 0, 139, 140, 1, 0, 0, 0, 140, 144, 1, 0, 0, 0, 141, 143, 5, 7, 0, 0, 142, 141, 1, 0, 0, 0, 143, 146, 1, 0, 0, 0, 144, 142, 1, 0, 0, 0, 144, 145, 1, 0, 0, 0, 145, 9, 1, 0, 0, 0, 146, 144, 1, 0, 0, 0, 147, 152, 3, 26, 13, 0, 148, 152, 3, 14, 7, 0, 149, 152, 3, 12, 6, 0, 150, 152, 3, 4, 2, 0, 151, 147, 1, 0, 0, 0, 151, 148, 1, 0, 0, 0, 151, 149, 1, 0, 0, 0, 151, 150, 1, 0, 0, 0, 152, 11, 1, 0, 0, 0, 153, 154, 3, 76, 38, 0, 154, 155, 5, 42, 0, 0, 155, 156, 3, 36, 18, 0, 156, 157, 5, 7, 0, 0, 157, 13, 1, 0, 0, 0, 158, 159, 5, 25, 0, 0, 159, 163, 3, 16, 8, 0, 160, 162, 3, 22, 11, 0, 161, 160, 1, 0, 0, 0, 162, 165, 1, 0, 0, 0, 163, 161, 1, 0, 0, 0, 163, 164, 1, 0, 0, 0, 164, 15, 1, 0, 0, 0, 165, 163, 1, 0, 0, 0, 166, 167, 3, 18, 9, 0, 167, 168, 5, 7, 0, 0, 168, 17, 1, 0, 0, 0, 169, 170, 3, 20, 10, 0, 170, 19, 1, 0, 0, 0, 171, 181, 3, 36, 18, 0, 172, 174, 5, 7, 0, 0, 173, 175, 5, 29, 0, 0, 174, 173, 1, 0, 0, 0, 175, 176, 1, 0, 0, 0, 176, 174, 1, 0, 0, 0, 176, 177, 1, 0, 0, 0, 177, 178, 1, 0, 0, 0, 178, 180, 3, 36, 18, 0, 179, 172, 1, 0, 0, 0, 180, 183, 1, 0, 0, 0, 181, 179, 1, 0, 0, 0, 181, 182, 1, 0, 0, 0, 182, 21, 1, 0, 0, 0, 183, 181, 1, 0, 0, 0, 184, 185, 5, 20, 0, 0, 185, 189, 3, 16, 8, 0, 186, 188, 3, 24, 12, 0, 187, 186, 1, 0, 0, 0, 188, 191, 1, 0, 0, 0, 189, 187, 1, 0, 0, 0, 189, 190, 1, 0, 0, 0, 190, 23, 1, 0, 0, 0, 191, 189, 1, 0, 0, 0, 192, 193, 5, 21, 0, 0, 193, 194, 3, 16, 8, 0, 194, 25, 1, 0, 0, 0, 195, 199, 3, 28, 14, 0, 196, 198, 3, 22, 11, 0, 197, 196, 1, 0, 0, 0, 198, 201, 1, 0, 0, 0, 199, 197, 1, 0, 0, 0, 199, 200, 1, 0, 0, 0, 200, 27, 1, 0, 0, 0, 201, 199, 1, 0, 0, 0, 202, 205, 3, 30, 15, 0, 203, 204, 5, 29, 0, 0, 204, 206, 3, 34, 17, 0, 205, 203, 1, 0, 0, 0, 205, 206, 1, 0, 0, 0, 206, 207, 1, 0, 0, 0, 207, 208, 3, 18, 9, 0, 208, 209, 5, 7, 0, 0, 209, 29, 1, 0, 0, 0, 210, 215, 5, 8, 0, 0, 211, 215, 3, 32, 16, 0, 212, 215, 5, 40, 0, 0, 213, 215, 5, 41, 0, 0, 214, 210, 1, 0, 0, 0, 214, 211, 1, 0, 0, 0, 214, 212, 1, 0, 0, 0, 214, 213, 1, 0, 0, 0, 215, 31, 1, 0, 0, 0, 216, 219, 7, 0, 0, 0, 217, 218, 5, 42, 0, 0, 218, 220, 3, 52, 26, 0, 219, 217, 1, 0, 0, 0, 219, 220, 1, 0, 0, 0, 220, 33, 1, 0, 0, 0, 221, 222, 5, 15, 0, 0, 222, 35, 1, 0, 0, 0, 223, 225, 3, 38, 19, 0, 224, 223, 1, 0, 0, 0, 225, 226, 1, 0, 0, 0, 226, 224, 1, 0, 0, 0, 226, 227, 1, 0, 0, 0, 227, 37, 1, 0, 0, 0, 228, 231, 5, 29, 0, 0, 229, 230, 5, 36, 0, 0, 230, 232, 3, 56, 28, 0, 231, 229, 1, 0, 0, 0, 231, 232, 1, 0, 0, 0, 232, 237, 1, 0, 0, 0, 233, 236, 3, 56, 28, 0, 234, 236, 5, 37, 0, 0, 235, 233, 1, 0, 0, 0, 235, 234, 1, 0, 0, 0, 236, 239, 1, 0, 0, 0, 237, 235, 1, 0, 0, 0, 237, 238, 1, 0, 0, 0, 238, 242, 1, 0, 0, 0, 239, 237, 1, 0, 0, 0, 240, 243, 3, 40, 20, 0, 241, 243, 3, 72, 36, 0, 242, 240, 1, 0, 0, 0, 242, 241, 1, 0, 0, 0, 242, 243, 1, 0, 0, 0, 243, 252, 1, 0, 0, 0, 244, 249, 3, 54, 27, 0, 245, 248, 3, 54, 27, 0, 246, 248, 3, 48, 24, 0, 247, 245, 1, 0, 0, 0, 247, 246, 1, 0, 0, 0, 248, 251, 1, 0, 0, 0, 249, 247, 1, 0, 0, 0, 249, 250, 1, 0, 0, 0, 250, 253, 1, 0, 0, 0, 251, 249, 1, 0, 0, 0, 252, 244, 1, 0, 0, 0, 252, 253, 1, 0, 0, 0, 253, 255, 1, 0, 0, 0, 254, 256, 3, 76, 38, 0, 255, 254, 1, 0, 0, 0, 255, 256, 1, 0, 0, 0, 256, 39, 1, 0, 0, 0, 257, 265, 3, 60, 30, 0, 258, 265, 3, 62, 31, 0, 259, 265, 3, 74, 37, 0, 260, 265, 3, 44, 22, 0, 261, 265, 3, 46, 23, 0, 262, 265, 3, 76, 38, 0, 263, 265, 3, 34, 17, 0, 264, 257, 1, 0, 0, 0, 264, 258, 1, 0, 0, 0, 264, 259, 1, 0, 0, 0, 264, 260, 1, 0, 0, 0, 264, 261, 1, 0, 0, 0, 264, 262, 1, 0, 0, 0, 264, 263, 1, 0, 0, 0, 265, 41, 1, 0, 0, 0, 266, 267, 5, 17, 0, 0, 267, 43, 1, 0, 0, 0, 268, 269, 5, 16, 0, 0, 269, 270, 5, 42, 0, 0, 270, 271, 5, 42, 0, 0, 271, 272, 3, 46, 23, 0, 272, 45, 1, 0, 0, 0, 273, 283, 3, 48, 24, 0, 274, 276, 3, 58, 29, 0, 275, 274, 1, 0, 0, 0, 276, 277, 1, 0, 0, 0, 277, 275, 1, 0, 0, 0, 277, 278, 1, 0, 0, 0, 278, 279, 1, 0, 0, 0, 279, 280, 3, 48, 24, 0, 280, 282, 1, 0, 0, 0, 281, 275, 1, 0, 0, 0, 282, 285, 1, 0, 0, 0, 283, 281, 1, 0, 0, 0, 283, 284, 1, 0, 0, 0, 284, 47, 1, 0, 0, 0, 285, 283, 1, 0, 0, 0, 286, 296, 5, 16, 0, 0, 287, 296, 5, 19, 0, 0, 288, 296, 5, 14, 0, 0, 289, 296, 5, 15, 0, 0, 290, 296, 3, 50, 25, 0, 291, 296, 3, 52, 26, 0, 292, 296, 3, 42, 21, 0, 293, 296, 5, 8, 0, 0, 294, 296, 5, 9, 0, 0, 295, 286, 1, 0, 0, 0, 295, 287, 1, 0, 0, 0, 295, 288, 1, 0, 0, 0, 295, 289, 1, 0, 0, 0, 295, 290, 1, 0, 0, 0, 295, 291, 1, 0, 0, 0, 295, 292, 1, 0, 0, 0, 295, 293, 1, 0, 0, 0, 295, 294, 1, 0, 0, 0, 296, 49, 1, 0, 0, 0, 297, 298, 5, 10, 0, 0, 298, 51, 1, 0, 0, 0, 299, 300, 5, 11, 0, 0, 300, 53, 1, 0, 0, 0, 301, 309, 5, 36, 0, 0, 302, 309, 5, 37, 0, 0, 303, 309, 5, 24, 0, 0, 304, 309, 5, 23, 0, 0, 305, 309, 3, 56, 28, 0, 306, 309, 3, 60, 30, 0, 307, 309, 3, 58, 29, 0, 308, 301, 1, 0, 0, 0, 308, 302, 1, 0, 0, 0, 308, 303, 1, 0, 0, 0, 308, 304, 1, 0, 0, 0, 308, 305, 1, 0, 0, 0, 308, 306, 1, 0, 0, 0, 308, 307, 1, 0, 0, 0, 309, 55, 1, 0, 0, 0, 310, 311, 7, 1, 0, 0, 311, 57, 1, 0, 0, 0, 312, 313, 7, 2, 0, 0, 313, 59, 1, 0, 0, 0, 314, 315, 7, 3, 0, 0, 315, 61, 1, 0, 0, 0, 316, 321, 3, 64, 32, 0, 317, 321, 3, 66, 33, 0, 318, 321, 3, 68, 34, 0, 319, 321, 3, 70, 35, 0, 320, 316, 1, 0, 0, 0, 320, 317, 1, 0, 0, 0, 320, 318, 1, 0, 0, 0, 320, 319, 1, 0, 0, 0, 321, 63, 1, 0, 0, 0, 322, 323, 5, 32, 0, 0, 323, 324, 5, 16, 0, 0, 324, 65, 1, 0, 0, 0, 325, 326, 5, 33, 0, 0, 326, 327, 5, 16, 0, 0, 327, 67, 1, 0, 0, 0, 328, 329, 5, 35, 0, 0, 329, 330, 5, 16, 0, 0, 330, 69, 1, 0, 0, 0, 331, 332, 5, 34, 0, 0, 332, 333, 5, 16, 0, 0, 333, 71, 1, 0, 0, 0, 334, 339, 5, 36, 0, 0, 335, 340, 3, 40, 20, 0, 336, 340, 3, 34, 17, 0, 337, 340, 5, 1, 0, 0, 338, 340, 5, 2, 0, 0, 339, 335, 1, 0, 0, 0, 339, 336, 1, 0, 0, 0, 339, 337, 1, 0, 0, 0, 339, 338, 1, 0, 0, 0, 340, 341, 1, 0, 0, 0, 341, 339, 1, 0, 0, 0, 341, 342, 1, 0, 0, 0, 342, 343, 1, 0, 0, 0, 343, 353, 5, 36, 0, 0, 344, 346, 5, 37, 0, 0, 345, 347, 3, 40, 20, 0, 346, 345, 1, 0, 0, 0, 347, 348, 1, 0, 0, 0, 348, 346, 1, 0, 0, 0, 348, 349, 1, 0, 0, 0, 349, 350, 1, 0, 0, 0, 350, 351, 5, 37, 0, 0, 351, 353, 1, 0, 0, 0, 352, 334, 1, 0, 0, 0, 352, 344, 1, 0, 0, 0, 353, 73, 1, 0, 0, 0, 354, 355, 5, 1, 0, 0, 355, 356, 3, 46, 23, 0, 356, 357, 5, 2, 0, 0, 357, 75, 1, 0, 0, 0, 358, 359, 5, 3, 0, 0, 359, 360, 3, 46, 23, 0, 360, 361, 5, 4, 0, 0, 361, 77, 1, 0, 0, 0, 362, 366, 3, 86, 43, 0, 363, 365, 5, 7, 0, 0, 364, 363, 1, 0, 0, 0, 365, 368, 1, 0, 0, 0, 366, 364, 1, 0, 0, 0, 366, 367, 1, 0, 0, 0, 367, 372, 1, 0, 0, 0, 368, 366, 1, 0, 0, 0, 369, 371, 3, 8, 4, 0, 370, 369, 1, 0, 0, 0, 371, 374, 1, 0, 0, 0, 372, 370, 1, 0, 0, 0, 372, 373, 1, 0, 0, 0, 373, 381, 1, 0, 0, 0, 374, 372, 1, 0, 0, 0, 375, 377, 5, 7, 0, 0, 376, 375, 1, 0, 0, 0, 376, 377, 1, 0, 0, 0, 377, 378, 1, 0, 0, 0, 378, 380, 3, 80, 40, 0, 379, 376, 1, 0, 0, 0, 380, 383, 1, 0, 0, 0, 381, 379, 1, 0, 0, 0, 381, 382, 1, 0, 0, 0, 382, 79, 1, 0, 0, 0, 383, 381, 1, 0, 0, 0, 384, 388, 3, 88, 44, 0, 385, 387, 5, 7, 0, 0, 386, 385, 1, 0, 0, 0, 387, 390, 1, 0, 0, 0, 388, 386, 1, 0, 0, 0, 388, 389, 1, 0, 0, 0, 389, 394, 1, 0, 0, 0, 390, 388, 1, 0, 0, 0, 391, 393, 3, 8, 4, 0, 392, 391, 1, 0, 0, 0, 393, 396, 1, 0, 0, 0, 394, 392, 1, 0, 0, 0, 394, 395, 1, 0, 0, 0, 395, 403, 1, 0, 0, 0, 396, 394, 1, 0, 0, 0, 397, 399, 5, 7, 0, 0, 398, 397, 1, 0, 0, 0, 398, 399, 1, 0, 0, 0, 399, 400, 1, 0, 0, 0, 400, 402, 3, 82, 41, 0, 401, 398, 1, 0, 0, 0, 402, 405, 1, 0, 0, 0, 403, 401, 1, 0, 0, 0, 403, 404, 1, 0, 0, 0, 404, 81, 1, 0, 0, 0, 405, 403, 1, 0, 0, 0, 406, 410, 3, 90, 45, 0, 407, 409, 5, 7, 0, 0, 408, 407, 1, 0, 0, 0, 409, 412, 1, 0, 0, 0, 410, 408, 1, 0, 0, 0, 410, 411, 1, 0, 0, 0, 411, 416, 1, 0, 0, 0, 412, 410, 1, 0, 0, 0, 413, 415, 3, 8, 4, 0, 414, 413, 1, 0, 0, 0, 415, 418, 1, 0, 0, 0, 416, 414, 1, 0, 0, 0, 416, 417, 1, 0, 0, 0, 417, 425, 1, 0, 0, 0, 418, 416, 1, 0, 0, 0, 419, 421, 5, 7, 0, 0, 420, 419, 1, 0, 0, 0, 420, 421, 1, 0, 0, 0, 421, 422, 1, 0, 0, 0, 422, 424, 3, 84, 42, 0, 423, 420, 1, 0, 0, 0, 424, 427, 1, 0, 0, 0, 425, 423, 1, 0, 0, 0, 425, 426, 1, 0, 0, 0, 426, 83, 1, 0, 0, 0, 427, 425, 1, 0, 0, 0, 428, 432, 3, 92, 46, 0, 429, 431, 5, 7, 0, 0, 430, 429, 1, 0, 0, 0, 431, 434, 1, 0, 0, 0, 432, 430, 1, 0, 0, 0, 432, 433, 1, 0, 0, 0, 433, 438, 1, 0, 0, 0, 434, 432, 1, 0, 0, 0, 435, 437, 3, 8, 4, 0, 436, 435, 1, 0, 0, 0, 437, 440, 1, 0, 0, 0, 438, 436, 1, 0, 0, 0, 438, 439, 1, 0, 0, 0, 439, 85, 1, 0, 0, 0, 440, 438, 1, 0, 0, 0, 441, 442, 5, 32, 0, 0, 442, 443, 5, 32, 0, 0, 443, 444, 5, 32, 0, 0, 444, 445, 5, 32, 0, 0, 445, 446, 5, 32, 0, 0, 446, 447, 5, 32, 0, 0, 447, 448, 5, 32, 0, 0, 448, 449, 5, 32, 0, 0, 449, 450, 5, 32, 0, 0, 450, 451, 3, 36, 18, 0, 451, 452, 3, 94, 47, 0, 452, 87, 1, 0, 0, 0, 453, 454, 5, 5, 0, 0, 454, 455, 3, 36, 18, 0, 455, 456, 3, 94, 47, 0, 456, 89, 1, 0, 0, 0, 457, 458, 5, 6, 0, 0, 458, 459, 3, 36, 18, 0, 459, 460, 3, 94, 47, 0, 460, 91, 1, 0, 0, 0, 461, 462, 5, 25, 0, 0, 462, 463, 5, 25, 0, 0, 463, 464, 5, 25, 0, 0, 464, 465, 3, 36, 18, 0, 465, 466, 3, 94, 47, 0, 466, 93, 1, 0, 0, 0, 467, 468, 7, 4, 0, 0, 468, 95, 1, 0, 0, 0, 51, 98, 105, 109, 116, 121, 127, 133, 139, 144, 151, 163, 176, 181, 189, 199, 205, 214, 219, 226, 231, 235, 237, 242, 247, 249, 252, 255, 264, 277, 283, 295, 308, 320, 339, 341, 348, 352, 366, 372, 376, 381, 388, 394, 398, 403, 410, 416, 420, 425, 432, 438]
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.interp` & `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.interp`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,140 @@
 token literal names:
 null
-'['
-']'
 '[['
 ']]'
+'['
+']'
 '======='
 '*****'
 null
 'o'
 'x'
 null
 null
 null
 null
 null
+null
+null
+null
+null
+null
 '  -'
 '    -'
 null
+'$'
+'^'
 '-'
 '.'
 '/'
 '_'
-':'
 ' '
 '('
 ')'
 '#'
 '@'
 '+'
 '%'
 '\''
 '"'
 '~'
 '*'
 '<'
 '>'
+':'
 
 token symbolic names:
 null
 null
 null
 null
 null
 null
 null
 NL
 LOWER_O
 LOWER_X
 DATE
 TIME
+CREATE_RANGE_HEAD
+MODIFY_RANGE_HEAD
+DATE_RANGE_TAIL
+PRIORITY
 ID
 ZID
+SHORT_DATE
 NUM_ID
 TWO_SPACE_DASH
 FOUR_SPACE_DASH
 SYMBOL
+DOLLAR
+HAT
 DASH
 DOT
 FSLASH
 UNDERSCORE
-COLON
 SPACE
 LPAREN
 RPAREN
 HASH
 AT_SIGN
 PLUS
 PERCENT
 SQUOTE
 DQUOTE
 TILDE
 STAR
 LANGLE
 RANGLE
+COLON
 
 rule names:
 T__0
 T__1
 T__2
 T__3
 T__4
 T__5
 NL
 LOWER_O
 LOWER_X
 DATE
 TIME
+CREATE_RANGE_HEAD
+MODIFY_RANGE_HEAD
+DATE_RANGE_TAIL
+PRIORITY
 ID
 ZID
+SHORT_DATE
 NUM_ID
 TWO_SPACE_DASH
 FOUR_SPACE_DASH
 SYMBOL
+DOLLAR
+HAT
 DASH
 DOT
 FSLASH
 UNDERSCORE
-COLON
 SPACE
 LPAREN
 RPAREN
 HASH
 AT_SIGN
 PLUS
 PERCENT
 SQUOTE
 DQUOTE
 TILDE
 STAR
 LANGLE
 RANGLE
+COLON
 UPPER_LETTER
 LOWER_LETTER
 ZID_CHAR
 NUM
 FIRST_D_NUM
 FIRST_M_NUM
 ALPHA
@@ -123,8 +144,8 @@
 DEFAULT_TOKEN_CHANNEL
 HIDDEN
 
 mode names:
 DEFAULT_MODE
 
 atn:
-[4, 0, 35, 234, 6, -1, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 1, 0, 1, 0, 1, 1, 1, 1, 1, 2, 1, 2, 1, 2, 1, 3, 1, 3, 1, 3, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 3, 6, 113, 8, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 11, 1, 11, 1, 11, 5, 11, 140, 8, 11, 10, 11, 12, 11, 143, 9, 11, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 1, 12, 3, 12, 155, 8, 12, 1, 13, 1, 13, 1, 13, 5, 13, 160, 8, 13, 10, 13, 12, 13, 163, 9, 13, 1, 14, 1, 14, 1, 14, 1, 14, 1, 15, 1, 15, 1, 15, 1, 15, 1, 15, 1, 15, 1, 16, 1, 16, 1, 17, 1, 17, 1, 18, 1, 18, 1, 19, 1, 19, 1, 20, 1, 20, 1, 21, 1, 21, 1, 22, 1, 22, 1, 23, 1, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 32, 1, 32, 1, 33, 1, 33, 1, 34, 1, 34, 1, 35, 1, 35, 1, 36, 1, 36, 1, 37, 1, 37, 3, 37, 219, 8, 37, 1, 38, 1, 38, 1, 39, 1, 39, 1, 40, 1, 40, 1, 41, 1, 41, 3, 41, 229, 8, 41, 1, 42, 1, 42, 3, 42, 233, 8, 42, 0, 0, 43, 1, 1, 3, 2, 5, 3, 7, 4, 9, 5, 11, 6, 13, 7, 15, 8, 17, 9, 19, 10, 21, 11, 23, 12, 25, 13, 27, 14, 29, 15, 31, 16, 33, 17, 35, 18, 37, 19, 39, 20, 41, 21, 43, 22, 45, 23, 47, 24, 49, 25, 51, 26, 53, 27, 55, 28, 57, 29, 59, 30, 61, 31, 63, 32, 65, 33, 67, 34, 69, 35, 71, 0, 73, 0, 75, 0, 77, 0, 79, 0, 81, 0, 83, 0, 85, 0, 1, 0, 2, 10, 0, 33, 33, 36, 36, 38, 38, 44, 44, 59, 59, 61, 61, 63, 63, 91, 94, 96, 96, 123, 125, 6, 0, 65, 72, 74, 78, 80, 90, 97, 105, 107, 107, 109, 122, 234, 0, 1, 1, 0, 0, 0, 0, 3, 1, 0, 0, 0, 0, 5, 1, 0, 0, 0, 0, 7, 1, 0, 0, 0, 0, 9, 1, 0, 0, 0, 0, 11, 1, 0, 0, 0, 0, 13, 1, 0, 0, 0, 0, 15, 1, 0, 0, 0, 0, 17, 1, 0, 0, 0, 0, 19, 1, 0, 0, 0, 0, 21, 1, 0, 0, 0, 0, 23, 1, 0, 0, 0, 0, 25, 1, 0, 0, 0, 0, 27, 1, 0, 0, 0, 0, 29, 1, 0, 0, 0, 0, 31, 1, 0, 0, 0, 0, 33, 1, 0, 0, 0, 0, 35, 1, 0, 0, 0, 0, 37, 1, 0, 0, 0, 0, 39, 1, 0, 0, 0, 0, 41, 1, 0, 0, 0, 0, 43, 1, 0, 0, 0, 0, 45, 1, 0, 0, 0, 0, 47, 1, 0, 0, 0, 0, 49, 1, 0, 0, 0, 0, 51, 1, 0, 0, 0, 0, 53, 1, 0, 0, 0, 0, 55, 1, 0, 0, 0, 0, 57, 1, 0, 0, 0, 0, 59, 1, 0, 0, 0, 0, 61, 1, 0, 0, 0, 0, 63, 1, 0, 0, 0, 0, 65, 1, 0, 0, 0, 0, 67, 1, 0, 0, 0, 0, 69, 1, 0, 0, 0, 1, 87, 1, 0, 0, 0, 3, 89, 1, 0, 0, 0, 5, 91, 1, 0, 0, 0, 7, 94, 1, 0, 0, 0, 9, 97, 1, 0, 0, 0, 11, 105, 1, 0, 0, 0, 13, 112, 1, 0, 0, 0, 15, 116, 1, 0, 0, 0, 17, 118, 1, 0, 0, 0, 19, 120, 1, 0, 0, 0, 21, 131, 1, 0, 0, 0, 23, 136, 1, 0, 0, 0, 25, 144, 1, 0, 0, 0, 27, 156, 1, 0, 0, 0, 29, 164, 1, 0, 0, 0, 31, 168, 1, 0, 0, 0, 33, 174, 1, 0, 0, 0, 35, 176, 1, 0, 0, 0, 37, 178, 1, 0, 0, 0, 39, 180, 1, 0, 0, 0, 41, 182, 1, 0, 0, 0, 43, 184, 1, 0, 0, 0, 45, 186, 1, 0, 0, 0, 47, 188, 1, 0, 0, 0, 49, 190, 1, 0, 0, 0, 51, 192, 1, 0, 0, 0, 53, 194, 1, 0, 0, 0, 55, 196, 1, 0, 0, 0, 57, 198, 1, 0, 0, 0, 59, 200, 1, 0, 0, 0, 61, 202, 1, 0, 0, 0, 63, 204, 1, 0, 0, 0, 65, 206, 1, 0, 0, 0, 67, 208, 1, 0, 0, 0, 69, 210, 1, 0, 0, 0, 71, 212, 1, 0, 0, 0, 73, 214, 1, 0, 0, 0, 75, 218, 1, 0, 0, 0, 77, 220, 1, 0, 0, 0, 79, 222, 1, 0, 0, 0, 81, 224, 1, 0, 0, 0, 83, 228, 1, 0, 0, 0, 85, 232, 1, 0, 0, 0, 87, 88, 5, 91, 0, 0, 88, 2, 1, 0, 0, 0, 89, 90, 5, 93, 0, 0, 90, 4, 1, 0, 0, 0, 91, 92, 5, 91, 0, 0, 92, 93, 5, 91, 0, 0, 93, 6, 1, 0, 0, 0, 94, 95, 5, 93, 0, 0, 95, 96, 5, 93, 0, 0, 96, 8, 1, 0, 0, 0, 97, 98, 5, 61, 0, 0, 98, 99, 5, 61, 0, 0, 99, 100, 5, 61, 0, 0, 100, 101, 5, 61, 0, 0, 101, 102, 5, 61, 0, 0, 102, 103, 5, 61, 0, 0, 103, 104, 5, 61, 0, 0, 104, 10, 1, 0, 0, 0, 105, 106, 5, 42, 0, 0, 106, 107, 5, 42, 0, 0, 107, 108, 5, 42, 0, 0, 108, 109, 5, 42, 0, 0, 109, 110, 5, 42, 0, 0, 110, 12, 1, 0, 0, 0, 111, 113, 5, 13, 0, 0, 112, 111, 1, 0, 0, 0, 112, 113, 1, 0, 0, 0, 113, 114, 1, 0, 0, 0, 114, 115, 5, 10, 0, 0, 115, 14, 1, 0, 0, 0, 116, 117, 5, 111, 0, 0, 117, 16, 1, 0, 0, 0, 118, 119, 5, 120, 0, 0, 119, 18, 1, 0, 0, 0, 120, 121, 5, 50, 0, 0, 121, 122, 3, 77, 38, 0, 122, 123, 3, 77, 38, 0, 123, 124, 3, 77, 38, 0, 124, 125, 3, 35, 17, 0, 125, 126, 3, 81, 40, 0, 126, 127, 3, 77, 38, 0, 127, 128, 3, 35, 17, 0, 128, 129, 3, 79, 39, 0, 129, 130, 3, 77, 38, 0, 130, 20, 1, 0, 0, 0, 131, 132, 2, 48, 50, 0, 132, 133, 3, 77, 38, 0, 133, 134, 2, 48, 53, 0, 134, 135, 3, 77, 38, 0, 135, 22, 1, 0, 0, 0, 136, 141, 3, 85, 42, 0, 137, 140, 3, 85, 42, 0, 138, 140, 3, 41, 20, 0, 139, 137, 1, 0, 0, 0, 139, 138, 1, 0, 0, 0, 140, 143, 1, 0, 0, 0, 141, 139, 1, 0, 0, 0, 141, 142, 1, 0, 0, 0, 142, 24, 1, 0, 0, 0, 143, 141, 1, 0, 0, 0, 144, 145, 3, 77, 38, 0, 145, 146, 3, 77, 38, 0, 146, 147, 3, 81, 40, 0, 147, 148, 3, 77, 38, 0, 148, 149, 3, 79, 39, 0, 149, 150, 3, 77, 38, 0, 150, 151, 3, 51, 25, 0, 151, 152, 3, 75, 37, 0, 152, 154, 3, 75, 37, 0, 153, 155, 3, 75, 37, 0, 154, 153, 1, 0, 0, 0, 154, 155, 1, 0, 0, 0, 155, 26, 1, 0, 0, 0, 156, 161, 3, 77, 38, 0, 157, 160, 3, 85, 42, 0, 158, 160, 3, 41, 20, 0, 159, 157, 1, 0, 0, 0, 159, 158, 1, 0, 0, 0, 160, 163, 1, 0, 0, 0, 161, 159, 1, 0, 0, 0, 161, 162, 1, 0, 0, 0, 162, 28, 1, 0, 0, 0, 163, 161, 1, 0, 0, 0, 164, 165, 5, 32, 0, 0, 165, 166, 5, 32, 0, 0, 166, 167, 5, 45, 0, 0, 167, 30, 1, 0, 0, 0, 168, 169, 5, 32, 0, 0, 169, 170, 5, 32, 0, 0, 170, 171, 5, 32, 0, 0, 171, 172, 5, 32, 0, 0, 172, 173, 5, 45, 0, 0, 173, 32, 1, 0, 0, 0, 174, 175, 7, 0, 0, 0, 175, 34, 1, 0, 0, 0, 176, 177, 5, 45, 0, 0, 177, 36, 1, 0, 0, 0, 178, 179, 5, 46, 0, 0, 179, 38, 1, 0, 0, 0, 180, 181, 5, 47, 0, 0, 181, 40, 1, 0, 0, 0, 182, 183, 5, 95, 0, 0, 183, 42, 1, 0, 0, 0, 184, 185, 5, 58, 0, 0, 185, 44, 1, 0, 0, 0, 186, 187, 5, 32, 0, 0, 187, 46, 1, 0, 0, 0, 188, 189, 5, 40, 0, 0, 189, 48, 1, 0, 0, 0, 190, 191, 5, 41, 0, 0, 191, 50, 1, 0, 0, 0, 192, 193, 5, 35, 0, 0, 193, 52, 1, 0, 0, 0, 194, 195, 5, 64, 0, 0, 195, 54, 1, 0, 0, 0, 196, 197, 5, 43, 0, 0, 197, 56, 1, 0, 0, 0, 198, 199, 5, 37, 0, 0, 199, 58, 1, 0, 0, 0, 200, 201, 5, 39, 0, 0, 201, 60, 1, 0, 0, 0, 202, 203, 5, 34, 0, 0, 203, 62, 1, 0, 0, 0, 204, 205, 5, 126, 0, 0, 205, 64, 1, 0, 0, 0, 206, 207, 5, 42, 0, 0, 207, 66, 1, 0, 0, 0, 208, 209, 5, 60, 0, 0, 209, 68, 1, 0, 0, 0, 210, 211, 5, 62, 0, 0, 211, 70, 1, 0, 0, 0, 212, 213, 2, 65, 90, 0, 213, 72, 1, 0, 0, 0, 214, 215, 2, 97, 122, 0, 215, 74, 1, 0, 0, 0, 216, 219, 3, 77, 38, 0, 217, 219, 7, 1, 0, 0, 218, 216, 1, 0, 0, 0, 218, 217, 1, 0, 0, 0, 219, 76, 1, 0, 0, 0, 220, 221, 2, 48, 57, 0, 221, 78, 1, 0, 0, 0, 222, 223, 2, 48, 51, 0, 223, 80, 1, 0, 0, 0, 224, 225, 2, 48, 49, 0, 225, 82, 1, 0, 0, 0, 226, 229, 3, 71, 35, 0, 227, 229, 3, 73, 36, 0, 228, 226, 1, 0, 0, 0, 228, 227, 1, 0, 0, 0, 229, 84, 1, 0, 0, 0, 230, 233, 3, 83, 41, 0, 231, 233, 3, 77, 38, 0, 232, 230, 1, 0, 0, 0, 232, 231, 1, 0, 0, 0, 233, 86, 1, 0, 0, 0, 10, 0, 112, 139, 141, 154, 159, 161, 218, 228, 232, 0]
+[4, 0, 42, 266, 6, -1, 2, 0, 7, 0, 2, 1, 7, 1, 2, 2, 7, 2, 2, 3, 7, 3, 2, 4, 7, 4, 2, 5, 7, 5, 2, 6, 7, 6, 2, 7, 7, 7, 2, 8, 7, 8, 2, 9, 7, 9, 2, 10, 7, 10, 2, 11, 7, 11, 2, 12, 7, 12, 2, 13, 7, 13, 2, 14, 7, 14, 2, 15, 7, 15, 2, 16, 7, 16, 2, 17, 7, 17, 2, 18, 7, 18, 2, 19, 7, 19, 2, 20, 7, 20, 2, 21, 7, 21, 2, 22, 7, 22, 2, 23, 7, 23, 2, 24, 7, 24, 2, 25, 7, 25, 2, 26, 7, 26, 2, 27, 7, 27, 2, 28, 7, 28, 2, 29, 7, 29, 2, 30, 7, 30, 2, 31, 7, 31, 2, 32, 7, 32, 2, 33, 7, 33, 2, 34, 7, 34, 2, 35, 7, 35, 2, 36, 7, 36, 2, 37, 7, 37, 2, 38, 7, 38, 2, 39, 7, 39, 2, 40, 7, 40, 2, 41, 7, 41, 2, 42, 7, 42, 2, 43, 7, 43, 2, 44, 7, 44, 2, 45, 7, 45, 2, 46, 7, 46, 2, 47, 7, 47, 2, 48, 7, 48, 2, 49, 7, 49, 1, 0, 1, 0, 1, 0, 1, 1, 1, 1, 1, 1, 1, 2, 1, 2, 1, 3, 1, 3, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 4, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 5, 1, 6, 3, 6, 127, 8, 6, 1, 6, 1, 6, 1, 7, 1, 7, 1, 8, 1, 8, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 9, 1, 10, 1, 10, 1, 10, 1, 10, 1, 10, 1, 11, 1, 11, 1, 11, 1, 12, 1, 12, 1, 12, 1, 13, 1, 13, 1, 13, 1, 14, 1, 14, 1, 14, 1, 15, 1, 15, 1, 15, 5, 15, 166, 8, 15, 10, 15, 12, 15, 169, 9, 15, 1, 16, 1, 16, 1, 16, 1, 16, 1, 16, 3, 16, 176, 8, 16, 1, 17, 1, 17, 1, 17, 1, 17, 1, 17, 1, 17, 1, 17, 1, 18, 1, 18, 1, 18, 5, 18, 188, 8, 18, 10, 18, 12, 18, 191, 9, 18, 1, 19, 1, 19, 1, 19, 1, 19, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 20, 1, 21, 1, 21, 1, 22, 1, 22, 1, 23, 1, 23, 1, 24, 1, 24, 1, 25, 1, 25, 1, 26, 1, 26, 1, 27, 1, 27, 1, 28, 1, 28, 1, 29, 1, 29, 1, 30, 1, 30, 1, 31, 1, 31, 1, 32, 1, 32, 1, 33, 1, 33, 1, 34, 1, 34, 1, 35, 1, 35, 1, 36, 1, 36, 1, 37, 1, 37, 1, 38, 1, 38, 1, 39, 1, 39, 1, 40, 1, 40, 1, 41, 1, 41, 1, 42, 1, 42, 1, 43, 1, 43, 1, 44, 1, 44, 3, 44, 251, 8, 44, 1, 45, 1, 45, 1, 46, 1, 46, 1, 47, 1, 47, 1, 48, 1, 48, 3, 48, 261, 8, 48, 1, 49, 1, 49, 3, 49, 265, 8, 49, 0, 0, 50, 1, 1, 3, 2, 5, 3, 7, 4, 9, 5, 11, 6, 13, 7, 15, 8, 17, 9, 19, 10, 21, 11, 23, 12, 25, 13, 27, 14, 29, 15, 31, 16, 33, 17, 35, 18, 37, 19, 39, 20, 41, 21, 43, 22, 45, 23, 47, 24, 49, 25, 51, 26, 53, 27, 55, 28, 57, 29, 59, 30, 61, 31, 63, 32, 65, 33, 67, 34, 69, 35, 71, 36, 73, 37, 75, 38, 77, 39, 79, 40, 81, 41, 83, 42, 85, 0, 87, 0, 89, 0, 91, 0, 93, 0, 95, 0, 97, 0, 99, 0, 1, 0, 2, 9, 0, 33, 33, 38, 38, 44, 44, 59, 59, 61, 61, 63, 63, 91, 93, 96, 96, 123, 125, 6, 0, 65, 72, 74, 78, 80, 90, 97, 105, 107, 107, 109, 122, 266, 0, 1, 1, 0, 0, 0, 0, 3, 1, 0, 0, 0, 0, 5, 1, 0, 0, 0, 0, 7, 1, 0, 0, 0, 0, 9, 1, 0, 0, 0, 0, 11, 1, 0, 0, 0, 0, 13, 1, 0, 0, 0, 0, 15, 1, 0, 0, 0, 0, 17, 1, 0, 0, 0, 0, 19, 1, 0, 0, 0, 0, 21, 1, 0, 0, 0, 0, 23, 1, 0, 0, 0, 0, 25, 1, 0, 0, 0, 0, 27, 1, 0, 0, 0, 0, 29, 1, 0, 0, 0, 0, 31, 1, 0, 0, 0, 0, 33, 1, 0, 0, 0, 0, 35, 1, 0, 0, 0, 0, 37, 1, 0, 0, 0, 0, 39, 1, 0, 0, 0, 0, 41, 1, 0, 0, 0, 0, 43, 1, 0, 0, 0, 0, 45, 1, 0, 0, 0, 0, 47, 1, 0, 0, 0, 0, 49, 1, 0, 0, 0, 0, 51, 1, 0, 0, 0, 0, 53, 1, 0, 0, 0, 0, 55, 1, 0, 0, 0, 0, 57, 1, 0, 0, 0, 0, 59, 1, 0, 0, 0, 0, 61, 1, 0, 0, 0, 0, 63, 1, 0, 0, 0, 0, 65, 1, 0, 0, 0, 0, 67, 1, 0, 0, 0, 0, 69, 1, 0, 0, 0, 0, 71, 1, 0, 0, 0, 0, 73, 1, 0, 0, 0, 0, 75, 1, 0, 0, 0, 0, 77, 1, 0, 0, 0, 0, 79, 1, 0, 0, 0, 0, 81, 1, 0, 0, 0, 0, 83, 1, 0, 0, 0, 1, 101, 1, 0, 0, 0, 3, 104, 1, 0, 0, 0, 5, 107, 1, 0, 0, 0, 7, 109, 1, 0, 0, 0, 9, 111, 1, 0, 0, 0, 11, 119, 1, 0, 0, 0, 13, 126, 1, 0, 0, 0, 15, 130, 1, 0, 0, 0, 17, 132, 1, 0, 0, 0, 19, 134, 1, 0, 0, 0, 21, 145, 1, 0, 0, 0, 23, 150, 1, 0, 0, 0, 25, 153, 1, 0, 0, 0, 27, 156, 1, 0, 0, 0, 29, 159, 1, 0, 0, 0, 31, 162, 1, 0, 0, 0, 33, 170, 1, 0, 0, 0, 35, 177, 1, 0, 0, 0, 37, 184, 1, 0, 0, 0, 39, 192, 1, 0, 0, 0, 41, 196, 1, 0, 0, 0, 43, 202, 1, 0, 0, 0, 45, 204, 1, 0, 0, 0, 47, 206, 1, 0, 0, 0, 49, 208, 1, 0, 0, 0, 51, 210, 1, 0, 0, 0, 53, 212, 1, 0, 0, 0, 55, 214, 1, 0, 0, 0, 57, 216, 1, 0, 0, 0, 59, 218, 1, 0, 0, 0, 61, 220, 1, 0, 0, 0, 63, 222, 1, 0, 0, 0, 65, 224, 1, 0, 0, 0, 67, 226, 1, 0, 0, 0, 69, 228, 1, 0, 0, 0, 71, 230, 1, 0, 0, 0, 73, 232, 1, 0, 0, 0, 75, 234, 1, 0, 0, 0, 77, 236, 1, 0, 0, 0, 79, 238, 1, 0, 0, 0, 81, 240, 1, 0, 0, 0, 83, 242, 1, 0, 0, 0, 85, 244, 1, 0, 0, 0, 87, 246, 1, 0, 0, 0, 89, 250, 1, 0, 0, 0, 91, 252, 1, 0, 0, 0, 93, 254, 1, 0, 0, 0, 95, 256, 1, 0, 0, 0, 97, 260, 1, 0, 0, 0, 99, 264, 1, 0, 0, 0, 101, 102, 5, 91, 0, 0, 102, 103, 5, 91, 0, 0, 103, 2, 1, 0, 0, 0, 104, 105, 5, 93, 0, 0, 105, 106, 5, 93, 0, 0, 106, 4, 1, 0, 0, 0, 107, 108, 5, 91, 0, 0, 108, 6, 1, 0, 0, 0, 109, 110, 5, 93, 0, 0, 110, 8, 1, 0, 0, 0, 111, 112, 5, 61, 0, 0, 112, 113, 5, 61, 0, 0, 113, 114, 5, 61, 0, 0, 114, 115, 5, 61, 0, 0, 115, 116, 5, 61, 0, 0, 116, 117, 5, 61, 0, 0, 117, 118, 5, 61, 0, 0, 118, 10, 1, 0, 0, 0, 119, 120, 5, 42, 0, 0, 120, 121, 5, 42, 0, 0, 121, 122, 5, 42, 0, 0, 122, 123, 5, 42, 0, 0, 123, 124, 5, 42, 0, 0, 124, 12, 1, 0, 0, 0, 125, 127, 5, 13, 0, 0, 126, 125, 1, 0, 0, 0, 126, 127, 1, 0, 0, 0, 127, 128, 1, 0, 0, 0, 128, 129, 5, 10, 0, 0, 129, 14, 1, 0, 0, 0, 130, 131, 5, 111, 0, 0, 131, 16, 1, 0, 0, 0, 132, 133, 5, 120, 0, 0, 133, 18, 1, 0, 0, 0, 134, 135, 5, 50, 0, 0, 135, 136, 3, 91, 45, 0, 136, 137, 3, 91, 45, 0, 137, 138, 3, 91, 45, 0, 138, 139, 3, 49, 24, 0, 139, 140, 3, 95, 47, 0, 140, 141, 3, 91, 45, 0, 141, 142, 3, 49, 24, 0, 142, 143, 3, 93, 46, 0, 143, 144, 3, 91, 45, 0, 144, 20, 1, 0, 0, 0, 145, 146, 2, 48, 50, 0, 146, 147, 3, 91, 45, 0, 147, 148, 2, 48, 53, 0, 148, 149, 3, 91, 45, 0, 149, 22, 1, 0, 0, 0, 150, 151, 3, 47, 23, 0, 151, 152, 3, 35, 17, 0, 152, 24, 1, 0, 0, 0, 153, 154, 3, 45, 22, 0, 154, 155, 3, 35, 17, 0, 155, 26, 1, 0, 0, 0, 156, 157, 3, 83, 41, 0, 157, 158, 3, 35, 17, 0, 158, 28, 1, 0, 0, 0, 159, 160, 5, 80, 0, 0, 160, 161, 3, 91, 45, 0, 161, 30, 1, 0, 0, 0, 162, 167, 3, 99, 49, 0, 163, 166, 3, 99, 49, 0, 164, 166, 3, 55, 27, 0, 165, 163, 1, 0, 0, 0, 165, 164, 1, 0, 0, 0, 166, 169, 1, 0, 0, 0, 167, 165, 1, 0, 0, 0, 167, 168, 1, 0, 0, 0, 168, 32, 1, 0, 0, 0, 169, 167, 1, 0, 0, 0, 170, 171, 3, 35, 17, 0, 171, 172, 3, 63, 31, 0, 172, 173, 3, 89, 44, 0, 173, 175, 3, 89, 44, 0, 174, 176, 3, 89, 44, 0, 175, 174, 1, 0, 0, 0, 175, 176, 1, 0, 0, 0, 176, 34, 1, 0, 0, 0, 177, 178, 3, 91, 45, 0, 178, 179, 3, 91, 45, 0, 179, 180, 3, 95, 47, 0, 180, 181, 3, 91, 45, 0, 181, 182, 3, 93, 46, 0, 182, 183, 3, 91, 45, 0, 183, 36, 1, 0, 0, 0, 184, 189, 3, 91, 45, 0, 185, 188, 3, 99, 49, 0, 186, 188, 3, 55, 27, 0, 187, 185, 1, 0, 0, 0, 187, 186, 1, 0, 0, 0, 188, 191, 1, 0, 0, 0, 189, 187, 1, 0, 0, 0, 189, 190, 1, 0, 0, 0, 190, 38, 1, 0, 0, 0, 191, 189, 1, 0, 0, 0, 192, 193, 5, 32, 0, 0, 193, 194, 5, 32, 0, 0, 194, 195, 5, 45, 0, 0, 195, 40, 1, 0, 0, 0, 196, 197, 5, 32, 0, 0, 197, 198, 5, 32, 0, 0, 198, 199, 5, 32, 0, 0, 199, 200, 5, 32, 0, 0, 200, 201, 5, 45, 0, 0, 201, 42, 1, 0, 0, 0, 202, 203, 7, 0, 0, 0, 203, 44, 1, 0, 0, 0, 204, 205, 5, 36, 0, 0, 205, 46, 1, 0, 0, 0, 206, 207, 5, 94, 0, 0, 207, 48, 1, 0, 0, 0, 208, 209, 5, 45, 0, 0, 209, 50, 1, 0, 0, 0, 210, 211, 5, 46, 0, 0, 211, 52, 1, 0, 0, 0, 212, 213, 5, 47, 0, 0, 213, 54, 1, 0, 0, 0, 214, 215, 5, 95, 0, 0, 215, 56, 1, 0, 0, 0, 216, 217, 5, 32, 0, 0, 217, 58, 1, 0, 0, 0, 218, 219, 5, 40, 0, 0, 219, 60, 1, 0, 0, 0, 220, 221, 5, 41, 0, 0, 221, 62, 1, 0, 0, 0, 222, 223, 5, 35, 0, 0, 223, 64, 1, 0, 0, 0, 224, 225, 5, 64, 0, 0, 225, 66, 1, 0, 0, 0, 226, 227, 5, 43, 0, 0, 227, 68, 1, 0, 0, 0, 228, 229, 5, 37, 0, 0, 229, 70, 1, 0, 0, 0, 230, 231, 5, 39, 0, 0, 231, 72, 1, 0, 0, 0, 232, 233, 5, 34, 0, 0, 233, 74, 1, 0, 0, 0, 234, 235, 5, 126, 0, 0, 235, 76, 1, 0, 0, 0, 236, 237, 5, 42, 0, 0, 237, 78, 1, 0, 0, 0, 238, 239, 5, 60, 0, 0, 239, 80, 1, 0, 0, 0, 240, 241, 5, 62, 0, 0, 241, 82, 1, 0, 0, 0, 242, 243, 5, 58, 0, 0, 243, 84, 1, 0, 0, 0, 244, 245, 2, 65, 90, 0, 245, 86, 1, 0, 0, 0, 246, 247, 2, 97, 122, 0, 247, 88, 1, 0, 0, 0, 248, 251, 3, 91, 45, 0, 249, 251, 7, 1, 0, 0, 250, 248, 1, 0, 0, 0, 250, 249, 1, 0, 0, 0, 251, 90, 1, 0, 0, 0, 252, 253, 2, 48, 57, 0, 253, 92, 1, 0, 0, 0, 254, 255, 2, 48, 51, 0, 255, 94, 1, 0, 0, 0, 256, 257, 2, 48, 49, 0, 257, 96, 1, 0, 0, 0, 258, 261, 3, 85, 42, 0, 259, 261, 3, 87, 43, 0, 260, 258, 1, 0, 0, 0, 260, 259, 1, 0, 0, 0, 261, 98, 1, 0, 0, 0, 262, 265, 3, 97, 48, 0, 263, 265, 3, 91, 45, 0, 264, 262, 1, 0, 0, 0, 264, 263, 1, 0, 0, 0, 265, 100, 1, 0, 0, 0, 10, 0, 126, 165, 167, 175, 187, 189, 250, 260, 264, 0]
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileLexer.py` & `zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryLexer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,171 +1,249 @@
-# Generated from ZorgFile.g4 by ANTLR 4.13.1
+# Generated from ZorgQuery.g4 by ANTLR 4.13.1
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
 
 
 def serializedATN():
     return [
-        4,0,35,234,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,
+        4,0,61,359,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,
         2,6,7,6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,
         13,7,13,2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,
         19,2,20,7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,
         26,7,26,2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,
         32,2,33,7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,
-        39,7,39,2,40,7,40,2,41,7,41,2,42,7,42,1,0,1,0,1,1,1,1,1,2,1,2,1,
-        2,1,3,1,3,1,3,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,5,1,
-        5,1,5,1,6,3,6,113,8,6,1,6,1,6,1,7,1,7,1,8,1,8,1,9,1,9,1,9,1,9,1,
-        9,1,9,1,9,1,9,1,9,1,9,1,9,1,10,1,10,1,10,1,10,1,10,1,11,1,11,1,11,
-        5,11,140,8,11,10,11,12,11,143,9,11,1,12,1,12,1,12,1,12,1,12,1,12,
-        1,12,1,12,1,12,1,12,3,12,155,8,12,1,13,1,13,1,13,5,13,160,8,13,10,
-        13,12,13,163,9,13,1,14,1,14,1,14,1,14,1,15,1,15,1,15,1,15,1,15,1,
-        15,1,16,1,16,1,17,1,17,1,18,1,18,1,19,1,19,1,20,1,20,1,21,1,21,1,
-        22,1,22,1,23,1,23,1,24,1,24,1,25,1,25,1,26,1,26,1,27,1,27,1,28,1,
-        28,1,29,1,29,1,30,1,30,1,31,1,31,1,32,1,32,1,33,1,33,1,34,1,34,1,
-        35,1,35,1,36,1,36,1,37,1,37,3,37,219,8,37,1,38,1,38,1,39,1,39,1,
-        40,1,40,1,41,1,41,3,41,229,8,41,1,42,1,42,3,42,233,8,42,0,0,43,1,
-        1,3,2,5,3,7,4,9,5,11,6,13,7,15,8,17,9,19,10,21,11,23,12,25,13,27,
-        14,29,15,31,16,33,17,35,18,37,19,39,20,41,21,43,22,45,23,47,24,49,
-        25,51,26,53,27,55,28,57,29,59,30,61,31,63,32,65,33,67,34,69,35,71,
-        0,73,0,75,0,77,0,79,0,81,0,83,0,85,0,1,0,2,10,0,33,33,36,36,38,38,
-        44,44,59,59,61,61,63,63,91,94,96,96,123,125,6,0,65,72,74,78,80,90,
-        97,105,107,107,109,122,234,0,1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,0,0,
-        7,1,0,0,0,0,9,1,0,0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,0,17,
-        1,0,0,0,0,19,1,0,0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,0,27,
-        1,0,0,0,0,29,1,0,0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,0,37,
-        1,0,0,0,0,39,1,0,0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,0,47,
-        1,0,0,0,0,49,1,0,0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,0,57,
-        1,0,0,0,0,59,1,0,0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,0,67,
-        1,0,0,0,0,69,1,0,0,0,1,87,1,0,0,0,3,89,1,0,0,0,5,91,1,0,0,0,7,94,
-        1,0,0,0,9,97,1,0,0,0,11,105,1,0,0,0,13,112,1,0,0,0,15,116,1,0,0,
-        0,17,118,1,0,0,0,19,120,1,0,0,0,21,131,1,0,0,0,23,136,1,0,0,0,25,
-        144,1,0,0,0,27,156,1,0,0,0,29,164,1,0,0,0,31,168,1,0,0,0,33,174,
-        1,0,0,0,35,176,1,0,0,0,37,178,1,0,0,0,39,180,1,0,0,0,41,182,1,0,
-        0,0,43,184,1,0,0,0,45,186,1,0,0,0,47,188,1,0,0,0,49,190,1,0,0,0,
-        51,192,1,0,0,0,53,194,1,0,0,0,55,196,1,0,0,0,57,198,1,0,0,0,59,200,
-        1,0,0,0,61,202,1,0,0,0,63,204,1,0,0,0,65,206,1,0,0,0,67,208,1,0,
-        0,0,69,210,1,0,0,0,71,212,1,0,0,0,73,214,1,0,0,0,75,218,1,0,0,0,
-        77,220,1,0,0,0,79,222,1,0,0,0,81,224,1,0,0,0,83,228,1,0,0,0,85,232,
-        1,0,0,0,87,88,5,91,0,0,88,2,1,0,0,0,89,90,5,93,0,0,90,4,1,0,0,0,
-        91,92,5,91,0,0,92,93,5,91,0,0,93,6,1,0,0,0,94,95,5,93,0,0,95,96,
-        5,93,0,0,96,8,1,0,0,0,97,98,5,61,0,0,98,99,5,61,0,0,99,100,5,61,
-        0,0,100,101,5,61,0,0,101,102,5,61,0,0,102,103,5,61,0,0,103,104,5,
-        61,0,0,104,10,1,0,0,0,105,106,5,42,0,0,106,107,5,42,0,0,107,108,
-        5,42,0,0,108,109,5,42,0,0,109,110,5,42,0,0,110,12,1,0,0,0,111,113,
-        5,13,0,0,112,111,1,0,0,0,112,113,1,0,0,0,113,114,1,0,0,0,114,115,
-        5,10,0,0,115,14,1,0,0,0,116,117,5,111,0,0,117,16,1,0,0,0,118,119,
-        5,120,0,0,119,18,1,0,0,0,120,121,5,50,0,0,121,122,3,77,38,0,122,
-        123,3,77,38,0,123,124,3,77,38,0,124,125,3,35,17,0,125,126,3,81,40,
-        0,126,127,3,77,38,0,127,128,3,35,17,0,128,129,3,79,39,0,129,130,
-        3,77,38,0,130,20,1,0,0,0,131,132,2,48,50,0,132,133,3,77,38,0,133,
-        134,2,48,53,0,134,135,3,77,38,0,135,22,1,0,0,0,136,141,3,85,42,0,
-        137,140,3,85,42,0,138,140,3,41,20,0,139,137,1,0,0,0,139,138,1,0,
-        0,0,140,143,1,0,0,0,141,139,1,0,0,0,141,142,1,0,0,0,142,24,1,0,0,
-        0,143,141,1,0,0,0,144,145,3,77,38,0,145,146,3,77,38,0,146,147,3,
-        81,40,0,147,148,3,77,38,0,148,149,3,79,39,0,149,150,3,77,38,0,150,
-        151,3,51,25,0,151,152,3,75,37,0,152,154,3,75,37,0,153,155,3,75,37,
-        0,154,153,1,0,0,0,154,155,1,0,0,0,155,26,1,0,0,0,156,161,3,77,38,
-        0,157,160,3,85,42,0,158,160,3,41,20,0,159,157,1,0,0,0,159,158,1,
-        0,0,0,160,163,1,0,0,0,161,159,1,0,0,0,161,162,1,0,0,0,162,28,1,0,
-        0,0,163,161,1,0,0,0,164,165,5,32,0,0,165,166,5,32,0,0,166,167,5,
-        45,0,0,167,30,1,0,0,0,168,169,5,32,0,0,169,170,5,32,0,0,170,171,
-        5,32,0,0,171,172,5,32,0,0,172,173,5,45,0,0,173,32,1,0,0,0,174,175,
-        7,0,0,0,175,34,1,0,0,0,176,177,5,45,0,0,177,36,1,0,0,0,178,179,5,
-        46,0,0,179,38,1,0,0,0,180,181,5,47,0,0,181,40,1,0,0,0,182,183,5,
-        95,0,0,183,42,1,0,0,0,184,185,5,58,0,0,185,44,1,0,0,0,186,187,5,
-        32,0,0,187,46,1,0,0,0,188,189,5,40,0,0,189,48,1,0,0,0,190,191,5,
-        41,0,0,191,50,1,0,0,0,192,193,5,35,0,0,193,52,1,0,0,0,194,195,5,
-        64,0,0,195,54,1,0,0,0,196,197,5,43,0,0,197,56,1,0,0,0,198,199,5,
-        37,0,0,199,58,1,0,0,0,200,201,5,39,0,0,201,60,1,0,0,0,202,203,5,
-        34,0,0,203,62,1,0,0,0,204,205,5,126,0,0,205,64,1,0,0,0,206,207,5,
-        42,0,0,207,66,1,0,0,0,208,209,5,60,0,0,209,68,1,0,0,0,210,211,5,
-        62,0,0,211,70,1,0,0,0,212,213,2,65,90,0,213,72,1,0,0,0,214,215,2,
-        97,122,0,215,74,1,0,0,0,216,219,3,77,38,0,217,219,7,1,0,0,218,216,
-        1,0,0,0,218,217,1,0,0,0,219,76,1,0,0,0,220,221,2,48,57,0,221,78,
-        1,0,0,0,222,223,2,48,51,0,223,80,1,0,0,0,224,225,2,48,49,0,225,82,
-        1,0,0,0,226,229,3,71,35,0,227,229,3,73,36,0,228,226,1,0,0,0,228,
-        227,1,0,0,0,229,84,1,0,0,0,230,233,3,83,41,0,231,233,3,77,38,0,232,
-        230,1,0,0,0,232,231,1,0,0,0,233,86,1,0,0,0,10,0,112,139,141,154,
-        159,161,218,228,232,0
+        39,7,39,2,40,7,40,2,41,7,41,2,42,7,42,2,43,7,43,2,44,7,44,2,45,7,
+        45,2,46,7,46,2,47,7,47,2,48,7,48,2,49,7,49,2,50,7,50,2,51,7,51,2,
+        52,7,52,2,53,7,53,2,54,7,54,2,55,7,55,2,56,7,56,2,57,7,57,2,58,7,
+        58,2,59,7,59,2,60,7,60,2,61,7,61,2,62,7,62,2,63,7,63,2,64,7,64,2,
+        65,7,65,2,66,7,66,2,67,7,67,2,68,7,68,1,0,1,0,1,1,1,1,1,2,1,2,1,
+        3,1,3,1,4,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,6,1,6,1,7,1,7,1,8,1,8,1,
+        9,1,9,1,10,1,10,1,11,1,11,1,12,1,12,1,13,1,13,1,14,1,14,1,15,1,15,
+        1,16,1,16,1,17,1,17,1,17,1,18,1,18,1,18,1,19,1,19,1,20,1,20,1,20,
+        1,20,1,20,1,20,1,20,1,21,1,21,1,21,1,21,1,21,1,21,1,21,1,22,1,22,
+        1,22,1,22,1,22,1,22,1,22,1,22,1,22,1,23,1,23,1,23,1,23,1,23,1,24,
+        1,24,1,24,1,24,1,24,1,25,3,25,220,8,25,1,25,1,25,1,26,1,26,1,27,
+        1,27,1,28,1,28,1,28,1,28,1,28,1,28,1,28,1,28,1,28,1,28,1,28,1,29,
+        1,29,1,29,1,29,1,29,1,30,1,30,1,30,1,31,1,31,1,31,1,32,1,32,1,32,
+        1,33,1,33,1,33,1,34,1,34,1,34,5,34,259,8,34,10,34,12,34,262,9,34,
+        1,35,1,35,1,35,1,35,1,35,3,35,269,8,35,1,36,1,36,1,36,1,36,1,36,
+        1,36,1,36,1,37,1,37,1,37,5,37,281,8,37,10,37,12,37,284,9,37,1,38,
+        1,38,1,38,1,38,1,39,1,39,1,39,1,39,1,39,1,39,1,40,1,40,1,41,1,41,
+        1,42,1,42,1,43,1,43,1,44,1,44,1,45,1,45,1,46,1,46,1,47,1,47,1,48,
+        1,48,1,49,1,49,1,50,1,50,1,51,1,51,1,52,1,52,1,53,1,53,1,54,1,54,
+        1,55,1,55,1,56,1,56,1,57,1,57,1,58,1,58,1,59,1,59,1,60,1,60,1,61,
+        1,61,1,62,1,62,1,63,1,63,3,63,344,8,63,1,64,1,64,1,65,1,65,1,66,
+        1,66,1,67,1,67,3,67,354,8,67,1,68,1,68,3,68,358,8,68,0,0,69,1,1,
+        3,2,5,3,7,4,9,5,11,6,13,7,15,8,17,9,19,10,21,11,23,12,25,13,27,14,
+        29,15,31,16,33,17,35,18,37,19,39,20,41,21,43,22,45,23,47,24,49,25,
+        51,26,53,27,55,28,57,29,59,30,61,31,63,32,65,33,67,34,69,35,71,36,
+        73,37,75,38,77,39,79,40,81,41,83,42,85,43,87,44,89,45,91,46,93,47,
+        95,48,97,49,99,50,101,51,103,52,105,53,107,54,109,55,111,56,113,
+        57,115,58,117,59,119,60,121,61,123,0,125,0,127,0,129,0,131,0,133,
+        0,135,0,137,0,1,0,2,9,0,33,33,38,38,44,44,59,59,61,61,63,63,91,93,
+        96,96,123,125,6,0,65,72,74,78,80,90,97,105,107,107,109,122,359,0,
+        1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,0,0,7,1,0,0,0,0,9,1,0,0,0,0,11,1,
+        0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,0,17,1,0,0,0,0,19,1,0,0,0,0,21,1,
+        0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,0,27,1,0,0,0,0,29,1,0,0,0,0,31,1,
+        0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,0,37,1,0,0,0,0,39,1,0,0,0,0,41,1,
+        0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,0,47,1,0,0,0,0,49,1,0,0,0,0,51,1,
+        0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,0,57,1,0,0,0,0,59,1,0,0,0,0,61,1,
+        0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,0,67,1,0,0,0,0,69,1,0,0,0,0,71,1,
+        0,0,0,0,73,1,0,0,0,0,75,1,0,0,0,0,77,1,0,0,0,0,79,1,0,0,0,0,81,1,
+        0,0,0,0,83,1,0,0,0,0,85,1,0,0,0,0,87,1,0,0,0,0,89,1,0,0,0,0,91,1,
+        0,0,0,0,93,1,0,0,0,0,95,1,0,0,0,0,97,1,0,0,0,0,99,1,0,0,0,0,101,
+        1,0,0,0,0,103,1,0,0,0,0,105,1,0,0,0,0,107,1,0,0,0,0,109,1,0,0,0,
+        0,111,1,0,0,0,0,113,1,0,0,0,0,115,1,0,0,0,0,117,1,0,0,0,0,119,1,
+        0,0,0,0,121,1,0,0,0,1,139,1,0,0,0,3,141,1,0,0,0,5,143,1,0,0,0,7,
+        145,1,0,0,0,9,147,1,0,0,0,11,152,1,0,0,0,13,155,1,0,0,0,15,157,1,
+        0,0,0,17,159,1,0,0,0,19,161,1,0,0,0,21,163,1,0,0,0,23,165,1,0,0,
+        0,25,167,1,0,0,0,27,169,1,0,0,0,29,171,1,0,0,0,31,173,1,0,0,0,33,
+        175,1,0,0,0,35,177,1,0,0,0,37,180,1,0,0,0,39,183,1,0,0,0,41,185,
+        1,0,0,0,43,192,1,0,0,0,45,199,1,0,0,0,47,208,1,0,0,0,49,213,1,0,
+        0,0,51,219,1,0,0,0,53,223,1,0,0,0,55,225,1,0,0,0,57,227,1,0,0,0,
+        59,238,1,0,0,0,61,243,1,0,0,0,63,246,1,0,0,0,65,249,1,0,0,0,67,252,
+        1,0,0,0,69,255,1,0,0,0,71,263,1,0,0,0,73,270,1,0,0,0,75,277,1,0,
+        0,0,77,285,1,0,0,0,79,289,1,0,0,0,81,295,1,0,0,0,83,297,1,0,0,0,
+        85,299,1,0,0,0,87,301,1,0,0,0,89,303,1,0,0,0,91,305,1,0,0,0,93,307,
+        1,0,0,0,95,309,1,0,0,0,97,311,1,0,0,0,99,313,1,0,0,0,101,315,1,0,
+        0,0,103,317,1,0,0,0,105,319,1,0,0,0,107,321,1,0,0,0,109,323,1,0,
+        0,0,111,325,1,0,0,0,113,327,1,0,0,0,115,329,1,0,0,0,117,331,1,0,
+        0,0,119,333,1,0,0,0,121,335,1,0,0,0,123,337,1,0,0,0,125,339,1,0,
+        0,0,127,343,1,0,0,0,129,345,1,0,0,0,131,347,1,0,0,0,133,349,1,0,
+        0,0,135,353,1,0,0,0,137,357,1,0,0,0,139,140,5,83,0,0,140,2,1,0,0,
+        0,141,142,5,87,0,0,142,4,1,0,0,0,143,144,5,79,0,0,144,6,1,0,0,0,
+        145,146,5,71,0,0,146,8,1,0,0,0,147,148,5,110,0,0,148,149,5,111,0,
+        0,149,150,5,116,0,0,150,151,5,101,0,0,151,10,1,0,0,0,152,153,5,111,
+        0,0,153,154,5,114,0,0,154,12,1,0,0,0,155,156,5,49,0,0,156,14,1,0,
+        0,0,157,158,5,50,0,0,158,16,1,0,0,0,159,160,5,51,0,0,160,18,1,0,
+        0,0,161,162,5,52,0,0,162,20,1,0,0,0,163,164,5,53,0,0,164,22,1,0,
+        0,0,165,166,5,54,0,0,166,24,1,0,0,0,167,168,5,55,0,0,168,26,1,0,
+        0,0,169,170,5,56,0,0,170,28,1,0,0,0,171,172,5,57,0,0,172,30,1,0,
+        0,0,173,174,5,33,0,0,174,32,1,0,0,0,175,176,5,48,0,0,176,34,1,0,
+        0,0,177,178,5,60,0,0,178,179,5,61,0,0,179,36,1,0,0,0,180,181,5,62,
+        0,0,181,182,5,61,0,0,182,38,1,0,0,0,183,184,5,99,0,0,184,40,1,0,
+        0,0,185,186,5,99,0,0,186,187,5,114,0,0,187,188,5,101,0,0,188,189,
+        5,97,0,0,189,190,5,116,0,0,190,191,5,101,0,0,191,42,1,0,0,0,192,
+        193,5,109,0,0,193,194,5,111,0,0,194,195,5,100,0,0,195,196,5,105,
+        0,0,196,197,5,102,0,0,197,198,5,121,0,0,198,44,1,0,0,0,199,200,5,
+        112,0,0,200,201,5,114,0,0,201,202,5,105,0,0,202,203,5,111,0,0,203,
+        204,5,114,0,0,204,205,5,105,0,0,205,206,5,116,0,0,206,207,5,121,
+        0,0,207,46,1,0,0,0,208,209,5,102,0,0,209,210,5,105,0,0,210,211,5,
+        108,0,0,211,212,5,101,0,0,212,48,1,0,0,0,213,214,5,116,0,0,214,215,
+        5,121,0,0,215,216,5,112,0,0,216,217,5,101,0,0,217,50,1,0,0,0,218,
+        220,5,13,0,0,219,218,1,0,0,0,219,220,1,0,0,0,220,221,1,0,0,0,221,
+        222,5,10,0,0,222,52,1,0,0,0,223,224,5,111,0,0,224,54,1,0,0,0,225,
+        226,5,120,0,0,226,56,1,0,0,0,227,228,5,50,0,0,228,229,3,129,64,0,
+        229,230,3,129,64,0,230,231,3,129,64,0,231,232,3,87,43,0,232,233,
+        3,133,66,0,233,234,3,129,64,0,234,235,3,87,43,0,235,236,3,131,65,
+        0,236,237,3,129,64,0,237,58,1,0,0,0,238,239,2,48,50,0,239,240,3,
+        129,64,0,240,241,2,48,53,0,241,242,3,129,64,0,242,60,1,0,0,0,243,
+        244,3,85,42,0,244,245,3,73,36,0,245,62,1,0,0,0,246,247,3,83,41,0,
+        247,248,3,73,36,0,248,64,1,0,0,0,249,250,3,121,60,0,250,251,3,73,
+        36,0,251,66,1,0,0,0,252,253,5,80,0,0,253,254,3,129,64,0,254,68,1,
+        0,0,0,255,260,3,137,68,0,256,259,3,137,68,0,257,259,3,93,46,0,258,
+        256,1,0,0,0,258,257,1,0,0,0,259,262,1,0,0,0,260,258,1,0,0,0,260,
+        261,1,0,0,0,261,70,1,0,0,0,262,260,1,0,0,0,263,264,3,73,36,0,264,
+        265,3,101,50,0,265,266,3,127,63,0,266,268,3,127,63,0,267,269,3,127,
+        63,0,268,267,1,0,0,0,268,269,1,0,0,0,269,72,1,0,0,0,270,271,3,129,
+        64,0,271,272,3,129,64,0,272,273,3,133,66,0,273,274,3,129,64,0,274,
+        275,3,131,65,0,275,276,3,129,64,0,276,74,1,0,0,0,277,282,3,129,64,
+        0,278,281,3,137,68,0,279,281,3,93,46,0,280,278,1,0,0,0,280,279,1,
+        0,0,0,281,284,1,0,0,0,282,280,1,0,0,0,282,283,1,0,0,0,283,76,1,0,
+        0,0,284,282,1,0,0,0,285,286,5,32,0,0,286,287,5,32,0,0,287,288,5,
+        45,0,0,288,78,1,0,0,0,289,290,5,32,0,0,290,291,5,32,0,0,291,292,
+        5,32,0,0,292,293,5,32,0,0,293,294,5,45,0,0,294,80,1,0,0,0,295,296,
+        7,0,0,0,296,82,1,0,0,0,297,298,5,36,0,0,298,84,1,0,0,0,299,300,5,
+        94,0,0,300,86,1,0,0,0,301,302,5,45,0,0,302,88,1,0,0,0,303,304,5,
+        46,0,0,304,90,1,0,0,0,305,306,5,47,0,0,306,92,1,0,0,0,307,308,5,
+        95,0,0,308,94,1,0,0,0,309,310,5,32,0,0,310,96,1,0,0,0,311,312,5,
+        40,0,0,312,98,1,0,0,0,313,314,5,41,0,0,314,100,1,0,0,0,315,316,5,
+        35,0,0,316,102,1,0,0,0,317,318,5,64,0,0,318,104,1,0,0,0,319,320,
+        5,43,0,0,320,106,1,0,0,0,321,322,5,37,0,0,322,108,1,0,0,0,323,324,
+        5,39,0,0,324,110,1,0,0,0,325,326,5,34,0,0,326,112,1,0,0,0,327,328,
+        5,126,0,0,328,114,1,0,0,0,329,330,5,42,0,0,330,116,1,0,0,0,331,332,
+        5,60,0,0,332,118,1,0,0,0,333,334,5,62,0,0,334,120,1,0,0,0,335,336,
+        5,58,0,0,336,122,1,0,0,0,337,338,2,65,90,0,338,124,1,0,0,0,339,340,
+        2,97,122,0,340,126,1,0,0,0,341,344,3,129,64,0,342,344,7,1,0,0,343,
+        341,1,0,0,0,343,342,1,0,0,0,344,128,1,0,0,0,345,346,2,48,57,0,346,
+        130,1,0,0,0,347,348,2,48,51,0,348,132,1,0,0,0,349,350,2,48,49,0,
+        350,134,1,0,0,0,351,354,3,123,61,0,352,354,3,125,62,0,353,351,1,
+        0,0,0,353,352,1,0,0,0,354,136,1,0,0,0,355,358,3,135,67,0,356,358,
+        3,129,64,0,357,355,1,0,0,0,357,356,1,0,0,0,358,138,1,0,0,0,10,0,
+        219,258,260,268,280,282,343,353,357,0
     ]
 
-class ZorgFileLexer(Lexer):
+class ZorgQueryLexer(Lexer):
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
 
     T__0 = 1
     T__1 = 2
     T__2 = 3
     T__3 = 4
     T__4 = 5
     T__5 = 6
-    NL = 7
-    LOWER_O = 8
-    LOWER_X = 9
-    DATE = 10
-    TIME = 11
-    ID = 12
-    ZID = 13
-    NUM_ID = 14
-    TWO_SPACE_DASH = 15
-    FOUR_SPACE_DASH = 16
-    SYMBOL = 17
-    DASH = 18
-    DOT = 19
-    FSLASH = 20
-    UNDERSCORE = 21
-    COLON = 22
-    SPACE = 23
-    LPAREN = 24
-    RPAREN = 25
-    HASH = 26
-    AT_SIGN = 27
-    PLUS = 28
-    PERCENT = 29
-    SQUOTE = 30
-    DQUOTE = 31
-    TILDE = 32
-    STAR = 33
-    LANGLE = 34
-    RANGLE = 35
+    T__6 = 7
+    T__7 = 8
+    T__8 = 9
+    T__9 = 10
+    T__10 = 11
+    T__11 = 12
+    T__12 = 13
+    T__13 = 14
+    T__14 = 15
+    T__15 = 16
+    T__16 = 17
+    T__17 = 18
+    T__18 = 19
+    T__19 = 20
+    T__20 = 21
+    T__21 = 22
+    T__22 = 23
+    T__23 = 24
+    T__24 = 25
+    NL = 26
+    LOWER_O = 27
+    LOWER_X = 28
+    DATE = 29
+    TIME = 30
+    CREATE_RANGE_HEAD = 31
+    MODIFY_RANGE_HEAD = 32
+    DATE_RANGE_TAIL = 33
+    PRIORITY = 34
+    ID = 35
+    ZID = 36
+    SHORT_DATE = 37
+    NUM_ID = 38
+    TWO_SPACE_DASH = 39
+    FOUR_SPACE_DASH = 40
+    SYMBOL = 41
+    DOLLAR = 42
+    HAT = 43
+    DASH = 44
+    DOT = 45
+    FSLASH = 46
+    UNDERSCORE = 47
+    SPACE = 48
+    LPAREN = 49
+    RPAREN = 50
+    HASH = 51
+    AT_SIGN = 52
+    PLUS = 53
+    PERCENT = 54
+    SQUOTE = 55
+    DQUOTE = 56
+    TILDE = 57
+    STAR = 58
+    LANGLE = 59
+    RANGLE = 60
+    COLON = 61
 
     channelNames = [ u"DEFAULT_TOKEN_CHANNEL", u"HIDDEN" ]
 
     modeNames = [ "DEFAULT_MODE" ]
 
     literalNames = [ "<INVALID>",
-            "'['", "']'", "'[['", "']]'", "'======='", "'*****'", "'o'", 
-            "'x'", "'  -'", "'    -'", "'-'", "'.'", "'/'", "'_'", "':'", 
-            "' '", "'('", "')'", "'#'", "'@'", "'+'", "'%'", "'''", "'\"'", 
-            "'~'", "'*'", "'<'", "'>'" ]
+            "'S'", "'W'", "'O'", "'G'", "'note'", "'or'", "'1'", "'2'", 
+            "'3'", "'4'", "'5'", "'6'", "'7'", "'8'", "'9'", "'!'", "'0'", 
+            "'<='", "'>='", "'c'", "'create'", "'modify'", "'priority'", 
+            "'file'", "'type'", "'o'", "'x'", "'  -'", "'    -'", "'$'", 
+            "'^'", "'-'", "'.'", "'/'", "'_'", "' '", "'('", "')'", "'#'", 
+            "'@'", "'+'", "'%'", "'''", "'\"'", "'~'", "'*'", "'<'", "'>'", 
+            "':'" ]
 
     symbolicNames = [ "<INVALID>",
-            "NL", "LOWER_O", "LOWER_X", "DATE", "TIME", "ID", "ZID", "NUM_ID", 
-            "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", "DOT", 
-            "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", "RPAREN", 
-            "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", "DQUOTE", "TILDE", 
-            "STAR", "LANGLE", "RANGLE" ]
-
-    ruleNames = [ "T__0", "T__1", "T__2", "T__3", "T__4", "T__5", "NL", 
-                  "LOWER_O", "LOWER_X", "DATE", "TIME", "ID", "ZID", "NUM_ID", 
-                  "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", 
-                  "DOT", "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", 
-                  "RPAREN", "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", 
-                  "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE", "UPPER_LETTER", 
-                  "LOWER_LETTER", "ZID_CHAR", "NUM", "FIRST_D_NUM", "FIRST_M_NUM", 
-                  "ALPHA", "ALPHANUM" ]
+            "NL", "LOWER_O", "LOWER_X", "DATE", "TIME", "CREATE_RANGE_HEAD", 
+            "MODIFY_RANGE_HEAD", "DATE_RANGE_TAIL", "PRIORITY", "ID", "ZID", 
+            "SHORT_DATE", "NUM_ID", "TWO_SPACE_DASH", "FOUR_SPACE_DASH", 
+            "SYMBOL", "DOLLAR", "HAT", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
+            "SPACE", "LPAREN", "RPAREN", "HASH", "AT_SIGN", "PLUS", "PERCENT", 
+            "SQUOTE", "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE", "COLON" ]
+
+    ruleNames = [ "T__0", "T__1", "T__2", "T__3", "T__4", "T__5", "T__6", 
+                  "T__7", "T__8", "T__9", "T__10", "T__11", "T__12", "T__13", 
+                  "T__14", "T__15", "T__16", "T__17", "T__18", "T__19", 
+                  "T__20", "T__21", "T__22", "T__23", "T__24", "NL", "LOWER_O", 
+                  "LOWER_X", "DATE", "TIME", "CREATE_RANGE_HEAD", "MODIFY_RANGE_HEAD", 
+                  "DATE_RANGE_TAIL", "PRIORITY", "ID", "ZID", "SHORT_DATE", 
+                  "NUM_ID", "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", 
+                  "DOLLAR", "HAT", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
+                  "SPACE", "LPAREN", "RPAREN", "HASH", "AT_SIGN", "PLUS", 
+                  "PERCENT", "SQUOTE", "DQUOTE", "TILDE", "STAR", "LANGLE", 
+                  "RANGLE", "COLON", "UPPER_LETTER", "LOWER_LETTER", "ZID_CHAR", 
+                  "NUM", "FIRST_D_NUM", "FIRST_M_NUM", "ALPHA", "ALPHANUM" ]
 
-    grammarFileName = "ZorgFile.g4"
+    grammarFileName = "ZorgQuery.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.13.1")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileListener.py` & `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileListener.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -166,23 +166,14 @@
         pass
 
     # Exit a parse tree produced by ZorgFileParser#priority.
     def exitPriority(self, ctx:ZorgFileParser.PriorityContext):
         pass
 
 
-    # Enter a parse tree produced by ZorgFileParser#zid.
-    def enterZid(self, ctx:ZorgFileParser.ZidContext):
-        pass
-
-    # Exit a parse tree produced by ZorgFileParser#zid.
-    def exitZid(self, ctx:ZorgFileParser.ZidContext):
-        pass
-
-
     # Enter a parse tree produced by ZorgFileParser#space_atoms.
     def enterSpace_atoms(self, ctx:ZorgFileParser.Space_atomsContext):
         pass
 
     # Exit a parse tree produced by ZorgFileParser#space_atoms.
     def exitSpace_atoms(self, ctx:ZorgFileParser.Space_atomsContext):
         pass
@@ -202,14 +193,23 @@
         pass
 
     # Exit a parse tree produced by ZorgFileParser#atom.
     def exitAtom(self, ctx:ZorgFileParser.AtomContext):
         pass
 
 
+    # Enter a parse tree produced by ZorgFileParser#zid.
+    def enterZid(self, ctx:ZorgFileParser.ZidContext):
+        pass
+
+    # Exit a parse tree produced by ZorgFileParser#zid.
+    def exitZid(self, ctx:ZorgFileParser.ZidContext):
+        pass
+
+
     # Enter a parse tree produced by ZorgFileParser#property.
     def enterProperty(self, ctx:ZorgFileParser.PropertyContext):
         pass
 
     # Exit a parse tree produced by ZorgFileParser#property.
     def exitProperty(self, ctx:ZorgFileParser.PropertyContext):
         pass
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/zorg_file/ZorgFileParser.py` & `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,213 +6,216 @@
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
 	from typing.io import TextIO
 
 def serializedATN():
     return [
-        4,1,35,473,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
+        4,1,42,470,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
         6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,13,7,13,
         2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,19,2,20,
         7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,26,7,26,
         2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,32,2,33,
         7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,39,7,39,
         2,40,7,40,2,41,7,41,2,42,7,42,2,43,7,43,2,44,7,44,2,45,7,45,2,46,
         7,46,2,47,7,47,1,0,1,0,3,0,99,8,0,1,0,1,0,1,1,4,1,104,8,1,11,1,12,
         1,105,1,2,1,2,3,2,110,8,2,1,2,1,2,1,3,4,3,115,8,3,11,3,12,3,116,
         1,3,5,3,120,8,3,10,3,12,3,123,9,3,1,3,5,3,126,8,3,10,3,12,3,129,
         9,3,1,3,5,3,132,8,3,10,3,12,3,135,9,3,1,4,4,4,138,8,4,11,4,12,4,
         139,1,4,5,4,143,8,4,10,4,12,4,146,9,4,1,5,1,5,1,5,1,5,3,5,152,8,
         5,1,6,1,6,1,6,1,6,1,6,1,7,1,7,1,7,5,7,162,8,7,10,7,12,7,165,9,7,
-        1,8,1,8,1,8,1,9,1,9,3,9,172,8,9,1,9,1,9,1,10,1,10,1,10,4,10,179,
-        8,10,11,10,12,10,180,1,10,5,10,184,8,10,10,10,12,10,187,9,10,1,11,
-        1,11,1,11,5,11,192,8,11,10,11,12,11,195,9,11,1,12,1,12,1,12,1,13,
-        1,13,5,13,202,8,13,10,13,12,13,205,9,13,1,14,1,14,1,14,3,14,210,
-        8,14,1,14,1,14,1,14,1,15,1,15,1,15,1,15,3,15,219,8,15,1,16,1,16,
-        1,16,3,16,224,8,16,1,17,1,17,1,17,1,17,1,17,1,18,1,18,1,19,4,19,
-        234,8,19,11,19,12,19,235,1,20,1,20,1,20,3,20,241,8,20,1,20,1,20,
-        5,20,245,8,20,10,20,12,20,248,9,20,1,20,1,20,3,20,252,8,20,1,20,
-        1,20,1,20,5,20,257,8,20,10,20,12,20,260,9,20,3,20,262,8,20,1,20,
-        3,20,265,8,20,1,21,1,21,1,21,1,21,1,21,1,21,1,21,1,21,3,21,275,8,
-        21,1,22,1,22,1,22,1,22,1,22,1,23,1,23,4,23,284,8,23,11,23,12,23,
-        285,1,23,1,23,5,23,290,8,23,10,23,12,23,293,9,23,1,24,1,24,1,24,
-        1,24,1,24,1,24,3,24,301,8,24,1,25,1,25,1,26,1,26,1,27,1,27,1,27,
-        1,27,1,27,3,27,312,8,27,1,28,1,28,1,29,1,29,1,30,1,30,1,31,1,31,
-        1,31,1,31,3,31,324,8,31,1,32,1,32,1,32,1,33,1,33,1,33,1,34,1,34,
-        1,34,1,35,1,35,1,35,1,36,1,36,1,36,1,36,1,36,4,36,343,8,36,11,36,
-        12,36,344,1,36,1,36,1,36,4,36,350,8,36,11,36,12,36,351,1,36,1,36,
-        3,36,356,8,36,1,37,1,37,1,37,1,37,1,38,1,38,1,38,1,38,1,39,1,39,
-        5,39,368,8,39,10,39,12,39,371,9,39,1,39,5,39,374,8,39,10,39,12,39,
-        377,9,39,1,39,3,39,380,8,39,1,39,5,39,383,8,39,10,39,12,39,386,9,
-        39,1,40,1,40,5,40,390,8,40,10,40,12,40,393,9,40,1,40,5,40,396,8,
-        40,10,40,12,40,399,9,40,1,40,3,40,402,8,40,1,40,5,40,405,8,40,10,
-        40,12,40,408,9,40,1,41,1,41,5,41,412,8,41,10,41,12,41,415,9,41,1,
-        41,5,41,418,8,41,10,41,12,41,421,9,41,1,41,3,41,424,8,41,1,41,5,
-        41,427,8,41,10,41,12,41,430,9,41,1,42,1,42,5,42,434,8,42,10,42,12,
-        42,437,9,42,1,42,5,42,440,8,42,10,42,12,42,443,9,42,1,43,1,43,1,
-        43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,44,1,44,1,44,1,
-        44,1,45,1,45,1,45,1,45,1,46,1,46,1,46,1,46,1,46,1,46,1,47,1,47,1,
-        47,0,0,48,0,2,4,6,8,10,12,14,16,18,20,22,24,26,28,30,32,34,36,38,
-        40,42,44,46,48,50,52,54,56,58,60,62,64,66,68,70,72,74,76,78,80,82,
-        84,86,88,90,92,94,0,5,2,0,9,9,32,32,4,0,17,17,21,21,24,25,32,35,
-        2,0,18,20,22,22,1,0,26,29,1,1,7,7,498,0,96,1,0,0,0,2,103,1,0,0,0,
-        4,107,1,0,0,0,6,114,1,0,0,0,8,137,1,0,0,0,10,151,1,0,0,0,12,153,
-        1,0,0,0,14,158,1,0,0,0,16,166,1,0,0,0,18,171,1,0,0,0,20,175,1,0,
-        0,0,22,188,1,0,0,0,24,196,1,0,0,0,26,199,1,0,0,0,28,206,1,0,0,0,
-        30,218,1,0,0,0,32,220,1,0,0,0,34,225,1,0,0,0,36,230,1,0,0,0,38,233,
-        1,0,0,0,40,237,1,0,0,0,42,274,1,0,0,0,44,276,1,0,0,0,46,281,1,0,
-        0,0,48,300,1,0,0,0,50,302,1,0,0,0,52,304,1,0,0,0,54,311,1,0,0,0,
-        56,313,1,0,0,0,58,315,1,0,0,0,60,317,1,0,0,0,62,323,1,0,0,0,64,325,
-        1,0,0,0,66,328,1,0,0,0,68,331,1,0,0,0,70,334,1,0,0,0,72,355,1,0,
-        0,0,74,357,1,0,0,0,76,361,1,0,0,0,78,365,1,0,0,0,80,387,1,0,0,0,
-        82,409,1,0,0,0,84,431,1,0,0,0,86,444,1,0,0,0,88,456,1,0,0,0,90,460,
-        1,0,0,0,92,464,1,0,0,0,94,470,1,0,0,0,96,98,3,2,1,0,97,99,3,6,3,
-        0,98,97,1,0,0,0,98,99,1,0,0,0,99,100,1,0,0,0,100,101,5,0,0,1,101,
-        1,1,0,0,0,102,104,3,4,2,0,103,102,1,0,0,0,104,105,1,0,0,0,105,103,
-        1,0,0,0,105,106,1,0,0,0,106,3,1,0,0,0,107,109,5,26,0,0,108,110,3,
-        38,19,0,109,108,1,0,0,0,109,110,1,0,0,0,110,111,1,0,0,0,111,112,
-        5,7,0,0,112,5,1,0,0,0,113,115,5,7,0,0,114,113,1,0,0,0,115,116,1,
-        0,0,0,116,114,1,0,0,0,116,117,1,0,0,0,117,121,1,0,0,0,118,120,3,
-        8,4,0,119,118,1,0,0,0,120,123,1,0,0,0,121,119,1,0,0,0,121,122,1,
-        0,0,0,122,127,1,0,0,0,123,121,1,0,0,0,124,126,3,80,40,0,125,124,
-        1,0,0,0,126,129,1,0,0,0,127,125,1,0,0,0,127,128,1,0,0,0,128,133,
-        1,0,0,0,129,127,1,0,0,0,130,132,3,78,39,0,131,130,1,0,0,0,132,135,
-        1,0,0,0,133,131,1,0,0,0,133,134,1,0,0,0,134,7,1,0,0,0,135,133,1,
-        0,0,0,136,138,3,10,5,0,137,136,1,0,0,0,138,139,1,0,0,0,139,137,1,
-        0,0,0,139,140,1,0,0,0,140,144,1,0,0,0,141,143,5,7,0,0,142,141,1,
-        0,0,0,143,146,1,0,0,0,144,142,1,0,0,0,144,145,1,0,0,0,145,9,1,0,
-        0,0,146,144,1,0,0,0,147,152,3,26,13,0,148,152,3,14,7,0,149,152,3,
-        12,6,0,150,152,3,4,2,0,151,147,1,0,0,0,151,148,1,0,0,0,151,149,1,
-        0,0,0,151,150,1,0,0,0,152,11,1,0,0,0,153,154,3,76,38,0,154,155,5,
-        22,0,0,155,156,3,38,19,0,156,157,5,7,0,0,157,13,1,0,0,0,158,159,
-        5,18,0,0,159,163,3,16,8,0,160,162,3,22,11,0,161,160,1,0,0,0,162,
-        165,1,0,0,0,163,161,1,0,0,0,163,164,1,0,0,0,164,15,1,0,0,0,165,163,
-        1,0,0,0,166,167,3,18,9,0,167,168,5,7,0,0,168,17,1,0,0,0,169,170,
-        5,23,0,0,170,172,3,36,18,0,171,169,1,0,0,0,171,172,1,0,0,0,172,173,
-        1,0,0,0,173,174,3,20,10,0,174,19,1,0,0,0,175,185,3,38,19,0,176,178,
-        5,7,0,0,177,179,5,23,0,0,178,177,1,0,0,0,179,180,1,0,0,0,180,178,
-        1,0,0,0,180,181,1,0,0,0,181,182,1,0,0,0,182,184,3,38,19,0,183,176,
-        1,0,0,0,184,187,1,0,0,0,185,183,1,0,0,0,185,186,1,0,0,0,186,21,1,
-        0,0,0,187,185,1,0,0,0,188,189,5,15,0,0,189,193,3,16,8,0,190,192,
-        3,24,12,0,191,190,1,0,0,0,192,195,1,0,0,0,193,191,1,0,0,0,193,194,
-        1,0,0,0,194,23,1,0,0,0,195,193,1,0,0,0,196,197,5,16,0,0,197,198,
-        3,16,8,0,198,25,1,0,0,0,199,203,3,28,14,0,200,202,3,22,11,0,201,
-        200,1,0,0,0,202,205,1,0,0,0,203,201,1,0,0,0,203,204,1,0,0,0,204,
-        27,1,0,0,0,205,203,1,0,0,0,206,209,3,30,15,0,207,208,5,23,0,0,208,
-        210,3,34,17,0,209,207,1,0,0,0,209,210,1,0,0,0,210,211,1,0,0,0,211,
-        212,3,18,9,0,212,213,5,7,0,0,213,29,1,0,0,0,214,219,5,8,0,0,215,
-        219,3,32,16,0,216,219,5,34,0,0,217,219,5,35,0,0,218,214,1,0,0,0,
-        218,215,1,0,0,0,218,216,1,0,0,0,218,217,1,0,0,0,219,31,1,0,0,0,220,
-        223,7,0,0,0,221,222,5,22,0,0,222,224,3,52,26,0,223,221,1,0,0,0,223,
-        224,1,0,0,0,224,33,1,0,0,0,225,226,5,1,0,0,226,227,5,26,0,0,227,
-        228,5,12,0,0,228,229,5,2,0,0,229,35,1,0,0,0,230,231,5,13,0,0,231,
-        37,1,0,0,0,232,234,3,40,20,0,233,232,1,0,0,0,234,235,1,0,0,0,235,
-        233,1,0,0,0,235,236,1,0,0,0,236,39,1,0,0,0,237,240,5,23,0,0,238,
-        239,5,30,0,0,239,241,3,56,28,0,240,238,1,0,0,0,240,241,1,0,0,0,241,
-        246,1,0,0,0,242,245,3,56,28,0,243,245,5,31,0,0,244,242,1,0,0,0,244,
-        243,1,0,0,0,245,248,1,0,0,0,246,244,1,0,0,0,246,247,1,0,0,0,247,
-        251,1,0,0,0,248,246,1,0,0,0,249,252,3,42,21,0,250,252,3,72,36,0,
-        251,249,1,0,0,0,251,250,1,0,0,0,251,252,1,0,0,0,252,261,1,0,0,0,
-        253,258,3,54,27,0,254,257,3,54,27,0,255,257,3,48,24,0,256,254,1,
-        0,0,0,256,255,1,0,0,0,257,260,1,0,0,0,258,256,1,0,0,0,258,259,1,
-        0,0,0,259,262,1,0,0,0,260,258,1,0,0,0,261,253,1,0,0,0,261,262,1,
-        0,0,0,262,264,1,0,0,0,263,265,3,76,38,0,264,263,1,0,0,0,264,265,
-        1,0,0,0,265,41,1,0,0,0,266,275,3,60,30,0,267,275,3,62,31,0,268,275,
-        3,74,37,0,269,275,3,44,22,0,270,275,3,46,23,0,271,275,3,76,38,0,
-        272,275,3,36,18,0,273,275,3,34,17,0,274,266,1,0,0,0,274,267,1,0,
-        0,0,274,268,1,0,0,0,274,269,1,0,0,0,274,270,1,0,0,0,274,271,1,0,
-        0,0,274,272,1,0,0,0,274,273,1,0,0,0,275,43,1,0,0,0,276,277,5,12,
-        0,0,277,278,5,22,0,0,278,279,5,22,0,0,279,280,3,46,23,0,280,45,1,
-        0,0,0,281,291,3,48,24,0,282,284,3,58,29,0,283,282,1,0,0,0,284,285,
-        1,0,0,0,285,283,1,0,0,0,285,286,1,0,0,0,286,287,1,0,0,0,287,288,
-        3,48,24,0,288,290,1,0,0,0,289,283,1,0,0,0,290,293,1,0,0,0,291,289,
-        1,0,0,0,291,292,1,0,0,0,292,47,1,0,0,0,293,291,1,0,0,0,294,301,5,
-        12,0,0,295,301,5,14,0,0,296,301,3,50,25,0,297,301,3,52,26,0,298,
-        301,5,8,0,0,299,301,5,9,0,0,300,294,1,0,0,0,300,295,1,0,0,0,300,
-        296,1,0,0,0,300,297,1,0,0,0,300,298,1,0,0,0,300,299,1,0,0,0,301,
-        49,1,0,0,0,302,303,5,10,0,0,303,51,1,0,0,0,304,305,5,11,0,0,305,
-        53,1,0,0,0,306,312,5,30,0,0,307,312,5,31,0,0,308,312,3,56,28,0,309,
-        312,3,60,30,0,310,312,3,58,29,0,311,306,1,0,0,0,311,307,1,0,0,0,
-        311,308,1,0,0,0,311,309,1,0,0,0,311,310,1,0,0,0,312,55,1,0,0,0,313,
-        314,7,1,0,0,314,57,1,0,0,0,315,316,7,2,0,0,316,59,1,0,0,0,317,318,
-        7,3,0,0,318,61,1,0,0,0,319,324,3,64,32,0,320,324,3,66,33,0,321,324,
-        3,68,34,0,322,324,3,70,35,0,323,319,1,0,0,0,323,320,1,0,0,0,323,
-        321,1,0,0,0,323,322,1,0,0,0,324,63,1,0,0,0,325,326,5,26,0,0,326,
-        327,5,12,0,0,327,65,1,0,0,0,328,329,5,27,0,0,329,330,5,12,0,0,330,
-        67,1,0,0,0,331,332,5,29,0,0,332,333,5,12,0,0,333,69,1,0,0,0,334,
-        335,5,28,0,0,335,336,5,12,0,0,336,71,1,0,0,0,337,342,5,30,0,0,338,
-        343,3,42,21,0,339,343,3,34,17,0,340,343,5,3,0,0,341,343,5,4,0,0,
-        342,338,1,0,0,0,342,339,1,0,0,0,342,340,1,0,0,0,342,341,1,0,0,0,
-        343,344,1,0,0,0,344,342,1,0,0,0,344,345,1,0,0,0,345,346,1,0,0,0,
-        346,356,5,30,0,0,347,349,5,31,0,0,348,350,3,42,21,0,349,348,1,0,
-        0,0,350,351,1,0,0,0,351,349,1,0,0,0,351,352,1,0,0,0,352,353,1,0,
-        0,0,353,354,5,31,0,0,354,356,1,0,0,0,355,337,1,0,0,0,355,347,1,0,
-        0,0,356,73,1,0,0,0,357,358,5,3,0,0,358,359,3,46,23,0,359,360,5,4,
-        0,0,360,75,1,0,0,0,361,362,5,1,0,0,362,363,3,46,23,0,363,364,5,2,
-        0,0,364,77,1,0,0,0,365,369,3,86,43,0,366,368,5,7,0,0,367,366,1,0,
-        0,0,368,371,1,0,0,0,369,367,1,0,0,0,369,370,1,0,0,0,370,375,1,0,
-        0,0,371,369,1,0,0,0,372,374,3,8,4,0,373,372,1,0,0,0,374,377,1,0,
-        0,0,375,373,1,0,0,0,375,376,1,0,0,0,376,384,1,0,0,0,377,375,1,0,
-        0,0,378,380,5,7,0,0,379,378,1,0,0,0,379,380,1,0,0,0,380,381,1,0,
-        0,0,381,383,3,80,40,0,382,379,1,0,0,0,383,386,1,0,0,0,384,382,1,
-        0,0,0,384,385,1,0,0,0,385,79,1,0,0,0,386,384,1,0,0,0,387,391,3,88,
-        44,0,388,390,5,7,0,0,389,388,1,0,0,0,390,393,1,0,0,0,391,389,1,0,
-        0,0,391,392,1,0,0,0,392,397,1,0,0,0,393,391,1,0,0,0,394,396,3,8,
-        4,0,395,394,1,0,0,0,396,399,1,0,0,0,397,395,1,0,0,0,397,398,1,0,
-        0,0,398,406,1,0,0,0,399,397,1,0,0,0,400,402,5,7,0,0,401,400,1,0,
-        0,0,401,402,1,0,0,0,402,403,1,0,0,0,403,405,3,82,41,0,404,401,1,
-        0,0,0,405,408,1,0,0,0,406,404,1,0,0,0,406,407,1,0,0,0,407,81,1,0,
-        0,0,408,406,1,0,0,0,409,413,3,90,45,0,410,412,5,7,0,0,411,410,1,
-        0,0,0,412,415,1,0,0,0,413,411,1,0,0,0,413,414,1,0,0,0,414,419,1,
-        0,0,0,415,413,1,0,0,0,416,418,3,8,4,0,417,416,1,0,0,0,418,421,1,
-        0,0,0,419,417,1,0,0,0,419,420,1,0,0,0,420,428,1,0,0,0,421,419,1,
-        0,0,0,422,424,5,7,0,0,423,422,1,0,0,0,423,424,1,0,0,0,424,425,1,
-        0,0,0,425,427,3,84,42,0,426,423,1,0,0,0,427,430,1,0,0,0,428,426,
-        1,0,0,0,428,429,1,0,0,0,429,83,1,0,0,0,430,428,1,0,0,0,431,435,3,
-        92,46,0,432,434,5,7,0,0,433,432,1,0,0,0,434,437,1,0,0,0,435,433,
-        1,0,0,0,435,436,1,0,0,0,436,441,1,0,0,0,437,435,1,0,0,0,438,440,
-        3,8,4,0,439,438,1,0,0,0,440,443,1,0,0,0,441,439,1,0,0,0,441,442,
-        1,0,0,0,442,85,1,0,0,0,443,441,1,0,0,0,444,445,5,26,0,0,445,446,
-        5,26,0,0,446,447,5,26,0,0,447,448,5,26,0,0,448,449,5,26,0,0,449,
-        450,5,26,0,0,450,451,5,26,0,0,451,452,5,26,0,0,452,453,5,26,0,0,
-        453,454,3,38,19,0,454,455,3,94,47,0,455,87,1,0,0,0,456,457,5,5,0,
-        0,457,458,3,38,19,0,458,459,3,94,47,0,459,89,1,0,0,0,460,461,5,6,
-        0,0,461,462,3,38,19,0,462,463,3,94,47,0,463,91,1,0,0,0,464,465,5,
-        18,0,0,465,466,5,18,0,0,466,467,5,18,0,0,467,468,3,38,19,0,468,469,
-        3,94,47,0,469,93,1,0,0,0,470,471,7,4,0,0,471,95,1,0,0,0,52,98,105,
-        109,116,121,127,133,139,144,151,163,171,180,185,193,203,209,218,
-        223,235,240,244,246,251,256,258,261,264,274,285,291,300,311,323,
-        342,344,351,355,369,375,379,384,391,397,401,406,413,419,423,428,
-        435,441
+        1,8,1,8,1,8,1,9,1,9,1,10,1,10,1,10,4,10,175,8,10,11,10,12,10,176,
+        1,10,5,10,180,8,10,10,10,12,10,183,9,10,1,11,1,11,1,11,5,11,188,
+        8,11,10,11,12,11,191,9,11,1,12,1,12,1,12,1,13,1,13,5,13,198,8,13,
+        10,13,12,13,201,9,13,1,14,1,14,1,14,3,14,206,8,14,1,14,1,14,1,14,
+        1,15,1,15,1,15,1,15,3,15,215,8,15,1,16,1,16,1,16,3,16,220,8,16,1,
+        17,1,17,1,18,4,18,225,8,18,11,18,12,18,226,1,19,1,19,1,19,3,19,232,
+        8,19,1,19,1,19,5,19,236,8,19,10,19,12,19,239,9,19,1,19,1,19,3,19,
+        243,8,19,1,19,1,19,1,19,5,19,248,8,19,10,19,12,19,251,9,19,3,19,
+        253,8,19,1,19,3,19,256,8,19,1,20,1,20,1,20,1,20,1,20,1,20,1,20,3,
+        20,265,8,20,1,21,1,21,1,22,1,22,1,22,1,22,1,22,1,23,1,23,4,23,276,
+        8,23,11,23,12,23,277,1,23,1,23,5,23,282,8,23,10,23,12,23,285,9,23,
+        1,24,1,24,1,24,1,24,1,24,1,24,1,24,1,24,1,24,3,24,296,8,24,1,25,
+        1,25,1,26,1,26,1,27,1,27,1,27,1,27,1,27,1,27,1,27,3,27,309,8,27,
+        1,28,1,28,1,29,1,29,1,30,1,30,1,31,1,31,1,31,1,31,3,31,321,8,31,
+        1,32,1,32,1,32,1,33,1,33,1,33,1,34,1,34,1,34,1,35,1,35,1,35,1,36,
+        1,36,1,36,1,36,1,36,4,36,340,8,36,11,36,12,36,341,1,36,1,36,1,36,
+        4,36,347,8,36,11,36,12,36,348,1,36,1,36,3,36,353,8,36,1,37,1,37,
+        1,37,1,37,1,38,1,38,1,38,1,38,1,39,1,39,5,39,365,8,39,10,39,12,39,
+        368,9,39,1,39,5,39,371,8,39,10,39,12,39,374,9,39,1,39,3,39,377,8,
+        39,1,39,5,39,380,8,39,10,39,12,39,383,9,39,1,40,1,40,5,40,387,8,
+        40,10,40,12,40,390,9,40,1,40,5,40,393,8,40,10,40,12,40,396,9,40,
+        1,40,3,40,399,8,40,1,40,5,40,402,8,40,10,40,12,40,405,9,40,1,41,
+        1,41,5,41,409,8,41,10,41,12,41,412,9,41,1,41,5,41,415,8,41,10,41,
+        12,41,418,9,41,1,41,3,41,421,8,41,1,41,5,41,424,8,41,10,41,12,41,
+        427,9,41,1,42,1,42,5,42,431,8,42,10,42,12,42,434,9,42,1,42,5,42,
+        437,8,42,10,42,12,42,440,9,42,1,43,1,43,1,43,1,43,1,43,1,43,1,43,
+        1,43,1,43,1,43,1,43,1,43,1,44,1,44,1,44,1,44,1,45,1,45,1,45,1,45,
+        1,46,1,46,1,46,1,46,1,46,1,46,1,47,1,47,1,47,0,0,48,0,2,4,6,8,10,
+        12,14,16,18,20,22,24,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,
+        56,58,60,62,64,66,68,70,72,74,76,78,80,82,84,86,88,90,92,94,0,5,
+        2,0,9,9,38,38,4,0,22,22,28,28,30,31,38,41,2,0,25,27,42,42,1,0,32,
+        35,1,1,7,7,498,0,96,1,0,0,0,2,103,1,0,0,0,4,107,1,0,0,0,6,114,1,
+        0,0,0,8,137,1,0,0,0,10,151,1,0,0,0,12,153,1,0,0,0,14,158,1,0,0,0,
+        16,166,1,0,0,0,18,169,1,0,0,0,20,171,1,0,0,0,22,184,1,0,0,0,24,192,
+        1,0,0,0,26,195,1,0,0,0,28,202,1,0,0,0,30,214,1,0,0,0,32,216,1,0,
+        0,0,34,221,1,0,0,0,36,224,1,0,0,0,38,228,1,0,0,0,40,264,1,0,0,0,
+        42,266,1,0,0,0,44,268,1,0,0,0,46,273,1,0,0,0,48,295,1,0,0,0,50,297,
+        1,0,0,0,52,299,1,0,0,0,54,308,1,0,0,0,56,310,1,0,0,0,58,312,1,0,
+        0,0,60,314,1,0,0,0,62,320,1,0,0,0,64,322,1,0,0,0,66,325,1,0,0,0,
+        68,328,1,0,0,0,70,331,1,0,0,0,72,352,1,0,0,0,74,354,1,0,0,0,76,358,
+        1,0,0,0,78,362,1,0,0,0,80,384,1,0,0,0,82,406,1,0,0,0,84,428,1,0,
+        0,0,86,441,1,0,0,0,88,453,1,0,0,0,90,457,1,0,0,0,92,461,1,0,0,0,
+        94,467,1,0,0,0,96,98,3,2,1,0,97,99,3,6,3,0,98,97,1,0,0,0,98,99,1,
+        0,0,0,99,100,1,0,0,0,100,101,5,0,0,1,101,1,1,0,0,0,102,104,3,4,2,
+        0,103,102,1,0,0,0,104,105,1,0,0,0,105,103,1,0,0,0,105,106,1,0,0,
+        0,106,3,1,0,0,0,107,109,5,32,0,0,108,110,3,36,18,0,109,108,1,0,0,
+        0,109,110,1,0,0,0,110,111,1,0,0,0,111,112,5,7,0,0,112,5,1,0,0,0,
+        113,115,5,7,0,0,114,113,1,0,0,0,115,116,1,0,0,0,116,114,1,0,0,0,
+        116,117,1,0,0,0,117,121,1,0,0,0,118,120,3,8,4,0,119,118,1,0,0,0,
+        120,123,1,0,0,0,121,119,1,0,0,0,121,122,1,0,0,0,122,127,1,0,0,0,
+        123,121,1,0,0,0,124,126,3,80,40,0,125,124,1,0,0,0,126,129,1,0,0,
+        0,127,125,1,0,0,0,127,128,1,0,0,0,128,133,1,0,0,0,129,127,1,0,0,
+        0,130,132,3,78,39,0,131,130,1,0,0,0,132,135,1,0,0,0,133,131,1,0,
+        0,0,133,134,1,0,0,0,134,7,1,0,0,0,135,133,1,0,0,0,136,138,3,10,5,
+        0,137,136,1,0,0,0,138,139,1,0,0,0,139,137,1,0,0,0,139,140,1,0,0,
+        0,140,144,1,0,0,0,141,143,5,7,0,0,142,141,1,0,0,0,143,146,1,0,0,
+        0,144,142,1,0,0,0,144,145,1,0,0,0,145,9,1,0,0,0,146,144,1,0,0,0,
+        147,152,3,26,13,0,148,152,3,14,7,0,149,152,3,12,6,0,150,152,3,4,
+        2,0,151,147,1,0,0,0,151,148,1,0,0,0,151,149,1,0,0,0,151,150,1,0,
+        0,0,152,11,1,0,0,0,153,154,3,76,38,0,154,155,5,42,0,0,155,156,3,
+        36,18,0,156,157,5,7,0,0,157,13,1,0,0,0,158,159,5,25,0,0,159,163,
+        3,16,8,0,160,162,3,22,11,0,161,160,1,0,0,0,162,165,1,0,0,0,163,161,
+        1,0,0,0,163,164,1,0,0,0,164,15,1,0,0,0,165,163,1,0,0,0,166,167,3,
+        18,9,0,167,168,5,7,0,0,168,17,1,0,0,0,169,170,3,20,10,0,170,19,1,
+        0,0,0,171,181,3,36,18,0,172,174,5,7,0,0,173,175,5,29,0,0,174,173,
+        1,0,0,0,175,176,1,0,0,0,176,174,1,0,0,0,176,177,1,0,0,0,177,178,
+        1,0,0,0,178,180,3,36,18,0,179,172,1,0,0,0,180,183,1,0,0,0,181,179,
+        1,0,0,0,181,182,1,0,0,0,182,21,1,0,0,0,183,181,1,0,0,0,184,185,5,
+        20,0,0,185,189,3,16,8,0,186,188,3,24,12,0,187,186,1,0,0,0,188,191,
+        1,0,0,0,189,187,1,0,0,0,189,190,1,0,0,0,190,23,1,0,0,0,191,189,1,
+        0,0,0,192,193,5,21,0,0,193,194,3,16,8,0,194,25,1,0,0,0,195,199,3,
+        28,14,0,196,198,3,22,11,0,197,196,1,0,0,0,198,201,1,0,0,0,199,197,
+        1,0,0,0,199,200,1,0,0,0,200,27,1,0,0,0,201,199,1,0,0,0,202,205,3,
+        30,15,0,203,204,5,29,0,0,204,206,3,34,17,0,205,203,1,0,0,0,205,206,
+        1,0,0,0,206,207,1,0,0,0,207,208,3,18,9,0,208,209,5,7,0,0,209,29,
+        1,0,0,0,210,215,5,8,0,0,211,215,3,32,16,0,212,215,5,40,0,0,213,215,
+        5,41,0,0,214,210,1,0,0,0,214,211,1,0,0,0,214,212,1,0,0,0,214,213,
+        1,0,0,0,215,31,1,0,0,0,216,219,7,0,0,0,217,218,5,42,0,0,218,220,
+        3,52,26,0,219,217,1,0,0,0,219,220,1,0,0,0,220,33,1,0,0,0,221,222,
+        5,15,0,0,222,35,1,0,0,0,223,225,3,38,19,0,224,223,1,0,0,0,225,226,
+        1,0,0,0,226,224,1,0,0,0,226,227,1,0,0,0,227,37,1,0,0,0,228,231,5,
+        29,0,0,229,230,5,36,0,0,230,232,3,56,28,0,231,229,1,0,0,0,231,232,
+        1,0,0,0,232,237,1,0,0,0,233,236,3,56,28,0,234,236,5,37,0,0,235,233,
+        1,0,0,0,235,234,1,0,0,0,236,239,1,0,0,0,237,235,1,0,0,0,237,238,
+        1,0,0,0,238,242,1,0,0,0,239,237,1,0,0,0,240,243,3,40,20,0,241,243,
+        3,72,36,0,242,240,1,0,0,0,242,241,1,0,0,0,242,243,1,0,0,0,243,252,
+        1,0,0,0,244,249,3,54,27,0,245,248,3,54,27,0,246,248,3,48,24,0,247,
+        245,1,0,0,0,247,246,1,0,0,0,248,251,1,0,0,0,249,247,1,0,0,0,249,
+        250,1,0,0,0,250,253,1,0,0,0,251,249,1,0,0,0,252,244,1,0,0,0,252,
+        253,1,0,0,0,253,255,1,0,0,0,254,256,3,76,38,0,255,254,1,0,0,0,255,
+        256,1,0,0,0,256,39,1,0,0,0,257,265,3,60,30,0,258,265,3,62,31,0,259,
+        265,3,74,37,0,260,265,3,44,22,0,261,265,3,46,23,0,262,265,3,76,38,
+        0,263,265,3,34,17,0,264,257,1,0,0,0,264,258,1,0,0,0,264,259,1,0,
+        0,0,264,260,1,0,0,0,264,261,1,0,0,0,264,262,1,0,0,0,264,263,1,0,
+        0,0,265,41,1,0,0,0,266,267,5,17,0,0,267,43,1,0,0,0,268,269,5,16,
+        0,0,269,270,5,42,0,0,270,271,5,42,0,0,271,272,3,46,23,0,272,45,1,
+        0,0,0,273,283,3,48,24,0,274,276,3,58,29,0,275,274,1,0,0,0,276,277,
+        1,0,0,0,277,275,1,0,0,0,277,278,1,0,0,0,278,279,1,0,0,0,279,280,
+        3,48,24,0,280,282,1,0,0,0,281,275,1,0,0,0,282,285,1,0,0,0,283,281,
+        1,0,0,0,283,284,1,0,0,0,284,47,1,0,0,0,285,283,1,0,0,0,286,296,5,
+        16,0,0,287,296,5,19,0,0,288,296,5,14,0,0,289,296,5,15,0,0,290,296,
+        3,50,25,0,291,296,3,52,26,0,292,296,3,42,21,0,293,296,5,8,0,0,294,
+        296,5,9,0,0,295,286,1,0,0,0,295,287,1,0,0,0,295,288,1,0,0,0,295,
+        289,1,0,0,0,295,290,1,0,0,0,295,291,1,0,0,0,295,292,1,0,0,0,295,
+        293,1,0,0,0,295,294,1,0,0,0,296,49,1,0,0,0,297,298,5,10,0,0,298,
+        51,1,0,0,0,299,300,5,11,0,0,300,53,1,0,0,0,301,309,5,36,0,0,302,
+        309,5,37,0,0,303,309,5,24,0,0,304,309,5,23,0,0,305,309,3,56,28,0,
+        306,309,3,60,30,0,307,309,3,58,29,0,308,301,1,0,0,0,308,302,1,0,
+        0,0,308,303,1,0,0,0,308,304,1,0,0,0,308,305,1,0,0,0,308,306,1,0,
+        0,0,308,307,1,0,0,0,309,55,1,0,0,0,310,311,7,1,0,0,311,57,1,0,0,
+        0,312,313,7,2,0,0,313,59,1,0,0,0,314,315,7,3,0,0,315,61,1,0,0,0,
+        316,321,3,64,32,0,317,321,3,66,33,0,318,321,3,68,34,0,319,321,3,
+        70,35,0,320,316,1,0,0,0,320,317,1,0,0,0,320,318,1,0,0,0,320,319,
+        1,0,0,0,321,63,1,0,0,0,322,323,5,32,0,0,323,324,5,16,0,0,324,65,
+        1,0,0,0,325,326,5,33,0,0,326,327,5,16,0,0,327,67,1,0,0,0,328,329,
+        5,35,0,0,329,330,5,16,0,0,330,69,1,0,0,0,331,332,5,34,0,0,332,333,
+        5,16,0,0,333,71,1,0,0,0,334,339,5,36,0,0,335,340,3,40,20,0,336,340,
+        3,34,17,0,337,340,5,1,0,0,338,340,5,2,0,0,339,335,1,0,0,0,339,336,
+        1,0,0,0,339,337,1,0,0,0,339,338,1,0,0,0,340,341,1,0,0,0,341,339,
+        1,0,0,0,341,342,1,0,0,0,342,343,1,0,0,0,343,353,5,36,0,0,344,346,
+        5,37,0,0,345,347,3,40,20,0,346,345,1,0,0,0,347,348,1,0,0,0,348,346,
+        1,0,0,0,348,349,1,0,0,0,349,350,1,0,0,0,350,351,5,37,0,0,351,353,
+        1,0,0,0,352,334,1,0,0,0,352,344,1,0,0,0,353,73,1,0,0,0,354,355,5,
+        1,0,0,355,356,3,46,23,0,356,357,5,2,0,0,357,75,1,0,0,0,358,359,5,
+        3,0,0,359,360,3,46,23,0,360,361,5,4,0,0,361,77,1,0,0,0,362,366,3,
+        86,43,0,363,365,5,7,0,0,364,363,1,0,0,0,365,368,1,0,0,0,366,364,
+        1,0,0,0,366,367,1,0,0,0,367,372,1,0,0,0,368,366,1,0,0,0,369,371,
+        3,8,4,0,370,369,1,0,0,0,371,374,1,0,0,0,372,370,1,0,0,0,372,373,
+        1,0,0,0,373,381,1,0,0,0,374,372,1,0,0,0,375,377,5,7,0,0,376,375,
+        1,0,0,0,376,377,1,0,0,0,377,378,1,0,0,0,378,380,3,80,40,0,379,376,
+        1,0,0,0,380,383,1,0,0,0,381,379,1,0,0,0,381,382,1,0,0,0,382,79,1,
+        0,0,0,383,381,1,0,0,0,384,388,3,88,44,0,385,387,5,7,0,0,386,385,
+        1,0,0,0,387,390,1,0,0,0,388,386,1,0,0,0,388,389,1,0,0,0,389,394,
+        1,0,0,0,390,388,1,0,0,0,391,393,3,8,4,0,392,391,1,0,0,0,393,396,
+        1,0,0,0,394,392,1,0,0,0,394,395,1,0,0,0,395,403,1,0,0,0,396,394,
+        1,0,0,0,397,399,5,7,0,0,398,397,1,0,0,0,398,399,1,0,0,0,399,400,
+        1,0,0,0,400,402,3,82,41,0,401,398,1,0,0,0,402,405,1,0,0,0,403,401,
+        1,0,0,0,403,404,1,0,0,0,404,81,1,0,0,0,405,403,1,0,0,0,406,410,3,
+        90,45,0,407,409,5,7,0,0,408,407,1,0,0,0,409,412,1,0,0,0,410,408,
+        1,0,0,0,410,411,1,0,0,0,411,416,1,0,0,0,412,410,1,0,0,0,413,415,
+        3,8,4,0,414,413,1,0,0,0,415,418,1,0,0,0,416,414,1,0,0,0,416,417,
+        1,0,0,0,417,425,1,0,0,0,418,416,1,0,0,0,419,421,5,7,0,0,420,419,
+        1,0,0,0,420,421,1,0,0,0,421,422,1,0,0,0,422,424,3,84,42,0,423,420,
+        1,0,0,0,424,427,1,0,0,0,425,423,1,0,0,0,425,426,1,0,0,0,426,83,1,
+        0,0,0,427,425,1,0,0,0,428,432,3,92,46,0,429,431,5,7,0,0,430,429,
+        1,0,0,0,431,434,1,0,0,0,432,430,1,0,0,0,432,433,1,0,0,0,433,438,
+        1,0,0,0,434,432,1,0,0,0,435,437,3,8,4,0,436,435,1,0,0,0,437,440,
+        1,0,0,0,438,436,1,0,0,0,438,439,1,0,0,0,439,85,1,0,0,0,440,438,1,
+        0,0,0,441,442,5,32,0,0,442,443,5,32,0,0,443,444,5,32,0,0,444,445,
+        5,32,0,0,445,446,5,32,0,0,446,447,5,32,0,0,447,448,5,32,0,0,448,
+        449,5,32,0,0,449,450,5,32,0,0,450,451,3,36,18,0,451,452,3,94,47,
+        0,452,87,1,0,0,0,453,454,5,5,0,0,454,455,3,36,18,0,455,456,3,94,
+        47,0,456,89,1,0,0,0,457,458,5,6,0,0,458,459,3,36,18,0,459,460,3,
+        94,47,0,460,91,1,0,0,0,461,462,5,25,0,0,462,463,5,25,0,0,463,464,
+        5,25,0,0,464,465,3,36,18,0,465,466,3,94,47,0,466,93,1,0,0,0,467,
+        468,7,4,0,0,468,95,1,0,0,0,51,98,105,109,116,121,127,133,139,144,
+        151,163,176,181,189,199,205,214,219,226,231,235,237,242,247,249,
+        252,255,264,277,283,295,308,320,339,341,348,352,366,372,376,381,
+        388,394,398,403,410,416,420,425,432,438
     ]
 
 class ZorgFileParser ( Parser ):
 
     grammarFileName = "ZorgFile.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
 
     sharedContextCache = PredictionContextCache()
 
-    literalNames = [ "<INVALID>", "'['", "']'", "'[['", "']]'", "'======='", 
+    literalNames = [ "<INVALID>", "'[['", "']]'", "'['", "']'", "'======='", 
                      "'*****'", "<INVALID>", "'o'", "'x'", "<INVALID>", 
                      "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
-                     "'  -'", "'    -'", "<INVALID>", "'-'", "'.'", "'/'", 
-                     "'_'", "':'", "' '", "'('", "')'", "'#'", "'@'", "'+'", 
-                     "'%'", "'''", "'\"'", "'~'", "'*'", "'<'", "'>'" ]
+                     "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
+                     "<INVALID>", "'  -'", "'    -'", "<INVALID>", "'$'", 
+                     "'^'", "'-'", "'.'", "'/'", "'_'", "' '", "'('", "')'", 
+                     "'#'", "'@'", "'+'", "'%'", "'''", "'\"'", "'~'", "'*'", 
+                     "'<'", "'>'", "':'" ]
 
     symbolicNames = [ "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "<INVALID>", "NL", "LOWER_O", 
-                      "LOWER_X", "DATE", "TIME", "ID", "ZID", "NUM_ID", 
-                      "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", 
-                      "DOT", "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", 
-                      "RPAREN", "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", 
-                      "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE" ]
+                      "LOWER_X", "DATE", "TIME", "CREATE_RANGE_HEAD", "MODIFY_RANGE_HEAD", 
+                      "DATE_RANGE_TAIL", "PRIORITY", "ID", "ZID", "SHORT_DATE", 
+                      "NUM_ID", "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", 
+                      "DOLLAR", "HAT", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
+                      "SPACE", "LPAREN", "RPAREN", "HASH", "AT_SIGN", "PLUS", 
+                      "PERCENT", "SQUOTE", "DQUOTE", "TILDE", "STAR", "LANGLE", 
+                      "RANGLE", "COLON" ]
 
     RULE_prog = 0
     RULE_head = 1
     RULE_comment = 2
     RULE_body = 3
     RULE_block = 4
     RULE_item = 5
@@ -224,18 +227,18 @@
     RULE_subnote = 11
     RULE_subsubnote = 12
     RULE_todo = 13
     RULE_base_todo = 14
     RULE_todo_prefix = 15
     RULE_x_or_tilde = 16
     RULE_priority = 17
-    RULE_zid = 18
-    RULE_space_atoms = 19
-    RULE_space_atom = 20
-    RULE_atom = 21
+    RULE_space_atoms = 18
+    RULE_space_atom = 19
+    RULE_atom = 20
+    RULE_zid = 21
     RULE_property = 22
     RULE_id_group = 23
     RULE_id = 24
     RULE_date = 25
     RULE_time = 26
     RULE_any_symbol = 27
     RULE_non_tag_symbol = 28
@@ -258,15 +261,15 @@
     RULE_h3_header = 45
     RULE_h4_header = 46
     RULE_eol = 47
 
     ruleNames =  [ "prog", "head", "comment", "body", "block", "item", "footnote", 
                    "note", "base_note", "id_note_body", "note_body", "subnote", 
                    "subsubnote", "todo", "base_todo", "todo_prefix", "x_or_tilde", 
-                   "priority", "zid", "space_atoms", "space_atom", "atom", 
+                   "priority", "space_atoms", "space_atom", "atom", "zid", 
                    "property", "id_group", "id", "date", "time", "any_symbol", 
                    "non_tag_symbol", "id_symbol", "tag_symbol", "tag", "area", 
                    "context", "person", "project", "quoted", "link", "ref", 
                    "h1_section", "h2_section", "h3_section", "h4_section", 
                    "h1_header", "h2_header", "h3_header", "h4_header", "eol" ]
 
     EOF = Token.EOF
@@ -277,38 +280,45 @@
     T__4=5
     T__5=6
     NL=7
     LOWER_O=8
     LOWER_X=9
     DATE=10
     TIME=11
-    ID=12
-    ZID=13
-    NUM_ID=14
-    TWO_SPACE_DASH=15
-    FOUR_SPACE_DASH=16
-    SYMBOL=17
-    DASH=18
-    DOT=19
-    FSLASH=20
-    UNDERSCORE=21
-    COLON=22
-    SPACE=23
-    LPAREN=24
-    RPAREN=25
-    HASH=26
-    AT_SIGN=27
-    PLUS=28
-    PERCENT=29
-    SQUOTE=30
-    DQUOTE=31
-    TILDE=32
-    STAR=33
-    LANGLE=34
-    RANGLE=35
+    CREATE_RANGE_HEAD=12
+    MODIFY_RANGE_HEAD=13
+    DATE_RANGE_TAIL=14
+    PRIORITY=15
+    ID=16
+    ZID=17
+    SHORT_DATE=18
+    NUM_ID=19
+    TWO_SPACE_DASH=20
+    FOUR_SPACE_DASH=21
+    SYMBOL=22
+    DOLLAR=23
+    HAT=24
+    DASH=25
+    DOT=26
+    FSLASH=27
+    UNDERSCORE=28
+    SPACE=29
+    LPAREN=30
+    RPAREN=31
+    HASH=32
+    AT_SIGN=33
+    PLUS=34
+    PERCENT=35
+    SQUOTE=36
+    DQUOTE=37
+    TILDE=38
+    STAR=39
+    LANGLE=40
+    RANGLE=41
+    COLON=42
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.13.1")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
@@ -415,15 +425,15 @@
             _la = self._input.LA(1)
             while True:
                 self.state = 102
                 self.comment()
                 self.state = 105 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if not (_la==26):
+                if not (_la==32):
                     break
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -470,15 +480,15 @@
         try:
             self.enterOuterAlt(localctx, 1)
             self.state = 107
             self.match(ZorgFileParser.HASH)
             self.state = 109
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==23:
+            if _la==29:
                 self.state = 108
                 self.space_atoms()
 
 
             self.state = 111
             self.match(ZorgFileParser.NL)
         except RecognitionException as re:
@@ -577,15 +587,15 @@
                 self.state = 129
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
             self.state = 133
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while _la==26:
+            while _la==32:
                 self.state = 130
                 self.h1_section()
                 self.state = 135
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
@@ -712,30 +722,30 @@
 
         localctx = ZorgFileParser.ItemContext(self, self._ctx, self.state)
         self.enterRule(localctx, 10, self.RULE_item)
         try:
             self.state = 151
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [8, 9, 32, 34, 35]:
+            if token in [8, 9, 38, 40, 41]:
                 self.enterOuterAlt(localctx, 1)
                 self.state = 147
                 self.todo()
                 pass
-            elif token in [18]:
+            elif token in [25]:
                 self.enterOuterAlt(localctx, 2)
                 self.state = 148
                 self.note()
                 pass
-            elif token in [1]:
+            elif token in [3]:
                 self.enterOuterAlt(localctx, 3)
                 self.state = 149
                 self.footnote()
                 pass
-            elif token in [26]:
+            elif token in [32]:
                 self.enterOuterAlt(localctx, 4)
                 self.state = 150
                 self.comment()
                 pass
             else:
                 raise NoViableAltException(self)
 
@@ -851,15 +861,15 @@
             self.state = 158
             self.match(ZorgFileParser.DASH)
             self.state = 159
             self.base_note()
             self.state = 163
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while _la==15:
+            while _la==20:
                 self.state = 160
                 self.subnote()
                 self.state = 165
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
@@ -925,21 +935,14 @@
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def note_body(self):
             return self.getTypedRuleContext(ZorgFileParser.Note_bodyContext,0)
 
 
-        def SPACE(self):
-            return self.getToken(ZorgFileParser.SPACE, 0)
-
-        def zid(self):
-            return self.getTypedRuleContext(ZorgFileParser.ZidContext,0)
-
-
         def getRuleIndex(self):
             return ZorgFileParser.RULE_id_note_body
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterId_note_body" ):
                 listener.enterId_note_body(self)
 
@@ -952,25 +955,15 @@
 
     def id_note_body(self):
 
         localctx = ZorgFileParser.Id_note_bodyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 18, self.RULE_id_note_body)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 171
-            self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,11,self._ctx)
-            if la_ == 1:
-                self.state = 169
-                self.match(ZorgFileParser.SPACE)
-                self.state = 170
-                self.zid()
-
-
-            self.state = 173
+            self.state = 169
             self.note_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1019,42 +1012,42 @@
 
     def note_body(self):
 
         localctx = ZorgFileParser.Note_bodyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 20, self.RULE_note_body)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 175
+            self.state = 171
             self.space_atoms()
-            self.state = 185
+            self.state = 181
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,13,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,12,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 176
+                    self.state = 172
                     self.match(ZorgFileParser.NL)
-                    self.state = 178 
+                    self.state = 174 
                     self._errHandler.sync(self)
                     _alt = 1
                     while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                         if _alt == 1:
-                            self.state = 177
+                            self.state = 173
                             self.match(ZorgFileParser.SPACE)
 
                         else:
                             raise NoViableAltException(self)
-                        self.state = 180 
+                        self.state = 176 
                         self._errHandler.sync(self)
-                        _alt = self._interp.adaptivePredict(self._input,12,self._ctx)
+                        _alt = self._interp.adaptivePredict(self._input,11,self._ctx)
 
-                    self.state = 182
+                    self.state = 178
                     self.space_atoms() 
-                self.state = 187
+                self.state = 183
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,13,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,12,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1099,25 +1092,25 @@
     def subnote(self):
 
         localctx = ZorgFileParser.SubnoteContext(self, self._ctx, self.state)
         self.enterRule(localctx, 22, self.RULE_subnote)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 188
+            self.state = 184
             self.match(ZorgFileParser.TWO_SPACE_DASH)
-            self.state = 189
+            self.state = 185
             self.base_note()
-            self.state = 193
+            self.state = 189
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while _la==16:
-                self.state = 190
+            while _la==21:
+                self.state = 186
                 self.subsubnote()
-                self.state = 195
+                self.state = 191
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1156,17 +1149,17 @@
 
     def subsubnote(self):
 
         localctx = ZorgFileParser.SubsubnoteContext(self, self._ctx, self.state)
         self.enterRule(localctx, 24, self.RULE_subsubnote)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 196
+            self.state = 192
             self.match(ZorgFileParser.FOUR_SPACE_DASH)
-            self.state = 197
+            self.state = 193
             self.base_note()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1208,23 +1201,23 @@
     def todo(self):
 
         localctx = ZorgFileParser.TodoContext(self, self._ctx, self.state)
         self.enterRule(localctx, 26, self.RULE_todo)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 199
+            self.state = 195
             self.base_todo()
-            self.state = 203
+            self.state = 199
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while _la==15:
-                self.state = 200
+            while _la==20:
+                self.state = 196
                 self.subnote()
-                self.state = 205
+                self.state = 201
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1274,29 +1267,29 @@
 
     def base_todo(self):
 
         localctx = ZorgFileParser.Base_todoContext(self, self._ctx, self.state)
         self.enterRule(localctx, 28, self.RULE_base_todo)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 206
+            self.state = 202
             self.todo_prefix()
-            self.state = 209
+            self.state = 205
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,16,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,15,self._ctx)
             if la_ == 1:
-                self.state = 207
+                self.state = 203
                 self.match(ZorgFileParser.SPACE)
-                self.state = 208
+                self.state = 204
                 self.priority()
 
 
-            self.state = 211
+            self.state = 207
             self.id_note_body()
-            self.state = 212
+            self.state = 208
             self.match(ZorgFileParser.NL)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1339,31 +1332,31 @@
 
     def todo_prefix(self):
 
         localctx = ZorgFileParser.Todo_prefixContext(self, self._ctx, self.state)
         self.enterRule(localctx, 30, self.RULE_todo_prefix)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 218
+            self.state = 214
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [8]:
-                self.state = 214
+                self.state = 210
                 self.match(ZorgFileParser.LOWER_O)
                 pass
-            elif token in [9, 32]:
-                self.state = 215
+            elif token in [9, 38]:
+                self.state = 211
                 self.x_or_tilde()
                 pass
-            elif token in [34]:
-                self.state = 216
+            elif token in [40]:
+                self.state = 212
                 self.match(ZorgFileParser.LANGLE)
                 pass
-            elif token in [35]:
-                self.state = 217
+            elif token in [41]:
+                self.state = 213
                 self.match(ZorgFileParser.RANGLE)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -1411,28 +1404,28 @@
     def x_or_tilde(self):
 
         localctx = ZorgFileParser.X_or_tildeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 32, self.RULE_x_or_tilde)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 220
+            self.state = 216
             _la = self._input.LA(1)
-            if not(_la==9 or _la==32):
+            if not(_la==9 or _la==38):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
-            self.state = 223
+            self.state = 219
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==22:
-                self.state = 221
+            if _la==42:
+                self.state = 217
                 self.match(ZorgFileParser.COLON)
-                self.state = 222
+                self.state = 218
                 self.time()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1444,19 +1437,16 @@
     class PriorityContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def HASH(self):
-            return self.getToken(ZorgFileParser.HASH, 0)
-
-        def ID(self):
-            return self.getToken(ZorgFileParser.ID, 0)
+        def PRIORITY(self):
+            return self.getToken(ZorgFileParser.PRIORITY, 0)
 
         def getRuleIndex(self):
             return ZorgFileParser.RULE_priority
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterPriority" ):
                 listener.enterPriority(self)
@@ -1470,63 +1460,16 @@
 
     def priority(self):
 
         localctx = ZorgFileParser.PriorityContext(self, self._ctx, self.state)
         self.enterRule(localctx, 34, self.RULE_priority)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 225
-            self.match(ZorgFileParser.T__0)
-            self.state = 226
-            self.match(ZorgFileParser.HASH)
-            self.state = 227
-            self.match(ZorgFileParser.ID)
-            self.state = 228
-            self.match(ZorgFileParser.T__1)
-        except RecognitionException as re:
-            localctx.exception = re
-            self._errHandler.reportError(self, re)
-            self._errHandler.recover(self, re)
-        finally:
-            self.exitRule()
-        return localctx
-
-
-    class ZidContext(ParserRuleContext):
-        __slots__ = 'parser'
-
-        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
-            super().__init__(parent, invokingState)
-            self.parser = parser
-
-        def ZID(self):
-            return self.getToken(ZorgFileParser.ZID, 0)
-
-        def getRuleIndex(self):
-            return ZorgFileParser.RULE_zid
-
-        def enterRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "enterZid" ):
-                listener.enterZid(self)
-
-        def exitRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "exitZid" ):
-                listener.exitZid(self)
-
-
-
-
-    def zid(self):
-
-        localctx = ZorgFileParser.ZidContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 36, self.RULE_zid)
-        try:
-            self.enterOuterAlt(localctx, 1)
-            self.state = 230
-            self.match(ZorgFileParser.ZID)
+            self.state = 221
+            self.match(ZorgFileParser.PRIORITY)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -1559,28 +1502,28 @@
 
 
 
 
     def space_atoms(self):
 
         localctx = ZorgFileParser.Space_atomsContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 38, self.RULE_space_atoms)
+        self.enterRule(localctx, 36, self.RULE_space_atoms)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 233 
+            self.state = 224 
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while True:
-                self.state = 232
+                self.state = 223
                 self.space_atom()
-                self.state = 235 
+                self.state = 226 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if not (_la==23):
+                if not (_la==29):
                     break
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -1653,100 +1596,100 @@
 
 
 
 
     def space_atom(self):
 
         localctx = ZorgFileParser.Space_atomContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 40, self.RULE_space_atom)
+        self.enterRule(localctx, 38, self.RULE_space_atom)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 237
+            self.state = 228
             self.match(ZorgFileParser.SPACE)
-            self.state = 240
+            self.state = 231
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,20,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,19,self._ctx)
             if la_ == 1:
-                self.state = 238
+                self.state = 229
                 self.match(ZorgFileParser.SQUOTE)
-                self.state = 239
+                self.state = 230
                 self.non_tag_symbol()
 
 
-            self.state = 246
+            self.state = 237
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,22,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,21,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 244
+                    self.state = 235
                     self._errHandler.sync(self)
                     token = self._input.LA(1)
-                    if token in [17, 21, 24, 25, 32, 33, 34, 35]:
-                        self.state = 242
+                    if token in [22, 28, 30, 31, 38, 39, 40, 41]:
+                        self.state = 233
                         self.non_tag_symbol()
                         pass
-                    elif token in [31]:
-                        self.state = 243
+                    elif token in [37]:
+                        self.state = 234
                         self.match(ZorgFileParser.DQUOTE)
                         pass
                     else:
                         raise NoViableAltException(self)
              
-                self.state = 248
+                self.state = 239
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,22,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,21,self._ctx)
 
-            self.state = 251
+            self.state = 242
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,23,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,22,self._ctx)
             if la_ == 1:
-                self.state = 249
+                self.state = 240
                 self.atom()
 
             elif la_ == 2:
-                self.state = 250
+                self.state = 241
                 self.quoted()
 
 
-            self.state = 261
+            self.state = 252
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if (((_la) & ~0x3f) == 0 and ((1 << _la) & 68710957056) != 0):
-                self.state = 253
+            if (((_la) & ~0x3f) == 0 and ((1 << _la) & 8795551956992) != 0):
+                self.state = 244
                 self.any_symbol()
-                self.state = 258
+                self.state = 249
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while (((_la) & ~0x3f) == 0 and ((1 << _la) & 68710981376) != 0):
-                    self.state = 256
+                while (((_la) & ~0x3f) == 0 and ((1 << _la) & 8795552730880) != 0):
+                    self.state = 247
                     self._errHandler.sync(self)
                     token = self._input.LA(1)
-                    if token in [17, 18, 19, 20, 21, 22, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34, 35]:
-                        self.state = 254
+                    if token in [22, 23, 24, 25, 26, 27, 28, 30, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42]:
+                        self.state = 245
                         self.any_symbol()
                         pass
-                    elif token in [8, 9, 10, 11, 12, 14]:
-                        self.state = 255
+                    elif token in [8, 9, 10, 11, 14, 15, 16, 17, 19]:
+                        self.state = 246
                         self.id_()
                         pass
                     else:
                         raise NoViableAltException(self)
 
-                    self.state = 260
+                    self.state = 251
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
 
 
-            self.state = 264
+            self.state = 255
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==1:
-                self.state = 263
+            if _la==3:
+                self.state = 254
                 self.ref()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1782,18 +1725,14 @@
             return self.getTypedRuleContext(ZorgFileParser.Id_groupContext,0)
 
 
         def ref(self):
             return self.getTypedRuleContext(ZorgFileParser.RefContext,0)
 
 
-        def zid(self):
-            return self.getTypedRuleContext(ZorgFileParser.ZidContext,0)
-
-
         def priority(self):
             return self.getTypedRuleContext(ZorgFileParser.PriorityContext,0)
 
 
         def getRuleIndex(self):
             return ZorgFileParser.RULE_atom
 
@@ -1807,77 +1746,112 @@
 
 
 
 
     def atom(self):
 
         localctx = ZorgFileParser.AtomContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 42, self.RULE_atom)
+        self.enterRule(localctx, 40, self.RULE_atom)
         try:
-            self.state = 274
+            self.state = 264
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,28,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,27,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 266
+                self.state = 257
                 self.tag_symbol()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 267
+                self.state = 258
                 self.tag()
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 268
+                self.state = 259
                 self.link()
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 269
+                self.state = 260
                 self.property_()
                 pass
 
             elif la_ == 5:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 270
+                self.state = 261
                 self.id_group()
                 pass
 
             elif la_ == 6:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 271
+                self.state = 262
                 self.ref()
                 pass
 
             elif la_ == 7:
                 self.enterOuterAlt(localctx, 7)
-                self.state = 272
-                self.zid()
-                pass
-
-            elif la_ == 8:
-                self.enterOuterAlt(localctx, 8)
-                self.state = 273
+                self.state = 263
                 self.priority()
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
+    class ZidContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def ZID(self):
+            return self.getToken(ZorgFileParser.ZID, 0)
+
+        def getRuleIndex(self):
+            return ZorgFileParser.RULE_zid
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterZid" ):
+                listener.enterZid(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitZid" ):
+                listener.exitZid(self)
+
+
+
+
+    def zid(self):
+
+        localctx = ZorgFileParser.ZidContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 42, self.RULE_zid)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 266
+            self.match(ZorgFileParser.ZID)
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
     class PropertyContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
@@ -1910,21 +1884,21 @@
 
     def property_(self):
 
         localctx = ZorgFileParser.PropertyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 44, self.RULE_property)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 276
+            self.state = 268
             self.match(ZorgFileParser.ID)
-            self.state = 277
+            self.state = 269
             self.match(ZorgFileParser.COLON)
-            self.state = 278
+            self.state = 270
             self.match(ZorgFileParser.COLON)
-            self.state = 279
+            self.state = 271
             self.id_group()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1969,38 +1943,38 @@
     def id_group(self):
 
         localctx = ZorgFileParser.Id_groupContext(self, self._ctx, self.state)
         self.enterRule(localctx, 46, self.RULE_id_group)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 281
+            self.state = 273
             self.id_()
-            self.state = 291
+            self.state = 283
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,30,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,29,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 283 
+                    self.state = 275 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     while True:
-                        self.state = 282
+                        self.state = 274
                         self.id_symbol()
-                        self.state = 285 
+                        self.state = 277 
                         self._errHandler.sync(self)
                         _la = self._input.LA(1)
-                        if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 6029312) != 0)):
+                        if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 4398281392128) != 0)):
                             break
 
-                    self.state = 287
+                    self.state = 279
                     self.id_() 
-                self.state = 293
+                self.state = 285
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,30,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,29,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2016,22 +1990,32 @@
 
         def ID(self):
             return self.getToken(ZorgFileParser.ID, 0)
 
         def NUM_ID(self):
             return self.getToken(ZorgFileParser.NUM_ID, 0)
 
+        def DATE_RANGE_TAIL(self):
+            return self.getToken(ZorgFileParser.DATE_RANGE_TAIL, 0)
+
+        def PRIORITY(self):
+            return self.getToken(ZorgFileParser.PRIORITY, 0)
+
         def date(self):
             return self.getTypedRuleContext(ZorgFileParser.DateContext,0)
 
 
         def time(self):
             return self.getTypedRuleContext(ZorgFileParser.TimeContext,0)
 
 
+        def zid(self):
+            return self.getTypedRuleContext(ZorgFileParser.ZidContext,0)
+
+
         def LOWER_O(self):
             return self.getToken(ZorgFileParser.LOWER_O, 0)
 
         def LOWER_X(self):
             return self.getToken(ZorgFileParser.LOWER_X, 0)
 
         def getRuleIndex(self):
@@ -2049,45 +2033,60 @@
 
 
     def id_(self):
 
         localctx = ZorgFileParser.IdContext(self, self._ctx, self.state)
         self.enterRule(localctx, 48, self.RULE_id)
         try:
-            self.state = 300
+            self.state = 295
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [12]:
+            if token in [16]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 294
+                self.state = 286
                 self.match(ZorgFileParser.ID)
                 pass
-            elif token in [14]:
+            elif token in [19]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 295
+                self.state = 287
                 self.match(ZorgFileParser.NUM_ID)
                 pass
-            elif token in [10]:
+            elif token in [14]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 296
+                self.state = 288
+                self.match(ZorgFileParser.DATE_RANGE_TAIL)
+                pass
+            elif token in [15]:
+                self.enterOuterAlt(localctx, 4)
+                self.state = 289
+                self.match(ZorgFileParser.PRIORITY)
+                pass
+            elif token in [10]:
+                self.enterOuterAlt(localctx, 5)
+                self.state = 290
                 self.date()
                 pass
             elif token in [11]:
-                self.enterOuterAlt(localctx, 4)
-                self.state = 297
+                self.enterOuterAlt(localctx, 6)
+                self.state = 291
                 self.time()
                 pass
+            elif token in [17]:
+                self.enterOuterAlt(localctx, 7)
+                self.state = 292
+                self.zid()
+                pass
             elif token in [8]:
-                self.enterOuterAlt(localctx, 5)
-                self.state = 298
+                self.enterOuterAlt(localctx, 8)
+                self.state = 293
                 self.match(ZorgFileParser.LOWER_O)
                 pass
             elif token in [9]:
-                self.enterOuterAlt(localctx, 6)
-                self.state = 299
+                self.enterOuterAlt(localctx, 9)
+                self.state = 294
                 self.match(ZorgFileParser.LOWER_X)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2124,15 +2123,15 @@
 
     def date(self):
 
         localctx = ZorgFileParser.DateContext(self, self._ctx, self.state)
         self.enterRule(localctx, 50, self.RULE_date)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 302
+            self.state = 297
             self.match(ZorgFileParser.DATE)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2165,15 +2164,15 @@
 
     def time(self):
 
         localctx = ZorgFileParser.TimeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 52, self.RULE_time)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 304
+            self.state = 299
             self.match(ZorgFileParser.TIME)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2189,14 +2188,20 @@
 
         def SQUOTE(self):
             return self.getToken(ZorgFileParser.SQUOTE, 0)
 
         def DQUOTE(self):
             return self.getToken(ZorgFileParser.DQUOTE, 0)
 
+        def HAT(self):
+            return self.getToken(ZorgFileParser.HAT, 0)
+
+        def DOLLAR(self):
+            return self.getToken(ZorgFileParser.DOLLAR, 0)
+
         def non_tag_symbol(self):
             return self.getTypedRuleContext(ZorgFileParser.Non_tag_symbolContext,0)
 
 
         def tag_symbol(self):
             return self.getTypedRuleContext(ZorgFileParser.Tag_symbolContext,0)
 
@@ -2220,40 +2225,50 @@
 
 
     def any_symbol(self):
 
         localctx = ZorgFileParser.Any_symbolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 54, self.RULE_any_symbol)
         try:
-            self.state = 311
+            self.state = 308
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [30]:
+            if token in [36]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 306
+                self.state = 301
                 self.match(ZorgFileParser.SQUOTE)
                 pass
-            elif token in [31]:
+            elif token in [37]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 307
+                self.state = 302
                 self.match(ZorgFileParser.DQUOTE)
                 pass
-            elif token in [17, 21, 24, 25, 32, 33, 34, 35]:
+            elif token in [24]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 308
-                self.non_tag_symbol()
+                self.state = 303
+                self.match(ZorgFileParser.HAT)
                 pass
-            elif token in [26, 27, 28, 29]:
+            elif token in [23]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 309
-                self.tag_symbol()
+                self.state = 304
+                self.match(ZorgFileParser.DOLLAR)
                 pass
-            elif token in [18, 19, 20, 22]:
+            elif token in [22, 28, 30, 31, 38, 39, 40, 41]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 310
+                self.state = 305
+                self.non_tag_symbol()
+                pass
+            elif token in [32, 33, 34, 35]:
+                self.enterOuterAlt(localctx, 6)
+                self.state = 306
+                self.tag_symbol()
+                pass
+            elif token in [25, 26, 27, 42]:
+                self.enterOuterAlt(localctx, 7)
+                self.state = 307
                 self.id_symbol()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2312,17 +2327,17 @@
     def non_tag_symbol(self):
 
         localctx = ZorgFileParser.Non_tag_symbolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 56, self.RULE_non_tag_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 313
+            self.state = 310
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 64477069312) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 4126662459392) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -2368,17 +2383,17 @@
     def id_symbol(self):
 
         localctx = ZorgFileParser.Id_symbolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 58, self.RULE_id_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 315
+            self.state = 312
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 6029312) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 4398281392128) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -2424,17 +2439,17 @@
     def tag_symbol(self):
 
         localctx = ZorgFileParser.Tag_symbolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 60, self.RULE_tag_symbol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 317
+            self.state = 314
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006632960) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 64424509440) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -2482,35 +2497,35 @@
 
 
     def tag(self):
 
         localctx = ZorgFileParser.TagContext(self, self._ctx, self.state)
         self.enterRule(localctx, 62, self.RULE_tag)
         try:
-            self.state = 323
+            self.state = 320
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [26]:
+            if token in [32]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 319
+                self.state = 316
                 self.area()
                 pass
-            elif token in [27]:
+            elif token in [33]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 320
+                self.state = 317
                 self.context()
                 pass
-            elif token in [29]:
+            elif token in [35]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 321
+                self.state = 318
                 self.person()
                 pass
-            elif token in [28]:
+            elif token in [34]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 322
+                self.state = 319
                 self.project()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2550,17 +2565,17 @@
 
     def area(self):
 
         localctx = ZorgFileParser.AreaContext(self, self._ctx, self.state)
         self.enterRule(localctx, 64, self.RULE_area)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 325
+            self.state = 322
             self.match(ZorgFileParser.HASH)
-            self.state = 326
+            self.state = 323
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2596,17 +2611,17 @@
 
     def context(self):
 
         localctx = ZorgFileParser.ContextContext(self, self._ctx, self.state)
         self.enterRule(localctx, 66, self.RULE_context)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 328
+            self.state = 325
             self.match(ZorgFileParser.AT_SIGN)
-            self.state = 329
+            self.state = 326
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2642,17 +2657,17 @@
 
     def person(self):
 
         localctx = ZorgFileParser.PersonContext(self, self._ctx, self.state)
         self.enterRule(localctx, 68, self.RULE_person)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 331
+            self.state = 328
             self.match(ZorgFileParser.PERCENT)
-            self.state = 332
+            self.state = 329
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2688,17 +2703,17 @@
 
     def project(self):
 
         localctx = ZorgFileParser.ProjectContext(self, self._ctx, self.state)
         self.enterRule(localctx, 70, self.RULE_project)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 334
+            self.state = 331
             self.match(ZorgFileParser.PLUS)
-            self.state = 335
+            self.state = 332
             self.match(ZorgFileParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -2755,73 +2770,73 @@
     def quoted(self):
 
         localctx = ZorgFileParser.QuotedContext(self, self._ctx, self.state)
         self.enterRule(localctx, 72, self.RULE_quoted)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 355
+            self.state = 352
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [30]:
-                self.state = 337
+            if token in [36]:
+                self.state = 334
                 self.match(ZorgFileParser.SQUOTE)
-                self.state = 342 
+                self.state = 339 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 342
+                    self.state = 339
                     self._errHandler.sync(self)
-                    la_ = self._interp.adaptivePredict(self._input,34,self._ctx)
+                    la_ = self._interp.adaptivePredict(self._input,33,self._ctx)
                     if la_ == 1:
-                        self.state = 338
+                        self.state = 335
                         self.atom()
                         pass
 
                     elif la_ == 2:
-                        self.state = 339
+                        self.state = 336
                         self.priority()
                         pass
 
                     elif la_ == 3:
-                        self.state = 340
-                        self.match(ZorgFileParser.T__2)
+                        self.state = 337
+                        self.match(ZorgFileParser.T__0)
                         pass
 
                     elif la_ == 4:
-                        self.state = 341
-                        self.match(ZorgFileParser.T__3)
+                        self.state = 338
+                        self.match(ZorgFileParser.T__1)
                         pass
 
 
-                    self.state = 344 
+                    self.state = 341 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006665498) != 0)):
+                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 64425283342) != 0)):
                         break
 
-                self.state = 346
+                self.state = 343
                 self.match(ZorgFileParser.SQUOTE)
                 pass
-            elif token in [31]:
-                self.state = 347
+            elif token in [37]:
+                self.state = 344
                 self.match(ZorgFileParser.DQUOTE)
-                self.state = 349 
+                self.state = 346 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 348
+                    self.state = 345
                     self.atom()
-                    self.state = 351 
+                    self.state = 348 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1006665482) != 0)):
+                    if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 64425283338) != 0)):
                         break
 
-                self.state = 353
+                self.state = 350
                 self.match(ZorgFileParser.DQUOTE)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2859,20 +2874,20 @@
 
     def link(self):
 
         localctx = ZorgFileParser.LinkContext(self, self._ctx, self.state)
         self.enterRule(localctx, 74, self.RULE_link)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 357
-            self.match(ZorgFileParser.T__2)
-            self.state = 358
+            self.state = 354
+            self.match(ZorgFileParser.T__0)
+            self.state = 355
             self.id_group()
-            self.state = 359
-            self.match(ZorgFileParser.T__3)
+            self.state = 356
+            self.match(ZorgFileParser.T__1)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -2905,20 +2920,20 @@
 
     def ref(self):
 
         localctx = ZorgFileParser.RefContext(self, self._ctx, self.state)
         self.enterRule(localctx, 76, self.RULE_ref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 361
-            self.match(ZorgFileParser.T__0)
-            self.state = 362
+            self.state = 358
+            self.match(ZorgFileParser.T__2)
+            self.state = 359
             self.id_group()
-            self.state = 363
-            self.match(ZorgFileParser.T__1)
+            self.state = 360
+            self.match(ZorgFileParser.T__3)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -2972,53 +2987,53 @@
     def h1_section(self):
 
         localctx = ZorgFileParser.H1_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 78, self.RULE_h1_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 365
+            self.state = 362
             self.h1_header()
-            self.state = 369
+            self.state = 366
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,37,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 366
+                    self.state = 363
                     self.match(ZorgFileParser.NL) 
-                self.state = 371
+                self.state = 368
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,37,self._ctx)
 
-            self.state = 375
+            self.state = 372
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,39,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 372
+                    self.state = 369
                     self.block() 
-                self.state = 377
+                self.state = 374
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,39,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,38,self._ctx)
 
-            self.state = 384
+            self.state = 381
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la==5 or _la==7:
-                self.state = 379
+                self.state = 376
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la==7:
-                    self.state = 378
+                    self.state = 375
                     self.match(ZorgFileParser.NL)
 
 
-                self.state = 381
+                self.state = 378
                 self.h2_section()
-                self.state = 386
+                self.state = 383
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3075,56 +3090,56 @@
     def h2_section(self):
 
         localctx = ZorgFileParser.H2_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 80, self.RULE_h2_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 387
+            self.state = 384
             self.h2_header()
-            self.state = 391
+            self.state = 388
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,41,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 388
+                    self.state = 385
                     self.match(ZorgFileParser.NL) 
-                self.state = 393
+                self.state = 390
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,41,self._ctx)
 
-            self.state = 397
+            self.state = 394
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 394
+                    self.state = 391
                     self.block() 
-                self.state = 399
+                self.state = 396
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,43,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,42,self._ctx)
 
-            self.state = 406
+            self.state = 403
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,44,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 401
+                    self.state = 398
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==7:
-                        self.state = 400
+                        self.state = 397
                         self.match(ZorgFileParser.NL)
 
 
-                    self.state = 403
+                    self.state = 400
                     self.h3_section() 
-                self.state = 408
+                self.state = 405
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,44,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3179,56 +3194,56 @@
     def h3_section(self):
 
         localctx = ZorgFileParser.H3_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 82, self.RULE_h3_section)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 409
+            self.state = 406
             self.h3_header()
-            self.state = 413
+            self.state = 410
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 410
+                    self.state = 407
                     self.match(ZorgFileParser.NL) 
-                self.state = 415
+                self.state = 412
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,45,self._ctx)
 
-            self.state = 419
+            self.state = 416
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,47,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 416
+                    self.state = 413
                     self.block() 
-                self.state = 421
+                self.state = 418
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,47,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
 
-            self.state = 428
+            self.state = 425
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,48,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 423
+                    self.state = 420
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la==7:
-                        self.state = 422
+                        self.state = 419
                         self.match(ZorgFileParser.NL)
 
 
-                    self.state = 425
+                    self.state = 422
                     self.h4_section() 
-                self.state = 430
+                self.state = 427
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,48,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3275,37 +3290,37 @@
 
     def h4_section(self):
 
         localctx = ZorgFileParser.H4_sectionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 84, self.RULE_h4_section)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 431
+            self.state = 428
             self.h4_header()
-            self.state = 435
+            self.state = 432
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 432
+                    self.state = 429
                     self.match(ZorgFileParser.NL) 
-                self.state = 437
+                self.state = 434
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,49,self._ctx)
 
-            self.state = 441
+            self.state = 438
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 438
+                    self.state = 435
                     self.block() 
-                self.state = 443
+                self.state = 440
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,50,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3349,35 +3364,35 @@
 
     def h1_header(self):
 
         localctx = ZorgFileParser.H1_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 86, self.RULE_h1_header)
         try:
             self.enterOuterAlt(localctx, 1)
+            self.state = 441
+            self.match(ZorgFileParser.HASH)
+            self.state = 442
+            self.match(ZorgFileParser.HASH)
+            self.state = 443
+            self.match(ZorgFileParser.HASH)
             self.state = 444
             self.match(ZorgFileParser.HASH)
             self.state = 445
             self.match(ZorgFileParser.HASH)
             self.state = 446
             self.match(ZorgFileParser.HASH)
             self.state = 447
             self.match(ZorgFileParser.HASH)
             self.state = 448
             self.match(ZorgFileParser.HASH)
             self.state = 449
             self.match(ZorgFileParser.HASH)
             self.state = 450
-            self.match(ZorgFileParser.HASH)
-            self.state = 451
-            self.match(ZorgFileParser.HASH)
-            self.state = 452
-            self.match(ZorgFileParser.HASH)
-            self.state = 453
             self.space_atoms()
-            self.state = 454
+            self.state = 451
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3415,19 +3430,19 @@
 
     def h2_header(self):
 
         localctx = ZorgFileParser.H2_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 88, self.RULE_h2_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 456
+            self.state = 453
             self.match(ZorgFileParser.T__4)
-            self.state = 457
+            self.state = 454
             self.space_atoms()
-            self.state = 458
+            self.state = 455
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3465,19 +3480,19 @@
 
     def h3_header(self):
 
         localctx = ZorgFileParser.H3_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 90, self.RULE_h3_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 460
+            self.state = 457
             self.match(ZorgFileParser.T__5)
-            self.state = 461
+            self.state = 458
             self.space_atoms()
-            self.state = 462
+            self.state = 459
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3521,23 +3536,23 @@
 
     def h4_header(self):
 
         localctx = ZorgFileParser.H4_headerContext(self, self._ctx, self.state)
         self.enterRule(localctx, 92, self.RULE_h4_header)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 464
+            self.state = 461
             self.match(ZorgFileParser.DASH)
-            self.state = 465
+            self.state = 462
             self.match(ZorgFileParser.DASH)
-            self.state = 466
+            self.state = 463
             self.match(ZorgFileParser.DASH)
-            self.state = 467
+            self.state = 464
             self.space_atoms()
-            self.state = 468
+            self.state = 465
             self.eol()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3574,15 +3589,15 @@
     def eol(self):
 
         localctx = ZorgFileParser.EolContext(self, self._ctx, self.state)
         self.enterRule(localctx, 94, self.RULE_eol)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 470
+            self.state = 467
             _la = self._input.LA(1)
             if not(_la==-1 or _la==7):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQuery.tokens` & `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFile.tokens`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,72 @@
 T__0=1
 T__1=2
 T__2=3
 T__3=4
 T__4=5
 T__5=6
-T__6=7
-T__7=8
-T__8=9
-T__9=10
-T__10=11
-T__11=12
-T__12=13
-NL=14
-LOWER_O=15
-LOWER_X=16
-DATE=17
-TIME=18
-ID=19
-ZID=20
-NUM_ID=21
-TWO_SPACE_DASH=22
-FOUR_SPACE_DASH=23
-SYMBOL=24
+NL=7
+LOWER_O=8
+LOWER_X=9
+DATE=10
+TIME=11
+CREATE_RANGE_HEAD=12
+MODIFY_RANGE_HEAD=13
+DATE_RANGE_TAIL=14
+PRIORITY=15
+ID=16
+ZID=17
+SHORT_DATE=18
+NUM_ID=19
+TWO_SPACE_DASH=20
+FOUR_SPACE_DASH=21
+SYMBOL=22
+DOLLAR=23
+HAT=24
 DASH=25
 DOT=26
 FSLASH=27
 UNDERSCORE=28
-COLON=29
-SPACE=30
-LPAREN=31
-RPAREN=32
-HASH=33
-AT_SIGN=34
-PLUS=35
-PERCENT=36
-SQUOTE=37
-DQUOTE=38
-TILDE=39
-STAR=40
-LANGLE=41
-RANGLE=42
-'S'=1
-'W'=2
-'O'=3
-'G'=4
-'note'=5
-'or'=6
-'['=7
-']'=8
-'!'=9
-'date'=10
-'priority'=11
-'file'=12
-'type'=13
-'o'=15
-'x'=16
-'  -'=22
-'    -'=23
+SPACE=29
+LPAREN=30
+RPAREN=31
+HASH=32
+AT_SIGN=33
+PLUS=34
+PERCENT=35
+SQUOTE=36
+DQUOTE=37
+TILDE=38
+STAR=39
+LANGLE=40
+RANGLE=41
+COLON=42
+'[['=1
+']]'=2
+'['=3
+']'=4
+'======='=5
+'*****'=6
+'o'=8
+'x'=9
+'  -'=20
+'    -'=21
+'$'=23
+'^'=24
 '-'=25
 '.'=26
 '/'=27
 '_'=28
-':'=29
-' '=30
-'('=31
-')'=32
-'#'=33
-'@'=34
-'+'=35
-'%'=36
-'\''=37
-'"'=38
-'~'=39
-'*'=40
-'<'=41
-'>'=42
+' '=29
+'('=30
+')'=31
+'#'=32
+'@'=33
+'+'=34
+'%'=35
+'\''=36
+'"'=37
+'~'=38
+'*'=39
+'<'=40
+'>'=41
+':'=42
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryLexer.py` & `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,193 +1,191 @@
-# Generated from ZorgQuery.g4 by ANTLR 4.13.1
+# Generated from ZorgFile.g4 by ANTLR 4.13.1
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
 
 
 def serializedATN():
     return [
-        4,0,42,270,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,
+        4,0,42,266,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,
         2,6,7,6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,
         13,7,13,2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,
         19,2,20,7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,
         26,7,26,2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,
         32,2,33,7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,
         39,7,39,2,40,7,40,2,41,7,41,2,42,7,42,2,43,7,43,2,44,7,44,2,45,7,
-        45,2,46,7,46,2,47,7,47,2,48,7,48,2,49,7,49,1,0,1,0,1,1,1,1,1,2,1,
-        2,1,3,1,3,1,4,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,6,1,6,1,7,1,7,1,8,1,
-        8,1,9,1,9,1,9,1,9,1,9,1,10,1,10,1,10,1,10,1,10,1,10,1,10,1,10,1,
-        10,1,11,1,11,1,11,1,11,1,11,1,12,1,12,1,12,1,12,1,12,1,13,3,13,149,
-        8,13,1,13,1,13,1,14,1,14,1,15,1,15,1,16,1,16,1,16,1,16,1,16,1,16,
-        1,16,1,16,1,16,1,16,1,16,1,17,1,17,1,17,1,17,1,17,1,18,1,18,1,18,
-        5,18,176,8,18,10,18,12,18,179,9,18,1,19,1,19,1,19,1,19,1,19,1,19,
-        1,19,1,19,1,19,1,19,3,19,191,8,19,1,20,1,20,1,20,5,20,196,8,20,10,
-        20,12,20,199,9,20,1,21,1,21,1,21,1,21,1,22,1,22,1,22,1,22,1,22,1,
-        22,1,23,1,23,1,24,1,24,1,25,1,25,1,26,1,26,1,27,1,27,1,28,1,28,1,
-        29,1,29,1,30,1,30,1,31,1,31,1,32,1,32,1,33,1,33,1,34,1,34,1,35,1,
-        35,1,36,1,36,1,37,1,37,1,38,1,38,1,39,1,39,1,40,1,40,1,41,1,41,1,
-        42,1,42,1,43,1,43,1,44,1,44,3,44,255,8,44,1,45,1,45,1,46,1,46,1,
-        47,1,47,1,48,1,48,3,48,265,8,48,1,49,1,49,3,49,269,8,49,0,0,50,1,
-        1,3,2,5,3,7,4,9,5,11,6,13,7,15,8,17,9,19,10,21,11,23,12,25,13,27,
-        14,29,15,31,16,33,17,35,18,37,19,39,20,41,21,43,22,45,23,47,24,49,
-        25,51,26,53,27,55,28,57,29,59,30,61,31,63,32,65,33,67,34,69,35,71,
-        36,73,37,75,38,77,39,79,40,81,41,83,42,85,0,87,0,89,0,91,0,93,0,
-        95,0,97,0,99,0,1,0,2,10,0,33,33,36,36,38,38,44,44,59,59,61,61,63,
-        63,91,94,96,96,123,125,6,0,65,72,74,78,80,90,97,105,107,107,109,
-        122,270,0,1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,0,0,7,1,0,0,0,0,9,1,0,
-        0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,0,17,1,0,0,0,0,19,1,0,
-        0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,0,27,1,0,0,0,0,29,1,0,
-        0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,0,37,1,0,0,0,0,39,1,0,
-        0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,0,47,1,0,0,0,0,49,1,0,
-        0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,0,57,1,0,0,0,0,59,1,0,
-        0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,0,67,1,0,0,0,0,69,1,0,
-        0,0,0,71,1,0,0,0,0,73,1,0,0,0,0,75,1,0,0,0,0,77,1,0,0,0,0,79,1,0,
-        0,0,0,81,1,0,0,0,0,83,1,0,0,0,1,101,1,0,0,0,3,103,1,0,0,0,5,105,
-        1,0,0,0,7,107,1,0,0,0,9,109,1,0,0,0,11,114,1,0,0,0,13,117,1,0,0,
-        0,15,119,1,0,0,0,17,121,1,0,0,0,19,123,1,0,0,0,21,128,1,0,0,0,23,
-        137,1,0,0,0,25,142,1,0,0,0,27,148,1,0,0,0,29,152,1,0,0,0,31,154,
-        1,0,0,0,33,156,1,0,0,0,35,167,1,0,0,0,37,172,1,0,0,0,39,180,1,0,
-        0,0,41,192,1,0,0,0,43,200,1,0,0,0,45,204,1,0,0,0,47,210,1,0,0,0,
-        49,212,1,0,0,0,51,214,1,0,0,0,53,216,1,0,0,0,55,218,1,0,0,0,57,220,
-        1,0,0,0,59,222,1,0,0,0,61,224,1,0,0,0,63,226,1,0,0,0,65,228,1,0,
-        0,0,67,230,1,0,0,0,69,232,1,0,0,0,71,234,1,0,0,0,73,236,1,0,0,0,
-        75,238,1,0,0,0,77,240,1,0,0,0,79,242,1,0,0,0,81,244,1,0,0,0,83,246,
-        1,0,0,0,85,248,1,0,0,0,87,250,1,0,0,0,89,254,1,0,0,0,91,256,1,0,
-        0,0,93,258,1,0,0,0,95,260,1,0,0,0,97,264,1,0,0,0,99,268,1,0,0,0,
-        101,102,5,83,0,0,102,2,1,0,0,0,103,104,5,87,0,0,104,4,1,0,0,0,105,
-        106,5,79,0,0,106,6,1,0,0,0,107,108,5,71,0,0,108,8,1,0,0,0,109,110,
-        5,110,0,0,110,111,5,111,0,0,111,112,5,116,0,0,112,113,5,101,0,0,
-        113,10,1,0,0,0,114,115,5,111,0,0,115,116,5,114,0,0,116,12,1,0,0,
-        0,117,118,5,91,0,0,118,14,1,0,0,0,119,120,5,93,0,0,120,16,1,0,0,
-        0,121,122,5,33,0,0,122,18,1,0,0,0,123,124,5,100,0,0,124,125,5,97,
-        0,0,125,126,5,116,0,0,126,127,5,101,0,0,127,20,1,0,0,0,128,129,5,
-        112,0,0,129,130,5,114,0,0,130,131,5,105,0,0,131,132,5,111,0,0,132,
-        133,5,114,0,0,133,134,5,105,0,0,134,135,5,116,0,0,135,136,5,121,
-        0,0,136,22,1,0,0,0,137,138,5,102,0,0,138,139,5,105,0,0,139,140,5,
-        108,0,0,140,141,5,101,0,0,141,24,1,0,0,0,142,143,5,116,0,0,143,144,
-        5,121,0,0,144,145,5,112,0,0,145,146,5,101,0,0,146,26,1,0,0,0,147,
-        149,5,13,0,0,148,147,1,0,0,0,148,149,1,0,0,0,149,150,1,0,0,0,150,
-        151,5,10,0,0,151,28,1,0,0,0,152,153,5,111,0,0,153,30,1,0,0,0,154,
-        155,5,120,0,0,155,32,1,0,0,0,156,157,5,50,0,0,157,158,3,91,45,0,
-        158,159,3,91,45,0,159,160,3,91,45,0,160,161,3,49,24,0,161,162,3,
-        95,47,0,162,163,3,91,45,0,163,164,3,49,24,0,164,165,3,93,46,0,165,
-        166,3,91,45,0,166,34,1,0,0,0,167,168,2,48,50,0,168,169,3,91,45,0,
-        169,170,2,48,53,0,170,171,3,91,45,0,171,36,1,0,0,0,172,177,3,99,
-        49,0,173,176,3,99,49,0,174,176,3,55,27,0,175,173,1,0,0,0,175,174,
-        1,0,0,0,176,179,1,0,0,0,177,175,1,0,0,0,177,178,1,0,0,0,178,38,1,
-        0,0,0,179,177,1,0,0,0,180,181,3,91,45,0,181,182,3,91,45,0,182,183,
-        3,95,47,0,183,184,3,91,45,0,184,185,3,93,46,0,185,186,3,91,45,0,
-        186,187,3,65,32,0,187,188,3,89,44,0,188,190,3,89,44,0,189,191,3,
-        89,44,0,190,189,1,0,0,0,190,191,1,0,0,0,191,40,1,0,0,0,192,197,3,
-        91,45,0,193,196,3,99,49,0,194,196,3,55,27,0,195,193,1,0,0,0,195,
-        194,1,0,0,0,196,199,1,0,0,0,197,195,1,0,0,0,197,198,1,0,0,0,198,
-        42,1,0,0,0,199,197,1,0,0,0,200,201,5,32,0,0,201,202,5,32,0,0,202,
-        203,5,45,0,0,203,44,1,0,0,0,204,205,5,32,0,0,205,206,5,32,0,0,206,
-        207,5,32,0,0,207,208,5,32,0,0,208,209,5,45,0,0,209,46,1,0,0,0,210,
-        211,7,0,0,0,211,48,1,0,0,0,212,213,5,45,0,0,213,50,1,0,0,0,214,215,
-        5,46,0,0,215,52,1,0,0,0,216,217,5,47,0,0,217,54,1,0,0,0,218,219,
-        5,95,0,0,219,56,1,0,0,0,220,221,5,58,0,0,221,58,1,0,0,0,222,223,
-        5,32,0,0,223,60,1,0,0,0,224,225,5,40,0,0,225,62,1,0,0,0,226,227,
-        5,41,0,0,227,64,1,0,0,0,228,229,5,35,0,0,229,66,1,0,0,0,230,231,
-        5,64,0,0,231,68,1,0,0,0,232,233,5,43,0,0,233,70,1,0,0,0,234,235,
-        5,37,0,0,235,72,1,0,0,0,236,237,5,39,0,0,237,74,1,0,0,0,238,239,
-        5,34,0,0,239,76,1,0,0,0,240,241,5,126,0,0,241,78,1,0,0,0,242,243,
-        5,42,0,0,243,80,1,0,0,0,244,245,5,60,0,0,245,82,1,0,0,0,246,247,
-        5,62,0,0,247,84,1,0,0,0,248,249,2,65,90,0,249,86,1,0,0,0,250,251,
-        2,97,122,0,251,88,1,0,0,0,252,255,3,91,45,0,253,255,7,1,0,0,254,
-        252,1,0,0,0,254,253,1,0,0,0,255,90,1,0,0,0,256,257,2,48,57,0,257,
-        92,1,0,0,0,258,259,2,48,51,0,259,94,1,0,0,0,260,261,2,48,49,0,261,
-        96,1,0,0,0,262,265,3,85,42,0,263,265,3,87,43,0,264,262,1,0,0,0,264,
-        263,1,0,0,0,265,98,1,0,0,0,266,269,3,97,48,0,267,269,3,91,45,0,268,
-        266,1,0,0,0,268,267,1,0,0,0,269,100,1,0,0,0,10,0,148,175,177,190,
-        195,197,254,264,268,0
+        45,2,46,7,46,2,47,7,47,2,48,7,48,2,49,7,49,1,0,1,0,1,0,1,1,1,1,1,
+        1,1,2,1,2,1,3,1,3,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,
+        5,1,5,1,5,1,6,3,6,127,8,6,1,6,1,6,1,7,1,7,1,8,1,8,1,9,1,9,1,9,1,
+        9,1,9,1,9,1,9,1,9,1,9,1,9,1,9,1,10,1,10,1,10,1,10,1,10,1,11,1,11,
+        1,11,1,12,1,12,1,12,1,13,1,13,1,13,1,14,1,14,1,14,1,15,1,15,1,15,
+        5,15,166,8,15,10,15,12,15,169,9,15,1,16,1,16,1,16,1,16,1,16,3,16,
+        176,8,16,1,17,1,17,1,17,1,17,1,17,1,17,1,17,1,18,1,18,1,18,5,18,
+        188,8,18,10,18,12,18,191,9,18,1,19,1,19,1,19,1,19,1,20,1,20,1,20,
+        1,20,1,20,1,20,1,21,1,21,1,22,1,22,1,23,1,23,1,24,1,24,1,25,1,25,
+        1,26,1,26,1,27,1,27,1,28,1,28,1,29,1,29,1,30,1,30,1,31,1,31,1,32,
+        1,32,1,33,1,33,1,34,1,34,1,35,1,35,1,36,1,36,1,37,1,37,1,38,1,38,
+        1,39,1,39,1,40,1,40,1,41,1,41,1,42,1,42,1,43,1,43,1,44,1,44,3,44,
+        251,8,44,1,45,1,45,1,46,1,46,1,47,1,47,1,48,1,48,3,48,261,8,48,1,
+        49,1,49,3,49,265,8,49,0,0,50,1,1,3,2,5,3,7,4,9,5,11,6,13,7,15,8,
+        17,9,19,10,21,11,23,12,25,13,27,14,29,15,31,16,33,17,35,18,37,19,
+        39,20,41,21,43,22,45,23,47,24,49,25,51,26,53,27,55,28,57,29,59,30,
+        61,31,63,32,65,33,67,34,69,35,71,36,73,37,75,38,77,39,79,40,81,41,
+        83,42,85,0,87,0,89,0,91,0,93,0,95,0,97,0,99,0,1,0,2,9,0,33,33,38,
+        38,44,44,59,59,61,61,63,63,91,93,96,96,123,125,6,0,65,72,74,78,80,
+        90,97,105,107,107,109,122,266,0,1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,
+        0,0,7,1,0,0,0,0,9,1,0,0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,
+        0,17,1,0,0,0,0,19,1,0,0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,
+        0,27,1,0,0,0,0,29,1,0,0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,
+        0,37,1,0,0,0,0,39,1,0,0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,
+        0,47,1,0,0,0,0,49,1,0,0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,
+        0,57,1,0,0,0,0,59,1,0,0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,
+        0,67,1,0,0,0,0,69,1,0,0,0,0,71,1,0,0,0,0,73,1,0,0,0,0,75,1,0,0,0,
+        0,77,1,0,0,0,0,79,1,0,0,0,0,81,1,0,0,0,0,83,1,0,0,0,1,101,1,0,0,
+        0,3,104,1,0,0,0,5,107,1,0,0,0,7,109,1,0,0,0,9,111,1,0,0,0,11,119,
+        1,0,0,0,13,126,1,0,0,0,15,130,1,0,0,0,17,132,1,0,0,0,19,134,1,0,
+        0,0,21,145,1,0,0,0,23,150,1,0,0,0,25,153,1,0,0,0,27,156,1,0,0,0,
+        29,159,1,0,0,0,31,162,1,0,0,0,33,170,1,0,0,0,35,177,1,0,0,0,37,184,
+        1,0,0,0,39,192,1,0,0,0,41,196,1,0,0,0,43,202,1,0,0,0,45,204,1,0,
+        0,0,47,206,1,0,0,0,49,208,1,0,0,0,51,210,1,0,0,0,53,212,1,0,0,0,
+        55,214,1,0,0,0,57,216,1,0,0,0,59,218,1,0,0,0,61,220,1,0,0,0,63,222,
+        1,0,0,0,65,224,1,0,0,0,67,226,1,0,0,0,69,228,1,0,0,0,71,230,1,0,
+        0,0,73,232,1,0,0,0,75,234,1,0,0,0,77,236,1,0,0,0,79,238,1,0,0,0,
+        81,240,1,0,0,0,83,242,1,0,0,0,85,244,1,0,0,0,87,246,1,0,0,0,89,250,
+        1,0,0,0,91,252,1,0,0,0,93,254,1,0,0,0,95,256,1,0,0,0,97,260,1,0,
+        0,0,99,264,1,0,0,0,101,102,5,91,0,0,102,103,5,91,0,0,103,2,1,0,0,
+        0,104,105,5,93,0,0,105,106,5,93,0,0,106,4,1,0,0,0,107,108,5,91,0,
+        0,108,6,1,0,0,0,109,110,5,93,0,0,110,8,1,0,0,0,111,112,5,61,0,0,
+        112,113,5,61,0,0,113,114,5,61,0,0,114,115,5,61,0,0,115,116,5,61,
+        0,0,116,117,5,61,0,0,117,118,5,61,0,0,118,10,1,0,0,0,119,120,5,42,
+        0,0,120,121,5,42,0,0,121,122,5,42,0,0,122,123,5,42,0,0,123,124,5,
+        42,0,0,124,12,1,0,0,0,125,127,5,13,0,0,126,125,1,0,0,0,126,127,1,
+        0,0,0,127,128,1,0,0,0,128,129,5,10,0,0,129,14,1,0,0,0,130,131,5,
+        111,0,0,131,16,1,0,0,0,132,133,5,120,0,0,133,18,1,0,0,0,134,135,
+        5,50,0,0,135,136,3,91,45,0,136,137,3,91,45,0,137,138,3,91,45,0,138,
+        139,3,49,24,0,139,140,3,95,47,0,140,141,3,91,45,0,141,142,3,49,24,
+        0,142,143,3,93,46,0,143,144,3,91,45,0,144,20,1,0,0,0,145,146,2,48,
+        50,0,146,147,3,91,45,0,147,148,2,48,53,0,148,149,3,91,45,0,149,22,
+        1,0,0,0,150,151,3,47,23,0,151,152,3,35,17,0,152,24,1,0,0,0,153,154,
+        3,45,22,0,154,155,3,35,17,0,155,26,1,0,0,0,156,157,3,83,41,0,157,
+        158,3,35,17,0,158,28,1,0,0,0,159,160,5,80,0,0,160,161,3,91,45,0,
+        161,30,1,0,0,0,162,167,3,99,49,0,163,166,3,99,49,0,164,166,3,55,
+        27,0,165,163,1,0,0,0,165,164,1,0,0,0,166,169,1,0,0,0,167,165,1,0,
+        0,0,167,168,1,0,0,0,168,32,1,0,0,0,169,167,1,0,0,0,170,171,3,35,
+        17,0,171,172,3,63,31,0,172,173,3,89,44,0,173,175,3,89,44,0,174,176,
+        3,89,44,0,175,174,1,0,0,0,175,176,1,0,0,0,176,34,1,0,0,0,177,178,
+        3,91,45,0,178,179,3,91,45,0,179,180,3,95,47,0,180,181,3,91,45,0,
+        181,182,3,93,46,0,182,183,3,91,45,0,183,36,1,0,0,0,184,189,3,91,
+        45,0,185,188,3,99,49,0,186,188,3,55,27,0,187,185,1,0,0,0,187,186,
+        1,0,0,0,188,191,1,0,0,0,189,187,1,0,0,0,189,190,1,0,0,0,190,38,1,
+        0,0,0,191,189,1,0,0,0,192,193,5,32,0,0,193,194,5,32,0,0,194,195,
+        5,45,0,0,195,40,1,0,0,0,196,197,5,32,0,0,197,198,5,32,0,0,198,199,
+        5,32,0,0,199,200,5,32,0,0,200,201,5,45,0,0,201,42,1,0,0,0,202,203,
+        7,0,0,0,203,44,1,0,0,0,204,205,5,36,0,0,205,46,1,0,0,0,206,207,5,
+        94,0,0,207,48,1,0,0,0,208,209,5,45,0,0,209,50,1,0,0,0,210,211,5,
+        46,0,0,211,52,1,0,0,0,212,213,5,47,0,0,213,54,1,0,0,0,214,215,5,
+        95,0,0,215,56,1,0,0,0,216,217,5,32,0,0,217,58,1,0,0,0,218,219,5,
+        40,0,0,219,60,1,0,0,0,220,221,5,41,0,0,221,62,1,0,0,0,222,223,5,
+        35,0,0,223,64,1,0,0,0,224,225,5,64,0,0,225,66,1,0,0,0,226,227,5,
+        43,0,0,227,68,1,0,0,0,228,229,5,37,0,0,229,70,1,0,0,0,230,231,5,
+        39,0,0,231,72,1,0,0,0,232,233,5,34,0,0,233,74,1,0,0,0,234,235,5,
+        126,0,0,235,76,1,0,0,0,236,237,5,42,0,0,237,78,1,0,0,0,238,239,5,
+        60,0,0,239,80,1,0,0,0,240,241,5,62,0,0,241,82,1,0,0,0,242,243,5,
+        58,0,0,243,84,1,0,0,0,244,245,2,65,90,0,245,86,1,0,0,0,246,247,2,
+        97,122,0,247,88,1,0,0,0,248,251,3,91,45,0,249,251,7,1,0,0,250,248,
+        1,0,0,0,250,249,1,0,0,0,251,90,1,0,0,0,252,253,2,48,57,0,253,92,
+        1,0,0,0,254,255,2,48,51,0,255,94,1,0,0,0,256,257,2,48,49,0,257,96,
+        1,0,0,0,258,261,3,85,42,0,259,261,3,87,43,0,260,258,1,0,0,0,260,
+        259,1,0,0,0,261,98,1,0,0,0,262,265,3,97,48,0,263,265,3,91,45,0,264,
+        262,1,0,0,0,264,263,1,0,0,0,265,100,1,0,0,0,10,0,126,165,167,175,
+        187,189,250,260,264,0
     ]
 
-class ZorgQueryLexer(Lexer):
+class ZorgFileLexer(Lexer):
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
 
     T__0 = 1
     T__1 = 2
     T__2 = 3
     T__3 = 4
     T__4 = 5
     T__5 = 6
-    T__6 = 7
-    T__7 = 8
-    T__8 = 9
-    T__9 = 10
-    T__10 = 11
-    T__11 = 12
-    T__12 = 13
-    NL = 14
-    LOWER_O = 15
-    LOWER_X = 16
-    DATE = 17
-    TIME = 18
-    ID = 19
-    ZID = 20
-    NUM_ID = 21
-    TWO_SPACE_DASH = 22
-    FOUR_SPACE_DASH = 23
-    SYMBOL = 24
+    NL = 7
+    LOWER_O = 8
+    LOWER_X = 9
+    DATE = 10
+    TIME = 11
+    CREATE_RANGE_HEAD = 12
+    MODIFY_RANGE_HEAD = 13
+    DATE_RANGE_TAIL = 14
+    PRIORITY = 15
+    ID = 16
+    ZID = 17
+    SHORT_DATE = 18
+    NUM_ID = 19
+    TWO_SPACE_DASH = 20
+    FOUR_SPACE_DASH = 21
+    SYMBOL = 22
+    DOLLAR = 23
+    HAT = 24
     DASH = 25
     DOT = 26
     FSLASH = 27
     UNDERSCORE = 28
-    COLON = 29
-    SPACE = 30
-    LPAREN = 31
-    RPAREN = 32
-    HASH = 33
-    AT_SIGN = 34
-    PLUS = 35
-    PERCENT = 36
-    SQUOTE = 37
-    DQUOTE = 38
-    TILDE = 39
-    STAR = 40
-    LANGLE = 41
-    RANGLE = 42
+    SPACE = 29
+    LPAREN = 30
+    RPAREN = 31
+    HASH = 32
+    AT_SIGN = 33
+    PLUS = 34
+    PERCENT = 35
+    SQUOTE = 36
+    DQUOTE = 37
+    TILDE = 38
+    STAR = 39
+    LANGLE = 40
+    RANGLE = 41
+    COLON = 42
 
     channelNames = [ u"DEFAULT_TOKEN_CHANNEL", u"HIDDEN" ]
 
     modeNames = [ "DEFAULT_MODE" ]
 
     literalNames = [ "<INVALID>",
-            "'S'", "'W'", "'O'", "'G'", "'note'", "'or'", "'['", "']'", 
-            "'!'", "'date'", "'priority'", "'file'", "'type'", "'o'", "'x'", 
-            "'  -'", "'    -'", "'-'", "'.'", "'/'", "'_'", "':'", "' '", 
-            "'('", "')'", "'#'", "'@'", "'+'", "'%'", "'''", "'\"'", "'~'", 
-            "'*'", "'<'", "'>'" ]
+            "'[['", "']]'", "'['", "']'", "'======='", "'*****'", "'o'", 
+            "'x'", "'  -'", "'    -'", "'$'", "'^'", "'-'", "'.'", "'/'", 
+            "'_'", "' '", "'('", "')'", "'#'", "'@'", "'+'", "'%'", "'''", 
+            "'\"'", "'~'", "'*'", "'<'", "'>'", "':'" ]
 
     symbolicNames = [ "<INVALID>",
-            "NL", "LOWER_O", "LOWER_X", "DATE", "TIME", "ID", "ZID", "NUM_ID", 
-            "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", "DOT", 
-            "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", "RPAREN", 
-            "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", "DQUOTE", "TILDE", 
-            "STAR", "LANGLE", "RANGLE" ]
-
-    ruleNames = [ "T__0", "T__1", "T__2", "T__3", "T__4", "T__5", "T__6", 
-                  "T__7", "T__8", "T__9", "T__10", "T__11", "T__12", "NL", 
-                  "LOWER_O", "LOWER_X", "DATE", "TIME", "ID", "ZID", "NUM_ID", 
-                  "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", "DASH", 
-                  "DOT", "FSLASH", "UNDERSCORE", "COLON", "SPACE", "LPAREN", 
-                  "RPAREN", "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", 
-                  "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE", "UPPER_LETTER", 
-                  "LOWER_LETTER", "ZID_CHAR", "NUM", "FIRST_D_NUM", "FIRST_M_NUM", 
-                  "ALPHA", "ALPHANUM" ]
+            "NL", "LOWER_O", "LOWER_X", "DATE", "TIME", "CREATE_RANGE_HEAD", 
+            "MODIFY_RANGE_HEAD", "DATE_RANGE_TAIL", "PRIORITY", "ID", "ZID", 
+            "SHORT_DATE", "NUM_ID", "TWO_SPACE_DASH", "FOUR_SPACE_DASH", 
+            "SYMBOL", "DOLLAR", "HAT", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
+            "SPACE", "LPAREN", "RPAREN", "HASH", "AT_SIGN", "PLUS", "PERCENT", 
+            "SQUOTE", "DQUOTE", "TILDE", "STAR", "LANGLE", "RANGLE", "COLON" ]
+
+    ruleNames = [ "T__0", "T__1", "T__2", "T__3", "T__4", "T__5", "NL", 
+                  "LOWER_O", "LOWER_X", "DATE", "TIME", "CREATE_RANGE_HEAD", 
+                  "MODIFY_RANGE_HEAD", "DATE_RANGE_TAIL", "PRIORITY", "ID", 
+                  "ZID", "SHORT_DATE", "NUM_ID", "TWO_SPACE_DASH", "FOUR_SPACE_DASH", 
+                  "SYMBOL", "DOLLAR", "HAT", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
+                  "SPACE", "LPAREN", "RPAREN", "HASH", "AT_SIGN", "PLUS", 
+                  "PERCENT", "SQUOTE", "DQUOTE", "TILDE", "STAR", "LANGLE", 
+                  "RANGLE", "COLON", "UPPER_LETTER", "LOWER_LETTER", "ZID_CHAR", 
+                  "NUM", "FIRST_D_NUM", "FIRST_M_NUM", "ALPHA", "ALPHANUM" ]
 
-    grammarFileName = "ZorgQuery.g4"
+    grammarFileName = "ZorgFile.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.13.1")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryLexer.tokens` & `zettel_org-0.7.3/src/zorg/grammar/zorg_file/ZorgFileLexer.tokens`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,72 @@
 T__0=1
 T__1=2
 T__2=3
 T__3=4
 T__4=5
 T__5=6
-T__6=7
-T__7=8
-T__8=9
-T__9=10
-T__10=11
-T__11=12
-T__12=13
-NL=14
-LOWER_O=15
-LOWER_X=16
-DATE=17
-TIME=18
-ID=19
-ZID=20
-NUM_ID=21
-TWO_SPACE_DASH=22
-FOUR_SPACE_DASH=23
-SYMBOL=24
+NL=7
+LOWER_O=8
+LOWER_X=9
+DATE=10
+TIME=11
+CREATE_RANGE_HEAD=12
+MODIFY_RANGE_HEAD=13
+DATE_RANGE_TAIL=14
+PRIORITY=15
+ID=16
+ZID=17
+SHORT_DATE=18
+NUM_ID=19
+TWO_SPACE_DASH=20
+FOUR_SPACE_DASH=21
+SYMBOL=22
+DOLLAR=23
+HAT=24
 DASH=25
 DOT=26
 FSLASH=27
 UNDERSCORE=28
-COLON=29
-SPACE=30
-LPAREN=31
-RPAREN=32
-HASH=33
-AT_SIGN=34
-PLUS=35
-PERCENT=36
-SQUOTE=37
-DQUOTE=38
-TILDE=39
-STAR=40
-LANGLE=41
-RANGLE=42
-'S'=1
-'W'=2
-'O'=3
-'G'=4
-'note'=5
-'or'=6
-'['=7
-']'=8
-'!'=9
-'date'=10
-'priority'=11
-'file'=12
-'type'=13
-'o'=15
-'x'=16
-'  -'=22
-'    -'=23
+SPACE=29
+LPAREN=30
+RPAREN=31
+HASH=32
+AT_SIGN=33
+PLUS=34
+PERCENT=35
+SQUOTE=36
+DQUOTE=37
+TILDE=38
+STAR=39
+LANGLE=40
+RANGLE=41
+COLON=42
+'[['=1
+']]'=2
+'['=3
+']'=4
+'======='=5
+'*****'=6
+'o'=8
+'x'=9
+'  -'=20
+'    -'=21
+'$'=23
+'^'=24
 '-'=25
 '.'=26
 '/'=27
 '_'=28
-':'=29
-' '=30
-'('=31
-')'=32
-'#'=33
-'@'=34
-'+'=35
-'%'=36
-'\''=37
-'"'=38
-'~'=39
-'*'=40
-'<'=41
-'>'=42
+' '=29
+'('=30
+')'=31
+'#'=32
+'@'=33
+'+'=34
+'%'=35
+'\''=36
+'"'=37
+'~'=38
+'*'=39
+'<'=40
+'>'=41
+':'=42
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryListener.py` & `zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryListener.py`

 * *Files 10% similar despite different names*

```diff
@@ -220,14 +220,95 @@
         pass
 
     # Exit a parse tree produced by ZorgQueryParser#subfilter.
     def exitSubfilter(self, ctx:ZorgQueryParser.SubfilterContext):
         pass
 
 
+    # Enter a parse tree produced by ZorgQueryParser#create_range.
+    def enterCreate_range(self, ctx:ZorgQueryParser.Create_rangeContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#create_range.
+    def exitCreate_range(self, ctx:ZorgQueryParser.Create_rangeContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#modify_range.
+    def enterModify_range(self, ctx:ZorgQueryParser.Modify_rangeContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#modify_range.
+    def exitModify_range(self, ctx:ZorgQueryParser.Modify_rangeContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#prop_filter.
+    def enterProp_filter(self, ctx:ZorgQueryParser.Prop_filterContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#prop_filter.
+    def exitProp_filter(self, ctx:ZorgQueryParser.Prop_filterContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#prop_op.
+    def enterProp_op(self, ctx:ZorgQueryParser.Prop_opContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#prop_op.
+    def exitProp_op(self, ctx:ZorgQueryParser.Prop_opContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#desc_filter.
+    def enterDesc_filter(self, ctx:ZorgQueryParser.Desc_filterContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#desc_filter.
+    def exitDesc_filter(self, ctx:ZorgQueryParser.Desc_filterContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#zid.
+    def enterZid(self, ctx:ZorgQueryParser.ZidContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#zid.
+    def exitZid(self, ctx:ZorgQueryParser.ZidContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#id.
+    def enterId(self, ctx:ZorgQueryParser.IdContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#id.
+    def exitId(self, ctx:ZorgQueryParser.IdContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#date.
+    def enterDate(self, ctx:ZorgQueryParser.DateContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#date.
+    def exitDate(self, ctx:ZorgQueryParser.DateContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#time.
+    def enterTime(self, ctx:ZorgQueryParser.TimeContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#time.
+    def exitTime(self, ctx:ZorgQueryParser.TimeContext):
+        pass
+
+
     # Enter a parse tree produced by ZorgQueryParser#group_by_body.
     def enterGroup_by_body(self, ctx:ZorgQueryParser.Group_by_bodyContext):
         pass
 
     # Exit a parse tree produced by ZorgQueryParser#group_by_body.
     def exitGroup_by_body(self, ctx:ZorgQueryParser.Group_by_bodyContext):
         pass
@@ -256,20 +337,29 @@
         pass
 
     # Exit a parse tree produced by ZorgQueryParser#order_by_atom.
     def exitOrder_by_atom(self, ctx:ZorgQueryParser.Order_by_atomContext):
         pass
 
 
-    # Enter a parse tree produced by ZorgQueryParser#date.
-    def enterDate(self, ctx:ZorgQueryParser.DateContext):
+    # Enter a parse tree produced by ZorgQueryParser#create.
+    def enterCreate(self, ctx:ZorgQueryParser.CreateContext):
         pass
 
-    # Exit a parse tree produced by ZorgQueryParser#date.
-    def exitDate(self, ctx:ZorgQueryParser.DateContext):
+    # Exit a parse tree produced by ZorgQueryParser#create.
+    def exitCreate(self, ctx:ZorgQueryParser.CreateContext):
+        pass
+
+
+    # Enter a parse tree produced by ZorgQueryParser#modify.
+    def enterModify(self, ctx:ZorgQueryParser.ModifyContext):
+        pass
+
+    # Exit a parse tree produced by ZorgQueryParser#modify.
+    def exitModify(self, ctx:ZorgQueryParser.ModifyContext):
         pass
 
 
     # Enter a parse tree produced by ZorgQueryParser#priority.
     def enterPriority(self, ctx:ZorgQueryParser.PriorityContext):
         pass
```

### Comparing `zettel_org-0.7.2/src/zorg/grammar/zorg_query/ZorgQueryParser.py` & `zettel_org-0.7.3/src/zorg/grammar/zorg_query/ZorgQueryParser.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,118 +6,165 @@
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
 	from typing.io import TextIO
 
 def serializedATN():
     return [
-        4,1,42,222,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
+        4,1,61,316,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
         6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,13,7,13,
         2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,19,2,20,
         7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,26,7,26,
-        2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,1,0,1,0,3,0,67,
-        8,0,1,1,1,1,3,1,71,8,1,1,2,1,2,1,2,3,2,76,8,2,1,2,1,2,1,2,3,2,81,
-        8,2,1,2,1,2,3,2,85,8,2,1,3,1,3,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,5,1,
-        6,1,6,1,6,1,6,1,7,1,7,1,7,1,7,1,8,1,8,1,8,1,8,1,8,1,8,3,8,111,8,
-        8,1,9,1,9,1,10,1,10,1,11,1,11,1,11,1,11,1,11,5,11,122,8,11,10,11,
-        12,11,125,9,11,1,12,1,12,1,12,5,12,130,8,12,10,12,12,12,133,9,12,
-        1,13,1,13,1,13,1,13,3,13,139,8,13,1,14,4,14,142,8,14,11,14,12,14,
-        143,1,15,1,15,1,16,1,16,1,16,1,16,1,16,1,17,3,17,154,8,17,1,17,1,
-        17,1,17,1,17,3,17,160,8,17,1,18,1,18,1,19,1,19,1,19,1,20,1,20,1,
-        20,1,21,1,21,1,21,1,22,1,22,1,22,1,23,1,23,1,23,1,23,1,24,1,24,1,
-        24,3,24,183,8,24,1,24,1,24,3,24,187,8,24,1,24,1,24,3,24,191,8,24,
-        1,25,1,25,1,25,1,25,1,25,1,25,3,25,199,8,25,1,26,1,26,1,26,5,26,
-        204,8,26,10,26,12,26,207,9,26,1,27,1,27,1,27,3,27,212,8,27,1,28,
-        1,28,1,29,1,29,1,30,1,30,1,31,1,31,1,31,0,0,32,0,2,4,6,8,10,12,14,
-        16,18,20,22,24,26,28,30,32,34,36,38,40,42,44,46,48,50,52,54,56,58,
-        60,62,0,1,4,0,15,16,25,25,39,39,41,42,220,0,64,1,0,0,0,2,70,1,0,
-        0,0,4,75,1,0,0,0,6,86,1,0,0,0,8,88,1,0,0,0,10,92,1,0,0,0,12,96,1,
-        0,0,0,14,100,1,0,0,0,16,110,1,0,0,0,18,112,1,0,0,0,20,114,1,0,0,
-        0,22,116,1,0,0,0,24,126,1,0,0,0,26,138,1,0,0,0,28,141,1,0,0,0,30,
-        145,1,0,0,0,32,147,1,0,0,0,34,153,1,0,0,0,36,161,1,0,0,0,38,163,
-        1,0,0,0,40,166,1,0,0,0,42,169,1,0,0,0,44,172,1,0,0,0,46,175,1,0,
-        0,0,48,179,1,0,0,0,50,198,1,0,0,0,52,200,1,0,0,0,54,211,1,0,0,0,
-        56,213,1,0,0,0,58,215,1,0,0,0,60,217,1,0,0,0,62,219,1,0,0,0,64,66,
-        3,2,1,0,65,67,5,14,0,0,66,65,1,0,0,0,66,67,1,0,0,0,67,1,1,0,0,0,
-        68,71,3,4,2,0,69,71,3,6,3,0,70,68,1,0,0,0,70,69,1,0,0,0,71,3,1,0,
-        0,0,72,73,3,8,4,0,73,74,5,30,0,0,74,76,1,0,0,0,75,72,1,0,0,0,75,
-        76,1,0,0,0,76,77,1,0,0,0,77,80,3,10,5,0,78,79,5,30,0,0,79,81,3,12,
-        6,0,80,78,1,0,0,0,80,81,1,0,0,0,81,84,1,0,0,0,82,83,5,30,0,0,83,
-        85,3,14,7,0,84,82,1,0,0,0,84,85,1,0,0,0,85,5,1,0,0,0,86,87,3,8,4,
-        0,87,7,1,0,0,0,88,89,5,1,0,0,89,90,5,30,0,0,90,91,3,16,8,0,91,9,
-        1,0,0,0,92,93,5,2,0,0,93,94,5,30,0,0,94,95,3,20,10,0,95,11,1,0,0,
-        0,96,97,5,3,0,0,97,98,5,30,0,0,98,99,3,52,26,0,99,13,1,0,0,0,100,
-        101,5,4,0,0,101,102,5,30,0,0,102,103,3,48,24,0,103,15,1,0,0,0,104,
-        111,3,60,30,0,105,111,3,18,9,0,106,111,5,34,0,0,107,111,5,33,0,0,
-        108,111,5,35,0,0,109,111,5,36,0,0,110,104,1,0,0,0,110,105,1,0,0,
-        0,110,106,1,0,0,0,110,107,1,0,0,0,110,108,1,0,0,0,110,109,1,0,0,
-        0,111,17,1,0,0,0,112,113,5,5,0,0,113,19,1,0,0,0,114,115,3,22,11,
-        0,115,21,1,0,0,0,116,123,3,24,12,0,117,118,5,30,0,0,118,119,5,6,
-        0,0,119,120,5,30,0,0,120,122,3,24,12,0,121,117,1,0,0,0,122,125,1,
-        0,0,0,123,121,1,0,0,0,123,124,1,0,0,0,124,23,1,0,0,0,125,123,1,0,
-        0,0,126,131,3,26,13,0,127,128,5,30,0,0,128,130,3,26,13,0,129,127,
-        1,0,0,0,130,133,1,0,0,0,131,129,1,0,0,0,131,132,1,0,0,0,132,25,1,
-        0,0,0,133,131,1,0,0,0,134,139,3,28,14,0,135,139,3,32,16,0,136,139,
-        3,34,17,0,137,139,3,46,23,0,138,134,1,0,0,0,138,135,1,0,0,0,138,
-        136,1,0,0,0,138,137,1,0,0,0,139,27,1,0,0,0,140,142,3,30,15,0,141,
-        140,1,0,0,0,142,143,1,0,0,0,143,141,1,0,0,0,143,144,1,0,0,0,144,
-        29,1,0,0,0,145,146,7,0,0,0,146,31,1,0,0,0,147,148,5,7,0,0,148,149,
-        5,33,0,0,149,150,5,19,0,0,150,151,5,8,0,0,151,33,1,0,0,0,152,154,
-        3,36,18,0,153,152,1,0,0,0,153,154,1,0,0,0,154,159,1,0,0,0,155,160,
-        3,38,19,0,156,160,3,40,20,0,157,160,3,42,21,0,158,160,3,44,22,0,
-        159,155,1,0,0,0,159,156,1,0,0,0,159,157,1,0,0,0,159,158,1,0,0,0,
-        160,35,1,0,0,0,161,162,5,9,0,0,162,37,1,0,0,0,163,164,5,33,0,0,164,
-        165,5,19,0,0,165,39,1,0,0,0,166,167,5,34,0,0,167,168,5,19,0,0,168,
-        41,1,0,0,0,169,170,5,36,0,0,170,171,5,19,0,0,171,43,1,0,0,0,172,
-        173,5,35,0,0,173,174,5,19,0,0,174,45,1,0,0,0,175,176,5,31,0,0,176,
-        177,3,22,11,0,177,178,5,32,0,0,178,47,1,0,0,0,179,182,3,50,25,0,
-        180,181,5,30,0,0,181,183,3,50,25,0,182,180,1,0,0,0,182,183,1,0,0,
-        0,183,186,1,0,0,0,184,185,5,30,0,0,185,187,3,50,25,0,186,184,1,0,
-        0,0,186,187,1,0,0,0,187,190,1,0,0,0,188,189,5,30,0,0,189,191,3,50,
-        25,0,190,188,1,0,0,0,190,191,1,0,0,0,191,49,1,0,0,0,192,199,3,60,
-        30,0,193,199,3,62,31,0,194,199,5,34,0,0,195,199,5,33,0,0,196,199,
-        5,36,0,0,197,199,5,35,0,0,198,192,1,0,0,0,198,193,1,0,0,0,198,194,
-        1,0,0,0,198,195,1,0,0,0,198,196,1,0,0,0,198,197,1,0,0,0,199,51,1,
-        0,0,0,200,205,3,54,27,0,201,202,5,30,0,0,202,204,3,54,27,0,203,201,
-        1,0,0,0,204,207,1,0,0,0,205,203,1,0,0,0,205,206,1,0,0,0,206,53,1,
-        0,0,0,207,205,1,0,0,0,208,212,3,56,28,0,209,212,3,58,29,0,210,212,
-        3,62,31,0,211,208,1,0,0,0,211,209,1,0,0,0,211,210,1,0,0,0,212,55,
-        1,0,0,0,213,214,5,10,0,0,214,57,1,0,0,0,215,216,5,11,0,0,216,59,
-        1,0,0,0,217,218,5,12,0,0,218,61,1,0,0,0,219,220,5,13,0,0,220,63,
-        1,0,0,0,18,66,70,75,80,84,110,123,131,138,143,153,159,182,186,190,
-        198,205,211
+        2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,32,2,33,
+        7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,39,7,39,
+        2,40,7,40,2,41,7,41,1,0,1,0,3,0,87,8,0,1,1,1,1,3,1,91,8,1,1,2,1,
+        2,1,2,3,2,96,8,2,1,2,1,2,1,2,3,2,101,8,2,1,2,1,2,3,2,105,8,2,1,3,
+        1,3,1,4,1,4,1,4,1,4,1,5,1,5,1,5,1,5,1,6,1,6,1,6,1,6,1,7,1,7,1,7,
+        1,7,1,8,1,8,1,8,1,8,1,8,1,8,3,8,131,8,8,1,9,1,9,1,10,1,10,1,11,1,
+        11,1,11,1,11,1,11,5,11,142,8,11,10,11,12,11,145,9,11,1,12,1,12,1,
+        12,5,12,150,8,12,10,12,12,12,153,9,12,1,13,1,13,1,13,1,13,1,13,1,
+        13,1,13,1,13,3,13,163,8,13,1,14,4,14,166,8,14,11,14,12,14,167,1,
+        15,1,15,1,16,1,16,1,16,3,16,175,8,16,1,17,3,17,178,8,17,1,17,1,17,
+        1,17,1,17,3,17,184,8,17,1,18,1,18,1,19,1,19,1,19,1,20,1,20,1,20,
+        1,21,1,21,1,21,1,22,1,22,1,22,1,23,1,23,1,23,1,23,1,24,1,24,3,24,
+        206,8,24,1,25,1,25,3,25,210,8,25,1,26,3,26,213,8,26,1,26,1,26,1,
+        26,3,26,218,8,26,1,26,1,26,4,26,222,8,26,11,26,12,26,223,3,26,226,
+        8,26,1,26,3,26,229,8,26,1,26,3,26,232,8,26,1,27,1,27,1,28,3,28,237,
+        8,28,1,28,3,28,240,8,28,1,28,1,28,1,28,1,28,5,28,246,8,28,10,28,
+        12,28,249,9,28,1,28,1,28,1,29,1,29,1,30,1,30,1,30,1,30,1,30,1,30,
+        1,30,1,30,1,30,3,30,264,8,30,1,31,1,31,1,32,1,32,1,33,1,33,1,33,
+        3,33,273,8,33,1,33,1,33,3,33,277,8,33,1,33,1,33,3,33,281,8,33,1,
+        34,1,34,1,34,1,34,1,34,1,34,1,34,3,34,290,8,34,1,35,1,35,1,35,5,
+        35,295,8,35,10,35,12,35,298,9,35,1,36,1,36,1,36,1,36,3,36,304,8,
+        36,1,37,1,37,1,38,1,38,1,39,1,39,1,40,1,40,1,41,1,41,1,41,0,0,42,
+        0,2,4,6,8,10,12,14,16,18,20,22,24,26,28,30,32,34,36,38,40,42,44,
+        46,48,50,52,54,56,58,60,62,64,66,68,70,72,74,76,78,80,82,0,4,4,0,
+        27,28,44,44,57,57,59,60,1,0,7,15,2,0,7,15,17,17,2,0,18,19,59,60,
+        330,0,84,1,0,0,0,2,90,1,0,0,0,4,95,1,0,0,0,6,106,1,0,0,0,8,108,1,
+        0,0,0,10,112,1,0,0,0,12,116,1,0,0,0,14,120,1,0,0,0,16,130,1,0,0,
+        0,18,132,1,0,0,0,20,134,1,0,0,0,22,136,1,0,0,0,24,146,1,0,0,0,26,
+        162,1,0,0,0,28,165,1,0,0,0,30,169,1,0,0,0,32,171,1,0,0,0,34,177,
+        1,0,0,0,36,185,1,0,0,0,38,187,1,0,0,0,40,190,1,0,0,0,42,193,1,0,
+        0,0,44,196,1,0,0,0,46,199,1,0,0,0,48,203,1,0,0,0,50,207,1,0,0,0,
+        52,212,1,0,0,0,54,233,1,0,0,0,56,236,1,0,0,0,58,252,1,0,0,0,60,263,
+        1,0,0,0,62,265,1,0,0,0,64,267,1,0,0,0,66,269,1,0,0,0,68,289,1,0,
+        0,0,70,291,1,0,0,0,72,303,1,0,0,0,74,305,1,0,0,0,76,307,1,0,0,0,
+        78,309,1,0,0,0,80,311,1,0,0,0,82,313,1,0,0,0,84,86,3,2,1,0,85,87,
+        5,26,0,0,86,85,1,0,0,0,86,87,1,0,0,0,87,1,1,0,0,0,88,91,3,4,2,0,
+        89,91,3,6,3,0,90,88,1,0,0,0,90,89,1,0,0,0,91,3,1,0,0,0,92,93,3,8,
+        4,0,93,94,5,48,0,0,94,96,1,0,0,0,95,92,1,0,0,0,95,96,1,0,0,0,96,
+        97,1,0,0,0,97,100,3,10,5,0,98,99,5,48,0,0,99,101,3,12,6,0,100,98,
+        1,0,0,0,100,101,1,0,0,0,101,104,1,0,0,0,102,103,5,48,0,0,103,105,
+        3,14,7,0,104,102,1,0,0,0,104,105,1,0,0,0,105,5,1,0,0,0,106,107,3,
+        8,4,0,107,7,1,0,0,0,108,109,5,1,0,0,109,110,5,48,0,0,110,111,3,16,
+        8,0,111,9,1,0,0,0,112,113,5,2,0,0,113,114,5,48,0,0,114,115,3,20,
+        10,0,115,11,1,0,0,0,116,117,5,3,0,0,117,118,5,48,0,0,118,119,3,70,
+        35,0,119,13,1,0,0,0,120,121,5,4,0,0,121,122,5,48,0,0,122,123,3,66,
+        33,0,123,15,1,0,0,0,124,131,3,80,40,0,125,131,3,18,9,0,126,131,5,
+        52,0,0,127,131,5,51,0,0,128,131,5,53,0,0,129,131,5,54,0,0,130,124,
+        1,0,0,0,130,125,1,0,0,0,130,126,1,0,0,0,130,127,1,0,0,0,130,128,
+        1,0,0,0,130,129,1,0,0,0,131,17,1,0,0,0,132,133,5,5,0,0,133,19,1,
+        0,0,0,134,135,3,22,11,0,135,21,1,0,0,0,136,143,3,24,12,0,137,138,
+        5,48,0,0,138,139,5,6,0,0,139,140,5,48,0,0,140,142,3,24,12,0,141,
+        137,1,0,0,0,142,145,1,0,0,0,143,141,1,0,0,0,143,144,1,0,0,0,144,
+        23,1,0,0,0,145,143,1,0,0,0,146,151,3,26,13,0,147,148,5,48,0,0,148,
+        150,3,26,13,0,149,147,1,0,0,0,150,153,1,0,0,0,151,149,1,0,0,0,151,
+        152,1,0,0,0,152,25,1,0,0,0,153,151,1,0,0,0,154,163,3,28,14,0,155,
+        163,3,32,16,0,156,163,3,34,17,0,157,163,3,46,23,0,158,163,3,48,24,
+        0,159,163,3,50,25,0,160,163,3,52,26,0,161,163,3,56,28,0,162,154,
+        1,0,0,0,162,155,1,0,0,0,162,156,1,0,0,0,162,157,1,0,0,0,162,158,
+        1,0,0,0,162,159,1,0,0,0,162,160,1,0,0,0,162,161,1,0,0,0,163,27,1,
+        0,0,0,164,166,3,30,15,0,165,164,1,0,0,0,166,167,1,0,0,0,167,165,
+        1,0,0,0,167,168,1,0,0,0,168,29,1,0,0,0,169,170,7,0,0,0,170,31,1,
+        0,0,0,171,174,5,34,0,0,172,173,5,44,0,0,173,175,7,1,0,0,174,172,
+        1,0,0,0,174,175,1,0,0,0,175,33,1,0,0,0,176,178,3,36,18,0,177,176,
+        1,0,0,0,177,178,1,0,0,0,178,183,1,0,0,0,179,184,3,38,19,0,180,184,
+        3,40,20,0,181,184,3,42,21,0,182,184,3,44,22,0,183,179,1,0,0,0,183,
+        180,1,0,0,0,183,181,1,0,0,0,183,182,1,0,0,0,184,35,1,0,0,0,185,186,
+        5,16,0,0,186,37,1,0,0,0,187,188,5,51,0,0,188,189,5,35,0,0,189,39,
+        1,0,0,0,190,191,5,52,0,0,191,192,5,35,0,0,192,41,1,0,0,0,193,194,
+        5,54,0,0,194,195,5,35,0,0,195,43,1,0,0,0,196,197,5,53,0,0,197,198,
+        5,35,0,0,198,45,1,0,0,0,199,200,5,49,0,0,200,201,3,22,11,0,201,202,
+        5,50,0,0,202,47,1,0,0,0,203,205,5,31,0,0,204,206,5,33,0,0,205,204,
+        1,0,0,0,205,206,1,0,0,0,206,49,1,0,0,0,207,209,5,32,0,0,208,210,
+        5,33,0,0,209,208,1,0,0,0,209,210,1,0,0,0,210,51,1,0,0,0,211,213,
+        3,36,18,0,212,211,1,0,0,0,212,213,1,0,0,0,213,214,1,0,0,0,214,215,
+        5,35,0,0,215,217,5,61,0,0,216,218,3,54,27,0,217,216,1,0,0,0,217,
+        218,1,0,0,0,218,231,1,0,0,0,219,226,5,35,0,0,220,222,7,2,0,0,221,
+        220,1,0,0,0,222,223,1,0,0,0,223,221,1,0,0,0,223,224,1,0,0,0,224,
+        226,1,0,0,0,225,219,1,0,0,0,225,221,1,0,0,0,226,228,1,0,0,0,227,
+        229,5,58,0,0,228,227,1,0,0,0,228,229,1,0,0,0,229,232,1,0,0,0,230,
+        232,5,58,0,0,231,225,1,0,0,0,231,230,1,0,0,0,232,53,1,0,0,0,233,
+        234,7,3,0,0,234,55,1,0,0,0,235,237,3,36,18,0,236,235,1,0,0,0,236,
+        237,1,0,0,0,237,239,1,0,0,0,238,240,5,20,0,0,239,238,1,0,0,0,239,
+        240,1,0,0,0,240,241,1,0,0,0,241,242,5,55,0,0,242,247,3,60,30,0,243,
+        244,5,48,0,0,244,246,3,60,30,0,245,243,1,0,0,0,246,249,1,0,0,0,247,
+        245,1,0,0,0,247,248,1,0,0,0,248,250,1,0,0,0,249,247,1,0,0,0,250,
+        251,5,55,0,0,251,57,1,0,0,0,252,253,5,36,0,0,253,59,1,0,0,0,254,
+        264,5,35,0,0,255,264,5,38,0,0,256,264,5,33,0,0,257,264,5,34,0,0,
+        258,264,3,62,31,0,259,264,3,64,32,0,260,264,3,58,29,0,261,264,5,
+        27,0,0,262,264,5,28,0,0,263,254,1,0,0,0,263,255,1,0,0,0,263,256,
+        1,0,0,0,263,257,1,0,0,0,263,258,1,0,0,0,263,259,1,0,0,0,263,260,
+        1,0,0,0,263,261,1,0,0,0,263,262,1,0,0,0,264,61,1,0,0,0,265,266,5,
+        29,0,0,266,63,1,0,0,0,267,268,5,30,0,0,268,65,1,0,0,0,269,272,3,
+        68,34,0,270,271,5,48,0,0,271,273,3,68,34,0,272,270,1,0,0,0,272,273,
+        1,0,0,0,273,276,1,0,0,0,274,275,5,48,0,0,275,277,3,68,34,0,276,274,
+        1,0,0,0,276,277,1,0,0,0,277,280,1,0,0,0,278,279,5,48,0,0,279,281,
+        3,68,34,0,280,278,1,0,0,0,280,281,1,0,0,0,281,67,1,0,0,0,282,290,
+        3,80,40,0,283,290,3,82,41,0,284,290,3,78,39,0,285,290,5,52,0,0,286,
+        290,5,51,0,0,287,290,5,54,0,0,288,290,5,53,0,0,289,282,1,0,0,0,289,
+        283,1,0,0,0,289,284,1,0,0,0,289,285,1,0,0,0,289,286,1,0,0,0,289,
+        287,1,0,0,0,289,288,1,0,0,0,290,69,1,0,0,0,291,296,3,72,36,0,292,
+        293,5,48,0,0,293,295,3,72,36,0,294,292,1,0,0,0,295,298,1,0,0,0,296,
+        294,1,0,0,0,296,297,1,0,0,0,297,71,1,0,0,0,298,296,1,0,0,0,299,304,
+        3,74,37,0,300,304,3,76,38,0,301,304,3,78,39,0,302,304,3,82,41,0,
+        303,299,1,0,0,0,303,300,1,0,0,0,303,301,1,0,0,0,303,302,1,0,0,0,
+        304,73,1,0,0,0,305,306,5,21,0,0,306,75,1,0,0,0,307,308,5,22,0,0,
+        308,77,1,0,0,0,309,310,5,23,0,0,310,79,1,0,0,0,311,312,5,24,0,0,
+        312,81,1,0,0,0,313,314,5,25,0,0,314,83,1,0,0,0,31,86,90,95,100,104,
+        130,143,151,162,167,174,177,183,205,209,212,217,223,225,228,231,
+        236,239,247,263,272,276,280,289,296,303
     ]
 
 class ZorgQueryParser ( Parser ):
 
     grammarFileName = "ZorgQuery.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
 
     sharedContextCache = PredictionContextCache()
 
     literalNames = [ "<INVALID>", "'S'", "'W'", "'O'", "'G'", "'note'", 
-                     "'or'", "'['", "']'", "'!'", "'date'", "'priority'", 
-                     "'file'", "'type'", "<INVALID>", "'o'", "'x'", "<INVALID>", 
+                     "'or'", "'1'", "'2'", "'3'", "'4'", "'5'", "'6'", "'7'", 
+                     "'8'", "'9'", "'!'", "'0'", "'<='", "'>='", "'c'", 
+                     "'create'", "'modify'", "'priority'", "'file'", "'type'", 
+                     "<INVALID>", "'o'", "'x'", "<INVALID>", "<INVALID>", 
                      "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
-                     "'  -'", "'    -'", "<INVALID>", "'-'", "'.'", "'/'", 
-                     "'_'", "':'", "' '", "'('", "')'", "'#'", "'@'", "'+'", 
-                     "'%'", "'''", "'\"'", "'~'", "'*'", "'<'", "'>'" ]
+                     "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
+                     "'  -'", "'    -'", "<INVALID>", "'$'", "'^'", "'-'", 
+                     "'.'", "'/'", "'_'", "' '", "'('", "')'", "'#'", "'@'", 
+                     "'+'", "'%'", "'''", "'\"'", "'~'", "'*'", "'<'", "'>'", 
+                     "':'" ]
 
     symbolicNames = [ "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
+                      "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
+                      "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
+                      "<INVALID>", "<INVALID>", "<INVALID>", "<INVALID>", 
                       "<INVALID>", "<INVALID>", "NL", "LOWER_O", "LOWER_X", 
-                      "DATE", "TIME", "ID", "ZID", "NUM_ID", "TWO_SPACE_DASH", 
-                      "FOUR_SPACE_DASH", "SYMBOL", "DASH", "DOT", "FSLASH", 
-                      "UNDERSCORE", "COLON", "SPACE", "LPAREN", "RPAREN", 
-                      "HASH", "AT_SIGN", "PLUS", "PERCENT", "SQUOTE", "DQUOTE", 
-                      "TILDE", "STAR", "LANGLE", "RANGLE" ]
+                      "DATE", "TIME", "CREATE_RANGE_HEAD", "MODIFY_RANGE_HEAD", 
+                      "DATE_RANGE_TAIL", "PRIORITY", "ID", "ZID", "SHORT_DATE", 
+                      "NUM_ID", "TWO_SPACE_DASH", "FOUR_SPACE_DASH", "SYMBOL", 
+                      "DOLLAR", "HAT", "DASH", "DOT", "FSLASH", "UNDERSCORE", 
+                      "SPACE", "LPAREN", "RPAREN", "HASH", "AT_SIGN", "PLUS", 
+                      "PERCENT", "SQUOTE", "DQUOTE", "TILDE", "STAR", "LANGLE", 
+                      "RANGLE", "COLON" ]
 
     RULE_prog = 0
     RULE_query = 1
     RULE_where_query = 2
     RULE_select_query = 3
     RULE_select = 4
     RULE_where = 5
@@ -135,30 +182,42 @@
     RULE_tag = 17
     RULE_not_op = 18
     RULE_area = 19
     RULE_context = 20
     RULE_person = 21
     RULE_project = 22
     RULE_subfilter = 23
-    RULE_group_by_body = 24
-    RULE_group_by_atom = 25
-    RULE_order_by_body = 26
-    RULE_order_by_atom = 27
-    RULE_date = 28
-    RULE_priority = 29
-    RULE_file = 30
-    RULE_type = 31
+    RULE_create_range = 24
+    RULE_modify_range = 25
+    RULE_prop_filter = 26
+    RULE_prop_op = 27
+    RULE_desc_filter = 28
+    RULE_zid = 29
+    RULE_id = 30
+    RULE_date = 31
+    RULE_time = 32
+    RULE_group_by_body = 33
+    RULE_group_by_atom = 34
+    RULE_order_by_body = 35
+    RULE_order_by_atom = 36
+    RULE_create = 37
+    RULE_modify = 38
+    RULE_priority = 39
+    RULE_file = 40
+    RULE_type = 41
 
     ruleNames =  [ "prog", "query", "where_query", "select_query", "select", 
                    "where", "order_by", "group_by", "select_body", "note", 
                    "where_body", "or_filter", "and_filter", "where_atom", 
                    "note_type", "note_type_char", "priority_range", "tag", 
                    "not_op", "area", "context", "person", "project", "subfilter", 
-                   "group_by_body", "group_by_atom", "order_by_body", "order_by_atom", 
-                   "date", "priority", "file", "type" ]
+                   "create_range", "modify_range", "prop_filter", "prop_op", 
+                   "desc_filter", "zid", "id", "date", "time", "group_by_body", 
+                   "group_by_atom", "order_by_body", "order_by_atom", "create", 
+                   "modify", "priority", "file", "type" ]
 
     EOF = Token.EOF
     T__0=1
     T__1=2
     T__2=3
     T__3=4
     T__4=5
@@ -166,43 +225,62 @@
     T__6=7
     T__7=8
     T__8=9
     T__9=10
     T__10=11
     T__11=12
     T__12=13
-    NL=14
-    LOWER_O=15
-    LOWER_X=16
-    DATE=17
-    TIME=18
-    ID=19
-    ZID=20
-    NUM_ID=21
-    TWO_SPACE_DASH=22
-    FOUR_SPACE_DASH=23
-    SYMBOL=24
-    DASH=25
-    DOT=26
-    FSLASH=27
-    UNDERSCORE=28
-    COLON=29
-    SPACE=30
-    LPAREN=31
-    RPAREN=32
-    HASH=33
-    AT_SIGN=34
-    PLUS=35
-    PERCENT=36
-    SQUOTE=37
-    DQUOTE=38
-    TILDE=39
-    STAR=40
-    LANGLE=41
-    RANGLE=42
+    T__13=14
+    T__14=15
+    T__15=16
+    T__16=17
+    T__17=18
+    T__18=19
+    T__19=20
+    T__20=21
+    T__21=22
+    T__22=23
+    T__23=24
+    T__24=25
+    NL=26
+    LOWER_O=27
+    LOWER_X=28
+    DATE=29
+    TIME=30
+    CREATE_RANGE_HEAD=31
+    MODIFY_RANGE_HEAD=32
+    DATE_RANGE_TAIL=33
+    PRIORITY=34
+    ID=35
+    ZID=36
+    SHORT_DATE=37
+    NUM_ID=38
+    TWO_SPACE_DASH=39
+    FOUR_SPACE_DASH=40
+    SYMBOL=41
+    DOLLAR=42
+    HAT=43
+    DASH=44
+    DOT=45
+    FSLASH=46
+    UNDERSCORE=47
+    SPACE=48
+    LPAREN=49
+    RPAREN=50
+    HASH=51
+    AT_SIGN=52
+    PLUS=53
+    PERCENT=54
+    SQUOTE=55
+    DQUOTE=56
+    TILDE=57
+    STAR=58
+    LANGLE=59
+    RANGLE=60
+    COLON=61
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.13.1")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
@@ -240,21 +318,21 @@
     def prog(self):
 
         localctx = ZorgQueryParser.ProgContext(self, self._ctx, self.state)
         self.enterRule(localctx, 0, self.RULE_prog)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 64
+            self.state = 84
             self.query()
-            self.state = 66
+            self.state = 86
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==14:
-                self.state = 65
+            if _la==26:
+                self.state = 85
                 self.match(ZorgQueryParser.NL)
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -293,26 +371,26 @@
 
 
     def query(self):
 
         localctx = ZorgQueryParser.QueryContext(self, self._ctx, self.state)
         self.enterRule(localctx, 2, self.RULE_query)
         try:
-            self.state = 70
+            self.state = 90
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,1,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 68
+                self.state = 88
                 self.where_query()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 69
+                self.state = 89
                 self.select_query()
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -368,43 +446,43 @@
     def where_query(self):
 
         localctx = ZorgQueryParser.Where_queryContext(self, self._ctx, self.state)
         self.enterRule(localctx, 4, self.RULE_where_query)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 75
+            self.state = 95
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la==1:
-                self.state = 72
+                self.state = 92
                 self.select()
-                self.state = 73
+                self.state = 93
                 self.match(ZorgQueryParser.SPACE)
 
 
-            self.state = 77
+            self.state = 97
             self.where()
-            self.state = 80
+            self.state = 100
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,3,self._ctx)
             if la_ == 1:
-                self.state = 78
+                self.state = 98
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 79
+                self.state = 99
                 self.order_by()
 
 
-            self.state = 84
+            self.state = 104
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==30:
-                self.state = 82
+            if _la==48:
+                self.state = 102
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 83
+                self.state = 103
                 self.group_by()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -440,15 +518,15 @@
 
     def select_query(self):
 
         localctx = ZorgQueryParser.Select_queryContext(self, self._ctx, self.state)
         self.enterRule(localctx, 6, self.RULE_select_query)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 86
+            self.state = 106
             self.select()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -485,19 +563,19 @@
 
     def select(self):
 
         localctx = ZorgQueryParser.SelectContext(self, self._ctx, self.state)
         self.enterRule(localctx, 8, self.RULE_select)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 88
+            self.state = 108
             self.match(ZorgQueryParser.T__0)
-            self.state = 89
+            self.state = 109
             self.match(ZorgQueryParser.SPACE)
-            self.state = 90
+            self.state = 110
             self.select_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -534,19 +612,19 @@
 
     def where(self):
 
         localctx = ZorgQueryParser.WhereContext(self, self._ctx, self.state)
         self.enterRule(localctx, 10, self.RULE_where)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 92
+            self.state = 112
             self.match(ZorgQueryParser.T__1)
-            self.state = 93
+            self.state = 113
             self.match(ZorgQueryParser.SPACE)
-            self.state = 94
+            self.state = 114
             self.where_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -583,19 +661,19 @@
 
     def order_by(self):
 
         localctx = ZorgQueryParser.Order_byContext(self, self._ctx, self.state)
         self.enterRule(localctx, 12, self.RULE_order_by)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 96
+            self.state = 116
             self.match(ZorgQueryParser.T__2)
-            self.state = 97
+            self.state = 117
             self.match(ZorgQueryParser.SPACE)
-            self.state = 98
+            self.state = 118
             self.order_by_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -632,19 +710,19 @@
 
     def group_by(self):
 
         localctx = ZorgQueryParser.Group_byContext(self, self._ctx, self.state)
         self.enterRule(localctx, 14, self.RULE_group_by)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 100
+            self.state = 120
             self.match(ZorgQueryParser.T__3)
-            self.state = 101
+            self.state = 121
             self.match(ZorgQueryParser.SPACE)
-            self.state = 102
+            self.state = 122
             self.group_by_body()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -693,45 +771,45 @@
 
 
     def select_body(self):
 
         localctx = ZorgQueryParser.Select_bodyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 16, self.RULE_select_body)
         try:
-            self.state = 110
+            self.state = 130
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [12]:
+            if token in [24]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 104
+                self.state = 124
                 self.file_()
                 pass
             elif token in [5]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 105
+                self.state = 125
                 self.note()
                 pass
-            elif token in [34]:
+            elif token in [52]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 106
+                self.state = 126
                 self.match(ZorgQueryParser.AT_SIGN)
                 pass
-            elif token in [33]:
+            elif token in [51]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 107
+                self.state = 127
                 self.match(ZorgQueryParser.HASH)
                 pass
-            elif token in [35]:
+            elif token in [53]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 108
+                self.state = 128
                 self.match(ZorgQueryParser.PLUS)
                 pass
-            elif token in [36]:
+            elif token in [54]:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 109
+                self.state = 129
                 self.match(ZorgQueryParser.PERCENT)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -766,15 +844,15 @@
 
     def note(self):
 
         localctx = ZorgQueryParser.NoteContext(self, self._ctx, self.state)
         self.enterRule(localctx, 18, self.RULE_note)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 112
+            self.state = 132
             self.match(ZorgQueryParser.T__4)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -808,15 +886,15 @@
 
     def where_body(self):
 
         localctx = ZorgQueryParser.Where_bodyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 20, self.RULE_where_body)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 114
+            self.state = 134
             self.or_filter()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -859,30 +937,30 @@
 
     def or_filter(self):
 
         localctx = ZorgQueryParser.Or_filterContext(self, self._ctx, self.state)
         self.enterRule(localctx, 22, self.RULE_or_filter)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 116
+            self.state = 136
             self.and_filter()
-            self.state = 123
+            self.state = 143
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,6,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 117
+                    self.state = 137
                     self.match(ZorgQueryParser.SPACE)
-                    self.state = 118
+                    self.state = 138
                     self.match(ZorgQueryParser.T__5)
-                    self.state = 119
+                    self.state = 139
                     self.match(ZorgQueryParser.SPACE)
-                    self.state = 120
+                    self.state = 140
                     self.and_filter() 
-                self.state = 125
+                self.state = 145
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,6,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -927,26 +1005,26 @@
 
     def and_filter(self):
 
         localctx = ZorgQueryParser.And_filterContext(self, self._ctx, self.state)
         self.enterRule(localctx, 24, self.RULE_and_filter)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 126
+            self.state = 146
             self.where_atom()
-            self.state = 131
+            self.state = 151
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,7,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 127
+                    self.state = 147
                     self.match(ZorgQueryParser.SPACE)
-                    self.state = 128
+                    self.state = 148
                     self.where_atom() 
-                self.state = 133
+                self.state = 153
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,7,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -974,14 +1052,30 @@
             return self.getTypedRuleContext(ZorgQueryParser.TagContext,0)
 
 
         def subfilter(self):
             return self.getTypedRuleContext(ZorgQueryParser.SubfilterContext,0)
 
 
+        def create_range(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Create_rangeContext,0)
+
+
+        def modify_range(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Modify_rangeContext,0)
+
+
+        def prop_filter(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Prop_filterContext,0)
+
+
+        def desc_filter(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Desc_filterContext,0)
+
+
         def getRuleIndex(self):
             return ZorgQueryParser.RULE_where_atom
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterWhere_atom" ):
                 listener.enterWhere_atom(self)
 
@@ -993,39 +1087,65 @@
 
 
     def where_atom(self):
 
         localctx = ZorgQueryParser.Where_atomContext(self, self._ctx, self.state)
         self.enterRule(localctx, 26, self.RULE_where_atom)
         try:
-            self.state = 138
+            self.state = 162
             self._errHandler.sync(self)
-            token = self._input.LA(1)
-            if token in [15, 16, 25, 39, 41, 42]:
+            la_ = self._interp.adaptivePredict(self._input,8,self._ctx)
+            if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 134
+                self.state = 154
                 self.note_type()
                 pass
-            elif token in [7]:
+
+            elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 135
+                self.state = 155
                 self.priority_range()
                 pass
-            elif token in [9, 33, 34, 35, 36]:
+
+            elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 136
+                self.state = 156
                 self.tag()
                 pass
-            elif token in [31]:
+
+            elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 137
+                self.state = 157
                 self.subfilter()
                 pass
-            else:
-                raise NoViableAltException(self)
+
+            elif la_ == 5:
+                self.enterOuterAlt(localctx, 5)
+                self.state = 158
+                self.create_range()
+                pass
+
+            elif la_ == 6:
+                self.enterOuterAlt(localctx, 6)
+                self.state = 159
+                self.modify_range()
+                pass
+
+            elif la_ == 7:
+                self.enterOuterAlt(localctx, 7)
+                self.state = 160
+                self.prop_filter()
+                pass
+
+            elif la_ == 8:
+                self.enterOuterAlt(localctx, 8)
+                self.state = 161
+                self.desc_filter()
+                pass
+
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1063,24 +1183,24 @@
     def note_type(self):
 
         localctx = ZorgQueryParser.Note_typeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 28, self.RULE_note_type)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 141 
+            self.state = 165 
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while True:
-                self.state = 140
+                self.state = 164
                 self.note_type_char()
-                self.state = 143 
+                self.state = 167 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 7146859233280) != 0)):
+                if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 1873515037574823936) != 0)):
                     break
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -1130,17 +1250,17 @@
     def note_type_char(self):
 
         localctx = ZorgQueryParser.Note_type_charContext(self, self._ctx, self.state)
         self.enterRule(localctx, 30, self.RULE_note_type_char)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 145
+            self.state = 169
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 7146859233280) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1873515037574823936) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -1153,19 +1273,19 @@
     class Priority_rangeContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def HASH(self):
-            return self.getToken(ZorgQueryParser.HASH, 0)
+        def PRIORITY(self):
+            return self.getToken(ZorgQueryParser.PRIORITY, 0)
 
-        def ID(self):
-            return self.getToken(ZorgQueryParser.ID, 0)
+        def DASH(self):
+            return self.getToken(ZorgQueryParser.DASH, 0)
 
         def getRuleIndex(self):
             return ZorgQueryParser.RULE_priority_range
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterPriority_range" ):
                 listener.enterPriority_range(self)
@@ -1177,24 +1297,34 @@
 
 
 
     def priority_range(self):
 
         localctx = ZorgQueryParser.Priority_rangeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 32, self.RULE_priority_range)
+        self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 147
-            self.match(ZorgQueryParser.T__6)
-            self.state = 148
-            self.match(ZorgQueryParser.HASH)
-            self.state = 149
-            self.match(ZorgQueryParser.ID)
-            self.state = 150
-            self.match(ZorgQueryParser.T__7)
+            self.state = 171
+            self.match(ZorgQueryParser.PRIORITY)
+            self.state = 174
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==44:
+                self.state = 172
+                self.match(ZorgQueryParser.DASH)
+                self.state = 173
+                _la = self._input.LA(1)
+                if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 65408) != 0)):
+                    self._errHandler.recoverInline(self)
+                else:
+                    self._errHandler.reportMatch(self)
+                    self.consume()
+
+
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -1244,39 +1374,39 @@
     def tag(self):
 
         localctx = ZorgQueryParser.TagContext(self, self._ctx, self.state)
         self.enterRule(localctx, 34, self.RULE_tag)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 153
+            self.state = 177
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==9:
-                self.state = 152
+            if _la==16:
+                self.state = 176
                 self.not_op()
 
 
-            self.state = 159
+            self.state = 183
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [33]:
-                self.state = 155
+            if token in [51]:
+                self.state = 179
                 self.area()
                 pass
-            elif token in [34]:
-                self.state = 156
+            elif token in [52]:
+                self.state = 180
                 self.context()
                 pass
-            elif token in [36]:
-                self.state = 157
+            elif token in [54]:
+                self.state = 181
                 self.person()
                 pass
-            elif token in [35]:
-                self.state = 158
+            elif token in [53]:
+                self.state = 182
                 self.project()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -1311,16 +1441,16 @@
 
     def not_op(self):
 
         localctx = ZorgQueryParser.Not_opContext(self, self._ctx, self.state)
         self.enterRule(localctx, 36, self.RULE_not_op)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 161
-            self.match(ZorgQueryParser.T__8)
+            self.state = 185
+            self.match(ZorgQueryParser.T__15)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -1355,17 +1485,17 @@
 
     def area(self):
 
         localctx = ZorgQueryParser.AreaContext(self, self._ctx, self.state)
         self.enterRule(localctx, 38, self.RULE_area)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 163
+            self.state = 187
             self.match(ZorgQueryParser.HASH)
-            self.state = 164
+            self.state = 188
             self.match(ZorgQueryParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1401,17 +1531,17 @@
 
     def context(self):
 
         localctx = ZorgQueryParser.ContextContext(self, self._ctx, self.state)
         self.enterRule(localctx, 40, self.RULE_context)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 166
+            self.state = 190
             self.match(ZorgQueryParser.AT_SIGN)
-            self.state = 167
+            self.state = 191
             self.match(ZorgQueryParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1447,17 +1577,17 @@
 
     def person(self):
 
         localctx = ZorgQueryParser.PersonContext(self, self._ctx, self.state)
         self.enterRule(localctx, 42, self.RULE_person)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 169
+            self.state = 193
             self.match(ZorgQueryParser.PERCENT)
-            self.state = 170
+            self.state = 194
             self.match(ZorgQueryParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1493,17 +1623,17 @@
 
     def project(self):
 
         localctx = ZorgQueryParser.ProjectContext(self, self._ctx, self.state)
         self.enterRule(localctx, 44, self.RULE_project)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 172
+            self.state = 196
             self.match(ZorgQueryParser.PLUS)
-            self.state = 173
+            self.state = 197
             self.match(ZorgQueryParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1543,29 +1673,644 @@
 
     def subfilter(self):
 
         localctx = ZorgQueryParser.SubfilterContext(self, self._ctx, self.state)
         self.enterRule(localctx, 46, self.RULE_subfilter)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 175
+            self.state = 199
             self.match(ZorgQueryParser.LPAREN)
-            self.state = 176
+            self.state = 200
             self.or_filter()
-            self.state = 177
+            self.state = 201
             self.match(ZorgQueryParser.RPAREN)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
+    class Create_rangeContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def CREATE_RANGE_HEAD(self):
+            return self.getToken(ZorgQueryParser.CREATE_RANGE_HEAD, 0)
+
+        def DATE_RANGE_TAIL(self):
+            return self.getToken(ZorgQueryParser.DATE_RANGE_TAIL, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_create_range
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterCreate_range" ):
+                listener.enterCreate_range(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitCreate_range" ):
+                listener.exitCreate_range(self)
+
+
+
+
+    def create_range(self):
+
+        localctx = ZorgQueryParser.Create_rangeContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 48, self.RULE_create_range)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 203
+            self.match(ZorgQueryParser.CREATE_RANGE_HEAD)
+            self.state = 205
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==33:
+                self.state = 204
+                self.match(ZorgQueryParser.DATE_RANGE_TAIL)
+
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class Modify_rangeContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def MODIFY_RANGE_HEAD(self):
+            return self.getToken(ZorgQueryParser.MODIFY_RANGE_HEAD, 0)
+
+        def DATE_RANGE_TAIL(self):
+            return self.getToken(ZorgQueryParser.DATE_RANGE_TAIL, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_modify_range
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterModify_range" ):
+                listener.enterModify_range(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitModify_range" ):
+                listener.exitModify_range(self)
+
+
+
+
+    def modify_range(self):
+
+        localctx = ZorgQueryParser.Modify_rangeContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 50, self.RULE_modify_range)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 207
+            self.match(ZorgQueryParser.MODIFY_RANGE_HEAD)
+            self.state = 209
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==33:
+                self.state = 208
+                self.match(ZorgQueryParser.DATE_RANGE_TAIL)
+
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class Prop_filterContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def ID(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgQueryParser.ID)
+            else:
+                return self.getToken(ZorgQueryParser.ID, i)
+
+        def COLON(self):
+            return self.getToken(ZorgQueryParser.COLON, 0)
+
+        def STAR(self):
+            return self.getToken(ZorgQueryParser.STAR, 0)
+
+        def not_op(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Not_opContext,0)
+
+
+        def prop_op(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Prop_opContext,0)
+
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_prop_filter
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterProp_filter" ):
+                listener.enterProp_filter(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitProp_filter" ):
+                listener.exitProp_filter(self)
+
+
+
+
+    def prop_filter(self):
+
+        localctx = ZorgQueryParser.Prop_filterContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 52, self.RULE_prop_filter)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 212
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==16:
+                self.state = 211
+                self.not_op()
+
+
+            self.state = 214
+            self.match(ZorgQueryParser.ID)
+            self.state = 215
+            self.match(ZorgQueryParser.COLON)
+            self.state = 217
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if (((_la) & ~0x3f) == 0 and ((1 << _la) & 1729382256911056896) != 0):
+                self.state = 216
+                self.prop_op()
+
+
+            self.state = 231
+            self._errHandler.sync(self)
+            token = self._input.LA(1)
+            if token in [7, 8, 9, 10, 11, 12, 13, 14, 15, 17, 35]:
+                self.state = 225
+                self._errHandler.sync(self)
+                token = self._input.LA(1)
+                if token in [35]:
+                    self.state = 219
+                    self.match(ZorgQueryParser.ID)
+                    pass
+                elif token in [7, 8, 9, 10, 11, 12, 13, 14, 15, 17]:
+                    self.state = 221 
+                    self._errHandler.sync(self)
+                    _la = self._input.LA(1)
+                    while True:
+                        self.state = 220
+                        _la = self._input.LA(1)
+                        if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 196480) != 0)):
+                            self._errHandler.recoverInline(self)
+                        else:
+                            self._errHandler.reportMatch(self)
+                            self.consume()
+                        self.state = 223 
+                        self._errHandler.sync(self)
+                        _la = self._input.LA(1)
+                        if not ((((_la) & ~0x3f) == 0 and ((1 << _la) & 196480) != 0)):
+                            break
+
+                    pass
+                else:
+                    raise NoViableAltException(self)
+
+                self.state = 228
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+                if _la==58:
+                    self.state = 227
+                    self.match(ZorgQueryParser.STAR)
+
+
+                pass
+            elif token in [58]:
+                self.state = 230
+                self.match(ZorgQueryParser.STAR)
+                pass
+            else:
+                raise NoViableAltException(self)
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class Prop_opContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def LANGLE(self):
+            return self.getToken(ZorgQueryParser.LANGLE, 0)
+
+        def RANGLE(self):
+            return self.getToken(ZorgQueryParser.RANGLE, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_prop_op
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterProp_op" ):
+                listener.enterProp_op(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitProp_op" ):
+                listener.exitProp_op(self)
+
+
+
+
+    def prop_op(self):
+
+        localctx = ZorgQueryParser.Prop_opContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 54, self.RULE_prop_op)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 233
+            _la = self._input.LA(1)
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1729382256911056896) != 0)):
+                self._errHandler.recoverInline(self)
+            else:
+                self._errHandler.reportMatch(self)
+                self.consume()
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class Desc_filterContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def SQUOTE(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgQueryParser.SQUOTE)
+            else:
+                return self.getToken(ZorgQueryParser.SQUOTE, i)
+
+        def id_(self, i:int=None):
+            if i is None:
+                return self.getTypedRuleContexts(ZorgQueryParser.IdContext)
+            else:
+                return self.getTypedRuleContext(ZorgQueryParser.IdContext,i)
+
+
+        def not_op(self):
+            return self.getTypedRuleContext(ZorgQueryParser.Not_opContext,0)
+
+
+        def SPACE(self, i:int=None):
+            if i is None:
+                return self.getTokens(ZorgQueryParser.SPACE)
+            else:
+                return self.getToken(ZorgQueryParser.SPACE, i)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_desc_filter
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterDesc_filter" ):
+                listener.enterDesc_filter(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitDesc_filter" ):
+                listener.exitDesc_filter(self)
+
+
+
+
+    def desc_filter(self):
+
+        localctx = ZorgQueryParser.Desc_filterContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 56, self.RULE_desc_filter)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 236
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==16:
+                self.state = 235
+                self.not_op()
+
+
+            self.state = 239
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            if _la==20:
+                self.state = 238
+                self.match(ZorgQueryParser.T__19)
+
+
+            self.state = 241
+            self.match(ZorgQueryParser.SQUOTE)
+            self.state = 242
+            self.id_()
+            self.state = 247
+            self._errHandler.sync(self)
+            _la = self._input.LA(1)
+            while _la==48:
+                self.state = 243
+                self.match(ZorgQueryParser.SPACE)
+                self.state = 244
+                self.id_()
+                self.state = 249
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+
+            self.state = 250
+            self.match(ZorgQueryParser.SQUOTE)
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class ZidContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def ZID(self):
+            return self.getToken(ZorgQueryParser.ZID, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_zid
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterZid" ):
+                listener.enterZid(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitZid" ):
+                listener.exitZid(self)
+
+
+
+
+    def zid(self):
+
+        localctx = ZorgQueryParser.ZidContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 58, self.RULE_zid)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 252
+            self.match(ZorgQueryParser.ZID)
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class IdContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def ID(self):
+            return self.getToken(ZorgQueryParser.ID, 0)
+
+        def NUM_ID(self):
+            return self.getToken(ZorgQueryParser.NUM_ID, 0)
+
+        def DATE_RANGE_TAIL(self):
+            return self.getToken(ZorgQueryParser.DATE_RANGE_TAIL, 0)
+
+        def PRIORITY(self):
+            return self.getToken(ZorgQueryParser.PRIORITY, 0)
+
+        def date(self):
+            return self.getTypedRuleContext(ZorgQueryParser.DateContext,0)
+
+
+        def time(self):
+            return self.getTypedRuleContext(ZorgQueryParser.TimeContext,0)
+
+
+        def zid(self):
+            return self.getTypedRuleContext(ZorgQueryParser.ZidContext,0)
+
+
+        def LOWER_O(self):
+            return self.getToken(ZorgQueryParser.LOWER_O, 0)
+
+        def LOWER_X(self):
+            return self.getToken(ZorgQueryParser.LOWER_X, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_id
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterId" ):
+                listener.enterId(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitId" ):
+                listener.exitId(self)
+
+
+
+
+    def id_(self):
+
+        localctx = ZorgQueryParser.IdContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 60, self.RULE_id)
+        try:
+            self.state = 263
+            self._errHandler.sync(self)
+            token = self._input.LA(1)
+            if token in [35]:
+                self.enterOuterAlt(localctx, 1)
+                self.state = 254
+                self.match(ZorgQueryParser.ID)
+                pass
+            elif token in [38]:
+                self.enterOuterAlt(localctx, 2)
+                self.state = 255
+                self.match(ZorgQueryParser.NUM_ID)
+                pass
+            elif token in [33]:
+                self.enterOuterAlt(localctx, 3)
+                self.state = 256
+                self.match(ZorgQueryParser.DATE_RANGE_TAIL)
+                pass
+            elif token in [34]:
+                self.enterOuterAlt(localctx, 4)
+                self.state = 257
+                self.match(ZorgQueryParser.PRIORITY)
+                pass
+            elif token in [29]:
+                self.enterOuterAlt(localctx, 5)
+                self.state = 258
+                self.date()
+                pass
+            elif token in [30]:
+                self.enterOuterAlt(localctx, 6)
+                self.state = 259
+                self.time()
+                pass
+            elif token in [36]:
+                self.enterOuterAlt(localctx, 7)
+                self.state = 260
+                self.zid()
+                pass
+            elif token in [27]:
+                self.enterOuterAlt(localctx, 8)
+                self.state = 261
+                self.match(ZorgQueryParser.LOWER_O)
+                pass
+            elif token in [28]:
+                self.enterOuterAlt(localctx, 9)
+                self.state = 262
+                self.match(ZorgQueryParser.LOWER_X)
+                pass
+            else:
+                raise NoViableAltException(self)
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class DateContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def DATE(self):
+            return self.getToken(ZorgQueryParser.DATE, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_date
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterDate" ):
+                listener.enterDate(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitDate" ):
+                listener.exitDate(self)
+
+
+
+
+    def date(self):
+
+        localctx = ZorgQueryParser.DateContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 62, self.RULE_date)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 265
+            self.match(ZorgQueryParser.DATE)
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class TimeContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def TIME(self):
+            return self.getToken(ZorgQueryParser.TIME, 0)
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_time
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterTime" ):
+                listener.enterTime(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitTime" ):
+                listener.exitTime(self)
+
+
+
+
+    def time(self):
+
+        localctx = ZorgQueryParser.TimeContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 64, self.RULE_time)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 267
+            self.match(ZorgQueryParser.TIME)
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
     class Group_by_bodyContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
@@ -1595,47 +2340,47 @@
 
 
 
 
     def group_by_body(self):
 
         localctx = ZorgQueryParser.Group_by_bodyContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 48, self.RULE_group_by_body)
+        self.enterRule(localctx, 66, self.RULE_group_by_body)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 179
+            self.state = 269
             self.group_by_atom()
-            self.state = 182
+            self.state = 272
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,12,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,25,self._ctx)
             if la_ == 1:
-                self.state = 180
+                self.state = 270
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 181
+                self.state = 271
                 self.group_by_atom()
 
 
-            self.state = 186
+            self.state = 276
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,13,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,26,self._ctx)
             if la_ == 1:
-                self.state = 184
+                self.state = 274
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 185
+                self.state = 275
                 self.group_by_atom()
 
 
-            self.state = 190
+            self.state = 280
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==30:
-                self.state = 188
+            if _la==48:
+                self.state = 278
                 self.match(ZorgQueryParser.SPACE)
-                self.state = 189
+                self.state = 279
                 self.group_by_atom()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1655,14 +2400,18 @@
             return self.getTypedRuleContext(ZorgQueryParser.FileContext,0)
 
 
         def type_(self):
             return self.getTypedRuleContext(ZorgQueryParser.TypeContext,0)
 
 
+        def priority(self):
+            return self.getTypedRuleContext(ZorgQueryParser.PriorityContext,0)
+
+
         def AT_SIGN(self):
             return self.getToken(ZorgQueryParser.AT_SIGN, 0)
 
         def HASH(self):
             return self.getToken(ZorgQueryParser.HASH, 0)
 
         def PERCENT(self):
@@ -1684,47 +2433,52 @@
 
 
 
 
     def group_by_atom(self):
 
         localctx = ZorgQueryParser.Group_by_atomContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 50, self.RULE_group_by_atom)
+        self.enterRule(localctx, 68, self.RULE_group_by_atom)
         try:
-            self.state = 198
+            self.state = 289
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [12]:
+            if token in [24]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 192
+                self.state = 282
                 self.file_()
                 pass
-            elif token in [13]:
+            elif token in [25]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 193
+                self.state = 283
                 self.type_()
                 pass
-            elif token in [34]:
+            elif token in [23]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 194
-                self.match(ZorgQueryParser.AT_SIGN)
+                self.state = 284
+                self.priority()
                 pass
-            elif token in [33]:
+            elif token in [52]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 195
-                self.match(ZorgQueryParser.HASH)
+                self.state = 285
+                self.match(ZorgQueryParser.AT_SIGN)
                 pass
-            elif token in [36]:
+            elif token in [51]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 196
-                self.match(ZorgQueryParser.PERCENT)
+                self.state = 286
+                self.match(ZorgQueryParser.HASH)
                 pass
-            elif token in [35]:
+            elif token in [54]:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 197
+                self.state = 287
+                self.match(ZorgQueryParser.PERCENT)
+                pass
+            elif token in [53]:
+                self.enterOuterAlt(localctx, 7)
+                self.state = 288
                 self.match(ZorgQueryParser.PLUS)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -1768,31 +2522,31 @@
 
 
 
 
     def order_by_body(self):
 
         localctx = ZorgQueryParser.Order_by_bodyContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 52, self.RULE_order_by_body)
+        self.enterRule(localctx, 70, self.RULE_order_by_body)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 200
+            self.state = 291
             self.order_by_atom()
-            self.state = 205
+            self.state = 296
             self._errHandler.sync(self)
-            _alt = self._interp.adaptivePredict(self._input,16,self._ctx)
+            _alt = self._interp.adaptivePredict(self._input,29,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 201
+                    self.state = 292
                     self.match(ZorgQueryParser.SPACE)
-                    self.state = 202
+                    self.state = 293
                     self.order_by_atom() 
-                self.state = 207
+                self.state = 298
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,16,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,29,self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -1802,16 +2556,20 @@
     class Order_by_atomContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def date(self):
-            return self.getTypedRuleContext(ZorgQueryParser.DateContext,0)
+        def create(self):
+            return self.getTypedRuleContext(ZorgQueryParser.CreateContext,0)
+
+
+        def modify(self):
+            return self.getTypedRuleContext(ZorgQueryParser.ModifyContext,0)
 
 
         def priority(self):
             return self.getTypedRuleContext(ZorgQueryParser.PriorityContext,0)
 
 
         def type_(self):
@@ -1831,76 +2589,120 @@
 
 
 
 
     def order_by_atom(self):
 
         localctx = ZorgQueryParser.Order_by_atomContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 54, self.RULE_order_by_atom)
+        self.enterRule(localctx, 72, self.RULE_order_by_atom)
         try:
-            self.state = 211
+            self.state = 303
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [10]:
+            if token in [21]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 208
-                self.date()
+                self.state = 299
+                self.create()
                 pass
-            elif token in [11]:
+            elif token in [22]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 209
-                self.priority()
+                self.state = 300
+                self.modify()
                 pass
-            elif token in [13]:
+            elif token in [23]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 210
+                self.state = 301
+                self.priority()
+                pass
+            elif token in [25]:
+                self.enterOuterAlt(localctx, 4)
+                self.state = 302
                 self.type_()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
 
-    class DateContext(ParserRuleContext):
+    class CreateContext(ParserRuleContext):
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
 
         def getRuleIndex(self):
-            return ZorgQueryParser.RULE_date
+            return ZorgQueryParser.RULE_create
 
         def enterRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "enterDate" ):
-                listener.enterDate(self)
+            if hasattr( listener, "enterCreate" ):
+                listener.enterCreate(self)
 
         def exitRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "exitDate" ):
-                listener.exitDate(self)
+            if hasattr( listener, "exitCreate" ):
+                listener.exitCreate(self)
 
 
 
 
-    def date(self):
+    def create(self):
 
-        localctx = ZorgQueryParser.DateContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 56, self.RULE_date)
+        localctx = ZorgQueryParser.CreateContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 74, self.RULE_create)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 305
+            self.match(ZorgQueryParser.T__20)
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class ModifyContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+
+        def getRuleIndex(self):
+            return ZorgQueryParser.RULE_modify
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterModify" ):
+                listener.enterModify(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitModify" ):
+                listener.exitModify(self)
+
+
+
+
+    def modify(self):
+
+        localctx = ZorgQueryParser.ModifyContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 76, self.RULE_modify)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 213
-            self.match(ZorgQueryParser.T__9)
+            self.state = 307
+            self.match(ZorgQueryParser.T__21)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -1927,19 +2729,19 @@
 
 
 
 
     def priority(self):
 
         localctx = ZorgQueryParser.PriorityContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 58, self.RULE_priority)
+        self.enterRule(localctx, 78, self.RULE_priority)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 215
-            self.match(ZorgQueryParser.T__10)
+            self.state = 309
+            self.match(ZorgQueryParser.T__22)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -1966,19 +2768,19 @@
 
 
 
 
     def file_(self):
 
         localctx = ZorgQueryParser.FileContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 60, self.RULE_file)
+        self.enterRule(localctx, 80, self.RULE_file)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 217
-            self.match(ZorgQueryParser.T__11)
+            self.state = 311
+            self.match(ZorgQueryParser.T__23)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -2005,19 +2807,19 @@
 
 
 
 
     def type_(self):
 
         localctx = ZorgQueryParser.TypeContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 62, self.RULE_type)
+        self.enterRule(localctx, 82, self.RULE_type)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 219
-            self.match(ZorgQueryParser.T__12)
+            self.state = 313
+            self.match(ZorgQueryParser.T__24)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
```

### Comparing `zettel_org-0.7.2/src/zorg/service/common.py` & `zettel_org-0.7.3/src/zorg/service/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Helper logic that is shared broadly across this package."""
 
 import datetime as dt
 from pathlib import Path
 import re
+import sys
 from typing import Any, Iterable
 
 import rich
 from typist import PathLike
 
 from ..domain.types import Color, VarMapType
 
@@ -32,14 +33,19 @@
         path = Path(p)
         new_paths.append(
             path if zdir_path in path.parents else zdir_path / path
         )
     return new_paths
 
 
+def strip_zdir(zdir: PathLike, path: PathLike) -> str:
+    """Strips {zdir} from {path}."""
+    return str(path).replace(f"{zdir}/", "")
+
+
 def zprint(
     *msg_parts: str,
     style: str = "bold",
     bg_color: Color = Color.WHITE,
     fg_color: Color = Color.BLACK,
 ) -> None:
     """Custom rich.print() wrapper used by Zorg."""
@@ -60,16 +66,17 @@
     contents = f"{space_call_count} | {hhmmss} | {msg}"
     rich.print(f"[{style} {fg} on {bg}]{contents}[/]")
 
     # set call count
     setattr(zprint, call_count_attr, call_count + 1)
 
 
-def strip_zdir(zdir: PathLike, path: PathLike) -> str:
-    """Strips {zdir} from {path}."""
-    return str(path).replace(f"{zdir}/", "")
+def zinput(prompt: str) -> str:
+    """Custom input() wrapper used by Zorg."""
+    print(prompt, file=sys.stderr, end="")
+    return input()
 
 
 def _var_map_value(value: str) -> Any:
     if re.match("^[0-9]{4}[01][0-9][0-3][0-9]$", value):
         return dt.datetime.strptime(value, "%Y%m%d")
     return value
```

### Comparing `zettel_org-0.7.2/src/zorg/service/compiler/_api.py` & `zettel_org-0.7.3/src/zorg/service/compiler/_api.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/src/zorg/service/compiler/_file_compiler.py` & `zettel_org-0.7.3/src/zorg/service/compiler/_file_compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Literal, Optional
 
 import antlr4
 from antlr4.error.ErrorListener import ErrorListener
 from logrus import Logger
 from typist import assert_never
 
+from .. import dates as zdt
 from ...domain.models import File, Note, TodoPayload
 from ...domain.types import NoteType, TodoPriorityType, TodoStatusPrefixChar
 from ...grammar.zorg_file.ZorgFileListener import ZorgFileListener
 from ...grammar.zorg_file.ZorgFileParser import ZorgFileParser
 
 
 TagName = Literal["areas", "contexts", "people", "projects"]
@@ -65,33 +66,33 @@
 
     def enterContext(
         self, ctx: ZorgFileParser.ContextContext
     ) -> None:  # noqa: D102
         self._add_tags(ctx, "contexts")
 
     def enterDate(self, ctx: ZorgFileParser.DateContext) -> None:  # noqa: D102
-        get_date = partial(
+        get_datetime = partial(
             dt.datetime.strptime, ctx.DATE().getText(), "%Y-%m-%d"
         )
         if (
             self._s.in_note
             and self._s.ids_in_note == 1
             and self._s.note_date is None
         ):
-            self._s.note_date = get_date()
+            self._s.note_date = get_datetime().date()
         elif self._s.in_h4_header:
-            self._s.h4_date = get_date()
+            self._s.h4_date = get_datetime().date()
         elif self._s.in_h3_header:
-            self._s.h3_date = get_date()
+            self._s.h3_date = get_datetime().date()
         elif self._s.in_h2_header:
-            self._s.h2_date = get_date()
+            self._s.h2_date = get_datetime().date()
         elif self._s.in_h1_header:
-            self._s.h1_date = get_date()
+            self._s.h1_date = get_datetime().date()
         elif self._s.in_first_comment:
-            self._s.file_date = get_date()
+            self._s.file_date = get_datetime().date()
 
     def enterH1_header(
         self, ctx: ZorgFileParser.H1_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h1_header = True
 
@@ -114,45 +115,53 @@
         self._s.in_h4_header = True
 
     def enterHead(self, ctx: ZorgFileParser.HeadContext) -> None:  # noqa: D102
         del ctx
         self._s.in_head = True
 
     def enterId(self, ctx: ZorgFileParser.IdContext) -> None:  # noqa: D102
-        del ctx
         if self._s.in_note:
             self._s.ids_in_note += 1
+            if self._s.ids_in_note == 1 and zdt.is_short_date(
+                short_date := ctx.getText()
+            ):
+                self._s.modify_date = zdt.from_short_date(short_date)
+            elif (
+                self._s.ids_in_note == 1
+                or (self._s.ids_in_note == 2 and self._s.modify_date)
+            ) and zdt.is_zid(zid := ctx.getText()):
+                self._s.zid = zid
+                zorg_id_date = f"20{zid.split('#')[0]}"
+                self._s.note_date = dt.datetime.strptime(
+                    zorg_id_date, "%Y%m%d"
+                ).date()
 
     def enterItem(self, ctx: ZorgFileParser.ItemContext) -> None:  # noqa: D102
         del ctx
         self._reset_note_context()
 
     def enterLink(self, ctx: ZorgFileParser.LinkContext) -> None:  # noqa: D102
         if self._s.in_note:
             link_text = ctx.children[1].getText()
             self._s.note_links.append(link_text)
 
-    def enterNote(self, ctx: ZorgFileParser.NoteContext) -> None:  # noqa: D102
-        del ctx
-        self._s.parent_id = None
-
     def enterPerson(
         self, ctx: ZorgFileParser.PersonContext
     ) -> None:  # noqa: D102
         self._add_tags(ctx, "people")
 
     def enterProject(
         self, ctx: ZorgFileParser.ProjectContext
     ) -> None:  # noqa: D102
         self._add_tags(ctx, "projects")
 
     def enterPriority(
         self, ctx: ZorgFileParser.PriorityContext
     ) -> None:  # noqa: D102
-        self._s.todo_priority = ctx.ID().getText()[0].upper()
+        self._s.todo_priority = ctx.getText().upper()
 
     def enterProperty(
         self, ctx: ZorgFileParser.PropertyContext
     ) -> None:  # noqa: D102
         key, value = ctx.ID().getText(), ctx.id_group().getText()
         if self._s.in_head:
             self._s.file_props[key] = value
@@ -163,35 +172,16 @@
         elif self._s.in_h3_header:
             self._s.h3_props[key] = value
         elif self._s.in_h4_header:
             self._s.h4_props[key] = value
         elif self._s.in_note:
             self._s.note_props[key] = value
 
-    def enterSubnote(
-        self, ctx: ZorgFileParser.SubnoteContext
-    ) -> None:  # noqa: D102
-        del ctx
-        if not self._s.in_subnote:
-            self._s.parent_id = self._s.next_id - 1
-        self._s.in_subnote = True
-        self._reset_note_context()
-
-    def enterSubsubnote(
-        self, ctx: ZorgFileParser.SubsubnoteContext
-    ) -> None:  # noqa: D102
-        del ctx
-        if not self._s.in_subsubnote:
-            self._s.parent_id = self._s.next_id - 1
-        self._s.in_subsubnote = True
-        self._reset_note_context()
-
     def enterTodo(self, ctx: ZorgFileParser.TodoContext) -> None:  # noqa: D102
         self._s.in_note = True
-        self._s.parent_id = None
         del ctx
 
     def enterTodo_prefix(
         self, ctx: ZorgFileParser.Todo_prefixContext
     ) -> None:  # noqa: D102
         status = NoteType.OPEN_TODO
         if self._s.in_note:
@@ -207,21 +197,14 @@
             elif ch == ">":
                 status = NoteType.PARENT_TODO
             else:
                 assert_never(ch)
 
             self._s.todo_status = status
 
-    def enterZid(self, ctx: ZorgFileParser.ZidContext) -> None:  # noqa: D102
-        if self._s.in_note and self._s.ids_in_note == 0:
-            zid = ctx.getText()
-            self._s.zid = zid
-            zorg_id_date = f"20{zid.split('#')[0]}"
-            self._s.note_date = dt.datetime.strptime(zorg_id_date, "%Y%m%d")
-
     def exitBase_todo(
         self, ctx: ZorgFileParser.Base_todoContext
     ) -> None:  # noqa: D102
         self._s.in_note = False
         kwargs = self._get_note_kwargs(
             ctx,
             {
@@ -242,15 +225,15 @@
             )
             self.zorg_file.has_errors = True
         else:
             todo = Note(id_note_body.getText(), **kwargs)
             self.zorg_file.notes.append(todo)
 
         # Reset todo priority and status back to defaults.
-        self._s.todo_priority = "C"
+        self._s.todo_priority = "P2"
         self._s.todo_status = NoteType.OPEN_TODO
 
     def exitH1_header(
         self, ctx: ZorgFileParser.H1_headerContext
     ) -> None:  # noqa: D102
         del ctx
         self._s.in_h1_header = False
@@ -315,17 +298,15 @@
         del ctx
         self._s.in_first_comment = False
 
     def exitBase_note(
         self, ctx: ZorgFileParser.Base_noteContext
     ) -> None:  # noqa: D102
         self._s.in_note = False
-        extra_kwargs = {}
-        if self._s.parent_id is not None:
-            extra_kwargs["parent_note_id"] = self._s.parent_id
+        extra_kwargs: dict[str, Any] = {}
         kwargs = self._get_note_kwargs(ctx, extra_kwargs)
         body: str = ctx.id_note_body().getText().strip()
         if body == "":
             _LOGGER.warning(
                 "Skipping note with empty body",
                 file_path=str(self.zorg_file.path),
             )
@@ -338,43 +319,33 @@
             )
             self.zorg_file.has_errors = True
             return
 
         note = Note(body, **kwargs)
         self.zorg_file.notes.append(note)
 
-    def exitItem(self, ctx: ZorgFileParser.ItemContext) -> None:  # noqa: D102
-        del ctx
-        self._s.in_subnote = False
-
-    def exitSubnote(
-        self, ctx: ZorgFileParser.SubnoteContext
-    ) -> None:  # noqa: D102
-        self._s.in_subsubnote = False
-        del ctx
-
-    def exitSubsubnote(
-        self, ctx: ZorgFileParser.SubsubnoteContext
-    ) -> None:  # noqa: D102
-        del ctx
-
     def _get_note_kwargs(
         self,
         ctx: antlr4.ParserRuleContext,
         extra_kwargs: dict[str, Any] = None,
     ) -> dict[str, Any]:
         if extra_kwargs is None:
             extra_kwargs = {}
         kwargs: dict[str, Any] = {
             "areas": self._s.areas,
             "contexts": self._s.contexts,
             "create_date": self._s.create_date,
             "file_path": self.zorg_file.path,
             "line_no": ctx.start.line,
             "links": self._s.note_links,
+            "modify_date": (
+                self._s.modify_date
+                if self._s.modify_date
+                else self._s.create_date
+            ),
             "people": self._s.people,
             "projects": self._s.projects,
             "properties": self._s.properties,
             "zid": self._s.zid,
         }
         self._s.next_id += 1
         return kwargs | extra_kwargs
@@ -382,14 +353,15 @@
     def _reset_note_context(self) -> None:
         self._s.zid = None
         self._s.ids_in_note = 0
         self._s.note_tags = _get_default_tags_map()
         self._s.note_props = {}
         self._s.note_links = []
         self._s.note_date = None
+        self._s.modify_date = None
 
     def _add_tags(
         self, ctx: antlr4.ParserRuleContext, tag_name: TagName
     ) -> None:
         text = ctx.children[1].getText()
         if all(ch.isdigit() for ch in text):
             _LOGGER.debug(
@@ -422,25 +394,22 @@
 
     zid: Optional[str] = None
 
     ids_in_note: int = 0
 
     # TODO(bugyi): Figure out a better way to track parent/child relationship
     next_id: int = 1
-    parent_id: Optional[int] = None
 
     in_first_comment: bool = True
     in_head: bool = False
     in_h1_header: bool = False
     in_h2_header: bool = False
     in_h3_header: bool = False
     in_h4_header: bool = False
     in_note: bool = False
-    in_subnote: bool = False
-    in_subsubnote: bool = False
 
     file_tags: dict[TagName, list[str]] = field(
         default_factory=_get_default_tags_map
     )
     h1_tags: dict[TagName, list[str]] = field(
         default_factory=_get_default_tags_map
     )
@@ -468,16 +437,17 @@
 
     file_date: Optional[dt.date] = None
     h1_date: Optional[dt.date] = None
     h2_date: Optional[dt.date] = None
     h3_date: Optional[dt.date] = None
     h4_date: Optional[dt.date] = None
     note_date: Optional[dt.date] = None
+    modify_date: Optional[dt.date] = None
 
-    todo_priority: TodoPriorityType = "C"
+    todo_priority: TodoPriorityType = "P2"
     todo_status: NoteType = NoteType.OPEN_TODO
 
     @property
     def areas(self) -> list[str]:
         """Area tags that are currently in-scope."""
         return self._get_current_tags("areas")
```

### Comparing `zettel_org-0.7.2/src/zorg/service/file_groups.py` & `zettel_org-0.7.3/src/zorg/service/file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/src/zorg/service/handlers.py` & `zettel_org-0.7.3/src/zorg/service/handlers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 """Zorg's event and command handlers live here."""
 
+import datetime as dt
 from functools import partial
 import hashlib
 import json
+from operator import attrgetter
 from pathlib import Path
 import sys
-from typing import Iterable, Iterator
+from typing import Callable, Iterable, Iterator, Optional, Sequence
 
 from logrus import Logger
 from tqdm import tqdm
 import vimala
 
-from . import common as c
+from . import common as c, dates as zdt
 from .. import APP_NAME
 from ..domain.messages import commands, events
+from ..domain.models import File, Note
 from ..domain.types import Color
 from ..storage.sql.session import SQLSession
 from .compiler import walk_zorg_file
 from .zid_manager import ZIDManager
 
 
 _LOGGER = Logger(__name__)
 
+_ThingFirstLineAdder = Callable[[str, str], str]
+_ThingGetter = Callable[[Note], str]
+
 
 def edit_files(cmd: commands.EditCommand, session: SQLSession) -> None:
     """Command handler for the EditCommand."""
     vimala.vim(
         *cmd.paths,
         commands=_process_vim_commands(cmd.zettel_dir, cmd.vim_commands),
     ).unwrap()
@@ -36,53 +42,53 @@
     event: events.EditorClosedEvent, session: SQLSession
 ) -> None:
     """Check if the 'keep alive' file exists and, if so, reopens the editor."""
     keep_alive_file = event.edit_cmd.keep_alive_file
     if not keep_alive_file.exists():
         _LOGGER.debug(
             "No keep alive file found.",
-            keep_alive_file=keep_alive_file,
+            keep_alive_file=str(keep_alive_file),
         )
         return
 
     zdir = event.edit_cmd.zettel_dir
     prepend_zdir = partial(c.prepend_zdir, zdir)
     vim_commands = list(event.edit_cmd.vim_commands)
     if keep_alive_file.stat().st_size == 0:
         _LOGGER.debug(
             "Empty keep alive file found.",
-            keep_alive_file=keep_alive_file,
+            keep_alive_file=str(keep_alive_file),
         )
         paths = event.edit_cmd.paths
     else:
         keep_alive_lines = list(keep_alive_file.read_text().split())
         focused_filename = keep_alive_lines.pop()
         vim_commands = [
             cmd for cmd in vim_commands if not cmd.startswith("edit ")
         ]
         vim_commands.append(f"edit {focused_filename}")
         new_paths = prepend_zdir([Path(p.strip()) for p in keep_alive_lines])
         _LOGGER.debug(
             "Editing files specified in the keep alive file.",
-            keep_alive_file=keep_alive_file,
-            old_paths=event.edit_cmd.paths,
-            new_paths=new_paths,
+            keep_alive_file=str(keep_alive_file),
+            old_paths=[str(p) for p in event.edit_cmd.paths],
+            new_paths=[str(p) for p in new_paths],
         )
         paths = new_paths
 
     verbose = event.edit_cmd.verbose
     if verbose <= 1:
         _LOGGER.debug(
-            "Unlinking keep-alive file", keep_alive_file=keep_alive_file
+            "Unlinking keep-alive file", keep_alive_file=str(keep_alive_file)
         )
         keep_alive_file.unlink()
     else:
         _LOGGER.debug(
             "We are NOT deleting the keep-alive file",
-            keep_alive_file=keep_alive_file,
+            keep_alive_file=str(keep_alive_file),
         )
     session.add_last_message(
         commands.EditCommand(
             zettel_dir=zdir,
             paths=paths,
             keep_alive_file=keep_alive_file,
             verbose=verbose,
@@ -95,19 +101,19 @@
     cmd: commands.CreateDBCommand, session: SQLSession
 ) -> None:
     """Create a new zorg DB from scratch."""
     zorg_files = []
     total_num_notes = 0
     total_num_todos = 0
     for zo_path in tqdm(
-        sorted(cmd.zettel_dir.rglob("*.zo"), key=lambda p: p.name),
+        _get_zo_paths_to_index(cmd.zettel_dir),
         desc="Reading notes from zorg files",
         file=sys.stdout,
     ):
-        _LOGGER.info("Starting to walk zorg file", zorg_file=zo_path.name)
+        _LOGGER.info("Starting to walk zorg file", zorg_file=str(zo_path))
         zorg_file = walk_zorg_file(cmd.zettel_dir, zo_path)
         num_notes = len(zorg_file.notes)
         num_todos = len(
             [note for note in zorg_file.notes if note.todo_payload]
         )
         total_num_notes += num_notes
         total_num_todos += num_todos
@@ -131,52 +137,55 @@
     session.add_message(events.DBModifiedEvent(cmd.zettel_dir))
 
 
 def reindex_database(
     cmd: commands.ReindexDBCommand, session: SQLSession
 ) -> None:
     """Reindex an existing zorg database."""
-    paths = cmd.paths if cmd.paths else sorted(cmd.zettel_dir.rglob("*.zo"))
-    file_to_hash = _get_file_hash_map(cmd.zettel_dir, paths)
+    file_to_hash = _get_file_hash_map(
+        cmd.zettel_dir, paths=cmd.paths if cmd.paths else None
+    )
     file_hash_path = _get_file_hash_path(cmd.zettel_dir)
     old_file_to_hash: dict[str, str] = (
         json.loads(file_hash_path.read_bytes())
         if file_hash_path.exists()
         else {}
     )
 
     num_of_updates = 0
-    for file, hash_ in file_to_hash.copy().items():
+    for zorg_file_name, hash_ in file_to_hash.copy().items():
+        # If this file has never been indexed OR the file contents have changed
+        # since the last time it was indexed.
         if (
-            file not in old_file_to_hash.keys()
-            or old_file_to_hash[file] != hash_
+            zorg_file_name not in old_file_to_hash.keys()
+            or old_file_to_hash[zorg_file_name] != hash_
         ):
             num_of_updates += 1
-            old_zorg_file = session.repo.get(file).unwrap()
+            old_zorg_file = session.repo.remove_by_key(zorg_file_name).unwrap()
             if old_zorg_file is not None:
-                _LOGGER.debug("Removing file from DB", file=file)
+                _LOGGER.debug("Removing file from DB", file=zorg_file_name)
                 c.zprint(
                     "UPDATING EXISTING FILE",
-                    file,
+                    zorg_file_name,
                     fg_color=Color.BLACK,
                     bg_color=Color.YELLOW,
                 )
-                session.repo.remove_by_key(str(old_zorg_file.path))
             else:
                 c.zprint(
                     "ADDING NEW FILE",
-                    file,
+                    zorg_file_name,
                     fg_color=Color.WHITE,
                     bg_color=Color.GREEN,
                 )
 
             zorg_file = walk_zorg_file(
-                cmd.zettel_dir, Path(file), verbose=cmd.verbose
+                cmd.zettel_dir, Path(zorg_file_name), verbose=cmd.verbose
             )
-            _LOGGER.debug("Adding zorg file", file=file)
+            _check_for_modified_notes(cmd.zettel_dir, zorg_file, old_zorg_file)
+            _LOGGER.debug("Adding zorg file", file=zorg_file_name)
             session.repo.add(zorg_file)
             session.commit()
 
     if num_of_updates == 0:
         c.zprint("NO ZORG FILES HAVE BEEN MODIFIED")
 
     _write_file_hash_to_disk(file_hash_path, file_to_hash)
@@ -192,40 +201,24 @@
         commands.ReindexDBCommand(event.edit_cmd.zettel_dir, paths=[])
     )
 
 
 def add_zids_to_notes_in_file(
     event: events.NewZorgNotesEvent, session: SQLSession
 ) -> None:
-    """Adds IDs to new zorg notes."""
+    """Adds ZIDs to new zorg notes."""
     del session
 
-    zlines = event.zorg_file_path.read_text().split("\n")
-    for note in event.new_notes:
-        assert note.zid is not None
-        assert note.line_no is not None
-
-        start_idx = note.line_no - 1
-        end_idx = note.line_no + len(note.body.split("\n")) - 1
-        new_note_lines = zlines[start_idx:end_idx]
-        first_note_line = new_note_lines[0]
-        new_note_lines[0] = _add_zid_to_line(note.zid, first_note_line)
-        zlines = zlines[:start_idx] + new_note_lines + zlines[end_idx:]
-
-    _LOGGER.info(
-        "Adding ZIDs to zorg file",
-        zorg_file=event.zorg_file_path,
-        new_notes=len(event.new_notes),
-    )
-    event.zorg_file_path.write_text("\n".join(zlines))
-
-    zdir = event.zettel_dir
-    _write_file_hash_to_disk(
-        _get_file_hash_path(zdir),
-        _get_file_hash_map(zdir, Path(zdir).rglob("*.zo")),
+    _update_zo_file(
+        zdir=event.zettel_dir,
+        zo_path=event.zorg_file_path,
+        notes_to_update=event.new_notes,
+        add_thing_to_first_line=_add_zid_to_line,
+        thing_getter=attrgetter("zid"),
+        log_message="Adding ZIDs to zorg file",
     )
 
 
 def increment_zid_counters(
     event: events.DBModifiedEvent, session: SQLSession
 ) -> None:
     """Increment the date-specific zorg ID counters.
@@ -234,15 +227,39 @@
     generating new IDs (they are the XX in the YYMMDD#XX ID format).
     """
     del session
     zid_manager = ZIDManager(event.zettel_dir)
     zid_manager.write_to_disk()
 
 
-def _get_file_hash_map(zdir: Path, paths: Iterable[Path]) -> dict[str, str]:
+def update_note_modify_dates(
+    event: events.ModifiedZorgNotesEvent, session: SQLSession
+) -> None:
+    """Creates or updates note modify dates."""
+    del session
+    today_short_date = zdt.to_short_date(dt.date.today())
+    _update_zo_file(
+        zdir=event.zettel_dir,
+        zo_path=event.zorg_file_path,
+        notes_to_update=event.modified_notes,
+        add_thing_to_first_line=_add_or_update_modify_date,
+        thing_getter=lambda _: today_short_date,
+        log_message="Updating modify dates",
+    )
+
+
+def _get_zo_paths_to_index(zdir: Path) -> list[Path]:
+    return sorted(zdir.rglob("*.zo"), key=lambda p: p.name)
+
+
+def _get_file_hash_map(
+    zdir: Path, *, paths: Iterable[Path] = None
+) -> dict[str, str]:
+    if paths is None:
+        paths = _get_zo_paths_to_index(zdir)
     file_to_hash: dict[str, str] = {}
     for path in paths:
         key = c.strip_zdir(zdir, path)
         file_to_hash[key] = _hash_file(path)
     return file_to_hash
 
 
@@ -257,38 +274,28 @@
 ) -> None:
     _LOGGER.debug("Writing hash map to disk", file=str(file_hash_path))
     with file_hash_path.open("w") as f:
         json.dump(dict(sorted(file_to_hash.items())), f, indent=4)
 
 
 def _add_zid_to_line(zid: str, line: str) -> str:
-    all_words = line.split(" ")
-
-    num_spaces = 0
-    while all_words[0] == "":
-        num_spaces += 1
-        all_words.pop(0)
-    spaces = " " * num_spaces
-
-    symbol = all_words[0]
-    words = all_words[1:]
-
-    priority = ""
-    if words[0].startswith("[#"):
-        priority = f"{words.pop(0)} "
+    words = line.split(" ")
+    line_before_zid = _pop_line_before_zid(words)
 
+    # Remove a YYYY-MM-DD create date if one existed prior to adding a ZID to
+    # the note.
     if len(words[0]) == 10:
         dash_idices = (4, 7)
         for i, ch in enumerate(words[0][:10]):
             if i not in dash_idices and not ch.isdigit():
                 break
         else:
             words.pop(0)
 
-    return f"{spaces}{symbol} {priority}{zid} {' '.join(words)}"
+    return f"{line_before_zid}{zid} {' '.join(words)}"
 
 
 def _hash_file(filepath: Path, chunk_size: int = 8192) -> str:
     """Hashes a file using SHA256 algorithm and returns the hash value.
 
     Args:
         filepath: Path to the file to be hashed.
@@ -308,7 +315,87 @@
     zettel_dir: Path, vim_commands: Iterable[str]
 ) -> Iterator[str]:
     for vim_cmd in vim_commands:
         if "{zdir}" in vim_cmd:
             yield vim_cmd.format(zdir=zettel_dir)
         else:
             yield vim_cmd
+
+
+def _check_for_modified_notes(
+    zdir: Path, zorg_file: File, old_zorg_file: Optional[File]
+) -> None:
+    today = dt.date.today()
+    modified_notes: list[Note] = []
+    notes = old_zorg_file.notes if old_zorg_file else []
+    old_zid_map = {note.zid: note for note in notes if note.zid is not None}
+    for note in zorg_file.notes:
+        old_note = old_zid_map.get(note.zid, None) if note.zid else None
+        note_has_changed = old_note and note != old_note
+        note_is_new = old_note is None and note.zid is not None
+        if note.modify_date != today and (note_has_changed or note_is_new):
+            modified_notes.append(note)
+    if modified_notes:
+        zorg_file.events.append(
+            events.ModifiedZorgNotesEvent(zdir, zorg_file.path, modified_notes)
+        )
+
+
+def _add_or_update_modify_date(short_modify_date: str, line: str) -> str:
+    words = line.split(" ")
+    line_before_zid = _pop_line_before_zid(words)
+    if words and len(words[0]) == 6 and all(ch.isdigit() for ch in words[0]):
+        old_modify_date = words.pop(0)
+        _LOGGER.debug(
+            "Removing old modify date", old_modify_date=old_modify_date
+        )
+    return f"{line_before_zid}{short_modify_date} {' '.join(words)}"
+
+
+def _pop_line_before_zid(words: list[str]) -> str:
+    num_spaces = 0
+    while words[0] == "":
+        num_spaces += 1
+        words.pop(0)
+    spaces = " " * num_spaces
+
+    symbol = words.pop(0)
+
+    priority = ""
+    if len(words[0]) == 2 and words[0][0] == "P" and words[0][1].isdigit():
+        priority = f"{words.pop(0)} "
+    return f"{spaces}{symbol} {priority}"
+
+
+def _update_zo_file(
+    *,
+    zdir: Path,
+    zo_path: Path,
+    notes_to_update: Sequence[Note],
+    add_thing_to_first_line: _ThingFirstLineAdder,
+    thing_getter: _ThingGetter,
+    log_message: str,
+) -> None:
+    zlines = zo_path.read_text().split("\n")
+    for note in notes_to_update:
+        assert note.zid is not None
+        assert note.line_no is not None
+
+        start_idx = note.line_no - 1
+        end_idx = note.line_no + len(note.body.split("\n")) - 1
+        new_note_lines = zlines[start_idx:end_idx]
+        first_note_line = new_note_lines[0]
+        new_note_lines[0] = add_thing_to_first_line(
+            thing_getter(note), first_note_line
+        )
+        zlines = zlines[:start_idx] + new_note_lines + zlines[end_idx:]
+
+    _LOGGER.info(
+        log_message,
+        zorg_file=str(zo_path),
+        notes_to_update=len(notes_to_update),
+    )
+    zo_path.write_text("\n".join(zlines))
+
+    _write_file_hash_to_disk(
+        _get_file_hash_path(zdir), _get_file_hash_map(zdir)
+    )
```

### Comparing `zettel_org-0.7.2/src/zorg/service/messagebus.py` & `zettel_org-0.7.3/src/zorg/service/messagebus.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     commands.ReindexDBCommand: handlers.reindex_database,
 }
 EVENT_HANDLERS: dict[type[events.Event], list[MessageHandler]] = {
     events.EditorClosedEvent: [
         handlers.check_keep_alive_file,
         handlers.reindex_database_after_edit,
     ],
+    events.ModifiedZorgNotesEvent: [handlers.update_note_modify_dates],
     events.NewZorgNotesEvent: [handlers.add_zids_to_notes_in_file],
     events.DBModifiedEvent: [handlers.increment_zid_counters],
 }
 
 
 def handle(messages: Sequence[Message], session: SQLSession) -> None:
     """Entry point into Zorg's event messagebus loop."""
```

### Comparing `zettel_org-0.7.2/src/zorg/service/swog/_executor.py` & `zettel_org-0.7.3/src/zorg/service/swog/_executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,26 +4,33 @@
 import itertools as it
 import time
 from typing import Iterable, Sequence, Union
 
 from logrus import Logger
 
 from ...domain.models import Note
-from ...domain.types import GroupByType, NoteType, SelectType
+from ...domain.types import (
+    GroupByType,
+    KeyFunc,
+    NoteType,
+    OrderByType,
+    SelectType,
+)
 from ...storage.sql.session import SQLSession
 from ..compiler import build_zorg_query
 
 
 _LOGGER = Logger(__name__)
 
 
 GroupNoteMap = dict[str, "NoteGroup"]
 NoteGroup = Union[list[Note], GroupNoteMap]
 
 
+# TODO(bugyi): Reduce package to single swog.py file
 def execute(session: SQLSession, query_string: str) -> str:
     """Execute a zorg query and then render it as a .zo file.
 
     In other words, a Zorg query goes in and a Zorg file comes out.
 
     Arguments:
     ----------
@@ -52,23 +59,43 @@
         seconds=f"{query_runtime:.3f}",
     )
 
     ### (G)ROUP BY
     note_group = _group_notes_by(filtered_notes, query.group_by)
 
     ### (O)RDER BY
-
-    # TODO(bugyi): Implement ORDER BY query functionality.
+    ordered_note_group = _order_notes_by(note_group, query.order_by)
 
     ### (S)ELECT
-    result = _select(query.select, note_group)
+    result = _select(query.select, ordered_note_group)
 
     return result.strip()
 
 
+def _order_notes_by(
+    note_group: NoteGroup, order_bys: Iterable[OrderByType]
+) -> NoteGroup:
+    keyfunc = _order_by_keyfunc(order_bys)
+    if isinstance(note_group, list):
+        return sorted(note_group, key=keyfunc)
+
+    assert isinstance(note_group, dict)
+    new_note_group = {}
+    for k, v in note_group.items():
+        new_note_group[k] = _order_notes_by(v, order_bys)
+    return new_note_group
+
+
+def _order_by_keyfunc(order_bys: Iterable[OrderByType]) -> KeyFunc:
+    def keyfunc(note: Note) -> str:
+        return " ".join(oby.keyfunc(note) for oby in order_bys)
+
+    return keyfunc
+
+
 def _select(
     select_type: SelectType, note_group: NoteGroup, *, level: int = 1
 ) -> str:
     result = ""
     if select_type is SelectType.NOTE:
         if isinstance(note_group, list):
             result += _select_note(note_group) + "\n"
@@ -89,23 +116,23 @@
     result = ""
     for note in filtered_notes:
         note_type = (
             note.todo_payload.status if note.todo_payload else NoteType.BASIC
         )
         char = note_type.to_prefix_char()
         priority = (
-            f" [#{note.todo_payload.priority}]" if note.todo_payload else ""
+            f" {note.todo_payload.priority}" if note.todo_payload else ""
         )
         result += f"{char}{priority} {note.body.strip()}\n"
     return result
 
 
 def _get_header(level: int) -> str:
     if level == 1:
-        return "#########"
+        return "\n#########"
     elif level == 2:
         return "======="
     elif level == 3:
         return "*****"
     elif level == 4:
         return "---"
     else:
```

### Comparing `zettel_org-0.7.2/src/zorg/service/templates.py` & `zettel_org-0.7.3/src/zorg/service/templates.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/src/zorg/service/zid_manager.py` & `zettel_org-0.7.3/src/zorg/service/zid_manager.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/src/zorg/storage/sql/converters.py` & `zettel_org-0.7.3/src/zorg/storage/sql/converters.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,73 @@
 """Contains logic to convert domain models to/from SQL models."""
 
 from collections import defaultdict
 from dataclasses import dataclass
+import operator
 from pathlib import Path
-from typing import Any, Callable, Optional, cast
+from typing import Any, Callable, Optional, TypeVar, cast
 
 import metaman
-from sqlmodel import Session, and_, or_, select
+from sqlalchemy import func
+from sqlmodel import Integer, Session, and_, or_, select
 from sqlmodel.sql.expression import ColumnElement, SelectOfScalar
 
 from . import models as sql
 from ...domain.models import (
     File,
     Note,
     TodoPayload,
     WhereAndFilter,
     WhereOrFilter,
 )
-from ...domain.types import EntityConverter, NoteType, TodoPriorityType
-from ...service import common
+from ...domain.types import (
+    DescOperator,
+    EntityConverter,
+    NoteType,
+    PropertyOperator,
+    PropertyValueType,
+    TodoPriorityType,
+)
+from ...service import common, dates as zdt
 
 
 _SONConverterParser = Callable[["_SONConverter"], Optional[ColumnElement]]
 # the @_son_converter_parser decorator should be used to mark a _SONConverter
 # parser method
 _SON_CONVERTER_PARSERS: list[_SONConverterParser] = []
 _son_converter_parser = metaman.register_function_factory(
     _SON_CONVERTER_PARSERS
 )
 
+_T = TypeVar("_T")
+
 
 # TODO(bugyi): Rename to_select_of_note() and other related identifiers.
+# TODO(bugyi): Move to_select_of_note() out of of this file!
 def to_select_of_note(
-    or_filter: Optional[WhereOrFilter],
+    or_filter: Optional[WhereOrFilter], session: Session
 ) -> SelectOfScalar[sql.ZorgNote]:
     """Converts a WhereOrFilter to a SQL SELECT that will fetch ZorgNotes."""
     if or_filter is None or not or_filter.and_filters:
         return select(sql.ZorgNote)
 
     return select(sql.ZorgNote).where(
         or_(*[
-            _SONConverter(and_filter).to_note_clause()
+            _SONConverter(and_filter, session).to_note_clause()
             for and_filter in or_filter.and_filters
         ])
     )
 
 
 @dataclass(frozen=True)
 class _SONConverter:
     """Converts a WhereAndFilter to a ColumnElement."""
 
     and_filter: WhereAndFilter
+    session: Session
 
     def to_note_clause(self) -> ColumnElement:
         """Constructs a SQL statement from the provided WhereAndFilter."""
         and_clauses = []
         for parse in _SON_CONVERTER_PARSERS:
             clause = parse(self)
             if clause is not None:
@@ -131,24 +144,148 @@
         if not or_filters:
             return None
 
         or_conds = []
         for or_filter in or_filters:
             or_conds.append(
                 or_(*[
-                    _SONConverter(and_filter).to_note_clause()
+                    _SONConverter(and_filter, self.session).to_note_clause()
                     for and_filter in or_filter.and_filters
                 ])
             )
         return (
             and_(or_conds[0], *or_conds[1:])
             if len(or_conds) > 1
             else or_conds[0]
         )
 
+    @_son_converter_parser
+    def date_ranges(self) -> Optional[ColumnElement]:
+        """Converter that handles create/modify date ranges."""
+        and_conds = []
+        for date_range_list, sql_date in [
+            (self.and_filter.create_date_ranges, sql.ZorgNote.create_date),
+            (self.and_filter.modify_date_ranges, sql.ZorgNote.modify_date),
+        ]:
+            for date_range in date_range_list:
+                date_filters = [sql_date >= date_range.start]
+                end_date = (
+                    date_range.end if date_range.end else date_range.start
+                )
+                date_filters.append(sql_date <= end_date)
+                and_conds.append(and_(*date_filters))
+
+        if and_conds:
+            return and_(and_conds[0], *and_conds[1:])
+        else:
+            return None
+
+    @_son_converter_parser
+    def property_filters(self) -> Optional[ColumnElement]:
+        """Converter tht handles property filters."""
+        if not self.and_filter.property_filters:
+            return None
+        and_conds = []
+        for property_filter in self.and_filter.property_filters:
+            negated = property_filter.negated
+            comp_op_map = {
+                PropertyOperator.EQ: operator.ne if negated else operator.eq,
+                PropertyOperator.LT: operator.ge if negated else operator.lt,
+                PropertyOperator.GT: operator.le if negated else operator.gt,
+                PropertyOperator.LE: operator.gt if negated else operator.le,
+                PropertyOperator.GE: operator.lt if negated else operator.ge,
+            }
+            subquery = (
+                select(sql.ZorgNote.id)
+                .join(sql.PropertyLink)
+                .join(sql.Property)
+                .where(sql.Property.name == property_filter.key)
+            )
+
+            op = sql.ZorgNote.id.in_  # type: ignore[union-attr]
+            if property_filter.op == PropertyOperator.EXISTS and negated:
+                op = sql.ZorgNote.id.not_in  # type: ignore[union-attr]
+            elif property_filter.op != PropertyOperator.EXISTS:
+                comp_op = comp_op_map[property_filter.op]
+
+                value_type_map: dict[
+                    PropertyValueType,
+                    tuple[Callable[[Any], Any], Callable[[Any], Any]],
+                ] = {
+                    PropertyValueType.DATE: (func.date, zdt.to_date),
+                    PropertyValueType.INTEGER: (_col_to_int, int),
+                    PropertyValueType.STRING: (_noop, _noop),
+                }
+                cast_model, cast_value = value_type_map[
+                    property_filter.value_type
+                ]
+                subquery = subquery.where(
+                    comp_op(
+                        cast_model(sql.PropertyLink.value),
+                        cast_value(property_filter.value),
+                    )
+                )
+
+            and_conds.append(op(subquery))
+
+        return and_(and_conds[0], *and_conds[1:])
+
+    @_son_converter_parser
+    def desc_filters(self) -> Optional[ColumnElement]:
+        and_conds = []
+        if not self.and_filter.desc_filters:
+            return None
+
+        for desc_filter in self.and_filter.desc_filters:
+            case_sensitive = desc_filter.case_sensitive
+            if case_sensitive is None:
+                case_sensitive = not bool(desc_filter.value.islower())
+
+            like_arg = f"%{desc_filter.value}%"
+            op_arg: Any
+            if case_sensitive:
+                cond = sql.ZorgNote.body.like(like_arg)  # type: ignore[attr-defined]
+                subquery = select(sql.ZorgNote.id, sql.ZorgNote.body).where(
+                    cond
+                )
+                id_list: list[int] = []
+                for ID, body in self.session.exec(subquery).all():
+                    assert (
+                        ID is not None
+                    ), "The DB shouldn't contain notes without an ID, right?"
+                    if desc_filter.value in body:
+                        id_list.append(ID)
+
+                op_map: dict[DescOperator, Any] = {
+                    DescOperator.CONTAINS: sql.ZorgNote.id.in_,  # type: ignore[union-attr]
+                    DescOperator.NOT_CONTAINS: sql.ZorgNote.id.not_in,  # type: ignore[union-attr]
+                }
+                op = op_map[desc_filter.op]
+                op_arg = id_list
+            else:
+                op_map = {
+                    DescOperator.CONTAINS: sql.ZorgNote.body.ilike,  # type: ignore[attr-defined]
+                    DescOperator.NOT_CONTAINS: sql.ZorgNote.body.not_ilike,  # type: ignore[attr-defined]
+                }
+                op = op_map[desc_filter.op]
+                op_arg = like_arg
+
+            and_conds.append(op(op_arg))
+        return and_(and_conds[0], *and_conds[1:])
+
+
+def _noop(value: _T) -> _T:
+    """A function that does nothing."""
+    return value
+
+
+def _col_to_int(value: Any) -> Any:
+    """Casts SQL table's column to integer."""
+    return func.cast(value, Integer)  # pylint: disable=not-callable
+
 
 def _to_todo_status(note_type: NoteType) -> Optional[NoteType]:
     if note_type is NoteType.BASIC:
         return None
     else:
         return note_type
 
@@ -205,14 +342,15 @@
 
     def _from_entity_with_session(
         self, entity: Note, session: Session
     ) -> sql.ZorgNote:
         kwargs: dict[str, Any] = {
             "body": entity.body,
             "create_date": entity.create_date,
+            "modify_date": entity.modify_date,
             "zid": entity.zid,
         }
         if entity.todo_payload:
             kwargs["todo_status"] = entity.todo_payload.status
             kwargs["todo_priority"] = entity.todo_payload.priority
         sql_zorg_note = sql.ZorgNote(**kwargs)
 
@@ -279,12 +417,15 @@
             and sql_model.todo_status is not None
             else None
         )
         return Note(
             sql_model.body,
             areas=list(area.name for area in sql_model.areas),
             contexts=list(context.name for context in sql_model.contexts),
+            create_date=sql_model.create_date,
             file_path=Path(sql_model.zorg_file.path),
+            modify_date=sql_model.modify_date,
             people=list(person.name for person in sql_model.people),
             projects=list(project.name for project in sql_model.projects),
             todo_payload=todo_payload,
+            zid=sql_model.zid,
         )
```

### Comparing `zettel_org-0.7.2/src/zorg/storage/sql/engine.py` & `zettel_org-0.7.3/src/zorg/storage/sql/engine.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/src/zorg/storage/sql/models.py` & `zettel_org-0.7.3/src/zorg/storage/sql/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     body: str
 
     # TODO(bugyi): Make zid required to persist to DB.
     # TODO(bugyi): Make zid unique.
     zid: Optional[str] = Field(default=None)
 
     create_date: dt.date = Field(default_factory=dt.date.today)
+    modify_date: dt.date = Field(default_factory=dt.date.today)
     todo_priority: Optional[str] = None
     todo_status: Optional[NoteType] = None
 
     # relationships
     zorg_file: ZorgFile = Relationship(
         back_populates="notes", link_model=ZorgFileLink
     )
```

### Comparing `zettel_org-0.7.2/src/zorg/storage/sql/repo.py` & `zettel_org-0.7.3/src/zorg/storage/sql/repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # pylint: disable=unsubscriptable-object
 
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Optional
 
-from eris import ErisResult, Err, Ok
+from eris import ErisResult, Ok
 from logrus import Logger
 from sqlmodel import Session, select
 
 from . import models as sql
 from ...domain.messages.events import NewZorgNotesEvent
 from ...domain.models import File, Note, WhereOrFilter
 from ...service.zid_manager import ZIDManager
@@ -84,17 +84,17 @@
                             self._session.delete(tag)
                             self._session.commit()
 
                 self._session.delete(sql_note)
             self._session.delete(sql_zorg_file)
             return Ok(zorg_file)
         else:
-            emsg = "Failed to delete Zorg File"
-            _LOGGER.warning(emsg, path=path)
-            return Err(emsg)
+            emsg = "Cannot delete zorg file since it does not exist."
+            _LOGGER.debug(emsg, path=path)
+            return Ok(None)
 
     def get(self, key: str) -> ErisResult[Optional[File]]:
         """Retrieve a file from the DB."""
         path = key
         stmt = select(sql.ZorgFile).where(sql.ZorgFile.path == path)
         results = self._session.exec(stmt)
         sql_zorg_file = results.first()
@@ -103,15 +103,15 @@
             self._seen_zorg_file(zorg_file)
             return Ok(zorg_file)
         else:
             return Ok(None)
 
     def get_by_query(self, query: Optional[WhereOrFilter]) -> list[Note]:
         """Get file(s) from DB by using a query."""
-        select_of_note = to_select_of_note(query)
+        select_of_note = to_select_of_note(query, self._session)
         # If the user asked for really verbose output...
         if self._verbose > 1:
             # ... then we print the SELECT statement.
             print(select_of_note)
 
         result: list[Note] = []
         for sql_note in self._session.exec(select_of_note):
```

### Comparing `zettel_org-0.7.2/src/zorg/storage/sql/session.py` & `zettel_org-0.7.3/src/zorg/storage/sql/session.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/targets.mk` & `zettel_org-0.7.3/targets.mk`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/__snapshots__/test_run_edit.ambr` & `zettel_org-0.7.3/tests/__snapshots__/test_run_edit.ambr`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   # 2000-01-03.Mon
   #
   # ^ = [[2000/20000103]]
   # < = [[2000/20000102_day]]
   # > = [[2000/20000104_day]]
   # @ = [[day_log.zot]]
   
-  o 000103#29 #gtd pomodoro
+  o 000103#01 #gtd pomodoro
     * Google Calendar (bbugyi@google + bryanbugyi34@gmail)
     * Process yesterday's bujo log (e.g. close events, add missing pomodoros, rollover goals)
     * Copy any important gchat convos from yesterday into chat/*.txt
     * Check today's tickler file: [[tick_03]]
     * Fill out yesterday's habit tracker: [[2000/20000102_habit]]
     * go/g3co
     * Review Google Keep Inbox
```

### Comparing `zettel_org-0.7.2/tests/__snapshots__/test_run_template.ambr` & `zettel_org-0.7.3/tests/__snapshots__/test_run_template.ambr`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/common.py` & `zettel_org-0.7.3/tests/common.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/conftest.py` & `zettel_org-0.7.3/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,50 +11,65 @@
 from typing import TYPE_CHECKING, Any, Iterator
 
 from _pytest.tmpdir import TempPathFactory
 from freezegun import freeze_time
 from pytest import fixture
 
 from zorg.app.__main__ import main as zorg_main
+from zorg.service.zid_manager import ZIDManager
 
 from . import common as c
 
 
 pytest_plugins = ["clack.pytest_plugin", "vimala.pytest_plugin"]
 
 
 if TYPE_CHECKING:  # fixes pytest warning
     from clack.pytest_plugin import MakeConfigFile
 
 
+@fixture(autouse=True)
+def clear_zid_cache() -> None:
+    """Clears the in-memory ZID mapping."""
+    ZIDManager._class_next_id_map = None
+
+
 @fixture(scope="session")
 def zettel_dir(tmp_path_factory: TempPathFactory) -> Path:
     """Returns a zettel directory that contains copies of all *.zo files."""
     return _get_zettel_dir(tmp_path_factory.getbasetemp())
 
 
-@fixture(scope="module")
-def module_zettel_dir(tmp_path_factory: TempPathFactory) -> Path:
+@fixture(scope="session", name="query_zettel_dir")
+def query_zettel_dir_fixture(tmp_path_factory: TempPathFactory) -> Path:
     """Returns a zettel directory that contains copies of all *.zo files."""
-    tmp_path = tmp_path_factory.getbasetemp() / "module_scope"
+    tmp_path = tmp_path_factory.getbasetemp() / "query_tests"
     tmp_path.mkdir()
     return _get_zettel_dir(tmp_path)
 
 
+@fixture(scope="session")
+def db_zettel_dir(main: c.MainType, query_zettel_dir: Path) -> Path:
+    """Returns zettel dir containing pre-initialized database.."""
+    ec = main("--log=null", "--dir", str(query_zettel_dir), "db", "create")
+    assert ec == 0
+    return query_zettel_dir
+
+
 def _get_zettel_dir(tmp_path: Path) -> Path:
     zdir = tmp_path / "org"
     zdir.mkdir()
     for zo_path in _get_all_zo_and_zot_paths():
         zettel_zo_path = zdir / zo_path.name
         zettel_zo_path.write_bytes(zo_path.read_bytes())
     return zdir
 
 
-@fixture(scope="session")
-def main(make_config_file: MakeConfigFile) -> c.MainType:
+@fixture(scope="session", name="main")
+def main_fixture(make_config_file: MakeConfigFile) -> c.MainType:
     """Returns a wrapper around zorg's main() function."""
 
     def inner_main(*args: str, **kwargs: Any) -> int:
         cfg_kwargs = {
             k: v if isinstance(v, (dict, list)) else str(v)
             for (k, v) in kwargs.items()
         }
```

### Comparing `zettel_org-0.7.2/tests/data/day_log.zot` & `zettel_org-0.7.3/tests/data/day_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/data/done_log.zot` & `zettel_org-0.7.3/tests/data/done_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/data/habit_log.zot` & `zettel_org-0.7.3/tests/data/habit_log.zot`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/test_config.py` & `zettel_org-0.7.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/test_file_groups.py` & `zettel_org-0.7.3/tests/test_file_groups.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/test_run_compile.py` & `zettel_org-0.7.3/tests/test_run_compile.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/test_run_db.py` & `zettel_org-0.7.3/tests/test_run_db.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/test_run_edit.py` & `zettel_org-0.7.3/tests/test_run_edit.py`

 * *Files identical despite different names*

### Comparing `zettel_org-0.7.2/tests/test_run_template.py` & `zettel_org-0.7.3/tests/test_run_template.py`

 * *Files identical despite different names*

