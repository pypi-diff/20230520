# Comparing `tmp/ansible-navigator-3.3.0.tar.gz` & `tmp/ansible-navigator-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-navigator-3.3.0.tar", last modified: Tue May 16 14:53:23 2023, max compression
+gzip compressed data, was "ansible-navigator-3.3.1.tar", last modified: Sat May 20 12:59:14 2023, max compression
```

## Comparing `ansible-navigator-3.3.0.tar` & `ansible-navigator-3.3.1.tar`

### file list

```diff
@@ -1,251 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.637551 ansible-navigator-3.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.605551 ansible-navigator-3.3.0/.config/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/documentation_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/chronographer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.prettierrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-16 14:53:23.633551 ansible-navigator-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/docs/.generated/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/.generated/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/_ext/regenerate_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/contributing/code-of-conduct.md
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/contributing/guidelines.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/contributing/security.md
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/settings.md
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/subcommands.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.613551 ansible-navigator-3.3.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.asottile_tm_tokenize.all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.dark_vs.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.source.json.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.source.shell.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.source.yaml.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.text.html.basic.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.text.html.derivative.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.text.html.markdown.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.text.log.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:53:23.637551 ansible-navigator-3.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.601551 ansible-navigator-3.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.613551 ansible-navigator-3.3.0/src/ansible_navigator/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/_version_doc_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/action_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/action_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/action_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.621551 ansible-navigator-3.3.0/src/ansible_navigator/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/back.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/help_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/open_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/quit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    36365 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/serialize_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/serialize_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/app_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.621551 ansible-navigator-3.3.0/src/ansible_navigator/command_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/command_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/command_runner/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.621551 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py
--rw-r--r--   0 runner    (1001) docker     (123)    31712 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    48249 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/content_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.621551 ansible-navigator-3.3.0/src/ansible_navigator/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/ansible-navigator.json
--rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/catalog_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.625551 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/html.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/log.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.json.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.shell.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.yaml.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.basic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.derivative.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.markdown.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.log.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/help.md
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/image_introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/images_dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/settings-sample.template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/settings-schema.partial.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.625551 ansible-navigator-3.3.0/src/ansible_navigator/data/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/themes/dark_vs.json
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/themes/terminal_colors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/welcome.md
--rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.625551 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/introspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/puller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.625551 ansible-navigator-3.3.0/src/ansible_navigator/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/command_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.629551 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/fchainmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/grammars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/reg.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.633551 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/curses_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/curses_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_curses_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_working.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_button.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/menu_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/sentinels.py
--rw-r--r--   0 runner    (1001) docker     (123)    33458 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.633551 ansible-navigator-3.3.0/src/ansible_navigator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/dict_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/dot_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/packaged_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/print.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.633551 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.613551 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.421589 ansible-navigator-3.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.373587 ansible-navigator-3.3.1/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.377587 ansible-navigator-3.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.377587 ansible-navigator-3.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/ISSUE_TEMPLATE/documentation_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/chronographer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.377587 ansible-navigator-3.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.377587 ansible-navigator-3.3.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-20 12:59:14.421589 ansible-navigator-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.377587 ansible-navigator-3.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.377587 ansible-navigator-3.3.1/docs/.generated/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/.generated/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.377587 ansible-navigator-3.3.1/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/_ext/regenerate_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.377587 ansible-navigator-3.3.1/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/contributing/code-of-conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/contributing/guidelines.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.377587 ansible-navigator-3.3.1/docs/contributing/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    55005 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/contributing/images/test_tree_view.png
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/contributing/security.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/settings.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/docs/subcommands.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.381587 ansible-navigator-3.3.1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/licenses/LICENSE.asottile_tm_tokenize.all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/licenses/LICENSE.dark_vs.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/licenses/LICENSE.source.json.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/licenses/LICENSE.source.shell.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/licenses/LICENSE.source.yaml.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/licenses/LICENSE.text.html.basic.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/licenses/LICENSE.text.html.derivative.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/licenses/LICENSE.text.html.markdown.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/licenses/LICENSE.text.log.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    17945 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 12:59:14.421589 ansible-navigator-3.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.369587 ansible-navigator-3.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.381587 ansible-navigator-3.3.1/src/ansible_navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 12:59:14.000000 ansible-navigator-3.3.1/src/ansible_navigator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/_version_doc_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/action_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/action_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/action_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.397588 ansible-navigator-3.3.1/src/ansible_navigator/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/back.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/help_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/quit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36365 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/sample_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/sample_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/sample_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/serialize_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/serialize_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/actions/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/app_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.397588 ansible-navigator-3.3.1/src/ansible_navigator/command_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/command_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/command_runner/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.397588 ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/defs_presentable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31712 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48249 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/content_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.401588 ansible-navigator-3.3.1/src/ansible_navigator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/ansible-navigator.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23668 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/catalog_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.405588 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/html.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/log.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/source.json.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/source.shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/source.yaml.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/text.html.basic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/text.html.derivative.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/text.html.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/text.log.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/help.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/image_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/images_dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/settings-sample.template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/settings-schema.partial.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.405588 ansible-navigator-3.3.1/src/ansible_navigator/data/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/themes/dark_vs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/themes/terminal_colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/data/welcome.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.405588 ansible-navigator-3.3.1/src/ansible_navigator/image_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/image_manager/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/image_manager/introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/image_manager/introspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/image_manager/puller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.405588 ansible-navigator-3.3.1/src/ansible_navigator/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/runner/ansible_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/runner/ansible_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/runner/ansible_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8697 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/runner/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/runner/command_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/runner/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.409589 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/fchainmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/grammars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.417589 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/curses_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/curses_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_curses_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_handler_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_handler_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_handler_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_handler_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_handler_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/menu_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/sentinels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33458 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/ui_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/ui_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.417589 ansible-navigator-3.3.1/src/ansible_navigator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/dict_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/dot_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/packaged_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.421589 ansible-navigator-3.3.1/src/ansible_navigator/utils/version_migration/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/version_migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/version_migration/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/version_migration/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/version_migration/settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/src/ansible_navigator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 12:59:14.389588 ansible-navigator-3.3.1/src/ansible_navigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-20 12:59:14.000000 ansible-navigator-3.3.1/src/ansible_navigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-05-20 12:59:14.000000 ansible-navigator-3.3.1/src/ansible_navigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 12:59:14.000000 ansible-navigator-3.3.1/src/ansible_navigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-20 12:59:14.000000 ansible-navigator-3.3.1/src/ansible_navigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-20 12:59:14.000000 ansible-navigator-3.3.1/src/ansible_navigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 12:59:14.000000 ansible-navigator-3.3.1/src/ansible_navigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-20 12:58:50.000000 ansible-navigator-3.3.1/tox.ini
```

### Comparing `ansible-navigator-3.3.0/.config/dictionary.txt` & `ansible-navigator-3.3.1/.config/dictionary.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,49 +42,49 @@
 00000290: 780a 6b65 6765 7865 730a 6c65 6e74 6578  x.kegexes.lentex
 000002a0: 740a 6c65 7665 6c6e 616d 650a 6c69 626f  t.levelname.libo
 000002b0: 6e69 670a 6c69 6768 7462 756c 6273 0a6c  nig.lightbulbs.l
 000002c0: 696e 656e 756d 730a 6c69 6e6b 6368 6563  inenums.linkchec
 000002d0: 6b0a 6c69 6e74 6162 6c65 0a6c 696e 7461  k.lintable.linta
 000002e0: 626c 6573 0a6d 6167 6963 6c69 6e6b 0a6d  bles.magiclink.m
 000002f0: 6173 6b61 626c 6573 0a6d 6178 7370 6c69  askables.maxspli
