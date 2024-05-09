# Comparing `tmp/ape-foundry-0.7.4.tar.gz` & `tmp/ape-foundry-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-foundry-0.7.4.tar", last modified: Fri Mar  8 21:19:53 2024, max compression
+gzip compressed data, was "ape-foundry-0.7.5.tar", last modified: Thu May  9 18:48:52 2024, max compression
```

## Comparing `ape-foundry-0.7.4.tar` & `ape-foundry-0.7.5.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.176632 ape-foundry-0.7.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.160632 ape-foundry-0.7.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.160632 ape-foundry-0.7.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.160632 ape-foundry-0.7.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-08 21:19:53.176632 ape-foundry-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.160632 ape-foundry-0.7.4/ape_foundry/
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/ape_foundry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/ape_foundry/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/ape_foundry/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37860 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/ape_foundry/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/ape_foundry/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-08 21:19:52.000000 ape-foundry-0.7.4/ape_foundry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.164632 ape-foundry-0.7.4/ape_foundry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-08 21:19:53.000000 ape-foundry-0.7.4/ape_foundry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-03-08 21:19:53.000000 ape-foundry-0.7.4/ape_foundry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 21:19:53.000000 ape-foundry-0.7.4/ape_foundry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 21:19:53.000000 ape-foundry-0.7.4/ape_foundry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-08 21:19:53.000000 ape-foundry-0.7.4/ape_foundry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-08 21:19:53.000000 ape-foundry-0.7.4/ape_foundry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-08 21:19:53.176632 ape-foundry-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.164632 ape-foundry-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.156632 ape-foundry-0.7.4/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.156632 ape-foundry-0.7.4/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.156632 ape-foundry-0.7.4/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.164632 ape-foundry-0.7.4/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (127)    77599 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (127)    75147 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (127)    32313 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/local/has_error.json
--rw-r--r--   0 runner    (1001) docker     (127)    33356 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.156632 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.176632 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (127)    19792 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (127)    44429 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (127)    23253 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.176632 ape-foundry-0.7.4/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 21:19:53.176632 ape-foundry-0.7.4/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/sources/RevertsContractVy.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/data/sources/TokenB.vy
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17506 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-08 21:18:57.000000 ape-foundry-0.7.4/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.058081 ape-foundry-0.7.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.058081 ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.058081 ape-foundry-0.7.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.058081 ape-foundry-0.7.5/ape_foundry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/ape_foundry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/ape_foundry/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/ape_foundry/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37942 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/ape_foundry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/ape_foundry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.058081 ape-foundry-0.7.5/ape_foundry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-09 18:48:52.000000 ape-foundry-0.7.5/ape_foundry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 18:48:51.000000 ape-foundry-0.7.5/ape_foundry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.062081 ape-foundry-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7442 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.054081 ape-foundry-0.7.5/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.054081 ape-foundry-0.7.5/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.054081 ape-foundry-0.7.5/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.062081 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (127)    77599 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (127)    75147 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32313 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33356 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28197 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.054081 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17042 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6842 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19792 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44429 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13125 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23253 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15942 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16307 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16282 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:48:52.074081 ape-foundry-0.7.5/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/sources/RevertsContractVy.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/data/sources/TokenB.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17730 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-09 18:47:59.000000 ape-foundry-0.7.5/tests/test_trace.py
```

### Comparing `ape-foundry-0.7.4/.github/ISSUE_TEMPLATE/bug.md` & `ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/.github/ISSUE_TEMPLATE/feature.md` & `ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/.github/ISSUE_TEMPLATE/work-item.md` & `ape-foundry-0.7.5/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/.github/release-drafter.yml` & `ape-foundry-0.7.5/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/.github/workflows/codeql.yml` & `ape-foundry-0.7.5/.github/workflows/codeql.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       security-events: write
 
     strategy:
       fail-fast: false
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Initialize CodeQL
       uses: github/codeql-action/init@v2
       with:
         languages: python
 
     - name: Autobuild
