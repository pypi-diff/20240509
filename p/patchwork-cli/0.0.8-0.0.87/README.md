# Comparing `tmp/patchwork_cli-0.0.8.tar.gz` & `tmp/patchwork_cli-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchwork_cli-0.0.8.tar", max compression
+gzip compressed data, was "patchwork_cli-0.0.87.tar", max compression
```

## Comparing `patchwork_cli-0.0.8.tar` & `patchwork_cli-0.0.87.tar`

### file list

```diff
@@ -1,132 +1,132 @@
--rw-r--r--   0        0        0    34523 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/LICENSE
--rw-r--r--   0        0        0     6380 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/__main__.py
--rw-r--r--   0        0        0     5253 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/app.py
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/common/client/__init__.py
--rw-r--r--   0        0        0    15540 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/common/client/scm.py
--rw-r--r--   0        0        0     3945 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/common/utils.py
--rw-r--r--   0        0        0     1546 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/logger.py
--rw-r--r--   0        0        0      168 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/managed_files.py
--rw-r--r--   0        0        0     3718 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/AutoFix/AutoFix.py
--rw-r--r--   0        0        0     6059 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/AutoFix/README.md
--rw-r--r--   0        0        0     2182 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/AutoFix/default_prompt.json
--rw-r--r--   0        0        0      919 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/AutoFix/defaults.yml
--rw-r--r--   0        0        0     5422 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
--rw-r--r--   0        0        0     5441 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/DependencyUpgrade/README.md
--rw-r--r--   0        0        0      754 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/DependencyUpgrade/defaults.yml
--rw-r--r--   0        0        0     2495 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
--rw-r--r--   0        0        0     2204 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/GenerateREADME/GenerateREADME.py
--rw-r--r--   0        0        0     3855 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/GenerateREADME/README.md
--rw-r--r--   0        0        0      662 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/GenerateREADME/defaults.yml
--rw-r--r--   0        0        0      484 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
--rw-r--r--   0        0        0     3542 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/PRReview/PRReview.py
--rw-r--r--   0        0        0     3653 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/PRReview/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/PRReview/__init__.py
--rw-r--r--   0        0        0      659 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/PRReview/defaults.yml
--rw-r--r--   0        0        0      557 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/PRReview/pr_review_prompt.json
--rw-r--r--   0        0        0     2163 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/README.md
--rw-r--r--   0        0        0     3773 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/ResolveIssue/README.md
--rw-r--r--   0        0        0     3819 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/ResolveIssue/ResolveIssue.py
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/ResolveIssue/__init__.py
--rw-r--r--   0        0        0      714 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/ResolveIssue/defaults.yml
--rw-r--r--   0        0        0      728 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/ResolveIssue/prompt.json
--rw-r--r--   0        0        0      344 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/patchflows/__init__.py
--rw-r--r--   0        0        0      499 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/step.py
--rw-r--r--   0        0        0     5984 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
--rw-r--r--   0        0        0     1205 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/AnalyzeImpact/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/AnalyzeImpact/__init__.py
--rw-r--r--   0        0        0      501 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/AnalyzeImpact/typed.py
--rw-r--r--   0        0        0     2461 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
--rw-r--r--   0        0        0      967 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CallCode2Prompt/README.md
--rw-r--r--   0        0        0      575 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CallCode2Prompt/__init__.py
--rw-r--r--   0        0        0      303 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CallCode2Prompt/typed.py
--rw-r--r--   0        0        0     7462 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CallLLM/CallLLM.py
--rw-r--r--   0        0        0      503 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CallLLM/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CallLLM/__init__.py
--rw-r--r--   0        0        0      453 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CallLLM/typed.py
--rw-r--r--   0        0        0     5255 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CommitChanges/CommitChanges.py
--rw-r--r--   0        0        0     1106 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CommitChanges/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CommitChanges/__init__.py
--rw-r--r--   0        0        0      368 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CommitChanges/typed.py
--rw-r--r--   0        0        0     1346 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreateIssueComment/CreateIssueComment.py
--rw-r--r--   0        0        0      541 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreateIssueComment/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreateIssueComment/__init__.py
--rw-r--r--   0        0        0      320 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreateIssueComment/typed.py
--rw-r--r--   0        0        0     3907 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreatePR/CreatePR.py
--rw-r--r--   0        0        0     1279 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreatePR/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreatePR/__init__.py
--rw-r--r--   0        0        0      437 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreatePR/typed.py
--rw-r--r--   0        0        0     1358 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreatePRComment/CreatePRComment.py
--rw-r--r--   0        0        0      621 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreatePRComment/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.216580 patchwork_cli-0.0.8/patchwork/steps/CreatePRComment/__init__.py
--rw-r--r--   0        0        0      326 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/CreatePRComment/typed.py
--rw-r--r--   0        0        0    11511 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/ExtractCode.py
--rw-r--r--   0        0        0      755 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/__init__.py
--rw-r--r--   0        0        0     2585 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
--rw-r--r--   0        0        0      593 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/generic.py
--rw-r--r--   0        0        0     1491 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/java.py
--rw-r--r--   0        0        0     2442 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/javascript.py
--rw-r--r--   0        0        0      281 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/protocol.py
--rw-r--r--   0        0        0     2885 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/python.py
--rw-r--r--   0        0        0      463 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractCode/typed.py
--rw-r--r--   0        0        0     8722 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractDiff/ExtractDiff.py
--rw-r--r--   0        0        0      833 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractDiff/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractDiff/__init__.py
--rw-r--r--   0        0        0      404 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractDiff/typed.py
--rw-r--r--   0        0        0     1648 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
--rw-r--r--   0        0        0     1318 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractModelResponse/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractModelResponse/__init__.py
--rw-r--r--   0        0        0      301 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractModelResponse/typed.py
--rw-r--r--   0        0        0    12415 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
--rw-r--r--   0        0        0     1765 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractPackageManagerFile/README.md
--rw-r--r--   0        0        0     6173 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractPackageManagerFile/__init__.py
--rw-r--r--   0        0        0      338 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ExtractPackageManagerFile/typed.py
--rw-r--r--   0        0        0     5337 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/GenerateCodeRepositoryEmbeddings/GenerateCodeRepositoryEmbeddings.py
--rw-r--r--   0        0        0     1572 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/GenerateCodeRepositoryEmbeddings/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/GenerateCodeRepositoryEmbeddings/__init__.py
--rw-r--r--   0        0        0      211 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/GenerateCodeRepositoryEmbeddings/typed.py
--rw-r--r--   0        0        0     2941 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/GenerateEmbeddings/GenerateEmbeddings.py
--rw-r--r--   0        0        0     1011 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/GenerateEmbeddings/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/GenerateEmbeddings/__init__.py
--rw-r--r--   0        0        0      238 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/GenerateEmbeddings/typed.py
--rw-r--r--   0        0        0     3366 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ModifyCode/ModifyCode.py
--rw-r--r--   0        0        0     1045 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ModifyCode/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ModifyCode/__init__.py
--rw-r--r--   0        0        0      346 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ModifyCode/typed.py
--rw-r--r--   0        0        0     3125 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/PreparePR/PreparePR.py
--rw-r--r--   0        0        0      743 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/PreparePR/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/PreparePR/__init__.py
--rw-r--r--   0        0        0      327 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/PreparePR/typed.py
--rw-r--r--   0        0        0     3289 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/PreparePrompt/PreparePrompt.py
--rw-r--r--   0        0        0     1274 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/PreparePrompt/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/PreparePrompt/__init__.py
--rw-r--r--   0        0        0      335 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/PreparePrompt/typed.py
--rw-r--r--   0        0        0     2617 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/QueryEmbeddings/QueryEmbeddings.py
--rw-r--r--   0        0        0     1117 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/QueryEmbeddings/README.md
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/QueryEmbeddings/__init__.py
--rw-r--r--   0        0        0      313 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/QueryEmbeddings/typed.py
--rw-r--r--   0        0        0     1652 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/README.md
--rw-r--r--   0        0        0     1078 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ReadIssues/README.md
--rw-r--r--   0        0        0     1149 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ReadIssues/ReadIssues.py
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ReadIssues/__init__.py
--rw-r--r--   0        0        0      277 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ReadIssues/typed.py
--rw-r--r--   0        0        0      903 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ReadPRDiffs/README.md
--rw-r--r--   0        0        0     1830 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ReadPRDiffs/__init__.py
--rw-r--r--   0        0        0      362 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ReadPRDiffs/typed.py
--rw-r--r--   0        0        0     1588 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ScanDepscan/README.md
--rw-r--r--   0        0        0     4884 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ScanDepscan/ScanDepscan.py
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ScanDepscan/__init__.py
--rw-r--r--   0        0        0      189 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ScanDepscan/typed.py
--rw-r--r--   0        0        0      677 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ScanSemgrep/README.md
--rw-r--r--   0        0        0     1096 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ScanSemgrep/ScanSemgrep.py
--rw-r--r--   0        0        0        0 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ScanSemgrep/__init__.py
--rw-r--r--   0        0        0      193 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/ScanSemgrep/typed.py
--rw-r--r--   0        0        0     2045 2024-05-09 11:24:31.220579 patchwork_cli-0.0.8/patchwork/steps/__init__.py
--rw-r--r--   0        0        0     2285 2024-05-09 11:24:31.224580 patchwork_cli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     8194 1970-01-01 00:00:00.000000 patchwork_cli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/LICENSE
+-rw-r--r--   0        0        0     5037 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/__main__.py
+-rw-r--r--   0        0        0     5253 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/app.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/common/client/__init__.py
+-rw-r--r--   0        0        0    15540 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/common/client/scm.py
+-rw-r--r--   0        0        0     3945 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/common/utils.py
+-rw-r--r--   0        0        0     1546 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/logger.py
+-rw-r--r--   0        0        0      168 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/managed_files.py
+-rw-r--r--   0        0        0     3718 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/AutoFix.py
+-rw-r--r--   0        0        0     6059 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/README.md
+-rw-r--r--   0        0        0     2182 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/default_prompt.json
+-rw-r--r--   0        0        0      919 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/defaults.yml
+-rw-r--r--   0        0        0     5422 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
+-rw-r--r--   0        0        0     5441 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/README.md
+-rw-r--r--   0        0        0      754 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/defaults.yml
+-rw-r--r--   0        0        0     2495 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
+-rw-r--r--   0        0        0     2204 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/GenerateREADME.py
+-rw-r--r--   0        0        0     3855 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/README.md
+-rw-r--r--   0        0        0      662 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/defaults.yml
+-rw-r--r--   0        0        0      484 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
+-rw-r--r--   0        0        0     3542 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/PRReview/PRReview.py
+-rw-r--r--   0        0        0     3653 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/PRReview/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/PRReview/__init__.py
+-rw-r--r--   0        0        0      659 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/PRReview/defaults.yml
+-rw-r--r--   0        0        0      557 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/PRReview/pr_review_prompt.json
+-rw-r--r--   0        0        0     2163 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/README.md
+-rw-r--r--   0        0        0     3773 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/README.md
+-rw-r--r--   0        0        0     3819 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/ResolveIssue.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/defaults.yml
+-rw-r--r--   0        0        0      728 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/prompt.json
+-rw-r--r--   0        0        0      344 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/patchflows/__init__.py
+-rw-r--r--   0        0        0      499 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/step.py
+-rw-r--r--   0        0        0     5984 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
+-rw-r--r--   0        0        0     1205 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/__init__.py
+-rw-r--r--   0        0        0      501 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/typed.py
+-rw-r--r--   0        0        0     2461 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
+-rw-r--r--   0        0        0      967 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/README.md
+-rw-r--r--   0        0        0      575 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/typed.py
+-rw-r--r--   0        0        0     7462 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallLLM/CallLLM.py
+-rw-r--r--   0        0        0      503 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallLLM/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallLLM/__init__.py
+-rw-r--r--   0        0        0      453 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CallLLM/typed.py
+-rw-r--r--   0        0        0     5255 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CommitChanges/CommitChanges.py
+-rw-r--r--   0        0        0     1106 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CommitChanges/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CommitChanges/__init__.py
+-rw-r--r--   0        0        0      368 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CommitChanges/typed.py
+-rw-r--r--   0        0        0     1346 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/CreateIssueComment.py
+-rw-r--r--   0        0        0      541 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/__init__.py
+-rw-r--r--   0        0        0      320 2024-05-09 09:16:47.285329 patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/typed.py
+-rw-r--r--   0        0        0     3907 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePR/CreatePR.py
+-rw-r--r--   0        0        0     1279 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePR/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePR/__init__.py
+-rw-r--r--   0        0        0      437 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePR/typed.py
+-rw-r--r--   0        0        0     1358 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/CreatePRComment.py
+-rw-r--r--   0        0        0      621 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/typed.py
+-rw-r--r--   0        0        0    11511 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/ExtractCode.py
+-rw-r--r--   0        0        0      755 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/__init__.py
+-rw-r--r--   0        0        0     2585 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
+-rw-r--r--   0        0        0      593 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/generic.py
+-rw-r--r--   0        0        0     1491 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/java.py
+-rw-r--r--   0        0        0     2442 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/javascript.py
+-rw-r--r--   0        0        0      281 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/protocol.py
+-rw-r--r--   0        0        0     2885 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/python.py
+-rw-r--r--   0        0        0      463 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractCode/typed.py
+-rw-r--r--   0        0        0     8722 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/ExtractDiff.py
+-rw-r--r--   0        0        0      833 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/__init__.py
+-rw-r--r--   0        0        0      404 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/typed.py
+-rw-r--r--   0        0        0     1648 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
+-rw-r--r--   0        0        0     1318 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/__init__.py
+-rw-r--r--   0        0        0      301 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/typed.py
+-rw-r--r--   0        0        0    12415 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
+-rw-r--r--   0        0        0     1765 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/README.md
+-rw-r--r--   0        0        0     6173 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/__init__.py
+-rw-r--r--   0        0        0      338 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/typed.py
+-rw-r--r--   0        0        0     5337 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/GenerateCodeRepositoryEmbeddings.py
+-rw-r--r--   0        0        0     1572 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/typed.py
+-rw-r--r--   0        0        0     2941 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/GenerateEmbeddings.py
+-rw-r--r--   0        0        0     1011 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/__init__.py
+-rw-r--r--   0        0        0      238 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/typed.py
+-rw-r--r--   0        0        0     3366 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ModifyCode/ModifyCode.py
+-rw-r--r--   0        0        0     1045 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ModifyCode/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ModifyCode/__init__.py
+-rw-r--r--   0        0        0      346 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ModifyCode/typed.py
+-rw-r--r--   0        0        0     3125 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePR/PreparePR.py
+-rw-r--r--   0        0        0      743 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePR/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePR/__init__.py
+-rw-r--r--   0        0        0      327 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePR/typed.py
+-rw-r--r--   0        0        0     3289 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/PreparePrompt.py
+-rw-r--r--   0        0        0     1274 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/__init__.py
+-rw-r--r--   0        0        0      335 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/typed.py
+-rw-r--r--   0        0        0     2617 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/QueryEmbeddings.py
+-rw-r--r--   0        0        0     1117 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/__init__.py
+-rw-r--r--   0        0        0      313 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/typed.py
+-rw-r--r--   0        0        0     1652 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/README.md
+-rw-r--r--   0        0        0     1078 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadIssues/README.md
+-rw-r--r--   0        0        0     1149 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadIssues/ReadIssues.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadIssues/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadIssues/typed.py
+-rw-r--r--   0        0        0      903 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/README.md
+-rw-r--r--   0        0        0     1830 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/__init__.py
+-rw-r--r--   0        0        0      362 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/typed.py
+-rw-r--r--   0        0        0     1588 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/README.md
+-rw-r--r--   0        0        0     4884 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/ScanDepscan.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/__init__.py
+-rw-r--r--   0        0        0      189 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/typed.py
+-rw-r--r--   0        0        0      677 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/README.md
+-rw-r--r--   0        0        0     1096 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/ScanSemgrep.py
+-rw-r--r--   0        0        0        0 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/typed.py
+-rw-r--r--   0        0        0     2045 2024-05-09 09:16:47.289329 patchwork_cli-0.0.87/patchwork/steps/__init__.py
+-rw-r--r--   0        0        0     2286 2024-05-09 09:16:47.293329 patchwork_cli-0.0.87/pyproject.toml
+-rw-r--r--   0        0        0     6852 1970-01-01 00:00:00.000000 patchwork_cli-0.0.87/PKG-INFO
```

### Comparing `patchwork_cli-0.0.8/LICENSE` & `patchwork_cli-0.0.87/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/README.md` & `patchwork_cli-0.0.87/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,106 @@
-<div align="center">
-  <picture>
-    <img alt="Patchwork logo" src="https://repository-images.githubusercontent.com/782544882/a9743f35-5e1c-43ed-a0e0-536322056d38" width="36%">
-  </picture>
-</div>
-
-<br>
-
-<div align="center">
-
-[![Build Status](https://img.shields.io/github/actions/workflow/status/patched-codes/patchwork/release.yml?logo=github)]()
-[![Downloads](https://static.pepy.tech/badge/patchwork-cli)](https://pepy.tech/project/patchwork-cli)
-[![Discord](https://img.shields.io/discord/1236886480471855104?style=flat&logo=discord&logoColor=white&label=discord)](https://discord.gg/FVcSNW6v)
-
-[Demo](https://youtu.be/3gRpqQoIino) |
-[Docs](https://docs.patched.codes/)
-
-</div>
-
+<p align="center">
+  <img src="https://github.com/patched-codes/patchwork/assets/126385808/a7adcf24-b615-43a0-a244-45789d184f0a" width="160" alt="PatchWork Logo">
+</p>
 
 # PatchWork
 
 An open-source framework for automating development chores using large language models. PatchWork allows you to automate workflows like PR reviews, bug fixing, security patching, and more using a self-hosted CLI agent and your preferred LLMs.
 
 ## Key Components
 
-- **Steps**: Reusable atomic actions like Create PR, commit changes, call an LLM etc
-- **Prompt Templates**: Customizable LLM prompts optimized for a chore like library updates, code generation, issue analysis etc.
-- **Patchflows**: LLM-assisted automations such as PR reviews, code fixing, documentation etc. built by combining steps and prompts.
-
-Patchflows can be run locally in your CLI and IDE, or as part of your CI/CD pipeline. There are [5 patchflows available][] out of the box, and you can always [create your own][].
-
-## Quickstart
+- **Steps**: A set of reusable atomic actions that define various operations.
+- **Patchflows**: LLM-assisted automations such as PR reviews, code fixing, debugging.
 
-[![Patchwork CLI Quickstart](https://img.youtube.com/vi/3gRpqQoIino/0.jpg)](https://youtu.be/3gRpqQoIino)
+Patchflows can be run locally in your CLI and IDE, or as part of your CI/CD pipeline.
 
 ## Installation
 
 ### Using Pip
 
 PatchWork is available on PyPI and can be installed using pip:
 
 ```bash
 pip install patchwork-cli --upgrade
 ```
 
 ### Using Poetry
 
-If you'd like to build from source using poetry, please see detailed documentation `here`[file](INSTALL.md) .
+PatchWork is built using Poetry, a dependency management and packaging tool for Python. To install PatchWork using Poetry, follow these steps:
+
+1. Make sure you have Poetry installed. If you don't have it installed, you can install it by running:
+   ```
+   curl -sSL https://install.python-poetry.org | python3 -
+   ```
+
+2. Clone the PatchWork repository:
+   ```
+   git clone https://github.com/patched-codes/patchwork.git
+   ```
+
+3. Navigate to the project directory:
+   ```
+   cd patchwork
+   ```
+
+4. Activate a shell using virtual environment:
+   ```
+   poetry shell
+   ```
+
+5. Install the dependencies using Poetry:
+   ```
+   poetry install
+   ```
 
 ## PatchWork CLI
 
 The CLI runs Patchflows, as follows:
 
 ```
-patchwork <PatchFlow> <?Arguments>
+patchwork <Patchflow> <?Arguments>
 ```
 
 Where
 - **Arguments**: Allow for overriding default/optional attributes of the Patchflow in the format of `key=value`. If `key` does not have any value, it is considered a boolean `True` flag.
 
 ### Example
 
 For an AutoFix patchflow which patches vulnerabilities based on a scan using Semgrep:
 
 ```bash
 patchwork AutoFix openai_api_key=<YOUR_OPENAI_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
-The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities. You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
+The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities.
 
-You can replace the OpenAI key with a key from our managed service
+You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. You will need to pass your own `openai_api_key` to call the LLM. Otherwise, to get started, you can get a `patched_api_key` for free by
 by signing in at [https://app.patched.codes/signin](https://app.patched.codes/signin) and generating an API key from the integrations tab. You can then call the patchflow with the key as follows:
 
 ```bash
 patchwork AutoFix patched_api_key=<YOUR_PATCHED_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
+Similarly, to use Google's models you can set the `google_api_key` and `model`, this is useful if you want to work with large contexts as the `gemini-pro-1.5` model supports a input context length of 1 million tokens.
 
-Similarly, to use Google's models you can set the `google_api_key` and `model`, this is useful if you want to work with large contexts as the `gemini-pro-1.5` model supports an input context length of 1 million tokens.
-
-The [patchwork-template](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
+The [patchwork-configs](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
 
 ```bash
 patchwork AutoFix --config /path/to/patchwork-configs/patchflows
 ```
 
 ## Patchflows
 
 Patchwork comes with a set of predefined patchflows, and more will be added over time. Below is a sample list of patchflows:
 
 - **AutoFix**: Generate and apply fixes to code vulnerabilities in a repository.
+- **DependencyUpgrade**: Update your dependencies from vulnerable to fixed versions.
 - **PRReview**: On PR creation, extract code diff, summarize changes, and comment on PR.
-- **GenerateREADME**: Create a README markdown file for a given folder, to add documentation to your repository.
-- **[Experimental] DependencyUpgrade**: Update your dependencies from vulnerable to fixed versions.
-- **[Experimental] ResolveIssue**: Identify the files in your repository that need to be updated to resolve an issue (or bug) and create a PR to fix it.
+- **GenerateREADME**: Create a README.md file for a given folder, to add documentation to your repository.
+- **ResolveIssue**: Identify the files in your repository that need to be updated to resolve an issue (or bug) and create a PR to fix it.
 
 ## Prompt Templates
 
 Prompt templates are used by patchflows and passed as queries to LLMs. Templates contain prompts with placeholder variables enclosed by {{}} which are replaced by the data from the steps or inputs on every run. 
 
 Below is a sample prompt template:
 
@@ -113,35 +116,15 @@
 }
 ```
 
 Each patchflow comes with an optimized default prompt template. But you can specify your own using the `prompt_template_file=/path/to/prompt/template/file` option. 
 
 ## Contributing
 
-Contributions for new patchflows and steps, or even to the core framework are welcome. Please look at open issues for details.
+To create a new patchflow, follow [these instructions](patchwork/patchflows/README.md).
 
-- To create a new patchflow, follow [these instructions](patchwork/patchflows/README.md).
-- To create a new step, follow [these instructions](patchwork/steps/README.md).
+To create a new step, follow [these instructions](patchwork/steps/README.md).
 
-We also provide chat assistants to help you create new steps and patchflows easily. Fair warning: they suffer from the same limitations as their underlying model.
+We also provide chat assitants to help you create new steps and patchflows easily.
 
 - [Patchwork Assistant GPT](https://chatgpt.com/g/g-0G4sCAd2y-patchwork-assistant) (requires ChatGPT pro subscription)
 - [Patchwork Assistant on HuggingChat ](https://hf.co/chat/assistant/66322701fd4787e0c1f7696b) (free)
-
-## Roadmap
-
-### Short Term Q2 '24
-- Expand patchflow library and integration options
-- Patchflow debugger and validation module
-- Bug fixing and performance improvements
-- Refactor code and documentation
-
-### Long Term Q3/Q4 '24
-- Support large-scale code embeddings in patchflows
-- Support parallelization and branching
-- Fine-tuned models that can be self-hosted
-- Open-source GUI
-
-## License
-
-Patchwork is licensed under [AGPL-3.0 terms](https://github.com/patched-codes/patchwork?tab=AGPL-3.0-1-ov-file#readme). However, custom patchflows and steps can be created and shared using the [patchwork template](https://github.com/patched-codes/patchwork-configs) repository which is licensed under [Apache-2.0 terms](https://github.com/patched-codes/patchwork-configs/blob/main/LICENSE).
-
```

### Comparing `patchwork_cli-0.0.8/patchwork/app.py` & `patchwork_cli-0.0.87/patchwork/app.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/common/client/scm.py` & `patchwork_cli-0.0.87/patchwork/common/client/scm.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/common/utils.py` & `patchwork_cli-0.0.87/patchwork/common/utils.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/logger.py` & `patchwork_cli-0.0.87/patchwork/logger.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/AutoFix/AutoFix.py` & `patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/AutoFix.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/AutoFix/README.md` & `patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/AutoFix/default_prompt.json` & `patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/default_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/AutoFix/defaults.yml` & `patchwork_cli-0.0.87/patchwork/patchflows/AutoFix/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py` & `patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/DependencyUpgrade/README.md` & `patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/DependencyUpgrade/defaults.yml` & `patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json` & `patchwork_cli-0.0.87/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/GenerateREADME/GenerateREADME.py` & `patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/GenerateREADME.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/GenerateREADME/README.md` & `patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/GenerateREADME/defaults.yml` & `patchwork_cli-0.0.87/patchwork/patchflows/GenerateREADME/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/PRReview/PRReview.py` & `patchwork_cli-0.0.87/patchwork/patchflows/PRReview/PRReview.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/PRReview/README.md` & `patchwork_cli-0.0.87/patchwork/patchflows/PRReview/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/PRReview/defaults.yml` & `patchwork_cli-0.0.87/patchwork/patchflows/PRReview/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/PRReview/pr_review_prompt.json` & `patchwork_cli-0.0.87/patchwork/patchflows/PRReview/pr_review_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/README.md` & `patchwork_cli-0.0.87/patchwork/patchflows/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/ResolveIssue/README.md` & `patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/ResolveIssue/ResolveIssue.py` & `patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/ResolveIssue.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/ResolveIssue/defaults.yml` & `patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/patchflows/ResolveIssue/prompt.json` & `patchwork_cli-0.0.87/patchwork/patchflows/ResolveIssue/prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py` & `patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/AnalyzeImpact/README.md` & `patchwork_cli-0.0.87/patchwork/steps/AnalyzeImpact/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py` & `patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CallCode2Prompt/README.md` & `patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py` & `patchwork_cli-0.0.87/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CallLLM/CallLLM.py` & `patchwork_cli-0.0.87/patchwork/steps/CallLLM/CallLLM.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CommitChanges/CommitChanges.py` & `patchwork_cli-0.0.87/patchwork/steps/CommitChanges/CommitChanges.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CommitChanges/README.md` & `patchwork_cli-0.0.87/patchwork/steps/CommitChanges/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CreateIssueComment/CreateIssueComment.py` & `patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/CreateIssueComment.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CreateIssueComment/README.md` & `patchwork_cli-0.0.87/patchwork/steps/CreateIssueComment/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CreatePR/CreatePR.py` & `patchwork_cli-0.0.87/patchwork/steps/CreatePR/CreatePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CreatePR/README.md` & `patchwork_cli-0.0.87/patchwork/steps/CreatePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CreatePRComment/CreatePRComment.py` & `patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/CreatePRComment.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/CreatePRComment/README.md` & `patchwork_cli-0.0.87/patchwork/steps/CreatePRComment/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractCode/ExtractCode.py` & `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/ExtractCode.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractCode/README.md` & `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/context_strategies.py` & `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/context_strategies.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/generic.py` & `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/generic.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/java.py` & `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/java.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/javascript.py` & `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/javascript.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractCode/context_strategy/python.py` & `patchwork_cli-0.0.87/patchwork/steps/ExtractCode/context_strategy/python.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractDiff/ExtractDiff.py` & `patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/ExtractDiff.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractDiff/README.md` & `patchwork_cli-0.0.87/patchwork/steps/ExtractDiff/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py` & `patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractModelResponse/README.md` & `patchwork_cli-0.0.87/patchwork/steps/ExtractModelResponse/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py` & `patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractPackageManagerFile/README.md` & `patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py` & `patchwork_cli-0.0.87/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/GenerateCodeRepositoryEmbeddings/GenerateCodeRepositoryEmbeddings.py` & `patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/GenerateCodeRepositoryEmbeddings.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/GenerateCodeRepositoryEmbeddings/README.md` & `patchwork_cli-0.0.87/patchwork/steps/GenerateCodeRepositoryEmbeddings/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/GenerateEmbeddings/GenerateEmbeddings.py` & `patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/GenerateEmbeddings.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/GenerateEmbeddings/README.md` & `patchwork_cli-0.0.87/patchwork/steps/GenerateEmbeddings/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ModifyCode/ModifyCode.py` & `patchwork_cli-0.0.87/patchwork/steps/ModifyCode/ModifyCode.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ModifyCode/README.md` & `patchwork_cli-0.0.87/patchwork/steps/ModifyCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/PreparePR/PreparePR.py` & `patchwork_cli-0.0.87/patchwork/steps/PreparePR/PreparePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/PreparePR/README.md` & `patchwork_cli-0.0.87/patchwork/steps/PreparePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/PreparePrompt/PreparePrompt.py` & `patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/PreparePrompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/PreparePrompt/README.md` & `patchwork_cli-0.0.87/patchwork/steps/PreparePrompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/QueryEmbeddings/QueryEmbeddings.py` & `patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/QueryEmbeddings.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/QueryEmbeddings/README.md` & `patchwork_cli-0.0.87/patchwork/steps/QueryEmbeddings/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/README.md` & `patchwork_cli-0.0.87/patchwork/steps/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ReadIssues/README.md` & `patchwork_cli-0.0.87/patchwork/steps/ReadIssues/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ReadIssues/ReadIssues.py` & `patchwork_cli-0.0.87/patchwork/steps/ReadIssues/ReadIssues.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ReadPRDiffs/README.md` & `patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py` & `patchwork_cli-0.0.87/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ScanDepscan/README.md` & `patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ScanDepscan/ScanDepscan.py` & `patchwork_cli-0.0.87/patchwork/steps/ScanDepscan/ScanDepscan.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ScanSemgrep/README.md` & `patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/ScanSemgrep/ScanSemgrep.py` & `patchwork_cli-0.0.87/patchwork/steps/ScanSemgrep/ScanSemgrep.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/patchwork/steps/__init__.py` & `patchwork_cli-0.0.87/patchwork/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.8/pyproject.toml` & `patchwork_cli-0.0.87/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "patchwork-cli"
-version = "0.0.8"
+version = "0.0.87"
 description = ""
 authors = ["patched.codes"]
 license = "AGPL"
 readme = "README.md"
 packages = [
     { include = "patchwork", from = "." }
 ]
```

### Comparing `patchwork_cli-0.0.8/PKG-INFO` & `patchwork_cli-0.0.87/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-cli
-Version: 0.0.8
+Version: 0.0.87
 Summary: 
 License: AGPL
 Author: patched.codes
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -38,110 +38,113 @@
 Requires-Dist: semver (>=3.0.2,<3.1.0)
 Requires-Dist: sentence-transformers (>=2.7.0,<2.8.0)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Requires-Dist: torch (>=2.2.2,<2.3.0)
 Requires-Dist: tree-sitter-languages (>=1.10.2,<2.0.0)
 Description-Content-Type: text/markdown
 
-<div align="center">
-  <picture>
-    <img alt="Patchwork logo" src="https://repository-images.githubusercontent.com/782544882/a9743f35-5e1c-43ed-a0e0-536322056d38" width="36%">
-  </picture>
-</div>
-
-<br>
-
-<div align="center">
-
-[![Build Status](https://img.shields.io/github/actions/workflow/status/patched-codes/patchwork/release.yml?logo=github)]()
-[![Downloads](https://static.pepy.tech/badge/patchwork-cli)](https://pepy.tech/project/patchwork-cli)
-[![Discord](https://img.shields.io/discord/1236886480471855104?style=flat&logo=discord&logoColor=white&label=discord)](https://discord.gg/FVcSNW6v)
-
-[Demo](https://youtu.be/3gRpqQoIino) |
-[Docs](https://docs.patched.codes/)
-
-</div>
-
+<p align="center">
+  <img src="https://github.com/patched-codes/patchwork/assets/126385808/a7adcf24-b615-43a0-a244-45789d184f0a" width="160" alt="PatchWork Logo">
+</p>
 
 # PatchWork
 
 An open-source framework for automating development chores using large language models. PatchWork allows you to automate workflows like PR reviews, bug fixing, security patching, and more using a self-hosted CLI agent and your preferred LLMs.
 
 ## Key Components
 
-- **Steps**: Reusable atomic actions like Create PR, commit changes, call an LLM etc
-- **Prompt Templates**: Customizable LLM prompts optimized for a chore like library updates, code generation, issue analysis etc.
-- **Patchflows**: LLM-assisted automations such as PR reviews, code fixing, documentation etc. built by combining steps and prompts.
-
-Patchflows can be run locally in your CLI and IDE, or as part of your CI/CD pipeline. There are [5 patchflows available][] out of the box, and you can always [create your own][].
-
-## Quickstart
+- **Steps**: A set of reusable atomic actions that define various operations.
+- **Patchflows**: LLM-assisted automations such as PR reviews, code fixing, debugging.
 
-[![Patchwork CLI Quickstart](https://img.youtube.com/vi/3gRpqQoIino/0.jpg)](https://youtu.be/3gRpqQoIino)
+Patchflows can be run locally in your CLI and IDE, or as part of your CI/CD pipeline.
 
 ## Installation
 
 ### Using Pip
 
 PatchWork is available on PyPI and can be installed using pip:
 
 ```bash
 pip install patchwork-cli --upgrade
 ```
 
 ### Using Poetry
 
-If you'd like to build from source using poetry, please see detailed documentation `here`[file](INSTALL.md) .
+PatchWork is built using Poetry, a dependency management and packaging tool for Python. To install PatchWork using Poetry, follow these steps:
+
+1. Make sure you have Poetry installed. If you don't have it installed, you can install it by running:
+   ```
+   curl -sSL https://install.python-poetry.org | python3 -
+   ```
+
+2. Clone the PatchWork repository:
+   ```
+   git clone https://github.com/patched-codes/patchwork.git
+   ```
+
+3. Navigate to the project directory:
+   ```
+   cd patchwork
+   ```
+
+4. Activate a shell using virtual environment:
+   ```
+   poetry shell
+   ```
+
+5. Install the dependencies using Poetry:
+   ```
+   poetry install
+   ```
 
 ## PatchWork CLI
 
 The CLI runs Patchflows, as follows:
 
 ```
-patchwork <PatchFlow> <?Arguments>
+patchwork <Patchflow> <?Arguments>
 ```
 
 Where
 - **Arguments**: Allow for overriding default/optional attributes of the Patchflow in the format of `key=value`. If `key` does not have any value, it is considered a boolean `True` flag.
 
 ### Example
 
 For an AutoFix patchflow which patches vulnerabilities based on a scan using Semgrep:
 
 ```bash
 patchwork AutoFix openai_api_key=<YOUR_OPENAI_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
-The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities. You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. 
+The above command will default to patching code in the current directory, by running Semgrep to identify the vulnerabilities.
 
-You can replace the OpenAI key with a key from our managed service
+You can take a look at the `default.yml` [file](patchwork/patchflows/AutoFix/defaults.yml) for the list of configurations you can set to manage the AutoFix patchflow. You will need to pass your own `openai_api_key` to call the LLM. Otherwise, to get started, you can get a `patched_api_key` for free by
 by signing in at [https://app.patched.codes/signin](https://app.patched.codes/signin) and generating an API key from the integrations tab. You can then call the patchflow with the key as follows:
 
 ```bash
 patchwork AutoFix patched_api_key=<YOUR_PATCHED_API_KEY> github_api_key=<YOUR_GITHUB_TOKEN>
 ```
 
+Similarly, to use Google's models you can set the `google_api_key` and `model`, this is useful if you want to work with large contexts as the `gemini-pro-1.5` model supports a input context length of 1 million tokens.
 
-Similarly, to use Google's models you can set the `google_api_key` and `model`, this is useful if you want to work with large contexts as the `gemini-pro-1.5` model supports an input context length of 1 million tokens.
-
-The [patchwork-template](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
+The [patchwork-configs](https://github.com/patched-codes/patchwork-configs) repository contains the default configuration and prompts for all the patchflows. You can clone that repo and pass it as a flag to the CLI:
 
 ```bash
 patchwork AutoFix --config /path/to/patchwork-configs/patchflows
 ```
 
 ## Patchflows
 
 Patchwork comes with a set of predefined patchflows, and more will be added over time. Below is a sample list of patchflows:
 
 - **AutoFix**: Generate and apply fixes to code vulnerabilities in a repository.
+- **DependencyUpgrade**: Update your dependencies from vulnerable to fixed versions.
 - **PRReview**: On PR creation, extract code diff, summarize changes, and comment on PR.
-- **GenerateREADME**: Create a README markdown file for a given folder, to add documentation to your repository.
-- **[Experimental] DependencyUpgrade**: Update your dependencies from vulnerable to fixed versions.
-- **[Experimental] ResolveIssue**: Identify the files in your repository that need to be updated to resolve an issue (or bug) and create a PR to fix it.
+- **GenerateREADME**: Create a README.md file for a given folder, to add documentation to your repository.
+- **ResolveIssue**: Identify the files in your repository that need to be updated to resolve an issue (or bug) and create a PR to fix it.
 
 ## Prompt Templates
 
 Prompt templates are used by patchflows and passed as queries to LLMs. Templates contain prompts with placeholder variables enclosed by {{}} which are replaced by the data from the steps or inputs on every run. 
 
 Below is a sample prompt template:
 
@@ -157,36 +160,16 @@
 }
 ```
 
 Each patchflow comes with an optimized default prompt template. But you can specify your own using the `prompt_template_file=/path/to/prompt/template/file` option. 
 
 ## Contributing
 
-Contributions for new patchflows and steps, or even to the core framework are welcome. Please look at open issues for details.
+To create a new patchflow, follow [these instructions](patchwork/patchflows/README.md).
 
-- To create a new patchflow, follow [these instructions](patchwork/patchflows/README.md).
-- To create a new step, follow [these instructions](patchwork/steps/README.md).
+To create a new step, follow [these instructions](patchwork/steps/README.md).
 
-We also provide chat assistants to help you create new steps and patchflows easily. Fair warning: they suffer from the same limitations as their underlying model.
+We also provide chat assitants to help you create new steps and patchflows easily.
 
 - [Patchwork Assistant GPT](https://chatgpt.com/g/g-0G4sCAd2y-patchwork-assistant) (requires ChatGPT pro subscription)
 - [Patchwork Assistant on HuggingChat ](https://hf.co/chat/assistant/66322701fd4787e0c1f7696b) (free)
 
-## Roadmap
-
-### Short Term Q2 '24
-- Expand patchflow library and integration options
-- Patchflow debugger and validation module
-- Bug fixing and performance improvements
-- Refactor code and documentation
-
-### Long Term Q3/Q4 '24
-- Support large-scale code embeddings in patchflows
-- Support parallelization and branching
-- Fine-tuned models that can be self-hosted
-- Open-source GUI
-
-## License
-
-Patchwork is licensed under [AGPL-3.0 terms](https://github.com/patched-codes/patchwork?tab=AGPL-3.0-1-ov-file#readme). However, custom patchflows and steps can be created and shared using the [patchwork template](https://github.com/patched-codes/patchwork-configs) repository which is licensed under [Apache-2.0 terms](https://github.com/patched-codes/patchwork-configs/blob/main/LICENSE).
-
-
```