-00000300: 740a 6d6b 646f 6373 7472 696e 6773 0a6d  t.mkdocstrings.m
-00000310: 6f64 756c 6561 7574 686f 720a 6d71 7565  oduleauthor.mque
-00000320: 7565 2020 2020 2020 2020 2020 2020 2020  ue              
-00000330: 2320 6874 7470 733a 2f2f 6769 7468 7562  # https://github
-00000340: 2e63 6f6d 2f61 6e73 6962 6c65 2f61 6e73  .com/ansible/ans
-00000350: 6962 6c65 2d72 756e 6e65 722f 6973 7375  ible-runner/issu
-00000360: 6573 2f39 3834 0a6d 7970 726f 6a65 6374  es/984.myproject
-00000370: 0a6e 6574 636f 6d6d 6f6e 2020 2020 2020  .netcommon      
-00000380: 2020 2020 2023 2041 6e73 6962 6c65 206e       # Ansible n
-00000390: 6574 776f 726b 2063 6f6c 6c65 6374 696f  etwork collectio
-000003a0: 6e2c 2073 6565 6e20 696e 2074 6573 7473  n, seen in tests
-000003b0: 2061 6e64 2052 4541 444d 450a 6e65 7463   and README.netc
-000003c0: 6f6e 660a 6e69 7470 6963 6b79 0a6e 6f6e  onf.nitpicky.non
-000003d0: 626c 6f63 6b69 6e67 0a6f 6c64 6d61 736b  blocking.oldmask
-000003e0: 0a6f 6e65 6c69 6e65 0a6f 6e69 6775 7275  .oneline.oniguru
-000003f0: 6d61 6366 6669 0a6f 7065 6e73 6561 7263  macffi.opensearc
-00000400: 680a 6f78 666f 7264 636f 6d6d 610a 7061  h.oxfordcomma.pa
-00000410: 6765 7669 6577 0a70 7265 636c 6561 720a  geview.preclear.
-00000420: 7072 6563 6f6d 6d61 6e64 0a70 7265 6d61  precommand.prema
-00000430: 6e65 6e74 0a70 756c 6c61 626c 650a 7079  nent.pullable.py
-00000440: 6d64 6f77 6e0a 7079 6d64 6f77 6e78 0a72  mdown.pymdownx.r
-00000450: 6564 6861 7469 6e73 6967 6874 730a 7265  edhatinsights.re
-00000460: 7072 6573 656e 7465 720a 7265 7475 726e  presenter.return
-00000470: 646f 6373 0a72 756e 7469 6d65 730a 7363  docs.runtimes.sc
-00000480: 726f 6c6c 6261 636b 0a73 6563 7469 6f6e  rollback.section
-00000490: 6175 7468 6f72 0a73 6574 7570 746f 6f6c  author.setuptool
-000004a0: 7320 2020 2020 2020 2020 2023 2055 7365  s          # Use
-000004b0: 6420 696e 205f 7665 7273 696f 6e2e 7079  d in _version.py
-000004c0: 690a 736d 6172 7471 756f 7465 730a 736f  i.smartquotes.so
-000004d0: 6d65 7661 6c75 650a 7374 6174 656d 6163  mevalue.statemac
-000004e0: 6869 6e65 0a73 7472 6970 7370 6163 6573  hine.stripspaces
-000004f0: 0a73 7562 6163 7469 6f6e 0a73 7562 7363  .subaction.subsc
-00000500: 6865 6d61 0a73 7570 6572 6665 6e63 6573  hema.superfences
-00000510: 0a74 656d 706c 6174 6162 6c65 0a74 656d  .templatable.tem
-00000520: 706c 6174 6564 0a74 656d 706c 6174 696e  plated.templatin
-00000530: 670a 7465 7374 686f 7374 0a74 6573 746e  g.testhost.testn
-00000540: 616d 650a 746f 7062 6172 0a74 7261 6365  ame.topbar.trace
-00000550: 6261 636b 730a 7472 7565 636f 6c6f 720a  backs.truecolor.
-00000560: 7573 6566 6978 7475 7265 730a 7573 6572  usefixtures.user
-00000570: 6261 7365 0a76 6965 7763 6f64 650a 766f  base.viewcode.vo
-00000580: 6c6d 6f75 6e74 0a77 6f72 6b64 6972 0a78  lmount.workdir.x
-00000590: 6d73 730a                                mss.
+00000300: 740a 6d6b 646f 6373 0a6d 6b64 6f63 7374  t.mkdocs.mkdocst
+00000310: 7269 6e67 730a 6d6f 6475 6c65 6175 7468  rings.moduleauth
+00000320: 6f72 0a6d 7175 6575 6520 2020 2020 2020  or.mqueue       
+00000330: 2020 2020 2020 2023 2068 7474 7073 3a2f         # https:/
+00000340: 2f67 6974 6875 622e 636f 6d2f 616e 7369  /github.com/ansi
+00000350: 626c 652f 616e 7369 626c 652d 7275 6e6e  ble/ansible-runn
+00000360: 6572 2f69 7373 7565 732f 3938 340a 6d79  er/issues/984.my
+00000370: 7072 6f6a 6563 740a 6e65 7463 6f6d 6d6f  project.netcommo
+00000380: 6e20 2020 2020 2020 2020 2020 2320 416e  n           # An
+00000390: 7369 626c 6520 6e65 7477 6f72 6b20 636f  sible network co
+000003a0: 6c6c 6563 7469 6f6e 2c20 7365 656e 2069  llection, seen i
+000003b0: 6e20 7465 7374 7320 616e 6420 5245 4144  n tests and READ
+000003c0: 4d45 0a6e 6574 636f 6e66 0a6e 6974 7069  ME.netconf.nitpi
+000003d0: 636b 790a 6e6f 6e62 6c6f 636b 696e 670a  cky.nonblocking.
+000003e0: 6f6c 646d 6173 6b0a 6f6e 656c 696e 650a  oldmask.oneline.
+000003f0: 6f6e 6967 7572 756d 6163 6666 690a 6f70  onigurumacffi.op
+00000400: 656e 7365 6172 6368 0a6f 7866 6f72 6463  ensearch.oxfordc
+00000410: 6f6d 6d61 0a70 6167 6576 6965 770a 7072  omma.pageview.pr
+00000420: 6563 6c65 6172 0a70 7265 636f 6d6d 616e  eclear.precomman
+00000430: 640a 7072 656d 616e 656e 740a 7075 6c6c  d.premanent.pull
+00000440: 6162 6c65 0a70 796d 646f 776e 0a70 796d  able.pymdown.pym
+00000450: 646f 776e 780a 7265 6468 6174 696e 7369  downx.redhatinsi
+00000460: 6768 7473 0a72 6570 7265 7365 6e74 6572  ghts.representer
+00000470: 0a72 6574 7572 6e64 6f63 730a 7275 6e74  .returndocs.runt
+00000480: 696d 6573 0a73 6372 6f6c 6c62 6163 6b0a  imes.scrollback.
+00000490: 7365 6374 696f 6e61 7574 686f 720a 7365  sectionauthor.se
+000004a0: 7475 7074 6f6f 6c73 2020 2020 2020 2020  tuptools        
+000004b0: 2020 2320 5573 6564 2069 6e20 5f76 6572    # Used in _ver
+000004c0: 7369 6f6e 2e70 7969 0a73 6d61 7274 7175  sion.pyi.smartqu
+000004d0: 6f74 6573 0a73 6f6d 6576 616c 7565 0a73  otes.somevalue.s
+000004e0: 7461 7465 6d61 6368 696e 650a 7374 7269  tatemachine.stri
+000004f0: 7073 7061 6365 730a 7375 6261 6374 696f  pspaces.subactio
+00000500: 6e0a 7375 6273 6368 656d 610a 7375 7065  n.subschema.supe
+00000510: 7266 656e 6365 730a 7465 6d70 6c61 7461  rfences.templata
+00000520: 626c 650a 7465 6d70 6c61 7465 640a 7465  ble.templated.te
+00000530: 6d70 6c61 7469 6e67 0a74 6573 7468 6f73  mplating.testhos
+00000540: 740a 7465 7374 6e61 6d65 0a74 6f70 6261  t.testname.topba
+00000550: 720a 7472 6163 6562 6163 6b73 0a74 7275  r.tracebacks.tru
+00000560: 6563 6f6c 6f72 0a75 7365 6669 7874 7572  ecolor.usefixtur
+00000570: 6573 0a75 7365 7262 6173 650a 7669 6577  es.userbase.view
+00000580: 636f 6465 0a76 6f6c 6d6f 756e 740a 776f  code.volmount.wo
+00000590: 726b 6469 720a 786d 7373 0a              rkdir.xmss.
```

### Comparing `ansible-navigator-3.3.0/.flake8` & `ansible-navigator-3.3.1/.flake8`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/.git_archival.txt` & `ansible-navigator-3.3.1/.git_archival.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/.github/CONTRIBUTING.md` & `ansible-navigator-3.3.1/.github/CONTRIBUTING.md`

 * *Files 16% similar despite different names*