```

### Comparing `ape-foundry-0.7.4/.github/workflows/commitlint.yaml` & `ape-foundry-0.7.5/.github/workflows/commitlint.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # NOTE: Skip check on PR so as not to confuse contributors
 # NOTE: Also install a PR title checker so we don't mess up merges
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
           with:
               fetch-depth: 0
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check commit history
```

### Comparing `ape-foundry-0.7.4/.github/workflows/prtitle.yaml` & `ape-foundry-0.7.5/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
```

### Comparing `ape-foundry-0.7.4/.github/workflows/publish.yaml` & `ape-foundry-0.7.5/.github/workflows/publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
```

### Comparing `ape-foundry-0.7.4/.github/workflows/stale-prs.yml` & `ape-foundry-0.7.5/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/.github/workflows/test.yaml` & `ape-foundry-0.7.5/.github/workflows/test.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,18 @@
   cancel-in-progress: true
 
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
@@ -38,18 +38,18 @@
         - name: Run mdformat
           run: mdformat . --check
 
     type-check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
@@ -58,27 +58,29 @@
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                # TODO: Replace with macos-latest when works again.
+                #   https://github.com/actions/setup-python/issues/808
+                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
+                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Install Foundry
           uses: foundry-rs/foundry-toolchain@v1
           with:
               version: nightly
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: pip install .[test]
 
         - name: Run Tests
@@ -98,18 +100,18 @@
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
 #
 #        steps:
-#        - uses: actions/checkout@v3
+#        - uses: actions/checkout@v4
 #
 #        - name: Setup Python
-#          uses: actions/setup-python@v4
+#          uses: actions/setup-python@v5
 #          with:
 #              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
```

### Comparing `ape-foundry-0.7.4/.gitignore` & `ape-foundry-0.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/.pre-commit-config.yaml` & `ape-foundry-0.7.5/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
 
--   repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.10.1
+-   repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.12.1
+    rev: 24.4.2
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
     rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.10.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-PyYAML, types-requests, types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
```

### Comparing `ape-foundry-0.7.4/CONTRIBUTING.md` & `ape-foundry-0.7.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/LICENSE` & `ape-foundry-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/PKG-INFO` & `ape-foundry-0.7.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-foundry
-Version: 0.7.4
+Version: 0.7.5
 Summary: ape-foundry: Ape network provider for Foundry
 Home-page: https://github.com/ApeWorX/ape-foundry
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
@@ -30,15 +31,15 @@
 # Quick Start
 
 Foundry network provider plugin for Ape.
 Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 - Foundry. See Foundry's [Installation](https://github.com/foundry-rs/foundry#installation) documentation for steps.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-foundry-0.7.4/README.md` & `ape-foundry-0.7.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Quick Start
 
 Foundry network provider plugin for Ape.
 Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 - Foundry. See Foundry's [Installation](https://github.com/foundry-rs/foundry#installation) documentation for steps.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-foundry-0.7.4/ape_foundry/__init__.py` & `ape-foundry-0.7.5/ape_foundry/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 
     for network in NETWORKS:
         yield "ethereum", f"{network}-fork", FoundryForkProvider
 
     yield "arbitrum", LOCAL_NETWORK_NAME, FoundryProvider
     yield "arbitrum", "mainnet-fork", FoundryForkProvider
     yield "arbitrum", "sepolia-fork", FoundryForkProvider
-    # TODO: Remove when goerli is sunset
-    yield "arbitrum", "goerli-fork", FoundryForkProvider
 
     yield "avalanche", LOCAL_NETWORK_NAME, FoundryProvider
     yield "avalanche", "mainnet-fork", FoundryForkProvider
     yield "avalanche", "fuji-fork", FoundryForkProvider
 
     yield "bsc", LOCAL_NETWORK_NAME, FoundryProvider
     yield "bsc", "mainnet-fork", FoundryForkProvider
