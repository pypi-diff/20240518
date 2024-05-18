# Comparing `tmp/OZI-1.7.4.tar.gz` & `tmp/OZI-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI-1.7.4.tar", last modified: Sat May 18 01:28:16 2024, max compression
+gzip compressed data, was "OZI-1.8.0.tar", last modified: Sat May 18 07:17:15 2024, max compression
```

## Comparing `OZI-1.7.4.tar` & `OZI-1.8.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.894777 OZI-1.7.4/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.866777 OZI-1.7.4/.github/
--rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/.markdownlint.json
--rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/CODEOWNERS
--rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/CONTRIBUTING.md
--rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/FUNDING.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.866777 OZI-1.7.4/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/SECURITY.md
--rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/dependabot.yml
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.870777 OZI-1.7.4/.github/workflows/
--rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/workflows/codeql.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/workflows/dependency-review.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     2900 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/workflows/dev-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     6530 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/workflows/dist-workflow.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3579 2024-05-18 01:25:25.000000 OZI-1.7.4/.github/workflows/scorecard.yml
--rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-18 01:25:25.000000 OZI-1.7.4/.gitignore
--rw-rw-r--   0 runner    (1001) docker     (127)   310795 2024-05-18 01:25:25.000000 OZI-1.7.4/CHANGELOG.md
--rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-18 01:25:25.000000 OZI-1.7.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-18 01:28:01.666776 OZI-1.7.4/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (127)     6937 2024-05-18 01:25:25.000000 OZI-1.7.4/README.rst
--rw-rw-r--   0 runner    (1001) docker     (127)    16774 2024-05-18 01:25:25.000000 OZI-1.7.4/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     7660 2024-05-18 01:25:25.000000 OZI-1.7.4/meson.options
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.890777 OZI-1.7.4/ozi/
--rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/actions.py
--rw-rw-r--   0 runner    (1001) docker     (127)     5811 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/comment.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.878777 OZI-1.7.4/ozi/dist/
--rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/dist/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.878777 OZI-1.7.4/ozi/dist/semantic_release/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/dist/semantic_release/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/dist/semantic_release/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.878777 OZI-1.7.4/ozi/dist/sigstore/
--rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/dist/sigstore/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/dist/sigstore/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.878777 OZI-1.7.4/ozi/fix/
--rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/fix/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/fix/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4061 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/fix/build_definition.py
--rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/fix/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6321 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/fix/missing.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/fix/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/fix/rewrite_command.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.882777 OZI-1.7.4/ozi/lint/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.878777 OZI-1.7.4/ozi/lint/bandit/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/bandit/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/bandit/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.882777 OZI-1.7.4/ozi/lint/black/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/black/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/black/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.882777 OZI-1.7.4/ozi/lint/flake8/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/flake8/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/flake8/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.882777 OZI-1.7.4/ozi/lint/isort/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/isort/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/isort/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.882777 OZI-1.7.4/ozi/lint/mypy/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/mypy/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/mypy/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.882777 OZI-1.7.4/ozi/lint/pyright/
--rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/pyright/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/pyright/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.882777 OZI-1.7.4/ozi/lint/readme-renderer/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/readme-renderer/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)       15 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/lint/readme-renderer/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/meson.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.886777 OZI-1.7.4/ozi/new/
--rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/new/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4745 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/new/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/new/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     6940 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/new/parser.py
--rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/new/validate.py
--rw-rw-r--   0 runner    (1001) docker     (127)     3128 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/pkg_extra.py
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     6696 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/render.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.886777 OZI-1.7.4/ozi/scripts/
--rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/scripts/core_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/scripts/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/scripts/meson_dist_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/scripts/meson_setuptools_scm.py
--rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/scripts/render_requirements.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/scripts/replace_ruff_target_version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/scripts/scm_version_snip.py
--rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/scripts/to_distribution_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/scripts/version_metadata_template.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spdx.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.890777 OZI-1.7.4/ozi/spec/
--rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spec/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spec/_license.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1660 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spec/_spec.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spec/base.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6233 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spec/ci.py
--rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spec/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)     4480 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spec/pkg.py
--rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spec/project.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spec/python.py
--rw-rw-r--   0 runner    (1001) docker     (127)     4564 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/spec/src.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/tap.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.890777 OZI-1.7.4/ozi/test/
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.890777 OZI-1.7.4/ozi/test/coverage/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/test/coverage/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/test/coverage/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/test/meson.build
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.890777 OZI-1.7.4/ozi/test/pytest/
--rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/test/pytest/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/test/pytest/requirements.in
--rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/trove.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.894777 OZI-1.7.4/ozi/vendor/
--rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/__init__.py
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.894777 OZI-1.7.4/ozi/vendor/email_validator/
--rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/email_validator/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/email_validator/__main__.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/email_validator/deliverability.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/email_validator/exceptions_types.py
--rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/email_validator/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/email_validator/py.typed
--rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/email_validator/rfc_constants.py
--rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/email_validator/syntax.py
--rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/email_validator/validate_email.py
--rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/email_validator/version.py
--rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-18 01:25:25.000000 OZI-1.7.4/ozi/vendor/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11225 2024-05-18 01:25:25.000000 OZI-1.7.4/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (127)      206 2024-05-18 01:25:25.000000 OZI-1.7.4/requirements.in
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.894777 OZI-1.7.4/templates/
--rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-18 01:25:25.000000 OZI-1.7.4/templates/CHANGELOG.md.j2
-drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 01:28:01.898777 OZI-1.7.4/tests/
--rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-18 01:25:25.000000 OZI-1.7.4/tests/meson.build
--rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-18 01:25:25.000000 OZI-1.7.4/tests/test_ozi_fix.py
--rw-rw-r--   0 runner    (1001) docker     (127)    14348 2024-05-18 01:25:25.000000 OZI-1.7.4/tests/test_ozi_new.py
--rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-18 01:25:25.000000 OZI-1.7.4/tests/test_tap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.232027 OZI-1.8.0/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.204028 OZI-1.8.0/.github/
+-rw-rw-r--   0 runner    (1001) docker     (127)      102 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/.markdownlint.json
+-rw-rw-r--   0 runner    (1001) docker     (127)      574 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/CODEOWNERS
+-rw-rw-r--   0 runner    (1001) docker     (127)     3227 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     2862 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/CONTRIBUTING.md
+-rw-rw-r--   0 runner    (1001) docker     (127)       85 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/FUNDING.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.204028 OZI-1.8.0/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 runner    (1001) docker     (127)      834 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      595 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-r--   0 runner    (1001) docker     (127)     1696 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/SECURITY.md
+-rw-rw-r--   0 runner    (1001) docker     (127)      434 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/dependabot.yml
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.204028 OZI-1.8.0/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (127)     3081 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/workflows/codeql.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     1091 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/workflows/dependency-review.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     2901 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/workflows/dev-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     6530 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/workflows/dist-workflow.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3579 2024-05-18 07:13:53.000000 OZI-1.8.0/.github/workflows/scorecard.yml
+-rw-rw-r--   0 runner    (1001) docker     (127)     3194 2024-05-18 07:13:53.000000 OZI-1.8.0/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (127)   312243 2024-05-18 07:13:53.000000 OZI-1.8.0/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (127)    12456 2024-05-18 07:13:53.000000 OZI-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-05-18 07:16:57.984029 OZI-1.8.0/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (127)     6968 2024-05-18 07:13:53.000000 OZI-1.8.0/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (127)    17469 2024-05-18 07:13:53.000000 OZI-1.8.0/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     7549 2024-05-18 07:13:53.000000 OZI-1.8.0/meson.options
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.228027 OZI-1.8.0/ozi/
+-rw-rw-r--   0 runner    (1001) docker     (127)      502 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3418 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7089 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/actions.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     5880 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/comment.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.212027 OZI-1.8.0/ozi/dist/
+-rw-rw-r--   0 runner    (1001) docker     (127)      481 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/dist/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.212027 OZI-1.8.0/ozi/dist/semantic_release/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/dist/semantic_release/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/dist/semantic_release/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.212027 OZI-1.8.0/ozi/dist/sigstore/
+-rw-rw-r--   0 runner    (1001) docker     (127)      412 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/dist/sigstore/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        8 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/dist/sigstore/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.216027 OZI-1.8.0/ozi/fix/
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/fix/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2469 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/fix/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4097 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/fix/build_definition.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      619 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/fix/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6391 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/fix/missing.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3927 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/fix/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     7879 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/fix/rewrite_command.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.220027 OZI-1.8.0/ozi/lint/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.216027 OZI-1.8.0/ozi/lint/bandit/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/bandit/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       12 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/bandit/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.216027 OZI-1.8.0/ozi/lint/black/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/black/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       14 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/black/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.216027 OZI-1.8.0/ozi/lint/flake8/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/flake8/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      276 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/flake8/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.216027 OZI-1.8.0/ozi/lint/isort/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/isort/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        5 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/isort/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      547 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.216027 OZI-1.8.0/ozi/lint/mypy/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/mypy/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        4 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/mypy/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.220027 OZI-1.8.0/ozi/lint/pyright/
+-rw-rw-r--   0 runner    (1001) docker     (127)      799 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/pyright/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       16 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/pyright/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.220027 OZI-1.8.0/ozi/lint/readme-renderer/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/readme-renderer/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)       19 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/lint/readme-renderer/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      808 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     8128 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/meson.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.220027 OZI-1.8.0/ozi/new/
+-rw-rw-r--   0 runner    (1001) docker     (127)      249 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/new/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4745 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/new/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      567 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/new/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     6940 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/new/parser.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     8155 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/new/validate.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     3164 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/pkg_extra.py
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     6696 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/render.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.224027 OZI-1.8.0/ozi/scripts/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1494 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/scripts/core_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      771 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/scripts/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     2088 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/scripts/meson_dist_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1850 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/scripts/meson_setuptools_scm.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      864 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/scripts/render_requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1026 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/scripts/replace_ruff_target_version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      721 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/scripts/scm_version_snip.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      716 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/scripts/to_distribution_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      589 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/scripts/version_metadata_template.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1045 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spdx.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.224027 OZI-1.8.0/ozi/spec/
+-rw-rw-r--   0 runner    (1001) docker     (127)      459 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spec/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4120 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spec/_license.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1660 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spec/_spec.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2414 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spec/base.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6164 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spec/ci.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      641 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spec/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)     4480 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spec/pkg.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     1373 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spec/project.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6472 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spec/python.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     4564 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/spec/src.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6649 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/tap.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.228027 OZI-1.8.0/ozi/test/
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.228027 OZI-1.8.0/ozi/test/coverage/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/test/coverage/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      195 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/test/coverage/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)      454 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/test/meson.build
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.228027 OZI-1.8.0/ozi/test/pytest/
+-rw-rw-r--   0 runner    (1001) docker     (127)      411 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/test/pytest/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)      104 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/test/pytest/requirements.in
+-rw-rw-r--   0 runner    (1001) docker     (127)     1990 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/trove.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.232027 OZI-1.8.0/ozi/vendor/
+-rw-rw-r--   0 runner    (1001) docker     (127)       26 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/__init__.py
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.232027 OZI-1.8.0/ozi/vendor/email_validator/
+-rw-rw-r--   0 runner    (1001) docker     (127)     4283 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/email_validator/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2181 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/email_validator/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6121 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/email_validator/deliverability.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6000 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/email_validator/exceptions_types.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      736 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/email_validator/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)        0 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/email_validator/py.typed
+-rw-rw-r--   0 runner    (1001) docker     (127)     2768 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/email_validator/rfc_constants.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    28340 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/email_validator/syntax.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     6845 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/email_validator/validate_email.py
+-rw-rw-r--   0 runner    (1001) docker     (127)       28 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/email_validator/version.py
+-rw-rw-r--   0 runner    (1001) docker     (127)      659 2024-05-18 07:13:53.000000 OZI-1.8.0/ozi/vendor/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    10976 2024-05-18 07:13:53.000000 OZI-1.8.0/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (127)      278 2024-05-18 07:13:53.000000 OZI-1.8.0/requirements.in
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.232027 OZI-1.8.0/templates/
+-rw-rw-r--   0 runner    (1001) docker     (127)     1152 2024-05-18 07:13:53.000000 OZI-1.8.0/templates/CHANGELOG.md.j2
+drwxrwxr-x   0 runner    (1001) docker     (127)        0 2024-05-18 07:16:58.232027 OZI-1.8.0/tests/
+-rw-rw-r--   0 runner    (1001) docker     (127)      556 2024-05-18 07:13:53.000000 OZI-1.8.0/tests/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (127)    11130 2024-05-18 07:13:53.000000 OZI-1.8.0/tests/test_ozi_fix.py
+-rw-rw-r--   0 runner    (1001) docker     (127)    14348 2024-05-18 07:13:53.000000 OZI-1.8.0/tests/test_ozi_new.py
+-rw-rw-r--   0 runner    (1001) docker     (127)     2238 2024-05-18 07:13:53.000000 OZI-1.8.0/tests/test_tap.py
```

### Comparing `OZI-1.7.4/.github/CODEOWNERS` & `OZI-1.8.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/.github/CODE_OF_CONDUCT.md` & `OZI-1.8.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/.github/CONTRIBUTING.md` & `OZI-1.8.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/.github/ISSUE_TEMPLATE/bug_report.md` & `OZI-1.8.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/.github/ISSUE_TEMPLATE/feature_request.md` & `OZI-1.8.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/.github/SECURITY.md` & `OZI-1.8.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/.github/workflows/codeql.yml` & `OZI-1.8.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/.github/workflows/dependency-review.yml` & `OZI-1.8.0/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/.github/workflows/dev-workflow.yml` & `OZI-1.8.0/.github/workflows/dev-workflow.yml`

 * *Files 13% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@1ad9ec15d60558ee3da890634bb8b0406838e17a
+      - uses: OZI-Project/checkpoint@0f75e9157058098617d7c11cd43c909f10fa974a
         with:
           python-version: "3.10"
 
   checkpoint-cp311-ubuntu-latest:
     name: checkpoint (Python 3.11 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -60,15 +60,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@1ad9ec15d60558ee3da890634bb8b0406838e17a
+      - uses: OZI-Project/checkpoint@0f75e9157058098617d7c11cd43c909f10fa974a
         with:
           python-version: "3.11"
 
   checkpoint-cp312-ubuntu-latest:
     name: checkpoint (Python 3.12 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -88,10 +88,10 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@1ad9ec15d60558ee3da890634bb8b0406838e17a
+      - uses: OZI-Project/checkpoint@0f75e9157058098617d7c11cd43c909f10fa974a
         with:
-          python-version: "3.12"
+          python-version: "3.12"
```