```diff
@@ -62,26 +62,59 @@
     Because the version of python is pinned to a specific version to ensure the
     outcome of running `tox -e lint` locally is the same as `tox -e lint` being run
     by github actions, you may see the following error: `RuntimeError: failed to
     find interpreter for Builtin discover of python_spec='python3.XX'`. This
     indicates the version of python that needs to be installed for tox to run
     locally. In this case, the version of python that needs to be installed is
 
-## Debugging Ansible Navigator with VS Code
+## Getting started with Ansible Navigator
 
-Getting started:
+### Building from the source and installing packages for testing
 
-After cloning the repository, all we need is to install ansible-navigator from
-the source. Use the following command in workspace (root folder of navigator).
-This will install all the required dependencies for testing the local changes.
+After cloning the repository, create and activate a new [virtual environment] in
+the root of the repository. Once that is done all we need is to install
+ansible-navigator from the source. Use the following command in workspace (root
+folder of navigator).This will install package in editable/development mode,
+along with its additional dependencies required for testing.
 
 ```shell-session
-pip install -e .
+pip install -e .\[test]
 ```
 
+[virtual environment]: https://docs.python.org/3/library/venv.html
+
+### Testing process and examples
+
+Once all the dependencies are installed, we can execute our tests using
+[pytest]. To run tests inside a file test_xyz.py, we will need to traverse to
+that file.
+
+[pytest]: https://docs.pytest.org/en/7.3.x/
+
+Example: To run an unit test "test_circular_imports.py", we will execute:
+
+`pytest tests/unit/test_circular_imports.py`
+
+Example: To run an integration test "test_stdout_vault.py ", we will execute:
+
+`pytest tests/integration/actions/exec/test_stdout_vault.py`
+
+and so on ...
+
+Additionally, leverage the ability of VSCode test tree to run and debug tests in
+a more easier and interactive way. There is a dedicated configuration provided
+inside launch.json named as **Debug tests** to interactively debug the tests
+through VSCode test tree.
+
+Hover to the **Testing** icon in the Activity Bar to see VSCode test tree. From
+there expand and reach to the desired unit or integration test and hit
+`Run Test` or `Debug Test` appropriately.
+
+![VSCode test tree](images/test_tree_view.png)
+
 ### Configure VSCode settings
 
 Once we are inside vscode with project installed, we should see a `.vscode`
 folder in our workspace. Having a launch configuration file is beneficial
 because it allow us to configure and save debugging setup details. VS Code keeps
 debugging configuration information in a `launch.json` file located in a
 `.vscode` folder in our workspace (project root folder).
@@ -103,15 +136,15 @@
 
 ### Debug Ansible-Navigator Subcommands
 
 Ansible-Navigator comes in with bunch of [sub-commands]. To debug around any
 specific subcommand, we will need to add `args` attribute (arguments passed to
 the program to debug) in our launch.json configuration file.
 
-[sub-commands]: https://ansible-navigator.readthedocs.io/en/latest/subcommands/
+[sub-commands]: https://ansible-navigator.readthedocs.io/subcommands/
 
 **Example:**
 
 - Debug `ansible-navigator run` subcommand, use _args_ attribute, provide
   absolute path to the playbook as mentioned. Following configuration will allow
   to debug `ansible-navigator site.yml --mode stdout`.
```

