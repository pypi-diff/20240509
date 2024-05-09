# Comparing `tmp/patchwork_cli-0.0.6.tar.gz` & `tmp/patchwork_cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchwork_cli-0.0.6.tar", max compression
+gzip compressed data, was "patchwork_cli-0.0.7.tar", max compression
```

## Comparing `patchwork_cli-0.0.6.tar` & `patchwork_cli-0.0.7.tar`

### file list

```diff
@@ -1,93 +1,132 @@
--rw-r--r--   0        0        0    34523 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/LICENSE
--rw-r--r--   0        0        0     5534 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/__main__.py
--rw-r--r--   0        0        0     3953 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/app.py
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/common/client/__init__.py
--rw-r--r--   0        0        0    12704 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/common/client/scm.py
--rw-r--r--   0        0        0      816 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/common/utils.py
--rw-r--r--   0        0        0     1548 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/interpreter.py
--rw-r--r--   0        0        0     1546 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/logger.py
--rw-r--r--   0        0        0      168 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/managed_files.py
--rw-r--r--   0        0        0     3724 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/AutoFix.py
--rw-r--r--   0        0        0     4783 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/README.md
--rw-r--r--   0        0        0     2182 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/default_prompt.json
--rw-r--r--   0        0        0      869 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/defaults.yml
--rw-r--r--   0        0        0     5434 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
--rw-r--r--   0        0        0     5418 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/README.md
--rw-r--r--   0        0        0      704 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/defaults.yml
--rw-r--r--   0        0        0     2495 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
--rw-r--r--   0        0        0     2210 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/GenerateREADME.py
--rw-r--r--   0        0        0     3834 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/README.md
--rw-r--r--   0        0        0      612 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/defaults.yml
--rw-r--r--   0        0        0      484 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
--rw-r--r--   0        0        0     3551 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/PRReview/PRReview.py
--rw-r--r--   0        0        0     3631 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/PRReview/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/PRReview/__init__.py
--rw-r--r--   0        0        0      608 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/PRReview/defaults.yml
--rw-r--r--   0        0        0      557 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/PRReview/pr_review_prompt.json
--rw-r--r--   0        0        0     2163 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/README.md
--rw-r--r--   0        0        0      276 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/__init__.py
--rw-r--r--   0        0        0      499 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/step.py
--rw-r--r--   0        0        0     5970 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
--rw-r--r--   0        0        0     1205 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/AnalyzeImpact/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/AnalyzeImpact/__init__.py
--rw-r--r--   0        0        0     2437 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
--rw-r--r--   0        0        0      967 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/README.md
--rw-r--r--   0        0        0      575 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/__init__.py
--rw-r--r--   0        0        0     4131 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallOpenAI/CallOpenAI.py
--rw-r--r--   0        0        0      503 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallOpenAI/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallOpenAI/__init__.py
--rw-r--r--   0        0        0     5255 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CommitChanges/CommitChanges.py
--rw-r--r--   0        0        0     1106 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CommitChanges/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CommitChanges/__init__.py
--rw-r--r--   0        0        0     3907 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePR/CreatePR.py
--rw-r--r--   0        0        0     1279 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePR/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePR/__init__.py
--rw-r--r--   0        0        0     1358 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePRComment/CreatePRComment.py
--rw-r--r--   0        0        0      621 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePRComment/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePRComment/__init__.py
--rw-r--r--   0        0        0    11565 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/ExtractCode.py
--rw-r--r--   0        0        0      755 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/__init__.py
--rw-r--r--   0        0        0     2585 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
--rw-r--r--   0        0        0      593 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/generic.py
--rw-r--r--   0        0        0     1491 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/java.py
--rw-r--r--   0        0        0     2442 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/javascript.py
--rw-r--r--   0        0        0      281 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/protocol.py
--rw-r--r--   0        0        0     2885 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/python.py
--rw-r--r--   0        0        0     8880 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractDiff/ExtractDiff.py
--rw-r--r--   0        0        0      833 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractDiff/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractDiff/__init__.py
--rw-r--r--   0        0        0     1648 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
--rw-r--r--   0        0        0     1318 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractModelResponse/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractModelResponse/__init__.py
--rw-r--r--   0        0        0    12392 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
--rw-r--r--   0        0        0     1765 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/README.md
--rw-r--r--   0        0        0     6173 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/__init__.py
--rw-r--r--   0        0        0     3366 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ModifyCode/ModifyCode.py
--rw-r--r--   0        0        0     1045 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ModifyCode/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ModifyCode/__init__.py
--rw-r--r--   0        0        0     3122 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePR/PreparePR.py
--rw-r--r--   0        0        0      743 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePR/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePR/__init__.py
--rw-r--r--   0        0        0     3262 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePrompt/PreparePrompt.py
--rw-r--r--   0        0        0     1274 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePrompt/README.md
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePrompt/__init__.py
--rw-r--r--   0        0        0     1652 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/README.md
--rw-r--r--   0        0        0      903 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ReadPRDiffs/README.md
--rw-r--r--   0        0        0     1764 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ReadPRDiffs/__init__.py
--rw-r--r--   0        0        0     1588 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/README.md
--rw-r--r--   0        0        0     4744 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/ScanDepscan.py
--rw-r--r--   0        0        0     2026 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/TestScanDepscan.py
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/__init__.py
--rw-r--r--   0        0        0      677 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanSemgrep/README.md
--rw-r--r--   0        0        0     1055 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanSemgrep/ScanSemgrep.py
--rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanSemgrep/__init__.py
--rw-r--r--   0        0        0     1481 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/__init__.py
--rw-r--r--   0        0        0     2243 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     7213 1970-01-01 00:00:00.000000 patchwork_cli-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4798 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/__main__.py
+-rw-r--r--   0        0        0     5253 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/app.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/common/client/__init__.py
+-rw-r--r--   0        0        0    15540 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/common/client/scm.py
+-rw-r--r--   0        0        0     3964 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/common/utils.py
+-rw-r--r--   0        0        0     1546 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/logger.py
+-rw-r--r--   0        0        0      168 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/managed_files.py
+-rw-r--r--   0        0        0     3718 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/AutoFix/AutoFix.py
+-rw-r--r--   0        0        0     6059 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/AutoFix/README.md
+-rw-r--r--   0        0        0     2182 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/AutoFix/default_prompt.json
+-rw-r--r--   0        0        0      920 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/AutoFix/defaults.yml
+-rw-r--r--   0        0        0     5422 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
+-rw-r--r--   0        0        0     5441 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/DependencyUpgrade/README.md
+-rw-r--r--   0        0        0      755 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/DependencyUpgrade/defaults.yml
+-rw-r--r--   0        0        0     2495 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
+-rw-r--r--   0        0        0     2204 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/GenerateREADME/GenerateREADME.py
+-rw-r--r--   0        0        0     3855 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/GenerateREADME/README.md
+-rw-r--r--   0        0        0      663 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/GenerateREADME/defaults.yml
+-rw-r--r--   0        0        0      484 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
+-rw-r--r--   0        0        0     3542 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/PRReview/PRReview.py
+-rw-r--r--   0        0        0     3653 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/PRReview/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/PRReview/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/PRReview/defaults.yml
+-rw-r--r--   0        0        0      557 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/PRReview/pr_review_prompt.json
+-rw-r--r--   0        0        0     2163 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/README.md
+-rw-r--r--   0        0        0     3773 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/ResolveIssue/README.md
+-rw-r--r--   0        0        0     3616 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/ResolveIssue/ResolveIssue.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/ResolveIssue/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/ResolveIssue/defaults.yml
+-rw-r--r--   0        0        0      728 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/ResolveIssue/prompt.json
+-rw-r--r--   0        0        0      344 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/patchflows/__init__.py
+-rw-r--r--   0        0        0      499 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/step.py
+-rw-r--r--   0        0        0     5984 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
+-rw-r--r--   0        0        0     1205 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/AnalyzeImpact/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/AnalyzeImpact/__init__.py
+-rw-r--r--   0        0        0      501 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/AnalyzeImpact/typed.py
+-rw-r--r--   0        0        0     2461 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
+-rw-r--r--   0        0        0      967 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CallCode2Prompt/README.md
+-rw-r--r--   0        0        0      575 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CallCode2Prompt/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CallCode2Prompt/typed.py
+-rw-r--r--   0        0        0     7462 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CallLLM/CallLLM.py
+-rw-r--r--   0        0        0      503 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CallLLM/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CallLLM/__init__.py
+-rw-r--r--   0        0        0      453 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CallLLM/typed.py
+-rw-r--r--   0        0        0     5255 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CommitChanges/CommitChanges.py
+-rw-r--r--   0        0        0     1106 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CommitChanges/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CommitChanges/__init__.py
+-rw-r--r--   0        0        0      368 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CommitChanges/typed.py
+-rw-r--r--   0        0        0     1346 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreateIssueComment/CreateIssueComment.py
+-rw-r--r--   0        0        0      541 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreateIssueComment/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreateIssueComment/__init__.py
+-rw-r--r--   0        0        0      320 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreateIssueComment/typed.py
+-rw-r--r--   0        0        0     3907 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreatePR/CreatePR.py
+-rw-r--r--   0        0        0     1279 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreatePR/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreatePR/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreatePR/typed.py
+-rw-r--r--   0        0        0     1358 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreatePRComment/CreatePRComment.py
+-rw-r--r--   0        0        0      621 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreatePRComment/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreatePRComment/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/CreatePRComment/typed.py
+-rw-r--r--   0        0        0    11511 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/ExtractCode.py
+-rw-r--r--   0        0        0      755 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.935801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/__init__.py
+-rw-r--r--   0        0        0     2585 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
+-rw-r--r--   0        0        0      593 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/generic.py
+-rw-r--r--   0        0        0     1491 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/java.py
+-rw-r--r--   0        0        0     2442 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/javascript.py
+-rw-r--r--   0        0        0      281 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/protocol.py
+-rw-r--r--   0        0        0     2885 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/python.py
+-rw-r--r--   0        0        0      463 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractCode/typed.py
+-rw-r--r--   0        0        0     8897 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractDiff/ExtractDiff.py
+-rw-r--r--   0        0        0      833 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractDiff/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractDiff/__init__.py
+-rw-r--r--   0        0        0      404 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractDiff/typed.py
+-rw-r--r--   0        0        0     1648 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
+-rw-r--r--   0        0        0     1318 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractModelResponse/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractModelResponse/__init__.py
+-rw-r--r--   0        0        0      301 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractModelResponse/typed.py
+-rw-r--r--   0        0        0    12415 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
+-rw-r--r--   0        0        0     1765 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractPackageManagerFile/README.md
+-rw-r--r--   0        0        0     6173 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractPackageManagerFile/__init__.py
+-rw-r--r--   0        0        0      338 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ExtractPackageManagerFile/typed.py
+-rw-r--r--   0        0        0     5337 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/GenerateCodeRepositoryEmbeddings/GenerateCodeRepositoryEmbeddings.py
+-rw-r--r--   0        0        0     1572 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/GenerateCodeRepositoryEmbeddings/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/GenerateCodeRepositoryEmbeddings/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/GenerateCodeRepositoryEmbeddings/typed.py
+-rw-r--r--   0        0        0     2941 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/GenerateEmbeddings/GenerateEmbeddings.py
+-rw-r--r--   0        0        0     1011 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/GenerateEmbeddings/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/GenerateEmbeddings/__init__.py
+-rw-r--r--   0        0        0      238 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/GenerateEmbeddings/typed.py
+-rw-r--r--   0        0        0     3366 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ModifyCode/ModifyCode.py
+-rw-r--r--   0        0        0     1045 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ModifyCode/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ModifyCode/__init__.py
+-rw-r--r--   0        0        0      346 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ModifyCode/typed.py
+-rw-r--r--   0        0        0     3125 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/PreparePR/PreparePR.py
+-rw-r--r--   0        0        0      743 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/PreparePR/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/PreparePR/__init__.py
+-rw-r--r--   0        0        0      327 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/PreparePR/typed.py
+-rw-r--r--   0        0        0     3289 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/PreparePrompt/PreparePrompt.py
+-rw-r--r--   0        0        0     1274 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/PreparePrompt/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/PreparePrompt/__init__.py
+-rw-r--r--   0        0        0      335 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/PreparePrompt/typed.py
+-rw-r--r--   0        0        0     2617 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/QueryEmbeddings/QueryEmbeddings.py
+-rw-r--r--   0        0        0     1117 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/QueryEmbeddings/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/QueryEmbeddings/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/QueryEmbeddings/typed.py
+-rw-r--r--   0        0        0     1652 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/README.md
+-rw-r--r--   0        0        0     1078 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ReadIssues/README.md
+-rw-r--r--   0        0        0     1149 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ReadIssues/ReadIssues.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ReadIssues/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ReadIssues/typed.py
+-rw-r--r--   0        0        0      903 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ReadPRDiffs/README.md
+-rw-r--r--   0        0        0     1830 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ReadPRDiffs/__init__.py
+-rw-r--r--   0        0        0      362 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ReadPRDiffs/typed.py
+-rw-r--r--   0        0        0     1588 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ScanDepscan/README.md
+-rw-r--r--   0        0        0     4884 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ScanDepscan/ScanDepscan.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ScanDepscan/__init__.py
+-rw-r--r--   0        0        0      189 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ScanDepscan/typed.py
+-rw-r--r--   0        0        0      677 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ScanSemgrep/README.md
+-rw-r--r--   0        0        0     1096 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ScanSemgrep/ScanSemgrep.py
+-rw-r--r--   0        0        0        0 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ScanSemgrep/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/ScanSemgrep/typed.py
+-rw-r--r--   0        0        0     2045 2024-05-09 04:12:52.939801 patchwork_cli-0.0.7/patchwork/steps/__init__.py
+-rw-r--r--   0        0        0     2285 2024-05-09 04:12:52.943801 patchwork_cli-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6612 1970-01-01 00:00:00.000000 patchwork_cli-0.0.7/PKG-INFO
```

### Comparing `patchwork_cli-0.0.6/LICENSE` & `patchwork_cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/README.md` & `patchwork_cli-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <p align="center">
   <img src="https://github.com/patched-codes/patchwork/assets/126385808/a7adcf24-b615-43a0-a244-45789d184f0a" width="160" alt="PatchWork Logo">
 </p>
 
 # PatchWork
 
