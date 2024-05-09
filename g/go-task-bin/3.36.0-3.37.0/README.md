# Comparing `tmp/go_task_bin-3.36.0.tar.gz` & `tmp/go_task_bin-3.37.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go_task_bin-3.36.0.tar", last modified: Thu Apr 18 05:27:35 2024, max compression
+gzip compressed data, was "go_task_bin-3.37.0.tar", last modified: Thu May  9 01:41:37 2024, max compression
```

## Comparing `go_task_bin-3.36.0.tar` & `go_task_bin-3.37.0.tar`

### file list

```diff
@@ -1,408 +1,414 @@
--rw-r--r--   0        0        0     1074 2024-04-18 05:25:30.803037 go_task_bin-3.36.0/LICENSE
--rw-r--r--   0        0        0     1031 2024-04-18 05:25:30.803037 go_task_bin-3.36.0/README.md
--rw-r--r--   0        0        0        0 2024-04-18 05:25:30.803037 go_task_bin-3.36.0/go_task_bin/__init__.py
--rw-r--r--   0        0        0     1384 2024-04-18 05:25:30.803037 go_task_bin-3.36.0/pdm_build.py
--rw-r--r--   0        0        0     1245 2024-04-18 05:27:35.819217 go_task_bin-3.36.0/pyproject.toml
--rw-r--r--   0        0        0      231 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.editorconfig
--rw-r--r--   0        0        0       37 2024-04-18 05:25:32.395039 go_task_bin-3.36.0/task/.git
--rw-r--r--   0        0        0       12 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.gitattributes
--rw-r--r--   0        0        0     3217 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      521 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       88 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/FUNDING.yml
--rw-r--r--   0        0        0      387 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      552 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      368 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      462 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/dependabot.yml
--rw-r--r--   0        0        0      225 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/pull_request_template.md
--rw-r--r--   0        0        0     1463 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/issue-awaiting-response.yml
--rw-r--r--   0        0        0      838 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/issue-closed.yml
--rw-r--r--   0        0        0     6565 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/issue-experiment.yml
--rw-r--r--   0        0        0      813 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/issue-needs-triage.yml
--rw-r--r--   0        0        0      865 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/lint.yml
--rw-r--r--   0        0        0      476 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/release.yml
--rw-r--r--   0        0        0      872 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/test.yml
--rw-r--r--   0        0        0      922 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.github/workflows/upload-source-documents.yml
--rw-r--r--   0        0        0      445 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.gitignore
--rw-r--r--   0        0        0      387 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.golangci.yml
--rw-r--r--   0        0        0     3037 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.goreleaser.yml
--rw-r--r--   0        0        0       77 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.mockery.yaml
--rw-r--r--   0        0        0        8 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.nvmrc
--rw-r--r--   0        0        0      125 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.prettierrc.yml
--rw-r--r--   0        0        0      324 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/.vscode/settings-sample.json
--rw-r--r--   0        0        0    37761 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/CHANGELOG.md
--rw-r--r--   0        0        0     1080 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/LICENSE
--rw-r--r--   0        0        0      634 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/README.md
--rw-r--r--   0        0        0     2948 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/Taskfile.yml
--rw-r--r--   0        0        0      586 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/args/args.go
--rw-r--r--   0        0        0     2393 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/args/args_test.go
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.403040 go_task_bin-3.36.0/task/bin/.keep
--rw-r--r--   0        0        0     3288 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/cmd/release/main.go
--rw-r--r--   0        0        0     4874 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/cmd/sleepit/sleepit.go
--rw-r--r--   0        0        0     4466 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/cmd/task/task.go
--rw-r--r--   0        0        0     1329 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/completion/bash/task.bash
--rw-r--r--   0        0        0     2342 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/completion/fish/task.fish
--rw-r--r--   0        0        0     1992 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/completion/ps/task.ps1
--rwxr-xr-x   0        0        0     2431 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/completion/zsh/_task
--rw-r--r--   0        0        0      436 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/concurrency.go
--rw-r--r--   0        0        0     1558 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/errors/errors.go
--rw-r--r--   0        0        0     3645 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/errors/errors_task.go
--rw-r--r--   0        0        0     4674 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/errors/errors_taskfile.go
--rw-r--r--   0        0        0      979 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/go.mod
--rw-r--r--   0        0        0     5796 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/go.sum
--rw-r--r--   0        0        0      445 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/hash.go
--rw-r--r--   0        0        0     5727 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/help.go
--rw-r--r--   0        0        0      770 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/init.go
--rwxr-xr-x   0        0        0     9634 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/install-task.sh
--rw-r--r--   0        0        0     5633 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/compiler/compiler.go
--rw-r--r--   0        0        0      380 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/compiler/env.go
--rw-r--r--   0        0        0     3621 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/deepcopy/deepcopy.go
--rw-r--r--   0        0        0      659 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/editors/output.go
--rw-r--r--   0        0        0      430 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/env/env.go
--rw-r--r--   0        0        0      287 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/execext/devnull.go
--rw-r--r--   0        0        0     3349 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/execext/exec.go
--rw-r--r--   0        0        0     1082 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/exp/maps.go
--rw-r--r--   0        0        0     2550 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/experiments/experiments.go
--rw-r--r--   0        0        0     1031 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/filepathext/filepathext.go
--rw-r--r--   0        0        0      518 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/checker.go
--rw-r--r--   0        0        0     1094 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/glob.go
--rw-r--r--   0        0        0      388 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/sources.go
--rw-r--r--   0        0        0     2791 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/sources_checksum.go
--rw-r--r--   0        0        0      396 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/sources_checksum_test.go
--rw-r--r--   0        0        0      459 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/sources_none.go
--rw-r--r--   0        0        0     3521 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/sources_timestamp.go
--rw-r--r--   0        0        0      890 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/status.go
--rw-r--r--   0        0        0     2938 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/task.go
--rw-r--r--   0        0        0     5500 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/fingerprint/task_test.go
--rw-r--r--   0        0        0     5766 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/flags/flags.go
--rw-r--r--   0        0        0     1191 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/goext/meta.go
--rw-r--r--   0        0        0      439 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/hash/hash.go
--rw-r--r--   0        0        0     4053 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/logger/logger.go
--rw-r--r--   0        0        0     6003 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/mocks/sources_checkable.go
--rw-r--r--   0        0        0     2592 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/mocks/status_checkable.go
--rw-r--r--   0        0        0     3805 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/omap/orderedmap.go
--rw-r--r--   0        0        0     2607 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/omap/orderedmap_test.go
--rw-r--r--   0        0        0     1058 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/output/group.go
--rw-r--r--   0        0        0      292 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/output/interleaved.go
--rw-r--r--   0        0        0     1075 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/output/output.go
--rw-r--r--   0        0        0     3496 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/output/output_test.go
--rw-r--r--   0        0        0     1359 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/output/prefixed.go
--rw-r--r--   0        0        0      286 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/slicesext/slicesext.go
--rw-r--r--   0        0        0     1063 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/sort/sorter.go
--rw-r--r--   0        0        0     1895 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/sort/sorter_test.go
--rw-r--r--   0        0        0     2531 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/summary/summary.go
--rw-r--r--   0        0        0     3636 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/summary/summary_test.go
--rw-r--r--   0        0        0      308 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/sysinfo/uid.go
--rw-r--r--   0        0        0      208 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/sysinfo/uid_win.go
--rw-r--r--   0        0        0     2034 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/templater/funcs.go
--rw-r--r--   0        0        0     2817 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/templater/templater.go
--rw-r--r--   0        0        0      165 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/term/term.go
--rw-r--r--   0        0        0      348 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/internal/version/version.go
--rw-r--r--   0        0        0      924 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/package-lock.json
--rw-r--r--   0        0        0      807 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/package.json
--rw-r--r--   0        0        0      804 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/precondition.go
--rw-r--r--   0        0        0      679 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/requires.go
--rw-r--r--   0        0        0     5731 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/setup.go
--rw-r--r--   0        0        0      700 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/signals.go
--rw-r--r--   0        0        0     7605 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/signals_test.go
--rw-r--r--   0        0        0     1172 2024-04-18 05:25:32.407039 go_task_bin-3.36.0/task/status.go
--rw-r--r--   0        0        0    13331 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/task.go
--rw-r--r--   0        0        0    62564 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/task_test.go
--rw-r--r--   0        0        0      185 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/call.go
--rw-r--r--   0        0        0     2490 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/cmd.go
--rw-r--r--   0        0        0      921 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/dep.go
--rw-r--r--   0        0        0     1156 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/for.go
--rw-r--r--   0        0        0      530 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/glob.go
--rw-r--r--   0        0        0     2938 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/include.go
--rw-r--r--   0        0        0      247 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/location.go
--rw-r--r--   0        0        0     1373 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/output.go
--rw-r--r--   0        0        0     2431 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/platforms.go
--rw-r--r--   0        0        0     1522 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/platforms_test.go
--rw-r--r--   0        0        0     1150 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/precondition.go
--rw-r--r--   0        0        0      976 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/precondition_test.go
--rw-r--r--   0        0        0      318 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/requires.go
--rw-r--r--   0        0        0     5704 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/task.go
--rw-r--r--   0        0        0     2128 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/taskfile.go
--rw-r--r--   0        0        0     1887 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/taskfile_test.go
--rw-r--r--   0        0        0     4111 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/tasks.go
--rw-r--r--   0        0        0     3559 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/ast/var.go
--rw-r--r--   0        0        0     1232 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/cache.go
--rw-r--r--   0        0        0     1011 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/dotenv.go
--rw-r--r--   0        0        0     2100 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/node.go
--rw-r--r--   0        0        0     1013 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/node_base.go
--rw-r--r--   0        0        0     2752 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/node_file.go
--rw-r--r--   0        0        0     2592 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/node_http.go
--rw-r--r--   0        0        0     1444 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/node_stdin.go
--rw-r--r--   0        0        0     7476 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/reader.go
--rw-r--r--   0        0        0     5106 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/taskfile/taskfile.go
--rw-r--r--   0        0        0      243 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/alias/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/alias/Taskfile2.yml
--rw-r--r--   0        0        0      111 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/alias/alias-summary.txt
--rw-r--r--   0        0        0       90 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/alias/alias.txt
--rw-r--r--   0        0        0       21 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/checksum/.gitignore
--rw-r--r--   0        0        0      428 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/checksum/Taskfile.yml
--rw-r--r--   0        0        0       14 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/checksum/ignore_me.txt
--rw-r--r--   0        0        0       14 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/checksum/source.txt
--rw-r--r--   0        0        0      351 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/concurrency/Taskfile.yml
--rw-r--r--   0        0        0      104 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/cyclic/Taskfile.yml
--rw-r--r--   0        0        0      243 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/deferred/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/deps/.gitignore
--rw-r--r--   0        0        0      703 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/deps/Taskfile.yml
--rw-r--r--   0        0        0       72 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/dynamic_var/.gitignore
--rw-r--r--   0        0        0      649 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/dynamic_var/Taskfile.yml
--rw-r--r--   0        0        0      377 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/dynamic_var/subdirectory/Taskfile.yml
--rw-r--r--   0        0        0      136 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/dynamic_var_on_created_dir/Taskfile.yml
--rw-r--r--   0        0        0       90 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/explicit_doesnt_exist/Taskfile.yml
--rw-r--r--   0        0        0       88 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/explicit_exists/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dir/explicit_exists/exists/.keep
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/.gitignore
--rw-r--r--   0        0        0      168 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/default/Taskfile.yml
--rw-r--r--   0        0        0       31 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/env_var_in_path/.env.testing
--rw-r--r--   0        0        0      119 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/env_var_in_path/Taskfile.yml
--rw-r--r--   0        0        0      158 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/error_included_envs/Taskfile.yml
--rw-r--r--   0        0        0       23 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/include1/.env
--rw-r--r--   0        0        0       31 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/include1/Taskfile.yml
--rw-r--r--   0        0        0       23 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/include1/envs/.env
--rw-r--r--   0        0        0       31 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/local_env_in_path/.env.testing
--rw-r--r--   0        0        0      148 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/local_env_in_path/Taskfile.yml
--rw-r--r--   0        0        0       31 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/local_var_in_path/.env.testing
--rw-r--r--   0        0        0      195 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/local_var_in_path/Taskfile.yml
--rw-r--r--   0        0        0      131 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv/missing_env/Taskfile.yml
--rw-r--r--   0        0        0        8 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv_task/default/.env
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv_task/default/.gitignore
--rw-r--r--   0        0        0      456 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dotenv_task/default/Taskfile.yml
--rw-r--r--   0        0        0       63 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dry/Taskfile.yml
--rw-r--r--   0        0        0      121 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dry_checksum/Taskfile.yml
--rw-r--r--   0        0        0       13 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/dry_checksum/source.txt
--rw-r--r--   0        0        0       32 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/empty_task/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/env/.gitignore
--rw-r--r--   0        0        0      499 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/env/Taskfile.yml
--rw-r--r--   0        0        0      101 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/error_code/Taskfile.yml
--rw-r--r--   0        0        0      280 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/evaluate_symlinks_in_paths/Taskfile.yaml
--rw-r--r--   0        0        0       19 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/evaluate_symlinks_in_paths/shared/b
--rw-r--r--   0        0        0       25 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/evaluate_symlinks_in_paths/shared/inner_shared/c
--rw-r--r--   0        0        0       12 2024-04-18 05:25:32.411039 go_task_bin-3.36.0/task/testdata/evaluate_symlinks_in_paths/src/a
--rw-r--r--   0        0        0       89 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/exit_immediately/Taskfile.yml
--rw-r--r--   0        0        0       80 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/expand/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/file_names/.gitignore
--rw-r--r--   0        0        0       58 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/file_names/Taskfile.dist.yaml/Taskfile.dist.yaml
--rw-r--r--   0        0        0       58 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/file_names/Taskfile.dist.yml/Taskfile.dist.yml
--rw-r--r--   0        0        0       58 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/file_names/Taskfile.yaml/Taskfile.yaml
--rw-r--r--   0        0        0       58 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/file_names/Taskfile.yml/Taskfile.yml
--rw-r--r--   0        0        0     1635 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/cmds/Taskfile.yml
--rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/cmds/bar.txt
--rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/cmds/foo.txt
--rw-r--r--   0        0        0     1876 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/deps/Taskfile.yml
--rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/deps/bar.txt
--rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/for/deps/foo.txt
--rw-r--r--   0        0        0      295 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/force/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/generates/.gitignore
--rw-r--r--   0        0        0      986 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/generates/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/generates/sub/.keep
--rw-r--r--   0        0        0      262 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_errors/Taskfile.yml
--rw-r--r--   0        0        0       80 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_nil_elements/cmds/Taskfile.yml
--rw-r--r--   0        0        0      116 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_nil_elements/deps/Taskfile.yml
--rw-r--r--   0        0        0       94 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_nil_elements/includes/Taskfile.yml
--rw-r--r--   0        0        0       81 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_nil_elements/includes/inc.yml
--rw-r--r--   0        0        0      123 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_nil_elements/preconditions/Taskfile.yml
--rw-r--r--   0        0        0       66 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/ignore_signals/Taskfile.yml
--rw-r--r--   0        0        0      385 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars/Taskfile.yml
--rw-r--r--   0        0        0      229 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars/include/Taskfile.include.yml
--rw-r--r--   0        0        0      266 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars_multi_level/Taskfile.yml
--rw-r--r--   0        0        0       97 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars_multi_level/bar/Taskfile.yml
--rw-r--r--   0        0        0       97 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars_multi_level/foo/Taskfile.yml
--rw-r--r--   0        0        0      130 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/include_with_vars_multi_level/lib/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/.gitignore
--rw-r--r--   0        0        0      768 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/Taskfile.yml
--rw-r--r--   0        0        0       93 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/Taskfile2.yml
--rw-r--r--   0        0        0       55 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/Taskfile_darwin.yml
--rw-r--r--   0        0        0       55 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/Taskfile_linux.yml
--rw-r--r--   0        0        0       55 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/Taskfile_windows.yml
--rw-r--r--   0        0        0       95 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/included/Taskfile.yml
--rw-r--r--   0        0        0      225 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/module1/Taskfile.yml
--rw-r--r--   0        0        0      213 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes/module2/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_call_root_task/.gitignore
--rw-r--r--   0        0        0      122 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_call_root_task/Taskfile.yml
--rw-r--r--   0        0        0       69 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_call_root_task/Taskfile2.yml
--rw-r--r--   0        0        0      173 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_cycle/Taskfile.yml
--rw-r--r--   0        0        0      109 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_cycle/one/Taskfile.yml
--rw-r--r--   0        0        0      109 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_cycle/one/two/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_deps/.gitignore
--rw-r--r--   0        0        0      110 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_deps/Taskfile.yml
--rw-r--r--   0        0        0      267 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_deps/Taskfile2.yml
--rw-r--r--   0        0        0        9 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_empty/.gitignore
--rw-r--r--   0        0        0       50 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_empty/Taskfile.yml
--rw-r--r--   0        0        0      125 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_empty/Taskfile2.yml
--rw-r--r--   0        0        0       51 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_incorrect/Taskfile.yml
--rw-r--r--   0        0        0       28 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_incorrect/incomplete.yml
--rw-r--r--   0        0        0      188 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_internal/Taskfile.yml
--rw-r--r--   0        0        0       70 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_internal/Taskfile2.yml
--rw-r--r--   0        0        0      196 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_interpolation/Taskfile.yml
--rw-r--r--   0        0        0       66 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_interpolation/included/Taskfile.yml
--rw-r--r--   0        0        0      161 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/Taskfile.yml
--rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/called_one.txt
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/called_three.txt
--rw-r--r--   0        0        0        4 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/called_two.txt
--rw-r--r--   0        0        0       85 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/one/Taskfile.yml
--rw-r--r--   0        0        0      101 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/one/two/Taskfile.yml
--rw-r--r--   0        0        0       62 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_multi_level/one/two/three/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_optional/.gitignore
--rw-r--r--   0        0        0      162 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_optional/Taskfile.yml
--rw-r--r--   0        0        0      149 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_optional_explicit_false/Taskfile.yml
--rw-r--r--   0        0        0      115 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_optional_implicit_false/Taskfile.yml
--rw-r--r--   0        0        0      133 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_rel_path/Taskfile.yml
--rw-r--r--   0        0        0       32 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_rel_path/common/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_rel_path/included/Taskfile.yml
--rw-r--r--   0        0        0      129 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_shadowed_default/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_shadowed_default/Taskfile2.yml
--rw-r--r--   0        0        0        9 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_shadowed_default/file.txt
--rw-r--r--   0        0        0       64 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_unshadowed_default/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_unshadowed_default/Taskfile2.yml
--rw-r--r--   0        0        0        9 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_unshadowed_default/file.txt
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_yaml/.gitignore
--rw-r--r--   0        0        0      226 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_yaml/Custom.ext
--rw-r--r--   0        0        0      115 2024-04-18 05:25:32.415039 go_task_bin-3.36.0/task/testdata/includes_yaml/included/Taskfile.yaml
--rw-r--r--   0        0        0      109 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/includes_yaml/included/custom.yaml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/init/.gitignore
--rw-r--r--   0        0        0      167 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/internal_task/Taskfile.yml
--rw-r--r--   0        0        0       77 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/label_list/Taskfile.yml
--rw-r--r--   0        0        0       76 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/label_status/Taskfile.yml
--rw-r--r--   0        0        0      104 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/label_summary/Taskfile.yml
--rw-r--r--   0        0        0       82 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/label_uptodate/Taskfile.yml
--rw-r--r--   0        0        0      105 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/label_var/Taskfile.yml
--rw-r--r--   0        0        0       90 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/list_desc_interpolation/Taskfile.yml
--rw-r--r--   0        0        0      164 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/list_mixed_desc/Taskfile.yml
--rw-r--r--   0        0        0      199 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/output_group/Taskfile.yml
--rw-r--r--   0        0        0      255 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/output_group_error_only/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/params/.gitignore
--rw-r--r--   0        0        0     1255 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/params/Taskfile.yml
--rw-r--r--   0        0        0     1584 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/platforms/Taskfile.yml
--rw-r--r--   0        0        0      285 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/precondition/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/precondition/foo.txt
--rw-r--r--   0        0        0      226 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/prompt/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/run/.gitignore
--rw-r--r--   0        0        0      468 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/run/Taskfile.yml
--rw-r--r--   0        0        0      201 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/shopts/command_level/Taskfile.yml
--rw-r--r--   0        0        0      175 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/shopts/global_level/Taskfile.yml
--rw-r--r--   0        0        0      183 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/shopts/task_level/Taskfile.yml
--rw-r--r--   0        0        0      174 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/short_task_notation/Taskfile.yml
--rw-r--r--   0        0        0     1350 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/silent/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/single_cmd_dep/.gitignore
--rw-r--r--   0        0        0       99 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/single_cmd_dep/Taskfile.yml
--rw-r--r--   0        0        0      282 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/special_vars/Taskfile.yml
--rw-r--r--   0        0        0      214 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/special_vars/included/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/special_vars/subdir/.gitkeep
--rw-r--r--   0        0        0       92 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/split_args/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/status/.gitignore
--rw-r--r--   0        0        0      331 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/status/Taskfile.yml
--rw-r--r--   0        0        0       14 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/status_vars/.gitignore
--rw-r--r--   0        0        0      170 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/status_vars/Taskfile.yml
--rw-r--r--   0        0        0       14 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/status_vars/source.txt
--rw-r--r--   0        0        0      566 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/summary/Taskfile.yml
--rw-r--r--   0        0        0      346 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/summary/task-with-summary.txt
--rw-r--r--   0        0        0       78 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/taskfile_walk/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/taskfile_walk/foo/bar/.gitkeep
--rw-r--r--   0        0        0       96 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/user_working_dir/Taskfile.yml
--rw-r--r--   0        0        0       74 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/user_working_dir_with_includes/Taskfile.yml
--rw-r--r--   0        0        0      101 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/user_working_dir_with_includes/included/Taskfile.yml
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/user_working_dir_with_includes/somedir/.keep
--rw-r--r--   0        0        0       27 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/.env
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/.gitignore
--rw-r--r--   0        0        0     1008 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/Taskfile.yml
--rw-r--r--   0        0        0     2188 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/any/Taskfile.yml
--rw-r--r--   0        0        0     2385 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/any2/Taskfile.yml
--rw-r--r--   0        0        0      276 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/any2/example.json
--rw-r--r--   0        0        0      111 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/vars/any2/example.yaml
--rw-r--r--   0        0        0       93 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/version/v1/Taskfile.yml
--rw-r--r--   0        0        0       93 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/version/v2/Taskfile.yml
--rw-r--r--   0        0        0       93 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/version/v3/Taskfile.yml
--rw-r--r--   0        0        0        6 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/watcher_interval/.gitignore
--rw-r--r--   0        0        0      194 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/watcher_interval/Taskfile.yaml
--rw-r--r--   0        0        0      519 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/testdata/wildcards/Taskfile.yml
--rw-r--r--   0        0        0     9862 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/variables.go
--rw-r--r--   0        0        0     4215 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/watch.go
--rw-r--r--   0        0        0     2041 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/watch_test.go
--rw-r--r--   0        0        0      238 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/.gitignore
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/.nojekyll
--rw-r--r--   0        0        0     1523 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/Taskfile.yml
--rw-r--r--   0        0        0       70 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/babel.config.ts
--rw-r--r--   0        0        0     6842 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/blog/2023-09-02-introducing-experiments.md
--rw-r--r--   0        0        0      279 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/blog/authors.yml
--rw-r--r--   0        0        0      242 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/constants.ts
--rw-r--r--   0        0        0      359 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/crowdin.yml
--rw-r--r--   0        0        0    41797 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/docs/api_reference.mdx
--rw-r--r--   0        0        0    37809 2024-04-18 05:25:32.419040 go_task_bin-3.36.0/task/website/docs/changelog.mdx
--rw-r--r--   0        0        0     1529 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/community.mdx
--rw-r--r--   0        0        0     7804 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/contributing.mdx
--rw-r--r--   0        0        0      711 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/deprecations/deprecations.mdx
--rw-r--r--   0        0        0      655 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/deprecations/template.mdx
--rw-r--r--   0        0        0     1245 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/deprecations/version_2_schema.mdx
--rw-r--r--   0        0        0     8037 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/experiments/any_variables.mdx
--rw-r--r--   0        0        0     5677 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/experiments/experiments.mdx
--rw-r--r--   0        0        0     1536 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/experiments/gentle_force.mdx
--rw-r--r--   0        0        0     4244 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/experiments/remote_taskfiles.mdx
--rw-r--r--   0        0        0     1124 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/experiments/template.mdx
--rw-r--r--   0        0        0     2583 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/faq.mdx
--rw-r--r--   0        0        0     6941 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/installation.mdx
--rw-r--r--   0        0        0     2911 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/integrations.mdx
--rw-r--r--   0        0        0     1993 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/intro.mdx
--rw-r--r--   0        0        0     2797 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/releasing.mdx
--rw-r--r--   0        0        0     2974 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/styleguide.mdx
--rw-r--r--   0        0        0     5454 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/taskfile_versions.mdx
--rw-r--r--   0        0        0      763 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/translate.mdx
--rw-r--r--   0        0        0    45153 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docs/usage.mdx
--rw-r--r--   0        0        0     6526 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/docusaurus.config.ts
--rw-r--r--   0        0        0     1508 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/package.json
--rw-r--r--   0        0        0      208 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/prettier.config.js
--rw-r--r--   0        0        0      271 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/sidebars.ts
--rw-r--r--   0        0        0     1050 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/api/crowdin.js
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/components/.keep
--rw-r--r--   0        0        0     1202 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/css/carbon.css
--rw-r--r--   0        0        0     3089 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/css/custom.css
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/pages/.keep
--rw-r--r--   0        0        0     1922 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/pages/donate.md
--rw-r--r--   0        0        0     1342 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/themes/prismDark.js
--rw-r--r--   0        0        0     1679 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/src/themes/prismLight.js
--rw-r--r--   0        0        0        0 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/.nojekyll
--rw-r--r--   0        0        0       13 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/CNAME
--rw-r--r--   0        0        0      109 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/Taskfile.yml
--rw-r--r--   0        0        0     7281 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/appwrite.svg
--rw-r--r--   0        0        0   173915 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/favicon.ico
--rw-r--r--   0        0        0     1321 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/icon-discord.svg
--rw-r--r--   0        0        0     1227 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/icon-github.svg
--rw-r--r--   0        0        0     1717 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/icon-mastodon.svg
--rw-r--r--   0        0        0     1742 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/icon-twitter.svg
--rw-r--r--   0        0        0    13524 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/logo.png
--rw-r--r--   0        0        0      435 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/logo.svg
--rw-r--r--   0        0        0      360 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/logo_mono.svg
--rw-r--r--   0        0        0    19847 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/og-image.png
--rw-r--r--   0        0        0     1276 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/img/pix.png
--rwxr-xr-x   0        0        0     9634 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/install.sh
--rw-r--r--   0        0        0      784 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/js/carbon.js
--rw-r--r--   0        0        0    22415 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/static/schema.json
--rw-r--r--   0        0        0       87 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/tsconfig.json
--rw-r--r--   0        0        0    41797 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/api_reference.mdx
--rw-r--r--   0        0        0    37809 2024-04-18 05:25:32.423040 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/changelog.mdx
--rw-r--r--   0        0        0     1529 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/community.mdx
--rw-r--r--   0        0        0     7804 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/contributing.mdx
--rw-r--r--   0        0        0      711 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/deprecations.mdx
--rw-r--r--   0        0        0      655 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/template.mdx
--rw-r--r--   0        0        0     1245 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/version_2_schema.mdx
--rw-r--r--   0        0        0     8037 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/any_variables.mdx
--rw-r--r--   0        0        0     5677 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/experiments.mdx
--rw-r--r--   0        0        0     1536 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/gentle_force.mdx
--rw-r--r--   0        0        0     4244 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/remote_taskfiles.mdx
--rw-r--r--   0        0        0     1124 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/template.mdx
--rw-r--r--   0        0        0     2583 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/faq.mdx
--rw-r--r--   0        0        0     6941 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/installation.mdx
--rw-r--r--   0        0        0     2911 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/integrations.mdx
--rw-r--r--   0        0        0     1993 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/intro.mdx
--rw-r--r--   0        0        0     2797 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/releasing.mdx
--rw-r--r--   0        0        0     2974 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/styleguide.mdx
--rw-r--r--   0        0        0     5454 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/taskfile_versions.mdx
--rw-r--r--   0        0        0      763 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/translate.mdx
--rw-r--r--   0        0        0    45153 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_docs/version-latest/usage.mdx
--rw-r--r--   0        0        0      174 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versioned_sidebars/version-latest-sidebars.json
--rw-r--r--   0        0        0       15 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/versions.json
--rw-r--r--   0        0        0   364377 2024-04-18 05:25:32.427039 go_task_bin-3.36.0/task/website/yarn.lock
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 go_task_bin-3.36.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-09 01:39:37.449707 go_task_bin-3.37.0/LICENSE
+-rw-r--r--   0        0        0     1031 2024-05-09 01:39:37.449707 go_task_bin-3.37.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:37.449707 go_task_bin-3.37.0/go_task_bin/__init__.py
+-rw-r--r--   0        0        0     1384 2024-05-09 01:39:37.449707 go_task_bin-3.37.0/pdm_build.py
+-rw-r--r--   0        0        0     1245 2024-05-09 01:41:37.154029 go_task_bin-3.37.0/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.editorconfig
+-rw-r--r--   0        0        0       37 2024-05-09 01:39:39.317712 go_task_bin-3.37.0/task/.git
+-rw-r--r--   0        0        0       12 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.gitattributes
+-rw-r--r--   0        0        0     3217 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      521 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       88 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/FUNDING.yml
+-rw-r--r--   0        0        0      387 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      552 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      368 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      462 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/dependabot.yml
+-rw-r--r--   0        0        0      225 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1463 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/issue-awaiting-response.yml
+-rw-r--r--   0        0        0      838 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/issue-closed.yml
+-rw-r--r--   0        0        0     6565 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/issue-experiment.yml
+-rw-r--r--   0        0        0      813 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/issue-needs-triage.yml
+-rw-r--r--   0        0        0      865 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      476 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/release.yml
+-rw-r--r--   0        0        0      872 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/test.yml
+-rw-r--r--   0        0        0      922 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.github/workflows/upload-source-documents.yml
+-rw-r--r--   0        0        0      468 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.gitignore
+-rw-r--r--   0        0        0      382 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.golangci.yml
+-rw-r--r--   0        0        0     3037 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.goreleaser.yml
+-rw-r--r--   0        0        0       77 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.mockery.yaml
+-rw-r--r--   0        0        0        8 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.nvmrc
+-rw-r--r--   0        0        0      125 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.prettierrc.yml
+-rw-r--r--   0        0        0      324 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/.vscode/settings-sample.json
+-rw-r--r--   0        0        0    38766 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/CHANGELOG.md
+-rw-r--r--   0        0        0     1080 2024-05-09 01:39:39.325712 go_task_bin-3.37.0/task/LICENSE
+-rw-r--r--   0        0        0      634 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/README.md
+-rw-r--r--   0        0        0     2948 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/Taskfile.yml
+-rw-r--r--   0        0        0      586 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/args/args.go
+-rw-r--r--   0        0        0     2393 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/args/args_test.go
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/bin/.keep
+-rw-r--r--   0        0        0     3288 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/cmd/release/main.go
+-rw-r--r--   0        0        0     4874 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/cmd/sleepit/sleepit.go
+-rw-r--r--   0        0        0     4694 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/cmd/task/task.go
+-rw-r--r--   0        0        0     1329 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/completion/bash/task.bash
+-rw-r--r--   0        0        0     2342 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/completion/fish/task.fish
+-rw-r--r--   0        0        0     1992 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/completion/ps/task.ps1
+-rwxr-xr-x   0        0        0     2466 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/completion/zsh/_task
+-rw-r--r--   0        0        0      436 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/concurrency.go
+-rw-r--r--   0        0        0     1612 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/errors/errors.go
+-rw-r--r--   0        0        0     3645 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/errors/errors_task.go
+-rw-r--r--   0        0        0     5111 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/errors/errors_taskfile.go
+-rw-r--r--   0        0        0     1084 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/go.mod
+-rw-r--r--   0        0        0     6204 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/go.sum
+-rw-r--r--   0        0        0      445 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/hash.go
+-rw-r--r--   0        0        0     5727 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/help.go
+-rw-r--r--   0        0        0      770 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/init.go
+-rwxr-xr-x   0        0        0     9634 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/install-task.sh
+-rw-r--r--   0        0        0     5499 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/compiler/compiler.go
+-rw-r--r--   0        0        0      380 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/compiler/env.go
+-rw-r--r--   0        0        0     3621 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/deepcopy/deepcopy.go
+-rw-r--r--   0        0        0      659 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/editors/output.go
+-rw-r--r--   0        0        0      430 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/env/env.go
+-rw-r--r--   0        0        0      287 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/execext/devnull.go
+-rw-r--r--   0        0        0     3463 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/execext/exec.go
+-rw-r--r--   0        0        0     1082 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/exp/maps.go
+-rw-r--r--   0        0        0     2625 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/experiments/experiments.go
+-rw-r--r--   0        0        0     1031 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/filepathext/filepathext.go
+-rw-r--r--   0        0        0      518 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/checker.go
+-rw-r--r--   0        0        0     1094 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/glob.go
+-rw-r--r--   0        0        0      388 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/sources.go
+-rw-r--r--   0        0        0     2791 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/sources_checksum.go
+-rw-r--r--   0        0        0      396 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/sources_checksum_test.go
+-rw-r--r--   0        0        0      459 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/sources_none.go
+-rw-r--r--   0        0        0     3521 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/sources_timestamp.go
+-rw-r--r--   0        0        0      890 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/status.go
+-rw-r--r--   0        0        0     2938 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/task.go
+-rw-r--r--   0        0        0     5500 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/fingerprint/task_test.go
+-rw-r--r--   0        0        0     5815 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/flags/flags.go
+-rw-r--r--   0        0        0     1191 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/goext/meta.go
+-rw-r--r--   0        0        0      439 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/hash/hash.go
+-rw-r--r--   0        0        0     4144 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/logger/logger.go
+-rw-r--r--   0        0        0     6003 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/mocks/sources_checkable.go
+-rw-r--r--   0        0        0     2592 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/mocks/status_checkable.go
+-rw-r--r--   0        0        0     3805 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/omap/orderedmap.go
+-rw-r--r--   0        0        0     2607 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/omap/orderedmap_test.go
+-rw-r--r--   0        0        0     1058 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/output/group.go
+-rw-r--r--   0        0        0      292 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/output/interleaved.go
+-rw-r--r--   0        0        0     1075 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/output/output.go
+-rw-r--r--   0        0        0     3496 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/output/output_test.go
+-rw-r--r--   0        0        0     1359 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/output/prefixed.go
+-rw-r--r--   0        0        0      286 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/slicesext/slicesext.go
+-rw-r--r--   0        0        0     1063 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/sort/sorter.go
+-rw-r--r--   0        0        0     1895 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/sort/sorter_test.go
+-rw-r--r--   0        0        0     2531 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/summary/summary.go
+-rw-r--r--   0        0        0     3636 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/summary/summary_test.go
+-rw-r--r--   0        0        0      308 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/sysinfo/uid.go
+-rw-r--r--   0        0        0      208 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/sysinfo/uid_win.go
+-rw-r--r--   0        0        0     2122 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/templater/funcs.go
+-rw-r--r--   0        0        0     3291 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/templater/templater.go
+-rw-r--r--   0        0        0      165 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/term/term.go
+-rw-r--r--   0        0        0      348 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/internal/version/version.go
+-rw-r--r--   0        0        0      924 2024-05-09 01:39:39.329712 go_task_bin-3.37.0/task/package-lock.json
+-rw-r--r--   0        0        0      807 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/package.json
+-rw-r--r--   0        0        0      804 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/precondition.go
+-rw-r--r--   0        0        0      679 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/requires.go
+-rw-r--r--   0        0        0     5808 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/setup.go
+-rw-r--r--   0        0        0      700 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/signals.go
+-rw-r--r--   0        0        0     7605 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/signals_test.go
+-rw-r--r--   0        0        0     1172 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/status.go
+-rw-r--r--   0        0        0    13331 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/task.go
+-rw-r--r--   0        0        0    62707 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/task_test.go
+-rw-r--r--   0        0        0      185 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/call.go
+-rw-r--r--   0        0        0     2490 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/cmd.go
+-rw-r--r--   0        0        0      921 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/dep.go
+-rw-r--r--   0        0        0     1156 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/for.go
+-rw-r--r--   0        0        0      530 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/glob.go
+-rw-r--r--   0        0        0     2729 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/graph.go
+-rw-r--r--   0        0        0     2941 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/include.go
+-rw-r--r--   0        0        0      247 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/location.go
+-rw-r--r--   0        0        0     1373 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/output.go
+-rw-r--r--   0        0        0     2431 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/platforms.go
+-rw-r--r--   0        0        0     1522 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/platforms_test.go
+-rw-r--r--   0        0        0     1150 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/precondition.go
+-rw-r--r--   0        0        0      976 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/precondition_test.go
+-rw-r--r--   0        0        0      318 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/requires.go
+-rw-r--r--   0        0        0     5704 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/task.go
+-rw-r--r--   0        0        0     2502 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/taskfile.go
+-rw-r--r--   0        0        0     1887 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/taskfile_test.go
+-rw-r--r--   0        0        0     4508 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/tasks.go
+-rw-r--r--   0        0        0     3751 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/ast/var.go
+-rw-r--r--   0        0        0     1232 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/cache.go
+-rw-r--r--   0        0        0     1011 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/dotenv.go
+-rw-r--r--   0        0        0     2017 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/node.go
+-rw-r--r--   0        0        0      780 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/node_base.go
+-rw-r--r--   0        0        0     2752 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/node_file.go
+-rw-r--r--   0        0        0     2592 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/node_http.go
+-rw-r--r--   0        0        0     1444 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/node_stdin.go
+-rw-r--r--   0        0        0     7915 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/reader.go
+-rw-r--r--   0        0        0     4843 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/taskfile/taskfile.go
+-rw-r--r--   0        0        0      243 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/alias/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/alias/Taskfile2.yml
+-rw-r--r--   0        0        0      111 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/alias/alias-summary.txt
+-rw-r--r--   0        0        0       90 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/alias/alias.txt
+-rw-r--r--   0        0        0       21 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/checksum/.gitignore
+-rw-r--r--   0        0        0      428 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/checksum/Taskfile.yml
+-rw-r--r--   0        0        0       14 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/checksum/ignore_me.txt
+-rw-r--r--   0        0        0       14 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/checksum/source.txt
+-rw-r--r--   0        0        0      351 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/concurrency/Taskfile.yml
+-rw-r--r--   0        0        0      104 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/cyclic/Taskfile.yml
+-rw-r--r--   0        0        0      243 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/deferred/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/deps/.gitignore
+-rw-r--r--   0        0        0      703 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/deps/Taskfile.yml
+-rw-r--r--   0        0        0       72 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/dynamic_var/.gitignore
+-rw-r--r--   0        0        0      649 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/dynamic_var/Taskfile.yml
+-rw-r--r--   0        0        0      377 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/dynamic_var/subdirectory/Taskfile.yml
+-rw-r--r--   0        0        0      136 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/dynamic_var_on_created_dir/Taskfile.yml
+-rw-r--r--   0        0        0       90 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/explicit_doesnt_exist/Taskfile.yml
+-rw-r--r--   0        0        0       88 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/explicit_exists/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dir/explicit_exists/exists/.keep
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/.gitignore
+-rw-r--r--   0        0        0      168 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/default/Taskfile.yml
+-rw-r--r--   0        0        0       31 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/env_var_in_path/.env.testing
+-rw-r--r--   0        0        0      119 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/env_var_in_path/Taskfile.yml
+-rw-r--r--   0        0        0      158 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/error_included_envs/Taskfile.yml
+-rw-r--r--   0        0        0       23 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/include1/.env
+-rw-r--r--   0        0        0       31 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/include1/Taskfile.yml
+-rw-r--r--   0        0        0       23 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/include1/envs/.env
+-rw-r--r--   0        0        0       31 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/local_env_in_path/.env.testing
+-rw-r--r--   0        0        0      148 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/local_env_in_path/Taskfile.yml
+-rw-r--r--   0        0        0       31 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/local_var_in_path/.env.testing
+-rw-r--r--   0        0        0      195 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/local_var_in_path/Taskfile.yml
+-rw-r--r--   0        0        0      131 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv/missing_env/Taskfile.yml
+-rw-r--r--   0        0        0        8 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv_task/default/.env
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv_task/default/.gitignore
+-rw-r--r--   0        0        0      456 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dotenv_task/default/Taskfile.yml
+-rw-r--r--   0        0        0       63 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dry/Taskfile.yml
+-rw-r--r--   0        0        0      121 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dry_checksum/Taskfile.yml
+-rw-r--r--   0        0        0       13 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/dry_checksum/source.txt
+-rw-r--r--   0        0        0       32 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/empty_task/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.333712 go_task_bin-3.37.0/task/testdata/env/.gitignore
+-rw-r--r--   0        0        0      499 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/env/Taskfile.yml
+-rw-r--r--   0        0        0      101 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/error_code/Taskfile.yml
+-rw-r--r--   0        0        0      280 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/evaluate_symlinks_in_paths/Taskfile.yaml
+-rw-r--r--   0        0        0       19 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/evaluate_symlinks_in_paths/shared/b
+-rw-r--r--   0        0        0       25 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/evaluate_symlinks_in_paths/shared/inner_shared/c
+-rw-r--r--   0        0        0       12 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/evaluate_symlinks_in_paths/src/a
+-rw-r--r--   0        0        0       89 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/exit_immediately/Taskfile.yml
+-rw-r--r--   0        0        0       80 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/expand/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/file_names/.gitignore
+-rw-r--r--   0        0        0       58 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/file_names/Taskfile.dist.yaml/Taskfile.dist.yaml
+-rw-r--r--   0        0        0       58 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/file_names/Taskfile.dist.yml/Taskfile.dist.yml
+-rw-r--r--   0        0        0       58 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/file_names/Taskfile.yaml/Taskfile.yaml
+-rw-r--r--   0        0        0       58 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/file_names/Taskfile.yml/Taskfile.yml
+-rw-r--r--   0        0        0     1635 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/cmds/Taskfile.yml
+-rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/cmds/bar.txt
+-rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/cmds/foo.txt
+-rw-r--r--   0        0        0     1876 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/deps/Taskfile.yml
+-rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/deps/bar.txt
+-rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/for/deps/foo.txt
+-rw-r--r--   0        0        0      295 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/force/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/generates/.gitignore
+-rw-r--r--   0        0        0      986 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/generates/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/generates/sub/.keep
+-rw-r--r--   0        0        0      262 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_errors/Taskfile.yml
+-rw-r--r--   0        0        0       80 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_nil_elements/cmds/Taskfile.yml
+-rw-r--r--   0        0        0      116 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_nil_elements/deps/Taskfile.yml
+-rw-r--r--   0        0        0       94 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_nil_elements/includes/Taskfile.yml
+-rw-r--r--   0        0        0       81 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_nil_elements/includes/inc.yml
+-rw-r--r--   0        0        0      123 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_nil_elements/preconditions/Taskfile.yml
+-rw-r--r--   0        0        0       66 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/ignore_signals/Taskfile.yml
+-rw-r--r--   0        0        0      388 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars/Taskfile.yml
+-rw-r--r--   0        0        0      229 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars/include/Taskfile.include1.yml
+-rw-r--r--   0        0        0      229 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars/include/Taskfile.include2.yml
+-rw-r--r--   0        0        0      229 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars/include/Taskfile.include3.yml
+-rw-r--r--   0        0        0      266 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars_multi_level/Taskfile.yml
+-rw-r--r--   0        0        0       97 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars_multi_level/bar/Taskfile.yml
+-rw-r--r--   0        0        0       97 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars_multi_level/foo/Taskfile.yml
+-rw-r--r--   0        0        0      130 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/include_with_vars_multi_level/lib/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/.gitignore
+-rw-r--r--   0        0        0      768 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/Taskfile.yml
+-rw-r--r--   0        0        0       93 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/Taskfile2.yml
+-rw-r--r--   0        0        0       55 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/Taskfile_darwin.yml
+-rw-r--r--   0        0        0       55 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/Taskfile_linux.yml
+-rw-r--r--   0        0        0       55 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/Taskfile_windows.yml
+-rw-r--r--   0        0        0       95 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/included/Taskfile.yml
+-rw-r--r--   0        0        0      225 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/module1/Taskfile.yml
+-rw-r--r--   0        0        0      213 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes/module2/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_call_root_task/.gitignore
+-rw-r--r--   0        0        0      122 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_call_root_task/Taskfile.yml
+-rw-r--r--   0        0        0       69 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_call_root_task/Taskfile2.yml
+-rw-r--r--   0        0        0      173 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_cycle/Taskfile.yml
+-rw-r--r--   0        0        0      109 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_cycle/one/Taskfile.yml
+-rw-r--r--   0        0        0      109 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_cycle/one/two/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_deps/.gitignore
+-rw-r--r--   0        0        0      110 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_deps/Taskfile.yml
+-rw-r--r--   0        0        0      267 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_deps/Taskfile2.yml
+-rw-r--r--   0        0        0        9 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_empty/.gitignore
+-rw-r--r--   0        0        0       50 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_empty/Taskfile.yml
+-rw-r--r--   0        0        0      125 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_empty/Taskfile2.yml
+-rw-r--r--   0        0        0       51 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_incorrect/Taskfile.yml
+-rw-r--r--   0        0        0       28 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_incorrect/incomplete.yml
+-rw-r--r--   0        0        0      188 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_internal/Taskfile.yml
+-rw-r--r--   0        0        0       70 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_internal/Taskfile2.yml
+-rw-r--r--   0        0        0      101 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_interpolation/include/Taskfile.yml
+-rw-r--r--   0        0        0      155 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_interpolation/include_with_dir/Taskfile.yml
+-rw-r--r--   0        0        0       83 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_interpolation/include_with_env_variable/Taskfile.yml
+-rw-r--r--   0        0        0       66 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_interpolation/included/Taskfile.yml
+-rw-r--r--   0        0        0      161 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/Taskfile.yml
+-rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/called_one.txt
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/called_three.txt
+-rw-r--r--   0        0        0        4 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/called_two.txt
+-rw-r--r--   0        0        0       85 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/one/Taskfile.yml
+-rw-r--r--   0        0        0      101 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/one/two/Taskfile.yml
+-rw-r--r--   0        0        0       62 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_multi_level/one/two/three/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_optional/.gitignore
+-rw-r--r--   0        0        0      162 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_optional/Taskfile.yml
+-rw-r--r--   0        0        0      149 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_optional_explicit_false/Taskfile.yml
+-rw-r--r--   0        0        0      115 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_optional_implicit_false/Taskfile.yml
+-rw-r--r--   0        0        0      133 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_rel_path/Taskfile.yml
+-rw-r--r--   0        0        0       32 2024-05-09 01:39:39.337712 go_task_bin-3.37.0/task/testdata/includes_rel_path/common/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_rel_path/included/Taskfile.yml
+-rw-r--r--   0        0        0      129 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_shadowed_default/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_shadowed_default/Taskfile2.yml
+-rw-r--r--   0        0        0        9 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_shadowed_default/file.txt
+-rw-r--r--   0        0        0       64 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_unshadowed_default/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_unshadowed_default/Taskfile2.yml
+-rw-r--r--   0        0        0        9 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_unshadowed_default/file.txt
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_yaml/.gitignore
+-rw-r--r--   0        0        0      226 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_yaml/Custom.ext
+-rw-r--r--   0        0        0      115 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_yaml/included/Taskfile.yaml
+-rw-r--r--   0        0        0      109 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/includes_yaml/included/custom.yaml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/init/.gitignore
+-rw-r--r--   0        0        0      167 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/internal_task/Taskfile.yml
+-rw-r--r--   0        0        0       77 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/label_list/Taskfile.yml
+-rw-r--r--   0        0        0       76 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/label_status/Taskfile.yml
+-rw-r--r--   0        0        0      104 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/label_summary/Taskfile.yml
+-rw-r--r--   0        0        0       82 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/label_uptodate/Taskfile.yml
+-rw-r--r--   0        0        0      105 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/label_var/Taskfile.yml
+-rw-r--r--   0        0        0       90 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/list_desc_interpolation/Taskfile.yml
+-rw-r--r--   0        0        0      164 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/list_mixed_desc/Taskfile.yml
+-rw-r--r--   0        0        0      199 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/output_group/Taskfile.yml
+-rw-r--r--   0        0        0      255 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/output_group_error_only/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/params/.gitignore
+-rw-r--r--   0        0        0     1255 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/params/Taskfile.yml
+-rw-r--r--   0        0        0     1584 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/platforms/Taskfile.yml
+-rw-r--r--   0        0        0      285 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/precondition/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/precondition/foo.txt
+-rw-r--r--   0        0        0      226 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/prompt/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/run/.gitignore
+-rw-r--r--   0        0        0      468 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/run/Taskfile.yml
+-rw-r--r--   0        0        0      201 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/shopts/command_level/Taskfile.yml
+-rw-r--r--   0        0        0      175 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/shopts/global_level/Taskfile.yml
+-rw-r--r--   0        0        0      183 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/shopts/task_level/Taskfile.yml
+-rw-r--r--   0        0        0      174 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/short_task_notation/Taskfile.yml
+-rw-r--r--   0        0        0     1350 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/silent/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/single_cmd_dep/.gitignore
+-rw-r--r--   0        0        0       99 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/single_cmd_dep/Taskfile.yml
+-rw-r--r--   0        0        0      282 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/special_vars/Taskfile.yml
+-rw-r--r--   0        0        0      214 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/special_vars/included/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/special_vars/subdir/.gitkeep
+-rw-r--r--   0        0        0       92 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/split_args/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/status/.gitignore
+-rw-r--r--   0        0        0      331 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/status/Taskfile.yml
+-rw-r--r--   0        0        0       14 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/status_vars/.gitignore
+-rw-r--r--   0        0        0      170 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/status_vars/Taskfile.yml
+-rw-r--r--   0        0        0       14 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/status_vars/source.txt
+-rw-r--r--   0        0        0      566 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/summary/Taskfile.yml
+-rw-r--r--   0        0        0      346 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/summary/task-with-summary.txt
+-rw-r--r--   0        0        0       78 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/taskfile_walk/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/taskfile_walk/foo/bar/.gitkeep
+-rw-r--r--   0        0        0       96 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/user_working_dir/Taskfile.yml
+-rw-r--r--   0        0        0       74 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/user_working_dir_with_includes/Taskfile.yml
+-rw-r--r--   0        0        0      101 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/user_working_dir_with_includes/included/Taskfile.yml
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/user_working_dir_with_includes/somedir/.keep
+-rw-r--r--   0        0        0       27 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/.env
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/.gitignore
+-rw-r--r--   0        0        0     1008 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/Taskfile.yml
+-rw-r--r--   0        0        0     2188 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/any/Taskfile.yml
+-rw-r--r--   0        0        0     2791 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/any2/Taskfile.yml
+-rw-r--r--   0        0        0      276 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/any2/example.json
+-rw-r--r--   0        0        0      111 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/vars/any2/example.yaml
+-rw-r--r--   0        0        0       93 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/version/v1/Taskfile.yml
+-rw-r--r--   0        0        0       93 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/version/v2/Taskfile.yml
+-rw-r--r--   0        0        0       93 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/version/v3/Taskfile.yml
+-rw-r--r--   0        0        0        6 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/watcher_interval/.gitignore
+-rw-r--r--   0        0        0      194 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/watcher_interval/Taskfile.yaml
+-rw-r--r--   0        0        0      519 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/testdata/wildcards/Taskfile.yml
+-rw-r--r--   0        0        0     9281 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/variables.go
+-rw-r--r--   0        0        0     4215 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/watch.go
+-rw-r--r--   0        0        0     2041 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/watch_test.go
+-rw-r--r--   0        0        0      238 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/.gitignore
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/.nojekyll
+-rw-r--r--   0        0        0     1523 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/Taskfile.yml
+-rw-r--r--   0        0        0       70 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/babel.config.ts
+-rw-r--r--   0        0        0     6841 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/blog/2023-09-02-introducing-experiments.mdx
+-rw-r--r--   0        0        0     4459 2024-05-09 01:39:39.341712 go_task_bin-3.37.0/task/website/blog/2024-04-09-variables.mdx
+-rw-r--r--   0        0        0      279 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/blog/authors.yml
+-rw-r--r--   0        0        0      242 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/constants.ts
+-rw-r--r--   0        0        0      359 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/crowdin.yml
+-rw-r--r--   0        0        0    41801 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/api_reference.mdx
+-rw-r--r--   0        0        0    38814 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/changelog.mdx
+-rw-r--r--   0        0        0     1529 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/community.mdx
+-rw-r--r--   0        0        0     7804 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/contributing.mdx
+-rw-r--r--   0        0        0      711 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/deprecations/deprecations.mdx
+-rw-r--r--   0        0        0      655 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/deprecations/template.mdx
+-rw-r--r--   0        0        0     1245 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/deprecations/version_2_schema.mdx
+-rw-r--r--   0        0        0     5677 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/experiments/experiments.mdx
+-rw-r--r--   0        0        0     1540 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/experiments/gentle_force.mdx
+-rw-r--r--   0        0        0     7895 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/experiments/map_variables.mdx
+-rw-r--r--   0        0        0     4706 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/experiments/remote_taskfiles.mdx
+-rw-r--r--   0        0        0     1128 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/experiments/template.mdx
+-rw-r--r--   0        0        0     2583 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/faq.mdx
+-rw-r--r--   0        0        0     6930 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/installation.mdx
+-rw-r--r--   0        0        0     2911 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/integrations.mdx
+-rw-r--r--   0        0        0     1993 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/intro.mdx
+-rw-r--r--   0        0        0     2797 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/releasing.mdx
+-rw-r--r--   0        0        0     2974 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/styleguide.mdx
+-rw-r--r--   0        0        0     5473 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/taskfile_versions.mdx
+-rw-r--r--   0        0        0      763 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/translate.mdx
+-rw-r--r--   0        0        0    46204 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docs/usage.mdx
+-rw-r--r--   0        0        0     5155 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/docusaurus.config.ts
+-rw-r--r--   0        0        0     1508 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/package.json
+-rw-r--r--   0        0        0      208 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/prettier.config.js
+-rw-r--r--   0        0        0      271 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/sidebars.ts
+-rw-r--r--   0        0        0     1050 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/api/crowdin.js
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/components/.keep
+-rw-r--r--   0        0        0     1202 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/css/carbon.css
+-rw-r--r--   0        0        0     3089 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/css/custom.css
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/pages/.keep
+-rw-r--r--   0        0        0     1922 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/pages/donate.md
+-rw-r--r--   0        0        0     1342 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/themes/prismDark.js
+-rw-r--r--   0        0        0     1679 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/src/themes/prismLight.js
+-rw-r--r--   0        0        0        0 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/.nojekyll
+-rw-r--r--   0        0        0       13 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/CNAME
+-rw-r--r--   0        0        0      109 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/Taskfile.yml
+-rw-r--r--   0        0        0     7281 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/appwrite.svg
+-rw-r--r--   0        0        0   173915 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/favicon.ico
+-rw-r--r--   0        0        0     1321 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/icon-discord.svg
+-rw-r--r--   0        0        0     1227 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/icon-github.svg
+-rw-r--r--   0        0        0     1717 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/icon-mastodon.svg
+-rw-r--r--   0        0        0     1742 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/icon-twitter.svg
+-rw-r--r--   0        0        0    13524 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/logo.png
+-rw-r--r--   0        0        0      435 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/logo.svg
+-rw-r--r--   0        0        0      360 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/logo_mono.svg
+-rw-r--r--   0        0        0    19847 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/og-image.png
+-rw-r--r--   0        0        0     1276 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/img/pix.png
+-rwxr-xr-x   0        0        0     9634 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/install.sh
+-rw-r--r--   0        0        0      784 2024-05-09 01:39:39.345712 go_task_bin-3.37.0/task/website/static/js/carbon.js
+-rw-r--r--   0        0        0    22415 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/static/schema.json
+-rw-r--r--   0        0        0       87 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/tsconfig.json
+-rw-r--r--   0        0        0    41801 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/api_reference.mdx
+-rw-r--r--   0        0        0    38814 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/changelog.mdx
+-rw-r--r--   0        0        0     1529 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/community.mdx
+-rw-r--r--   0        0        0     7804 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/contributing.mdx
+-rw-r--r--   0        0        0      711 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/deprecations.mdx
+-rw-r--r--   0        0        0      655 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/template.mdx
+-rw-r--r--   0        0        0     1245 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/version_2_schema.mdx
+-rw-r--r--   0        0        0     5677 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/experiments.mdx
+-rw-r--r--   0        0        0     1540 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/gentle_force.mdx
+-rw-r--r--   0        0        0     7895 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/map_variables.mdx
+-rw-r--r--   0        0        0     4706 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/remote_taskfiles.mdx
+-rw-r--r--   0        0        0     1128 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/template.mdx
+-rw-r--r--   0        0        0     2583 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/faq.mdx
+-rw-r--r--   0        0        0     6930 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/installation.mdx
+-rw-r--r--   0        0        0     2911 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/integrations.mdx
+-rw-r--r--   0        0        0     1993 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/intro.mdx
+-rw-r--r--   0        0        0     2797 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/releasing.mdx
+-rw-r--r--   0        0        0     2974 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/styleguide.mdx
+-rw-r--r--   0        0        0     5473 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/taskfile_versions.mdx
+-rw-r--r--   0        0        0      763 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/translate.mdx
+-rw-r--r--   0        0        0    46204 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_docs/version-latest/usage.mdx
+-rw-r--r--   0        0        0      174 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versioned_sidebars/version-latest-sidebars.json
+-rw-r--r--   0        0        0       15 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/versions.json
+-rw-r--r--   0        0        0   364377 2024-05-09 01:39:39.349712 go_task_bin-3.37.0/task/website/yarn.lock
+-rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 go_task_bin-3.37.0/PKG-INFO
```

### Comparing `go_task_bin-3.36.0/LICENSE` & `go_task_bin-3.37.0/LICENSE`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/README.md` & `go_task_bin-3.37.0/README.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/pdm_build.py` & `go_task_bin-3.37.0/pdm_build.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from wheel.cli.tags import tags
 
 if TYPE_CHECKING:
     from pdm.backend.hooks import Context
 
 NAME = "task"
-VERSION = "3.36.0"
+VERSION = "3.37.0"
 
 
 def is_windows():
     if "GOOS" in os.environ:
         return os.environ["GOOS"] == "windows"
     return sys.platform == "win32"
```