### Comparing `ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ansible-navigator-3.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/.github/SECURITY.md` & `ansible-navigator-3.3.1/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/.github/dependabot.yml` & `ansible-navigator-3.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/.github/workflows/release.yml` & `ansible-navigator-3.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/.github/workflows/tox.yml` & `ansible-navigator-3.3.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/.gitignore` & `ansible-navigator-3.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/.pre-commit-config.yaml` & `ansible-navigator-3.3.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 ---
 default_language_version:
   # ensures that we get same behavior on CI(s) as on local machines
   python: python3.11
+exclude: >
+  (?x)^(
+    _readthedocs|
+    .tox
+  )$
 repos:
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         # Original hook implementation is flaky due to *several* bugs described
         # in https://github.com/prettier/prettier/issues/12364
@@ -160,19 +165,20 @@
     hooks:
       - id: pylint
         args:
           - docs/
           - src/
           - tests/
         additional_dependencies:
-          - dill>=0.3.6 # needed for py311
           - ansible-core
-          - astroid
           - ansible-runner
+          - astroid
+          - dill>=0.3.6 # needed for py311
           - jinja2
           - jsonschema
           - libtmux
+          - mkdocs-gen-files
           - onigurumacffi
           - pytest
           - pytest-mock
           - setuptools-scm
         pass_filenames: false