-An open-source framework for patching and managing code repositories using large language models. PatchWork allows you to automate workflows like PR reviews, bug fixing, security patching, and more using a self-hosted CLI agent and your preferred LLMs.
+An open-source framework for automating development chores using large language models. PatchWork allows you to automate workflows like PR reviews, bug fixing, security patching, and more using a self-hosted CLI agent and your preferred LLMs.
 
 ## Key Components
 
 - **Steps**: A set of reusable atomic actions that define various operations.
 - **Patchflows**: LLM-assisted automations such as PR reviews, code fixing, debugging.
 
 Patchflows can be run locally in your CLI and IDE, or as part of your CI/CD pipeline.
@@ -69,120 +69,60 @@
 
 ```bash
 patchwork AutoFix openai_api_key=<YOUR_OPENAI_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
 The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities.
 
-You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
-
-The [patchwork-configs](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
+You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. You will need to pass your own `openai_api_key` to call the LLM. Otherwise, to get started, you can get a `patched_api_key` for free by
+by signing in at [https://app.patched.codes/signin](https://app.patched.codes/signin) and generating an API key from the integrations tab. You can then call the patchflow with the key as follows:
 
 ```bash
-patchwork AutoFix --config /path/to/patchwork-configs/patchflows
-```
-
-## PatchWork in CI
-
-You can also run PatchWork in a CI environment with ease:
-
-### Jenkins CI
-
-```groovy
-pipeline {
-  agent any
-    stages {
-      stage('Auto Fix Vulnerabilities') {
-        steps {
-          sh 'pip3 install patchwork'
-          sh 'patchwork AutoFix'
-      }
-    }
-  }
-}
-```
-
-### GitHub Actions
-
-- **Workflow**
-```yaml
-name: Auto Fix Vulnerabilities
-
-on:
-  # Patch files in PRs (diff-aware scanning):
-  pull_request: {}
-  # Patch on-demand through GitHub Actions interface:
-  workflow_dispatch: {}
-
-jobs:
-  patchwork:
-    # User definable name of this GitHub Actions job.
-    name: patchwork/ci
-    runs-on: ubuntu-latest
-
-    container:
-      # A Docker image with patchwork installed. Do not change this.
-      image: patched-codes/patchwork
-
-    steps:
-      # Fetch project source with GitHub Actions Checkout.
-      - uses: actions/checkout@v3
-      # Run the "patchwork" command on the command line of the docker image.
-      - run: patchwork AutoFix
+patchwork AutoFix patched_api_key=<YOUR_PATCHED_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
-- **Action (Available on Github Marketplace)**
-
-```yaml
-- name: Auto Fix Vulnerabilities
-  uses: patchwork/AutoFix@main
-```
-
-### Gitlab CI
-
-```yaml
-patchwork:
-  # A Docker image with PatchWork installed.
-  image: patched-codes/patchwork
-  # Run "patchwork" command on the command line of the docker image.
-  script: patchwork AutoFix
-
-  rules:
-  # Patch changed files in MRs, (diff-aware patching):
-  - if: $CI_MERGE_REQUEST_IID
+The [patchwork-configs](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
 
-  # Patch mainline (default) branches and fix all findings.
-  - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
+```bash
+patchwork AutoFix --config /path/to/patchwork-configs/patchflows
 ```
 
 ## Patchflows
 
 Patchwork comes with a set of predefined patchflows, and more will be added over time. Below is a sample list of patchflows:
 
 - AutoFix: Generate and apply fixes to code vulnerabilities in a repository.
 - DependencyUpgrade: Update your dependencies from vulnerable to fixed versions.
 - PRReview: On PR creation, extract code diff, summarize changes, and comment on PR.
 - GenerateREADME: Create a README.md file for a given folder, to add documentation to your repository.
+- ResolveIssue: Identify the files in your repository that need to be updated to resolve an issue (or bug) and create a PR to fix it.
 
 ## Prompt Templates
 
 Prompt templates are used by patchflows and passed as queries to LLMs. Templates contain prompts with placeholder variables enclosed by {{}} which are replaced by the data from the steps or inputs on every run. 
 
 Below is a sample prompt template:
 
 ```json
 {
-    "id": "ReviewPR",
+  "id": "diffreview_summary",
     "prompts": [
-        {"role": "system", "content": "You are a helpful assistant."},
-        {"role": "user", "content": "Create a well-structured message for the pull request body based on a review of the code diff. CODE DIFF - {{prDiff}}"}
+      {
+        "role": "user",
+        "content": "Summarize the following code change descriptions in 1 paragraph. {{diffreviews}}"
+      }
     ]
 }
 ```
 
 Each patchflow comes with an optimized default prompt template. But you can specify your own using the `prompt_template_file=/path/to/prompt/template/file` option. 
 
 ## Contributing
 
 To create a new patchflow, follow [these instructions](patchwork/patchflows/README.md).
 
 To create a new step, follow [these instructions](patchwork/steps/README.md).
+
+We also provide chat assitants to help you create new steps and patchflows easily.
+
+- [Patchwork Assistant GPT](https://chatgpt.com/g/g-0G4sCAd2y-patchwork-assistant) (requires ChatGPT pro subscription)
+- [Patchwork Assistant on HuggingChat ](https://hf.co/chat/assistant/66322701fd4787e0c1f7696b) (free)
```

### Comparing `patchwork_cli-0.0.6/patchwork/app.py` & `patchwork_cli-0.0.7/patchwork/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 import importlib
+import importlib.util
 import json
 import traceback
+from collections import deque
 from pathlib import Path
+from types import ModuleType
+from typing import Iterable
 
 import click
 import yaml
 
 from patchwork.logger import init_cli_logger, logger
 from patchwork.steps.PreparePrompt import PreparePrompt
 
+_DATA_FORMAT_MAPPING = {
+    "yaml": yaml.dump,
+    "json": json.dumps,
+}
 
-def _get_config_path(config: str, patchflow: str) -> tuple[Path | None, Path | None]:
-    config_path = Path(config)
-    prompt_path = None
-    if config_path.is_dir():
-        patchwork_config_path = config_path / patchflow / "config.yml"
-        patchwork_prompt_path = config_path / patchflow / "prompt.json"
-        config_path = None
-
-        if patchwork_config_path.is_file():
-            config_path = patchwork_config_path
-        else:
-            logger.warning(
-                f'Config file "{patchwork_config_path}" not found from directory "{config}", using default config'
-            )
+_CONFIG_NAME = "config.yml"
+_PROMPT_NAME = "prompt.json"
+_PATCHFLOW_MODULE_NAME = "patchwork.patchflows"
 
-        if patchwork_prompt_path.is_file():
-            prompt_path = patchwork_prompt_path
-        else:
-            logger.warning(
-                f'Prompt file "{patchwork_prompt_path}" not found from directory "{config}", using default prompt'
-            )
 
-    return config_path, prompt_path
+def _get_config_path(config: str | None, patchflow: str) -> Path | None:
+    prompt_path = None
+    config_path = Path(config)
+    if config_path.is_dir():
+        patchwork_path = config_path / patchflow
+        if patchwork_path.is_dir():
+            return patchwork_path
 
 
 @click.command(
     context_settings=dict(
         ignore_unknown_options=True,
     )
 )