@@ -45,24 +43,21 @@
     yield "fantom", LOCAL_NETWORK_NAME, FoundryProvider
     yield "fantom", "opera-fork", FoundryForkProvider
     yield "fantom", "testnet-fork", FoundryForkProvider
 
     yield "optimism", LOCAL_NETWORK_NAME, FoundryProvider
     yield "optimism", "mainnet-fork", FoundryForkProvider
     yield "optimism", "sepolia-fork", FoundryForkProvider
-    # TODO: Remove when goerli is sunset
-    yield "optimism", "goerli-fork", FoundryForkProvider
 
     yield "polygon", LOCAL_NETWORK_NAME, FoundryProvider
     yield "polygon", "mainnet-fork", FoundryForkProvider
-    yield "polygon", "mumbai-fork", FoundryForkProvider
+    yield "polygon", "amoy-fork", FoundryForkProvider
 
     yield "base", LOCAL_NETWORK_NAME, FoundryProvider
     yield "base", "mainnet-fork", FoundryForkProvider
-    yield "base", "goerli-fork", FoundryForkProvider
     yield "base", "sepolia-fork", FoundryForkProvider
 
     yield "blast", LOCAL_NETWORK_NAME, FoundryProvider
     yield "blast", "mainnet-fork", FoundryForkProvider
     yield "blast", "sepolia-fork", FoundryForkProvider
```

### Comparing `ape-foundry-0.7.4/ape_foundry/constants.py` & `ape-foundry-0.7.5/ape_foundry/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,29 +9,24 @@
             4370000: "byzantium",
             7280000: "petersburg",
             9069000: "istanbul",
             9200000: "muirglacier",
             12244000: "berlin",
             12965000: "london",
         },
-        "goerli": {
-            0: "petersburg",
-            1561651: "istanbul",
-            4460644: "berlin",
-            5062605: "london",
+        "sepolia": {
+            0: "london",
         },
     },
     "polygon": {
         "mainnet": {
             0: "petersburg",
             3395000: "muirglacier",
             14750000: "berlin",
             23850000: "london",
         },
-        "mumbai": {
-            0: "petersburg",
-            2722000: "muirglacier",
-            13996000: "berlin",
-            22640000: "london",
+        "amoy": {
+            0: "berlin",
+            73100: "london",
         },
     },
 }
```

### Comparing `ape-foundry-0.7.4/ape_foundry/exceptions.py` & `ape-foundry-0.7.5/ape_foundry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/ape_foundry/provider.py` & `ape-foundry-0.7.5/ape_foundry/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from ape_test import ApeTestConfig
 from eth_pydantic_types import HashBytes32, HexBytes
 from eth_typing import HexStr
 from eth_utils import add_0x_prefix, is_0x_prefixed, is_hex, to_hex
 from evm_trace import CallType, ParityTraceList
 from evm_trace import TraceFrame as EvmTraceFrame
 from evm_trace import get_calltree_from_geth_trace, get_calltree_from_parity_trace
-from pydantic import model_validator
+from pydantic import field_validator, model_validator
 from pydantic_settings import SettingsConfigDict
 from web3 import HTTPProvider, Web3
 from web3.exceptions import ContractCustomError
 from web3.exceptions import ContractLogicError as Web3ContractLogicError
 from web3.exceptions import ExtraDataLengthError
 from web3.gas_strategies.rpc import rpc_gas_price_strategy
 from web3.middleware import geth_poa_middleware
@@ -92,31 +92,37 @@
     gas_price: int = 0
 
     # For setting the values in --fork and --fork-block-number command arguments.
     # Used only in FoundryForkProvider.
     # Mapping of ecosystem_name => network_name => FoundryForkConfig
     fork: Dict[str, Dict[str, FoundryForkConfig]] = {}
 
+    disable_block_gas_limit: bool = False
     """
     Disable the ``call.gas_limit <= block.gas_limit`` constraint.
     """
-    disable_block_gas_limit: bool = False
 
     auto_mine: bool = True
     """
     Automatically mine blocks instead of manually doing so.
     """
 
     block_time: Optional[int] = None
     """
     Set a block time to allow mining to happen on an interval
     rather than only when a new transaction is submitted.
     """