```

### Comparing `ansible-navigator-3.3.0/.prettierignore` & `ansible-navigator-3.3.1/.prettierignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/.vscode/launch.json` & `ansible-navigator-3.3.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/.vscode/settings.json` & `ansible-navigator-3.3.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/LICENSE` & `ansible-navigator-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/PKG-INFO` & `ansible-navigator-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.3.0
+Version: 3.3.1
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
```

### Comparing `ansible-navigator-3.3.0/README.md` & `ansible-navigator-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/cspell.config.yaml` & `ansible-navigator-3.3.1/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/docs/_ext/regenerate_docs.py` & `ansible-navigator-3.3.1/docs/_ext/regenerate_docs.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import logging
 
 from copy import copy
 from pathlib import Path
 from re import match
 
+import mkdocs_gen_files
+
 from ansible_navigator.configuration_subsystem import Constants as C
 from ansible_navigator.configuration_subsystem import NavigatorConfiguration
 from ansible_navigator.configuration_subsystem.definitions import SettingsEntry
 from ansible_navigator.utils.functions import oxfordcomma
 from ansible_navigator.version import __version__
 
 
@@ -180,14 +182,15 @@
         else:
             sample_settings.append(line)
     sample_settings.append("```")
     result = "\n".join(sample_settings)
     return result
 
 
-if __name__ == "__main__":
-    with DOCS_SETTINGS_SAMPLE.open("w") as f:
-        f.write(md_settings_sample())
-    with DOCS_SETTINGS_DUMP.open("w") as f:
-        f.write(md_settings_dump())
-    with DOCS_SUBCOMMANDS_OVERVIEW.open("w") as f:
-        f.write(_subcommands_overview())
+with mkdocs_gen_files.open(DOCS_SETTINGS_SAMPLE, "w") as f:
+    f.write(md_settings_sample())
+
+with mkdocs_gen_files.open(DOCS_SETTINGS_DUMP, "w") as f:
+    f.write(md_settings_dump())
+
+with mkdocs_gen_files.open(DOCS_SUBCOMMANDS_OVERVIEW, "w") as f:
+    f.write(_subcommands_overview())
```

### Comparing `ansible-navigator-3.3.0/docs/contributing/guidelines.md` & `ansible-navigator-3.3.1/docs/contributing/guidelines.md`

 * *Files 16% similar despite different names*

```diff
@@ -62,26 +62,59 @@
     Because the version of python is pinned to a specific version to ensure the
     outcome of running `tox -e lint` locally is the same as `tox -e lint` being run
     by github actions, you may see the following error: `RuntimeError: failed to
     find interpreter for Builtin discover of python_spec='python3.XX'`. This
     indicates the version of python that needs to be installed for tox to run
     locally. In this case, the version of python that needs to be installed is
 
-## Debugging Ansible Navigator with VS Code
+## Getting started with Ansible Navigator
 
-Getting started:
+### Building from the source and installing packages for testing
 
-After cloning the repository, all we need is to install ansible-navigator from
-the source. Use the following command in workspace (root folder of navigator).
-This will install all the required dependencies for testing the local changes.
+After cloning the repository, create and activate a new [virtual environment] in
+the root of the repository. Once that is done all we need is to install
+ansible-navigator from the source. Use the following command in workspace (root
+folder of navigator).This will install package in editable/development mode,
+along with its additional dependencies required for testing.
 
 ```shell-session
-pip install -e .
+pip install -e .\[test]
 ```
 