-@click.version_option(message="%(version)s")
+@click.version_option(message="%(version)s", package_name="patchwork-cli")
 @click.help_option("-h", "--help")
 @click.option(
     "--log",
     hidden=True,
     default="INFO",
     type=click.Choice(
         [
@@ -63,64 +60,99 @@
 )
 @click.argument("patchflow", nargs=1, required=True)
 @click.argument("opts", nargs=-1, type=click.UNPROCESSED, required=False)
 @click.option("--config", type=click.Path(exists=True, dir_okay=True, resolve_path=True, file_okay=True))
 @click.option("--output", type=click.Path(exists=False, resolve_path=True, writable=True), help="Output data file")
 @click.option("data_format", "--format", type=click.Choice(["yaml", "json"]), default="json", help="Output data format")
 def cli(log: str, patchflow: str, opts: list[str], config: str | None, output: str | None, data_format: str):
-    try:
-        module = importlib.import_module(".patchflows", "patchwork")
-    except ModuleNotFoundError:
-        logger.debug(f"Patchflow {patchflow} not found")
-        exit(1)
-
-    try:
-        patchflow_class = getattr(module, patchflow)
-    except AttributeError:
-        logger.debug(f"Patchflow {patchflow} not found as a class in {Path(__file__).parent / 'patchflows'}")
-        from patchwork.interpreter import run_chat
-
-        run_chat()
-        exit(1)
+    if "::" in patchflow:
+        module_path, _, patchflow_name = patchflow.partition("::")
+    else:
+        patchflow_name = patchflow
+        module_path = _PATCHFLOW_MODULE_NAME
 
+    possbile_module_paths = deque((module_path,))
     inputs = {}
+
     if config is not None:
-        config_path, prompt_path = _get_config_path(config, patchflow)
-        if config_path is None and prompt_path is None:
+        config_path = Path(config)
+        if config_path.is_file():
+            inputs = yaml.safe_load(config_path.read_text()) or {}
+        elif config_path.is_dir():
+            patchwork_path = config_path / patchflow_name
+
+            patchwork_python_path = patchwork_path / f"{patchflow_name}.py"
+            if patchwork_python_path.is_file():
+                possbile_module_paths.appendleft(str(patchwork_python_path.resolve()))
+
+            patchwork_config_path = patchwork_path / _CONFIG_NAME
+            if patchwork_config_path.is_file():
+                inputs = yaml.safe_load(patchwork_config_path.read_text()) or {}
+            else:
+                logger.warning(
+                    f'Config file "{patchwork_config_path}" not found from directory "{config}", using default config'
+                )
+
+            patchwork_prompt_path = patchwork_path / _PROMPT_NAME
+            if patchwork_prompt_path.is_file():
+                inputs[PreparePrompt.PROMPT_TEMPLATE_FILE_KEY] = patchwork_prompt_path
+            else:
+                logger.warning(
+                    f'Prompt file "{patchwork_prompt_path}" not found from directory "{config}", using default prompt'
+                )
+        else:
+            logger.error(f"Config path {config} is not a file or directory")
             exit(1)
 
-        if config_path is not None:
-            inputs = yaml.safe_load(config_path.read_text())
-        if prompt_path is not None:
-            inputs[PreparePrompt.PROMPT_TEMPLATE_FILE_KEY] = prompt_path
-
     for opt in opts:
         key, equal_sign, value = opt.partition("=")
         key = key.lstrip("-")
 
         if equal_sign == "":
             # treat --key as a flag
             inputs[key] = True
         else:
             # treat --key=value as a key-value pair
             inputs[key] = value
+
+    module = find_module(possbile_module_paths, patchflow)
+
+    try:
+        patchflow_class = getattr(module, patchflow_name)
+    except AttributeError:
+        logger.debug(f"Patchflow {patchflow} not found as a class in {module_path}")
+        exit(1)
+
     try:
         patchflow_instance = patchflow_class(inputs)
         patchflow_instance.run()
     except Exception as e:
         logger.debug(traceback.format_exc())
         logger.error(f"Error running patchflow {patchflow}: {e}")
         exit(1)
 
-    data_format_mapping = {
-        "yaml": yaml.dump,
-        "json": json.dumps,
-    }
-
     if output is not None:
-        serialize = data_format_mapping.get(data_format, json.dumps)
+        serialize = _DATA_FORMAT_MAPPING.get(data_format, json.dumps)
         with open(output, "w") as file:
             file.write(serialize(inputs))
 
 
+def find_module(possible_module_paths: Iterable[str], patchflow: str) -> ModuleType | None:
+    for module_path in possible_module_paths:
+        try:
+            spec = importlib.util.spec_from_file_location("custom_module", module_path)
+            module = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(module)
+            return module
+        except Exception:
+            logger.debug(f"Patchflow {patchflow} not found as a file/directory in {module_path}")
+
+        try:
+            return importlib.import_module(module_path)
+        except ModuleNotFoundError:
+            logger.debug(f"Patchflow {patchflow} not found as a module in {module_path}")
+
+    return None
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `patchwork_cli-0.0.6/patchwork/common/client/scm.py` & `patchwork_cli-0.0.7/patchwork/common/client/scm.py`

 * *Files 15% similar despite different names*

```diff
@@ -101,14 +101,23 @@
 class ScmPlatformClientProtocol(Protocol):
     def test(self) -> bool:
         ...
 
     def set_url(self, url: str) -> None:
         ...
 
+    def get_slug_and_id_from_url(self, url: str) -> tuple[str, int] | None:
+        ...
+
+    def find_issue_by_url(self, url: str) -> list[str] | None:
+        ...
+
+    def find_issue_by_id(self, slug: str, issue_id: int) -> list[str] | None:
+        ...
+
     def get_pr_by_url(self, url: str) -> PullRequestProtocol | None:
         ...
 
     def find_pr_by_id(self, slug: str, pr_id: int) -> PullRequestProtocol | None:
         ...
 
     def find_pr(self, slug: str, original_branch: str, feature_branch: str) -> PullRequestProtocol | None:
@@ -120,14 +129,19 @@
         title: str,
         body: str,
         original_branch: str,
         feature_branch: str,
     ) -> PullRequestProtocol:
         ...
 
+    def create_issue_comment(
+        self, slug: str, issue_text: str, title: str | None = None, issue_id: int | None = None
+    ) -> str:
+        ...
+
 
 class GitlabMergeRequest(PullRequestProtocol):
     def __init__(self, mr: ProjectMergeRequest):
         self._mr = mr
 
     def url(self) -> str:
         return self._mr.web_url
@@ -259,29 +273,48 @@
 
     def test(self) -> bool:
         return True
 
     def set_url(self, url: str) -> None:
         self._url = url
 
-    def get_pr_by_url(self, url: str) -> PullRequestProtocol | None:
+    def get_slug_and_id_from_url(self, url: str) -> tuple[str, int] | None:
         url_parts = url.split("/")
         if len(url_parts) < 5:
-            logger.error(f"Invalid PR URL: {url}")
+            logger.error(f"Invalid issue URL: {url}")
             return None
 
         try:
-            pr_id = url_parts[-1]
+            resource_id = int(url_parts[-1])
         except ValueError:
-            logger.error(f"Invalid PR URL: {url}")
+            logger.error(f"Invalid issue URL: {url}")
             return None
 
         slug = "/".join(url_parts[-4:-2])
 
-        return self.find_pr_by_id(slug, int(pr_id))
+        return slug, resource_id
+
+    def find_issue_by_url(self, url: str) -> list[str] | None:
+        slug, issue_id = self.get_slug_and_id_from_url(url)
+        return self.find_issue_by_id(slug, issue_id)
+
+    def find_issue_by_id(self, slug: str, issue_id: int) -> list[str] | None:
+        repo = self.github.get_repo(slug)
+        try:
+            issue = repo.get_issue(issue_id)
+            body = issue.body
+            comments = [issue_comment.body for issue_comment in issue.get_comments()]
+            return [body] + comments
+        except GithubException as e:
+            logger.warn(f"Failed to get issue: {e}")
+            return None
+
+    def get_pr_by_url(self, url: str) -> PullRequestProtocol | None:
+        slug, pr_id = self.get_slug_and_id_from_url(url)
+        return self.find_pr_by_id(slug, pr_id)
 
     def find_pr_by_id(self, slug: str, pr_id: int) -> PullRequestProtocol | None:
         repo = self.github.get_repo(slug)
         try:
             pr = repo.get_pull(pr_id)
             return GithubPullRequest(pr)
         except GithubException as e:
@@ -307,14 +340,23 @@
     ) -> PullRequestProtocol:
         # before creating a PR, check if one already exists
         repo = self.github.get_repo(slug)
         gh_pr = repo.create_pull(title=title, body=body, base=original_branch, head=feature_branch)
         pr = GithubPullRequest(gh_pr)
         return pr
 
+    def create_issue_comment(
+        self, slug: str, issue_text: str, title: str | None = None, issue_id: int | None = None
+    ) -> str:
+        repo = self.github.get_repo(slug)
+        if issue_id is not None:
+            return repo.get_issue(issue_id).create_comment(issue_text).html_url
+        else:
+            return repo.create_issue(title, issue_text).html_url
+
 
 class GitlabClient(ScmPlatformClientProtocol):
     DEFAULT_URL = gitlab.const.DEFAULT_URL
 
     def __init__(self, access_token: str, url: str = DEFAULT_URL):
         self._access_token = access_token
         self._url = url
@@ -329,29 +371,48 @@
     def test(self) -> bool:
         try:
             self.gitlab.auth()
         except GitlabAuthenticationError:
             return False
         return self.gitlab.user is not None
 
-    def get_pr_by_url(self, url: str) -> PullRequestProtocol | None:
+    def get_slug_and_id_from_url(self, url: str) -> tuple[str, int] | None:
         url_parts = url.split("/")
         if len(url_parts) < 5:
-            logger.error(f"Invalid PR URL: {url}")
+            logger.error(f"Invalid issue URL: {url}")
             return None
 
         try:
-            pr_id = url_parts[-1]
+            resource_id = int(url_parts[-1])
         except ValueError:
-            logger.error(f"Invalid PR URL: {url}")
+            logger.error(f"Invalid issue URL: {url}")
             return None
 
         slug = "/".join(url_parts[-5:-3])
 
-        return self.find_pr_by_id(slug, int(pr_id))
+        return slug, resource_id
+
+    def find_issue_by_url(self, url: str) -> list[str] | None:
+        slug, issue_id = self.get_slug_and_id_from_url(url)
+        return self.find_issue_by_id(slug, issue_id)
+
+    def find_issue_by_id(self, slug: str, issue_id: int) -> list[str] | None:
+        project = self.gitlab.projects.get(slug)
+        try:
+            issue = project.issues.get(issue_id)
+            body = issue["description"]
+            comments = [note["body"] for note in issue.notes.list()]
+            return [body] + comments
+        except GitlabError as e:
+            logger.warn(f"Failed to get issue: {e}")
+            return None
+
+    def get_pr_by_url(self, url: str) -> PullRequestProtocol | None:
+        slug, pr_id = self.get_slug_and_id_from_url(url)
+        return self.find_pr_by_id(slug, pr_id)
 
     def find_pr_by_id(self, slug: str, pr_id: int) -> PullRequestProtocol | None:
         project = self.gitlab.projects.get(slug)
         try:
             mr = project.mergerequests.get(pr_id)
             return GitlabMergeRequest(mr)
         except GitlabError as e:
@@ -391,7 +452,17 @@
                 "target_branch": original_branch,
                 "title": title,
                 "description": body,
             }
         )
         mr = GitlabMergeRequest(gl_mr)  # type: ignore
         return mr
+
+    def create_issue_comment(
+        self, slug: str, issue_text: str, title: str | None = None, issue_id: int | None = None
+    ) -> str:
+        if issue_id is not None:
+            obj = self.gitlab.projects.get(slug).issues.get(issue_id).notes.create({"body": issue_text})
+            return obj["web_url"]
+
+        obj = self.gitlab.projects.get(slug).issues.create({"title": title, "description": issue_text})
+        return obj["web_url"]
```

### Comparing `patchwork_cli-0.0.6/patchwork/logger.py` & `patchwork_cli-0.0.7/patchwork/logger.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/AutoFix.py` & `patchwork_cli-0.0.7/patchwork/patchflows/AutoFix/AutoFix.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import yaml
 
 from patchwork.logger import logger
 from patchwork.step import Step
 from patchwork.steps import (
-    CallOpenAI,
+    CallLLM,
     CommitChanges,
     CreatePR,
     ExtractCode,
     ExtractModelResponse,
     ModifyCode,
     PreparePR,
     PreparePrompt,
@@ -67,15 +67,15 @@
         self.inputs.update(outputs)
         outputs = ExtractCode(self.inputs).run()
         self.inputs.update(outputs)
 
         for i in range(self.n):
             outputs = PreparePrompt(self.inputs).run()
             self.inputs.update(outputs)
-            outputs = CallOpenAI(self.inputs).run()
+            outputs = CallLLM(self.inputs).run()
             self.inputs.update(outputs)
             outputs = ExtractModelResponse(self.inputs).run()
             self.inputs.update(outputs)
 
             for extracted_response in self.inputs["extracted_responses"]:
                 response_compatibility = Compatibility.from_str(
                     extracted_response.get("compatibility", "UNKNOWN").strip()
```

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/README.md` & `patchwork_cli-0.0.7/patchwork/patchflows/DependencyUpgrade/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# AutoFix
+# DependencyUpgrade
 
-The AutoFix patchflow aims to automatically fix code vulnerabilities in your repository. 
+The DependencyUpgrade patchflow aims to automatically update vulnerable versions of dependencies in your repository to the fixed version. 
 
 ## How to run?
  
 You can run it as follows:
 
-`patchwork AutoFix`
+`patchwork DependencyUpgrade`
 
 by default you will need to provide the `openai_api_key` and the `github_api_key` you can pass them as arguments: 
 
-`patchwork AutoFix openai_api_key=<Your_API_KEY> github_api_key=<Your_GH_Token>`
+`patchwork DependencyUpgrade openai_api_key=<Your_API_KEY> github_api_key=<Your_GH_Token>`
 
 ## What it does?
 
-The AutoFix patchflow will first scan the code in your repository using an open-source scanner Semgrep. It will then take the vulnerabilities that are detected by the scan and use create a prompt to be sent to `gpt-3.5-turbo` to generate the fix for the vulnerabilities. You can check the default [prompt template](./default_prompt.json). The generated fixes are then committed to the repository under a new branch and finally a pull request is created for the user to review and merge the changes. 
+The DependencyUpgrade patchflow will first scan your repository using an open-source scanner [dep-scan](https://github.com/owasp-dep-scan/dep-scan). It will then extract the vulnerable libraries information detected by the scan and use them to create a prompt to be sent to `gpt-3.5-turbo` to update your package manager file. You can check the default [prompt template](./dependency_upgrade_prompt.json). The fixed package manager file is then committed to the repository under a new branch and finally a pull request is created for the user to review and merge the changes. 
 
 ## Configuration
 
-The following are the default configurations that can be modified by the user to adapt the AutoFix patchflow to their needs. All the options can be set both via CLI arguments and and the yaml config file.
+The following are the default configurations that can be modified by the user to adapt the DependencyUpgrade patchflow to their needs. All the options can be set both via CLI arguments and and the yaml config file.
 
 ### Model
 
 You can choose any LLM API as long as it has an OpenAI API compatible chat completions endpoint. Just update the default values of the following options:
 
 ```yaml
 - model: gpt-3.5-turbo
@@ -38,75 +38,65 @@
 model_top_p: 0.95
 model_max_tokens: 2000
 ```
 and pass your HuggingFace token in the `openai_api_key` option.
 
 You can also use llama.cpp to run inference on CPU locally. Just install the [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) package and run their OpenAI compatible web server as described [here](https://github.com/abetlen/llama-cpp-python) with the command:
 
-`python3 -m llama_cpp.server --hf_model_repo_id TheBloke/deepseek-coder-6.7B-instruct-GGUF --model 'deepseek-coder-6.7b-instruct.Q4_0.gguf'`
+`python3 -m llama_cpp.server --hf_model_repo_id TheBloke/deepseek-coder-6.7B-instruct-GGUF --model 'deepseek-coder-6.7b-instruct.Q4_K_M.gguf' --chat_format chatml`
 
 Once the local server is running you can set:
 
 ```yaml
 client_base_url: http://localhost:8000/v1
 model: TheBloke/deepseek-coder-6.7B-instruct-GGUF
 model_temperature: 0.2
 model_top_p: 0.95
 model_max_tokens: 1000
 ```
 and use the local model for inference.
 
-### Context size
-By default we chunk the code to `context_size` tokens to pass on to the LLM. You can change the default value by setting:
+### Upgrade Threshold
+You can set the upgrade threshold you want to update the libraries to. The accepted values are 'major', 'minor' or  'patch'.
+E.g.
+```yaml
+upgrade_threshold: minor
+```
+would only upgrade across minor and patch versions of the library, i.e. an upgrade to another major wouldn't be done.
 
+### Severity
+You can also set the severity of the vulnerabilities that you want to upgrade. Severity is derived from the CVSS score and can take values of 'none', 'low', 'medium', 'high', and 'critical'. 
+E.g.
 ```yaml
-context_size: 1000
+severity: medium
 ```
-in general we have found that a larger `context_size `doesn't necessarily lead to better fixes.
+means that all libraries that have medium and above vulnerabilities will be upgraded.
 
-### Vulnerability limit
-By default we process and fix only `vulnerability_limit` number of issues. This is to avoid making large number of LLMs calls and to keep the generated PR manageable. You can set the value to your preference:
+### Analyze Impact
+By default we update the libraries to their fixed versions. If the upgrades are across major versions or a lot has changed between the versions of the library updating it may break your application. The `analyze_impact` option can be set to enable an impact analysis of the library upgrades as follows:
 
 ```yaml
-vulnerability_limit: 10
-``` 
+analyze_impact: true
+libraries_api_key: <Your_API_KEY>
+```
+This will get the diff between the vulnerable and fixed versions of the library and determine the impacted methods. Then, we will analyze your repository to determine if you are using the impacted methods. And, finally we will use this information to prompt an LLM to migrate the code that uses these impacted methods in your repository. The code changes are then committed in a new branch in your repository to be included in the same PR that has the update t the package manager file. We use [libraries.io](https://libraries.io/) as the source of information about libraries. You will need to get a free api key from [them](https://libraries.io/api) and set in the options.
 
 ### Manage PRs
 In addition, there are options to let you manage the PRs as you like, by setting a `branch_prefix`,  or disabling the creation of new branches with `disable_branch` (commits will be made on the current branch). You can also disable PR creation with `disable_pr` or force push commits to existing PR with `force_pr_creation`.
 
 ```yaml
-branch_prefix: Auto-Generated-Fixes
+branch_prefix: Auto-Generated-Dependency-Upgrades
 disable_branch: false
 disable_pr: false
 force_pr_creation: false
 ```
 
-### Scanner
-By default we use the open-source Semgrep scanner that comes with a community rule set for finding vulnerabilities. You can also do a `semgrep login` before running the AutoFix patchflow to get access to your own custom or pro rules if you have a Semgrep account (available for free).  In addition, you can use any SAST scanner that outputs results in the standard SARIF format. Just pass your scan results with the following:
-
-```yaml
-sarif_file_path: /path/to/your/sarif.json
-```
-
 ### Prompt template
 
-You can update the default [prompt template](./default_prompt.json). Note the use of variables `{{messageText}}` and `{{affectedCode}}`. They are generated by the steps within the AutoFix patchflow and replaced by the actual values during the execution. Also, remember to keep the output format as given in the default prompt as it is used to extract information that is used by the steps after the model response is processed.  The following output format is expected at the moment:
-```
-A. Commit message:
-<brief summary of the diff>
-
-B. Change summary:
-<description of the changes made in the diff>
-
-C. Compatibility Risk:
-<Low, Medium, High> 
-
-D. Fixed Code:
-<original code with the vulnerability now fixed>
-```
+You can update the default [prompt template](./dependency_upgrade_prompt.json). The basic prompt that upgrades the dependencies is with `"id": "depupgrade"`. Note the use of variables `{{Updates}}` and `{{PackageManagerFile}}`. They are generated by the steps within the DependencyUpgrade patchflow and replaced by the actual values during the execution. The expected output response is complete content of the package manager file with the libraries updated to their fixed versions.
 
 ## Examples
 
-Here are some example PRs generated with the AutoFix patchflow:
+Here are some example PRs generated with the DependencyUpgrade patchflow:
 
-- https://github.com/patched-codes/AltoroJ/pull/7
-- https://github.com/patched-codes/pygoat/pull/2
+- https://github.com/codelion/example-python/pull/32
+- https://github.com/codelion/example-java-maven/pull/3
```

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/default_prompt.json` & `patchwork_cli-0.0.7/patchwork/patchflows/AutoFix/default_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py` & `patchwork_cli-0.0.7/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import yaml
 
 from patchwork.step import Step
 from patchwork.steps import (
     AnalyzeImpact,
-    CallOpenAI,
+    CallLLM,
     CommitChanges,
     CreatePR,
     ExtractDiff,
     ExtractModelResponse,
     ExtractPackageManagerFile,
     ModifyCode,
     PreparePR,
@@ -72,38 +72,38 @@
                     if len(outputs) == 0:
                         continue
                     analyze_inputs.update(outputs)
                     analyze_inputs["prompt_id"] = "getimpact"
                     analyze_inputs["response_partitions"] = {"impacted_methods": ["A. Impacted methods:", ""]}
                     outputs = PreparePrompt(analyze_inputs).run()
                     analyze_inputs.update(outputs)
-                    outputs = CallOpenAI(analyze_inputs).run()
+                    outputs = CallLLM(analyze_inputs).run()
                     analyze_inputs.update(outputs)
                     outputs = ExtractModelResponse(analyze_inputs).run()
                     analyze_inputs.update(outputs)
 
                     # Do analysis on potential dependency upgrades and migrate the code as needed.
                     outputs = AnalyzeImpact(analyze_inputs).run()
                     analyze_inputs.update(outputs)
                     analyze_inputs["prompt_id"] = "migratecode"
                     analyze_inputs["response_partitions"] = {"patch": []}
                     outputs = PreparePrompt(analyze_inputs).run()
                     analyze_inputs.update(outputs)
-                    outputs = CallOpenAI(analyze_inputs).run()
+                    outputs = CallLLM(analyze_inputs).run()
                     analyze_inputs.update(outputs)
                     outputs = ExtractModelResponse(analyze_inputs).run()
                     analyze_inputs.update(outputs)
                     outputs = ModifyCode(analyze_inputs).run()
                     modified_files = modified_files + outputs["modified_code_files"]
 
             self.inputs["prompt_id"] = "depupgrade"
             self.inputs["response_partitions"] = {"patch": []}
             outputs = PreparePrompt(self.inputs).run()
             self.inputs.update(outputs)
-            outputs = CallOpenAI(self.inputs).run()
+            outputs = CallLLM(self.inputs).run()
             self.inputs.update(outputs)
             outputs = ExtractModelResponse(self.inputs).run()
             self.inputs.update(outputs)
             outputs = ModifyCode(self.inputs).run()
             self.inputs.update(outputs)
             self.inputs["modified_code_files"] = self.inputs["modified_code_files"] + modified_files
```

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/README.md` & `patchwork_cli-0.0.7/patchwork/patchflows/AutoFix/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# DependencyUpgrade
+# AutoFix
 
-The DependencyUpgrade patchflow aims to automatically update vulnerable versions of dependencies in your repository to the fixed version. 
+The AutoFix patchflow aims to automatically fix code vulnerabilities in your repository. 
 
 ## How to run?
  
 You can run it as follows:
 
-`patchwork DependencyUpgrade`
+`patchwork AutoFix`
 
 by default you will need to provide the `openai_api_key` and the `github_api_key` you can pass them as arguments: 
 
-`patchwork DependencyUpgrade openai_api_key=<Your_API_KEY> github_api_key=<Your_GH_Token>`
+`patchwork AutoFix openai_api_key=<Your_API_KEY> github_api_key=<Your_GH_Token>`
 
 ## What it does?
 
-The DependencyUpgrade patchflow will first scan your repository using an open-source scanner [dep-scan](https://github.com/owasp-dep-scan/dep-scan). It will then extract the vulnerable libraries information detected by the scan and use them to create a prompt to be sent to `gpt-3.5-turbo` to update your package manager file. You can check the default [prompt template](./dependency_upgrade_prompt.json). The fixed package manager file is then committed to the repository under a new branch and finally a pull request is created for the user to review and merge the changes. 
+The AutoFix patchflow will first scan the code in your repository using an open-source scanner Semgrep. It will then take the vulnerabilities that are detected by the scan and create a prompt to be sent to `gpt-3.5-turbo` to generate the fix for the vulnerabilities. You can check the default [prompt template](./default_prompt.json). The generated fixes are then committed to the repository under a new branch and finally a pull request is created for the user to review and merge the changes. 
 
 ## Configuration
 
-The following are the default configurations that can be modified by the user to adapt the DependencyUpgrade patchflow to their needs. All the options can be set both via CLI arguments and and the yaml config file.
+The following are the default configurations that can be modified by the user to adapt the AutoFix patchflow to their needs. All the options can be set both via CLI arguments and and the yaml config file.
 
 ### Model
 
 You can choose any LLM API as long as it has an OpenAI API compatible chat completions endpoint. Just update the default values of the following options:
 
 ```yaml
 - model: gpt-3.5-turbo
@@ -38,65 +38,106 @@
 model_top_p: 0.95
 model_max_tokens: 2000
 ```
 and pass your HuggingFace token in the `openai_api_key` option.
 
 You can also use llama.cpp to run inference on CPU locally. Just install the [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) package and run their OpenAI compatible web server as described [here](https://github.com/abetlen/llama-cpp-python) with the command:
 
-`python3 -m llama_cpp.server --hf_model_repo_id TheBloke/deepseek-coder-6.7B-instruct-GGUF --model 'deepseek-coder-6.7b-instruct.Q4_0.gguf'`
+`python3 -m llama_cpp.server --hf_model_repo_id TheBloke/deepseek-coder-6.7B-instruct-GGUF --model 'deepseek-coder-6.7b-instruct.Q4_K_M.gguf' --chat_format chatml`
 
 Once the local server is running you can set:
 
 ```yaml
 client_base_url: http://localhost:8000/v1
 model: TheBloke/deepseek-coder-6.7B-instruct-GGUF
 model_temperature: 0.2
 model_top_p: 0.95
 model_max_tokens: 1000
 ```
 and use the local model for inference.
 
-### Upgrade Threshold
-You can set the upgrade threshold you want to update the libraries to. The accepted values are 'major', 'minor' or  'patch'.
-E.g.
+### Context size
+By default we chunk the code to `context_size` tokens to pass on to the LLM. You can change the default value by setting:
+
+```yaml
+context_size: 1000
+```
+in general we have found that a larger `context_size `doesn't necessarily lead to better fixes.
+
+### Semgrep extra args
+You can pass any additional arguments to the Semgrep scanner using the `semgrep_extra_args` option as follows:
+
 ```yaml
-upgrade_threshold: minor
+semgrep_extra_args: --config auto
 ```
-would only upgrade across minor and patch versions of the library, i.e. an upgrade to another major wouldn't be done.
+
+### SARIF input
+We can use any SAST scanner that can export the results in SARIF format. Just set the `sarif_file_path` to the SARIF file and AutoFix will use the information there to generate the fixes. Otherwise, we will do a scan using Semgrep.
+
+```yaml
+sarif_file_path: /path/to/sarif/file
+```
+
+### Vulnerability limit
+By default we process and fix only `vulnerability_limit` number of issues. This is to avoid making large number of LLMs calls and to keep the generated PR manageable. You can set the value to your preference:
+
+```yaml
+vulnerability_limit: 10
+``` 
+set this value to a negative number (e.g. `-1`) to fix all vulnerabilities found in the scan.
 
 ### Severity
-You can also set the severity of the vulnerabilities that you want to upgrade. Severity is derived from the CVSS score and can take values of 'none', 'low', 'medium', 'high', and 'critical'. 
-E.g.
+You can also set the severity of the vulnerabilities that you want to fix. Severity is derived from the information available in the SARIF file and can take values of 'unknown', 'note'/'info', 'warning'/'low', 'medium', 'error'/'high', and 'critical'. E.g.
+
 ```yaml
 severity: medium
 ```
-means that all libraries that have medium and above vulnerabilities will be upgraded.
+means that all medium and above vulnerabilities will be fixed.
 
-### Analyze Impact
-By default we update the libraries to their fixed versions. If the upgrades are across major versions or a lot has changed between the versions of the library updating it may break your application. The `analyze_impact` option can be set to enable an impact analysis of the library upgrades as follows:
+### Compatibility
+You can also set the compatibility threshold of the suggested fixes to be included in the pull request. Compatibility can take values of 'unknown', 'low', 'medium', and 'high'. E.g.
 
 ```yaml
-analyze_impact: true
-libraries_api_key: <Your_API_KEY>
+compatibility: medium
 ```
-This will get the diff between the vulnerable and fixed versions of the library and determine the impacted methods. Then, we will analyze your repository to determine if you are using the impacted methods. And, finally we will use this information to prompt an LLM to migrate the code that uses these impacted methods in your repository. The code changes are then committed in a new branch in your repository to be included in the same PR that has the update t the package manager file. We use [libraries.io](https://libraries.io/) as the source of information about libraries. You will need to get a free api key from [them](https://libraries.io/api) and set in the options.
+means that all fixes with mediuam and above threshold will be included in the PR.
 
 ### Manage PRs
 In addition, there are options to let you manage the PRs as you like, by setting a `branch_prefix`,  or disabling the creation of new branches with `disable_branch` (commits will be made on the current branch). You can also disable PR creation with `disable_pr` or force push commits to existing PR with `force_pr_creation`.
 
 ```yaml
-branch_prefix: Auto-Generated-Dependency-Upgrades
+branch_prefix: Auto-Generated-Fixes
 disable_branch: false
 disable_pr: false
 force_pr_creation: false
 ```
 
+### Scanner
+By default we use the open-source Semgrep scanner that comes with a community rule set for finding vulnerabilities. You can also do a `semgrep login` before running the AutoFix patchflow to get access to your own custom or pro rules if you have a Semgrep account (available for free).  In addition, you can use any SAST scanner that outputs results in the standard SARIF format. Just pass your scan results with the following:
+
+```yaml
+sarif_file_path: /path/to/your/sarif.json
+```
+
 ### Prompt template
 
-You can update the default [prompt template](./dependency_upgrade_prompt.json). The basic prompt that upgrades the dependencies is with `"id": "depupgrade"`. Note the use of variables `{{Updates}}` and `{{PackageManagerFile}}`. They are generated by the steps within the DependencyUpgrade patchflow and replaced by the actual values during the execution. The expected output response is complete content of the package manager file with the libraries updated to their fixed versions.
+You can update the default [prompt template](./default_prompt.json). Note the use of variables `{{messageText}}` and `{{affectedCode}}`. They are generated by the steps within the AutoFix patchflow and replaced by the actual values during the execution. Also, remember to keep the output format as given in the default prompt as it is used to extract information that is used by the steps after the model response is processed.  The following output format is expected at the moment:
+```
+A. Commit message:
+<brief summary of the diff>
+
+B. Change summary:
+<description of the changes made in the diff>
+
+C. Compatibility Risk:
+<Low, Medium, High> 
+
+D. Fixed Code:
+<original code with the vulnerability now fixed>
+```
 
 ## Examples
 
-Here are some example PRs generated with the DependencyUpgrade patchflow:
+Here are some example PRs generated with the AutoFix patchflow:
 
-- https://github.com/codelion/example-python/pull/32
-- https://github.com/codelion/example-java-maven/pull/3
+- https://github.com/patched-codes/AltoroJ/pull/7
+- https://github.com/patched-codes/pygoat/pull/2
```

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/defaults.yml` & `patchwork_cli-0.0.7/patchwork/patchflows/GenerateREADME/defaults.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # PreparePrompt Inputs
 # prompt_template_file: your-prompt-template-here
 
-# CallOpenAI Inputs
-# openai_api_key: required
-model: gpt-3.5-turbo
-client_base_url: https://api.openai.com/v1
+# CallLLM Inputs
+# openai_api_key: required-for-chatgpt
+# google_api_key: required-for-gemini
+# model: gpt-3.5-turbo
+# client_base_url: https://api.openai.com/v1
 # Example HF model
 # client_base_url: https://api-inference.huggingface.co/models/codellama/CodeLlama-70b-Instruct-hf/v1
 # model: codellama/CodeLlama-70b-Instruct-hf
 # model_temperature: 0.2
 # model_top_p: 0.95
 # model_max_tokens: 2000
 
-# Do impact analysis after dependency upgrades to modify source code
-analyze_impact: false
-
 # CommitChanges Inputs
 disable_branch: false
 
 # CreatePR Inputs
 disable_pr: false
 force_pr_creation: false
 # github_api_key: required-for-github-scm
```

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json` & `patchwork_cli-0.0.7/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/GenerateREADME.py` & `patchwork_cli-0.0.7/patchwork/patchflows/GenerateREADME/GenerateREADME.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import yaml
 
 from patchwork.step import Step
 from patchwork.steps import (
     CallCode2Prompt,
-    CallOpenAI,
+    CallLLM,
     CommitChanges,
     CreatePR,
     ExtractModelResponse,
     ModifyCode,
     PreparePR,
     PreparePrompt,
 )
@@ -43,15 +43,15 @@
 
     def run(self) -> dict:
         outputs = CallCode2Prompt(self.inputs).run()
         self.inputs.update(outputs)
         self.inputs["response_partitions"] = {"patch": []}
         outputs = PreparePrompt(self.inputs).run()
         self.inputs.update(outputs)
-        outputs = CallOpenAI(self.inputs).run()
+        outputs = CallLLM(self.inputs).run()
         self.inputs.update(outputs)
         outputs = ExtractModelResponse(self.inputs).run()
         self.inputs.update(outputs)
         outputs = ModifyCode(self.inputs).run()
         self.inputs.update(outputs)
 
         number = len(self.inputs["modified_code_files"])
```

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/README.md` & `patchwork_cli-0.0.7/patchwork/patchflows/GenerateREADME/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 model_top_p: 0.95
 model_max_tokens: 2000
 ```
 and pass your HuggingFace token in the `openai_api_key` option.
 
 You can also use llama.cpp to run inference on CPU locally. Just install the [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) package and run their OpenAI compatible web server as described [here](https://github.com/abetlen/llama-cpp-python) with the command:
 
-`python3 -m llama_cpp.server --hf_model_repo_id TheBloke/deepseek-coder-6.7B-instruct-GGUF --model 'deepseek-coder-6.7b-instruct.Q4_0.gguf'`
+`python3 -m llama_cpp.server --hf_model_repo_id TheBloke/deepseek-coder-6.7B-instruct-GGUF --model 'deepseek-coder-6.7b-instruct.Q4_K_M.gguf' --chat_format chatml`
 
 Once the local server is running you can set:
 
 ```yaml
 client_base_url: http://localhost:8000/v1
 model: TheBloke/deepseek-coder-6.7B-instruct-GGUF
 model_temperature: 0.2
@@ -81,9 +81,9 @@
 
 You can update the default [prompt template](./generate_readme_prompt.json). Note the use of variable `{{fullContent}}`. It is generated by the steps within the GenerateREADME patchflow and replaced by the actual value during the execution. The expected output response is complete content of the README.md file with the documentation.
 
 ## Examples
 
 Here are some example PRs generated with the GenerateREADME patchflow:
 
-- https://github.com/patched-codes/patchwork/pull/162
-- https://github.com/patched-codes/patchwork/pull/161
+- https://github.com/patched-codes/patchwork/pull/53
+- https://github.com/patched-codes/patchwork/pull/52
```

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/PRReview/PRReview.py` & `patchwork_cli-0.0.7/patchwork/patchflows/PRReview/PRReview.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 
 import yaml
 
 from patchwork.step import Step
 from patchwork.steps import (
-    CallOpenAI,
+    CallLLM,
     CreatePRComment,
     ExtractModelResponse,
     PreparePR,
     PreparePrompt,
     ReadPRDiffs,
 )
 
@@ -59,15 +59,15 @@
         self.inputs["prompt_id"] = "diffreview"
         self.inputs["response_partitions"] = {
             "summary": ["A. Summary:", ""],
             "suggestion": ["B. Suggestion:", "A. Summary:"],
         }
         outputs = PreparePrompt(self.inputs).run()
         self.inputs.update(outputs)
-        outputs = CallOpenAI(self.inputs).run()
+        outputs = CallLLM(self.inputs).run()
         self.inputs.update(outputs)
         outputs = ExtractModelResponse(self.inputs).run()
         self.inputs.update(outputs)
 
         summaries = []
         for response, prompt_values in zip(self.inputs["extracted_responses"], self.inputs["prompt_values"]):
             summary = {}
@@ -83,15 +83,15 @@
         if self.verbosity > _SUMMARY_LEVEL[_SHORT]:
             filtered_summaries = [summary["commit_message"] for summary in summaries]
             self.inputs["prompt_id"] = "diffreview_summary"
             self.inputs["prompt_values"] = [{"diffreviews": "\n".join(filtered_summaries)}]
 
             outputs = PreparePrompt(self.inputs).run()
             self.inputs.update(outputs)
-            outputs = CallOpenAI(self.inputs).run()
+            outputs = CallLLM(self.inputs).run()
             self.inputs.update(outputs)
             header = self.inputs["openai_responses"][0]
 
         self.inputs["pr_header"] = header
         self.inputs["modified_code_files"] = summaries
         outputs = PreparePR(self.inputs).run()
         self.inputs.update(outputs)
```

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/PRReview/README.md` & `patchwork_cli-0.0.7/patchwork/patchflows/PRReview/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 model_top_p: 0.95
 model_max_tokens: 2000
 ```
 and pass your HuggingFace token in the `openai_api_key` option.
 
 You can also use llama.cpp to run inference on CPU locally. Just install the [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) package and run their OpenAI compatible web server as described [here](https://github.com/abetlen/llama-cpp-python) with the command:
 
-`python3 -m llama_cpp.server --hf_model_repo_id TheBloke/deepseek-coder-6.7B-instruct-GGUF --model 'deepseek-coder-6.7b-instruct.Q4_0.gguf'`
+`python3 -m llama_cpp.server --hf_model_repo_id TheBloke/deepseek-coder-6.7B-instruct-GGUF --model 'deepseek-coder-6.7b-instruct.Q4_K_M.gguf' --chat_format chatml`
 
 Once the local server is running you can set:
 
 ```yaml
 client_base_url: http://localhost:8000/v1
 model: TheBloke/deepseek-coder-6.7B-instruct-GGUF
 model_temperature: 0.2
@@ -84,9 +84,9 @@
 <summary of the diff>
 ```
 
 ## Examples
 
 Here are some example comments generated with the PRReview patchflow:
 
-- https://github.com/patched-codes/patchwork/pull/176#issuecomment-2032030464
-- https://github.com/patched-codes/patchwork/pull/80#issuecomment-2031400047
+- https://github.com/patched-codes/patchwork/pull/59#issuecomment-2092735385
+- https://github.com/patched-codes/patchwork/pull/56#issuecomment-2092584306
```

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/PRReview/defaults.yml` & `patchwork_cli-0.0.7/patchwork/patchflows/PRReview/defaults.yml`

 * *Files 15% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 # github_api_key: required-for-github-scm
 # gitlab_api_key: required-for-gitlab-scm
 # pr_url: required
 
 # PreparePrompt Inputs
 # prompt_template_file: your-prompt-template-here
 
-# CallOpenAI Inputs
-# openai_api_key: required
-model: gpt-3.5-turbo
-client_base_url: https://api.openai.com/v1
+# CallLLM Inputs
+# openai_api_key: required-for-chatgpt
+# google_api_key: required-for-gemini
+# model: gpt-3.5-turbo
+# client_base_url: https://api.openai.com/v1
 # Example HF model
 # client_base_url: https://api-inference.huggingface.co/models/codellama/CodeLlama-70b-Instruct-hf/v1
 # model: codellama/CodeLlama-70b-Instruct-hf
 # model_temperature: 0.2
 # model_top_p: 0.95
 # model_max_tokens: 2000
```

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/PRReview/pr_review_prompt.json` & `patchwork_cli-0.0.7/patchwork/patchflows/PRReview/pr_review_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/patchflows/README.md` & `patchwork_cli-0.0.7/patchwork/patchflows/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py` & `patchwork_cli-0.0.7/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import os
-import tempfile
 from pathlib import Path
 
+from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 _PURL_TO_LANGUAGE_ = {
     "pypi": "python",
     "npm": "javascript",
     "maven": "java",
@@ -142,13 +142,13 @@
                 previousCode=file_content,
                 methodInfoList="\n".join(method_infos),
             )
             extracted_data.append(data)
 
         # Save extracted data to JSON
 
-        output_file = Path(tempfile.mktemp(".json"))
-        with open(output_file, "w", encoding="utf-8") as f:
-            json.dump(extracted_data, f, indent=2)
+        with defered_temp_file("w", suffix=".json") as fp:
+            json.dump(extracted_data, fp)
+            output_file = Path(fp.name)
 
         logger.info(f"Run completed {self.__class__.__name__}")
         return dict(prompt_value_file=output_file, code_file=output_file)
```

### Comparing `patchwork_cli-0.0.6/patchwork/steps/AnalyzeImpact/README.md` & `patchwork_cli-0.0.7/patchwork/steps/AnalyzeImpact/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py` & `patchwork_cli-0.0.7/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 import subprocess
-import tempfile
 from pathlib import Path
 
+from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 FOLDER_PATH = "folder_path"
 
 
 class CallCode2Prompt(Step):
@@ -65,13 +65,13 @@
 
         data["uri"] = self.code_file_path
         data["startLine"] = 0
         data["endLine"] = len(lines)
 
         self.extracted_data.append(data)
 
-        output_file = Path(tempfile.mktemp(".json"))
-        with open(output_file, "w", encoding="utf-8") as f:
-            json.dump(self.extracted_data, f, indent=2)
+        with defered_temp_file("w", suffix=".json") as fp:
+            json.dump(self.extracted_data, fp, indent=2)
+            output_file = Path(fp.name)
 
         logger.info(f"Run completed {self.__class__.__name__}")
         return {"prompt_value_file": output_file, "code_file": output_file}
```

### Comparing `patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/README.md` & `patchwork_cli-0.0.7/patchwork/steps/CallCode2Prompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py` & `patchwork_cli-0.0.7/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/CommitChanges/CommitChanges.py` & `patchwork_cli-0.0.7/patchwork/steps/CommitChanges/CommitChanges.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/CommitChanges/README.md` & `patchwork_cli-0.0.7/patchwork/steps/CommitChanges/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/CreatePR/CreatePR.py` & `patchwork_cli-0.0.7/patchwork/steps/CreatePR/CreatePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/CreatePR/README.md` & `patchwork_cli-0.0.7/patchwork/steps/CreatePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/CreatePRComment/CreatePRComment.py` & `patchwork_cli-0.0.7/patchwork/steps/CreatePRComment/CreatePRComment.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/CreatePRComment/README.md` & `patchwork_cli-0.0.7/patchwork/steps/CreatePRComment/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/ExtractCode.py` & `patchwork_cli-0.0.7/patchwork/steps/ExtractCode/ExtractCode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import json
 import os
 import sys
-import tempfile
 from collections import defaultdict
 from enum import IntEnum
 from pathlib import Path
 from typing import Any
 from urllib.parse import urlparse
 
-import tiktoken
-
+from patchwork.common.utils import (
+    count_openai_tokens,
+    defered_temp_file,
+    open_with_chardet,
+)
 from patchwork.logger import logger
 from patchwork.step import Step
-
-from ...common.utils import open_with_chardet
-from .context_strategy.context_strategies import ContextStrategies
-
-_ENCODING = tiktoken.get_encoding("cl100k_base")
-
-
-def count_tokens(code: str):
-    return len(_ENCODING.encode(code))
+from patchwork.steps.ExtractCode.context_strategy.context_strategies import (
+    ContextStrategies,
+)
 
 
 def get_source_code_context(
     uri: str, source_lines: list[str], start_line: int, end_line: int, context_token_length: int
 ) -> tuple[int | None, int | None]:
     context_strategies = ContextStrategies.get_context_strategies(*ContextStrategies.ALL)
     context_strategies = [strategy for strategy in context_strategies if strategy.is_file_supported(uri, source_lines)]
@@ -32,15 +28,15 @@
         context_start, context_end = context_strategy.get_context_indexes(source_lines, start_line, end_line)
         if context_start is None or context_end is None:
             logger.info(f'Context Strategy: "{context_strategy.__class__.__name__}" failed to return context')
             continue
 
         logger.info(f'"{context_strategy.__class__.__name__}" Context Strategy used: {context_start}, {context_end}')
         context = "".join(source_lines[context_start:context_end])
-        if count_tokens(context) <= context_token_length:
+        if count_openai_tokens(context) <= context_token_length:
             return context_start, context_end
 
     return None, None
 
 
 def parse_sarif_location(base_path: Path, location_str: str) -> Path | None:
     uri = urlparse(location_str)
@@ -242,15 +238,15 @@
                 if source_code_context is None:
                     logger.info(f"No context found for {file_path} at {start_line}:{end_line}")
                     continue
 
                 start = context_start if context_start is not None else start_line
                 end = context_end if context_end is not None else end_line
 
-                grouped_messages[(uri, start, end, source_code_context)].append(
+                grouped_messages[(file_path, start, end, source_code_context)].append(
                     result.get("message", {}).get("text", "")
                 )
 
                 vulnerability_count = vulnerability_count + 1
                 if 0 < vulnerability_limit <= vulnerability_count:
                     return grouped_messages
 
@@ -298,17 +294,17 @@
                 "affectedCode": context,
                 "messageText": "\n".join(msgs),
             }
             for (file_path, start, end, context), msgs in grouped_messages.items()
         ]
 
         # Save extracted data to JSON
-        output_file = Path(tempfile.mktemp(".json"))
-        with open(output_file, "w", encoding="utf-8") as f:
-            json.dump(self.extracted_code_contexts, f, indent=2)
+        with defered_temp_file("w", suffix=".json") as fp:
+            json.dump(self.extracted_code_contexts, fp, indent=2)
+            output_file = Path(fp.name)
 
         logger.info(f"Run completed {self.__class__.__name__}")
 
         return dict(
             code_file=output_file,
             prompt_values=self.extracted_code_contexts,
         )
```

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/README.md` & `patchwork_cli-0.0.7/patchwork/steps/ExtractCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/context_strategies.py` & `patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/context_strategies.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/generic.py` & `patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/generic.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/java.py` & `patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/java.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/javascript.py` & `patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/javascript.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/python.py` & `patchwork_cli-0.0.7/patchwork/steps/ExtractCode/context_strategy/python.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractDiff/ExtractDiff.py` & `patchwork_cli-0.0.7/patchwork/steps/ExtractDiff/ExtractDiff.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import os
 import re
 import string
-import tempfile
 from pathlib import Path
 from typing import Dict, List
 
 import requests
 from packageurl import PackageURL
 
+from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 _PURL_TO_LANGUAGE_ = {
     "pypi": "python",
     "npm": "javascript",
     "maven": "java",
@@ -208,30 +208,30 @@
 
         temp_file_path = None
 
         for vuln_version, fixed_version in generate_version_combinations(vuln_version, fixed_version):
             diff_file = requests.get(compare_url + vuln_version + "..." + fixed_version, headers=headers)
 
             if diff_file.text.startswith("diff"):
-                temp_file_path = tempfile.mktemp()
-                with open(temp_file_path, "w") as file:
-                    file.write(diff_file.text)
+                with defered_temp_file("w") as fp:
+                    fp.write(diff_file.text)
+                    temp_file_path = Path(fp.name)
 
         if temp_file_path is None:
             logger.info(
                 f"Unable to generate diff for the repo {compare_url} between versions {vuln_version} and {fixed_version}"
             )
             return {}
 
         diff_sections = get_diff_sections(temp_file_path, _PURL_TO_LANGUAGE_.get(platform_type))
         extracted_data = []
 
         for diff_section in diff_sections:
             extracted_data.append({"diffSection": diff_section})
 
         # Save extracted data to JSON
-        output_file = Path(tempfile.mktemp(".json"))
-        with open(output_file, "w", encoding="utf-8") as f:
-            json.dump(extracted_data, f, indent=2)
+        with defered_temp_file("w", suffix=".json") as fp:
+            json.dump(extracted_data, fp, indent=2)
+            output_file = Path(fp.name)
 
         logger.info(f"Run completed {self.__class__.__name__}")
         return dict(prompt_value_file=output_file, library_name=name, platform_type=platform_type)
```

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractDiff/README.md` & `patchwork_cli-0.0.7/patchwork/steps/ExtractDiff/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py` & `patchwork_cli-0.0.7/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractModelResponse/README.md` & `patchwork_cli-0.0.7/patchwork/steps/ExtractModelResponse/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py` & `patchwork_cli-0.0.7/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 import os
 import re
-import tempfile
 from collections import defaultdict
 from pathlib import Path
 
 import semver
 from packageurl import PackageURL
 
+from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 # Define a mapping from CVSS severity level strings to numbers
 SEVERITY_LEVELS = {"none": 0, "low": 1, "medium": 2, "high": 3, "critical": 4}
 
 
@@ -269,14 +269,13 @@
             data["UpdateMsg"] = update_msg
             data["uri"] = src_file
             data["startLine"] = 0
             data["endLine"] = len(lines)
             self.extracted_data.append(data)
 
         # Save extracted data to JSON
-
-        output_file = Path(tempfile.mktemp(".json"))
-        with open(output_file, "w", encoding="utf-8") as f:
-            json.dump(self.extracted_data, f, indent=2)
+        with defered_temp_file("w", suffix=".json") as fp:
+            json.dump(self.extracted_data, fp, indent=2)
+            output_file = Path(fp.name)
 
         logger.info(f"Run completed {self.__class__.__name__}")
         return dict(prompt_value_file=output_file, code_file=output_file)
```

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/README.md` & `patchwork_cli-0.0.7/patchwork/steps/ExtractPackageManagerFile/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py` & `patchwork_cli-0.0.7/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ModifyCode/ModifyCode.py` & `patchwork_cli-0.0.7/patchwork/steps/ModifyCode/ModifyCode.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ModifyCode/README.md` & `patchwork_cli-0.0.7/patchwork/steps/ModifyCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/PreparePR/PreparePR.py` & `patchwork_cli-0.0.7/patchwork/steps/PreparePR/PreparePR.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
 
         if not all(key in inputs.keys() for key in self.required_keys):
             raise ValueError(f'Missing required data: "{self.required_keys}"')
 
         if len(inputs["modified_code_files"]) < 1:
-            logger.warn("No modified files to prepare a PR for.")
+            logger.warning("No modified files to prepare a PR for.")
         self.modified_code_files = inputs["modified_code_files"]
 
         self.header = f"This pull request from patched fixes {len(self.modified_code_files)} issues."
         if "pr_header" in inputs.keys():
             self.header = inputs["pr_header"]
 
     def run(self) -> dict:
```

### Comparing `patchwork_cli-0.0.6/patchwork/steps/PreparePR/README.md` & `patchwork_cli-0.0.7/patchwork/steps/PreparePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/PreparePrompt/PreparePrompt.py` & `patchwork_cli-0.0.7/patchwork/steps/PreparePrompt/PreparePrompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
-import tempfile
 from pathlib import Path
 
+from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 PROMPT_TEMPLATE_FILE_KEY = "prompt_template_file"
 
 
 class PreparePrompt(Step):
-    required_keys = {("%s" % PROMPT_TEMPLATE_FILE_KEY), "prompt_id"}
+    required_keys = {PROMPT_TEMPLATE_FILE_KEY, "prompt_id"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
 
         if not all(key in inputs.keys() for key in self.required_keys):
             raise ValueError(f'Missing required data: "{self.required_keys}"')
 
@@ -63,13 +63,13 @@
                     new_value = value
                     for replacement_key, replacement_value in prompt_value.items():
                         new_value = new_value.replace("{{" + replacement_key + "}}", str(replacement_value))
                     prompt_instance[key] = new_value
                 prompt.append(prompt_instance)
             prompts.append(prompt)
 
-        prompt_file = Path(tempfile.mktemp(".json"))
-        with open(prompt_file, "w") as file:
-            json.dump(prompts, file, indent=2)
+        with defered_temp_file("w", suffix=".json") as fp:
+            json.dump(prompts, fp, indent=2)
+            prompt_file = Path(fp.name)
 
         logger.info(f"Run completed {self.__class__.__name__}")
         return {"prompt_file": prompt_file}
```

### Comparing `patchwork_cli-0.0.6/patchwork/steps/PreparePrompt/README.md` & `patchwork_cli-0.0.7/patchwork/steps/PreparePrompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/README.md` & `patchwork_cli-0.0.7/patchwork/steps/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ReadPRDiffs/README.md` & `patchwork_cli-0.0.7/patchwork/steps/ReadPRDiffs/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py` & `patchwork_cli-0.0.7/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
-import tempfile
+from pathlib import Path
 
 from patchwork.common.client.scm import GithubClient, GitlabClient
+from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 _IGNORED_EXTENSIONS = [
     ".png",
     ".jpg",
     ".jpeg",
@@ -50,11 +51,12 @@
     def run(self) -> dict:
         prompt_values = []
         for path, diffs in self.pr.file_diffs().items():
             if filter_by_extension(path, _IGNORED_EXTENSIONS):
                 continue
             prompt_values.append(dict(path=path, diff=diffs))
 
-        prompt_value_file = tempfile.mktemp(".json")
-        with open(prompt_value_file, "w") as fp:
+        with defered_temp_file("w", suffix=".json") as fp:
             json.dump(prompt_values, fp)
+            prompt_value_file = Path(fp.name)
+
         return dict(prompt_value_file=prompt_value_file, prompt_values=prompt_values)
```

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/README.md` & `patchwork_cli-0.0.7/patchwork/steps/ScanDepscan/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/ScanDepscan.py` & `patchwork_cli-0.0.7/patchwork/steps/ScanDepscan/ScanDepscan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import atexit
 import os
+import shutil
 import subprocess
 import tempfile
+from pathlib import Path
 
 from patchwork.logger import logger
 from patchwork.step import Step
 
 
 def is_cdxgen_installed():
     """Check if cdxgen is installed."""
@@ -81,20 +84,21 @@
         - This method assumes that 'depscan' is installed and accessible in the system's PATH.
         - The generated temporary directory path is based on a temporary file path and is manipulated to be a directory path;
         however, the directory itself is not automatically created by this method.
         - The caller is responsible for ensuring that the 'depscan' tool can run successfully and that the specified
         temporary directory exists and is writable.
         """
         # Generate a unique temporary file path
-        temp_file_path = tempfile.mktemp()
+        temp_file_path = Path(tempfile.mkdtemp())
+        atexit.register(shutil.rmtree, temp_file_path, ignore_errors=True)
 
         cmd = [
             "depscan",
             "--reports-dir",
-            temp_file_path,
+            str(temp_file_path),
         ]
 
         if self.language is not None:
             cmd.append("-t")
             cmd.append(self.language)
             sbom_vdr_file_name = "sbom-" + self.language
         else:
```

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ScanSemgrep/README.md` & `patchwork_cli-0.0.7/patchwork/steps/ScanSemgrep/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.6/patchwork/steps/ScanSemgrep/ScanSemgrep.py` & `patchwork_cli-0.0.7/patchwork/steps/ScanSemgrep/ScanSemgrep.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 import subprocess
-import tempfile
 from pathlib import Path
 
+from patchwork.common.utils import defered_temp_file
 from patchwork.logger import logger
 from patchwork.step import Step
 
 
 class ScanSemgrep(Step):
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
+        self.extra_args = inputs.get("semgrep_extra_args", "")
         self.enabled = "sarif_file_path" not in inputs.keys()
 
     def run(self) -> dict:
         if not self.enabled:
             logger.info(f"Run skipped {self.__class__.__name__} because sarif_file_path is already present in inputs")
             return dict()
 
         cwd = Path.cwd()
-        sarif_file_path = Path(tempfile.mktemp(".sarif"))
 
         cmd = [
             "semgrep",
-            "--config",
-            "auto",
-            "--config",
-            "p/python",
+            *self.extra_args.split(),
             str(cwd),
             "--sarif",
         ]
 
         p = subprocess.run(cmd, capture_output=True, text=True)
 
-        with open(sarif_file_path, "w") as file:
-            file.write(p.stdout)
+        with defered_temp_file("w", suffix=".sarif") as fp:
+            fp.write(p.stdout)
+            sarif_file_path = Path(fp.name)
 
         logger.info(f"Run completed {self.__class__.__name__}")
         return {"sarif_file_path": sarif_file_path}
```

### Comparing `patchwork_cli-0.0.6/patchwork/steps/__init__.py` & `patchwork_cli-0.0.7/patchwork/steps/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 from patchwork.steps.AnalyzeImpact.AnalyzeImpact import AnalyzeImpact
 from patchwork.steps.CallCode2Prompt.CallCode2Prompt import CallCode2Prompt
-from patchwork.steps.CallOpenAI.CallOpenAI import CallOpenAI
+from patchwork.steps.CallLLM.CallLLM import CallLLM
 from patchwork.steps.CommitChanges.CommitChanges import CommitChanges
+from patchwork.steps.CreateIssueComment.CreateIssueComment import CreateIssueComment
 from patchwork.steps.CreatePR.CreatePR import CreatePR
 from patchwork.steps.CreatePRComment.CreatePRComment import CreatePRComment
 from patchwork.steps.ExtractCode.ExtractCode import ExtractCode
 from patchwork.steps.ExtractDiff.ExtractDiff import ExtractDiff
 from patchwork.steps.ExtractModelResponse.ExtractModelResponse import (
     ExtractModelResponse,
 )
 from patchwork.steps.ExtractPackageManagerFile.ExtractPackageManagerFile import (
     ExtractPackageManagerFile,
 )
+from patchwork.steps.GenerateCodeRepositoryEmbeddings.GenerateCodeRepositoryEmbeddings import (
+    GenerateCodeRepositoryEmbeddings,
+)
+from patchwork.steps.GenerateEmbeddings.GenerateEmbeddings import GenerateEmbeddings
 from patchwork.steps.ModifyCode.ModifyCode import ModifyCode
 from patchwork.steps.PreparePR.PreparePR import PreparePR
 from patchwork.steps.PreparePrompt.PreparePrompt import PreparePrompt
+from patchwork.steps.QueryEmbeddings.QueryEmbeddings import QueryEmbeddings
+from patchwork.steps.ReadIssues.ReadIssues import ReadIssues
 from patchwork.steps.ReadPRDiffs.ReadPRDiffs import ReadPRDiffs
 from patchwork.steps.ScanDepscan.ScanDepscan import ScanDepscan
 from patchwork.steps.ScanSemgrep.ScanSemgrep import ScanSemgrep
 
 __all__ = [
     "AnalyzeImpact",
     "CallCode2Prompt",
-    "CallOpenAI",
+    "CallLLM",
     "CommitChanges",
     "CreatePR",
     "CreatePRComment",
+    "CreateIssueComment",
     "ExtractCode",
     "ExtractDiff",
     "ExtractModelResponse",
     "ExtractPackageManagerFile",
+    "GenerateCodeRepositoryEmbeddings",
+    "GenerateEmbeddings",
     "ModifyCode",
     "PreparePR",
     "PreparePrompt",
+    "QueryEmbeddings",
+    "ReadIssues",
     "ReadPRDiffs",
     "ScanDepscan",
     "ScanSemgrep",
 ]
```

### Comparing `patchwork_cli-0.0.6/pyproject.toml` & `patchwork_cli-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patchwork-cli"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["patched.codes"]
 license = "AGPL"
 readme = "README.md"
 packages = [
     { include = "patchwork", from = "." }
 ]
@@ -19,67 +19,72 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10, <3.12"
+python = "^3.10"
 click = "~8.1.0"
-pygithub = "~2.1.1"
-gitpython = "~3.1.40"
 semgrep = "^1.51.0"
-pydantic = "^2.6.4"
 openai = "^1.13.3"
 tree-sitter-languages = "^1.10.2"
-tiktoken = "~0.5.2"
-libcst = "~1.2.0"
 python-gitlab = "^4.4.0"
-owasp-depscan = "^5.2.12"
+owasp-depscan = "~5.2.12"
+pygithub = "~2.1.1"
+gitpython = "~3.1.40"
+pydantic = "~2.6.4"
+tiktoken = "~0.6.0"
+libcst = "~1.2.0"
 patched-code2prompt = "0.2.0"
 pyyaml = "^6.0.1"
 packageurl-python = "~0.15.0"
 semver = "~3.0.2"
 requests = "~2.31.0"
 chardet = "^5.2.0"
-# TODO: bump this to at least 0.2.5 when it's released to fix python version dependency resolution issues
-open-interpreter = "~0.2.4"
+chromadb = "~0.4.24"
+sentence-transformers = "~2.7.0"
 # pinning transitive dependencies
 orjson = "~3.9.15"
+torch = "~2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "*"
 poethepoet = { version = "^0.24.2", extras = ["poetry-plugin"] }
 mypy = "^1.7.1"
 types-requests = "~2.31.0"
 black = "^23.12.0"
 isort = "^5.13.2"
 autoflake = "^2.3.1"
 pytest = "^8.1.1"
+pytest-mock = "^3.8.0"
+
+datasets = "^1.14.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 patchwork = 'patchwork.app:cli'
 
 [tool.poe.poetry_hooks]
 #pre_build = "mypy"
 post_update = "lint"
 
 [tool.poe.env]
 PROJ_PATH.default = "patchwork"
+TEST_PATH.default = "tests"
 
 [tool.poe.tasks]
 #mypy = "mypy ${PROJ_PATH}"
 lint = [
-    {cmd = "autoflake --recursive ${PROJ_PATH}"},
-    {cmd = "isort ${PROJ_PATH}"},
-    {cmd = "black ${PROJ_PATH}"}
+    {cmd = "autoflake --recursive ${PROJ_PATH} ${TEST_PATH}"},
+    {cmd = "isort ${PROJ_PATH} ${TEST_PATH}"},
+    {cmd = "black ${PROJ_PATH} ${TEST_PATH}"}
 ]
 
 [tool.black]
 target-version = ['py310']
 line-length = 120
 
 [tool.isort]
```

### Comparing `patchwork_cli-0.0.6/PKG-INFO` & `patchwork_cli-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 Metadata-Version: 2.1
 Name: patchwork-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 License: AGPL
 Author: patched.codes
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
+Requires-Dist: chromadb (>=0.4.24,<0.5.0)
 Requires-Dist: click (>=8.1.0,<8.2.0)
 Requires-Dist: gitpython (>=3.1.40,<3.2.0)
 Requires-Dist: libcst (>=1.2.0,<1.3.0)
-Requires-Dist: open-interpreter (>=0.2.4,<0.3.0)
 Requires-Dist: openai (>=1.13.3,<2.0.0)
 Requires-Dist: orjson (>=3.9.15,<3.10.0)
-Requires-Dist: owasp-depscan (>=5.2.12,<6.0.0)
+Requires-Dist: owasp-depscan (>=5.2.12,<5.3.0)
 Requires-Dist: packageurl-python (>=0.15.0,<0.16.0)
 Requires-Dist: patched-code2prompt (==0.2.0)
-Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydantic (>=2.6.4,<2.7.0)
 Requires-Dist: pygithub (>=2.1.1,<2.2.0)
 Requires-Dist: python-gitlab (>=4.4.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<2.32.0)
 Requires-Dist: semgrep (>=1.51.0,<2.0.0)
 Requires-Dist: semver (>=3.0.2,<3.1.0)
-Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
+Requires-Dist: sentence-transformers (>=2.7.0,<2.8.0)
+Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
+Requires-Dist: torch (>=2.2.2,<2.3.0)
 Requires-Dist: tree-sitter-languages (>=1.10.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://github.com/patched-codes/patchwork/assets/126385808/a7adcf24-b615-43a0-a244-45789d184f0a" width="160" alt="PatchWork Logo">
 </p>
 
 # PatchWork
 
-An open-source framework for patching and managing code repositories using large language models. PatchWork allows you to automate workflows like PR reviews, bug fixing, security patching, and more using a self-hosted CLI agent and your preferred LLMs.
+An open-source framework for automating development chores using large language models. PatchWork allows you to automate workflows like PR reviews, bug fixing, security patching, and more using a self-hosted CLI agent and your preferred LLMs.
 
 ## Key Components
 
 - **Steps**: A set of reusable atomic actions that define various operations.
 - **Patchflows**: LLM-assisted automations such as PR reviews, code fixing, debugging.
 
 Patchflows can be run locally in your CLI and IDE, or as part of your CI/CD pipeline.
@@ -110,121 +113,61 @@
 
 ```bash
 patchwork AutoFix openai_api_key=<YOUR_OPENAI_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
 The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities.
 
-You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
-
-The [patchwork-configs](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
+You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. You will need to pass your own `openai_api_key` to call the LLM. Otherwise, to get started, you can get a `patched_api_key` for free by
+by signing in at [https://app.patched.codes/signin](https://app.patched.codes/signin) and generating an API key from the integrations tab. You can then call the patchflow with the key as follows:
 
 ```bash
-patchwork AutoFix --config /path/to/patchwork-configs/patchflows
-```
-
-## PatchWork in CI
-
-You can also run PatchWork in a CI environment with ease:
-
-### Jenkins CI
-
-```groovy
-pipeline {
-  agent any
-    stages {
-      stage('Auto Fix Vulnerabilities') {
-        steps {
-          sh 'pip3 install patchwork'
-          sh 'patchwork AutoFix'
-      }
-    }
-  }
-}
-```
-
-### GitHub Actions
-
-- **Workflow**
-```yaml
-name: Auto Fix Vulnerabilities
-
-on:
-  # Patch files in PRs (diff-aware scanning):
-  pull_request: {}
-  # Patch on-demand through GitHub Actions interface:
-  workflow_dispatch: {}
-
-jobs:
-  patchwork:
-    # User definable name of this GitHub Actions job.
-    name: patchwork/ci
-    runs-on: ubuntu-latest
-
-    container:
-      # A Docker image with patchwork installed. Do not change this.
-      image: patched-codes/patchwork
-
-    steps:
-      # Fetch project source with GitHub Actions Checkout.
-      - uses: actions/checkout@v3
-      # Run the "patchwork" command on the command line of the docker image.
-      - run: patchwork AutoFix
+patchwork AutoFix patched_api_key=<YOUR_PATCHED_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
-- **Action (Available on Github Marketplace)**
-
-```yaml
-- name: Auto Fix Vulnerabilities
-  uses: patchwork/AutoFix@main
-```
-
-### Gitlab CI
-
-```yaml
-patchwork:
-  # A Docker image with PatchWork installed.
-  image: patched-codes/patchwork
-  # Run "patchwork" command on the command line of the docker image.
-  script: patchwork AutoFix
-
-  rules:
-  # Patch changed files in MRs, (diff-aware patching):
-  - if: $CI_MERGE_REQUEST_IID
+The [patchwork-configs](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
 
-  # Patch mainline (default) branches and fix all findings.
-  - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
+```bash
+patchwork AutoFix --config /path/to/patchwork-configs/patchflows
 ```
 
 ## Patchflows
 
 Patchwork comes with a set of predefined patchflows, and more will be added over time. Below is a sample list of patchflows:
 
 - AutoFix: Generate and apply fixes to code vulnerabilities in a repository.
 - DependencyUpgrade: Update your dependencies from vulnerable to fixed versions.
 - PRReview: On PR creation, extract code diff, summarize changes, and comment on PR.
 - GenerateREADME: Create a README.md file for a given folder, to add documentation to your repository.
+- ResolveIssue: Identify the files in your repository that need to be updated to resolve an issue (or bug) and create a PR to fix it.
 
 ## Prompt Templates
 
 Prompt templates are used by patchflows and passed as queries to LLMs. Templates contain prompts with placeholder variables enclosed by {{}} which are replaced by the data from the steps or inputs on every run. 
 
 Below is a sample prompt template:
 
 ```json
 {
-    "id": "ReviewPR",
+  "id": "diffreview_summary",
     "prompts": [
-        {"role": "system", "content": "You are a helpful assistant."},
-        {"role": "user", "content": "Create a well-structured message for the pull request body based on a review of the code diff. CODE DIFF - {{prDiff}}"}
+      {
+        "role": "user",
+        "content": "Summarize the following code change descriptions in 1 paragraph. {{diffreviews}}"
+      }
     ]
 }
 ```
 
 Each patchflow comes with an optimized default prompt template. But you can specify your own using the `prompt_template_file=/path/to/prompt/template/file` option. 
 
 ## Contributing
 
 To create a new patchflow, follow [these instructions](patchwork/patchflows/README.md).
 
 To create a new step, follow [these instructions](patchwork/steps/README.md).
 
+We also provide chat assitants to help you create new steps and patchflows easily.
+
+- [Patchwork Assistant GPT](https://chatgpt.com/g/g-0G4sCAd2y-patchwork-assistant) (requires ChatGPT pro subscription)
+- [Patchwork Assistant on HuggingChat ](https://hf.co/chat/assistant/66322701fd4787e0c1f7696b) (free)
+
```