### Comparing `OZI-1.7.4/.github/workflows/dist-workflow.yml` & `OZI-1.8.0/.github/workflows/dist-workflow.yml`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@1ad9ec15d60558ee3da890634bb8b0406838e17a
+      - uses: OZI-Project/checkpoint@0f75e9157058098617d7c11cd43c909f10fa974a
         with:
           python-version: "3.10"
 
   checkpoint-cp311-ubuntu-latest:
     name: checkpoint (Python 3.11 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -62,15 +62,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@1ad9ec15d60558ee3da890634bb8b0406838e17a
+      - uses: OZI-Project/checkpoint@0f75e9157058098617d7c11cd43c909f10fa974a
         with:
           python-version: "3.11"
 
   checkpoint-cp312-ubuntu-latest:
     name: checkpoint (Python 3.12 on ubuntu-latest)
     runs-on: ubuntu-latest
     strategy:
@@ -90,15 +90,15 @@
             pypi.org:443
             registry.npmjs.org:443
             objects.githubusercontent.com:443
             fulcio.sigstore.dev:443
             rekor.sigstore.dev:443
             tuf-repo-cdn.sigstore.dev:443
 
-      - uses: OZI-Project/checkpoint@1ad9ec15d60558ee3da890634bb8b0406838e17a
+      - uses: OZI-Project/checkpoint@0f75e9157058098617d7c11cd43c909f10fa974a
         with:
           python-version: "3.12"
 
   checkpoint:
     runs-on: ubuntu-latest
     needs: [checkpoint-cp310-ubuntu-latest, checkpoint-cp311-ubuntu-latest, checkpoint-cp312-ubuntu-latest]
     steps:
```

### Comparing `OZI-1.7.4/.github/workflows/scorecard.yml` & `OZI-1.8.0/.github/workflows/scorecard.yml`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/.gitignore` & `OZI-1.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/CHANGELOG.md` & `OZI-1.8.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,56 @@
 # CHANGELOG
+## 1.8.0 (2024-05-18)
+
+### :arrow_up:
+
+* :arrow_up: OZI-Project/checkpoint 0.2.0
+
+Signed-off-by: Eden Ross Duff, MSc &lt;ozi.project@outlook.com&gt; ([`1cc5620`](https://github.com/OZI-Project/OZI/commit/1cc5620f3bea66a56247a7ad61f9f854926b0286))
+
+### :pushpin:
+
+* :pushpin: Update ozi/spec/ci.py - checkpoint 0.2.0
+
+Signed-off-by: Eden Ross Duff, MSc &lt;ozi.project@outlook.com&gt; ([`48b4cf6`](https://github.com/OZI-Project/OZI/commit/48b4cf699fd69af3ae5d152beeb80a43184352a2))
+
+### :sparkles:
+
+* :sparkles: Update README.rst for 1.8
+
+Signed-off-by: Eden Ross Duff, MSc &lt;ozi.project@outlook.com&gt; ([`31f26dd`](https://github.com/OZI-Project/OZI/commit/31f26dd17f6ed28adf0250e9f4725a93696742d4))
+
+### Other
+
+* Feature/1.8 pipx integration (#540)
+
+* :sparkles: Enable pipx isolation of apps.
+* :hammer: Update spec files.
+* :arrow_up: OZI Spec v0.4
+* :wrench: add 1.8 release branch pattern.
+
+The following are no longer in ``meson.options:module-only``:
+* sigstore
+* Flake8-pyproject
+* coverage
+* flake8
+* bandit
+* black
+* isort
+* pyright
+* mypy
+
+---------
+
+Signed-off-by: rjdbcm &lt;ozi.project@outlook.com&gt; ([`50d4509`](https://github.com/OZI-Project/OZI/commit/50d450935d3333a58c98c8dbf19d594620adce36))
+
+* Update dist-workflow.yml checkpoint 0.2.0
+
+Signed-off-by: Eden Ross Duff, MSc &lt;ozi.project@outlook.com&gt; ([`a155b06`](https://github.com/OZI-Project/OZI/commit/a155b0627a82cf6d9868b13b74f7697568cbbfd5))
+
 ## 1.7.4 (2024-05-18)
 
 ### :arrow_up:
 
 * :arrow_up: Bump OZI-Project/draft from 0.1.1 to 0.1.2
 
 Bumps [OZI-Project/draft](https://github.com/ozi-project/draft) from 0.1.1 to 0.1.2.
```

### Comparing `OZI-1.7.4/LICENSE.txt` & `OZI-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/PKG-INFO` & `OZI-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: OZI
-Version: 1.7.4
+Version: 1.8.0
 Summary: Package Python projects with Meson.
-Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.7.4.tar.gz
+Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/1.8.0.tar.gz
 Home-page: https://oziproject.dev/
 Author: Eden Ross Duff MSc
 Author-email: help@oziproject.dev
 License: Apache-2.0 WITH LLVM-exception
 Keywords: meson,packaging,wheel
 Project-URL: Bug Tracker, https://github.com/rjdbcm/ozi/issues
 Project-URL: Community, https://github.com/orgs/OZI-Project/discussions
-Requires-Dist: blastpipe~=2024.7.4
 Requires-Dist: GitPython>=3
+Requires-Dist: blastpipe~=2024.7.4
 Requires-Dist: dnspython
 Requires-Dist: idna>=2
 Requires-Dist: jinja2>=3
-Requires-Dist: meson>=1.1.0
+Requires-Dist: meson[ninja]>=1.1.0
 Requires-Dist: packaging~=24.0
+Requires-Dist: pip-tools
 Requires-Dist: pyparsing~=3.1
 Requires-Dist: requests
+Requires-Dist: setuptools_scm[toml]
 Requires-Dist: spdx-license-list
+Requires-Dist: tomli>=2.0.0;python_version<"3.11"
 Requires-Dist: trove-classifiers
 Requires-Dist: types-requests
 Requires-Dist: typing-extensions;python_version=="3.10"
 Requires-External: git
 Requires-Python: >=3.10, <3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -74,23 +77,24 @@
 ^^^^^^^
 
 OZI is meant for Python developers as a standardized and opinionated
 Python packaging style guide and continuous integration checkpointing API using the Meson build system.
 
 The OZI continuous integration strategy consists of:
 
-1. The following checkpointed environments:
+1. The following isolated checkpoint environments:
 
 * code testing and coverage
 * distributing Python packages with Meson_
 * code linting and formatting
 
 2. Release drafting
-3. Provenance generation (`SLSA v1.0 - Level 3 <https://slsa.dev/spec/v1.0/levels#build-l3>`_)
-4. Publishing
+3. Building of releases
+4. Provenance generation (`SLSA v1.0 - Level 3 <https://slsa.dev/spec/v1.0/levels#build-l3>`_)
+5. Publishing
 
 What OZI is **not**
 ###################
 
 * A replacement for test environment managers like tox_, as a matter of fact OZI uses ``tox``.
 * A replacement for git hook package management tools like pre-commit_
```

### Comparing `OZI-1.7.4/README.rst` & `OZI-1.8.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,24 @@
 ^^^^^^^
 
 OZI is meant for Python developers as a standardized and opinionated
 Python packaging style guide and continuous integration checkpointing API using the Meson build system.
 
 The OZI continuous integration strategy consists of:
 
-1. The following checkpointed environments:
+1. The following isolated checkpoint environments:
 
 * code testing and coverage
 * distributing Python packages with Meson_
 * code linting and formatting
 
 2. Release drafting
-3. Provenance generation (`SLSA v1.0 - Level 3 <https://slsa.dev/spec/v1.0/levels#build-l3>`_)
-4. Publishing
+3. Building of releases
+4. Provenance generation (`SLSA v1.0 - Level 3 <https://slsa.dev/spec/v1.0/levels#build-l3>`_)
+5. Publishing
 
 What OZI is **not**
 ###################
 
 * A replacement for test environment managers like tox_, as a matter of fact OZI uses ``tox``.
 * A replacement for git hook package management tools like pre-commit_
```

### Comparing `OZI-1.7.4/meson.build` & `OZI-1.8.0/meson.build`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
         '-c',
         python_readlines.format(scripts / 'replace_ruff_target_version.py'),
     ],
     check: true,
 ).stdout()
 run_command(python, ['-c', replace_ruff_target_version], check: true)
 pip = find_program('pip', required: true, disabler: true)
+pipx = find_program('pipx', required: true, disabler: true)
 pip_compile = find_program('pip-compile', required: true)
 if not meson.is_subproject()
     custom_target(
         'requirements.txt',
         input: root_files[3],
         output: 'requirements.txt',
         build_always_stale: true,
@@ -236,28 +237,44 @@
             modules += [command.underscorify()]  # we should collapse repeated `_`
         endif
         flag = disabler()
         if (
             (get_option('dev').enabled() or suite.enabled())
             and command not in plugin_only
         )
-            run_command(
-                pip,
-                [
-                    'install',
-                    '-r',
-                    meson.project_build_root() / 'ozi' / name / command / 'requirements.txt',
-                ],
-                check: true
-            )
+            if command not in module_only and get_option('tox-env-dir') != ''
+                run_command(
+                    pipx,
+                    [
+                        'runpip',
+                        'meson',
+                        '--python', python,
+                        'install',
+                        '-r',
+                        meson.project_build_root() / 'ozi' / name / command / 'requirements.txt',
+                    ],
+                    check: true
+                )
+            else
+                run_command(
+                    pip,
+                    [
+                        'install',
+                        '-r',
+                        meson.project_build_root() / 'ozi' / name / command / 'requirements.txt',
+                    ],
+                    check: true
+                )
+            endif
             if not flag.found() and command not in module_only
                 flag = find_program(
                     command,
                     required: false,
                     disabler: true,
+                    dirs: [get_option('tox-env-dir') / 'bin']
                 )
             elif command in module_only
                 command = command.replace('-', '_')
                 flag = command
             endif
         endif
         if command not in plugin_only
```

### Comparing `OZI-1.7.4/meson.options` & `OZI-1.8.0/meson.options`

 * *Files 4% similar despite different names*

```diff
@@ -177,33 +177,28 @@
         'pytest-xdist',
         'semantic_release',
         'sphinxawesome-codelinter',
         'sphinxawesome-theme',
         'flake8-comprehensions',
     ],
 )
-
+option(
+    'tox-env-dir',
+    type: 'string',
+    value: ''
+)
 option(
     'module-only',
     type: 'array',
     description: 'no application - python module entry point only',
     value: [
         'semantic_release',
-        'sigstore',
         'sphinxawesome-codelinter',
         'sphinxawesome-theme',
-        'Flake8-pyproject',
         'pytest',
-        'coverage',
-        'flake8',
-        'bandit',
-        'black',
-        'isort',
-        'pyright',
-        'mypy',
         'readme-renderer',
     ],
 )
 # test application arguments
 option('args-sigstore', type: 'array', value: ['--version'], yield: true)
 option(
     'args-semantic_release',
```

### Comparing `OZI-1.7.4/ozi/__main__.py` & `OZI-1.8.0/ozi/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/actions.py` & `OZI-1.8.0/ozi/actions.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/comment.py` & `OZI-1.8.0/ozi/comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 # ozi/comment.py
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 """Linter comment check utilities."""
+from __future__ import annotations
+
 import re
 from collections import Counter
 from enum import IntFlag
 from functools import lru_cache
 from math import log
 from math import log10
-from pathlib import Path  # noqa: TC003, RUF100
+from typing import TYPE_CHECKING
 from typing import Generator
 from typing import Sequence
 
 from ozi.spec import METADATA
 from ozi.tap import TAP
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 TIER3_COMMENTS = [
     'nosec',
     'pragma_defer_to',
     'pragma_no_cover',
     'type_ignore',
     'mypy',
     'pyright_ignore',
```

### Comparing `OZI-1.7.4/ozi/fix/__main__.py` & `OZI-1.8.0/ozi/fix/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/fix/build_definition.py` & `OZI-1.8.0/ozi/fix/build_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # ozi/fix/build_definition.py
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 """Build definition check utilities."""
+from __future__ import annotations
+
 import os
 from pathlib import Path
 from typing import Generator
 
 from ozi import comment
 from ozi.meson import get_items_by_suffix
 from ozi.meson import query_build_value
```

### Comparing `OZI-1.7.4/ozi/fix/meson.build` & `OZI-1.8.0/ozi/fix/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/fix/missing.py` & `OZI-1.8.0/ozi/fix/missing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 # ozi/fix/missing.py
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 """Find missing OZI project files."""
+from __future__ import annotations
+
 import re
 import sys
 from email import message_from_string
-from email.message import Message  # noqa: TC003, RUF100
 from pathlib import Path
 
 if sys.version_info >= (3, 11):  # pragma: no cover
     import tomllib as toml
 elif sys.version_info < (3, 11):  # pragma: no cover
     import tomli as toml
 
+from typing import TYPE_CHECKING
+
 from blastpipe.ozi_templates.filter import underscorify  # pyright: ignore
 
 from ozi.fix.build_definition import walk
 from ozi.meson import load_ast
 from ozi.meson import project_metadata
 from ozi.pkg_extra import parse_extra_pkg_info
 from ozi.spec import METADATA
 from ozi.tap import TAP
 
+if TYPE_CHECKING:
+    from email.message import Message
+
 
 def render_requirements(target: Path) -> str:
     """Render requirements.in as it would appear in PKG-INFO"""
     requirements = (
         r.partition('\u0023')[0]
         for r in filter(
             lambda r: not (r.startswith('\u0023') or r == '\n'),
```

### Comparing `OZI-1.7.4/ozi/fix/parser.py` & `OZI-1.8.0/ozi/fix/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/fix/rewrite_command.py` & `OZI-1.8.0/ozi/fix/rewrite_command.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/lint/meson.build` & `OZI-1.8.0/ozi/lint/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/lint/pyright/meson.build` & `OZI-1.8.0/ozi/lint/pyright/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/meson.build` & `OZI-1.8.0/ozi/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/meson.py` & `OZI-1.8.0/ozi/meson.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/new/__main__.py` & `OZI-1.8.0/ozi/new/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/new/meson.build` & `OZI-1.8.0/ozi/new/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/new/parser.py` & `OZI-1.8.0/ozi/new/parser.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/new/validate.py` & `OZI-1.8.0/ozi/new/validate.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/pkg_extra.py` & `OZI-1.8.0/ozi/pkg_extra.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # ozi/pkg_extra.py
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 """Extra packaging metadata used by OZI."""
+from __future__ import annotations
+
 from email.message import Message
 from typing import Any
 
 from pyparsing import CaselessKeyword
 from pyparsing import Combine
 from pyparsing import Forward
 from pyparsing import Keyword
```

### Comparing `OZI-1.7.4/ozi/render.py` & `OZI-1.8.0/ozi/render.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/scripts/core_metadata_template.py` & `OZI-1.8.0/ozi/scripts/core_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/scripts/meson.build` & `OZI-1.8.0/ozi/scripts/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/scripts/meson_dist_setuptools_scm.py` & `OZI-1.8.0/ozi/scripts/meson_dist_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/scripts/meson_setuptools_scm.py` & `OZI-1.8.0/ozi/scripts/meson_setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/scripts/render_requirements.py` & `OZI-1.8.0/ozi/scripts/render_requirements.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/scripts/replace_ruff_target_version.py` & `OZI-1.8.0/ozi/scripts/replace_ruff_target_version.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/scripts/scm_version_snip.py` & `OZI-1.8.0/ozi/scripts/scm_version_snip.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/scripts/to_distribution_template.py` & `OZI-1.8.0/ozi/scripts/to_distribution_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/scripts/version_metadata_template.py` & `OZI-1.8.0/ozi/scripts/version_metadata_template.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/spdx.py` & `OZI-1.8.0/ozi/spdx.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/spec/_license.py` & `OZI-1.8.0/ozi/spec/_license.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/spec/_spec.py` & `OZI-1.8.0/ozi/spec/_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return str(get_version(root='..', relative_to=__file__))
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Spec(Default):
     """OZI Specification metadata."""
 
-    version: str = '0.3'
+    version: str = '0.4'
     python: PythonProject = ClassicProject()
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Experimental(Default):
     """Experimental OZI specifications."""
```

### Comparing `OZI-1.7.4/ozi/spec/base.py` & `OZI-1.8.0/ozi/spec/base.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/spec/ci.py` & `OZI-1.8.0/ozi/spec/ci.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 # ozi/spec/ci.py
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 """Continuous integration specification."""
+from __future__ import annotations
 
 from collections.abc import Mapping  # noqa: TCH003,TC003,RUF100
 from dataclasses import dataclass
 from dataclasses import field
 
 from ozi.spec.base import Default
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Publish(Default):
     """Publishing patterns for packaged project."""
 
     include: tuple[str, ...] = ('*.tar.gz', '*.whl', 'sig/*')
-    version: str = '0.1.1'
+    version: str = '0.1.2'
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Draft(Default):
     """Draft release patterns for packaged project."""
 
-    version: str = '0.1.1'
+    version: str = '0.1.2'
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Release(Default):
     """Release patterns for packaged project."""
 
-    version: str = '0.4.0'
+    version: str = '0.4.1'
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class Checkpoint(Default):
     """Checkpoint suites to run."""
 
     suites: tuple[str, ...] = ('dist', 'lint', 'test')
-    version: str = '0.1.6'
+    version: str = '0.2.0'
 
 
 @dataclass(kw_only=True, frozen=True, eq=True)
 class CheckpointSuite(Default):
     """OZI checkpoint base class."""
 
     exclude: tuple[str, ...] = field(default_factory=tuple)
@@ -109,15 +110,15 @@
         default_factory=lambda: {
             'bandit': 'bandit[toml]',
             'black': 'black>=24.3',
             'flake8': 'flake8',
             'isort': 'isort',
             'mypy': 'mypy',
             'pyright': 'pyright',
-            'readme-renderer': 'readme-renderer',
+            'readme-renderer': 'readme-renderer[md]',
         },
     )
     plugin: Mapping[str, str] = field(
         default_factory=lambda: {
             'Flake8-pyproject': 'Flake8-pyproject',
             'flake8-annotations': 'flake8-annotations',
             'flake8-broken-line': 'flake8-broken-line',
@@ -177,20 +178,18 @@
 @dataclass(slots=True, frozen=True, eq=True)
 class Build(Default):
     """Build backend and required packages for OZI."""
 
     backend: str = 'ozi_build.buildapi'
     requires: Mapping[str, str] = field(
         default_factory=lambda: {
-            'OZI.build': 'OZI.build>=0.0.15',
-            'meson': 'meson[ninja]>=1.1.0',
+            'OZI.build': 'OZI.build>=0.0.18',
             'pip-tools': 'pip-tools>=7',
-            'setuptools': 'setuptools>=64',
-            'setuptools_scm': 'setuptools_scm>=8.0',
-            'tomli': 'tomli>=2.0.0;python_version<"3.11"',
+            'pipx': 'pipx~=1.5',
+            'setuptools_scm': 'setuptools_scm[toml]~=8.0',
         },
     )
 
 
 @dataclass(slots=True, frozen=True, eq=True)
 class CI(Default):
     """Provider-agnostic CI information."""
```

### Comparing `OZI-1.7.4/ozi/spec/meson.build` & `OZI-1.8.0/ozi/spec/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/spec/pkg.py` & `OZI-1.8.0/ozi/spec/pkg.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/spec/project.py` & `OZI-1.8.0/ozi/spec/project.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/spec/python.py` & `OZI-1.8.0/ozi/spec/python.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/spec/src.py` & `OZI-1.8.0/ozi/spec/src.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/tap.py` & `OZI-1.8.0/ozi/tap.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/trove.py` & `OZI-1.8.0/ozi/trove.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/vendor/email_validator/__init__.py` & `OZI-1.8.0/ozi/vendor/email_validator/__init__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/vendor/email_validator/__main__.py` & `OZI-1.8.0/ozi/vendor/email_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/vendor/email_validator/deliverability.py` & `OZI-1.8.0/ozi/vendor/email_validator/deliverability.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/vendor/email_validator/exceptions_types.py` & `OZI-1.8.0/ozi/vendor/email_validator/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/vendor/email_validator/meson.build` & `OZI-1.8.0/ozi/vendor/email_validator/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/vendor/email_validator/rfc_constants.py` & `OZI-1.8.0/ozi/vendor/email_validator/rfc_constants.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/vendor/email_validator/syntax.py` & `OZI-1.8.0/ozi/vendor/email_validator/syntax.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/vendor/email_validator/validate_email.py` & `OZI-1.8.0/ozi/vendor/email_validator/validate_email.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/ozi/vendor/meson.build` & `OZI-1.8.0/ozi/vendor/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/pyproject.toml` & `OZI-1.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,44 +2,29 @@
 # Part of the OZI Project, under the Apache License v2.0 with LLVM Exceptions.
 # See LICENSE.txt for license information.
 # SPDX-License-Identifier: Apache-2.0 WITH LLVM-exception
 [build-system]
 build-backend = "ozi_build.buildapi"
 requires      = [
     "OZI.build>=0.0.18",
-    "meson[ninja]>=1.1.0",
     "pip-tools>=7",
-    "setuptools>=64",
-    "setuptools_scm>=8.0",
-    'tomli>=2.0.0;python_version<"3.11"',
+    "pipx~=1.5",
+    "setuptools_scm[toml]~=8.0",
 ]
 
 [tool.ozi-build.entry-points]
 console_scripts = [
     "ozi = ozi.__main__:main",
     "ozi-new = ozi.new.__main__:main",
     "ozi-fix = ozi.fix.__main__:main",
 ]
 
 [tool.ozi-build.metadata]
-summary = 'Packager for Python projects using Meson.'
 pkg-info-file = 'PKG-INFO'
 
-[tool.cibuildwheel]
-build-frontend = "build"
-before-build = [
-     "pip install --upgrade pip",
-     "pip install --upgrade build",
-     "pip install --upgrade sigstore",
-     "pip install --upgrade meson[ninja]>=1.1.0",
-     "pip install --upgrade OZI.build",
-     "pip install --upgrade setuptools_scm",
-     "pip install --upgrade pip-tools",
-]
-
 [tool.setuptools_scm]
 version_file_template = """
 Metadata-Version: 2.1
 Name: @PROJECT_NAME@
 Version: @SCM_VERSION@
 Summary: Package Python projects with Meson.
 Download-URL: https://github.com/rjdbcm/OZI/archive/refs/tags/@SCM_VERSION@.tar.gz
@@ -79,16 +64,14 @@
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.in"] }
 
 [project]
 dynamic = ["dependencies", "version"]
 license = {file = "LICENSE.txt"}
-readme = "README.rst"
-requires-python = ">=3.10, <3.13"
 
 [project.optional_dependencies] # also meson test suite names
 # continuous integration
 ci   = ["tox>4", "tox-gh>1.2"]
 # tox -e fix
 fix  = ["black", "ruff>=0.1.6", "autoflake", "isort"]
 # Default meson test setup
@@ -321,14 +304,19 @@
 prerelease = false
 
 [tool.semantic_release.branches."release/1.7"]
 match = "release/1.7"
 prerelease_token = "alpha"
 prerelease = false
 
+[tool.semantic_release.branches."release/1.8"]
+match = "release/1.8"
+prerelease_token = "alpha"
+prerelease = false
+
 [tool.semantic_release.commit_parser_options]
 major_tags = [":boom:"]
 minor_tags = [
     ":sparkles:",
 ]
 patch_tags = [
     ":adhesive_bandage:",
@@ -400,55 +388,57 @@
 [gh]
 python =
      3.12 = dist,lint,test
      3.11 = dist,lint,test
      3.10 = dist,lint,test
 
 [testenv]
-allowlist_externals = rm
+allowlist_externals = 
+    rm
+    pipx
+    meson
+    python
 package = wheel
 deps =
-     meson >= 1.1.0
-     ninja >= 1.8.2
-     pip-tools
-     setuptools_scm[toml]
-     tomli >= 2.0.0
      -r requirements.in
+     virtualenv
 commands =
      meson compile -C {env_tmp_dir}
      rm -rf {env_tmp_dir}/.gitignore
 
 [testenv:dist]
 description = OZI distribution checkpoint
-commands_pre = meson setup {env_tmp_dir} -Ddist=enabled
+commands_pre =
+    pipx install --python=python meson
+    meson setup {env_tmp_dir} -Ddist=enabled -Dtox-env-dir={env_dir}
 commands_post = meson test --no-rebuild --maxfail=1 -C {env_tmp_dir} --setup=dist
 
 [testenv:lint]
 description = OZI format/lint checkpoint
-commands_pre = meson setup {env_tmp_dir} -Dlint=enabled
+commands_pre =
+    pipx install --python=python meson
+    meson setup {env_tmp_dir} -Dlint=enabled -Dtox-env-dir={env_dir}
 commands_post = meson test --no-rebuild --maxfail=1 -C {env_tmp_dir} --setup=lint
 
 [testenv:test]
 description = OZI unit tests checkpoint
-commands_pre = meson setup {env_tmp_dir} -Dtest=enabled -Dozi-blastpipe=enabled
+commands_pre =
+    pipx install --python=python meson
+    meson setup {env_tmp_dir} -Dtest=enabled -Dozi-blastpipe=enabled -Dtox-env-dir={env_dir}
 commands_post = meson test --no-rebuild --maxfail=1 -C {env_tmp_dir} --setup=test
 
 [testenv:fix]
 description = OZI project fix issues utility (black, isort, autoflake, ruff)
-deps = 
-     black>=24.3
-     isort
-     autoflake
-     ruff
+deps = pipx
 skip_install = true
 commands =
-     {env_python} -m black -S .
-     {env_python} -m isort .
-     {env_python} -m autoflake -i -r .
-     {env_python} -m ruff check ozi --fix
+     pipx run --python {env_python} black -S .
+     pipx run --python {env_python} isort .
+     pipx run --python {env_python} autoflake -i -r .
+     pipx run --python {env_python} ruff check ozi --fix
 
 [testenv:scm]
 description = OZI supply chain management (setuptools_scm)
 deps =
      setuptools_scm[toml]>=8
 commands =
      {env_python} -m setuptools_scm {posargs}
```

### Comparing `OZI-1.7.4/templates/CHANGELOG.md.j2` & `OZI-1.8.0/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/tests/meson.build` & `OZI-1.8.0/tests/meson.build`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/tests/test_ozi_fix.py` & `OZI-1.8.0/tests/test_ozi_fix.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/tests/test_ozi_new.py` & `OZI-1.8.0/tests/test_ozi_new.py`

 * *Files identical despite different names*

### Comparing `OZI-1.7.4/tests/test_tap.py` & `OZI-1.8.0/tests/test_tap.py`

 * *Files identical despite different names*