+[virtual environment]: https://docs.python.org/3/library/venv.html
+
+### Testing process and examples
+
+Once all the dependencies are installed, we can execute our tests using
+[pytest]. To run tests inside a file test_xyz.py, we will need to traverse to
+that file.
+
+[pytest]: https://docs.pytest.org/en/7.3.x/
+
+Example: To run an unit test "test_circular_imports.py", we will execute:
+
+`pytest tests/unit/test_circular_imports.py`
+
+Example: To run an integration test "test_stdout_vault.py ", we will execute:
+
+`pytest tests/integration/actions/exec/test_stdout_vault.py`
+
+and so on ...
+
+Additionally, leverage the ability of VSCode test tree to run and debug tests in
+a more easier and interactive way. There is a dedicated configuration provided
+inside launch.json named as **Debug tests** to interactively debug the tests
+through VSCode test tree.
+
+Hover to the **Testing** icon in the Activity Bar to see VSCode test tree. From
+there expand and reach to the desired unit or integration test and hit
+`Run Test` or `Debug Test` appropriately.
+
+![VSCode test tree](images/test_tree_view.png)
+
 ### Configure VSCode settings
 
 Once we are inside vscode with project installed, we should see a `.vscode`
 folder in our workspace. Having a launch configuration file is beneficial
 because it allow us to configure and save debugging setup details. VS Code keeps
 debugging configuration information in a `launch.json` file located in a
 `.vscode` folder in our workspace (project root folder).
@@ -103,15 +136,15 @@
 
 ### Debug Ansible-Navigator Subcommands
 
 Ansible-Navigator comes in with bunch of [sub-commands]. To debug around any
 specific subcommand, we will need to add `args` attribute (arguments passed to
 the program to debug) in our launch.json configuration file.
 
-[sub-commands]: https://ansible-navigator.readthedocs.io/en/latest/subcommands/
+[sub-commands]: https://ansible-navigator.readthedocs.io/subcommands/
 
 **Example:**
 
 - Debug `ansible-navigator run` subcommand, use _args_ attribute, provide
   absolute path to the playbook as mentioned. Following configuration will allow
   to debug `ansible-navigator site.yml --mode stdout`.
```

### Comparing `ansible-navigator-3.3.0/docs/contributing/security.md` & `ansible-navigator-3.3.1/docs/contributing/security.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/docs/faq.md` & `ansible-navigator-3.3.1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/docs/index.md` & `ansible-navigator-3.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/docs/installation.md` & `ansible-navigator-3.3.1/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/docs/settings.md` & `ansible-navigator-3.3.1/docs/settings.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/docs/subcommands.md` & `ansible-navigator-3.3.1/docs/subcommands.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/licenses/LICENSE.asottile_tm_tokenize.all.txt` & `ansible-navigator-3.3.1/licenses/LICENSE.asottile_tm_tokenize.all.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/licenses/LICENSE.dark_vs.json.txt` & `ansible-navigator-3.3.1/licenses/LICENSE.dark_vs.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/licenses/LICENSE.source.json.json.txt` & `ansible-navigator-3.3.1/licenses/LICENSE.source.json.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/licenses/LICENSE.source.shell.json.txt` & `ansible-navigator-3.3.1/licenses/LICENSE.source.shell.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/licenses/LICENSE.source.yaml.json.txt` & `ansible-navigator-3.3.1/licenses/LICENSE.source.yaml.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/licenses/LICENSE.text.html.markdown.json.txt` & `ansible-navigator-3.3.1/licenses/LICENSE.text.html.markdown.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/licenses/LICENSE.text.log.json.txt` & `ansible-navigator-3.3.1/licenses/LICENSE.text.log.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/mkdocs.yml` & `ansible-navigator-3.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/mypy.ini` & `ansible-navigator-3.3.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/pyproject.toml` & `ansible-navigator-3.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,19 @@
 enable = [
   "useless-suppression", # Identify unneeded pylint disable statements
 
 ]
 
 [tool.pytest.ini_options]
 addopts = "-n=auto --dist=loadfile --maxfail=10 --durations=30 --showlocals"