### Comparing `go_task_bin-3.36.0/pyproject.toml` & `go_task_bin-3.37.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "go-task-bin"
 description = "task - A task runner / simpler Make alternative written in Go"
-version = "3.36.0"
+version = "3.37.0"
 authors = [
     { name = "dowon", email = "ks2515@naver.com" },
 ]
 dependencies = []
 requires-python = ">=3.8"
 readme = "README.md"
 keywords = [
```

### Comparing `go_task_bin-3.36.0/task/.github/CODE_OF_CONDUCT.md` & `go_task_bin-3.37.0/task/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/.github/CONTRIBUTING.md` & `go_task_bin-3.37.0/task/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/.github/ISSUE_TEMPLATE/config.yml` & `go_task_bin-3.37.0/task/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/.github/workflows/issue-awaiting-response.yml` & `go_task_bin-3.37.0/task/.github/workflows/issue-awaiting-response.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/.github/workflows/issue-closed.yml` & `go_task_bin-3.37.0/task/.github/workflows/issue-closed.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/.github/workflows/issue-experiment.yml` & `go_task_bin-3.37.0/task/.github/workflows/issue-experiment.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/.github/workflows/issue-needs-triage.yml` & `go_task_bin-3.37.0/task/.github/workflows/issue-needs-triage.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/.github/workflows/lint.yml` & `go_task_bin-3.37.0/task/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/.github/workflows/test.yml` & `go_task_bin-3.37.0/task/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/.github/workflows/upload-source-documents.yml` & `go_task_bin-3.37.0/task/.github/workflows/upload-source-documents.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/.goreleaser.yml` & `go_task_bin-3.37.0/task/.goreleaser.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/CHANGELOG.md` & `go_task_bin-3.37.0/task/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,30 @@
 # Changelog
 
+## v3.37.0 - 2024-05-08
+
+- Released the
+  [Any Variables experiment](https://taskfile.dev/blog/any-variables), but
+  [_without support for maps_](https://github.com/go-task/task/issues/1415#issuecomment-2044756925)
+  (#1415, #1547 by @pd93).
+- Refactored how Task reads, parses and merges Taskfiles using a DAG (#1563,
+  #1607 by @pd93).
+- Fix a bug which stopped tasks from using `stdin` as input (#1593, #1623 by
+  @pd03).
+- Fix error when a file or directory in the project contained a special char
+  like `&`, `(` or `)` (#1551, #1584 by @andreynering).
+- Added alias `q` for template function `shellQuote` (#1601, #1603 by @vergenzt)
+- Added support for `~` on ZSH completions (#1613 by @jwater7).
+- Added the ability to pass variables by reference using Go template syntax when
+  the
+  [Map Variables experiment](https://taskfile.dev/experiments/map-variables/) is
+  enabled (#1612 by @pd93).
+- Added support for environment variables in the templating engine in `includes`
+  (#1610 by @vmaerten).
+
 ## v3.36.0 - 2024-04-08
 
 - Added support for
   [looping over dependencies](https://taskfile.dev/usage/#looping-over-dependencies)
   (#1299, #1541 by @pd93).
 - When using the
   "[Remote Taskfiles](https://taskfile.dev/experiments/remote-taskfiles/)"
```

### Comparing `go_task_bin-3.36.0/task/LICENSE` & `go_task_bin-3.37.0/task/LICENSE`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/README.md` & `go_task_bin-3.37.0/task/README.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/Taskfile.yml` & `go_task_bin-3.37.0/task/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/args/args.go` & `go_task_bin-3.37.0/task/args/args.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/args/args_test.go` & `go_task_bin-3.37.0/task/args/args_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/cmd/release/main.go` & `go_task_bin-3.37.0/task/cmd/release/main.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/cmd/sleepit/sleepit.go` & `go_task_bin-3.37.0/task/cmd/sleepit/sleepit.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/cmd/task/task.go` & `go_task_bin-3.37.0/task/cmd/task/task.go`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 package main
 
 import (
 	"context"
 	"fmt"
-	"log"
 	"os"
 	"strings"
 
 	"github.com/spf13/pflag"
 	"mvdan.cc/sh/v3/syntax"
 
 	"github.com/go-task/task/v3"
@@ -40,16 +39,20 @@
 		l.Errf(logger.Red, "%v\n", err)
 		os.Exit(errors.CodeUnknown)
 	}
 	os.Exit(errors.CodeOk)
 }
 
 func run() error {
-	log.SetFlags(0)
-	log.SetOutput(os.Stderr)
+	logger := &logger.Logger{
+		Stdout:  os.Stdout,
+		Stderr:  os.Stderr,
+		Verbose: flags.Verbose,
+		Color:   flags.Color,
+	}
 
 	if err := flags.Validate(); err != nil {
 		return err
 	}
 
 	dir := flags.Dir
 	entrypoint := flags.Entrypoint
@@ -61,30 +64,24 @@
 
 	if flags.Help {
 		pflag.Usage()
 		return nil
 	}
 
 	if flags.Experiments {
-		l := &logger.Logger{
-			Stdout:  os.Stdout,
-			Stderr:  os.Stderr,
-			Verbose: flags.Verbose,
-			Color:   flags.Color,
-		}
-		return experiments.List(l)
+		return experiments.List(logger)
 	}
 
 	if flags.Init {
 		wd, err := os.Getwd()
 		if err != nil {
-			log.Fatal(err)
+			return err
 		}
 		if err := task.InitTaskfile(os.Stdout, wd); err != nil {
-			log.Fatal(err)
+			return err
 		}
 		return nil
 	}
 
 	if flags.Global {
 		home, err := os.UserHomeDir()
 		if err != nil {
@@ -134,14 +131,18 @@
 		return err
 	}
 
 	if err := e.Setup(); err != nil {
 		return err
 	}
 
+	if experiments.AnyVariables.Enabled {
+		logger.Warnf("The 'Any Variables' experiment flag is no longer required to use non-map variable types. If you wish to use map variables, please use 'TASK_X_MAP_VARIABLES' instead. See https://github.com/go-task/task/issues/1585\n")
+	}
+
 	// If the download flag is specified, we should stop execution as soon as
 	// taskfile is downloaded
 	if flags.Download {
 		return nil
 	}
 
 	if (listOptions.ShouldListTasks()) && flags.Silent {
@@ -174,15 +175,15 @@
 	// If there are no calls, run the default task instead
 	if len(calls) == 0 {
 		calls = append(calls, &ast.Call{Task: "default"})
 	}
 
 	globals.Set("CLI_ARGS", ast.Var{Value: cliArgs})
 	globals.Set("CLI_FORCE", ast.Var{Value: flags.Force || flags.ForceAll})
-	e.Taskfile.Vars.Merge(globals)
+	e.Taskfile.Vars.Merge(globals, nil)
 
 	if !flags.Watch {
 		e.InterceptInterruptSignals()
 	}
 
 	ctx := context.Background()
```

### Comparing `go_task_bin-3.36.0/task/completion/bash/task.bash` & `go_task_bin-3.37.0/task/completion/bash/task.bash`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/completion/fish/task.fish` & `go_task_bin-3.37.0/task/completion/fish/task.fish`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/completion/ps/task.ps1` & `go_task_bin-3.37.0/task/completion/ps/task.ps1`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/completion/zsh/_task` & `go_task_bin-3.37.0/task/completion/zsh/_task`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 # Listing commands from Taskfile.yml
 function __task_list() {
     local -a scripts cmd
     local -i enabled=0
     local taskfile item task desc
 
     cmd=(task)
-    taskfile="${(v)opt_args[(i)-t|--taskfile]}"
+    taskfile=${(Qv)opt_args[(i)-t|--taskfile]}
+    taskfile=${taskfile//\~/$HOME}
+
 
     if [[ -n "$taskfile" && -f "$taskfile" ]]; then
         enabled=1
         cmd+=(--taskfile "$taskfile")
     else
         for taskfile in {T,t}askfile{,.dist}.{yaml,yml}; do
             if [[ -f "$taskfile" ]]; then
```

### Comparing `go_task_bin-3.36.0/task/errors/errors.go` & `go_task_bin-3.37.0/task/errors/errors.go`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 	CodeTaskfileInvalid
 	CodeTaskfileFetchFailed
 	CodeTaskfileNotTrusted
 	CodeTaskfileNotSecure
 	CodeTaskfileCacheNotFound
 	CodeTaskfileVersionCheckError
 	CodeTaskfileNetworkTimeout
+	_ // CodeTaskfileDuplicateInclude
+	CodeTaskfileCycle
 )
 
 // Task related exit codes
 const (
 	CodeTaskNotFound int = iota + 200
 	CodeTaskRunError
 	CodeTaskInternal
```

### Comparing `go_task_bin-3.36.0/task/errors/errors_task.go` & `go_task_bin-3.37.0/task/errors/errors_task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/errors/errors_taskfile.go` & `go_task_bin-3.37.0/task/errors/errors_taskfile.go`

 * *Files 2% similar despite different names*

```diff
@@ -170,7 +170,25 @@
 		err.Timeout, err.URI, cacheText,
 	)
 }
 
 func (err *TaskfileNetworkTimeoutError) Code() int {
 	return CodeTaskfileNetworkTimeout
 }
+
+// TaskfileCycleError is returned when we detect that a Taskfile includes a
+// set of Taskfiles that include each other in a cycle.
+type TaskfileCycleError struct {
+	Source      string
+	Destination string
+}
+
+func (err TaskfileCycleError) Error() string {
+	return fmt.Sprintf("task: include cycle detected between %s <--> %s",
+		err.Source,
+		err.Destination,
+	)
+}
+
+func (err TaskfileCycleError) Code() int {
+	return CodeTaskfileCycle
+}
```

### Comparing `go_task_bin-3.36.0/task/go.mod` & `go_task_bin-3.37.0/task/go.mod`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 module github.com/go-task/task/v3
 
-go 1.21
+go 1.21.0
 
 require (
 	github.com/Masterminds/semver/v3 v3.2.1
 	github.com/davecgh/go-spew v1.1.1
+	github.com/dominikbraun/graph v0.23.0
 	github.com/fatih/color v1.16.0
 	github.com/go-task/slim-sprig/v3 v3.0.0
+	github.com/go-task/template v0.0.0-20240422130016-8f6b279b1e90
 	github.com/joho/godotenv v1.5.1
 	github.com/mattn/go-zglob v0.0.4
 	github.com/mitchellh/hashstructure/v2 v2.0.2
 	github.com/otiai10/copy v1.14.0
 	github.com/radovskyb/watcher v1.0.7
 	github.com/sajari/fuzzy v1.0.0
 	github.com/spf13/pflag v1.0.5
```

### Comparing `go_task_bin-3.36.0/task/go.sum` & `go_task_bin-3.37.0/task/go.sum`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 github.com/Masterminds/semver/v3 v3.2.1 h1:RN9w6+7QoMeJVGyfmbcgs28Br8cvmnucEXnY0rYXWg0=
 github.com/Masterminds/semver/v3 v3.2.1/go.mod h1:qvl/7zhW3nngYb5+80sSMF+FG2BjYrf8m9wsX0PNOMQ=
 github.com/creack/pty v1.1.21 h1:1/QdRyBaHHJP61QkWMXlOIBfsgdDeeKfK8SYVUWJKf0=
 github.com/creack/pty v1.1.21/go.mod h1:MOBLtS5ELjhRRrroQr9kyvTxUAFNvYEK993ew/Vr4O4=
 github.com/davecgh/go-spew v1.1.1 h1:vj9j/u1bqnvCEfJOwUhtlOARqs3+rkHYY13jYWTU97c=
 github.com/davecgh/go-spew v1.1.1/go.mod h1:J7Y8YcW2NihsgmVo/mv3lAwl/skON4iLHjSsI+c5H38=
+github.com/dominikbraun/graph v0.23.0 h1:TdZB4pPqCLFxYhdyMFb1TBdFxp8XLcJfTTBQucVPgCo=
+github.com/dominikbraun/graph v0.23.0/go.mod h1:yOjYyogZLY1LSG9E33JWZJiq5k83Qy2C6POAuiViluc=
 github.com/fatih/color v1.16.0 h1:zmkK9Ngbjj+K0yRhTVONQh1p/HknKYSlNT+vZCzyokM=
 github.com/fatih/color v1.16.0/go.mod h1:fL2Sau1YI5c0pdGEVCbKQbLXB6edEj1ZgiY4NijnWvE=
 github.com/frankban/quicktest v1.14.6 h1:7Xjx+VpznH+oBnejlPUj8oUpdxnVs4f8XU8WnHkI4W8=
 github.com/frankban/quicktest v1.14.6/go.mod h1:4ptaffx2x8+WTWXmUCuVU6aPUX1/Mz7zb5vbUoiM6w0=
 github.com/go-task/slim-sprig/v3 v3.0.0 h1:sUs3vkvUymDpBKi3qH1YSqBQk9+9D/8M2mN1vB6EwHI=
 github.com/go-task/slim-sprig/v3 v3.0.0/go.mod h1:W848ghGpv3Qj3dhTPRyJypKRiqCdHZiAzKg9hl15HA8=
+github.com/go-task/template v0.0.0-20240422130016-8f6b279b1e90 h1:JBbiZ2CXIZ9Upe3O2yI5+3ksWoa7hNVNi4BINs8TIrs=
+github.com/go-task/template v0.0.0-20240422130016-8f6b279b1e90/go.mod h1:RgwRaZK+kni/hJJ7/AaOE2lPQFPbAdji/DyhC6pxo4k=
 github.com/google/go-cmp v0.6.0 h1:ofyhxvXcZhMsU5ulbFiLKl/XBFqE1GSq7atu8tAmTRI=
 github.com/google/go-cmp v0.6.0/go.mod h1:17dUlkBOakJ0+DkrSSNjCkIjxS6bF9zb3elmeNGIjoY=
 github.com/joho/godotenv v1.5.1 h1:7eLL/+HRGLY0ldzfGMeQkb7vMd0as4CfYvUVzLqw0N0=
 github.com/joho/godotenv v1.5.1/go.mod h1:f4LDr5Voq0i2e/R5DDNOoa2zzDfwtkZa6DnEwAbqwq4=
 github.com/klauspost/cpuid/v2 v2.0.9 h1:lgaqFMSdTdQYdZ04uHyN2d/eKdOMyi2YLSvlQIBFYa4=
 github.com/klauspost/cpuid/v2 v2.0.9/go.mod h1:FInQzS24/EEf25PyTYn52gqo7WaD8xa0213Md/qVLRg=
 github.com/kr/pretty v0.3.1 h1:flRD4NNwYAUpkphVc1HcthR4KEIFJ65n8Mw5qdRn3LE=
```

### Comparing `go_task_bin-3.36.0/task/help.go` & `go_task_bin-3.37.0/task/help.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/init.go` & `go_task_bin-3.37.0/task/init.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/install-task.sh` & `go_task_bin-3.37.0/task/install-task.sh`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/compiler/compiler.go` & `go_task_bin-3.37.0/task/internal/compiler/compiler.go`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,14 @@
 	}
 
 	getRangeFunc := func(dir string) func(k string, v ast.Var) error {
 		return func(k string, v ast.Var) error {
 			cache := &templater.Cache{Vars: result}
 			// Replace values
 			newVar := templater.ReplaceVar(v, cache)
-			// If the variable is a reference, we can resolve it
-			if newVar.Ref != "" {
-				newVar.Value = result.Get(newVar.Ref).Value
-			}
 			// If the variable should not be evaluated, but is nil, set it to an empty string
 			// This stops empty interface errors when using the templater to replace values later
 			if !evaluateShVars && newVar.Value == nil {
 				result.Set(k, ast.Var{Value: ""})
 				return nil
 			}
 			// If the variable should not be evaluated and it is set, we can set it and return
```

### Comparing `go_task_bin-3.36.0/task/internal/deepcopy/deepcopy.go` & `go_task_bin-3.37.0/task/internal/deepcopy/deepcopy.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/editors/output.go` & `go_task_bin-3.37.0/task/internal/editors/output.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/execext/exec.go` & `go_task_bin-3.37.0/task/internal/execext/exec.go`

 * *Files 12% similar despite different names*

```diff
@@ -99,14 +99,17 @@
 }
 
 // Expand is a helper to mvdan.cc/shell.Fields that returns the first field
 // if available.
 func Expand(s string) (string, error) {
 	s = filepath.ToSlash(s)
 	s = strings.ReplaceAll(s, " ", `\ `)
+	s = strings.ReplaceAll(s, "&", `\&`)
+	s = strings.ReplaceAll(s, "(", `\(`)
+	s = strings.ReplaceAll(s, ")", `\)`)
 	fields, err := shell.Fields(s, nil)
 	if err != nil {
 		return "", err
 	}
 	if len(fields) > 0 {
 		return fields[0], nil
 	}
```

### Comparing `go_task_bin-3.36.0/task/internal/exp/maps.go` & `go_task_bin-3.37.0/task/internal/exp/maps.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/experiments/experiments.go` & `go_task_bin-3.37.0/task/internal/experiments/experiments.go`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,23 @@
 }
 
 // A list of experiments.
 var (
 	GentleForce     Experiment
 	RemoteTaskfiles Experiment
 	AnyVariables    Experiment
+	MapVariables    Experiment
 )
 
 func init() {
 	readDotEnv()
 	GentleForce = New("GENTLE_FORCE")
 	RemoteTaskfiles = New("REMOTE_TASKFILES")
 	AnyVariables = New("ANY_VARIABLES", "1", "2")
+	MapVariables = New("MAP_VARIABLES", "1", "2")
 }
 
 func New(xName string, enabledValues ...string) Experiment {
 	if len(enabledValues) == 0 {
 		enabledValues = []string{"1"}
 	}
 	value := getEnv(xName)
@@ -97,10 +99,10 @@
 	l.FOutf(w, logger.Default, ": \t%s\n", x.String())
 }
 
 func List(l *logger.Logger) error {
 	w := tabwriter.NewWriter(os.Stdout, 0, 8, 0, ' ', 0)
 	printExperiment(w, l, GentleForce)
 	printExperiment(w, l, RemoteTaskfiles)
-	printExperiment(w, l, AnyVariables)
+	printExperiment(w, l, MapVariables)
 	return w.Flush()
 }
```

### Comparing `go_task_bin-3.36.0/task/internal/filepathext/filepathext.go` & `go_task_bin-3.37.0/task/internal/filepathext/filepathext.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/fingerprint/checker.go` & `go_task_bin-3.37.0/task/internal/fingerprint/checker.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/fingerprint/glob.go` & `go_task_bin-3.37.0/task/internal/fingerprint/glob.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/fingerprint/sources_checksum.go` & `go_task_bin-3.37.0/task/internal/fingerprint/sources_checksum.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/fingerprint/sources_timestamp.go` & `go_task_bin-3.37.0/task/internal/fingerprint/sources_timestamp.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/fingerprint/status.go` & `go_task_bin-3.37.0/task/internal/fingerprint/status.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/fingerprint/task.go` & `go_task_bin-3.37.0/task/internal/fingerprint/task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/fingerprint/task_test.go` & `go_task_bin-3.37.0/task/internal/fingerprint/task_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/flags/flags.go` & `go_task_bin-3.37.0/task/internal/flags/flags.go`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 package flags
 
 import (
 	"errors"
 	"log"
+	"os"
 	"time"
 
 	"github.com/spf13/pflag"
 
 	"github.com/go-task/task/v3/internal/experiments"
 	"github.com/go-task/task/v3/taskfile/ast"
 )
@@ -64,14 +65,16 @@
 	Experiments bool
 	Download    bool
 	Offline     bool
 	Timeout     time.Duration
 )
 
 func init() {
+	log.SetFlags(0)
+	log.SetOutput(os.Stderr)
 	pflag.Usage = func() {
 		log.Print(usage)
 		pflag.PrintDefaults()
 	}
 
 	pflag.BoolVar(&Version, "version", false, "Show Task version.")
 	pflag.BoolVarP(&Help, "help", "h", false, "Shows Task usage.")
```

### Comparing `go_task_bin-3.36.0/task/internal/goext/meta.go` & `go_task_bin-3.37.0/task/internal/goext/meta.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/logger/logger.go` & `go_task_bin-3.37.0/task/internal/logger/logger.go`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,18 @@
 // VerboseErrf prints stuff to STDERR if verbose mode is enabled.
 func (l *Logger) VerboseErrf(color Color, s string, args ...any) {
 	if l.Verbose {
 		l.Errf(color, s, args...)
 	}
 }
 
+func (l *Logger) Warnf(message string, args ...any) {
+	l.Errf(Yellow, message, args...)
+}
+
 func (l *Logger) Prompt(color Color, prompt string, defaultValue string, continueValues ...string) error {
 	if l.AssumeYes {
 		l.Outf(color, "%s [assuming yes]\n", prompt)
 		return nil
 	}
 
 	if !l.AssumeTerm && !term.IsTerminal() {
```

### Comparing `go_task_bin-3.36.0/task/internal/mocks/sources_checkable.go` & `go_task_bin-3.37.0/task/internal/mocks/sources_checkable.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/mocks/status_checkable.go` & `go_task_bin-3.37.0/task/internal/mocks/status_checkable.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/omap/orderedmap.go` & `go_task_bin-3.37.0/task/internal/omap/orderedmap.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/omap/orderedmap_test.go` & `go_task_bin-3.37.0/task/internal/omap/orderedmap_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/output/group.go` & `go_task_bin-3.37.0/task/internal/output/group.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/output/output.go` & `go_task_bin-3.37.0/task/internal/output/output.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/output/output_test.go` & `go_task_bin-3.37.0/task/internal/output/output_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/output/prefixed.go` & `go_task_bin-3.37.0/task/internal/output/prefixed.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/sort/sorter.go` & `go_task_bin-3.37.0/task/internal/sort/sorter.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/sort/sorter_test.go` & `go_task_bin-3.37.0/task/internal/sort/sorter_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/summary/summary.go` & `go_task_bin-3.37.0/task/internal/summary/summary.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/summary/summary_test.go` & `go_task_bin-3.37.0/task/internal/summary/summary_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/internal/templater/funcs.go` & `go_task_bin-3.37.0/task/internal/templater/funcs.go`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 package templater
 
 import (
 	"path/filepath"
 	"runtime"
 	"strings"
-	"text/template"
 
 	"github.com/davecgh/go-spew/spew"
 	"mvdan.cc/sh/v3/shell"
 	"mvdan.cc/sh/v3/syntax"
 
 	sprig "github.com/go-task/slim-sprig/v3"
+	"github.com/go-task/template"
 )
 
 var templateFuncs template.FuncMap
 
 func init() {
 	taskFuncs := template.FuncMap{
 		"OS":   func() string { return runtime.GOOS },
@@ -69,17 +69,21 @@
 			}
 			return result
 		},
 		"spew": func(v any) string {
 			return spew.Sdump(v)
 		},
 	}
+
+	// aliases
+	taskFuncs["q"] = taskFuncs["shellQuote"]
+
 	// Deprecated aliases for renamed functions.
 	taskFuncs["FromSlash"] = taskFuncs["fromSlash"]
 	taskFuncs["ToSlash"] = taskFuncs["toSlash"]
 	taskFuncs["ExeExt"] = taskFuncs["exeExt"]
 
-	templateFuncs = sprig.TxtFuncMap()
+	templateFuncs = template.FuncMap(sprig.TxtFuncMap())
 	for k, v := range taskFuncs {
 		templateFuncs[k] = v
 	}
 }
```

### Comparing `go_task_bin-3.36.0/task/internal/templater/templater.go` & `go_task_bin-3.37.0/task/internal/templater/templater.go`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 package templater
 
 import (
 	"bytes"
 	"maps"
 	"strings"
-	"text/template"
 
 	"github.com/go-task/task/v3/internal/deepcopy"
 	"github.com/go-task/task/v3/taskfile/ast"
+	"github.com/go-task/template"
 )
 
 // Cache is a help struct that allow us to call "replaceX" funcs multiple
 // times, without having to check for error each time. The first error that
 // happen will be assigned to r.err, and consecutive calls to funcs will just
 // return the zero value.
 type Cache struct {
@@ -25,14 +25,33 @@
 	r.cacheMap = r.Vars.ToCacheMap()
 }
 
 func (r *Cache) Err() error {
 	return r.err
 }
 
+func ResolveRef(ref string, cache *Cache) any {
+	// If there is already an error, do nothing
+	if cache.err != nil {
+		return nil
+	}
+
+	// Initialize the cache map if it's not already initialized
+	if cache.cacheMap == nil {
+		cache.cacheMap = cache.Vars.ToCacheMap()
+	}
+
+	val, err := template.ResolveRef(ref, cache.cacheMap)
+	if err != nil {
+		cache.err = err
+		return nil
+	}
+	return val
+}
+
 func Replace[T any](v T, cache *Cache) T {
 	return ReplaceWithExtra(v, cache, nil)
 }
 
 func ReplaceWithExtra[T any](v T, cache *Cache, extra map[string]any) T {
 	// If there is already an error, do nothing
 	if cache.err != nil {
@@ -87,14 +106,17 @@
 }
 
 func ReplaceVar(v ast.Var, cache *Cache) ast.Var {
 	return ReplaceVarWithExtra(v, cache, nil)
 }
 
 func ReplaceVarWithExtra(v ast.Var, cache *Cache, extra map[string]any) ast.Var {
+	if v.Ref != "" {
+		return ast.Var{Value: ResolveRef(v.Ref, cache)}
+	}
 	return ast.Var{
 		Value: ReplaceWithExtra(v.Value, cache, extra),
 		Sh:    ReplaceWithExtra(v.Sh, cache, extra),
 		Live:  v.Live,
 		Ref:   v.Ref,
 		Dir:   v.Dir,
 		Json:  ReplaceWithExtra(v.Json, cache, extra),
```

### Comparing `go_task_bin-3.36.0/task/package-lock.json` & `go_task_bin-3.37.0/task/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'version'": "'3.37.0'"}*

```diff
@@ -24,9 +24,9 @@
             },
             "integrity": "sha512-vQbdtBvesHm8EUFHX8QKg4rbBodmu9VsAXH1ozpbiN5jdTMOYHTCMM31EurAYmY+rNNtxJQ4JGy6t383RPlqbw==",
             "resolved": "https://registry.npmjs.org/@go-task/go-npm/-/go-npm-0.2.0.tgz",
             "version": "0.2.0"
         }
     },
     "requires": true,
-    "version": "3.36.0"
+    "version": "3.37.0"
 }
```

### Comparing `go_task_bin-3.36.0/task/package.json` & `go_task_bin-3.37.0/task/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'3.37.0'"}*

```diff
@@ -26,9 +26,9 @@
         "type": "git",
         "url": "https://github.com/go-task/task.git"
     },
     "scripts": {
         "postinstall": "go-npm install",
         "preuninstall": "go-npm uninstall"
     },
-    "version": "3.36.0"
+    "version": "3.37.0"
 }
```

### Comparing `go_task_bin-3.36.0/task/precondition.go` & `go_task_bin-3.37.0/task/precondition.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/requires.go` & `go_task_bin-3.37.0/task/requires.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/setup.go` & `go_task_bin-3.37.0/task/setup.go`

 * *Files 2% similar despite different names*

```diff
@@ -59,27 +59,30 @@
 		return nil, err
 	}
 	e.Dir = node.Dir()
 	return node, err
 }
 
 func (e *Executor) readTaskfile(node taskfile.Node) error {
-	var err error
-	e.Taskfile, err = taskfile.Read(
+	reader := taskfile.NewReader(
 		node,
 		e.Insecure,
 		e.Download,
 		e.Offline,
 		e.Timeout,
 		e.TempDir,
 		e.Logger,
 	)
+	graph, err := reader.Read()
 	if err != nil {
 		return err
 	}
+	if e.Taskfile, err = graph.Merge(); err != nil {
+		return err
+	}
 	return nil
 }
 
 func (e *Executor) setupFuzzyModel() {
 	if e.Taskfile != nil {
 		return
 	}
```

### Comparing `go_task_bin-3.36.0/task/signals.go` & `go_task_bin-3.37.0/task/signals.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/signals_test.go` & `go_task_bin-3.37.0/task/signals_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/status.go` & `go_task_bin-3.37.0/task/status.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/task.go` & `go_task_bin-3.37.0/task/task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/task_test.go` & `go_task_bin-3.37.0/task/task_test.go`

 * *Files 2% similar despite different names*

```diff
@@ -1195,23 +1195,25 @@
 	const dir = "testdata/includes_interpolation"
 	tests := []struct {
 		name           string
 		task           string
 		expectedErr    bool
 		expectedOutput string
 	}{
-		{"include", "include", false, "includes_interpolation\n"},
-		{"include with dir", "include-with-dir", false, "included\n"},
+		{"include", "include", false, "include\n"},
+		{"include_with_env_variable", "include-with-env-variable", false, "include_with_env_variable\n"},
+		{"include_with_dir", "include-with-dir", false, "included\n"},
 	}
+	t.Setenv("MODULE", "included")
 
 	for _, test := range tests {
 		t.Run(test.name, func(t *testing.T) {
 			var buff bytes.Buffer
 			e := task.Executor{
-				Dir:    dir,
+				Dir:    filepath.Join(dir, test.name),
 				Stdout: &buff,
 				Stderr: &buff,
 				Silent: true,
 			}
 			require.NoError(t, e.Setup())
 
 			err := e.Run(context.Background(), &ast.Call{Task: test.task})
```

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/cmd.go` & `go_task_bin-3.37.0/task/taskfile/ast/cmd.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/dep.go` & `go_task_bin-3.37.0/task/taskfile/ast/dep.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/for.go` & `go_task_bin-3.37.0/task/taskfile/ast/for.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/glob.go` & `go_task_bin-3.37.0/task/taskfile/ast/glob.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/include.go` & `go_task_bin-3.37.0/task/taskfile/ast/include.go`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	Aliases        []string
 	AdvancedImport bool
 	Vars           *Vars
 }
 
 // Includes represents information about included tasksfiles
 type Includes struct {
-	omap.OrderedMap[string, Include]
+	omap.OrderedMap[string, *Include]
 }
 
 // UnmarshalYAML implements the yaml.Unmarshaler interface.
 func (includes *Includes) UnmarshalYAML(node *yaml.Node) error {
 	switch node.Kind {
 	case yaml.MappingNode:
 		// NOTE(@andreynering): on this style of custom unmarshalling,
@@ -37,15 +37,15 @@
 			valueNode := node.Content[i+1]
 
 			var v Include
 			if err := valueNode.Decode(&v); err != nil {
 				return err
 			}
 			v.Namespace = keyNode.Value
-			includes.Set(keyNode.Value, v)
+			includes.Set(keyNode.Value, &v)
 		}
 		return nil
 	}
 
 	return fmt.Errorf("yaml: line %d: cannot unmarshal %s into included taskfiles", node.Line, node.ShortTag())
 }
 
@@ -54,15 +54,15 @@
 	if includes == nil {
 		return 0
 	}
 	return includes.OrderedMap.Len()
 }
 
 // Wrapper around OrderedMap.Set to ensure we don't get nil pointer errors
-func (includes *Includes) Range(f func(k string, v Include) error) error {
+func (includes *Includes) Range(f func(k string, v *Include) error) error {
 	if includes == nil {
 		return nil
 	}
 	return includes.OrderedMap.Range(f)
 }
 
 func (include *Include) UnmarshalYAML(node *yaml.Node) error {
```

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/output.go` & `go_task_bin-3.37.0/task/taskfile/ast/output.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/platforms.go` & `go_task_bin-3.37.0/task/taskfile/ast/platforms.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/platforms_test.go` & `go_task_bin-3.37.0/task/taskfile/ast/platforms_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/precondition.go` & `go_task_bin-3.37.0/task/taskfile/ast/precondition.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/precondition_test.go` & `go_task_bin-3.37.0/task/taskfile/ast/precondition_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/task.go` & `go_task_bin-3.37.0/task/taskfile/ast/task.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/taskfile.go` & `go_task_bin-3.37.0/task/taskfile/ast/taskfile.go`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 package ast
 
 import (
+	"errors"
 	"fmt"
 	"time"
 
 	"github.com/Masterminds/semver/v3"
 	"gopkg.in/yaml.v3"
 )
 
 // NamespaceSeparator contains the character that separates namespaces
 const NamespaceSeparator = ":"
 
 var V3 = semver.MustParse("3")
 
+// ErrIncludedTaskfilesCantHaveDotenvs is returned when a included Taskfile contains dotenvs
+var ErrIncludedTaskfilesCantHaveDotenvs = errors.New("task: Included Taskfiles can't have dotenv declarations. Please, move the dotenv declaration to the main Taskfile")
+
 // Taskfile is the abstract syntax tree for a Taskfile
 type Taskfile struct {
 	Location string
 	Version  *semver.Version
 	Output   Output
 	Method   string
 	Includes *Includes
@@ -32,26 +36,29 @@
 }
 
 // Merge merges the second Taskfile into the first
 func (t1 *Taskfile) Merge(t2 *Taskfile, include *Include) error {
 	if !t1.Version.Equal(t2.Version) {
 		return fmt.Errorf(`task: Taskfiles versions should match. First is "%s" but second is "%s"`, t1.Version, t2.Version)
 	}
+	if len(t2.Dotenv) > 0 {
+		return ErrIncludedTaskfilesCantHaveDotenvs
+	}
 	if t2.Output.IsSet() {
 		t1.Output = t2.Output
 	}
 	if t1.Vars == nil {
 		t1.Vars = &Vars{}
 	}
 	if t1.Env == nil {
 		t1.Env = &Vars{}
 	}
-	t1.Vars.Merge(t2.Vars)
-	t1.Env.Merge(t2.Env)
-	t1.Tasks.Merge(t2.Tasks, include)
+	t1.Vars.Merge(t2.Vars, include)
+	t1.Env.Merge(t2.Env, include)
+	t1.Tasks.Merge(t2.Tasks, include, t1.Vars)
 	return nil
 }
 
 func (tf *Taskfile) UnmarshalYAML(node *yaml.Node) error {
 	switch node.Kind {
 	case yaml.MappingNode:
 		var taskfile struct {
```

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/taskfile_test.go` & `go_task_bin-3.37.0/task/taskfile/ast/taskfile_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/tasks.go` & `go_task_bin-3.37.0/task/taskfile/ast/tasks.go`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import (
 	"fmt"
 	"strings"
 
 	"gopkg.in/yaml.v3"
 
+	"github.com/go-task/task/v3/internal/filepathext"
 	"github.com/go-task/task/v3/internal/omap"
 )
 
 // Tasks represents a group of tasks
 type Tasks struct {
 	omap.OrderedMap[string, *Task]
 }
@@ -40,48 +41,62 @@
 			})
 		}
 		return nil
 	})
 	return matchingTasks
 }
 
-func (t1 *Tasks) Merge(t2 Tasks, include *Include) {
+func (t1 *Tasks) Merge(t2 Tasks, include *Include, includedTaskfileVars *Vars) {
 	_ = t2.Range(func(k string, v *Task) error {
 		// We do a deep copy of the task struct here to ensure that no data can
 		// be changed elsewhere once the taskfile is merged.
 		task := v.DeepCopy()
 
 		// Set the task to internal if EITHER the included task or the included
 		// taskfile are marked as internal
 		task.Internal = task.Internal || (include != nil && include.Internal)
 
-		// Add namespaces to dependencies, commands and aliases
+		// Add namespaces to task dependencies
 		for _, dep := range task.Deps {
 			if dep != nil && dep.Task != "" {
 				dep.Task = taskNameWithNamespace(dep.Task, include.Namespace)
 			}
 		}
+
+		// Add namespaces to task commands
 		for _, cmd := range task.Cmds {
 			if cmd != nil && cmd.Task != "" {
 				cmd.Task = taskNameWithNamespace(cmd.Task, include.Namespace)
 			}
 		}
+
+		// Add namespaces to task aliases
 		for i, alias := range task.Aliases {
 			task.Aliases[i] = taskNameWithNamespace(alias, include.Namespace)
 		}
+
 		// Add namespace aliases
 		if include != nil {
 			for _, namespaceAlias := range include.Aliases {
 				task.Aliases = append(task.Aliases, taskNameWithNamespace(task.Task, namespaceAlias))
 				for _, alias := range v.Aliases {
 					task.Aliases = append(task.Aliases, taskNameWithNamespace(alias, namespaceAlias))
 				}
 			}
 		}
 
+		if include.AdvancedImport {
+			task.Dir = filepathext.SmartJoin(include.Dir, task.Dir)
+			if task.IncludeVars == nil {
+				task.IncludeVars = &Vars{}
+			}
+			task.IncludeVars.Merge(include.Vars, nil)
+			task.IncludedTaskfileVars = includedTaskfileVars
+		}
+
 		// Add the task to the merged taskfile
 		taskNameWithNamespace := taskNameWithNamespace(k, include.Namespace)
 		task.Task = taskNameWithNamespace
 		t1.Set(taskNameWithNamespace, task)
 
 		return nil
 	})
```

### Comparing `go_task_bin-3.36.0/task/taskfile/ast/var.go` & `go_task_bin-3.37.0/task/taskfile/ast/var.go`

 * *Files 5% similar despite different names*

```diff
@@ -41,19 +41,25 @@
 	if vs == nil {
 		return nil
 	}
 	return vs.OrderedMap.Range(f)
 }
 
 // Wrapper around OrderedMap.Merge to ensure we don't get nil pointer errors
-func (vs *Vars) Merge(other *Vars) {
+func (vs *Vars) Merge(other *Vars, include *Include) {
 	if vs == nil || other == nil {
 		return
 	}
-	vs.OrderedMap.Merge(other.OrderedMap)
+	_ = other.Range(func(key string, value Var) error {
+		if include != nil && include.AdvancedImport {
+			value.Dir = include.Dir
+		}
+		vs.Set(key, value)
+		return nil
+	})
 }
 
 // Wrapper around OrderedMap.Len to ensure we don't get nil pointer errors
 func (vs *Vars) Len() int {
 	if vs == nil {
 		return 0
 	}
@@ -79,18 +85,18 @@
 	Ref   string
 	Json  string
 	Yaml  string
 	Dir   string
 }
 
 func (v *Var) UnmarshalYAML(node *yaml.Node) error {
-	if experiments.AnyVariables.Enabled {
+	if experiments.MapVariables.Enabled {
 
 		// This implementation is not backwards-compatible and replaces the 'sh' key with map variables
-		if experiments.AnyVariables.Value == "1" {
+		if experiments.MapVariables.Value == "1" {
 			var value any
 			if err := node.Decode(&value); err != nil {
 				return err
 			}
 			// If the value is a string and it starts with $, then it's a shell command
 			if str, ok := value.(string); ok {
 				if str, ok = strings.CutPrefix(str, "$"); ok {
@@ -99,15 +105,15 @@
 				}
 			}
 			v.Value = value
 			return nil
 		}
 
 		// This implementation IS backwards-compatible and keeps the 'sh' key and allows map variables to be added under the `map` key
-		if experiments.AnyVariables.Value == "2" {
+		if experiments.MapVariables.Value == "2" {
 			switch node.Kind {
 			case yaml.MappingNode:
 				key := node.Content[0].Value
 				switch key {
 				case "sh", "ref", "map", "json", "yaml":
 					var m struct {
 						Sh   string
@@ -137,28 +143,29 @@
 				return nil
 			}
 		}
 	}
 
 	switch node.Kind {
 
-	case yaml.ScalarNode:
-		var str string
-		if err := node.Decode(&str); err != nil {
-			return err
-		}
-		v.Value = str
-		return nil
-
 	case yaml.MappingNode:
+		if len(node.Content) > 2 || node.Content[0].Value != "sh" {
+			return fmt.Errorf(`task: line %d: maps cannot be assigned to variables`, node.Line)
+		}
 		var sh struct {
 			Sh string
 		}
 		if err := node.Decode(&sh); err != nil {
 			return err
 		}
 		v.Sh = sh.Sh
 		return nil
-	}
 
-	return fmt.Errorf("yaml: line %d: cannot unmarshal %s into variable", node.Line, node.ShortTag())
+	default:
+		var value any
+		if err := node.Decode(&value); err != nil {
+			return err
+		}
+		v.Value = value
+		return nil
+	}
 }
```

### Comparing `go_task_bin-3.36.0/task/taskfile/cache.go` & `go_task_bin-3.37.0/task/taskfile/cache.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/dotenv.go` & `go_task_bin-3.37.0/task/taskfile/dotenv.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/node.go` & `go_task_bin-3.37.0/task/taskfile/node.go`

 * *Files 24% similar despite different names*

```diff
@@ -13,31 +13,29 @@
 )
 
 type Node interface {
 	Read(ctx context.Context) ([]byte, error)
 	Parent() Node
 	Location() string
 	Dir() string
-	Optional() bool
 	Remote() bool
 	ResolveEntrypoint(entrypoint string) (string, error)
 	ResolveDir(dir string) (string, error)
 }
 
 func NewRootNode(
 	l *logger.Logger,
 	entrypoint string,
 	dir string,
 	insecure bool,
 	timeout time.Duration,
 ) (Node, error) {
 	dir = getDefaultDir(entrypoint, dir)
-	// Check if there is something to read on STDIN
-	stat, _ := os.Stdin.Stat()
-	if (stat.Mode()&os.ModeCharDevice) == 0 && stat.Size() > 0 {
+	// If the entrypoint is "-", we read from stdin
+	if entrypoint == "-" {
 		return NewStdinNode(dir)
 	}
 	return NewNode(l, entrypoint, dir, insecure, timeout)
 }
 
 func NewNode(
 	l *logger.Logger,
```

### Comparing `go_task_bin-3.36.0/task/taskfile/node_base.go` & `go_task_bin-3.37.0/task/taskfile/node_base.go`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 package taskfile
 
 type (
 	NodeOption func(*BaseNode)
-	// BaseNode is a generic node that implements the Parent() and Optional()
-	// methods of the NodeReader interface. It does not implement the Read() method
-	// and it designed to be embedded in other node types so that this boilerplate
-	// code does not need to be repeated.
+	// BaseNode is a generic node that implements the Parent() methods of the
+	// NodeReader interface. It does not implement the Read() method and it
+	// designed to be embedded in other node types so that this boilerplate code
+	// does not need to be repeated.
 	BaseNode struct {
-		parent   Node
-		optional bool
-		dir      string
+		parent Node
+		dir    string
 	}
 )
 
 func NewBaseNode(dir string, opts ...NodeOption) *BaseNode {
 	node := &BaseNode{
-		parent:   nil,
-		optional: false,
-		dir:      dir,
+		parent: nil,
+		dir:    dir,
 	}
 
 	// Apply options
 	for _, opt := range opts {
 		opt(node)
 	}
 
@@ -34,20 +32,10 @@
 	}
 }
 
 func (node *BaseNode) Parent() Node {
 	return node.parent
 }
 
-func WithOptional(optional bool) NodeOption {
-	return func(node *BaseNode) {
-		node.optional = optional
-	}
-}
-
-func (node *BaseNode) Optional() bool {
-	return node.optional
-}
-
 func (node *BaseNode) Dir() string {
 	return node.dir
 }
```

### Comparing `go_task_bin-3.36.0/task/taskfile/node_file.go` & `go_task_bin-3.37.0/task/taskfile/node_file.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/node_http.go` & `go_task_bin-3.37.0/task/taskfile/node_http.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/node_stdin.go` & `go_task_bin-3.37.0/task/taskfile/node_stdin.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/taskfile/reader.go` & `go_task_bin-3.37.0/task/taskfile/reader.go`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 
 import (
 	"context"
 	"fmt"
 	"os"
 	"time"
 
+	"github.com/dominikbraun/graph"
+	"golang.org/x/sync/errgroup"
 	"gopkg.in/yaml.v3"
 
 	"github.com/go-task/task/v3/errors"
+	"github.com/go-task/task/v3/internal/compiler"
 	"github.com/go-task/task/v3/internal/filepathext"
 	"github.com/go-task/task/v3/internal/logger"
 	"github.com/go-task/task/v3/internal/templater"
 	"github.com/go-task/task/v3/taskfile/ast"
 )
 
 const (
@@ -20,41 +23,91 @@
 --- Make sure you trust the source of this Taskfile before continuing ---
 Continue?`
 	taskfileChangedPrompt = `The Taskfile at %q has changed since you last used it!
 --- Make sure you trust the source of this Taskfile before continuing ---
 Continue?`
 )
 
-// Read reads a Read for a given directory
-// Uses current dir when dir is left empty. Uses Read.yml
-// or Read.yaml when entrypoint is left empty
-func Read(
+// A Reader will recursively read Taskfiles from a given source using a directed
+// acyclic graph (DAG).
+type Reader struct {
+	graph    *ast.TaskfileGraph
+	node     Node
+	insecure bool
+	download bool
+	offline  bool
+	timeout  time.Duration
+	tempDir  string
+	logger   *logger.Logger
+}
+
+func NewReader(
 	node Node,
 	insecure bool,
 	download bool,
 	offline bool,
 	timeout time.Duration,
 	tempDir string,
-	l *logger.Logger,
-) (*ast.Taskfile, error) {
-	var _taskfile func(Node) (*ast.Taskfile, error)
-	_taskfile = func(node Node) (*ast.Taskfile, error) {
-		tf, err := readTaskfile(node, download, offline, timeout, tempDir, l)
-		if err != nil {
-			return nil, err
-		}
+	logger *logger.Logger,
+) *Reader {
+	return &Reader{
+		graph:    ast.NewTaskfileGraph(),
+		node:     node,
+		insecure: insecure,
+		download: download,
+		offline:  offline,
+		timeout:  timeout,
+		tempDir:  tempDir,
+		logger:   logger,
+	}
+}
 
-		// Check that the Taskfile is set and has a schema version
-		if tf == nil || tf.Version == nil {
-			return nil, &errors.TaskfileVersionCheckError{URI: node.Location()}
-		}
+func (r *Reader) Read() (*ast.TaskfileGraph, error) {
+	// Recursively loop through each Taskfile, adding vertices/edges to the graph
+	if err := r.include(r.node); err != nil {
+		return nil, err
+	}
+
+	return r.graph, nil
+}
+
+func (r *Reader) include(node Node) error {
+	// Create a new vertex for the Taskfile
+	vertex := &ast.TaskfileVertex{
+		URI:      node.Location(),
+		Taskfile: nil,
+	}
+
+	// Add the included Taskfile to the DAG
+	// If the vertex already exists, we return early since its Taskfile has
+	// already been read and its children explored
+	if err := r.graph.AddVertex(vertex); err == graph.ErrVertexAlreadyExists {
+		return nil
+	} else if err != nil {
+		return err
+	}
 
-		err = tf.Includes.Range(func(namespace string, include ast.Include) error {
-			cache := &templater.Cache{Vars: tf.Vars}
-			include = ast.Include{
+	// Read and parse the Taskfile from the file and add it to the vertex
+	var err error
+	vertex.Taskfile, err = r.readNode(node)
+	if err != nil {
+		return err
+	}
+
+	// Create an error group to wait for all included Taskfiles to be read
+	var g errgroup.Group
+
+	// Loop over each included taskfile
+	_ = vertex.Taskfile.Includes.Range(func(namespace string, include *ast.Include) error {
+		vars := compiler.GetEnviron()
+		vars.Merge(vertex.Taskfile.Vars, nil)
+		// Start a goroutine to process each included Taskfile
+		g.Go(func() error {
+			cache := &templater.Cache{Vars: vars}
+			include = &ast.Include{
 				Namespace:      include.Namespace,
 				Taskfile:       templater.Replace(include.Taskfile, cache),
 				Dir:            templater.Replace(include.Dir, cache),
 				Optional:       include.Optional,
 				Internal:       include.Internal,
 				Aliases:        include.Aliases,
 				AdvancedImport: include.AdvancedImport,
@@ -65,213 +118,168 @@
 			}
 
 			entrypoint, err := node.ResolveEntrypoint(include.Taskfile)
 			if err != nil {
 				return err
 			}
 
-			dir, err := node.ResolveDir(include.Dir)
+			include.Dir, err = node.ResolveDir(include.Dir)
 			if err != nil {
 				return err
 			}
 
-			includeReaderNode, err := NewNode(l, entrypoint, dir, insecure, timeout,
+			includeNode, err := NewNode(r.logger, entrypoint, include.Dir, r.insecure, r.timeout,
 				WithParent(node),
-				WithOptional(include.Optional),
 			)
 			if err != nil {
 				if include.Optional {
 					return nil
 				}
 				return err
 			}
 
-			if err := checkCircularIncludes(includeReaderNode); err != nil {
-				return err
-			}
-
-			includedTaskfile, err := _taskfile(includeReaderNode)
-			if err != nil {
-				if include.Optional {
-					return nil
-				}
+			// Recurse into the included Taskfile
+			if err := r.include(includeNode); err != nil {
 				return err
 			}
 
-			if len(includedTaskfile.Dotenv) > 0 {
-				return ErrIncludedTaskfilesCantHaveDotenvs
-			}
-
-			if include.AdvancedImport {
-				// nolint: errcheck
-				includedTaskfile.Vars.Range(func(k string, v ast.Var) error {
-					o := v
-					o.Dir = dir
-					includedTaskfile.Vars.Set(k, o)
-					return nil
-				})
-				// nolint: errcheck
-				includedTaskfile.Env.Range(func(k string, v ast.Var) error {
-					o := v
-					o.Dir = dir
-					includedTaskfile.Env.Set(k, o)
-					return nil
-				})
-
-				for _, task := range includedTaskfile.Tasks.Values() {
-					task.Dir = filepathext.SmartJoin(dir, task.Dir)
-					if task.IncludeVars == nil {
-						task.IncludeVars = &ast.Vars{}
-					}
-					task.IncludeVars.Merge(include.Vars)
-					task.IncludedTaskfileVars = includedTaskfile.Vars
+			// Create an edge between the Taskfiles
+			r.graph.Lock()
+			defer r.graph.Unlock()
+			edge, err := r.graph.Edge(node.Location(), includeNode.Location())
+			if err == graph.ErrEdgeNotFound {
+				// If the edge doesn't exist, create it
+				err = r.graph.AddEdge(
+					node.Location(),
+					includeNode.Location(),
+					graph.EdgeData([]*ast.Include{include}),
+					graph.EdgeWeight(1),
+				)
+			} else {
+				// If the edge already exists
+				edgeData := append(edge.Properties.Data.([]*ast.Include), include)
+				err = r.graph.UpdateEdge(
+					node.Location(),
+					includeNode.Location(),
+					graph.EdgeData(edgeData),
+					graph.EdgeWeight(len(edgeData)),
+				)
+			}
+			if errors.Is(err, graph.ErrEdgeCreatesCycle) {
+				return errors.TaskfileCycleError{
+					Source:      node.Location(),
+					Destination: includeNode.Location(),
 				}
 			}
-
-			if err = tf.Merge(includedTaskfile, &include); err != nil {
-				return err
-			}
-
-			return nil
+			return err
 		})
-		if err != nil {
-			return nil, err
-		}
-
-		for _, task := range tf.Tasks.Values() {
-			// If the task is not defined, create a new one
-			if task == nil {
-				task = &ast.Task{}
-			}
-			// Set the location of the taskfile for each task
-			if task.Location.Taskfile == "" {
-				task.Location.Taskfile = tf.Location
-			}
-		}
+		return nil
+	})
 
-		return tf, nil
-	}
-	return _taskfile(node)
+	// Wait for all the go routines to finish
+	return g.Wait()
 }
 
-func readTaskfile(
-	node Node,
-	download,
-	offline bool,
-	timeout time.Duration,
-	tempDir string,
-	l *logger.Logger,
-) (*ast.Taskfile, error) {
+func (r *Reader) readNode(node Node) (*ast.Taskfile, error) {
 	var b []byte
 	var err error
 	var cache *Cache
 
 	if node.Remote() {
-		cache, err = NewCache(tempDir)
+		cache, err = NewCache(r.tempDir)
 		if err != nil {
 			return nil, err
 		}
 	}
 
 	// If the file is remote and we're in offline mode, check if we have a cached copy
-	if node.Remote() && offline {
+	if node.Remote() && r.offline {
 		if b, err = cache.read(node); errors.Is(err, os.ErrNotExist) {
 			return nil, &errors.TaskfileCacheNotFoundError{URI: node.Location()}
 		} else if err != nil {
 			return nil, err
 		}
-		l.VerboseOutf(logger.Magenta, "task: [%s] Fetched cached copy\n", node.Location())
-
+		r.logger.VerboseOutf(logger.Magenta, "task: [%s] Fetched cached copy\n", node.Location())
 	} else {
 
 		downloaded := false
-		ctx, cf := context.WithTimeout(context.Background(), timeout)
+		ctx, cf := context.WithTimeout(context.Background(), r.timeout)
 		defer cf()
 
 		// Read the file
 		b, err = node.Read(ctx)
 		// If we timed out then we likely have a network issue
 		if node.Remote() && errors.Is(ctx.Err(), context.DeadlineExceeded) {
 			// If a download was requested, then we can't use a cached copy
-			if download {
-				return nil, &errors.TaskfileNetworkTimeoutError{URI: node.Location(), Timeout: timeout}
+			if r.download {
+				return nil, &errors.TaskfileNetworkTimeoutError{URI: node.Location(), Timeout: r.timeout}
 			}
 			// Search for any cached copies
 			if b, err = cache.read(node); errors.Is(err, os.ErrNotExist) {
-				return nil, &errors.TaskfileNetworkTimeoutError{URI: node.Location(), Timeout: timeout, CheckedCache: true}
+				return nil, &errors.TaskfileNetworkTimeoutError{URI: node.Location(), Timeout: r.timeout, CheckedCache: true}
 			} else if err != nil {
 				return nil, err
 			}
-			l.VerboseOutf(logger.Magenta, "task: [%s] Network timeout. Fetched cached copy\n", node.Location())
+			r.logger.VerboseOutf(logger.Magenta, "task: [%s] Network timeout. Fetched cached copy\n", node.Location())
 		} else if err != nil {
 			return nil, err
 		} else {
 			downloaded = true
 		}
 
 		// If the node was remote, we need to check the checksum
 		if node.Remote() && downloaded {
-			l.VerboseOutf(logger.Magenta, "task: [%s] Fetched remote copy\n", node.Location())
+			r.logger.VerboseOutf(logger.Magenta, "task: [%s] Fetched remote copy\n", node.Location())
 
 			// Get the checksums
 			checksum := checksum(b)
 			cachedChecksum := cache.readChecksum(node)
 
 			var prompt string
 			if cachedChecksum == "" {
 				// If the checksum doesn't exist, prompt the user to continue
 				prompt = fmt.Sprintf(taskfileUntrustedPrompt, node.Location())
 			} else if checksum != cachedChecksum {
 				// If there is a cached hash, but it doesn't match the expected hash, prompt the user to continue
 				prompt = fmt.Sprintf(taskfileChangedPrompt, node.Location())
 			}
 			if prompt != "" {
-				if err := l.Prompt(logger.Yellow, prompt, "n", "y", "yes"); err != nil {
+				if err := r.logger.Prompt(logger.Yellow, prompt, "n", "y", "yes"); err != nil {
 					return nil, &errors.TaskfileNotTrustedError{URI: node.Location()}
 				}
 			}
 
 			// If the hash has changed (or is new)
 			if checksum != cachedChecksum {
 				// Store the checksum
 				if err := cache.writeChecksum(node, checksum); err != nil {
 					return nil, err
 				}
 				// Cache the file
-				l.VerboseOutf(logger.Magenta, "task: [%s] Caching downloaded file\n", node.Location())
+				r.logger.VerboseOutf(logger.Magenta, "task: [%s] Caching downloaded file\n", node.Location())
 				if err = cache.write(node, b); err != nil {
 					return nil, err
 				}
 			}
 		}
 	}
 
 	var t ast.Taskfile
 	if err := yaml.Unmarshal(b, &t); err != nil {
 		return nil, &errors.TaskfileInvalidError{URI: filepathext.TryAbsToRel(node.Location()), Err: err}
 	}
-	t.Location = node.Location()
-
-	return &t, nil
-}
 
-func checkCircularIncludes(node Node) error {
-	if node == nil {
-		return errors.New("task: failed to check for include cycle: node was nil")
-	}
-	if node.Parent() == nil {
-		return errors.New("task: failed to check for include cycle: node.Parent was nil")
-	}
-	curNode := node
-	location := node.Location()
-	for curNode.Parent() != nil {
-		curNode = curNode.Parent()
-		curLocation := curNode.Location()
-		if curLocation == location {
-			return fmt.Errorf("task: include cycle detected between %s <--> %s",
-				curLocation,
-				node.Parent().Location(),
-			)
+	// Set the taskfile/task's locations
+	t.Location = node.Location()
+	for _, task := range t.Tasks.Values() {
+		// If the task is not defined, create a new one
+		if task == nil {
+			task = &ast.Task{}
+		}
+		// Set the location of the taskfile for each task
+		if task.Location.Taskfile == "" {
+			task.Location.Taskfile = t.Location
 		}
 	}
-	return nil
+
+	return &t, nil
 }
```

### Comparing `go_task_bin-3.36.0/task/taskfile/taskfile.go` & `go_task_bin-3.37.0/task/taskfile/taskfile.go`

 * *Files 7% similar despite different names*

```diff
@@ -12,28 +12,24 @@
 	"github.com/go-task/task/v3/errors"
 	"github.com/go-task/task/v3/internal/filepathext"
 	"github.com/go-task/task/v3/internal/logger"
 	"github.com/go-task/task/v3/internal/sysinfo"
 )
 
 var (
-	// ErrIncludedTaskfilesCantHaveDotenvs is returned when a included Taskfile contains dotenvs
-	ErrIncludedTaskfilesCantHaveDotenvs = errors.New("task: Included Taskfiles can't have dotenv declarations. Please, move the dotenv declaration to the main Taskfile")
-
 	defaultTaskfiles = []string{
 		"Taskfile.yml",
 		"taskfile.yml",
 		"Taskfile.yaml",
 		"taskfile.yaml",
 		"Taskfile.dist.yml",
 		"taskfile.dist.yml",
 		"Taskfile.dist.yaml",
 		"taskfile.dist.yaml",
 	}
-
 	allowedContentTypes = []string{
 		"text/plain",
 		"text/yaml",
 		"text/x-yaml",
 		"application/yaml",
 		"application/x-yaml",
 	}
```

### Comparing `go_task_bin-3.36.0/task/testdata/deps/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/deps/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/dir/dynamic_var/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/dir/dynamic_var/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/for/cmds/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/for/cmds/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/for/deps/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/for/deps/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/generates/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/generates/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/includes/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/includes/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/params/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/params/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/platforms/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/platforms/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/silent/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/silent/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/summary/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/summary/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/vars/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/vars/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/vars/any/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/vars/any/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/testdata/vars/any2/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/vars/any2/Taskfile.yml`

 * *Files 11% similar despite different names*

```diff
@@ -4,26 +4,27 @@
   default:
     - task: map
     - task: nested-map
     - task: slice
     - task: ref
     - task: ref-sh
     - task: ref-dep
+    - task: ref-resolver
     - task: json
     - task: yaml
 
   map:
     vars:
       MAP:
         map: {"name":"Alice","age":30,"children":[{"name":"Bob","age":5},{"name":"Charlie","age":3},{"name":"Diane","age":1}]}
     cmds:
-      - task: print-var
+      - task: print-story
         vars:
           VAR:
-            ref: MAP
+            ref: .MAP
 
   nested-map:
     vars:
       FOO: "foo"
       nested:
         map:
           variables:
@@ -40,71 +41,87 @@
       - echo {{index .slice_variables_work 0}} {{index .slice_variables_work 1}}
 
   ref:
     vars:
       MAP:
         map: {"name":"Alice","age":30,"children":[{"name":"Bob","age":5},{"name":"Charlie","age":3},{"name":"Diane","age":1}]}
       MAP_REF:
-        ref: MAP
+        ref: .MAP
     cmds:
-      - task: print-var
+      - task: print-story
         vars:
           VAR:
-            ref: MAP_REF
+            ref: .MAP_REF
 
   ref-sh:
     vars:
       JSON_STRING:
         sh: echo '{"name":"Alice","age":30,"children":[{"name":"Bob","age":5},{"name":"Charlie","age":3},{"name":"Diane","age":1}]}'
       JSON:
         json: "{{.JSON_STRING}}"
       MAP_REF:
-        ref: JSON
+        ref: .JSON
     cmds:
-      - task: print-var
+      - task: print-story
         vars:
           VAR:
-            ref: MAP_REF
+            ref: .MAP_REF
 
   ref-dep:
     vars:
       MAP:
         map: {"name":"Alice","age":30,"children":[{"name":"Bob","age":5},{"name":"Charlie","age":3},{"name":"Diane","age":1}]}
     deps:
+      - task: print-story
+        vars:
+          VAR:
+            ref: .MAP
+
+  ref-resolver:
+    vars:
+      MAP:
+        map: {"name":"Alice","age":30,"children":[{"name":"Bob","age":5},{"name":"Charlie","age":3},{"name":"Diane","age":1}]}
+      MAP_REF:
+        ref: .MAP
+    cmds:
       - task: print-var
         vars:
           VAR:
-            ref: MAP
+            ref: (index .MAP_REF.children 0).name
 
   json:
     vars:
       JSON_STRING:
         sh: cat example.json
       JSON:
         json: "{{.JSON_STRING}}"
     cmds:
-      - task: print-var
+      - task: print-story
         vars:
           VAR:
-            ref: JSON
+            ref: .JSON
 
   yaml:
     vars:
       YAML_STRING:
         sh: cat example.yaml
       YAML:
         yaml: "{{.YAML_STRING}}"
     cmds:
-      - task: print-var
+      - task: print-story
         vars:
           VAR:
-            ref: YAML
+            ref: .YAML
 
   print-var:
     cmds:
+      - echo "{{.VAR}}"
+
+  print-story:
+    cmds:
       - >-
         echo "{{.VAR.name}} has {{len .VAR.children}} children called
         {{- $children := .VAR.children -}}
         {{- range $i, $child := $children -}}
           {{- if lt $i (sub (len $children) 1)}} {{$child.name -}},
           {{- else}} and {{$child.name -}}
           {{- end -}}
```

### Comparing `go_task_bin-3.36.0/task/testdata/wildcards/Taskfile.yml` & `go_task_bin-3.37.0/task/testdata/wildcards/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/variables.go` & `go_task_bin-3.37.0/task/variables.go`

 * *Files 3% similar despite different names*

```diff
@@ -100,17 +100,17 @@
 					dotenvEnvs.Set(key, ast.Var{Value: value})
 				}
 			}
 		}
 	}
 
 	new.Env = &ast.Vars{}
-	new.Env.Merge(templater.ReplaceVars(e.Taskfile.Env, cache))
-	new.Env.Merge(templater.ReplaceVars(dotenvEnvs, cache))
-	new.Env.Merge(templater.ReplaceVars(origTask.Env, cache))
+	new.Env.Merge(templater.ReplaceVars(e.Taskfile.Env, cache), nil)
+	new.Env.Merge(templater.ReplaceVars(dotenvEnvs, cache), nil)
+	new.Env.Merge(templater.ReplaceVars(origTask.Env, cache), nil)
 	if evaluateShVars {
 		err = new.Env.Range(func(k string, v ast.Var) error {
 			// If the variable is not dynamic, we can set it and return
 			if v.Value != nil || v.Sh == "" {
 				new.Env.Set(k, ast.Var{Value: v.Value})
 				return nil
 			}
@@ -160,25 +160,14 @@
 				}
 				continue
 			}
 			newCmd := cmd.DeepCopy()
 			newCmd.Cmd = templater.Replace(cmd.Cmd, cache)
 			newCmd.Task = templater.Replace(cmd.Task, cache)
 			newCmd.Vars = templater.ReplaceVars(cmd.Vars, cache)
-			// Loop over the command's variables and resolve any references to other variables
-			err := cmd.Vars.Range(func(k string, v ast.Var) error {
-				if v.Ref != "" {
-					refVal := vars.Get(v.Ref)
-					newCmd.Vars.Set(k, refVal)
-				}
-				return nil
-			})
-			if err != nil {
-				return nil, err
-			}
 			new.Cmds = append(new.Cmds, newCmd)
 		}
 	}
 	if len(origTask.Deps) > 0 {
 		new.Deps = make([]*ast.Dep, 0, len(origTask.Deps))
 		for _, dep := range origTask.Deps {
 			if dep == nil {
@@ -210,25 +199,14 @@
 					new.Deps = append(new.Deps, newDep)
 				}
 				continue
 			}
 			newDep := dep.DeepCopy()
 			newDep.Task = templater.Replace(dep.Task, cache)
 			newDep.Vars = templater.ReplaceVars(dep.Vars, cache)
-			// Loop over the dep's variables and resolve any references to other variables
-			err := dep.Vars.Range(func(k string, v ast.Var) error {
-				if v.Ref != "" {
-					refVal := vars.Get(v.Ref)
-					newDep.Vars.Set(k, refVal)
-				}
-				return nil
-			})
-			if err != nil {
-				return nil, err
-			}
 			new.Deps = append(new.Deps, newDep)
 		}
 	}
 
 	if len(origTask.Preconditions) > 0 {
 		new.Preconditions = make([]*ast.Precondition, 0, len(origTask.Preconditions))
 		for _, precondition := range origTask.Preconditions {
```

### Comparing `go_task_bin-3.36.0/task/watch.go` & `go_task_bin-3.37.0/task/watch.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/watch_test.go` & `go_task_bin-3.37.0/task/watch_test.go`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/Taskfile.yml` & `go_task_bin-3.37.0/task/website/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/blog/2023-09-02-introducing-experiments.md` & `go_task_bin-3.37.0/task/website/blog/2023-09-02-introducing-experiments.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Lately, Task has been growing extremely quickly and I've found myself thinking a
 lot about the future of the project and how we continue to evolve and grow. I'm
 not much of a writer, but I think one of the things we could do better is to
 communicate these kinds of thoughts to the community. So, with that in mind,
 this is the first (hopefully of many) blog posts talking about Task and what
 we're up to.
 
-<!--truncate-->
+{/* truncate */}
 
 ## :calendar: So, what have we been up to?
 
 Over the past 12 months or so, [@andreynering] (Author and maintainer of the
 project) and I ([@pd93]) have been working in our spare time to maintain and
 improve v3 of Task and we've made some amazing progress. Here are just some of
 the things we've released in that time:
@@ -118,15 +118,15 @@
 you to comment on or open [issues][issues] and [discussions][discussions] on
 GitHub. Alternatively, you can join us on [Discord][discord].
 
 I plan to write more of these blog posts in the future on a variety of
 Task-related topics, so make sure to check in occasionally and see what we're up
 to!
 
-<!-- prettier-ignore-start -->
+{/* prettier-ignore-start */}
 [vscode-task]: https://github.com/go-task/vscode-task
 [crowdin]: https://crowdin.com
 [contributors]: https://github.com/go-task/task/graphs/contributors
 [semver]: https://semver.org
 [breaking-change-proposal]: https://github.com/go-task/task/discussions/1191
 [@andreynering]: https://github.com/andreynering
 [@pd93]: https://github.com/pd93
@@ -135,8 +135,8 @@
 [deprecate-version-2-schema]: https://github.com/go-task/task/issues/1197
 [issues]: https://github.com/go-task/task/issues
 [discussions]: https://github.com/go-task/task/discussions
 [discord]: https://discord.gg/6TY36E39UK
 [experiments-project]: https://github.com/orgs/go-task/projects/1
 [gentle-force-experiment]: https://github.com/go-task/task/issues/1200
 [remote-taskfiles-experiment]: https://github.com/go-task/task/issues/1317
-<!-- prettier-ignore-end -->
+{/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/docs/api_reference.mdx` & `go_task_bin-3.37.0/task/website/docs/api_reference.mdx`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
 | `silent`        | `bool`                             | `false`                                               | Hides task name and command from output. The command's output will still be redirected to `STDOUT` and `STDERR`. When combined with the `--list` flag, task descriptions will be hidden.                                                                                                                 |
 | `interactive`   | `bool`                             | `false`                                               | Tells task that the command is interactive.                                                                                                                                                                                                                                                              |
 | `internal`      | `bool`                             | `false`                                               | Stops a task from being callable on the command line. It will also be omitted from the output when used with `--list`.                                                                                                                                                                                   |
 | `method`        | `string`                           | `checksum`                                            | Defines which method is used to check the task is up-to-date. `timestamp` will compare the timestamp of the sources and generates files. `checksum` will check the checksum (You probably want to ignore the .task folder in your .gitignore file). `none` skips any validation and always run the task. |
 | `prefix`        | `string`                           |                                                       | Defines a string to prefix the output of tasks running in parallel. Only used when the output mode is `prefixed`.                                                                                                                                                                                        |
 | `ignore_error`  | `bool`                             | `false`                                               | Continue execution if errors happen while executing commands.                                                                                                                                                                                                                                            |
 | `run`           | `string`                           | The one declared globally in the Taskfile or `always` | Specifies whether the task should run again or not if called more than once. Available options: `always`, `once` and `when_changed`.                                                                                                                                                                     |
-| `platforms`     | `[]string`                         | All platforms                                         | Specifies which platforms the task should be run on. [Valid GOOS and GOARCH values allowed](https://github.com/golang/go/blob/main/src/go/build/syslist.go). Task will be skipped otherwise.                                                                                                             |
+| `platforms`     | `[]string`                         | All platforms                                         | Specifies which platforms the task should be run on. [Valid GOOS and GOARCH values allowed](https://github.com/golang/go/blob/master/src/go/build/syslist.go). Task will be skipped otherwise.                                                                                                             |
 | `set`           | `[]string`                         |                                                       | Specify options for the [`set` builtin](https://www.gnu.org/software/bash/manual/html_node/The-Set-Builtin.html).                                                                                                                                                                                        |
 | `shopt`         | `[]string`                         |                                                       | Specify option for the [`shopt` builtin](https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html).                                                                                                                                                                                     |
 
 :::info
 
 These alternative syntaxes are available. They will set the given values to
 `cmds` and everything else will be set to their default values:
@@ -296,15 +296,15 @@
 | `cmd`          | `string`                           |               | The shell command to be executed.                                                                                                                                                                  |
 | `task`         | `string`                           |               | Set this to trigger execution of another task instead of running a command. This cannot be set together with `cmd`.                                                                                |
 | `for`          | [`For`](#for)                      |               | Runs the command once for each given value.                                                                                                                                                        |
 | `silent`       | `bool`                             | `false`       | Skips some output for this command. Note that STDOUT and STDERR of the commands will still be redirected.                                                                                          |
 | `vars`         | [`map[string]Variable`](#variable) |               | Optional additional variables to be passed to the referenced task. Only relevant when setting `task` instead of `cmd`.                                                                             |
 | `ignore_error` | `bool`                             | `false`       | Continue execution if errors happen while executing the command.                                                                                                                                   |
 | `defer`        | `string`                           |               | Alternative to `cmd`, but schedules the command to be executed at the end of this task instead of immediately. This cannot be used together with `cmd`.                                            |
-| `platforms`    | `[]string`                         | All platforms | Specifies which platforms the command should be run on. [Valid GOOS and GOARCH values allowed](https://github.com/golang/go/blob/main/src/go/build/syslist.go). Command will be skipped otherwise. |
+| `platforms`    | `[]string`                         | All platforms | Specifies which platforms the command should be run on. [Valid GOOS and GOARCH values allowed](https://github.com/golang/go/blob/master/src/go/build/syslist.go). Command will be skipped otherwise. |
 | `set`          | `[]string`                         |               | Specify options for the [`set` builtin](https://www.gnu.org/software/bash/manual/html_node/The-Set-Builtin.html).                                                                                  |
 | `shopt`        | `[]string`                         |               | Specify option for the [`shopt` builtin](https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html).                                                                               |
 
 :::info
 
 If given as a a string, the value will be assigned to `cmd`:
```

### Comparing `go_task_bin-3.36.0/task/website/docs/changelog.mdx` & `go_task_bin-3.37.0/task/website/docs/changelog.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 ---
 slug: /changelog/
 sidebar_position: 14
 ---
 
 # Changelog
 
+## v3.37.0 - 2024-05-08
+
+- Released the
+  [Any Variables experiment](https://taskfile.dev/blog/any-variables), but
+  [_without support for maps_](https://github.com/go-task/task/issues/1415#issuecomment-2044756925)
+  (#1415, #1547 by @pd93).
+- Refactored how Task reads, parses and merges Taskfiles using a DAG (#1563,
+  #1607 by @pd93).
+- Fix a bug which stopped tasks from using `stdin` as input (#1593, #1623 by
+  @pd03).
+- Fix error when a file or directory in the project contained a special char
+  like `&`, `(` or `)` (#1551, #1584 by @andreynering).
+- Added alias `q` for template function `shellQuote` (#1601, #1603 by @vergenzt)
+- Added support for `~` on ZSH completions (#1613 by @jwater7).
+- Added the ability to pass variables by reference using Go template syntax when
+  the
+  [Map Variables experiment](https://taskfile.dev/experiments/map-variables/) is
+  enabled (#1612 by @pd93).
+- Added support for environment variables in the templating engine in `includes`
+  (#1610 by @vmaerten).
+
 ## v3.36.0 - 2024-04-08
 
 - Added support for
   [looping over dependencies](https://taskfile.dev/usage/#looping-over-dependencies)
   (#1299, #1541 by @pd93).
 - When using the
   "[Remote Taskfiles](https://taskfile.dev/experiments/remote-taskfiles/)"
```

### Comparing `go_task_bin-3.36.0/task/website/docs/community.mdx` & `go_task_bin-3.37.0/task/website/docs/community.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/contributing.mdx` & `go_task_bin-3.37.0/task/website/docs/contributing.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/deprecations/deprecations.mdx` & `go_task_bin-3.37.0/task/website/docs/deprecations/deprecations.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/deprecations/template.mdx` & `go_task_bin-3.37.0/task/website/docs/deprecations/template.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/deprecations/version_2_schema.mdx` & `go_task_bin-3.37.0/task/website/docs/deprecations/version_2_schema.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/experiments/any_variables.mdx` & `go_task_bin-3.37.0/task/website/docs/experiments/map_variables.mdx`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 ---
-slug: /experiments/any-variables/
+slug: /experiments/map-variables/
 ---
 
 import Tabs from '@theme/Tabs';
 import TabItem from '@theme/TabItem';
 
-# Any Variables (#1415)
+# Map Variables (#1585)
 
 :::caution
 
 All experimental features are subject to breaking changes and/or removal _at any
 time_. We strongly recommend that you do not use these features in a production
 environment. They are intended for testing and feedback only.
 
 :::
 
-Currently, Task only supports string variables. This experiment allows you to
-specify and use the following variable types:
-
-- `string`
-- `bool`
-- `int`
-- `float`
-- `array`
-- `map`
-
-This allows you to have a lot more flexibility in how you use variables in
-Task's templating engine. There are two active proposals for this experiment.
-Click on the tabs below to switch between them.
+Currently, Task supports all variable types except for maps. This experiment
+adds two different proposals for map variables. Click on the tabs below to
+switch between them.
 
 <Tabs defaultValue="1" queryString="proposal"
   values={[
     {label: 'Proposal 1', value: '1'},
     {label: 'Proposal 2', value: '2'}
   ]}>
 
@@ -44,21 +34,19 @@
 - Dynamically defined variables (using the `sh` keyword)
 
 :::
 
 :::info
 
 To enable this experiment, set the environment variable:
-`TASK_X_ANY_VARIABLES=1`. Check out [our guide to enabling experiments
+`TASK_X_MAP_VARIABLES=1`. Check out [our guide to enabling experiments
 ][enabling-experiments] for more information.
 
 :::
 
-## Maps
-
 This proposal removes support for the `sh` keyword in favour of a new syntax for
 dynamically defined variables, This allows you to define a map directly as you
 would for any other type:
 
 ```yaml
 version: 3
 
@@ -107,27 +95,24 @@
 ```
 
 If your current Taskfile contains a string variable that begins with a `$`, you
 will now need to escape the `$` with a backslash (`\`) to stop Task from
 executing it as a command.
 
 </TabItem>
-
 <TabItem value="2">
 
 :::info
 
 To enable this experiment, set the environment variable:
-`TASK_X_ANY_VARIABLES=2`. Check out [our guide to enabling experiments
+`TASK_X_MAP_VARIABLES=2`. Check out [our guide to enabling experiments
 ][enabling-experiments] for more information.
 
 :::
 
-## Maps
-
 This proposal maintains backwards-compatibility and the `sh` subkey and adds
 another new `map` subkey for defining map variables:
 
 ```yaml
 version: 3
 
 tasks:
@@ -146,49 +131,70 @@
 
 In addition to the new `map` keyword, this proposal also adds support for the
 `json` and `yaml` keywords for parsing JSON and YAML strings into real
 objects/arrays. This is similar to the `fromJSON` template function, but means
 that you only have to parse the JSON/YAML once when you declare the variable,
 instead of every time you want to access a value.
 
-Before:
+<Tabs defaultValue="2"
+  values={[
+    {label: 'Before', value: '1'},
+    {label: 'After', value: '2'}
+  ]}>
+
+<TabItem value="1">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
       FOO: '{"a": 1, "b": 2, "c": 3}' # <-- JSON string
     cmds:
       - 'echo {{(fromJSON .FOO).a}}' # <-- Parse JSON string every time you want to access a value
       - 'echo {{(fromJSON .FOO).b}}'
 ```
 
-After:
+</TabItem>
+<TabItem value="2">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
       FOO:
         json: '{"a": 1, "b": 2, "c": 3}' # <-- JSON string parsed once
     cmds:
       - 'echo {{.FOO.a}}' # <-- Access values directly
       - 'echo {{.FOO.b}}'
 ```
 
+</TabItem></Tabs>
+
 ## Variables by reference
 
 Lastly, this proposal adds support for defining and passing variables by
 reference. This is really important now that variables can be types other than a
-string. Previously, to send a variable from one task to another, you would have
-to use the templating system to pass it:
+string.
+
+Previously, to send a variable from one task to another, you would have to use
+the templating system. Unfortunately, the templater _always_ outputs a string
+and operations on the passed variable may not have behaved as expected. With
+this proposal, you can now pass variables by reference using the `ref` subkey:
+
+<Tabs defaultValue="2"
+  values={[
+    {label: 'Before', value: '1'},
+    {label: 'After', value: '2'}
+  ]}>
+
+<TabItem value="1">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
@@ -198,149 +204,132 @@
         vars:
           FOO: '{{.FOO}}' # <-- FOO gets converted to a string when passed to bar
   bar:
     cmds:
       - 'echo {{index .FOO 0}}' # <-- FOO is a string so the task outputs '91' which is the ASCII code for '[' instead of the expected 'A'
 ```
 
-Unfortunately, this results in the value always being passed as a string as this
-is the output type of the templater and operations on the passed variable may
-not behave as expected. With this proposal, you can now pass variables by
-reference using the `ref` subkey:
+</TabItem>
+<TabItem value="2">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
       FOO: [A, B, C] # <-- FOO is defined as an array
     cmds:
       - task: bar
         vars:
           FOO:
-            ref: FOO # <-- FOO gets passed by reference to bar and maintains its type
+            ref: .FOO # <-- FOO gets passed by reference to bar and maintains its type
   bar:
     cmds:
       - 'echo {{index .FOO 0}}' # <-- FOO is still a map so the task outputs 'A' as expected
 ```
 
+</TabItem></Tabs>
+
 This means that the type of the variable is maintained when it is passed to
 another Task. This also works the same way when calling `deps` and when defining
 a variable and can be used in any combination:
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
       FOO: [A, B, C] # <-- FOO is defined as an array
       BAR:
-        ref: FOO # <-- BAR is defined as a reference to FOO
+        ref: .FOO # <-- BAR is defined as a reference to FOO
     deps:
       - task: bar
         vars:
           BAR:
-            ref: BAR # <-- BAR gets passed by reference to bar and maintains its type
+            ref: .BAR # <-- BAR gets passed by reference to bar and maintains its type
   bar:
     cmds:
       - 'echo {{index .BAR 0}}' # <-- BAR still refers to FOO so the task outputs 'A'
 ```
 
-</TabItem></Tabs>
-
----
-
-## Common to both proposals
-
-Both proposals add support for all other variable types by directly defining
-them in the Taskfile. For example:
-
-### Evaluating booleans
+All references use the same templating syntax as regular templates, so in
+addition to simply calling `.FOO`, you can also pass subkeys (`.FOO.BAR`) or
+indexes (`index .FOO 0`) and use functions (`len .FOO`):
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
-      BOOL: false
+      FOO: [A, B, C] # <-- FOO is defined as an array
     cmds:
-      - '{{if .BOOL}}echo foo{{end}}'
-```
-
-### Arithmetic
-
-```yaml
-version: 3
-
-tasks:
-  foo:
-    vars:
-      INT: 10
-      FLOAT: 3.14159
+      - task: bar
+        vars:
+          FOO:
+            ref: index .FOO 0 # <-- The element at index 0 is passed by reference to bar
+  bar:
     cmds:
-      - 'echo {{add .INT .FLOAT}}'
+      - 'echo {{.MYVAR}}' # <-- FOO is just the letter 'A'
 ```
 
-### Ranging
-
-```yaml
-version: 3
+</TabItem></Tabs>
 
-tasks:
-  foo:
-    vars:
-      ARRAY: [1, 2, 3]
-    cmds:
-      - 'echo {{range .ARRAY}}{{.}}{{end}}'
-```
+## Looping over maps
 
-There are many more templating functions which can be used with the new types of
-variables. For a full list, see the [slim-sprig][slim-sprig] documentation.
+This experiment also adds support for looping over maps using the `for` keyword,
+just like arrays. In addition to the `{{.ITEM}}` variable being populated when
+looping over a map, we also make an additional `{{.KEY}}` variable available
+that holds the string value of the map key.
 
-## Looping over variables
+<Tabs defaultValue="1" queryString="proposal"
+  values={[
+    {label: 'Proposal 1', value: '1'},
+    {label: 'Proposal 2', value: '2'}
+  ]}>
 
-Previously, you would have to use a delimiter separated string to loop over an
-arbitrary list of items in a variable and split them by using the `split` subkey
-to specify the delimiter:
+<TabItem value="1">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
-      LIST: 'foo,bar,baz'
+      MAP: {a: 1, b: 2, c: 3}
     cmds:
       - for:
-          var: LIST
-          split: ','
-        cmd: echo {{.ITEM}}
+          var: MAP
+        cmd: 'echo "{{.KEY}}: {{.ITEM}}"'
 ```
 
-Both of these proposals add support for looping over "collection-type" variables
-using the `for` keyword, so now you are able to loop over a map/array variable
-directly:
+</TabItem>
+<TabItem value="2">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
-      LIST: [foo, bar, baz]
+      map:
+        MAP: {a: 1, b: 2, c: 3}
     cmds:
       - for:
-          var: LIST
-        cmd: echo {{.ITEM}}
+          var: MAP
+        cmd: 'echo "{{.KEY}}: {{.ITEM}}"'
 ```
 
-When looping over a map we also make an additional `{{.KEY}}` variable availabe
-that holds the string value of the map key. Remember that maps are unordered, so
+:::note
+
+Remember that maps are unordered, so
 the order in which the items are looped over is random.
 
+:::
+
+</TabItem></Tabs>
+
 {/* prettier-ignore-start */}
-[enabling-experiments]: /experiments/#enabling-experiments
-[slim-sprig]: https://go-task.github.io/slim-sprig/
+[enabling-experiments]: ./experiments.mdx#enabling-experiments
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/docs/experiments/experiments.mdx` & `go_task_bin-3.37.0/task/website/docs/experiments/experiments.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/experiments/gentle_force.mdx` & `go_task_bin-3.37.0/task/website/docs/experiments/gentle_force.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -41,9 +41,9 @@
 
 If you want to migrate, but continue to force all dependant tasks to run, you
 should replace all uses of the `--force` flag with `--force-all`. Alternatively,
 if you want to adopt the new behavior, you can continue to use the `--force`
 flag as you do now!
 
 {/* prettier-ignore-start */}
-[enabling-experiments]: /experiments/#enabling-experiments
+[enabling-experiments]: ./experiments.mdx#enabling-experiments
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/docs/experiments/remote_taskfiles.mdx` & `go_task_bin-3.37.0/task/website/docs/experiments/remote_taskfiles.mdx`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,28 @@
     cmds:
       - echo "Hello from the remote Taskfile!"
 ```
 
 and you run `task my-remote-namespace:hello`, it will print the text: "Hello
 from the remote Taskfile!" to your console.
 
+The Taskfile location is processed by the templating system, so you can
+reference environment variables in your URL if you need to add authentication.
+For example:
+
+```yaml
+version: '3'
+
+includes:
+  my-remote-namespace: https://{{.TOKEN}}@raw.githubusercontent.com/my-org/my-repo/main/Taskfile.yml
+```
+
+`TOKEN=my-token task my-remote-namespace:hello` will be resolved by Task to
+`https://my-token@raw.githubusercontent.com/my-org/my-repo/main/Taskfile.yml`
+
 ## Security
 
 Running commands from sources that you do not control is always a potential
 security risk. For this reason, we have added some checks when using remote
 Taskfiles:
 
 1. When running a task from a remote Taskfile for the first time, Task will
@@ -95,10 +109,10 @@
 
 By default, Task will timeout requests to download remote files after 10 seconds
 and look for a cached copy instead. This timeout can be configured by setting
 the `--timeout` flag and specifying a duration. For example, `--timeout 5s` will
 set the timeout to 5 seconds.
 
 {/* prettier-ignore-start */}
-[enabling-experiments]: /experiments/#enabling-experiments
+[enabling-experiments]: ./experiments.mdx#enabling-experiments
 [man-in-the-middle-attacks]: https://en.wikipedia.org/wiki/Man-in-the-middle_attack
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/docs/experiments/template.mdx` & `go_task_bin-3.37.0/task/website/docs/experiments/template.mdx`

 * *Files 1% similar despite different names*

```diff
@@ -34,9 +34,9 @@
 :::
 
 \{Short description of the feature\}
 
 \{Short explanation of how users should migrate to the new behavior\}
 
 {/* prettier-ignore-start */}
-[enabling-experiments]: /experiments/#enabling-experiments
+[enabling-experiments]: ./experiments.mdx#enabling-experiments
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/docs/faq.mdx` & `go_task_bin-3.37.0/task/website/docs/faq.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/installation.mdx` & `go_task_bin-3.37.0/task/website/docs/installation.mdx`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ```shell
 brew install go-task
 ```
 
 ### pkgx
 
-If you're on macOS or Linux and have [pkgx](https://pkgx.sh/) installed, getting Task is as
+If you're on macOS or Linux and have [pkgx][pkgx] installed, getting Task is as
 simple as running:
 
 ```shell
 pkgx task
 ```
 
 or, if you have pkgx integration enabled:
@@ -295,9 +295,9 @@
 [snapcraft]: https://snapcraft.io/task
 [homebrew]: https://brew.sh/
 [installscript]: https://github.com/go-task/task/blob/main/install-task.sh
 [releases]: https://github.com/go-task/task/releases
 [godownloader]: https://github.com/goreleaser/godownloader
 [choco]: https://chocolatey.org/
 [scoop]: https://scoop.sh/
-[tea]: https://tea.xyz/
+[pkgx]: https://pkgx.sh/
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/docs/integrations.mdx` & `go_task_bin-3.37.0/task/website/docs/integrations.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/intro.mdx` & `go_task_bin-3.37.0/task/website/docs/intro.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/releasing.mdx` & `go_task_bin-3.37.0/task/website/docs/releasing.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/styleguide.mdx` & `go_task_bin-3.37.0/task/website/docs/styleguide.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/taskfile_versions.mdx` & `go_task_bin-3.37.0/task/website/docs/taskfile_versions.mdx`

 * *Files 3% similar despite different names*

```diff
@@ -252,12 +252,12 @@
 
 1. Call variables
 2. Environment
 3. Task variables
 4. `Taskvars.yml` variables
 
 {/* prettier-ignore-start */}
-[deprecate-version-2-schema]: /deprecations/version-2-schema/
-[output]: /usage#output-syntax
-[ignore_errors]: /usage#ignore-errors
-[includes]: /usage#including-other-taskfiles
+[deprecate-version-2-schema]: ./deprecations/version_2_schema.mdx
+[output]: ./usage.mdx#output-syntax
+[ignore_errors]: ./usage.mdx#ignore-errors
+[includes]: ./usage.mdx#including-other-taskfiles
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/docs/translate.mdx` & `go_task_bin-3.37.0/task/website/docs/translate.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/docs/usage.mdx` & `go_task_bin-3.37.0/task/website/docs/usage.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -117,21 +117,22 @@
 ```
 
 :::
 
 ### Reading a Taskfile from stdin
 
 Taskfile also supports reading from stdin. This is useful if you are generating
-Taskfiles dynamically and don't want write them to disk. This works just like
-any other program that supports stdin. For example:
+Taskfiles dynamically and don't want write them to disk. To tell task to read
+from stdin, you must specify the `-t/--taskfile` flag with the special `-`
+value. You may then pipe into Task as you would any other program:
 
 ```shell
-task < <(cat ./Taskfile.yml)
+task -t - <(cat ./Taskfile.yml)
 # OR
-cat ./Taskfile.yml | task
+cat ./Taskfile.yml | task -t -
 ```
 
 ## Environment variables
 
 ### Task
 
 You can use `env` to set custom environment variables for a specific task:
@@ -943,16 +944,34 @@
     # Make sure these variables are set before running
     requires:
       vars: [IMAGE_NAME, IMAGE_TAG]
 ```
 
 ## Variables
 
-When doing interpolation of variables, Task will look for the below. They are
-listed below in order of importance (i.e. most important first):
+Task allows you to set variables using the `vars` keyword. The following
+variable types are supported:
+
+- `string`
+- `bool`
+- `int`
+- `float`
+- `array`
+
+:::note
+
+Maps are not supported by default, but there is an
+[experiment][map-variables] that can be enabled to add support. If
+you're interested in this functionality, we would appreciate your feedback.
+:pray:
+
+:::
+
+Variables can be set in many places in a Taskfile. When executing templates,
+Task will look for variables in the order listed below (most important first):
 
 - Variables declared in the task definition
 - Variables given while calling a task from another (See
   [Calling another task](#calling-another-task) above)
 - Variables of the [included Taskfile](#including-other-taskfiles) (when the
   task is included)
 - Variables of the [inclusion of the Taskfile](#vars-of-included-taskfiles)
@@ -1089,44 +1108,64 @@
       - for: sources
         cmd: cat {{joinPath .MY_DIR .ITEM}}
 ```
 
 ### Looping over variables
 
 To loop over the contents of a variable, you simply need to specify the variable
-you want to loop over. By default, variables will be split on any whitespace
-characters.
+you want to loop over. By default, string variables will be split on any
+whitespace characters.
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     vars:
       MY_VAR: foo.txt bar.txt
     cmds:
       - for: { var: MY_VAR }
         cmd: cat {{.ITEM}}
 ```
 
-If you need to split on a different character, you can do this by specifying the
-`split` property:
+If you need to split a string on a different character, you can do this by
+specifying the `split` property:
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     vars:
       MY_VAR: foo.txt,bar.txt
     cmds:
       - for: { var: MY_VAR, split: ',' }
         cmd: cat {{.ITEM}}
 ```
 
+You can also loop over arrays directly (and maps if you have the
+[maps experiment](/experiments/map-variables) enabled):
+
+```yaml
+version: 3
+
+tasks:
+  foo:
+    vars:
+      LIST: [foo, bar, baz]
+    cmds:
+      - for:
+          var: LIST
+        cmd: echo {{.ITEM}}
+```
+
+When looping over a map we also make an additional `{{.KEY}}` variable available
+that holds the string value of the map key. Remember that maps are unordered, so
+the order in which the items are looped over is random.
+
 All of this also works with dynamic variables!
 
 ```yaml
 version: '3'
 
 tasks:
   default:
@@ -1373,15 +1412,15 @@
   space.
 - `toSlash`: Does nothing on Unix, but on Windows converts a string from `\`
   path format to `/`.
 - `fromSlash`: Opposite of `toSlash`. Does nothing on Unix, but on Windows
   converts a string from `/` path format to `\`.
 - `exeExt`: Returns the right executable extension for the current OS (`".exe"`
   for Windows, `""` for others).
-- `shellQuote`: Quotes a string to make it safe for use in shell scripts. Task
+- `shellQuote` (aliased to `q`): Quotes a string to make it safe for use in shell scripts. Task
   uses [this Go function](https://pkg.go.dev/mvdan.cc/sh/v3@v3.4.0/syntax#Quote)
   for this. The Bash dialect is assumed.
 - `splitArgs`: Splits a string as if it were a command's arguments. Task uses
   [this Go function](https://pkg.go.dev/mvdan.cc/sh/v3@v3.4.0/shell#Fields)
 - `joinPath`: Joins any number of arguments into a path. The same as Go's
   [filepath.Join](https://pkg.go.dev/path/filepath#Join).
 - `relPath`: Converts an absolute path (second argument) into a relative path,
@@ -1952,8 +1991,9 @@
 when running from the CLI via `task my-watch-task`, but won't run in watch mode
 if called by another task, either directly or as a dependency.
 
 :::
 
 {/* prettier-ignore-start */}
 [gotemplate]: https://golang.org/pkg/text/template/
+[map-variables]: ./experiments/map_variables.mdx
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/package.json` & `go_task_bin-3.37.0/task/website/package.json`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/src/api/crowdin.js` & `go_task_bin-3.37.0/task/website/src/api/crowdin.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/src/css/carbon.css` & `go_task_bin-3.37.0/task/website/src/css/carbon.css`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/src/css/custom.css` & `go_task_bin-3.37.0/task/website/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/src/pages/donate.md` & `go_task_bin-3.37.0/task/website/src/pages/donate.md`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/src/themes/prismDark.js` & `go_task_bin-3.37.0/task/website/src/themes/prismDark.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/src/themes/prismLight.js` & `go_task_bin-3.37.0/task/website/src/themes/prismLight.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/img/appwrite.svg` & `go_task_bin-3.37.0/task/website/static/img/appwrite.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/img/favicon.ico` & `go_task_bin-3.37.0/task/website/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/img/icon-discord.svg` & `go_task_bin-3.37.0/task/website/static/img/icon-discord.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/img/icon-github.svg` & `go_task_bin-3.37.0/task/website/static/img/icon-github.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/img/icon-mastodon.svg` & `go_task_bin-3.37.0/task/website/static/img/icon-mastodon.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/img/icon-twitter.svg` & `go_task_bin-3.37.0/task/website/static/img/icon-twitter.svg`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/img/logo.png` & `go_task_bin-3.37.0/task/website/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/img/og-image.png` & `go_task_bin-3.37.0/task/website/static/img/og-image.png`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/img/pix.png` & `go_task_bin-3.37.0/task/website/static/img/pix.png`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/install.sh` & `go_task_bin-3.37.0/task/website/static/install.sh`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/js/carbon.js` & `go_task_bin-3.37.0/task/website/static/js/carbon.js`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/static/schema.json` & `go_task_bin-3.37.0/task/website/static/schema.json`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/api_reference.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/api_reference.mdx`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
 | `silent`        | `bool`                             | `false`                                               | Hides task name and command from output. The command's output will still be redirected to `STDOUT` and `STDERR`. When combined with the `--list` flag, task descriptions will be hidden.                                                                                                                 |
 | `interactive`   | `bool`                             | `false`                                               | Tells task that the command is interactive.                                                                                                                                                                                                                                                              |
 | `internal`      | `bool`                             | `false`                                               | Stops a task from being callable on the command line. It will also be omitted from the output when used with `--list`.                                                                                                                                                                                   |
 | `method`        | `string`                           | `checksum`                                            | Defines which method is used to check the task is up-to-date. `timestamp` will compare the timestamp of the sources and generates files. `checksum` will check the checksum (You probably want to ignore the .task folder in your .gitignore file). `none` skips any validation and always run the task. |
 | `prefix`        | `string`                           |                                                       | Defines a string to prefix the output of tasks running in parallel. Only used when the output mode is `prefixed`.                                                                                                                                                                                        |
 | `ignore_error`  | `bool`                             | `false`                                               | Continue execution if errors happen while executing commands.                                                                                                                                                                                                                                            |
 | `run`           | `string`                           | The one declared globally in the Taskfile or `always` | Specifies whether the task should run again or not if called more than once. Available options: `always`, `once` and `when_changed`.                                                                                                                                                                     |
-| `platforms`     | `[]string`                         | All platforms                                         | Specifies which platforms the task should be run on. [Valid GOOS and GOARCH values allowed](https://github.com/golang/go/blob/main/src/go/build/syslist.go). Task will be skipped otherwise.                                                                                                             |
+| `platforms`     | `[]string`                         | All platforms                                         | Specifies which platforms the task should be run on. [Valid GOOS and GOARCH values allowed](https://github.com/golang/go/blob/master/src/go/build/syslist.go). Task will be skipped otherwise.                                                                                                             |
 | `set`           | `[]string`                         |                                                       | Specify options for the [`set` builtin](https://www.gnu.org/software/bash/manual/html_node/The-Set-Builtin.html).                                                                                                                                                                                        |
 | `shopt`         | `[]string`                         |                                                       | Specify option for the [`shopt` builtin](https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html).                                                                                                                                                                                     |
 
 :::info
 
 These alternative syntaxes are available. They will set the given values to
 `cmds` and everything else will be set to their default values:
@@ -296,15 +296,15 @@
 | `cmd`          | `string`                           |               | The shell command to be executed.                                                                                                                                                                  |
 | `task`         | `string`                           |               | Set this to trigger execution of another task instead of running a command. This cannot be set together with `cmd`.                                                                                |
 | `for`          | [`For`](#for)                      |               | Runs the command once for each given value.                                                                                                                                                        |
 | `silent`       | `bool`                             | `false`       | Skips some output for this command. Note that STDOUT and STDERR of the commands will still be redirected.                                                                                          |
 | `vars`         | [`map[string]Variable`](#variable) |               | Optional additional variables to be passed to the referenced task. Only relevant when setting `task` instead of `cmd`.                                                                             |
 | `ignore_error` | `bool`                             | `false`       | Continue execution if errors happen while executing the command.                                                                                                                                   |
 | `defer`        | `string`                           |               | Alternative to `cmd`, but schedules the command to be executed at the end of this task instead of immediately. This cannot be used together with `cmd`.                                            |
-| `platforms`    | `[]string`                         | All platforms | Specifies which platforms the command should be run on. [Valid GOOS and GOARCH values allowed](https://github.com/golang/go/blob/main/src/go/build/syslist.go). Command will be skipped otherwise. |
+| `platforms`    | `[]string`                         | All platforms | Specifies which platforms the command should be run on. [Valid GOOS and GOARCH values allowed](https://github.com/golang/go/blob/master/src/go/build/syslist.go). Command will be skipped otherwise. |
 | `set`          | `[]string`                         |               | Specify options for the [`set` builtin](https://www.gnu.org/software/bash/manual/html_node/The-Set-Builtin.html).                                                                                  |
 | `shopt`        | `[]string`                         |               | Specify option for the [`shopt` builtin](https://www.gnu.org/software/bash/manual/html_node/The-Shopt-Builtin.html).                                                                               |
 
 :::info
 
 If given as a a string, the value will be assigned to `cmd`:
```

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/changelog.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/changelog.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 ---
 slug: /changelog/
 sidebar_position: 14
 ---
 
 # Changelog
 
+## v3.37.0 - 2024-05-08
+
+- Released the
+  [Any Variables experiment](https://taskfile.dev/blog/any-variables), but
+  [_without support for maps_](https://github.com/go-task/task/issues/1415#issuecomment-2044756925)
+  (#1415, #1547 by @pd93).
+- Refactored how Task reads, parses and merges Taskfiles using a DAG (#1563,
+  #1607 by @pd93).
+- Fix a bug which stopped tasks from using `stdin` as input (#1593, #1623 by
+  @pd03).
+- Fix error when a file or directory in the project contained a special char
+  like `&`, `(` or `)` (#1551, #1584 by @andreynering).
+- Added alias `q` for template function `shellQuote` (#1601, #1603 by @vergenzt)
+- Added support for `~` on ZSH completions (#1613 by @jwater7).
+- Added the ability to pass variables by reference using Go template syntax when
+  the
+  [Map Variables experiment](https://taskfile.dev/experiments/map-variables/) is
+  enabled (#1612 by @pd93).
+- Added support for environment variables in the templating engine in `includes`
+  (#1610 by @vmaerten).
+
 ## v3.36.0 - 2024-04-08
 
 - Added support for
   [looping over dependencies](https://taskfile.dev/usage/#looping-over-dependencies)
   (#1299, #1541 by @pd93).
 - When using the
   "[Remote Taskfiles](https://taskfile.dev/experiments/remote-taskfiles/)"
```

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/community.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/community.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/contributing.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/contributing.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/deprecations.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/deprecations.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/template.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/template.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/deprecations/version_2_schema.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/deprecations/version_2_schema.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/any_variables.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/map_variables.mdx`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,27 @@
 ---
-slug: /experiments/any-variables/
+slug: /experiments/map-variables/
 ---
 
 import Tabs from '@theme/Tabs';
 import TabItem from '@theme/TabItem';
 
-# Any Variables (#1415)
+# Map Variables (#1585)
 
 :::caution
 
 All experimental features are subject to breaking changes and/or removal _at any
 time_. We strongly recommend that you do not use these features in a production
 environment. They are intended for testing and feedback only.
 
 :::
 
-Currently, Task only supports string variables. This experiment allows you to
-specify and use the following variable types:
-
-- `string`
-- `bool`
-- `int`
-- `float`
-- `array`
-- `map`
-
-This allows you to have a lot more flexibility in how you use variables in
-Task's templating engine. There are two active proposals for this experiment.
-Click on the tabs below to switch between them.
+Currently, Task supports all variable types except for maps. This experiment
+adds two different proposals for map variables. Click on the tabs below to
+switch between them.
 
 <Tabs defaultValue="1" queryString="proposal"
   values={[
     {label: 'Proposal 1', value: '1'},
     {label: 'Proposal 2', value: '2'}
   ]}>
 
@@ -44,21 +34,19 @@
 - Dynamically defined variables (using the `sh` keyword)
 
 :::
 
 :::info
 
 To enable this experiment, set the environment variable:
-`TASK_X_ANY_VARIABLES=1`. Check out [our guide to enabling experiments
+`TASK_X_MAP_VARIABLES=1`. Check out [our guide to enabling experiments
 ][enabling-experiments] for more information.
 
 :::
 
-## Maps
-
 This proposal removes support for the `sh` keyword in favour of a new syntax for
 dynamically defined variables, This allows you to define a map directly as you
 would for any other type:
 
 ```yaml
 version: 3
 
@@ -107,27 +95,24 @@
 ```
 
 If your current Taskfile contains a string variable that begins with a `$`, you
 will now need to escape the `$` with a backslash (`\`) to stop Task from
 executing it as a command.
 
 </TabItem>
-
 <TabItem value="2">
 
 :::info
 
 To enable this experiment, set the environment variable:
-`TASK_X_ANY_VARIABLES=2`. Check out [our guide to enabling experiments
+`TASK_X_MAP_VARIABLES=2`. Check out [our guide to enabling experiments
 ][enabling-experiments] for more information.
 
 :::
 
-## Maps
-
 This proposal maintains backwards-compatibility and the `sh` subkey and adds
 another new `map` subkey for defining map variables:
 
 ```yaml
 version: 3
 
 tasks:
@@ -146,49 +131,70 @@
 
 In addition to the new `map` keyword, this proposal also adds support for the
 `json` and `yaml` keywords for parsing JSON and YAML strings into real
 objects/arrays. This is similar to the `fromJSON` template function, but means
 that you only have to parse the JSON/YAML once when you declare the variable,
 instead of every time you want to access a value.
 
-Before:
+<Tabs defaultValue="2"
+  values={[
+    {label: 'Before', value: '1'},
+    {label: 'After', value: '2'}
+  ]}>
+
+<TabItem value="1">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
       FOO: '{"a": 1, "b": 2, "c": 3}' # <-- JSON string
     cmds:
       - 'echo {{(fromJSON .FOO).a}}' # <-- Parse JSON string every time you want to access a value
       - 'echo {{(fromJSON .FOO).b}}'
 ```
 
-After:
+</TabItem>
+<TabItem value="2">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
       FOO:
         json: '{"a": 1, "b": 2, "c": 3}' # <-- JSON string parsed once
     cmds:
       - 'echo {{.FOO.a}}' # <-- Access values directly
       - 'echo {{.FOO.b}}'
 ```
 
+</TabItem></Tabs>
+
 ## Variables by reference
 
 Lastly, this proposal adds support for defining and passing variables by
 reference. This is really important now that variables can be types other than a
-string. Previously, to send a variable from one task to another, you would have
-to use the templating system to pass it:
+string.
+
+Previously, to send a variable from one task to another, you would have to use
+the templating system. Unfortunately, the templater _always_ outputs a string
+and operations on the passed variable may not have behaved as expected. With
+this proposal, you can now pass variables by reference using the `ref` subkey:
+
+<Tabs defaultValue="2"
+  values={[
+    {label: 'Before', value: '1'},
+    {label: 'After', value: '2'}
+  ]}>
+
+<TabItem value="1">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
@@ -198,149 +204,132 @@
         vars:
           FOO: '{{.FOO}}' # <-- FOO gets converted to a string when passed to bar
   bar:
     cmds:
       - 'echo {{index .FOO 0}}' # <-- FOO is a string so the task outputs '91' which is the ASCII code for '[' instead of the expected 'A'
 ```
 
-Unfortunately, this results in the value always being passed as a string as this
-is the output type of the templater and operations on the passed variable may
-not behave as expected. With this proposal, you can now pass variables by
-reference using the `ref` subkey:
+</TabItem>
+<TabItem value="2">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
       FOO: [A, B, C] # <-- FOO is defined as an array
     cmds:
       - task: bar
         vars:
           FOO:
-            ref: FOO # <-- FOO gets passed by reference to bar and maintains its type
+            ref: .FOO # <-- FOO gets passed by reference to bar and maintains its type
   bar:
     cmds:
       - 'echo {{index .FOO 0}}' # <-- FOO is still a map so the task outputs 'A' as expected
 ```
 
+</TabItem></Tabs>
+
 This means that the type of the variable is maintained when it is passed to
 another Task. This also works the same way when calling `deps` and when defining
 a variable and can be used in any combination:
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
       FOO: [A, B, C] # <-- FOO is defined as an array
       BAR:
-        ref: FOO # <-- BAR is defined as a reference to FOO
+        ref: .FOO # <-- BAR is defined as a reference to FOO
     deps:
       - task: bar
         vars:
           BAR:
-            ref: BAR # <-- BAR gets passed by reference to bar and maintains its type
+            ref: .BAR # <-- BAR gets passed by reference to bar and maintains its type
   bar:
     cmds:
       - 'echo {{index .BAR 0}}' # <-- BAR still refers to FOO so the task outputs 'A'
 ```
 
-</TabItem></Tabs>
-
----
-
-## Common to both proposals
-
-Both proposals add support for all other variable types by directly defining
-them in the Taskfile. For example:
-
-### Evaluating booleans
+All references use the same templating syntax as regular templates, so in
+addition to simply calling `.FOO`, you can also pass subkeys (`.FOO.BAR`) or
+indexes (`index .FOO 0`) and use functions (`len .FOO`):
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
-      BOOL: false
+      FOO: [A, B, C] # <-- FOO is defined as an array
     cmds:
-      - '{{if .BOOL}}echo foo{{end}}'
-```
-
-### Arithmetic
-
-```yaml
-version: 3
-
-tasks:
-  foo:
-    vars:
-      INT: 10
-      FLOAT: 3.14159
+      - task: bar
+        vars:
+          FOO:
+            ref: index .FOO 0 # <-- The element at index 0 is passed by reference to bar
+  bar:
     cmds:
-      - 'echo {{add .INT .FLOAT}}'
+      - 'echo {{.MYVAR}}' # <-- FOO is just the letter 'A'
 ```
 
-### Ranging
-
-```yaml
-version: 3
+</TabItem></Tabs>
 
-tasks:
-  foo:
-    vars:
-      ARRAY: [1, 2, 3]
-    cmds:
-      - 'echo {{range .ARRAY}}{{.}}{{end}}'
-```
+## Looping over maps
 
-There are many more templating functions which can be used with the new types of
-variables. For a full list, see the [slim-sprig][slim-sprig] documentation.
+This experiment also adds support for looping over maps using the `for` keyword,
+just like arrays. In addition to the `{{.ITEM}}` variable being populated when
+looping over a map, we also make an additional `{{.KEY}}` variable available
+that holds the string value of the map key.
 
-## Looping over variables
+<Tabs defaultValue="1" queryString="proposal"
+  values={[
+    {label: 'Proposal 1', value: '1'},
+    {label: 'Proposal 2', value: '2'}
+  ]}>
 
-Previously, you would have to use a delimiter separated string to loop over an
-arbitrary list of items in a variable and split them by using the `split` subkey
-to specify the delimiter:
+<TabItem value="1">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
-      LIST: 'foo,bar,baz'
+      MAP: {a: 1, b: 2, c: 3}
     cmds:
       - for:
-          var: LIST
-          split: ','
-        cmd: echo {{.ITEM}}
+          var: MAP
+        cmd: 'echo "{{.KEY}}: {{.ITEM}}"'
 ```
 
-Both of these proposals add support for looping over "collection-type" variables
-using the `for` keyword, so now you are able to loop over a map/array variable
-directly:
+</TabItem>
+<TabItem value="2">
 
 ```yaml
 version: 3
 
 tasks:
   foo:
     vars:
-      LIST: [foo, bar, baz]
+      map:
+        MAP: {a: 1, b: 2, c: 3}
     cmds:
       - for:
-          var: LIST
-        cmd: echo {{.ITEM}}
+          var: MAP
+        cmd: 'echo "{{.KEY}}: {{.ITEM}}"'
 ```
 
-When looping over a map we also make an additional `{{.KEY}}` variable availabe
-that holds the string value of the map key. Remember that maps are unordered, so
+:::note
+
+Remember that maps are unordered, so
 the order in which the items are looped over is random.
 
+:::
+
+</TabItem></Tabs>
+
 {/* prettier-ignore-start */}
-[enabling-experiments]: /experiments/#enabling-experiments
-[slim-sprig]: https://go-task.github.io/slim-sprig/
+[enabling-experiments]: ./experiments.mdx#enabling-experiments
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/experiments.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/experiments.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/gentle_force.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/gentle_force.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -41,9 +41,9 @@
 
 If you want to migrate, but continue to force all dependant tasks to run, you
 should replace all uses of the `--force` flag with `--force-all`. Alternatively,
 if you want to adopt the new behavior, you can continue to use the `--force`
 flag as you do now!
 
 {/* prettier-ignore-start */}
-[enabling-experiments]: /experiments/#enabling-experiments
+[enabling-experiments]: ./experiments.mdx#enabling-experiments
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/remote_taskfiles.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/remote_taskfiles.mdx`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,28 @@
     cmds:
       - echo "Hello from the remote Taskfile!"
 ```
 
 and you run `task my-remote-namespace:hello`, it will print the text: "Hello
 from the remote Taskfile!" to your console.
 
+The Taskfile location is processed by the templating system, so you can
+reference environment variables in your URL if you need to add authentication.
+For example:
+
+```yaml
+version: '3'
+
+includes:
+  my-remote-namespace: https://{{.TOKEN}}@raw.githubusercontent.com/my-org/my-repo/main/Taskfile.yml
+```
+
+`TOKEN=my-token task my-remote-namespace:hello` will be resolved by Task to
+`https://my-token@raw.githubusercontent.com/my-org/my-repo/main/Taskfile.yml`
+
 ## Security
 
 Running commands from sources that you do not control is always a potential
 security risk. For this reason, we have added some checks when using remote
 Taskfiles:
 
 1. When running a task from a remote Taskfile for the first time, Task will
@@ -95,10 +109,10 @@
 
 By default, Task will timeout requests to download remote files after 10 seconds
 and look for a cached copy instead. This timeout can be configured by setting
 the `--timeout` flag and specifying a duration. For example, `--timeout 5s` will
 set the timeout to 5 seconds.
 
 {/* prettier-ignore-start */}
-[enabling-experiments]: /experiments/#enabling-experiments
+[enabling-experiments]: ./experiments.mdx#enabling-experiments
 [man-in-the-middle-attacks]: https://en.wikipedia.org/wiki/Man-in-the-middle_attack
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/experiments/template.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/experiments/template.mdx`

 * *Files 1% similar despite different names*

```diff
@@ -34,9 +34,9 @@
 :::
 
 \{Short description of the feature\}
 
 \{Short explanation of how users should migrate to the new behavior\}
 
 {/* prettier-ignore-start */}
-[enabling-experiments]: /experiments/#enabling-experiments
+[enabling-experiments]: ./experiments.mdx#enabling-experiments
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/faq.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/faq.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/installation.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/installation.mdx`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ```shell
 brew install go-task
 ```
 
 ### pkgx
 
-If you're on macOS or Linux and have [pkgx](https://pkgx.sh/) installed, getting Task is as
+If you're on macOS or Linux and have [pkgx][pkgx] installed, getting Task is as
 simple as running:
 
 ```shell
 pkgx task
 ```
 
 or, if you have pkgx integration enabled:
@@ -295,9 +295,9 @@
 [snapcraft]: https://snapcraft.io/task
 [homebrew]: https://brew.sh/
 [installscript]: https://github.com/go-task/task/blob/main/install-task.sh
 [releases]: https://github.com/go-task/task/releases
 [godownloader]: https://github.com/goreleaser/godownloader
 [choco]: https://chocolatey.org/
 [scoop]: https://scoop.sh/
-[tea]: https://tea.xyz/
+[pkgx]: https://pkgx.sh/
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/integrations.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/integrations.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/intro.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/intro.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/releasing.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/releasing.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/styleguide.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/styleguide.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/taskfile_versions.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/taskfile_versions.mdx`

 * *Files 3% similar despite different names*

```diff
@@ -252,12 +252,12 @@
 
 1. Call variables
 2. Environment
 3. Task variables
 4. `Taskvars.yml` variables
 
 {/* prettier-ignore-start */}
-[deprecate-version-2-schema]: /deprecations/version-2-schema/
-[output]: /usage#output-syntax
-[ignore_errors]: /usage#ignore-errors
-[includes]: /usage#including-other-taskfiles
+[deprecate-version-2-schema]: ./deprecations/version_2_schema.mdx
+[output]: ./usage.mdx#output-syntax
+[ignore_errors]: ./usage.mdx#ignore-errors
+[includes]: ./usage.mdx#including-other-taskfiles
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/translate.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/translate.mdx`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/task/website/versioned_docs/version-latest/usage.mdx` & `go_task_bin-3.37.0/task/website/versioned_docs/version-latest/usage.mdx`

 * *Files 2% similar despite different names*

```diff
@@ -117,21 +117,22 @@
 ```
 
 :::
 
 ### Reading a Taskfile from stdin
 
 Taskfile also supports reading from stdin. This is useful if you are generating
-Taskfiles dynamically and don't want write them to disk. This works just like
-any other program that supports stdin. For example:
+Taskfiles dynamically and don't want write them to disk. To tell task to read
+from stdin, you must specify the `-t/--taskfile` flag with the special `-`
+value. You may then pipe into Task as you would any other program:
 
 ```shell
-task < <(cat ./Taskfile.yml)
+task -t - <(cat ./Taskfile.yml)
 # OR
-cat ./Taskfile.yml | task
+cat ./Taskfile.yml | task -t -
 ```
 
 ## Environment variables
 
 ### Task
 
 You can use `env` to set custom environment variables for a specific task:
@@ -943,16 +944,34 @@
     # Make sure these variables are set before running
     requires:
       vars: [IMAGE_NAME, IMAGE_TAG]
 ```
 
 ## Variables
 
-When doing interpolation of variables, Task will look for the below. They are
-listed below in order of importance (i.e. most important first):
+Task allows you to set variables using the `vars` keyword. The following
+variable types are supported:
+
+- `string`
+- `bool`
+- `int`
+- `float`
+- `array`
+
+:::note
+
+Maps are not supported by default, but there is an
+[experiment][map-variables] that can be enabled to add support. If
+you're interested in this functionality, we would appreciate your feedback.
+:pray:
+
+:::
+
+Variables can be set in many places in a Taskfile. When executing templates,
+Task will look for variables in the order listed below (most important first):
 
 - Variables declared in the task definition
 - Variables given while calling a task from another (See
   [Calling another task](#calling-another-task) above)
 - Variables of the [included Taskfile](#including-other-taskfiles) (when the
   task is included)
 - Variables of the [inclusion of the Taskfile](#vars-of-included-taskfiles)
@@ -1089,44 +1108,64 @@
       - for: sources
         cmd: cat {{joinPath .MY_DIR .ITEM}}
 ```
 
 ### Looping over variables
 
 To loop over the contents of a variable, you simply need to specify the variable
-you want to loop over. By default, variables will be split on any whitespace
-characters.
+you want to loop over. By default, string variables will be split on any
+whitespace characters.
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     vars:
       MY_VAR: foo.txt bar.txt
     cmds:
       - for: { var: MY_VAR }
         cmd: cat {{.ITEM}}
 ```
 
-If you need to split on a different character, you can do this by specifying the
-`split` property:
+If you need to split a string on a different character, you can do this by
+specifying the `split` property:
 
 ```yaml
 version: '3'
 
 tasks:
   default:
     vars:
       MY_VAR: foo.txt,bar.txt
     cmds:
       - for: { var: MY_VAR, split: ',' }
         cmd: cat {{.ITEM}}
 ```
 
+You can also loop over arrays directly (and maps if you have the
+[maps experiment](/experiments/map-variables) enabled):
+
+```yaml
+version: 3
+
+tasks:
+  foo:
+    vars:
+      LIST: [foo, bar, baz]
+    cmds:
+      - for:
+          var: LIST
+        cmd: echo {{.ITEM}}
+```
+
+When looping over a map we also make an additional `{{.KEY}}` variable available
+that holds the string value of the map key. Remember that maps are unordered, so
+the order in which the items are looped over is random.
+
 All of this also works with dynamic variables!
 
 ```yaml
 version: '3'
 
 tasks:
   default:
@@ -1373,15 +1412,15 @@
   space.
 - `toSlash`: Does nothing on Unix, but on Windows converts a string from `\`
   path format to `/`.
 - `fromSlash`: Opposite of `toSlash`. Does nothing on Unix, but on Windows
   converts a string from `/` path format to `\`.
 - `exeExt`: Returns the right executable extension for the current OS (`".exe"`
   for Windows, `""` for others).
-- `shellQuote`: Quotes a string to make it safe for use in shell scripts. Task
+- `shellQuote` (aliased to `q`): Quotes a string to make it safe for use in shell scripts. Task
   uses [this Go function](https://pkg.go.dev/mvdan.cc/sh/v3@v3.4.0/syntax#Quote)
   for this. The Bash dialect is assumed.
 - `splitArgs`: Splits a string as if it were a command's arguments. Task uses
   [this Go function](https://pkg.go.dev/mvdan.cc/sh/v3@v3.4.0/shell#Fields)
 - `joinPath`: Joins any number of arguments into a path. The same as Go's
   [filepath.Join](https://pkg.go.dev/path/filepath#Join).
 - `relPath`: Converts an absolute path (second argument) into a relative path,
@@ -1952,8 +1991,9 @@
 when running from the CLI via `task my-watch-task`, but won't run in watch mode
 if called by another task, either directly or as a dependency.
 
 :::
 
 {/* prettier-ignore-start */}
 [gotemplate]: https://golang.org/pkg/text/template/
+[map-variables]: ./experiments/map_variables.mdx
 {/* prettier-ignore-end */}
```

### Comparing `go_task_bin-3.36.0/task/website/yarn.lock` & `go_task_bin-3.37.0/task/website/yarn.lock`

 * *Files identical despite different names*

### Comparing `go_task_bin-3.36.0/PKG-INFO` & `go_task_bin-3.37.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: go-task-bin
-Version: 3.36.0
+Version: 3.37.0
 Summary: task - A task runner / simpler Make alternative written in Go
 Keywords: build,build-tool,devops,go,make,makefile,runner,task,task-runner,taskfile,tool
 Author-Email: dowon <ks2515@naver.com>
 License: MIT
 Classifier: Programming Language :: Other
 Classifier: Topic :: Software Development :: Build Tools
 Project-URL: Repository, https://github.com/Bing-su/pip-binary-factory
```