+
     model_config = SettingsConfigDict(extra="allow")
 
+    @field_validator("fork", mode="before")
+    @classmethod
+    def _validate_fork(cls, value):
+        return value or {}
+
 
 def _call(*args):
     return call([*args], stderr=PIPE, stdout=PIPE, stdin=PIPE)
 
 
 class FoundryProvider(SubprocessProvider, Web3Provider, TestProviderAPI):
     _host: Optional[str] = None
@@ -568,15 +574,14 @@
                 vm_err = self.get_virtual_machine_error(err, txn=receipt)
                 raise vm_err from err
 
             # If we get here, for some reason the tx-replay did not produce
             # a VM error.
             receipt.raise_for_status()
 
-        logger.info(f"Confirmed {receipt.txn_hash} (total fees paid = {receipt.total_fees_paid})")
         self.chain_manager.history.append(receipt)
         return receipt
 
     def send_call(
         self,
         txn: TransactionAPI,
         block_id: Optional[BlockID] = None,
@@ -720,19 +725,20 @@
 
         def _handle_execution_reverted(
             exception: Exception, revert_message: Optional[str] = None, **kwargs
         ):
             if revert_message in ("", "0x", None):
                 revert_message = TransactionError.DEFAULT_MESSAGE
 
-            enriched = self.compiler_manager.enrich_error(
-                ContractLogicError(base_err=exception, revert_message=message, **kwargs)
+            sub_err = ContractLogicError(
+                base_err=exception, revert_message=revert_message, **kwargs
             )
+            enriched = self.compiler_manager.enrich_error(sub_err)
 
-            # Show call trace if availble
+            # Show call trace if available
             if enriched.txn:
                 # Unlikely scenario where a transaction is on the error even though a receipt
                 # exists.
                 if isinstance(enriched.txn, TransactionAPI) and enriched.txn.receipt:
                     enriched.txn.receipt.show_trace()
                 elif isinstance(enriched.txn, ReceiptAPI):
                     enriched.txn.show_trace()
```

### Comparing `ape-foundry-0.7.4/ape_foundry.egg-info/PKG-INFO` & `ape-foundry-0.7.5/ape_foundry.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-foundry
-Version: 0.7.4
+Version: 0.7.5
 Summary: ape-foundry: Ape network provider for Foundry
 Home-page: https://github.com/ApeWorX/ape-foundry
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,14 +14,15 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
@@ -30,15 +31,15 @@
 # Quick Start
 
 Foundry network provider plugin for Ape.
 Foundry is a development framework written in Rust for Ethereum that includes a local network implementation.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 - Foundry. See Foundry's [Installation](https://github.com/foundry-rs/foundry#installation) documentation for steps.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-foundry-0.7.4/ape_foundry.egg-info/SOURCES.txt` & `ape-foundry-0.7.5/ape_foundry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/ape_foundry.egg-info/requires.txt` & `ape-foundry-0.7.5/ape_foundry.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
 hypothesis<7.0,>=6.2.0
 ape-alchemy
 ape-polygon
-black<24,>=23.12.1
-mypy<2,>=1.8.0
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
 types-requests
 types-PyYAML
 flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
@@ -41,23 +41,23 @@
 
 [doc]
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 
 [lint]
-black<24,>=23.12.1
-mypy<2,>=1.8.0
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
 types-requests
 types-PyYAML
 flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
 setuptools
```

### Comparing `ape-foundry-0.7.4/pyproject.toml` & `ape-foundry-0.7.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-foundry-0.7.4/setup.py` & `ape-foundry-0.7.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "ape-alchemy",  # For running fork tests
         "ape-polygon",  # For running polygon fork tests
     ],
     "lint": [
-        "black>=23.12.1,<24",  # Auto-formatter and linter
-        "mypy>=1.8.0,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
         "types-requests",  # Needed for mypy type shed
         "types-PyYAML",  # Needed for mypy type shed
         "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "isort>=5.13.2,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "doc": [
         "Sphinx>=6.1.3,<7",  # Documentation generator
@@ -97,9 +96,10 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-foundry-0.7.4/tests/ape-config.yaml` & `ape-foundry-0.7.5/tests/ape-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     default_provider: alchemy
   local:
     default_provider: foundry
 
 polygon:
   local:
     default_provider: foundry
-  mumbai:
+  amoy:
     default_provider: alchemy
   mainnet:
     default_provider: alchemy
 
 foundry:
   request_timeout: 29
   fork_request_timeout: 360
@@ -21,17 +21,14 @@
   base_fee: 0
 
   fork:
     ethereum:
       mainnet:
         upstream_provider: alchemy
         block_number: 15776634
-      goerli:
-        upstream_provider: alchemy
-        block_number: 7849922
       sepolia:
         upstream_provider: alchemy
         block_number: 3091950
 
 test:
   # `false` because running pytest within pytest.
   disconnect_providers_after: false
```

### Comparing `ape-foundry-0.7.4/tests/conftest.py` & `ape-foundry-0.7.5/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 BASE_CONTRACTS_PATH = Path(__file__).parent / "data" / "contracts"
 LOCAL_CONTRACTS_PATH = BASE_CONTRACTS_PATH / "ethereum" / "local"
 NAME = "foundry"
 
 # Needed to test tracing support in core `ape test` command.
 pytest_plugins = ["pytester"]
 MAINNET_FORK_PORT = 9001
-GOERLI_FORK_PORT = 9002
+SEPOLIA_FORK_PORT = 9002
 
 
 def pytest_runtest_makereport(item, call):
     tr = orig_pytest_runtest_makereport(item, call)
     if call.excinfo is not None and "too many requests" in str(call.excinfo).lower():
         tr.outcome = "skipped"
         tr.wasxfail = "reason: Alchemy requests overloaded (likely in CI)"
@@ -226,32 +226,33 @@
     with mainnet_fork.use_provider(
         name, provider_settings={"host": f"http://127.0.0.1:{mainnet_fork_port}"}
     ) as provider:
         yield provider
 
 
 @pytest.fixture
-def goerli_fork_port():
-    return GOERLI_FORK_PORT
+def sepolia_fork_port():
+    return SEPOLIA_FORK_PORT
 
 
 @pytest.fixture
-def goerli_fork_provider(name, ethereum, goerli_fork_port):
-    with ethereum.goerli_fork.use_provider(
-        name, provider_settings={"host": f"http://127.0.0.1:{goerli_fork_port}"}
+def sepolia_fork_provider(name, ethereum, sepolia_fork_port):
+    with ethereum.sepolia_fork.use_provider(
+        name, provider_settings={"host": f"http://127.0.0.1:{sepolia_fork_port}"}
     ) as provider:
         yield provider
 
 
 @pytest.fixture(scope="session")
 def temp_config(config):
     @contextmanager
     def func(data: Dict, package_json: Optional[Dict] = None):
+        # TODO: Use `ape.utils.use_tempdir()` (once released)
         with tempfile.TemporaryDirectory() as temp_dir_str:
-            temp_dir = Path(temp_dir_str)
+            temp_dir = Path(temp_dir_str).resolve()
 
             config._cached_configs = {}
             config_file = temp_dir / CONFIG_FILE_NAME
             config_file.touch()
             config_file.write_text(yaml.dump(data))
             config.load(force_reload=True)
```

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/local/contract_a.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/local/contract_b.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/local/contract_c.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/local/has_error.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/has_error.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/local/token_a.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/local/token_b.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-foundry-0.7.5/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/python/pytest_tests.py` & `ape-foundry-0.7.5/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/sources/RevertsContractVy.vy` & `ape-foundry-0.7.5/tests/data/sources/RevertsContractVy.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/sources/TokenA.vy` & `ape-foundry-0.7.5/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/data/sources/TokenB.vy` & `ape-foundry-0.7.5/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/expected_traces.py` & `ape-foundry-0.7.5/tests/expected_traces.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/test_fork_provider.py` & `ape-foundry-0.7.5/tests/test_fork_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,97 +14,103 @@
 @pytest.fixture
 def mainnet_fork_contract_instance(owner, contract_container, mainnet_fork_provider):
     return owner.deploy(contract_container)
 
 
 @pytest.mark.fork
 def test_multiple_providers(
-    name, networks, ethereum, connected_provider, mainnet_fork_port, goerli_fork_port
+    name, networks, ethereum, connected_provider, mainnet_fork_port, sepolia_fork_port
 ):
     default_host = "http://127.0.0.1:8545"
     assert networks.active_provider.name == name
     assert networks.active_provider.network.name == LOCAL_NETWORK_NAME
     assert networks.active_provider.uri == default_host
     mainnet_fork_host = f"http://127.0.0.1:{mainnet_fork_port}"
 
     with ethereum.mainnet_fork.use_provider(name, provider_settings={"host": mainnet_fork_host}):
         assert networks.active_provider.name == name
         assert networks.active_provider.network.name == "mainnet-fork"
         assert networks.active_provider.uri == mainnet_fork_host
-        goerli_fork_host = f"http://127.0.0.1:{goerli_fork_port}"
+        sepolia_fork_host = f"http://127.0.0.1:{sepolia_fork_port}"
 
-        with ethereum.goerli_fork.use_provider(name, provider_settings={"host": goerli_fork_host}):
+        with ethereum.sepolia_fork.use_provider(
+            name, provider_settings={"host": sepolia_fork_host}
+        ):
             assert networks.active_provider.name == name
-            assert networks.active_provider.network.name == "goerli-fork"
-            assert networks.active_provider.uri == goerli_fork_host
+            assert networks.active_provider.network.name == "sepolia-fork"
+            assert networks.active_provider.uri == sepolia_fork_host
 
         assert networks.active_provider.name == name
         assert networks.active_provider.network.name == "mainnet-fork"
         assert networks.active_provider.uri == mainnet_fork_host
 
     assert networks.active_provider.name == name
     assert networks.active_provider.network.name == LOCAL_NETWORK_NAME
     assert networks.active_provider.uri == default_host
 
 
-@pytest.mark.parametrize("network", [k for k in NETWORKS.keys()])
+# TODO: Remove `in` check once goerli removed from core.
+@pytest.mark.parametrize("network", [k for k in NETWORKS.keys() if k not in ("goerli",)])
 def test_fork_config(name, config, network):
     plugin_config = config.get_config(name)
     network_config = plugin_config["fork"].get("ethereum", {}).get(network, {})
     message = f"Config not registered for network '{network}'."
     assert network_config.get("upstream_provider") == "alchemy", message
 
 
 @pytest.mark.fork
-def test_goerli_impersonate(accounts, goerli_fork_provider):
+def test_sepolia_impersonate(accounts, sepolia_fork_provider):
     impersonated_account = accounts[TEST_ADDRESS]
     other_account = accounts[0]
+    impersonated_account.balance += 1_000_000_000_000_000_000
     receipt = impersonated_account.transfer(other_account, "1 wei")
     assert receipt.receiver == other_account
     assert receipt.sender == impersonated_account
 
 
 @pytest.mark.fork
 def test_mainnet_impersonate(accounts, mainnet_fork_provider):
     impersonated_account = accounts[TEST_ADDRESS]
     other_account = accounts[0]
+    impersonated_account.balance += 1_000_000_000_000_000_000
     receipt = impersonated_account.transfer(other_account, "1 wei")
     assert receipt.receiver == other_account
     assert receipt.sender == impersonated_account
 
 
 @pytest.mark.fork
 def test_request_timeout(networks, config, mainnet_fork_provider):
     actual = mainnet_fork_provider.web3.provider._request_kwargs["timeout"]
     expected = 360  # Value set in `ape-config.yaml`
     assert actual == expected
 
     # Test default behavior
+    # TODO: Use `ape.utils.use_tempdir()` (once released)
     with tempfile.TemporaryDirectory() as temp_dir_str:
-        temp_dir = Path(temp_dir_str)
+        temp_dir = Path(temp_dir_str).resolve()
         with config.using_project(temp_dir):
             assert networks.active_provider.timeout == 300
 
 
 @pytest.mark.fork
-def test_reset_fork_no_fork_block_number(goerli_fork_provider):
-    goerli_fork_provider.mine(5)
-    prev_block_num = goerli_fork_provider.get_block("latest").number
-    goerli_fork_provider.reset_fork()
-    block_num_after_reset = goerli_fork_provider.get_block("latest").number
+def test_reset_fork_no_fork_block_number(sepolia_fork_provider):
+    sepolia_fork_provider.mine(5)
+    prev_block_num = sepolia_fork_provider.get_block("latest").number
+    sepolia_fork_provider.reset_fork()
+    block_num_after_reset = sepolia_fork_provider.get_block("latest").number
     assert block_num_after_reset < prev_block_num
 
 
 @pytest.mark.fork
-def test_reset_fork_specify_block_number_via_argument(goerli_fork_provider):
-    goerli_fork_provider.mine(5)
-    prev_block_num = goerli_fork_provider.get_block("latest").number
+def test_reset_fork_specify_block_number_via_argument(sepolia_fork_provider):
+    sepolia_fork_provider.mine(5)
+    prev_block_num = sepolia_fork_provider.get_block("latest").number
     new_block_number = prev_block_num - 1
-    goerli_fork_provider.reset_fork(block_number=new_block_number)
-    block_num_after_reset = goerli_fork_provider.get_block("latest").number
+    sepolia_fork_provider.reset_fork(block_number=new_block_number)
+    block_num_after_reset = sepolia_fork_provider.get_block("latest").number
     assert block_num_after_reset == new_block_number
 
 
 @pytest.mark.fork
 def test_reset_fork_specify_block_number_via_config(mainnet_fork_provider):
     mainnet_fork_provider.mine(5)
     mainnet_fork_provider.reset_fork()
@@ -167,21 +173,21 @@
 
 
 @pytest.mark.fork
 def test_connect_to_polygon(networks, owner, contract_container):
     """
     Ensures we don't get PoA middleware issue.
     """
-    with networks.polygon.mumbai_fork.use_provider("foundry"):
+    with networks.polygon.amoy_fork.use_provider("foundry"):
         contract = owner.deploy(contract_container)
         assert isinstance(contract, ContractInstance)  # Didn't fail
 
 
 @pytest.mark.fork
-@pytest.mark.parametrize("network,port", [("mumbai", 9878), ("mainnet", 9879)])
+@pytest.mark.parametrize("network,port", [("amoy", 9878), ("mainnet", 9879)])
 def test_provider_settings(networks, network, port):
     expected_block_number = 1234
     settings = {
         "host": f"http://127.0.0.1:{port}",
         "fork": {
             "polygon": {
                 network: {
```

### Comparing `ape-foundry-0.7.4/tests/test_provider.py` & `ape-foundry-0.7.5/tests/test_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ape_ethereum.transactions import TransactionStatusEnum, TransactionType
 from eth_pydantic_types import HashBytes32
 from eth_utils import encode_hex, to_int
 from evm_trace import CallType
 from hexbytes import HexBytes
 
 from ape_foundry import FoundryProviderError
-from ape_foundry.provider import FOUNDRY_CHAIN_ID, _extract_custom_error
+from ape_foundry.provider import FOUNDRY_CHAIN_ID, FoundryNetworkConfig, _extract_custom_error
 
 TEST_WALLET_ADDRESS = "0xD9b7fdb3FC0A0Aa3A507dCf0976bc23D49a9C7A3"
 
 
 def test_instantiation(disconnected_provider, name):
     assert disconnected_provider.name == name
 
@@ -155,16 +155,17 @@
 def test_request_timeout(connected_provider, config):
     # Test value set in `ape-config.yaml`
     expected = 29
     actual = connected_provider.web3.provider._request_kwargs["timeout"]
     assert actual == expected
 
     # Test default behavior
+    # TODO: Use `ape.utils.use_tempdir()` (once released)
     with tempfile.TemporaryDirectory() as temp_dir_str:
-        temp_dir = Path(temp_dir_str)
+        temp_dir = Path(temp_dir_str).resolve()
         with config.using_project(temp_dir):
             assert connected_provider.timeout == 30
 
 
 def test_contract_interaction(connected_provider, owner, contract_instance, mocker):
     # Spy on the estimate_gas RPC method.
     estimate_gas_spy = mocker.spy(connected_provider.web3.eth, "estimate_gas")
@@ -485,7 +486,12 @@
     provider._get_transaction_trace.side_effect = trace
 
     actual = _extract_custom_error(provider, txn=tx)
     assert actual == ""
 
     # Show failure was tracked
     assert tracker[0] == HexBytes(tx.txn_hash).hex()
+
+
+def test_fork_config_none():
+    cfg = FoundryNetworkConfig.model_validate({"fork": None})
+    assert isinstance(cfg["fork"], dict)
```

### Comparing `ape-foundry-0.7.4/tests/test_pytest.py` & `ape-foundry-0.7.5/tests/test_pytest.py`

 * *Files identical despite different names*

### Comparing `ape-foundry-0.7.4/tests/test_trace.py` & `ape-foundry-0.7.5/tests/test_trace.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,17 +58,18 @@
     return contract_a.methodWithoutArguments(sender=owner)
 
 
 def test_local_transaction_traces(local_receipt, captrace):
     # NOTE: Strange bug in Rich where we can't use sys.stdout for testing tree output.
     # And we have to write to a file, close it, and then re-open it to see output.
     def run_test():
+        # TODO: Use `ape.utils.use_tempdir()` (once released)
         with tempfile.TemporaryDirectory() as temp_dir:
             # Use a tempfile to avoid terminal inconsistencies affecting output.
-            file_path = Path(temp_dir) / "temp"
+            file_path = Path(temp_dir).resolve() / "temp"
             with open(file_path, "w") as file:
                 local_receipt.show_trace(file=file)
 
             with open(file_path, "r") as file:
                 lines = captrace.read_trace("Call trace for", file=file)
                 assert_rich_output(lines, LOCAL_TRACE)
 
@@ -76,16 +77,17 @@
 
     # Verify can happen more than once.
     run_test()
 
 
 def test_local_transaction_gas_report(local_receipt, captrace):
     def run_test():
+        # TODO: Use `ape.utils.use_tempdir()` (once released)
         with tempfile.TemporaryDirectory() as temp_dir:
-            temp_file = Path(temp_dir) / "temp"
+            temp_file = Path(temp_dir).resolve() / "temp"
             with open(temp_file, "w") as file:
                 local_receipt.show_gas_report(file=file)
 
             with open(temp_file, "r") as file:
                 lines = captrace.read_trace("ContractA Gas", file=file)
 
             assert_rich_output(lines, LOCAL_GAS_REPORT)
@@ -94,16 +96,17 @@
 
     # Verify can happen more than once.
     run_test()
 
 
 @pytest.mark.manual
 def test_mainnet_transaction_traces(mainnet_receipt, captrace):
+    # TODO: Use `ape.utils.use_tempdir()` (once released)
     with tempfile.TemporaryDirectory() as temp_dir:
-        temp_file = Path(temp_dir) / "temp"
+        temp_file = Path(temp_dir).resolve() / "temp"
 
         with open(temp_file, "w") as file:
             mainnet_receipt.show_trace(file=file)
 
         with open(temp_file, "r") as file:
             lines = captrace.read_trace("Call trace for", file=file)
```