+filterwarnings = [
+  "error",
+  # https://github.com/ansible/ansible-runner/issues/1246
+  "ignore::ResourceWarning:ansible_runner",
+]
 
 [tool.ruff]
 fix = true
 line-length = 100
 builtins = ["__"]
 select = ["ALL"]
 ignore = [
```

### Comparing `ansible-navigator-3.3.0/requirements.txt` & `ansible-navigator-3.3.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/_version_doc_cache.py` & `ansible-navigator-3.3.1/src/ansible_navigator/_version_doc_cache.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/action_base.py` & `ansible-navigator-3.3.1/src/ansible_navigator/action_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/action_defs.py` & `ansible-navigator-3.3.1/src/ansible_navigator/action_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/action_runner.py` & `ansible-navigator-3.3.1/src/ansible_navigator/action_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/__init__.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/_actions.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/_actions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/back.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/back.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/builder.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/collections.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/collections.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/config.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/doc.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/exec.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/exec.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/filter.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/filter.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/help_doc.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/help_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/images.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/images.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/inventory.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/lint.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/lint.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/log.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/log.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/open_file.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/open_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/quit.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/quit.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/refresh.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/refresh.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/rerun.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/rerun.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/run.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/run.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_form.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/sample_form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_notification.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/sample_notification.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_working.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/sample_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/save.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/save.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/select.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/select.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/serialize_json.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/serialize_json.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/serialize_yaml.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/serialize_yaml.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/settings.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/settings.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/stdout.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/stdout.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/template.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/template.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/welcome.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/welcome.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/actions/write_file.py` & `ansible-navigator-3.3.1/src/ansible_navigator/actions/write_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/app_public.py` & `ansible-navigator-3.3.1/src/ansible_navigator/app_public.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/cli.py` & `ansible-navigator-3.3.1/src/ansible_navigator/cli.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/command_runner/command_runner.py` & `ansible-navigator-3.3.1/src/ansible_navigator/command_runner/command_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/__init__.py` & `ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/configurator.py` & `ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/configurator.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/definitions.py` & `ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py` & `ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/defs_presentable.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py` & `ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/navigator_configuration.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py` & `ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/parser.py` & `ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/parser.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/transform.py` & `ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/transform.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/utils.py` & `ansible-navigator-3.3.1/src/ansible_navigator/configuration_subsystem/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/constants.py` & `ansible-navigator-3.3.1/src/ansible_navigator/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/content_defs.py` & `ansible-navigator-3.3.1/src/ansible_navigator/content_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/ansible-navigator.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/ansible-navigator.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/catalog_collections.py` & `ansible-navigator-3.3.1/src/ansible_navigator/data/catalog_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,16 @@
             if collection["known_as"] == "ansible.builtin":
                 plugin_dirs.append(Path(collection["path"], "modules"))
 
             for plugin_dir in plugin_dirs:
                 plugin_type = plugin_dir.name
                 if plugin_type == "modules":
                     plugin_type = "module"
-                filenames = plugin_dir.glob("**/*.py")
+                files = list(plugin_dir.glob("**/*.py")) + list(plugin_dir.glob("**/*.yml"))
+                filenames = (x for x in files)
                 self._process_plugin_dir(
                     plugin_type,
                     filenames,
                     file_checksums,
                     collection,
                 )
```

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/JSON.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/html.tmLanguage.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/html.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/log.tmLanguage.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/log.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/markdown.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.json.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/source.json.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.shell.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/source.shell.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.yaml.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/source.yaml.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.basic.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/text.html.basic.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.derivative.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/text.html.derivative.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.markdown.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/text.html.markdown.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.log.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/text.log.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/grammar/yaml.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/help.md` & `ansible-navigator-3.3.1/src/ansible_navigator/data/help.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/image_introspect.py` & `ansible-navigator-3.3.1/src/ansible_navigator/data/image_introspect.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/settings-sample.template.yml` & `ansible-navigator-3.3.1/src/ansible_navigator/data/settings-sample.template.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/settings-schema.partial.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/settings-schema.partial.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/themes/dark_vs.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/themes/dark_vs.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/themes/terminal_colors.json` & `ansible-navigator-3.3.1/src/ansible_navigator/data/themes/terminal_colors.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/data/welcome.md` & `ansible-navigator-3.3.1/src/ansible_navigator/data/welcome.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/diagnostics.py` & `ansible-navigator-3.3.1/src/ansible_navigator/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/image_manager/inspector.py` & `ansible-navigator-3.3.1/src/ansible_navigator/image_manager/inspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/image_manager/introspect.py` & `ansible-navigator-3.3.1/src/ansible_navigator/image_manager/introspect.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/image_manager/introspector.py` & `ansible-navigator-3.3.1/src/ansible_navigator/image_manager/introspector.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/image_manager/puller.py` & `ansible-navigator-3.3.1/src/ansible_navigator/image_manager/puller.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/initialization.py` & `ansible-navigator-3.3.1/src/ansible_navigator/initialization.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/logger.py` & `ansible-navigator-3.3.1/src/ansible_navigator/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_config.py` & `ansible-navigator-3.3.1/src/ansible_navigator/runner/ansible_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 """Herein lies the ability for ansible-runner to run the ansible-config command."""
 from __future__ import annotations
 
-from ansible_runner import get_ansible_config
+import warnings
+
+
+# Remove this catch-all once newer ansible-runner is released
+# https://github.com/ansible/ansible-runner/issues/1223
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore")
+    from ansible_runner import get_ansible_config
 
 from .base import Base
 
 
 class AnsibleConfig(Base):
     """Abstraction for ansible-config command-line."""
```

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_doc.py` & `ansible-navigator-3.3.1/src/ansible_navigator/runner/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_inventory.py` & `ansible-navigator-3.3.1/src/ansible_navigator/runner/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/runner/base.py` & `ansible-navigator-3.3.1/src/ansible_navigator/runner/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,22 @@
         self._rotate_artifacts = rotate_artifacts if isinstance(rotate_artifacts, int) else None
         self._timeout = timeout if isinstance(timeout, int) else None
         self.ansible_runner_instance: Runner
         self.cancelled: bool = False
         self.finished: bool = False
         self.status: str | None = None
         self._runner_args: dict = {}
+
+        # when the ce is podman, set the container user to root
+        if self._ce == "podman":
+            if container_options:
+                container_options.append("--user=root")
+            else:
+                container_options = ["--user=root"]
+
         if self._ee:
             self._runner_args.update(
                 {
                     "container_image": self._eei,
                     "process_isolation_executable": self._ce,
                     "process_isolation": True,
                     "container_volume_mounts": container_volume_mounts,
@@ -115,15 +123,19 @@
         if self._host_cwd:
             # ensure the CWD ends with a trailing slash
             host_cwd = os.path.join(self._host_cwd, "")
             self._runner_args["host_cwd"] = host_cwd
 
         if self._navigator_mode == "stdout":
             self._runner_args.update(
-                {"input_fd": sys.stdin, "output_fd": sys.stdout, "error_fd": sys.stderr},
+                {
+                    "input_fd": sys.stdin,
+                    "output_fd": sys.stdout,
+                    "error_fd": sys.stderr,
+                },
             )
 
     def __del__(self):
         """Drop the private_data_dir if it is temporary."""
         if (
             self._private_data_dir_is_tmp
             and self._private_data_dir
```

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/runner/command.py` & `ansible-navigator-3.3.1/src/ansible_navigator/runner/command.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/runner/command_async.py` & `ansible-navigator-3.3.1/src/ansible_navigator/runner/command_async.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/runner/command_base.py` & `ansible-navigator-3.3.1/src/ansible_navigator/runner/command_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/steps.py` & `ansible-navigator-3.3.1/src/ansible_navigator/steps.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/LICENSE` & `ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/compiler.py` & `ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/compiler.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/fchainmap.py` & `ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/fchainmap.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/grammars.py` & `ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/grammars.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/reg.py` & `ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/reg.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/rules.py` & `ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/rules.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/state.py` & `ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/state.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/tokenize.py` & `ansible-navigator-3.3.1/src/ansible_navigator/tm_tokenize/tokenize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/__init__.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/colorize.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/colorize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/curses_defs.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/curses_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/curses_window.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/curses_window.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_button.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_checks.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_curses_information.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_curses_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_information.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_option.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_option.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_radio.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_radio.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_text.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_working.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/field_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_button.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_handler_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_information.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_handler_information.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_options.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_handler_options.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_text.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_handler_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_working.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_handler_working.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_utils.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/form_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/menu_builder.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/menu_builder.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/sentinels.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/sentinels.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/ui.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui_config.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/ui_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui_constants.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/ui_constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/utils.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/utils.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/validators.py` & `ansible-navigator-3.3.1/src/ansible_navigator/ui_framework/validators.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/ansi.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/definitions.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/dict_merge.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/dict_merge.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/dot_paths.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/dot_paths.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/functions.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/functions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/json_schema.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/key_value_store.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/key_value_store.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/packaged_data.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/packaged_data.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/print.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/print.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/serialize.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/definitions.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/version_migration/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/migrate.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/version_migration/migrate.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/settings_file.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/version_migration/settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py` & `ansible-navigator-3.3.1/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator.egg-info/PKG-INFO` & `ansible-navigator-3.3.1/src/ansible_navigator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.3.0
+Version: 3.3.1
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
```

### Comparing `ansible-navigator-3.3.0/src/ansible_navigator.egg-info/SOURCES.txt` & `ansible-navigator-3.3.1/src/ansible_navigator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 docs/settings.md
 docs/subcommands.md
 docs/.generated/.gitignore
 docs/_ext/regenerate_docs.py
 docs/contributing/code-of-conduct.md
 docs/contributing/guidelines.md
 docs/contributing/security.md
+docs/contributing/images/test_tree_view.png
 licenses/LICENSE.asottile_tm_tokenize.all.txt
 licenses/LICENSE.dark_vs.json.txt
 licenses/LICENSE.source.json.json.txt
 licenses/LICENSE.source.shell.json.txt
 licenses/LICENSE.source.yaml.json.txt
 licenses/LICENSE.text.html.basic.json.txt
 licenses/LICENSE.text.html.derivative.json.txt
```

### Comparing `ansible-navigator-3.3.0/tox.ini` & `ansible-navigator-3.3.1/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 deps =
   --editable .[docs]
 description = Build The Docs
 # Intentionally not in alphabetical order due to execution order
 commands_pre =
   rm -rf .cache/plugin
 commands =
-  mkdocs build {posargs}
+  mkdocs build {posargs:--strict}
 isolated_build = true
 passenv =
   SSH_AUTH_SOCK
 skip_install = false
 usedevelop = true
```

