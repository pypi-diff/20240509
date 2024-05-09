# Comparing `tmp/schwifty-2024.5.0.tar.gz` & `tmp/schwifty-2024.5.1.tar.gz`

## Comparing `schwifty-2024.5.0.tar` & `schwifty-2024.5.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 schwifty-2024.5.0/.envrc
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schwifty-2024.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 schwifty-2024.5.0/.readthedocs.yml
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 schwifty-2024.5.0/CHANGELOG.rst
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 schwifty-2024.5.0/Makefile
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 schwifty-2024.5.0/devbox.json
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.0/devbox.lock
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 schwifty-2024.5.0/.github/workflows/lint-and-test.yml
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 schwifty-2024.5.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 schwifty-2024.5.0/docs/Makefile
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 schwifty-2024.5.0/docs/requirements.txt
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 schwifty-2024.5.0/docs/source/api.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 schwifty-2024.5.0/docs/source/changelog.rst
--rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 schwifty-2024.5.0/docs/source/conf.py
--rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 schwifty-2024.5.0/docs/source/examples.rst
--rw-r--r--   0        0        0   366898 2020-02-02 00:00:00.000000 schwifty-2024.5.0/docs/source/ilikewhatugot.png
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 schwifty-2024.5.0/docs/source/index.rst
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 schwifty-2024.5.0/docs/source/troubleshooting.rst
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/__init__.py
--rw-r--r--   0        0        0     8868 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bban.py
--rw-r--r--   0        0        0    16894 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bic.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/common.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/domain.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/exceptions.py
--rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/iban.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/py.typed
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/registry.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/README.md
--rw-r--r--   0        0        0   191535 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_at.json
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_ba.json
--rw-r--r--   0        0        0   134356 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_be.json
--rw-r--r--   0        0        0   218276 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_ch.json
--rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_cz.json
--rw-r--r--   0        0        0  1064251 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_de.json
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_ee.json
--rw-r--r--   0        0        0   105235 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_es.json
--rw-r--r--   0        0        0   123774 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_fi.json
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_ge.json
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_hr.json
--rw-r--r--   0        0        0    31389 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_hu.json
--rw-r--r--   0        0        0    59696 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_it.json
--rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_kz.json
--rw-r--r--   0        0        0    56450 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_lt.json
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_lv.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_md.json
--rw-r--r--   0        0        0    14272 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_nl.json
--rw-r--r--   0        0        0   406123 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_no.json
--rw-r--r--   0        0        0   768164 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_pl.json
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_ro.json
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_rs.json
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_se.json
--rw-r--r--   0        0        0   145633 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_si.json
--rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_sk.json
--rw-r--r--   0        0        0  1752206 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/generated_ua.json
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_ad.json
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_ae.json
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_bg.json
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_cr.json
--rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_cy.json
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_dk.json
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_es.json
--rw-r--r--   0        0        0    68361 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_fr.json
--rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_gb.json
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_gr.json
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_ie.json
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_il.json
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_is.json
--rw-r--r--   0        0        0    26893 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_it.json
--rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_lu.json
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_mc.json
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_me.json
--rw-r--r--   0        0        0    17257 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_pt.json
--rw-r--r--   0        0        0    25035 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_sa.json
--rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/bank_registry/manual_tr.json
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/__init__.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/albania.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/belgium.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/czech_republic.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/estonia.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/finland.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/france.py
--rw-r--r--   0        0        0    15549 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/germany.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/iceland.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/iso7064_mod97_10.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/iso7064_mod97_10_variant.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/italy.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/netherlands.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/norway.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/poland.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/registry.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/checksum/spain.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/iban_registry/README.md
--rw-r--r--   0        0        0    33306 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/iban_registry/generated.json
--rw-r--r--   0        0        0    16740 2020-02-02 00:00:00.000000 schwifty-2024.5.0/schwifty/iban_registry/overwrite.json
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/Dockerfile_se
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/README.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_at.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_be.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_ch.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_cz.py
--rwxr-xr-x   0        0        0     2066 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_de.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_es.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_fi.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_hr.py
--rwxr-xr-x   0        0        0     1213 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_hu.py
--rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_it.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_lt.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_lv.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_nl.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_no.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_pl.py
--rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_ro.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_se.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_si.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_sk.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_bank_registry_ua.py
--rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/get_iban_registry.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/requirements.txt
--rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 schwifty-2024.5.0/scripts/update-all.sh
--rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 schwifty-2024.5.0/tests/test_bic.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 schwifty-2024.5.0/tests/test_checksum.py
--rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 schwifty-2024.5.0/tests/test_iban.py
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 schwifty-2024.5.0/tests/test_registry.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 schwifty-2024.5.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 schwifty-2024.5.0/LICENSE
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 schwifty-2024.5.0/README.rst
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 schwifty-2024.5.0/hatch.toml
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 schwifty-2024.5.0/pyproject.toml
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 schwifty-2024.5.0/PKG-INFO
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.envrc
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0    20764 2020-02-02 00:00:00.000000 schwifty-2024.5.1/CHANGELOG.rst
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 schwifty-2024.5.1/Makefile
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 schwifty-2024.5.1/devbox.json
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.1/devbox.lock
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.github/workflows/lint-and-test.yml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/Makefile
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/requirements.txt
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/api.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/changelog.rst
+-rw-r--r--   0        0        0     6847 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/conf.py
+-rw-r--r--   0        0        0     7562 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/examples.rst
+-rw-r--r--   0        0        0   366898 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/ilikewhatugot.png
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/index.rst
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 schwifty-2024.5.1/docs/source/troubleshooting.rst
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/__init__.py
+-rw-r--r--   0        0        0     8868 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bban.py
+-rw-r--r--   0        0        0    16894 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bic.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/common.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/domain.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/exceptions.py
+-rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/iban.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/py.typed
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/registry.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/README.md
+-rw-r--r--   0        0        0   191535 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_at.json
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ba.json
+-rw-r--r--   0        0        0   134356 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_be.json
+-rw-r--r--   0        0        0   218276 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ch.json
+-rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_cz.json
+-rw-r--r--   0        0        0  1064251 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_de.json
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ee.json
+-rw-r--r--   0        0        0   105235 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_es.json
+-rw-r--r--   0        0        0   123774 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_fi.json
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ge.json
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_hr.json
+-rw-r--r--   0        0        0    31389 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_hu.json
+-rw-r--r--   0        0        0    59696 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_it.json
+-rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_kz.json
+-rw-r--r--   0        0        0    56450 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_lt.json
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_lv.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_md.json
+-rw-r--r--   0        0        0    14272 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_nl.json
+-rw-r--r--   0        0        0   406123 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_no.json
+-rw-r--r--   0        0        0   768164 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_pl.json
+-rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ro.json
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_rs.json
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_se.json
+-rw-r--r--   0        0        0   145633 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_si.json
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_sk.json
+-rw-r--r--   0        0        0  1752206 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/generated_ua.json
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_ad.json
+-rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_ae.json
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_bg.json
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_cr.json
+-rw-r--r--   0        0        0     8729 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_cy.json
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_dk.json
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_es.json
+-rw-r--r--   0        0        0    68361 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_fr.json
+-rw-r--r--   0        0        0     7604 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_gb.json
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_gr.json
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_ie.json
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_il.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_is.json
+-rw-r--r--   0        0        0    26893 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_it.json
+-rw-r--r--   0        0        0    21031 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_lu.json
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_mc.json
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_me.json
+-rw-r--r--   0        0        0    17257 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_pt.json
+-rw-r--r--   0        0        0    25035 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_sa.json
+-rw-r--r--   0        0        0    10797 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/bank_registry/manual_tr.json
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/__init__.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/albania.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/belgium.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/czech_republic.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/estonia.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/finland.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/france.py
+-rw-r--r--   0        0        0    15549 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/germany.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/iceland.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/iso7064_mod97_10.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/iso7064_mod97_10_variant.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/italy.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/netherlands.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/norway.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/poland.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/registry.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/checksum/spain.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/iban_registry/README.md
+-rw-r--r--   0        0        0    33306 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/iban_registry/generated.json
+-rw-r--r--   0        0        0    16740 2020-02-02 00:00:00.000000 schwifty-2024.5.1/schwifty/iban_registry/overwrite.json
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/Dockerfile_se
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/README.md
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_at.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_be.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_ch.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_cz.py
+-rwxr-xr-x   0        0        0     2066 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_de.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_es.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_fi.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_hr.py
+-rwxr-xr-x   0        0        0     1213 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_hu.py
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_it.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_lt.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_lv.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_nl.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_no.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_pl.py
+-rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_ro.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_se.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_si.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_sk.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_bank_registry_ua.py
+-rwxr-xr-x   0        0        0     3190 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/get_iban_registry.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/requirements.txt
+-rwxr-xr-x   0        0        0      322 2020-02-02 00:00:00.000000 schwifty-2024.5.1/scripts/update-all.sh
+-rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 schwifty-2024.5.1/tests/test_bic.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 schwifty-2024.5.1/tests/test_checksum.py
+-rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 schwifty-2024.5.1/tests/test_iban.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 schwifty-2024.5.1/tests/test_registry.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 schwifty-2024.5.1/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 schwifty-2024.5.1/LICENSE
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 schwifty-2024.5.1/README.rst
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 schwifty-2024.5.1/hatch.toml
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 schwifty-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 schwifty-2024.5.1/PKG-INFO
```

### Comparing `schwifty-2024.5.0/CHANGELOG.rst` & `schwifty-2024.5.1/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -2,1269 +2,1297 @@
 00000010: 4368 616e 6765 6c6f 670a 3d3d 3d3d 3d3d  Changelog.======
 00000020: 3d3d 3d0a 0a56 6572 7369 6f6e 7320 666f  ===..Versions fo
 00000030: 6c6c 6f77 2060 4361 6c56 6572 203c 6874  llow `CalVer <ht
 00000040: 7470 3a2f 2f77 7777 2e63 616c 7665 722e  tp://www.calver.
 00000050: 6f72 672f 3e60 5f20 7769 7468 2074 6865  org/>`_ with the
 00000060: 2073 6368 656d 6520 6060 5959 2e30 4d2e   scheme ``YY.0M.
 00000070: 4d69 6372 6f60 602e 0a0a 6032 3032 342e  Micro``...`2024.
-00000080: 3035 2e30 605f 202d 2032 3032 342f 3035  05.0`_ - 2024/05
-00000090: 2f30 370a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /07.------------
-000000a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 4669  -------------.Fi
-000000b0: 7865 640a 7e7e 7e7e 7e0a 2a20 4c6f 6164  xed.~~~~~.* Load
-000000c0: 696e 6720 4a53 4f4e 2064 6174 6120 696e  ing JSON data in
-000000d0: 746f 2061 2050 7964 616e 7469 6320 6d6f  to a Pydantic mo
-000000e0: 6465 6c20 7769 7468 2061 6e20 6060 4942  del with an ``IB
-000000f0: 414e 6060 206f 7220 6060 4249 4360 602d  AN`` or ``BIC``-
-00000100: 6669 656c 640a 2020 2860 604d 6f64 656c  field.  (``Model
-00000110: 2e6d 6f64 656c 5f76 616c 6964 6174 655f  .model_validate_
-00000120: 6a73 6f6e 2829 6060 2920 7761 7320 7072  json()``) was pr
-00000130: 6576 696f 7573 6c79 2062 726f 6b65 6e20  eviously broken 
-00000140: 616e 6420 6861 7320 6265 656e 2066 6978  and has been fix
-00000150: 6564 206e 6f77 2e0a 0a41 6464 6564 0a7e  ed now...Added.~
-00000160: 7e7e 7e7e 0a2a 204a 534f 4e20 7363 6865  ~~~~.* JSON sche
-00000170: 6d61 2067 656e 6572 6174 696f 6e20 666f  ma generation fo
-00000180: 7220 5079 6461 6e74 6963 206d 6f64 656c  r Pydantic model
-00000190: 732e 0a0a 4368 616e 6765 640a 7e7e 7e7e  s...Changed.~~~~
-000001a0: 7e7e 7e0a 2a20 5570 6461 7465 6420 6261  ~~~.* Updated ba
-000001b0: 6e6b 2072 6567 6973 7472 6965 732e 0a2a  nk registries..*
-000001c0: 2052 656d 6f76 6520 7468 6520 6465 7065   Remove the depe
-000001d0: 6e64 656e 6379 2074 6f20 6060 6973 6f33  ndency to ``iso3
-000001e0: 3136 3660 6020 7369 6e63 6520 6974 7320  166`` since its 
-000001f0: 6675 6e63 7469 6f6e 616c 6c69 7479 2069  functionallity i
-00000200: 7320 616c 7265 6164 7920 636f 7665 7265  s already covere
-00000210: 6420 6279 2060 6070 7963 6f75 6e74 7279  d by ``pycountry
-00000220: 6060 0a0a 0a60 3230 3234 2e30 342e 3060  ``...`2024.04.0`
-00000230: 5f20 2d20 3230 3234 2f30 342f 3138 0a2d  _ - 2024/04/18.-
-00000240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000250: 2d2d 2d2d 2d2d 2d2d 0a41 6464 6564 0a7e  --------.Added.~
-00000260: 7e7e 7e7e 0a2a 2041 6464 6564 2052 6576  ~~~~.* Added Rev
-00000270: 6f6c 7574 2042 616e 6b20 666f 7220 5370  olut Bank for Sp
-00000280: 6169 6e20 6040 6272 756e 6f76 696c 6c61  ain `@brunovilla
-00000290: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-000002a0: 2e63 6f6d 2f62 7275 6e6f 7669 6c61 3e60  .com/brunovila>`
-000002b0: 5f0a 2a20 4164 6465 6420 7375 7070 6f72  _.* Added suppor
-000002c0: 7420 666f 7220 5079 7468 6f6e 2033 2e31  t for Python 3.1
-000002d0: 320a 2a20 4164 6465 6420 6d61 6e75 616c  2.* Added manual
-000002e0: 6c79 2063 7572 6174 6564 2062 616e 6b20  ly curated bank 
-000002f0: 7265 6769 7374 7279 2066 6f72 204d 6f6e  registry for Mon
-00000300: 7465 6e65 6772 6f20 6040 446a 756b 6120  tenegro `@Djuka 
-00000310: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00000320: 636f 6d2f 446a 756b 613e 605f 0a0a 4368  com/Djuka>`_..Ch
-00000330: 616e 6765 640a 7e7e 7e7e 7e7e 7e0a 2a20  anged.~~~~~~~.* 
-00000340: 5468 6520 6261 6e6b 2072 6567 6973 7472  The bank registr
-00000350: 7920 6973 206e 6f77 2069 6e74 6572 6e61  y is now interna
-00000360: 6c6c 7920 7661 6c69 6461 7465 642c 2073  lly validated, s
-00000370: 6f20 7468 6174 2061 6c6c 2064 6f6d 6573  o that all domes
-00000380: 7469 6320 6261 6e6b 2063 6f64 6573 2061  tic bank codes a
-00000390: 6374 6175 6c6c 7920 6d61 7463 6820 7468  ctaully match th
-000003a0: 650a 2020 7370 6563 6966 6963 6174 696f  e.  specificatio
-000003b0: 6e20 6f66 2074 6865 2063 6f72 7265 7370  n of the corresp
-000003c0: 6f6e 6469 6e67 2042 4241 4e20 7374 7275  onding BBAN stru
-000003d0: 6374 7572 652e 2041 7320 6120 7265 7375  cture. As a resu
-000003e0: 6c74 2073 6f6d 6520 656e 7472 6965 7320  lt some entries 
-000003f0: 6861 6420 746f 2062 6520 7265 6d6f 7665  had to be remove
-00000400: 642c 0a20 2062 6563 6175 7365 2074 6865  d,.  because the
-00000410: 7920 6469 6420 636f 6e74 6169 6e20 696e  y did contain in
-00000420: 7661 6c69 6420 6261 6e6b 2063 6f64 6573  valid bank codes
-00000430: 2e0a 2a20 5468 6520 4461 6e69 7368 206e  ..* The Danish n
-00000440: 6174 696f 6e61 6c20 6368 6563 6b73 756d  ational checksum
-00000450: 2061 6c67 6f72 6974 686d 2069 7320 636f   algorithm is co
-00000460: 6e73 6964 6572 6564 206f 7061 7175 6520  nsidered opaque 
-00000470: 616e 6420 7468 6520 6368 6563 6b73 756d  and the checksum
-00000480: 2064 6967 6974 2069 7320 6173 7375 6d65   digit is assume
-00000490: 6420 746f 0a20 2062 6520 7061 7274 206f  d to.  be part o
-000004a0: 6620 7468 6520 6163 636f 756e 7420 6e75  f the account nu
-000004b0: 6d62 6572 2028 7768 6963 6820 6973 206e  mber (which is n
-000004c0: 6f77 2061 6c77 6179 7320 3130 2064 6967  ow always 10 dig
-000004d0: 6974 7320 6c6f 6e67 292e 0a0a 4669 7865  its long)...Fixe
-000004e0: 640a 7e7e 7e7e 7e0a 2a20 5468 6520 437a  d.~~~~~.* The Cz
-000004f0: 6563 6820 6261 6e6b 2072 6567 6973 7472  ech bank registr
-00000500: 7920 7761 7320 7374 6f72 6564 2069 6e20  y was stored in 
-00000510: 6c61 7469 6e2d 3120 656e 636f 6469 6e67  latin-1 encoding
-00000520: 2077 6869 6c65 2062 6569 6e67 2072 6561   while being rea
-00000530: 6420 6173 2055 5446 2d38 2e20 5468 6973  d as UTF-8. This
-00000540: 2072 6573 756c 7465 640a 2020 696e 2069   resulted.  in i
-00000550: 6e76 616c 6964 2062 616e 6b20 6e61 6d65  nvalid bank name
-00000560: 7320 6040 4e61 7469 6d20 3c68 7474 7073  s `@Natim <https
-00000570: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e61  ://github.com/Na
-00000580: 7469 6d3e 605f 2061 6e64 0a20 2060 4043  tim>`_ and.  `@C
-00000590: 6f67 6178 203c 6874 7470 733a 2f2f 6769  ogax <https://gi
-000005a0: 7468 7562 2e63 6f6d 2f43 6f67 6178 3e60  thub.com/Cogax>`
-000005b0: 5f2e 0a2a 2054 6865 204e 6f72 7765 6769  _..* The Norwegi
-000005c0: 616e 206e 6174 696f 6e61 6c20 6368 6563  an national chec
-000005d0: 6b73 756d 2061 6c67 6f72 6974 686d 2077  ksum algorithm w
-000005e0: 6173 2072 656e 6465 7269 6e67 2077 726f  as rendering wro
-000005f0: 6e67 2072 6573 756c 7473 2069 6e20 736f  ng results in so
-00000600: 6d65 2065 6467 652d 6361 7365 730a 2020  me edge-cases.  
-00000610: 6040 4e61 7469 6d20 3c68 7474 7073 3a2f  `@Natim <https:/
-00000620: 2f67 6974 6875 622e 636f 6d2f 4e61 7469  /github.com/Nati
-00000630: 6d3e 605f 0a0a 0a0a 6032 3032 342e 3031  m>`_....`2024.01
-00000640: 2e31 605f 202d 2032 3032 342f 3031 2f30  .1`_ - 2024/01/0
-00000650: 350a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  5.--------------
-00000660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 4164 6465  -----------.Adde
-00000670: 640a 7e7e 7e7e 7e0a 0a2a 2053 7570 706f  d.~~~~~..* Suppo
-00000680: 7274 2061 7370 6972 6174 696f 6e61 6c20  rt aspirational 
-00000690: 636f 756e 7472 6965 733a 0a0a 2020 2a20  countries:..  * 
-000006a0: 416c 6765 7269 610a 2020 2a20 416e 676f  Algeria.  * Ango
-000006b0: 6c61 0a20 202a 2042 656e 696e 0a20 202a  la.  * Benin.  *
-000006c0: 2042 7572 6b69 6e61 2046 6173 6f0a 2020   Burkina Faso.  
-000006d0: 2a20 4275 7275 6e64 690a 2020 2a20 4361  * Burundi.  * Ca
-000006e0: 626f 2056 6572 6465 0a20 202a 2043 616d  bo Verde.  * Cam
-000006f0: 6572 6f6f 6e0a 2020 2a20 4365 6e74 7261  eroon.  * Centra
-00000700: 6c20 4166 7269 6361 6e20 5265 7075 626c  l African Republ
-00000710: 6963 0a20 202a 2043 6861 640a 2020 2a20  ic.  * Chad.  * 
-00000720: 436f 6d6f 726f 730a 2020 2a20 436f 6e67  Comoros.  * Cong
-00000730: 6f0a 2020 2a20 43c3 b474 6520 6427 4976  o.  * C..te d'Iv
-00000740: 6f69 7265 0a20 202a 2044 6a69 626f 7574  oire.  * Djibout
-00000750: 690a 2020 2a20 4571 7561 746f 7269 616c  i.  * Equatorial
-00000760: 2047 7569 6e65 610a 2020 2a20 4761 626f   Guinea.  * Gabo
-00000770: 6e2c 0a20 202a 2047 7569 6e65 612d 4269  n,.  * Guinea-Bi
-00000780: 7373 6175 0a20 202a 2048 6f6e 6475 7261  ssau.  * Hondura
-00000790: 730a 2020 2a20 4972 616e 0a20 202a 204d  s.  * Iran.  * M
-000007a0: 6164 6167 6173 6361 720a 2020 2a20 4d61  adagascar.  * Ma
-000007b0: 6c69 0a20 202a 204d 6f72 6f63 636f 0a20  li.  * Morocco. 
-000007c0: 202a 204d 6f7a 616d 6269 7175 650a 2020   * Mozambique.  
-000007d0: 2a20 4e69 6361 7261 6775 610a 2020 2a20  * Nicaragua.  * 
-000007e0: 4e69 6765 720a 2020 2a20 5365 6e65 6761  Niger.  * Senega
-000007f0: 6c0a 2020 2a20 546f 676f 0a0a 2a20 4e61  l.  * Togo..* Na
-00000800: 7469 6f6e 616c 2063 6865 636b 7375 6d20  tional checksum 
-00000810: 616c 676f 7269 7468 6d73 2066 6f72 206d  algorithms for m
-00000820: 616e 7920 636f 756e 7472 6965 7320 6861  any countries ha
-00000830: 7665 2062 6565 6e20 6164 6465 643a 0a0a  ve been added:..
-00000840: 2020 2a20 416c 6261 6e69 610a 2020 2a20    * Albania.  * 
-00000850: 426f 736e 6961 2061 6e64 2048 6572 7a65  Bosnia and Herze
-00000860: 676f 7669 6e61 0a20 202a 2043 7a65 6368  govina.  * Czech
-00000870: 2052 6570 7562 6c69 630a 2020 2a20 4561   Republic.  * Ea
-00000880: 7374 2054 696d 6f72 0a20 202a 2045 7374  st Timor.  * Est
-00000890: 6f6e 6961 0a20 202a 2046 696e 6c61 6e64  onia.  * Finland
-000008a0: 0a20 202a 2049 6365 6c61 6e64 0a20 202a  .  * Iceland.  *
-000008b0: 204d 6175 7269 7461 6e69 610a 2020 2a20   Mauritania.  * 
-000008c0: 4d6f 6e74 656e 6567 726f 0a20 202a 204e  Montenegro.  * N
-000008d0: 6f72 7468 204d 6163 6564 6f6e 6961 0a20  orth Macedonia. 
-000008e0: 202a 204e 6f72 7761 790a 2020 2a20 506f   * Norway.  * Po
-000008f0: 6c61 6e64 0a20 202a 2050 6f72 7475 6761  land.  * Portuga
-00000900: 6c0a 2020 2a20 5365 7262 6961 0a20 202a  l.  * Serbia.  *
-00000910: 2053 6c6f 7661 6b69 610a 2020 2a20 536c   Slovakia.  * Sl
-00000920: 6f76 656e 6961 0a20 202a 2053 7061 696e  ovenia.  * Spain
-00000930: 0a20 202a 2054 756e 6973 6961 0a0a 2a20  .  * Tunisia..* 
-00000940: 4164 6420 6e65 7720 6261 6e6b 7320 746f  Add new banks to
-00000950: 2074 6865 206c 6973 7420 6f66 2046 7265   the list of Fre
-00000960: 6e63 6820 6261 6e6b 7320 6040 4e61 7469  nch banks `@Nati
-00000970: 6d20 3c68 7474 7073 3a2f 2f67 6974 6875  m <https://githu
-00000980: 622e 636f 6d2f 4e61 7469 6d3e 605f 3a0a  b.com/Natim>`_:.
-00000990: 0a20 202a 2041 524b 4541 2042 5020 4272  .  * ARKEA BP Br
-000009a0: 6573 740a 2020 2a20 416e 7974 696d 650a  est.  * Anytime.
-000009b0: 2020 2a20 4c79 6469 6120 4261 6e6b 0a20    * Lydia Bank. 
-000009c0: 202a 204d 454d 4f20 4241 4e4b 0a20 202a   * MEMO BANK.  *
-000009d0: 2052 6576 6f6c 7574 0a20 202a 2053 4849   Revolut.  * SHI
-000009e0: 4e45 0a20 202a 2053 756d 5570 204c 696d  NE.  * SumUp Lim
-000009f0: 6974 6564 0a0a 2a20 4e65 7720 3a61 7474  ited..* New :att
-00000a00: 723a 602e 4942 414e 2e69 6e5f 7365 7061  r:`.IBAN.in_sepa
-00000a10: 5f7a 6f6e 6560 2d70 726f 7065 7274 7920  _zone`-property 
-00000a20: 746f 2069 6e64 6963 6174 6520 6966 2074  to indicate if t
-00000a30: 6865 2049 4241 4e27 7320 636f 756e 7472  he IBAN's countr
-00000a40: 7920 6973 2070 6172 7420 6f66 2074 6865  y is part of the
-00000a50: 2053 4550 410a 2020 7a6f 6e65 2e0a 2a20   SEPA.  zone..* 
-00000a60: 4e65 7720 6d61 6e75 616c 2062 616e 6b20  New manual bank 
-00000a70: 7265 6769 7374 7269 6573 2066 6f72 0a0a  registries for..
-00000a80: 2020 2a20 416e 646f 7272 610a 2020 2a20    * Andorra.  * 
-00000a90: 4172 6162 6963 2045 6d69 7261 7465 730a  Arabic Emirates.
-00000aa0: 2020 2a20 436f 7374 6120 5269 6361 0a20    * Costa Rica. 
-00000ab0: 202a 2050 6f72 7475 6761 6c0a 0a2a 204e   * Portugal..* N
-00000ac0: 6577 2061 7474 7269 6275 7465 7320 3a61  ew attributes :a
-00000ad0: 7474 723a 602e 4942 414e 2e61 6363 6f75  ttr:`.IBAN.accou
-00000ae0: 6e74 5f69 6460 2c20 3a61 7474 723a 602e  nt_id`, :attr:`.
-00000af0: 4942 414e 2e61 6363 6f75 6e74 5f68 6f6c  IBAN.account_hol
-00000b00: 6465 725f 6964 6020 616e 640a 2020 3a61  der_id` and.  :a
-00000b10: 7474 723a 602e 4942 414e 2e61 6363 6f75  ttr:`.IBAN.accou
-00000b20: 6e74 5f74 7970 6560 2074 6861 7420 6172  nt_type` that ar
-00000b30: 6520 6176 6169 6c61 626c 6520 6465 7065  e available depe
-00000b40: 6e64 696e 6720 6f6e 2074 6865 2063 6f75  nding on the cou
-00000b50: 6e74 7279 2773 2042 4241 4e20 7370 6563  ntry's BBAN spec
-00000b60: 6966 6963 6174 696f 6e2e 0a20 2045 2e67  ification..  E.g
-00000b70: 2e20 3a61 7474 723a 602e 4942 414e 2e61  . :attr:`.IBAN.a
-00000b80: 6363 6f75 6e74 5f68 6f6c 6465 725f 6964  ccount_holder_id
-00000b90: 6020 6973 2063 7572 7265 6e74 6c79 206f  ` is currently o
-00000ba0: 6e6c 7920 6176 6169 6c61 626c 6520 666f  nly available fo
-00000bb0: 7220 4963 656c 616e 6420 284b 656e 6e69  r Iceland (Kenni
-00000bc0: 7461 6c61 2920 616e 6420 6f6e 6c79 0a20  tala) and only. 
-00000bd0: 2042 7261 7a69 6c20 6465 6669 6e65 7320   Brazil defines 
-00000be0: 616e 203a 6174 7472 3a60 2e49 4241 4e2e  an :attr:`.IBAN.
-00000bf0: 6163 636f 756e 745f 6964 602e 0a0a 4368  account_id`...Ch
-00000c00: 616e 6765 640a 7e7e 7e7e 7e7e 7e0a 2a20  anged.~~~~~~~.* 
-00000c10: 5573 6520 656e 6861 6e63 6564 2049 4241  Use enhanced IBA
-00000c20: 4e2f 4242 414e 2066 6f72 6d61 7420 6672  N/BBAN format fr
-00000c30: 6f6d 2060 5769 6b69 7065 6469 6120 3c68  om `Wikipedia <h
-00000c40: 7474 7073 3a2f 2f65 6e2e 7769 6b69 7065  ttps://en.wikipe
-00000c50: 6469 612e 6f72 672f 7769 6b69 2f49 6e74  dia.org/wiki/Int
-00000c60: 6572 6e61 7469 6f6e 616c 5f42 616e 6b5f  ernational_Bank_
-00000c70: 4163 636f 756e 745f 4e75 6d62 6572 2349  Account_Number#I
-00000c80: 4241 4e5f 666f 726d 6174 735f 6279 5f63  BAN_formats_by_c
-00000c90: 6f75 6e74 7279 3e60 5f2c 0a20 2073 696e  ountry>`_,.  sin
-00000ca0: 6365 2074 6865 206f 6666 6963 6961 6c20  ce the official 
-00000cb0: 696e 666f 726d 6174 696f 6e20 6672 6f6d  information from
-00000cc0: 2053 5749 4654 2069 7320 6f66 7465 6e20   SWIFT is often 
-00000cd0: 696e 6163 7572 6174 652e 0a2a 2054 6865  inacurate..* The
-00000ce0: 2073 7570 706f 7274 2066 6f72 206e 6174   support for nat
-00000cf0: 696f 6e61 6c20 6368 6563 6b73 756d 2064  ional checksum d
-00000d00: 6967 6974 7320 6861 7320 6265 656e 2072  igits has been r
-00000d10: 6569 6d70 6c65 6d65 6e74 6564 2e0a 2a20  eimplemented..* 
-00000d20: 5468 6520 3a63 6c61 7373 3a60 2e49 4241  The :class:`.IBA
-00000d30: 4e60 2d63 6c61 7373 206e 6f77 2068 6173  N`-class now has
-00000d40: 2061 6e20 6164 6469 7469 6f6e 616c 203a   an additional :
-00000d50: 6174 7472 3a60 2e49 4241 4e2e 6262 616e  attr:`.IBAN.bban
-00000d60: 602d 6174 7472 6962 7574 652c 2077 6865  `-attribute, whe
-00000d70: 7265 2061 6c6c 2063 6f75 6e74 7279 0a20  re all country. 
-00000d80: 2073 7065 6369 6669 6320 6675 6e63 7469   specific functi
-00000d90: 6f6e 616c 6974 7920 6861 7320 6265 656e  onality has been
-00000da0: 206d 6f76 6564 2074 6f2e 0a2a 2055 7064   moved to..* Upd
-00000db0: 6174 6564 2062 616e 6b20 7265 6769 7374  ated bank regist
-00000dc0: 7269 6573 2e20 5468 616e 6b73 2074 6f20  ries. Thanks to 
-00000dd0: 6040 7368 3464 6f77 6220 3c68 7474 7073  `@sh4dowb <https
-00000de0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7368  ://github.com/sh
-00000df0: 3464 6f77 623e 605f 2066 6f72 2074 6865  4dowb>`_ for the
-00000e00: 2054 7572 6b69 7368 2062 616e 6b73 2e0a   Turkish banks..
-00000e10: 0a0a 6032 3032 332e 3131 2e32 605f 202d  ..`2023.11.2`_ -
-00000e20: 2032 3032 332f 3131 2f32 370a 2d2d 2d2d   2023/11/27.----
-00000e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e40: 2d2d 2d2d 2d0a 4164 6465 640a 7e7e 7e7e  -----.Added.~~~~
-00000e50: 7e0a 2a20 4164 6420 4f4b 414c 4920 746f  ~.* Add OKALI to
-00000e60: 2074 6865 206c 6973 7420 6f66 2046 7265   the list of Fre
-00000e70: 6e63 6820 6261 6e6b 7320 6040 4e61 7469  nch banks `@Nati
-00000e80: 6d20 3c68 7474 7073 3a2f 2f67 6974 6875  m <https://githu
-00000e90: 622e 636f 6d2f 4e61 7469 6d3e 605f 2e0a  b.com/Natim>`_..
-00000ea0: 0a60 3230 3233 2e31 312e 3160 5f20 2d20  .`2023.11.1`_ - 
-00000eb0: 3230 3233 2f31 312f 3237 0a2d 2d2d 2d2d  2023/11/27.-----
-00000ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ed0: 2d2d 2d2d 0a43 6861 6e67 6564 0a7e 7e7e  ----.Changed.~~~
-00000ee0: 7e7e 7e7e 0a2a 2054 6865 2053 7769 7373  ~~~~.* The Swiss
-00000ef0: 2062 616e 6b20 7265 6769 7374 7279 2069   bank registry i
-00000f00: 7320 6e6f 7720 6765 6e65 7261 7465 6420  s now generated 
-00000f10: 6672 6f6d 2074 6865 2053 4958 2047 726f  from the SIX Gro
-00000f20: 7570 2e0a 2a20 4d61 6e75 616c 6c79 2061  up..* Manually a
-00000f30: 6464 206d 6973 7369 6e67 2062 616e 6b20  dd missing bank 
-00000f40: 656e 7472 7920 666f 7220 5370 6169 6e2e  entry for Spain.
-00000f50: 0a2a 2055 7064 6174 6564 2062 616e 6b20  .* Updated bank 
-00000f60: 7265 6769 7374 7220 666f 7220 4175 7374  registr for Aust
-00000f70: 7269 6120 616e 6420 506f 6c61 6e64 2e0a  ria and Poland..
-00000f80: 0a60 3230 3233 2e31 312e 3060 5f20 2d20  .`2023.11.0`_ - 
-00000f90: 3230 3233 2f31 312f 3137 0a2d 2d2d 2d2d  2023/11/17.-----
-00000fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000fb0: 2d2d 2d2d 0a43 6861 6e67 6564 0a7e 7e7e  ----.Changed.~~~
-00000fc0: 7e7e 7e7e 0a2a 2054 6865 2076 616c 6964  ~~~~.* The valid
-00000fd0: 6174 696f 6e20 6f66 2061 203a 636c 6173  ation of a :clas
-00000fe0: 733a 602e 4249 4360 2069 7320 6e6f 7720  s:`.BIC` is now 
-00000ff0: 7065 7266 6f72 6d65 6420 696e 2074 6865  performed in the
-00001000: 2063 6f6e 7465 7874 206f 6620 4953 4f20   context of ISO 
-00001010: 3933 3632 3a32 3032 3220 7768 6963 6820  9362:2022 which 
-00001020: 616c 6c6f 7773 0a20 206e 756d 6265 7273  allows.  numbers
-00001030: 2069 6e20 7468 6520 6275 7369 6e65 7373   in the business
-00001040: 2070 6172 7479 2070 7265 6669 782e 2049   party prefix. I
-00001050: 6620 7374 7269 6374 2053 5749 4654 2063  f strict SWIFT c
-00001060: 6f6d 706c 6961 6e63 6520 6973 2072 6571  ompliance is req
-00001070: 7275 6965 6420 7468 650a 2020 6060 656e  ruied the.  ``en
-00001080: 666f 7263 655f 7377 6966 745f 636f 6d70  force_swift_comp
-00001090: 6c69 616e 6365 6060 2070 6172 616d 6574  liance`` paramet
-000010a0: 6572 2063 616e 2062 6520 7365 7420 746f  er can be set to
-000010b0: 2060 6054 7275 6560 602e 0a2a 2054 6865   ``True``..* The
-000010c0: 203a 6d65 7468 3a60 2e42 4943 2e66 726f   :meth:`.BIC.fro
-000010d0: 6d5f 6261 6e6b 5f63 6f64 6560 2d6d 6574  m_bank_code`-met
-000010e0: 686f 6420 7769 6c6c 206e 6f77 2073 656c  hod will now sel
-000010f0: 6563 7420 7468 6520 6d6f 7374 2067 656e  ect the most gen
-00001100: 6572 6963 2042 4943 2028 652e 672e 2077  eric BIC (e.g. w
-00001110: 6974 6820 6e6f 2062 7261 6e63 680a 2020  ith no branch.  
-00001120: 7370 6563 6966 6965 7220 6f72 2074 6865  specifier or the
-00001130: 2022 5858 5822 2076 616c 7565 2920 6966   "XXX" value) if
-00001140: 206d 756c 7469 706c 6520 4249 4373 2061   multiple BICs a
-00001150: 7265 2061 7373 6f63 6961 7465 6420 746f  re associated to
-00001160: 2074 6865 2067 6976 656e 2064 6f6d 6573   the given domes
-00001170: 7469 6320 6261 6e6b 2063 6f64 652e 0a20  tic bank code.. 
-00001180: 2060 404e 6174 696d 203c 6874 7470 733a   `@Natim <https:
-00001190: 2f2f 6769 7468 7562 2e63 6f6d 2f4e 6174  //github.com/Nat
-000011a0: 696d 3e60 5f2e 0a2a 204d 616e 7920 6d61  im>`_..* Many ma
-000011b0: 6e75 616c 6c79 2063 7572 6174 6564 2062  nually curated b
-000011c0: 616e 6b20 7265 6769 7374 7279 2065 6e74  ank registry ent
-000011d0: 7269 6573 2068 6176 6520 6265 656e 2072  ries have been r
-000011e0: 652d 6164 6465 6420 6279 2060 4064 656e  e-added by `@den
-000011f0: 6e69 7378 7472 6961 203c 6874 7470 733a  nisxtria <https:
-00001200: 2f2f 6769 7468 7562 2e63 6f6d 2f64 656e  //github.com/den
-00001210: 6e69 7378 7472 6961 3e60 5f0a 0a60 3230  nisxtria>`_..`20
-00001220: 3233 2e31 302e 3060 5f20 2d20 3230 3233  23.10.0`_ - 2023
-00001230: 2f31 302f 3331 0a2d 2d2d 2d2d 2d2d 2d2d  /10/31.---------
-00001240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001250: 0a41 6464 6564 0a7e 7e7e 7e7e 7e7e 0a2a  .Added.~~~~~~~.*
-00001260: 2054 6865 2050 7964 616e 7469 6320 7632   The Pydantic v2
-00001270: 2070 726f 746f 636f 6c20 6973 206e 6f77   protocol is now
-00001280: 2073 7570 706f 7274 6564 2c20 736f 2074   supported, so t
-00001290: 6861 7420 7468 6520 3a63 6c61 7373 3a60  hat the :class:`
-000012a0: 2e49 4241 4e60 2061 6e64 203a 636c 6173  .IBAN` and :clas
-000012b0: 733a 602e 4249 4360 2063 6c61 7373 6573  s:`.BIC` classes
-000012c0: 0a20 2063 616e 2062 6520 6469 7265 6374  .  can be direct
-000012d0: 6c79 2075 7365 6420 6173 2074 7970 6520  ly used as type 
-000012e0: 616e 6e6f 7461 7469 6f6e 7320 696e 2060  annotations in `
-000012f0: 5079 6461 6e74 6963 206d 6f64 656c 7320  Pydantic models 
-00001300: 3c68 7474 7073 3a2f 2f64 6f63 732e 7079  <https://docs.py
-00001310: 6461 6e74 6963 2e64 6576 2f6c 6174 6573  dantic.dev/lates
-00001320: 742f 636f 6e63 6570 7473 2f6d 6f64 656c  t/concepts/model
-00001330: 732f 2362 6173 6963 2d6d 6f64 656c 2d75  s/#basic-model-u
-00001340: 7361 6765 3e60 5f0a 0a43 6861 6e67 6564  sage>`_..Changed
-00001350: 0a7e 7e7e 7e7e 7e7e 0a2a 2054 6865 203a  .~~~~~~~.* The :
-00001360: 636c 6173 733a 602e 4942 414e 6020 616e  class:`.IBAN` an
-00001370: 6420 3a63 6c61 7373 3a60 2e42 4943 6020  d :class:`.BIC` 
-00001380: 636c 6173 7365 7320 6172 6520 6e6f 7720  classes are now 
-00001390: 7375 6263 6c61 7373 6573 206f 6620 3a63  subclasses of :c
-000013a0: 6c61 7373 3a60 7374 7260 2073 6f20 7468  lass:`str` so th
-000013b0: 6174 2061 6c6c 2073 7472 696e 670a 2020  at all string.  
-000013c0: 7265 6c61 7465 6420 6d65 7468 6f64 7320  related methods 
-000013d0: 616e 6420 6675 6e63 7469 6f6e 616c 6c69  and functionalli
-000013e0: 7469 6573 2028 652e 672e 2073 6c69 6369  ties (e.g. slici
-000013f0: 6e67 2920 6172 6520 6469 7265 6374 6c79  ng) are directly
-00001400: 2061 7661 696c 6162 6c65 2e0a 0a60 3230   available...`20
-00001410: 3233 2e30 392e 3060 5f20 2d20 3230 3233  23.09.0`_ - 2023
-00001420: 2f30 392f 3235 0a2d 2d2d 2d2d 2d2d 2d2d  /09/25.---------
-00001430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001440: 0a52 656d 6f76 6564 0a7e 7e7e 7e7e 7e7e  .Removed.~~~~~~~
-00001450: 0a2a 2053 7570 706f 7274 2066 6f72 2050  .* Support for P
-00001460: 7974 686f 6e20 332e 3720 6861 7320 6265  ython 3.7 has be
-00001470: 656e 2064 726f 7070 6564 2e0a 0a41 6464  en dropped...Add
-00001480: 6564 0a7e 7e7e 7e7e 0a2a 204e 6577 206d  ed.~~~~~.* New m
-00001490: 6574 686f 6420 3a6d 6574 683a 602e 4249  ethod :meth:`.BI
-000014a0: 432e 6361 6e64 6964 6174 6573 5f66 726f  C.candidates_fro
-000014b0: 6d5f 6261 6e6b 5f63 6f64 6560 2074 6f20  m_bank_code` to 
-000014c0: 6c69 7374 2061 6c6c 206d 6174 6368 696e  list all matchin
-000014d0: 6720 4249 4373 2074 6f20 6120 6769 7665  g BICs to a give
-000014e0: 6e20 646f 6d65 7374 6963 0a20 2062 616e  n domestic.  ban
-000014f0: 6b20 636f 6465 2060 404e 6174 696d 203c  k code `@Natim <
-00001500: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001510: 6f6d 2f4e 6174 696d 3e60 5f2e 0a0a 4368  om/Natim>`_...Ch
-00001520: 616e 6765 640a 7e7e 7e7e 7e7e 7e0a 2a20  anged.~~~~~~~.* 
-00001530: 5468 6520 4974 616c 6961 6e20 6261 6e6b  The Italian bank
-00001540: 2072 6567 6973 7472 7920 6973 206e 6f77   registry is now
-00001550: 2061 7574 6f6d 6174 6963 616c 6c79 2067   automatically g
-00001560: 656e 6572 6174 6564 2074 6861 6e6b 7320  enerated thanks 
-00001570: 746f 0a20 2060 404b 7279 7374 6f66 6565  to.  `@Krystofee
-00001580: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00001590: 2e63 6f6d 2f4b 7279 7374 6f66 6565 3e60  .com/Krystofee>`
-000015a0: 5f0a 0a49 6e74 6572 6e61 6c0a 7e7e 7e7e  _..Internal.~~~~
-000015b0: 7e7e 7e7e 0a2a 2053 7769 7463 6820 7072  ~~~~.* Switch pr
-000015c0: 6f6a 6563 7420 746f 6f6c 696e 6720 746f  oject tooling to
-000015d0: 2060 6861 7463 6820 3c68 7474 7073 3a2f   `hatch <https:/
-000015e0: 2f68 6174 6368 2e70 7970 612e 696f 2f6c  /hatch.pypa.io/l
-000015f0: 6174 6573 742f 3e60 5f2e 0a2a 2055 7365  atest/>`_..* Use
-00001600: 2060 7275 6666 203c 6874 7470 733a 2f2f   `ruff <https://
-00001610: 646f 6373 2e61 7374 7261 6c2e 7368 2f72  docs.astral.sh/r
-00001620: 7566 662f 3e60 5f20 696e 7374 6561 6420  uff/>`_ instead 
-00001630: 6f66 205b 666c 616b 6538 5d28 6874 7470  of [flake8](http
-00001640: 733a 2f2f 666c 616b 6538 2e70 7963 7161  s://flake8.pycqa
-00001650: 2e6f 7267 2f65 6e2f 6c61 7465 7374 2f29  .org/en/latest/)
-00001660: 0a20 2061 7320 6c69 6e74 6572 2e0a 2a20  .  as linter..* 
-00001670: 5570 6772 6164 6520 606d 7970 7920 3c68  Upgrade `mypy <h
-00001680: 7474 7073 3a2f 2f77 7777 2e6d 7970 792d  ttps://www.mypy-
-00001690: 6c61 6e67 2e6f 7267 2f3e 605f 2074 6f20  lang.org/>`_ to 
-000016a0: 312e 352e 3120 616e 6420 6669 7820 616c  1.5.1 and fix al
-000016b0: 6c20 6e65 7720 7479 7069 6e67 2065 7272  l new typing err
-000016c0: 6f72 732e 0a0a 6032 3032 332e 3036 2e30  ors...`2023.06.0
-000016d0: 605f 202d 2032 3032 332f 3036 2f32 310a  `_ - 2023/06/21.
-000016e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000016f0: 2d2d 2d2d 2d2d 2d2d 2d0a 4669 7865 640a  ---------.Fixed.
-00001700: 7e7e 7e7e 7e0a 2a20 466f 7220 556b 7261  ~~~~~.* For Ukra
-00001710: 696e 6961 6e20 6261 6e6b 7320 6361 6c6c  inian banks call
-00001720: 696e 6720 6060 6962 616e 2e62 6963 6060  ing ``iban.bic``
-00001730: 2064 6964 2072 6573 756c 7420 696e 2061   did result in a
-00001740: 2060 6054 7970 6545 7272 6f72 6060 2e20   ``TypeError``. 
-00001750: 5468 616e 6b73 0a20 2060 4062 6572 6e6f  Thanks.  `@berno
-00001760: 7265 6974 736d 6120 3c68 7474 7073 3a2f  reitsma <https:/
-00001770: 2f67 6974 6875 622e 636f 6d2f 6265 726e  /github.com/bern
-00001780: 6f72 6569 7473 6d61 3e60 5f20 666f 7220  oreitsma>`_ for 
-00001790: 7265 706f 7274 696e 672e 0a0a 4368 616e  reporting...Chan
-000017a0: 6765 640a 7e7e 7e7e 7e7e 7e0a 2a20 5570  ged.~~~~~~~.* Up
-000017b0: 6461 7465 6420 6765 6e65 7261 7465 6420  dated generated 
-000017c0: 6261 6e6b 2072 6567 6973 7472 6965 7320  bank registries 
-000017d0: 666f 7220 4175 7374 7269 612c 2042 656c  for Austria, Bel
-000017e0: 6769 756d 2c20 437a 6563 6820 5265 7075  gium, Czech Repu
-000017f0: 626c 6963 2c20 4765 726d 616e 792c 204e  blic, Germany, N
-00001800: 6574 6865 726c 616e 6473 2c0a 2020 4875  etherlands,.  Hu
-00001810: 6e67 6172 792c 204e 6f72 7761 792c 2050  ngary, Norway, P
-00001820: 6f6c 616e 6420 616e 6420 556b 7261 696e  oland and Ukrain
-00001830: 652e 0a0a 0a60 3230 3233 2e30 332e 3060  e....`2023.03.0`
-00001840: 5f20 2d20 3230 3233 2f30 332f 3134 0a2d  _ - 2023/03/14.-
-00001850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001860: 2d2d 2d2d 2d2d 2d2d 0a43 6861 6e67 6564  --------.Changed
-00001870: 0a7e 7e7e 7e7e 7e7e 0a2a 2055 7064 6174  .~~~~~~~.* Updat
-00001880: 6564 2067 656e 6572 6174 6564 2062 616e  ed generated ban
-00001890: 6b20 7265 6769 7374 7269 6573 2066 6f72  k registries for
-000018a0: 2041 7573 7472 6961 2c20 4265 6c67 6975   Austria, Belgiu
-000018b0: 6d2c 2047 6572 6d61 6e79 2c20 4e65 7468  m, Germany, Neth
-000018c0: 6572 6c61 6e64 732c 0a20 2048 756e 6761  erlands,.  Hunga
-000018d0: 7279 2c20 536c 6f76 656e 6961 2061 6e64  ry, Slovenia and
-000018e0: 2055 6b72 6169 6e65 2e0a 0a41 6464 6564   Ukraine...Added
-000018f0: 0a7e 7e7e 7e7e 0a2a 204e 6577 2062 616e  .~~~~~.* New ban
-00001900: 6b20 7265 6769 7374 7279 2066 6f72 204e  k registry for N
-00001910: 6f72 7761 7920 7468 616e 6b73 2074 6f20  orway thanks to 
-00001920: 6040 657a 6574 203c 6874 7470 733a 2f2f  `@ezet <https://
-00001930: 6769 7468 7562 2e63 6f6d 2f65 7a65 743e  github.com/ezet>
-00001940: 605f 0a0a 6032 3032 332e 3032 2e31 605f  `_..`2023.02.1`_
-00001950: 202d 2032 3032 332f 3032 2f32 380a 2d2d   - 2023/02/28.--
-00001960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001970: 2d2d 2d2d 2d2d 2d0a 4669 7865 640a 7e7e  -------.Fixed.~~
-00001980: 7e7e 7e0a 2a20 5468 6520 646f 6d65 7374  ~~~.* The domest
-00001990: 6963 2063 6865 636b 7375 6d20 6361 6c63  ic checksum calc
-000019a0: 756c 6174 696f 6e20 666f 7220 4265 6c67  ulation for Belg
-000019b0: 6975 6d20 6e6f 7720 7265 7475 726e 7320  ium now returns 
-000019c0: 3937 2069 6e20 6361 7365 2074 6865 206d  97 in case the m
-000019d0: 6f64 756c 6f20 6f70 6572 6174 696f 6e0a  odulo operation.
-000019e0: 2020 7265 7375 6c74 7320 696e 2030 2e20    results in 0. 
-000019f0: 6040 6d68 656d 6572 7963 6b20 3c68 7474  `@mhemeryck <htt
-00001a00: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001a10: 6d68 656d 6572 7963 6b3e 605f 0a0a 4368  mhemeryck>`_..Ch
-00001a20: 616e 6765 640a 7e7e 7e7e 7e7e 7e0a 2a20  anged.~~~~~~~.* 
-00001a30: 5570 6461 7465 6420 6765 6e65 7261 7465  Updated generate
-00001a40: 6420 6261 6e6b 2072 6567 6973 7472 6965  d bank registrie
-00001a50: 7320 666f 7220 4175 7374 7269 612c 2042  s for Austria, B
-00001a60: 656c 6769 756d 2c20 437a 6563 6820 5265  elgium, Czech Re
-00001a70: 7075 626c 6963 2c20 4765 726d 616e 792c  public, Germany,
-00001a80: 2053 7061 696e 2c0a 2020 4875 6e67 6172   Spain,.  Hungar
-00001a90: 7920 616e 6420 4372 6f61 7469 612e 0a0a  y and Croatia...
-00001aa0: 6032 3032 332e 3032 2e30 605f 202d 2032  `2023.02.0`_ - 2
-00001ab0: 3032 332f 3032 2f30 360a 2d2d 2d2d 2d2d  023/02/06.------
-00001ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001ad0: 2d2d 2d0a 4164 6465 640a 7e7e 7e7e 7e0a  ---.Added.~~~~~.
-00001ae0: 2a20 4e65 7720 6261 6e6b 7320 666f 7220  * New banks for 
-00001af0: 506f 7274 7567 616c 2061 6e64 2049 7461  Portugal and Ita
-00001b00: 6c79 2060 4064 656e 6e69 7378 7472 6961  ly `@dennisxtria
-00001b10: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00001b20: 2e63 6f6d 2f64 656e 6e69 7378 7472 6961  .com/dennisxtria
-00001b30: 3e60 5f0a 2a20 4164 6465 6420 7375 7070  >`_.* Added supp
-00001b40: 6f72 7420 666f 7220 556b 7261 696e 6961  ort for Ukrainia
-00001b50: 6e20 6261 6e6b 7320 6040 7368 7069 6775  n banks `@shpigu
-00001b60: 6e6f 7620 3c68 7474 7073 3a2f 2f67 6974  nov <https://git
-00001b70: 6875 622e 636f 6d2f 7368 7069 6775 6e6f  hub.com/shpiguno
-00001b80: 763e 605f 0a0a 4669 7865 640a 7e7e 7e7e  v>`_..Fixed.~~~~
-00001b90: 7e0a 2a20 436f 7272 6563 7465 6420 6261  ~.* Corrected ba
-00001ba0: 6e6b 2063 6f64 6573 2066 6f72 2043 7970  nk codes for Cyp
-00001bb0: 7269 6f74 2062 616e 6b73 2060 404b 7279  riot banks `@Kry
-00001bc0: 7374 6f66 6565 203c 6874 7470 733a 2f2f  stofee <https://
-00001bd0: 6769 7468 7562 2e63 6f6d 2f4b 7279 7374  github.com/Kryst
-00001be0: 6f66 6565 3e60 5f0a 0a60 3230 3232 2e30  ofee>`_..`2022.0
-00001bf0: 392e 3060 5f20 2d20 3230 3232 2f31 362f  9.0`_ - 2022/16/
-00001c00: 3039 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  09.-------------
-00001c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a41 6464  ------------.Add
-00001c20: 6564 0a7e 7e7e 7e7e 0a2a 2049 4241 4e20  ed.~~~~~.* IBAN 
-00001c30: 7661 6c69 6461 7469 6f6e 2066 6f72 2053  validation for S
-00001c40: 656e 6567 616c 2060 6d6b 6f70 6563 3837  enegal `mkopec87
-00001c50: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00001c60: 2e63 6f6d 2f6d 6b6f 7065 6338 373e 605f  .com/mkopec87>`_
-00001c70: 0a0a 4368 616e 6765 640a 7e7e 7e7e 7e7e  ..Changed.~~~~~~
-00001c80: 7e0a 2a20 5265 6661 6374 6f72 6564 206d  ~.* Refactored m
-00001c90: 6f73 7420 6f66 2074 6865 2073 6372 6970  ost of the scrip
-00001ca0: 7473 2074 6f20 6765 6e65 7261 7465 2074  ts to generate t
-00001cb0: 6865 2062 616e 6b20 7265 6769 7374 7279  he bank registry
-00001cc0: 2074 6f20 7573 6520 5061 6e64 6173 2060   to use Pandas `
-00001cd0: 4070 6562 6f73 6920 3c68 7474 7073 3a2f  @pebosi <https:/
-00001ce0: 2f67 6974 6875 622e 636f 6d2f 7065 626f  /github.com/pebo
-00001cf0: 7369 3e60 5f0a 2a20 5570 6461 7465 6420  si>`_.* Updated 
-00001d00: 6261 6e6b 2072 6567 6973 7472 7920 666f  bank registry fo
-00001d10: 7220 4175 7374 7269 612c 2042 656c 6769  r Austria, Belgi
-00001d20: 756d 2c20 4765 726d 616e 792c 2053 7061  um, Germany, Spa
-00001d30: 696e 2c20 4875 6e67 6172 792c 204e 6574  in, Hungary, Net
-00001d40: 6865 726c 616e 6473 2061 6e64 2050 6f6c  herlands and Pol
-00001d50: 616e 642e 0a0a 6032 3032 322e 3037 2e31  and...`2022.07.1
-00001d60: 605f 202d 2032 3032 322f 3238 2f30 370a  `_ - 2022/28/07.
-00001d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001d80: 2d2d 2d2d 2d2d 2d2d 2d0a 4669 7865 640a  ---------.Fixed.
-00001d90: 7e7e 7e7e 7e0a 2a20 496e 2073 6f6d 6520  ~~~~~.* In some 
-00001da0: 636f 756e 7472 6965 7320 7468 6520 4242  countries the BB
-00001db0: 414e 2064 6f65 7320 6e6f 7420 696e 636c  AN does not incl
-00001dc0: 7564 6520 6120 6261 6e6b 2063 6f64 652c  ude a bank code,
-00001dd0: 2062 7574 206f 6e6c 7920 6120 6272 616e   but only a bran
-00001de0: 6368 2063 6f64 6520 2865 2e67 2e20 506f  ch code (e.g. Po
-00001df0: 6c61 6e64 292e 2049 6e0a 2020 7468 6f73  land). In.  thos
-00001e00: 6520 6361 7365 7320 7468 6520 6272 616e  e cases the bran
-00001e10: 6368 2063 6f64 6520 7368 6f75 6c64 2062  ch code should b
-00001e20: 6520 7573 6564 2074 6f20 6c6f 6f6b 7570  e used to lookup
-00001e30: 2074 6865 2062 616e 6b20 6173 736f 6369   the bank associ
-00001e40: 6174 6564 2074 6f20 616e 2049 4241 4e20  ated to an IBAN 
-00001e50: 696e 7374 6561 6420 6f66 2074 6865 0a20  instead of the. 
-00001e60: 206f 6276 696f 7573 6c79 2065 6d70 7479   obviously empty
-00001e70: 2062 616e 6b20 636f 6465 2e0a 0a60 3230   bank code...`20
-00001e80: 3232 2e30 372e 3060 5f20 2d20 3230 3232  22.07.0`_ - 2022
-00001e90: 2f30 372f 3037 0a2d 2d2d 2d2d 2d2d 2d2d  /07/07.---------
-00001ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001eb0: 0a46 6978 6564 0a7e 7e7e 7e7e 0a2a 2048  .Fixed.~~~~~.* H
-00001ec0: 756e 6761 7269 616e 2062 616e 6b20 7265  ungarian bank re
-00001ed0: 6769 7374 7279 2067 656e 6572 6174 6f72  gistry generator
-00001ee0: 2073 6372 6970 7420 7761 7320 6669 7865   script was fixe
-00001ef0: 6420 6279 2060 404b 7279 7374 6f66 6565  d by `@Krystofee
-00001f00: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00001f10: 2e63 6f6d 2f4b 7279 7374 6f66 6565 3e60  .com/Krystofee>`
-00001f20: 5f0a 0a60 3230 3232 2e30 362e 3360 5f20  _..`2022.06.3`_ 
-00001f30: 2d20 3230 3232 2f30 362f 3239 0a2d 2d2d  - 2022/06/29.---
-00001f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001f50: 2d2d 2d2d 2d2d 0a41 6464 6564 0a7e 7e7e  ------.Added.~~~
-00001f60: 7e7e 0a2a 2047 656e 6572 6174 6564 206c  ~~.* Generated l
-00001f70: 6973 7420 6f66 204c 6974 6875 616e 6961  ist of Lithuania
-00001f80: 6e20 4249 4373 2060 4044 7261 7567 656c  n BICs `@Draugel
-00001f90: 6973 203c 6874 7470 733a 2f2f 6769 7468  is <https://gith
-00001fa0: 7562 2e63 6f6d 2f44 7261 7567 656c 6973  ub.com/Draugelis
-00001fb0: 3e60 5f0a 2a20 5265 6d6f 7665 6420 6d61  >`_.* Removed ma
-00001fc0: 6e75 616c 6c79 2063 7572 6174 6564 206c  nually curated l
-00001fd0: 6973 7420 6f66 204c 6974 6875 616e 6961  ist of Lithuania
-00001fe0: 6e20 6261 6e6b 732e 0a0a 6032 3032 322e  n banks...`2022.
-00001ff0: 3036 2e32 605f 202d 2032 3032 322f 3036  06.2`_ - 2022/06
-00002000: 2f32 320a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /22.------------
-00002010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 4164  -------------.Ad
-00002020: 6465 640a 7e7e 7e7e 7e0a 2a20 4765 6e65  ded.~~~~~.* Gene
-00002030: 7261 7465 6420 6c69 7374 206f 6620 4772  rated list of Gr
-00002040: 6565 6b20 4249 4373 2060 406b 6f75 6e61  eek BICs `@kouna
-00002050: 6269 2020 3c68 7474 7073 3a2f 2f67 6974  bi  <https://git
-00002060: 6875 622e 636f 6d2f 6b6f 756e 6162 693e  hub.com/kounabi>
-00002070: 605f 0a2a 2047 656e 6572 6174 6564 206c  `_.* Generated l
-00002080: 6973 7420 6f66 2043 7970 7269 6f74 2042  ist of Cypriot B
-00002090: 4943 7320 6040 6b6f 756e 6162 6920 203c  ICs `@kounabi  <
-000020a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000020b0: 6f6d 2f6b 6f75 6e61 6269 3e60 5f0a 0a43  om/kounabi>`_..C
-000020c0: 6861 6e67 6564 0a7e 7e7e 7e7e 7e7e 0a2a  hanged.~~~~~~~.*
-000020d0: 2055 7064 6174 6564 2062 616e 6b20 7265   Updated bank re
-000020e0: 6769 7374 7279 2066 6f72 2041 7573 7472  gistry for Austr
-000020f0: 6961 2c20 4265 6c67 6975 6d2c 2043 7a65  ia, Belgium, Cze
-00002100: 6368 2052 6570 7562 6c69 632c 2047 6572  ch Republic, Ger
-00002110: 6d61 6e79 2c20 4372 6f61 7469 612c 204e  many, Croatia, N
-00002120: 6574 6865 726c 616e 6473 2c20 506f 6c61  etherlands, Pola
-00002130: 6e64 0a20 2061 6e64 2053 6c6f 7665 6e69  nd.  and Sloveni
-00002140: 612e 0a0a 4669 7865 640a 7e7e 7e7e 7e0a  a...Fixed.~~~~~.
-00002150: 2a20 5468 6520 646f 6d65 7374 6963 2062  * The domestic b
-00002160: 616e 6b20 636f 6465 2066 6f72 2048 756e  ank code for Hun
-00002170: 6761 7269 616e 2062 616e 6b73 2077 6173  garian banks was
-00002180: 2077 726f 6e67 6c79 2067 656e 6572 6174   wrongly generat
-00002190: 6564 2060 404b 7279 7374 6f66 6565 203c  ed `@Krystofee <
-000021a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000021b0: 6f6d 2f4b 7279 7374 6f66 6565 3e60 5f0a  om/Krystofee>`_.
-000021c0: 0a60 3230 3232 2e30 362e 3160 5f20 2d20  .`2022.06.1`_ - 
-000021d0: 3230 3232 2f30 362f 3036 0a2d 2d2d 2d2d  2022/06/06.-----
-000021e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000021f0: 2d2d 2d2d 0a0a 4164 6465 640a 7e7e 7e7e  ----..Added.~~~~
-00002200: 7e0a 2a20 4765 6e65 7261 7465 6420 6c69  ~.* Generated li
-00002210: 7374 206f 6620 526f 6d61 6e69 616e 2042  st of Romanian B
-00002220: 4943 7320 6040 4b72 7973 746f 6665 6520  ICs `@Krystofee 
-00002230: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00002240: 636f 6d2f 4b72 7973 746f 6665 653e 605f  com/Krystofee>`_
-00002250: 0a2a 2047 656e 6572 6174 6564 206c 6973  .* Generated lis
-00002260: 7420 6f66 2048 756e 6761 7269 616e 2042  t of Hungarian B
-00002270: 4943 7320 6040 4b72 7973 746f 6665 6520  ICs `@Krystofee 
-00002280: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00002290: 636f 6d2f 4b72 7973 746f 6665 653e 605f  com/Krystofee>`_
-000022a0: 0a2a 2045 7874 656e 6465 6420 6d61 6e75  .* Extended manu
-000022b0: 616c 6c79 2063 7572 6174 6564 206c 6973  ally curated lis
-000022c0: 7420 6f66 2049 7269 7368 2042 4943 7320  t of Irish BICs 
-000022d0: 6040 6465 6e6e 6973 7874 7269 6120 3c68  `@dennisxtria <h
-000022e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000022f0: 6d2f 6465 6e6e 6973 7874 7269 613e 605f  m/dennisxtria>`_
-00002300: 0a0a 0a60 3230 3232 2e30 362e 3060 5f20  ...`2022.06.0`_ 
-00002310: 2d20 3230 3232 2f30 362f 3036 0a2d 2d2d  - 2022/06/06.---
-00002320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002330: 2d2d 2d2d 2d2d 0a0a 4164 6465 640a 7e7e  ------..Added.~~
-00002340: 7e7e 7e0a 2a20 4d61 6e75 616c 6c79 2063  ~~~.* Manually c
-00002350: 7572 6174 6564 206c 6973 7420 6f66 2042  urated list of B
-00002360: 756c 6761 7269 616e 2042 4943 7320 6040  ulgarian BICs `@
-00002370: 4b72 7973 746f 6665 6520 3c68 7474 7073  Krystofee <https
-00002380: 3a2f 2f67 6974 6875 622e 636f 6d2f 4b72  ://github.com/Kr
-00002390: 7973 746f 6665 653e 605f 0a2a 204d 616e  ystofee>`_.* Man
-000023a0: 7561 6c6c 7920 6375 7261 7465 6420 6c69  ually curated li
-000023b0: 7374 206f 6620 5361 7564 6920 4172 6162  st of Saudi Arab
-000023c0: 6961 6e20 4249 4373 2060 4073 616d 697a  ian BICs `@samiz
-000023d0: 616d 616e 203c 6874 7470 733a 2f2f 6769  aman <https://gi
-000023e0: 7468 7562 2e63 6f6d 2f73 616d 697a 616d  thub.com/samizam
-000023f0: 616e 3e60 5f0a 2a20 5375 7070 6f72 7420  an>`_.* Support 
-00002400: 666f 7220 6050 7949 6e73 7461 6c6c 6572  for `PyInstaller
-00002410: 203c 6874 7470 733a 2f2f 7079 696e 7374   <https://pyinst
-00002420: 616c 6c65 722e 6f72 672f 656e 2f73 7461  aller.org/en/sta
-00002430: 626c 652f 3e60 5f20 6040 4c75 6b61 737a  ble/>`_ `@Lukasz
-00002440: 3837 203c 6874 7470 733a 2f2f 6769 7468  87 <https://gith
-00002450: 7562 2e63 6f6d 2f4c 756b 6173 7a38 373e  ub.com/Lukasz87>
-00002460: 605f 0a0a 496e 7465 726e 616c 0a7e 7e7e  `_..Internal.~~~
-00002470: 7e7e 7e7e 7e0a 2a20 5275 6e20 7465 7374  ~~~~~.* Run test
-00002480: 7320 6f6e 2050 7974 686f 6e20 332e 3130  s on Python 3.10
-00002490: 2060 4061 6461 6d63 6861 696e 7a20 3c68   `@adamchainz <h
-000024a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000024b0: 6d2f 6164 616d 6368 6169 6e7a 3e60 5f0a  m/adamchainz>`_.
-000024c0: 2a20 5573 6520 7374 616e 6461 7264 206b  * Use standard k
-000024d0: 6579 7320 696e 2060 6073 6574 7570 2e63  eys in ``setup.c
-000024e0: 6667 6060 2060 4061 6461 6d63 6861 696e  fg`` `@adamchain
-000024f0: 7a20 3c68 7474 7073 3a2f 2f67 6974 6875  z <https://githu
-00002500: 622e 636f 6d2f 6164 616d 6368 6169 6e7a  b.com/adamchainz
-00002510: 3e60 5f0a 2a20 446f 6e27 7420 7265 6c79  >`_.* Don't rely
-00002520: 206f 6e20 6060 6861 636b 696e 6760 6020   on ``hacking`` 
-00002530: 696e 2074 6573 742d 7365 7475 7020 6040  in test-setup `@
-00002540: 6164 616d 6368 6169 6e7a 203c 6874 7470  adamchainz <http
-00002550: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f61  s://github.com/a
-00002560: 6461 6d63 6861 696e 7a3e 605f 0a0a 6032  damchainz>`_..`2
-00002570: 3032 322e 3034 2e32 605f 202d 2032 3032  022.04.2`_ - 202
-00002580: 322f 3034 2f32 390a 2d2d 2d2d 2d2d 2d2d  2/04/29.--------
-00002590: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000025a0: 2d0a 0a43 6861 6e67 6564 0a7e 7e7e 7e7e  -..Changed.~~~~~
-000025b0: 7e7e 0a2a 2041 6c6c 6f77 2067 6574 7469  ~~.* Allow getti
-000025c0: 6e67 2062 616e 6b20 6e61 6d65 7320 6672  ng bank names fr
-000025d0: 6f6d 2049 4241 4e2e 2050 7265 7669 6f75  om IBAN. Previou
-000025e0: 736c 792c 2079 6f75 2063 6f75 6c64 2064  sly, you could d
-000025f0: 6f20 6060 6962 616e 2e62 6963 2e62 616e  o ``iban.bic.ban
-00002600: 6b5f 6e61 6d65 735b 305d 6060 2c20 6275  k_names[0]``, bu
-00002610: 7420 7369 6e63 650a 2020 6120 4249 4320  t since.  a BIC 
-00002620: 6361 6e20 6265 2061 7373 6f63 6961 7465  can be associate
-00002630: 6420 746f 206d 756c 7469 706c 6520 6261  d to multiple ba
-00002640: 6e6b 2063 6f64 6573 2074 6865 2063 6f6e  nk codes the con
-00002650: 7465 7874 206f 6620 7468 6520 7370 6563  text of the spec
-00002660: 6966 6963 2062 616e 6b20 6973 206c 6f73  ific bank is los
-00002670: 7420 616e 6420 796f 750a 2020 636f 756c  t and you.  coul
-00002680: 6420 656e 6420 7570 2077 6974 6820 7468  d end up with th
-00002690: 6520 7772 6f6e 6720 6261 6e6b 206e 616d  e wrong bank nam
-000026a0: 652e 2060 406a 6f73 652d 7265 7665 6e69  e. `@jose-reveni
-000026b0: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-000026c0: 2e63 6f6d 2f6a 6f73 652d 7265 7665 6e69  .com/jose-reveni
-000026d0: 3e60 5f0a 0a0a 6032 3032 322e 3034 2e31  >`_...`2022.04.1
-000026e0: 605f 202d 2032 3032 322f 3034 2f32 390a  `_ - 2022/04/29.
-000026f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002700: 2d2d 2d2d 2d2d 2d2d 2d0a 0a43 6861 6e67  ---------..Chang
-00002710: 6564 0a7e 7e7e 7e7e 7e7e 0a2a 2054 6865  ed.~~~~~~~.* The
-00002720: 2049 7461 6c69 616e 2042 4241 4e20 6368   Italian BBAN ch
-00002730: 6563 6b73 756d 2061 6c67 6f72 6974 686d  ecksum algorithm
-00002740: 2069 7320 6e6f 7720 616c 736f 2061 7070   is now also app
-00002750: 6c69 6564 2066 6f72 2053 616e 204d 6172  lied for San Mar
-00002760: 696e 6f20 6040 6661 6269 656e 7065 203c  ino `@fabienpe <
-00002770: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00002780: 6f6d 2f66 6162 6965 6e70 653e 605f 0a0a  om/fabienpe>`_..
-00002790: 4669 7865 640a 7e7e 7e7e 7e0a 2a20 4669  Fixed.~~~~~.* Fi
-000027a0: 7820 4974 616c 6961 6e20 4242 414e 2063  x Italian BBAN c
-000027b0: 6865 636b 7375 6d20 6361 6c63 756c 6174  hecksum calculat
-000027c0: 696f 6e20 6023 3738 203c 6874 7470 733a  ion `#78 <https:
-000027d0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 646f  //github.com/mdo
-000027e0: 6d6b 652f 7363 6877 6966 7479 2f69 7373  mke/schwifty/iss
-000027f0: 7565 732f 3738 3e60 5f0a 2a20 4669 7820  ues/78>`_.* Fix 
-00002800: 6261 6e6b 2063 6f64 6520 706f 7369 7469  bank code positi
-00002810: 6f6e 2069 6e20 4242 414e 2066 6f72 204a  on in BBAN for J
-00002820: 6f72 6461 6e20 6261 6e6b 7320 6040 6661  ordan banks `@fa
-00002830: 6269 656e 7065 203c 6874 7470 733a 2f2f  bienpe <https://
-00002840: 6769 7468 7562 2e63 6f6d 2f66 6162 6965  github.com/fabie
-00002850: 6e70 653e 605f 0a0a 0a60 3230 3232 2e30  npe>`_...`2022.0
-00002860: 342e 3060 5f20 2d20 3230 3232 2f30 342f  4.0`_ - 2022/04/
-00002870: 3131 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  11.-------------
-00002880: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4368  ------------..Ch
-00002890: 616e 6765 640a 7e7e 7e7e 7e7e 7e0a 2a20  anged.~~~~~~~.* 
-000028a0: 5570 6461 7465 2062 616e 6b20 7265 6769  Update bank regi
-000028b0: 7374 7279 2066 6f72 2041 7573 7472 6961  stry for Austria
-000028c0: 2c20 437a 6563 6820 5265 7075 626c 6963  , Czech Republic
-000028d0: 2c20 4765 726d 616e 792c 2053 7061 696e  , Germany, Spain
-000028e0: 2c20 506f 6c61 6e64 2061 6e64 2053 6c6f  , Poland and Slo
-000028f0: 7661 6b69 612e 0a0a 4669 7865 640a 7e7e  vakia...Fixed.~~
-00002900: 7e7e 7e0a 2a20 5265 6d6f 7665 6420 626f  ~~~.* Removed bo
-00002910: 6775 7320 6c69 6e65 2066 726f 6d20 6475  gus line from du
-00002920: 7463 6820 6261 6e6b 2072 6567 6973 7472  tch bank registr
-00002930: 792e 0a2a 204c 6f61 6469 6e67 2074 6865  y..* Loading the
-00002940: 2062 616e 6b20 7265 6769 7374 7279 206e   bank registry n
-00002950: 6f77 2061 6c73 6f20 776f 726b 7320 6f6e  ow also works on
-00002960: 206d 6163 6869 6e65 7320 7468 6174 2064   machines that d
-00002970: 6f6e 2774 2068 6176 6520 5554 462d 3820  on't have UTF-8 
-00002980: 6173 2074 6865 6972 2064 6566 6175 6c74  as their default
-00002990: 0a20 2065 6e63 6f64 696e 6720 6040 696d  .  encoding `@im
-000029a0: 6164 3376 203c 6874 7470 733a 2f2f 6769  ad3v <https://gi
-000029b0: 7468 7562 2e63 6f6d 2f69 6d61 6433 763e  thub.com/imad3v>
-000029c0: 605f 0a0a 0a60 3230 3232 2e30 332e 3160  `_...`2022.03.1`
-000029d0: 5f20 2d20 3230 3232 2f30 332f 3035 0a2d  _ - 2022/03/05.-
-000029e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000029f0: 2d2d 2d2d 2d2d 2d2d 0a0a 4164 6465 640a  --------..Added.
-00002a00: 7e7e 7e7e 7e0a 2a20 436f 756e 7472 7920  ~~~~~.* Country 
-00002a10: 7370 6563 6966 6320 6368 6563 6b73 756d  specifc checksum
-00002a20: 2076 616c 6964 6174 696f 6e20 666f 7220   validation for 
-00002a30: 4672 656e 6368 2062 616e 6b73 2028 6261  French banks (ba
-00002a40: 7365 6420 6f6e 2074 6865 2077 6f72 6b20  sed on the work 
-00002a50: 6f66 0a20 2060 4073 686f 6c61 6e20 3c68  of.  `@sholan <h
-00002a60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00002a70: 6d2f 7368 6f6c 616e 3e60 5f29 0a0a 0a60  m/sholan>`_)...`
-00002a80: 3230 3232 2e30 332e 3060 5f20 2d20 3230  2022.03.0`_ - 20
-00002a90: 3232 2f30 332f 3034 0a2d 2d2d 2d2d 2d2d  22/03/04.-------
-00002aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002ab0: 2d2d 0a0a 4164 6465 640a 7e7e 7e7e 7e0a  --..Added.~~~~~.
-00002ac0: 2a20 5468 6520 3a63 6c61 7373 3a60 2e49  * The :class:`.I
-00002ad0: 4241 4e60 2061 6e64 203a 636c 6173 733a  BAN` and :class:
-00002ae0: 602e 4249 4360 2063 6c61 7373 6573 206e  `.BIC` classes n
-00002af0: 6f77 2073 7570 706f 7274 2074 6865 2060  ow support the `
-00002b00: 605f 5f6c 656e 5f5f 6060 206d 6574 686f  `__len__`` metho
-00002b10: 6420 746f 2061 6c6c 6f77 2061 206d 6f72  d to allow a mor
-00002b20: 650a 2020 5079 7468 6f6e 6963 2063 616c  e.  Pythonic cal
-00002b30: 6375 6c61 7469 6f6e 206f 6620 7468 6520  culation of the 
-00002b40: 6c65 6e67 7468 2e0a 0a43 6861 6e67 6564  length...Changed
-00002b50: 0a7e 7e7e 7e7e 7e7e 0a2a 2055 7064 6174  .~~~~~~~.* Updat
-00002b60: 6520 6261 6e6b 2072 6567 6973 7472 7920  e bank registry 
-00002b70: 666f 7220 437a 6563 6820 5265 7075 626c  for Czech Republ
-00002b80: 6963 2c20 5370 6169 6e2c 2048 756e 6761  ic, Spain, Hunga
-00002b90: 7279 2c20 506f 6c61 6e64 2061 6e64 2053  ry, Poland and S
-00002ba0: 6c6f 7661 6b69 612e 0a0a 0a60 3230 3232  lovakia....`2022
-00002bb0: 2e30 322e 3060 5f20 2d20 3230 3232 2f30  .02.0`_ - 2022/0
-00002bc0: 322f 3135 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  2/15.-----------
-00002bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00002be0: 4164 6465 640a 7e7e 7e7e 7e0a 2a20 4e32  Added.~~~~~.* N2
-00002bf0: 3620 4249 4320 666f 7220 5370 6169 6e20  6 BIC for Spain 
-00002c00: 6040 6272 756e 6f76 696c 6120 3c68 7474  `@brunovila <htt
-00002c10: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002c20: 6272 756e 6f76 696c 613e 605f 0a2a 204d  brunovila>`_.* M
-00002c30: 616e 7561 6c6c 7920 6375 7261 7465 6420  anually curated 
-00002c40: 656e 7472 6965 7320 666f 7220 6261 6e6b  entries for bank
-00002c50: 7320 6672 6f6d 2049 6365 6c61 6e64 2060  s from Iceland `
-00002c60: 4067 6175 7469 6e69 6c73 203c 6874 7470  @gautinils <http
-00002c70: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
-00002c80: 6175 7469 6e69 6c73 3e60 5f0a 0a43 6861  autinils>`_..Cha
-00002c90: 6e67 6564 0a7e 7e7e 7e7e 7e7e 0a2a 2052  nged.~~~~~~~.* R
-00002ca0: 656d 6f76 6564 206d 616e 7561 6c6c 7920  emoved manually 
-00002cb0: 6375 7261 7465 6420 6261 6e6b 2065 6e74  curated bank ent
-00002cc0: 7269 6573 2066 6f72 2053 7061 696e 2073  ries for Spain s
-00002cd0: 696e 6365 2061 6c6c 2076 616c 7565 7320  ince all values 
-00002ce0: 7765 7265 2061 6c72 6561 6479 2070 6172  were already par
-00002cf0: 7420 6f66 0a20 2074 6865 2067 656e 6572  t of.  the gener
-00002d00: 6174 6564 2072 6567 6973 7472 792e 0a2a  ated registry..*
-00002d10: 2055 7064 6174 6564 2062 616e 6b20 7265   Updated bank re
-00002d20: 6769 7374 7279 2066 6f72 2041 7573 7472  gistry for Austr
-00002d30: 6961 2c20 4265 6c67 6975 6d2c 2043 7a65  ia, Belgium, Cze
-00002d40: 6368 2052 6570 7562 6c69 632c 2047 6572  ch Republic, Ger
-00002d50: 6d61 6e79 2c20 5370 6169 6e2c 204e 6574  many, Spain, Net
-00002d60: 6865 726c 616e 6473 2061 6e64 2050 6f6c  herlands and Pol
-00002d70: 616e 640a 2a20 4164 6465 6420 6f76 6572  and.* Added over
-00002d80: 7772 6974 6520 666f 7220 4942 414e 2073  write for IBAN s
-00002d90: 7065 6320 6f66 2043 7a65 6368 2052 6570  pec of Czech Rep
-00002da0: 7562 6c69 6320 616e 6420 4672 616e 6365  ublic and France
-00002db0: 2e20 5468 6520 6272 616e 6368 2061 6e64  . The branch and
-00002dc0: 2061 6363 6f75 6e74 2063 6f64 6520 706f   account code po
-00002dd0: 7369 7469 6f6e 730a 2020 6172 6520 7772  sitions.  are wr
-00002de0: 6f6e 676c 7920 7072 6f76 6964 6564 2069  ongly provided i
-00002df0: 6e20 7468 6520 6f66 6669 6369 616c 2049  n the official I
-00002e00: 4241 4e20 7265 6769 7374 7279 2e0a 0a60  BAN registry...`
-00002e10: 3230 3231 2e31 302e 3260 5f20 2d20 3230  2021.10.2`_ - 20
-00002e20: 3231 2f31 302f 3132 0a2d 2d2d 2d2d 2d2d  21/10/12.-------
-00002e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002e40: 2d2d 0a0a 4164 6465 640a 7e7e 7e7e 7e0a  --..Added.~~~~~.
-00002e50: 2a20 4164 6465 6420 3434 3020 6164 6469  * Added 440 addi
-00002e60: 7469 6f6e 616c 2062 616e 6b20 7265 636f  tional bank reco
-00002e70: 7264 7320 666f 7220 5370 6169 6e2e 0a0a  rds for Spain...
-00002e80: 6032 3032 312e 3130 2e31 605f 202d 2032  `2021.10.1`_ - 2
-00002e90: 3032 312f 3130 2f31 310a 2d2d 2d2d 2d2d  021/10/11.------
-00002ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00002eb0: 2d2d 2d0a 0a43 6861 6e67 6564 0a7e 7e7e  ---..Changed.~~~
-00002ec0: 7e7e 7e7e 0a2a 2055 7365 2060 696d 706f  ~~~~.* Use `impo
-00002ed0: 7274 6c69 622e 7265 736f 7572 6365 7320  rtlib.resources 
-00002ee0: 3c68 7474 7073 3a2f 2f64 6f63 732e 7079  <https://docs.py
-00002ef0: 7468 6f6e 2e6f 7267 2f33 2e39 2f6c 6962  thon.org/3.9/lib
-00002f00: 7261 7279 2f69 6d70 6f72 746c 6962 2e68  rary/importlib.h
-00002f10: 746d 6c23 6d6f 6475 6c65 2d69 6d70 6f72  tml#module-impor
-00002f20: 746c 6962 2e72 6573 6f75 7263 6573 3e60  tlib.resources>`
-00002f30: 5f0a 2020 666f 7220 6c6f 6164 696e 6720  _.  for loading 
-00002f40: 696e 7465 726e 616c 2072 6567 6973 7472  internal registr
-00002f50: 6965 732e 2054 6869 7320 7265 6d6f 7665  ies. This remove
-00002f60: 7320 7468 6520 6e65 6564 2074 6f20 6861  s the need to ha
-00002f70: 7665 2060 6073 6574 7570 746f 6f6c 7360  ve ``setuptools`
-00002f80: 6020 696e 7374 616c 6c65 642e 0a20 2054  ` installed..  T
-00002f90: 6861 6e6b 2079 6f75 2060 4061 2d72 6563  hank you `@a-rec
-00002fa0: 6b6e 6167 656c 203c 6874 7470 733a 2f2f  knagel <https://
-00002fb0: 6769 7468 7562 2e63 6f6d 2f61 2d72 6563  github.com/a-rec
-00002fc0: 6b6e 6167 656c 3e60 5f20 666f 7220 7468  knagel>`_ for th
-00002fd0: 6520 6964 6561 210a 0a46 6978 6564 0a7e  e idea!..Fixed.~
-00002fe0: 7e7e 7e7e 0a2a 2045 6e73 7572 6520 7468  ~~~~.* Ensure th
-00002ff0: 6174 2042 656c 6769 616e 2042 4241 4e20  at Belgian BBAN 
-00003000: 6368 6563 6b73 756d 7320 6172 6520 616c  checksums are al
-00003010: 7761 7973 2032 2064 6967 6974 7320 6c6f  ways 2 digits lo
-00003020: 6e67 2e0a 0a60 3230 3231 2e31 302e 3060  ng...`2021.10.0`
-00003030: 5f20 2d20 3230 3231 2f31 302f 3031 0a2d  _ - 2021/10/01.-
-00003040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003050: 2d2d 2d2d 2d2d 2d2d 0a0a 4164 6465 640a  --------..Added.
-00003060: 7e7e 7e7e 7e0a 2a20 4164 6465 6420 4942  ~~~~~.* Added IB
-00003070: 414e 2073 7065 6320 666f 7220 5375 6461  AN spec for Suda
-00003080: 6e20 2853 4429 2e0a 2a20 4164 6465 6420  n (SD)..* Added 
-00003090: 616e 6420 6578 7465 6e64 6564 206d 616e  and extended man
-000030a0: 7561 6c6c 7920 6375 7261 7465 6420 6261  ually curated ba
-000030b0: 6e6b 2065 6e74 7269 6573 2066 6f72 2054  nk entries for T
-000030c0: 7572 6b65 792c 2049 7461 6c79 2c20 4973  urkey, Italy, Is
-000030d0: 7261 656c 2c20 4972 656c 616e 642c 2053  rael, Ireland, S
-000030e0: 7061 696e 2c0a 2020 5377 6974 7a65 726c  pain,.  Switzerl
-000030f0: 616e 6420 616e 6420 4465 6e6d 6172 6b20  and and Denmark 
-00003100: 6040 686f 776f 726b 6f6e 203c 6874 7470  `@howorkon <http
-00003110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
-00003120: 6f77 6f72 6b6f 6e3e 605f 2e0a 0a43 6861  oworkon>`_...Cha
-00003130: 6e67 6564 0a7e 7e7e 7e7e 7e7e 0a2a 2055  nged.~~~~~~~.* U
-00003140: 7064 6174 6564 2062 616e 6b20 7265 6769  pdated bank regi
-00003150: 7374 7279 2066 6f72 2041 7573 7472 6961  stry for Austria
-00003160: 2c20 4265 6c67 6975 6d2c 2043 7a65 6368  , Belgium, Czech
-00003170: 2052 6570 7562 6c69 632c 2047 6572 6d61   Republic, Germa
-00003180: 6e79 2c20 4e65 7468 6572 6c61 6e64 732c  ny, Netherlands,
-00003190: 2050 6f6c 616e 642c 0a20 2053 6c6f 7665   Poland,.  Slove
-000031a0: 6e69 6120 616e 6420 536c 6f76 616b 6961  nia and Slovakia
-000031b0: 2e0a 0a46 6978 6564 0a7e 7e7e 7e7e 0a2a  ...Fixed.~~~~~.*
-000031c0: 2044 6973 616c 6c6f 7720 6060 7363 6877   Disallow ``schw
-000031d0: 6966 7479 6060 2074 6f20 6265 2069 6e73  ifty`` to be ins
-000031e0: 7461 6c6c 6564 2066 6f72 2050 7974 686f  talled for Pytho
-000031f0: 6e20 7665 7273 696f 6e73 206f 6c64 6572  n versions older
-00003200: 2074 6861 6e20 332e 372e 2049 7420 7761   than 3.7. It wa
-00003210: 7320 756e 7375 7070 6f72 7465 640a 2020  s unsupported.  
-00003220: 6265 666f 7265 2062 7574 2069 7320 6e6f  before but is no
-00003230: 7720 7265 6a65 6374 6564 2075 706f 6e20  w rejected upon 
-00003240: 696e 7374 616c 6c61 7469 6f6e 2077 6974  installation wit
-00003250: 6820 616e 2061 7070 726f 7072 6961 7465  h an appropriate
-00003260: 2065 7272 6f72 206d 6573 7361 6765 2e0a   error message..
-00003270: 2a20 4175 7374 7269 616e 2062 616e 6b20  * Austrian bank 
-00003280: 636f 6465 7320 6172 6520 6e6f 7720 636f  codes are now co
-00003290: 6e73 6973 7465 6e74 6c79 206c 6566 7420  nsistently left 
-000032a0: 7061 6464 6564 2077 6974 6820 7a65 726f  padded with zero
-000032b0: 732e 2054 6869 7320 6669 7865 7320 7468  s. This fixes th
-000032c0: 6520 6d61 7070 696e 6720 6672 6f6d 0a20  e mapping from. 
-000032d0: 2049 4241 4e20 746f 2042 4943 2066 6f72   IBAN to BIC for
-000032e0: 2074 6865 2041 7573 7472 6961 6e20 6665   the Austrian fe
-000032f0: 6465 7261 6c20 6261 6e6b 2069 6e73 7469  deral bank insti
-00003300: 7475 7465 732e 0a0a 6032 3032 312e 3036  tutes...`2021.06
-00003310: 2e31 605f 202d 2032 3032 312f 3036 2f32  .1`_ - 2021/06/2
-00003320: 340a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  4.--------------
-00003330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a41 6464  -----------..Add
-00003340: 6564 0a7e 7e7e 7e7e 0a2a 2045 6e61 626c  ed.~~~~~.* Enabl
-00003350: 6520 746f 6f6c 2062 6173 6564 2074 7970  e tool based typ
-00003360: 6520 6368 6563 6b69 6e67 2061 7320 6465  e checking as de
-00003370: 7363 7269 6265 6420 696e 2060 5045 502d  scribed in `PEP-
-00003380: 3035 3631 605f 2062 7920 6164 6469 6e67  0561`_ by adding
-00003390: 2074 6865 2060 6070 792e 7479 7065 6460   the ``py.typed`
-000033a0: 6020 6d61 726b 6572 0a20 2060 406a 6d66  ` marker.  `@jmf
-000033b0: 6564 6572 6963 6f20 3c68 7474 7073 3a2f  ederico <https:/
-000033c0: 2f67 6974 6875 622e 636f 6d2f 6a6d 6665  /github.com/jmfe
-000033d0: 6465 7269 636f 3e60 5f0a 0a0a 6032 3032  derico>`_...`202
-000033e0: 312e 3036 2e30 605f 202d 2032 3032 312f  1.06.0`_ - 2021/
-000033f0: 3036 2f31 370a 2d2d 2d2d 2d2d 2d2d 2d2d  06/17.----------
-00003400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00003410: 0a41 6464 6564 0a7e 7e7e 7e7e 0a2a 2041  .Added.~~~~~.* A
-00003420: 6464 6564 2062 616e 6b20 7265 6769 7374  dded bank regist
-00003430: 7279 2066 6f72 2053 7765 6469 7368 2042  ry for Swedish B
-00003440: 616e 6b73 2060 406a 6d66 6564 6572 6963  anks `@jmfederic
-00003450: 6f20 3c68 7474 7073 3a2f 2f67 6974 6875  o <https://githu
-00003460: 622e 636f 6d2f 6a6d 6665 6465 7269 636f  b.com/jmfederico
-00003470: 3e60 5f0a 0a0a 6032 3032 312e 3035 2e32  >`_...`2021.05.2
-00003480: 605f 202d 2032 3032 312f 3035 2f32 330a  `_ - 2021/05/23.
-00003490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000034a0: 2d2d 2d2d 2d2d 2d2d 2d0a 0a41 6464 6564  ---------..Added
-000034b0: 0a7e 7e7e 7e7e 0a2a 2043 6f75 6e74 7279  .~~~~~.* Country
-000034c0: 2073 7065 6369 6663 2063 6865 636b 7375   specifc checksu
-000034d0: 6d20 7661 6c69 6461 7469 6f6e 2066 6f72  m validation for
-000034e0: 2042 656c 6769 616e 2062 616e 6b73 2c20   Belgian banks, 
-000034f0: 6173 2077 656c 6c20 6173 2073 7570 706f  as well as suppo
-00003500: 7274 2066 6f72 2067 656e 6572 6174 696e  rt for generatin
-00003510: 6720 7468 650a 2020 6368 6563 6b73 756d  g the.  checksum
-00003520: 2077 6865 6e20 7573 696e 6720 7468 6520   when using the 
-00003530: 3a6d 6574 683a 602e 4942 414e 2e67 656e  :meth:`.IBAN.gen
-00003540: 6572 6174 6560 2d6d 6574 686f 642e 2060  erate`-method. `
-00003550: 406d 6865 6d65 7279 636b 203c 6874 7470  @mhemeryck <http
-00003560: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-00003570: 6865 6d65 7279 636b 3e60 5f0a 0a60 3230  hemeryck>`_..`20
-00003580: 3231 2e30 352e 3160 5f20 2d20 3230 3231  21.05.1`_ - 2021
-00003590: 2f30 352f 3230 0a2d 2d2d 2d2d 2d2d 2d2d  /05/20.---------
-000035a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000035b0: 0a0a 4164 6465 640a 7e7e 7e7e 7e0a 2a20  ..Added.~~~~~.* 
-000035c0: 5468 6520 4942 414e 2076 616c 6964 6174  The IBAN validat
-000035d0: 696f 6e20 6e6f 7720 6f70 7469 6f6e 616c  ion now optional
-000035e0: 6c79 2069 6e63 6c75 6465 7320 7468 6520  ly includes the 
-000035f0: 7665 7269 6669 6361 7469 6f6e 206f 6620  verification of 
-00003600: 7468 6520 636f 756e 7472 7920 7370 6563  the country spec
-00003610: 6966 6963 2063 6865 636b 7375 6d0a 2020  ific checksum.  
-00003620: 7769 7468 696e 2074 6865 2042 4241 4e2e  within the BBAN.
-00003630: 2054 6869 7320 6375 7272 656e 746c 7920   This currently 
-00003640: 776f 726b 7320 666f 7220 4765 726d 616e  works for German
-00003650: 2061 6e64 2049 7461 6c69 616e 2062 616e   and Italian ban
-00003660: 6b73 2e20 466f 7220 4765 726d 616e 2062  ks. For German b
-00003670: 616e 6b73 2074 6865 2063 6865 636b 7375  anks the checksu
-00003680: 6d0a 2020 616c 676f 7269 7468 6d20 666f  m.  algorithm fo
-00003690: 7220 7468 6520 6163 636f 756e 7420 636f  r the account co
-000036a0: 6465 2069 7320 6368 6f73 656e 2062 7920  de is chosen by 
-000036b0: 7468 6520 6261 6e6b 2063 6f64 652e 2053  the bank code. S
-000036c0: 696e 6365 2074 6865 7265 2061 7265 206f  ince there are o
-000036d0: 7665 7220 3135 3020 6261 6e6b 2073 7065  ver 150 bank spe
-000036e0: 6369 6669 630a 2020 616c 676f 7269 7468  cific.  algorith
-000036f0: 6d73 2069 6e20 4765 726d 616e 7920 6e6f  ms in Germany no
-00003700: 7420 616c 6c20 6f66 2074 6865 6d20 6172  t all of them ar
-00003710: 6520 696d 706c 656d 656e 7465 6420 6174  e implemented at
-00003720: 2074 6865 206d 6f6d 656e 742c 2062 7574   the moment, but
-00003730: 2074 6865 206d 616a 6f72 6974 7920 6f66   the majority of
-00003740: 2062 616e 6b73 0a20 2073 686f 756c 6420   banks.  should 
-00003750: 6265 2063 6f76 6572 6564 2e0a 0a43 6861  be covered...Cha
-00003760: 6e67 6564 0a7e 7e7e 7e7e 7e7e 0a2a 2055  nged.~~~~~~~.* U
-00003770: 7064 6174 6520 6261 6e6b 2072 6567 6973  pdate bank regis
-00003780: 7472 7920 666f 7220 4765 726d 616e 792c  try for Germany,
-00003790: 2050 6f6c 616e 642c 2043 7a65 6368 2052   Poland, Czech R
-000037a0: 6570 7562 6c69 632c 2041 7573 7472 6961  epublic, Austria
-000037b0: 2061 6e64 204e 6574 6865 726c 616e 6473   and Netherlands
-000037c0: 2e0a 0a60 3230 3231 2e30 352e 3060 5f20  ...`2021.05.0`_ 
-000037d0: 2d20 3230 3231 2f30 352f 3032 0a2d 2d2d  - 2021/05/02.---
-000037e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000037f0: 2d2d 2d2d 2d2d 0a0a 4164 6465 640a 7e7e  ------..Added.~~
-00003800: 7e7e 7e0a 2a20 4164 6465 6420 6d61 6e75  ~~~.* Added manu
-00003810: 616c 6c79 2063 7572 6174 6564 206c 6973  ally curated lis
-00003820: 7420 6f66 204c 6974 6875 616e 6961 6e20  t of Lithuanian 
-00003830: 4261 6e6b 7320 2865 2e67 2052 6576 6f6c  Banks (e.g Revol
-00003840: 7574 2050 6179 6d65 6e74 7320 5541 4229  ut Payments UAB)
-00003850: 2e0a 0a60 3230 3231 2e30 342e 3060 5f20  ...`2021.04.0`_ 
-00003860: 2d20 3230 3231 2f30 342f 3233 0a2d 2d2d  - 2021/04/23.---
-00003870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003880: 2d2d 2d2d 2d2d 0a0a 4368 616e 6765 640a  ------..Changed.
-00003890: 7e7e 7e7e 7e7e 7e0a 2a20 4164 6465 6420  ~~~~~~~.* Added 
-000038a0: 7479 7065 2068 696e 7473 2074 6f20 7468  type hints to th
-000038b0: 6520 656e 7469 7265 2063 6f64 6520 6261  e entire code ba
-000038c0: 7365 2e0a 2a20 4472 6f70 7065 6420 7375  se..* Dropped su
-000038d0: 7070 6f72 7420 666f 7220 5079 7468 6f6e  pport for Python
-000038e0: 2033 2e36 0a2a 2055 7064 6174 6520 6261   3.6.* Update ba
+00000080: 3035 2e31 605f 202d 2032 3032 342f 3035  05.1`_ - 2024/05
+00000090: 2f30 390a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /09.------------
+000000a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 4368  -------------.Ch
+000000b0: 616e 6765 640a 7e7e 7e7e 7e7e 7e0a 2a20  anged.~~~~~~~.* 
+000000c0: 5265 6d6f 7665 2063 7573 746f 6d20 636f  Remove custom co
+000000d0: 6c6c 6563 7469 6f6e 206c 6f67 6963 206f  llection logic o
+000000e0: 6620 7468 6520 6261 6e6b 2072 6567 6973  f the bank regis
+000000f0: 7472 7920 666f 7220 6060 7079 696e 7374  try for ``pyinst
+00000100: 616c 6c65 7260 602e 2054 6865 2063 6861  aller``. The cha
+00000110: 6e67 6573 2069 6e74 726f 6475 6365 6420  nges introduced 
+00000120: 696e 0a20 2060 2339 3220 3c68 7474 7073  in.  `#92 <https
+00000130: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d64  ://github.com/md
+00000140: 6f6d 6b65 2f73 6368 7769 6674 792f 7075  omke/schwifty/pu
+00000150: 6c6c 2f39 323e 605f 2077 6572 6520 7772  ll/92>`_ were wr
+00000160: 6f6e 6720 616e 6420 6861 7665 2062 6565  ong and have bee
+00000170: 6e20 7265 7665 7274 6564 2e20 5573 6167  n reverted. Usag
+00000180: 650a 2020 6578 616d 706c 650a 0a20 202e  e.  example..  .
+00000190: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2062  . code-block:: b
+000001a0: 6173 680a 0a20 2020 2024 2070 7969 6e73  ash..    $ pyins
+000001b0: 7461 6c6c 6572 203c 7363 7269 7074 3e20  taller <script> 
+000001c0: 2d2d 636f 6c6c 6563 742d 6461 7461 2073  --collect-data s
+000001d0: 6368 7769 6674 7920 2d2d 636f 7079 2d6d  chwifty --copy-m
+000001e0: 6574 6164 6174 6120 7363 6877 6966 7479  etadata schwifty
+000001f0: 0a0a 6032 3032 342e 3035 2e30 605f 202d  ..`2024.05.0`_ -
+00000200: 2032 3032 342f 3035 2f30 370a 2d2d 2d2d   2024/05/07.----
+00000210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000220: 2d2d 2d2d 2d0a 4669 7865 640a 7e7e 7e7e  -----.Fixed.~~~~
+00000230: 7e0a 2a20 4c6f 6164 696e 6720 4a53 4f4e  ~.* Loading JSON
+00000240: 2064 6174 6120 696e 746f 2061 2050 7964   data into a Pyd
+00000250: 616e 7469 6320 6d6f 6465 6c20 7769 7468  antic model with
+00000260: 2061 6e20 6060 4942 414e 6060 206f 7220   an ``IBAN`` or 
+00000270: 6060 4249 4360 602d 6669 656c 640a 2020  ``BIC``-field.  
+00000280: 2860 604d 6f64 656c 2e6d 6f64 656c 5f76  (``Model.model_v
+00000290: 616c 6964 6174 655f 6a73 6f6e 2829 6060  alidate_json()``
+000002a0: 2920 7761 7320 7072 6576 696f 7573 6c79  ) was previously
+000002b0: 2062 726f 6b65 6e20 616e 6420 6861 7320   broken and has 
+000002c0: 6265 656e 2066 6978 6564 206e 6f77 2e0a  been fixed now..
+000002d0: 0a41 6464 6564 0a7e 7e7e 7e7e 0a2a 204a  .Added.~~~~~.* J
+000002e0: 534f 4e20 7363 6865 6d61 2067 656e 6572  SON schema gener
+000002f0: 6174 696f 6e20 666f 7220 5079 6461 6e74  ation for Pydant
+00000300: 6963 206d 6f64 656c 732e 0a0a 4368 616e  ic models...Chan
+00000310: 6765 640a 7e7e 7e7e 7e7e 7e0a 2a20 5570  ged.~~~~~~~.* Up
+00000320: 6461 7465 6420 6261 6e6b 2072 6567 6973  dated bank regis
+00000330: 7472 6965 732e 0a2a 2052 656d 6f76 6520  tries..* Remove 
+00000340: 7468 6520 6465 7065 6e64 656e 6379 2074  the dependency t
+00000350: 6f20 6060 6973 6f33 3136 3660 6020 7369  o ``iso3166`` si
+00000360: 6e63 6520 6974 7320 6675 6e63 7469 6f6e  nce its function
+00000370: 616c 6c69 7479 2069 7320 616c 7265 6164  allity is alread
+00000380: 7920 636f 7665 7265 6420 6279 2060 6070  y covered by ``p
+00000390: 7963 6f75 6e74 7279 6060 0a0a 0a60 3230  ycountry``...`20
+000003a0: 3234 2e30 342e 3060 5f20 2d20 3230 3234  24.04.0`_ - 2024
+000003b0: 2f30 342f 3138 0a2d 2d2d 2d2d 2d2d 2d2d  /04/18.---------
+000003c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000003d0: 0a41 6464 6564 0a7e 7e7e 7e7e 0a2a 2041  .Added.~~~~~.* A
+000003e0: 6464 6564 2052 6576 6f6c 7574 2042 616e  dded Revolut Ban
+000003f0: 6b20 666f 7220 5370 6169 6e20 6040 6272  k for Spain `@br
+00000400: 756e 6f76 696c 6c61 203c 6874 7470 733a  unovilla <https:
+00000410: 2f2f 6769 7468 7562 2e63 6f6d 2f62 7275  //github.com/bru
+00000420: 6e6f 7669 6c61 3e60 5f0a 2a20 4164 6465  novila>`_.* Adde
+00000430: 6420 7375 7070 6f72 7420 666f 7220 5079  d support for Py
+00000440: 7468 6f6e 2033 2e31 320a 2a20 4164 6465  thon 3.12.* Adde
+00000450: 6420 6d61 6e75 616c 6c79 2063 7572 6174  d manually curat
+00000460: 6564 2062 616e 6b20 7265 6769 7374 7279  ed bank registry
+00000470: 2066 6f72 204d 6f6e 7465 6e65 6772 6f20   for Montenegro 
+00000480: 6040 446a 756b 6120 3c68 7474 7073 3a2f  `@Djuka <https:/
+00000490: 2f67 6974 6875 622e 636f 6d2f 446a 756b  /github.com/Djuk
+000004a0: 613e 605f 0a0a 4368 616e 6765 640a 7e7e  a>`_..Changed.~~
+000004b0: 7e7e 7e7e 7e0a 2a20 5468 6520 6261 6e6b  ~~~~~.* The bank
+000004c0: 2072 6567 6973 7472 7920 6973 206e 6f77   registry is now
+000004d0: 2069 6e74 6572 6e61 6c6c 7920 7661 6c69   internally vali
+000004e0: 6461 7465 642c 2073 6f20 7468 6174 2061  dated, so that a
+000004f0: 6c6c 2064 6f6d 6573 7469 6320 6261 6e6b  ll domestic bank
+00000500: 2063 6f64 6573 2061 6374 6175 6c6c 7920   codes actaully 
+00000510: 6d61 7463 6820 7468 650a 2020 7370 6563  match the.  spec
+00000520: 6966 6963 6174 696f 6e20 6f66 2074 6865  ification of the
+00000530: 2063 6f72 7265 7370 6f6e 6469 6e67 2042   corresponding B
+00000540: 4241 4e20 7374 7275 6374 7572 652e 2041  BAN structure. A
+00000550: 7320 6120 7265 7375 6c74 2073 6f6d 6520  s a result some 
+00000560: 656e 7472 6965 7320 6861 6420 746f 2062  entries had to b
+00000570: 6520 7265 6d6f 7665 642c 0a20 2062 6563  e removed,.  bec
+00000580: 6175 7365 2074 6865 7920 6469 6420 636f  ause they did co
+00000590: 6e74 6169 6e20 696e 7661 6c69 6420 6261  ntain invalid ba
+000005a0: 6e6b 2063 6f64 6573 2e0a 2a20 5468 6520  nk codes..* The 
+000005b0: 4461 6e69 7368 206e 6174 696f 6e61 6c20  Danish national 
+000005c0: 6368 6563 6b73 756d 2061 6c67 6f72 6974  checksum algorit
+000005d0: 686d 2069 7320 636f 6e73 6964 6572 6564  hm is considered
+000005e0: 206f 7061 7175 6520 616e 6420 7468 6520   opaque and the 
+000005f0: 6368 6563 6b73 756d 2064 6967 6974 2069  checksum digit i
+00000600: 7320 6173 7375 6d65 6420 746f 0a20 2062  s assumed to.  b
+00000610: 6520 7061 7274 206f 6620 7468 6520 6163  e part of the ac
+00000620: 636f 756e 7420 6e75 6d62 6572 2028 7768  count number (wh
+00000630: 6963 6820 6973 206e 6f77 2061 6c77 6179  ich is now alway
+00000640: 7320 3130 2064 6967 6974 7320 6c6f 6e67  s 10 digits long
+00000650: 292e 0a0a 4669 7865 640a 7e7e 7e7e 7e0a  )...Fixed.~~~~~.
+00000660: 2a20 5468 6520 437a 6563 6820 6261 6e6b  * The Czech bank
+00000670: 2072 6567 6973 7472 7920 7761 7320 7374   registry was st
+00000680: 6f72 6564 2069 6e20 6c61 7469 6e2d 3120  ored in latin-1 
+00000690: 656e 636f 6469 6e67 2077 6869 6c65 2062  encoding while b
+000006a0: 6569 6e67 2072 6561 6420 6173 2055 5446  eing read as UTF
+000006b0: 2d38 2e20 5468 6973 2072 6573 756c 7465  -8. This resulte
+000006c0: 640a 2020 696e 2069 6e76 616c 6964 2062  d.  in invalid b
+000006d0: 616e 6b20 6e61 6d65 7320 6040 4e61 7469  ank names `@Nati
+000006e0: 6d20 3c68 7474 7073 3a2f 2f67 6974 6875  m <https://githu
+000006f0: 622e 636f 6d2f 4e61 7469 6d3e 605f 2061  b.com/Natim>`_ a
+00000700: 6e64 0a20 2060 4043 6f67 6178 203c 6874  nd.  `@Cogax <ht
+00000710: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000720: 2f43 6f67 6178 3e60 5f2e 0a2a 2054 6865  /Cogax>`_..* The
+00000730: 204e 6f72 7765 6769 616e 206e 6174 696f   Norwegian natio
+00000740: 6e61 6c20 6368 6563 6b73 756d 2061 6c67  nal checksum alg
+00000750: 6f72 6974 686d 2077 6173 2072 656e 6465  orithm was rende
+00000760: 7269 6e67 2077 726f 6e67 2072 6573 756c  ring wrong resul
+00000770: 7473 2069 6e20 736f 6d65 2065 6467 652d  ts in some edge-
+00000780: 6361 7365 730a 2020 6040 4e61 7469 6d20  cases.  `@Natim 
+00000790: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+000007a0: 636f 6d2f 4e61 7469 6d3e 605f 0a0a 0a0a  com/Natim>`_....
+000007b0: 6032 3032 342e 3031 2e31 605f 202d 2032  `2024.01.1`_ - 2
+000007c0: 3032 342f 3031 2f30 350a 2d2d 2d2d 2d2d  024/01/05.------
+000007d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000007e0: 2d2d 2d0a 4164 6465 640a 7e7e 7e7e 7e0a  ---.Added.~~~~~.
+000007f0: 0a2a 2053 7570 706f 7274 2061 7370 6972  .* Support aspir
+00000800: 6174 696f 6e61 6c20 636f 756e 7472 6965  ational countrie
+00000810: 733a 0a0a 2020 2a20 416c 6765 7269 610a  s:..  * Algeria.
+00000820: 2020 2a20 416e 676f 6c61 0a20 202a 2042    * Angola.  * B
+00000830: 656e 696e 0a20 202a 2042 7572 6b69 6e61  enin.  * Burkina
+00000840: 2046 6173 6f0a 2020 2a20 4275 7275 6e64   Faso.  * Burund
+00000850: 690a 2020 2a20 4361 626f 2056 6572 6465  i.  * Cabo Verde
+00000860: 0a20 202a 2043 616d 6572 6f6f 6e0a 2020  .  * Cameroon.  
+00000870: 2a20 4365 6e74 7261 6c20 4166 7269 6361  * Central Africa
+00000880: 6e20 5265 7075 626c 6963 0a20 202a 2043  n Republic.  * C
+00000890: 6861 640a 2020 2a20 436f 6d6f 726f 730a  had.  * Comoros.
+000008a0: 2020 2a20 436f 6e67 6f0a 2020 2a20 43c3    * Congo.  * C.
+000008b0: b474 6520 6427 4976 6f69 7265 0a20 202a  .te d'Ivoire.  *
+000008c0: 2044 6a69 626f 7574 690a 2020 2a20 4571   Djibouti.  * Eq
+000008d0: 7561 746f 7269 616c 2047 7569 6e65 610a  uatorial Guinea.
+000008e0: 2020 2a20 4761 626f 6e2c 0a20 202a 2047    * Gabon,.  * G
+000008f0: 7569 6e65 612d 4269 7373 6175 0a20 202a  uinea-Bissau.  *
+00000900: 2048 6f6e 6475 7261 730a 2020 2a20 4972   Honduras.  * Ir
+00000910: 616e 0a20 202a 204d 6164 6167 6173 6361  an.  * Madagasca
+00000920: 720a 2020 2a20 4d61 6c69 0a20 202a 204d  r.  * Mali.  * M
+00000930: 6f72 6f63 636f 0a20 202a 204d 6f7a 616d  orocco.  * Mozam
+00000940: 6269 7175 650a 2020 2a20 4e69 6361 7261  bique.  * Nicara
+00000950: 6775 610a 2020 2a20 4e69 6765 720a 2020  gua.  * Niger.  
+00000960: 2a20 5365 6e65 6761 6c0a 2020 2a20 546f  * Senegal.  * To
+00000970: 676f 0a0a 2a20 4e61 7469 6f6e 616c 2063  go..* National c
+00000980: 6865 636b 7375 6d20 616c 676f 7269 7468  hecksum algorith
+00000990: 6d73 2066 6f72 206d 616e 7920 636f 756e  ms for many coun
+000009a0: 7472 6965 7320 6861 7665 2062 6565 6e20  tries have been 
+000009b0: 6164 6465 643a 0a0a 2020 2a20 416c 6261  added:..  * Alba
+000009c0: 6e69 610a 2020 2a20 426f 736e 6961 2061  nia.  * Bosnia a
+000009d0: 6e64 2048 6572 7a65 676f 7669 6e61 0a20  nd Herzegovina. 
+000009e0: 202a 2043 7a65 6368 2052 6570 7562 6c69   * Czech Republi
+000009f0: 630a 2020 2a20 4561 7374 2054 696d 6f72  c.  * East Timor
+00000a00: 0a20 202a 2045 7374 6f6e 6961 0a20 202a  .  * Estonia.  *
+00000a10: 2046 696e 6c61 6e64 0a20 202a 2049 6365   Finland.  * Ice
+00000a20: 6c61 6e64 0a20 202a 204d 6175 7269 7461  land.  * Maurita
+00000a30: 6e69 610a 2020 2a20 4d6f 6e74 656e 6567  nia.  * Monteneg
+00000a40: 726f 0a20 202a 204e 6f72 7468 204d 6163  ro.  * North Mac
+00000a50: 6564 6f6e 6961 0a20 202a 204e 6f72 7761  edonia.  * Norwa
+00000a60: 790a 2020 2a20 506f 6c61 6e64 0a20 202a  y.  * Poland.  *
+00000a70: 2050 6f72 7475 6761 6c0a 2020 2a20 5365   Portugal.  * Se
+00000a80: 7262 6961 0a20 202a 2053 6c6f 7661 6b69  rbia.  * Slovaki
+00000a90: 610a 2020 2a20 536c 6f76 656e 6961 0a20  a.  * Slovenia. 
+00000aa0: 202a 2053 7061 696e 0a20 202a 2054 756e   * Spain.  * Tun
+00000ab0: 6973 6961 0a0a 2a20 4164 6420 6e65 7720  isia..* Add new 
+00000ac0: 6261 6e6b 7320 746f 2074 6865 206c 6973  banks to the lis
+00000ad0: 7420 6f66 2046 7265 6e63 6820 6261 6e6b  t of French bank
+00000ae0: 7320 6040 4e61 7469 6d20 3c68 7474 7073  s `@Natim <https
+00000af0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e61  ://github.com/Na
+00000b00: 7469 6d3e 605f 3a0a 0a20 202a 2041 524b  tim>`_:..  * ARK
+00000b10: 4541 2042 5020 4272 6573 740a 2020 2a20  EA BP Brest.  * 
+00000b20: 416e 7974 696d 650a 2020 2a20 4c79 6469  Anytime.  * Lydi
+00000b30: 6120 4261 6e6b 0a20 202a 204d 454d 4f20  a Bank.  * MEMO 
+00000b40: 4241 4e4b 0a20 202a 2052 6576 6f6c 7574  BANK.  * Revolut
+00000b50: 0a20 202a 2053 4849 4e45 0a20 202a 2053  .  * SHINE.  * S
+00000b60: 756d 5570 204c 696d 6974 6564 0a0a 2a20  umUp Limited..* 
+00000b70: 4e65 7720 3a61 7474 723a 602e 4942 414e  New :attr:`.IBAN
+00000b80: 2e69 6e5f 7365 7061 5f7a 6f6e 6560 2d70  .in_sepa_zone`-p
+00000b90: 726f 7065 7274 7920 746f 2069 6e64 6963  roperty to indic
+00000ba0: 6174 6520 6966 2074 6865 2049 4241 4e27  ate if the IBAN'
+00000bb0: 7320 636f 756e 7472 7920 6973 2070 6172  s country is par
+00000bc0: 7420 6f66 2074 6865 2053 4550 410a 2020  t of the SEPA.  
+00000bd0: 7a6f 6e65 2e0a 2a20 4e65 7720 6d61 6e75  zone..* New manu
+00000be0: 616c 2062 616e 6b20 7265 6769 7374 7269  al bank registri
+00000bf0: 6573 2066 6f72 0a0a 2020 2a20 416e 646f  es for..  * Ando
+00000c00: 7272 610a 2020 2a20 4172 6162 6963 2045  rra.  * Arabic E
+00000c10: 6d69 7261 7465 730a 2020 2a20 436f 7374  mirates.  * Cost
+00000c20: 6120 5269 6361 0a20 202a 2050 6f72 7475  a Rica.  * Portu
+00000c30: 6761 6c0a 0a2a 204e 6577 2061 7474 7269  gal..* New attri
+00000c40: 6275 7465 7320 3a61 7474 723a 602e 4942  butes :attr:`.IB
+00000c50: 414e 2e61 6363 6f75 6e74 5f69 6460 2c20  AN.account_id`, 
+00000c60: 3a61 7474 723a 602e 4942 414e 2e61 6363  :attr:`.IBAN.acc
+00000c70: 6f75 6e74 5f68 6f6c 6465 725f 6964 6020  ount_holder_id` 
+00000c80: 616e 640a 2020 3a61 7474 723a 602e 4942  and.  :attr:`.IB
+00000c90: 414e 2e61 6363 6f75 6e74 5f74 7970 6560  AN.account_type`
+00000ca0: 2074 6861 7420 6172 6520 6176 6169 6c61   that are availa
+00000cb0: 626c 6520 6465 7065 6e64 696e 6720 6f6e  ble depending on
+00000cc0: 2074 6865 2063 6f75 6e74 7279 2773 2042   the country's B
+00000cd0: 4241 4e20 7370 6563 6966 6963 6174 696f  BAN specificatio
+00000ce0: 6e2e 0a20 2045 2e67 2e20 3a61 7474 723a  n..  E.g. :attr:
+00000cf0: 602e 4942 414e 2e61 6363 6f75 6e74 5f68  `.IBAN.account_h
+00000d00: 6f6c 6465 725f 6964 6020 6973 2063 7572  older_id` is cur
+00000d10: 7265 6e74 6c79 206f 6e6c 7920 6176 6169  rently only avai
+00000d20: 6c61 626c 6520 666f 7220 4963 656c 616e  lable for Icelan
+00000d30: 6420 284b 656e 6e69 7461 6c61 2920 616e  d (Kennitala) an
+00000d40: 6420 6f6e 6c79 0a20 2042 7261 7a69 6c20  d only.  Brazil 
+00000d50: 6465 6669 6e65 7320 616e 203a 6174 7472  defines an :attr
+00000d60: 3a60 2e49 4241 4e2e 6163 636f 756e 745f  :`.IBAN.account_
+00000d70: 6964 602e 0a0a 4368 616e 6765 640a 7e7e  id`...Changed.~~
+00000d80: 7e7e 7e7e 7e0a 2a20 5573 6520 656e 6861  ~~~~~.* Use enha
+00000d90: 6e63 6564 2049 4241 4e2f 4242 414e 2066  nced IBAN/BBAN f
+00000da0: 6f72 6d61 7420 6672 6f6d 2060 5769 6b69  ormat from `Wiki
+00000db0: 7065 6469 6120 3c68 7474 7073 3a2f 2f65  pedia <https://e
+00000dc0: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
+00000dd0: 7769 6b69 2f49 6e74 6572 6e61 7469 6f6e  wiki/Internation
+00000de0: 616c 5f42 616e 6b5f 4163 636f 756e 745f  al_Bank_Account_
+00000df0: 4e75 6d62 6572 2349 4241 4e5f 666f 726d  Number#IBAN_form
+00000e00: 6174 735f 6279 5f63 6f75 6e74 7279 3e60  ats_by_country>`
+00000e10: 5f2c 0a20 2073 696e 6365 2074 6865 206f  _,.  since the o
+00000e20: 6666 6963 6961 6c20 696e 666f 726d 6174  fficial informat
+00000e30: 696f 6e20 6672 6f6d 2053 5749 4654 2069  ion from SWIFT i
+00000e40: 7320 6f66 7465 6e20 696e 6163 7572 6174  s often inacurat
+00000e50: 652e 0a2a 2054 6865 2073 7570 706f 7274  e..* The support
+00000e60: 2066 6f72 206e 6174 696f 6e61 6c20 6368   for national ch
+00000e70: 6563 6b73 756d 2064 6967 6974 7320 6861  ecksum digits ha
+00000e80: 7320 6265 656e 2072 6569 6d70 6c65 6d65  s been reimpleme
+00000e90: 6e74 6564 2e0a 2a20 5468 6520 3a63 6c61  nted..* The :cla
+00000ea0: 7373 3a60 2e49 4241 4e60 2d63 6c61 7373  ss:`.IBAN`-class
+00000eb0: 206e 6f77 2068 6173 2061 6e20 6164 6469   now has an addi
+00000ec0: 7469 6f6e 616c 203a 6174 7472 3a60 2e49  tional :attr:`.I
+00000ed0: 4241 4e2e 6262 616e 602d 6174 7472 6962  BAN.bban`-attrib
+00000ee0: 7574 652c 2077 6865 7265 2061 6c6c 2063  ute, where all c
+00000ef0: 6f75 6e74 7279 0a20 2073 7065 6369 6669  ountry.  specifi
+00000f00: 6320 6675 6e63 7469 6f6e 616c 6974 7920  c functionality 
+00000f10: 6861 7320 6265 656e 206d 6f76 6564 2074  has been moved t
+00000f20: 6f2e 0a2a 2055 7064 6174 6564 2062 616e  o..* Updated ban
+00000f30: 6b20 7265 6769 7374 7269 6573 2e20 5468  k registries. Th
+00000f40: 616e 6b73 2074 6f20 6040 7368 3464 6f77  anks to `@sh4dow
+00000f50: 6220 3c68 7474 7073 3a2f 2f67 6974 6875  b <https://githu
+00000f60: 622e 636f 6d2f 7368 3464 6f77 623e 605f  b.com/sh4dowb>`_
+00000f70: 2066 6f72 2074 6865 2054 7572 6b69 7368   for the Turkish
+00000f80: 2062 616e 6b73 2e0a 0a0a 6032 3032 332e   banks....`2023.
+00000f90: 3131 2e32 605f 202d 2032 3032 332f 3131  11.2`_ - 2023/11
+00000fa0: 2f32 370a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /27.------------
+00000fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 4164  -------------.Ad
+00000fc0: 6465 640a 7e7e 7e7e 7e0a 2a20 4164 6420  ded.~~~~~.* Add 
+00000fd0: 4f4b 414c 4920 746f 2074 6865 206c 6973  OKALI to the lis
+00000fe0: 7420 6f66 2046 7265 6e63 6820 6261 6e6b  t of French bank
+00000ff0: 7320 6040 4e61 7469 6d20 3c68 7474 7073  s `@Natim <https
+00001000: 3a2f 2f67 6974 6875 622e 636f 6d2f 4e61  ://github.com/Na
+00001010: 7469 6d3e 605f 2e0a 0a60 3230 3233 2e31  tim>`_...`2023.1
+00001020: 312e 3160 5f20 2d20 3230 3233 2f31 312f  1.1`_ - 2023/11/
+00001030: 3237 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  27.-------------
+00001040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a43 6861  ------------.Cha
+00001050: 6e67 6564 0a7e 7e7e 7e7e 7e7e 0a2a 2054  nged.~~~~~~~.* T
+00001060: 6865 2053 7769 7373 2062 616e 6b20 7265  he Swiss bank re
+00001070: 6769 7374 7279 2069 7320 6e6f 7720 6765  gistry is now ge
+00001080: 6e65 7261 7465 6420 6672 6f6d 2074 6865  nerated from the
+00001090: 2053 4958 2047 726f 7570 2e0a 2a20 4d61   SIX Group..* Ma
+000010a0: 6e75 616c 6c79 2061 6464 206d 6973 7369  nually add missi
+000010b0: 6e67 2062 616e 6b20 656e 7472 7920 666f  ng bank entry fo
+000010c0: 7220 5370 6169 6e2e 0a2a 2055 7064 6174  r Spain..* Updat
+000010d0: 6564 2062 616e 6b20 7265 6769 7374 7220  ed bank registr 
+000010e0: 666f 7220 4175 7374 7269 6120 616e 6420  for Austria and 
+000010f0: 506f 6c61 6e64 2e0a 0a60 3230 3233 2e31  Poland...`2023.1
+00001100: 312e 3060 5f20 2d20 3230 3233 2f31 312f  1.0`_ - 2023/11/
+00001110: 3137 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  17.-------------
+00001120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a43 6861  ------------.Cha
+00001130: 6e67 6564 0a7e 7e7e 7e7e 7e7e 0a2a 2054  nged.~~~~~~~.* T
+00001140: 6865 2076 616c 6964 6174 696f 6e20 6f66  he validation of
+00001150: 2061 203a 636c 6173 733a 602e 4249 4360   a :class:`.BIC`
+00001160: 2069 7320 6e6f 7720 7065 7266 6f72 6d65   is now performe
+00001170: 6420 696e 2074 6865 2063 6f6e 7465 7874  d in the context
+00001180: 206f 6620 4953 4f20 3933 3632 3a32 3032   of ISO 9362:202
+00001190: 3220 7768 6963 6820 616c 6c6f 7773 0a20  2 which allows. 
+000011a0: 206e 756d 6265 7273 2069 6e20 7468 6520   numbers in the 
+000011b0: 6275 7369 6e65 7373 2070 6172 7479 2070  business party p
+000011c0: 7265 6669 782e 2049 6620 7374 7269 6374  refix. If strict
+000011d0: 2053 5749 4654 2063 6f6d 706c 6961 6e63   SWIFT complianc
+000011e0: 6520 6973 2072 6571 7275 6965 6420 7468  e is reqruied th
+000011f0: 650a 2020 6060 656e 666f 7263 655f 7377  e.  ``enforce_sw
+00001200: 6966 745f 636f 6d70 6c69 616e 6365 6060  ift_compliance``
+00001210: 2070 6172 616d 6574 6572 2063 616e 2062   parameter can b
+00001220: 6520 7365 7420 746f 2060 6054 7275 6560  e set to ``True`
+00001230: 602e 0a2a 2054 6865 203a 6d65 7468 3a60  `..* The :meth:`
+00001240: 2e42 4943 2e66 726f 6d5f 6261 6e6b 5f63  .BIC.from_bank_c
+00001250: 6f64 6560 2d6d 6574 686f 6420 7769 6c6c  ode`-method will
+00001260: 206e 6f77 2073 656c 6563 7420 7468 6520   now select the 
+00001270: 6d6f 7374 2067 656e 6572 6963 2042 4943  most generic BIC
+00001280: 2028 652e 672e 2077 6974 6820 6e6f 2062   (e.g. with no b
+00001290: 7261 6e63 680a 2020 7370 6563 6966 6965  ranch.  specifie
+000012a0: 7220 6f72 2074 6865 2022 5858 5822 2076  r or the "XXX" v
+000012b0: 616c 7565 2920 6966 206d 756c 7469 706c  alue) if multipl
+000012c0: 6520 4249 4373 2061 7265 2061 7373 6f63  e BICs are assoc
+000012d0: 6961 7465 6420 746f 2074 6865 2067 6976  iated to the giv
+000012e0: 656e 2064 6f6d 6573 7469 6320 6261 6e6b  en domestic bank
+000012f0: 2063 6f64 652e 0a20 2060 404e 6174 696d   code..  `@Natim
+00001300: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
+00001310: 2e63 6f6d 2f4e 6174 696d 3e60 5f2e 0a2a  .com/Natim>`_..*
+00001320: 204d 616e 7920 6d61 6e75 616c 6c79 2063   Many manually c
+00001330: 7572 6174 6564 2062 616e 6b20 7265 6769  urated bank regi
+00001340: 7374 7279 2065 6e74 7269 6573 2068 6176  stry entries hav
+00001350: 6520 6265 656e 2072 652d 6164 6465 6420  e been re-added 
+00001360: 6279 2060 4064 656e 6e69 7378 7472 6961  by `@dennisxtria
+00001370: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
+00001380: 2e63 6f6d 2f64 656e 6e69 7378 7472 6961  .com/dennisxtria
+00001390: 3e60 5f0a 0a60 3230 3233 2e31 302e 3060  >`_..`2023.10.0`
+000013a0: 5f20 2d20 3230 3233 2f31 302f 3331 0a2d  _ - 2023/10/31.-
+000013b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013c0: 2d2d 2d2d 2d2d 2d2d 0a41 6464 6564 0a7e  --------.Added.~
+000013d0: 7e7e 7e7e 7e7e 0a2a 2054 6865 2050 7964  ~~~~~~.* The Pyd
+000013e0: 616e 7469 6320 7632 2070 726f 746f 636f  antic v2 protoco
+000013f0: 6c20 6973 206e 6f77 2073 7570 706f 7274  l is now support
+00001400: 6564 2c20 736f 2074 6861 7420 7468 6520  ed, so that the 
+00001410: 3a63 6c61 7373 3a60 2e49 4241 4e60 2061  :class:`.IBAN` a
+00001420: 6e64 203a 636c 6173 733a 602e 4249 4360  nd :class:`.BIC`
+00001430: 2063 6c61 7373 6573 0a20 2063 616e 2062   classes.  can b
+00001440: 6520 6469 7265 6374 6c79 2075 7365 6420  e directly used 
+00001450: 6173 2074 7970 6520 616e 6e6f 7461 7469  as type annotati
+00001460: 6f6e 7320 696e 2060 5079 6461 6e74 6963  ons in `Pydantic
+00001470: 206d 6f64 656c 7320 3c68 7474 7073 3a2f   models <https:/
+00001480: 2f64 6f63 732e 7079 6461 6e74 6963 2e64  /docs.pydantic.d
+00001490: 6576 2f6c 6174 6573 742f 636f 6e63 6570  ev/latest/concep
+000014a0: 7473 2f6d 6f64 656c 732f 2362 6173 6963  ts/models/#basic
+000014b0: 2d6d 6f64 656c 2d75 7361 6765 3e60 5f0a  -model-usage>`_.
+000014c0: 0a43 6861 6e67 6564 0a7e 7e7e 7e7e 7e7e  .Changed.~~~~~~~
+000014d0: 0a2a 2054 6865 203a 636c 6173 733a 602e  .* The :class:`.
+000014e0: 4942 414e 6020 616e 6420 3a63 6c61 7373  IBAN` and :class
+000014f0: 3a60 2e42 4943 6020 636c 6173 7365 7320  :`.BIC` classes 
+00001500: 6172 6520 6e6f 7720 7375 6263 6c61 7373  are now subclass
+00001510: 6573 206f 6620 3a63 6c61 7373 3a60 7374  es of :class:`st
+00001520: 7260 2073 6f20 7468 6174 2061 6c6c 2073  r` so that all s
+00001530: 7472 696e 670a 2020 7265 6c61 7465 6420  tring.  related 
+00001540: 6d65 7468 6f64 7320 616e 6420 6675 6e63  methods and func
+00001550: 7469 6f6e 616c 6c69 7469 6573 2028 652e  tionallities (e.
+00001560: 672e 2073 6c69 6369 6e67 2920 6172 6520  g. slicing) are 
+00001570: 6469 7265 6374 6c79 2061 7661 696c 6162  directly availab
+00001580: 6c65 2e0a 0a60 3230 3233 2e30 392e 3060  le...`2023.09.0`
+00001590: 5f20 2d20 3230 3233 2f30 392f 3235 0a2d  _ - 2023/09/25.-
+000015a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000015b0: 2d2d 2d2d 2d2d 2d2d 0a52 656d 6f76 6564  --------.Removed
+000015c0: 0a7e 7e7e 7e7e 7e7e 0a2a 2053 7570 706f  .~~~~~~~.* Suppo
+000015d0: 7274 2066 6f72 2050 7974 686f 6e20 332e  rt for Python 3.
+000015e0: 3720 6861 7320 6265 656e 2064 726f 7070  7 has been dropp
+000015f0: 6564 2e0a 0a41 6464 6564 0a7e 7e7e 7e7e  ed...Added.~~~~~
+00001600: 0a2a 204e 6577 206d 6574 686f 6420 3a6d  .* New method :m
+00001610: 6574 683a 602e 4249 432e 6361 6e64 6964  eth:`.BIC.candid
+00001620: 6174 6573 5f66 726f 6d5f 6261 6e6b 5f63  ates_from_bank_c
+00001630: 6f64 6560 2074 6f20 6c69 7374 2061 6c6c  ode` to list all
+00001640: 206d 6174 6368 696e 6720 4249 4373 2074   matching BICs t
+00001650: 6f20 6120 6769 7665 6e20 646f 6d65 7374  o a given domest
+00001660: 6963 0a20 2062 616e 6b20 636f 6465 2060  ic.  bank code `
+00001670: 404e 6174 696d 203c 6874 7470 733a 2f2f  @Natim <https://
+00001680: 6769 7468 7562 2e63 6f6d 2f4e 6174 696d  github.com/Natim
+00001690: 3e60 5f2e 0a0a 4368 616e 6765 640a 7e7e  >`_...Changed.~~
+000016a0: 7e7e 7e7e 7e0a 2a20 5468 6520 4974 616c  ~~~~~.* The Ital
+000016b0: 6961 6e20 6261 6e6b 2072 6567 6973 7472  ian bank registr
+000016c0: 7920 6973 206e 6f77 2061 7574 6f6d 6174  y is now automat
+000016d0: 6963 616c 6c79 2067 656e 6572 6174 6564  ically generated
+000016e0: 2074 6861 6e6b 7320 746f 0a20 2060 404b   thanks to.  `@K
+000016f0: 7279 7374 6f66 6565 203c 6874 7470 733a  rystofee <https:
+00001700: 2f2f 6769 7468 7562 2e63 6f6d 2f4b 7279  //github.com/Kry
+00001710: 7374 6f66 6565 3e60 5f0a 0a49 6e74 6572  stofee>`_..Inter
+00001720: 6e61 6c0a 7e7e 7e7e 7e7e 7e7e 0a2a 2053  nal.~~~~~~~~.* S
+00001730: 7769 7463 6820 7072 6f6a 6563 7420 746f  witch project to
+00001740: 6f6c 696e 6720 746f 2060 6861 7463 6820  oling to `hatch 
+00001750: 3c68 7474 7073 3a2f 2f68 6174 6368 2e70  <https://hatch.p
+00001760: 7970 612e 696f 2f6c 6174 6573 742f 3e60  ypa.io/latest/>`
+00001770: 5f2e 0a2a 2055 7365 2060 7275 6666 203c  _..* Use `ruff <
+00001780: 6874 7470 733a 2f2f 646f 6373 2e61 7374  https://docs.ast
+00001790: 7261 6c2e 7368 2f72 7566 662f 3e60 5f20  ral.sh/ruff/>`_ 
+000017a0: 696e 7374 6561 6420 6f66 205b 666c 616b  instead of [flak
+000017b0: 6538 5d28 6874 7470 733a 2f2f 666c 616b  e8](https://flak
+000017c0: 6538 2e70 7963 7161 2e6f 7267 2f65 6e2f  e8.pycqa.org/en/
+000017d0: 6c61 7465 7374 2f29 0a20 2061 7320 6c69  latest/).  as li
+000017e0: 6e74 6572 2e0a 2a20 5570 6772 6164 6520  nter..* Upgrade 
+000017f0: 606d 7970 7920 3c68 7474 7073 3a2f 2f77  `mypy <https://w
+00001800: 7777 2e6d 7970 792d 6c61 6e67 2e6f 7267  ww.mypy-lang.org
+00001810: 2f3e 605f 2074 6f20 312e 352e 3120 616e  />`_ to 1.5.1 an
+00001820: 6420 6669 7820 616c 6c20 6e65 7720 7479  d fix all new ty
+00001830: 7069 6e67 2065 7272 6f72 732e 0a0a 6032  ping errors...`2
+00001840: 3032 332e 3036 2e30 605f 202d 2032 3032  023.06.0`_ - 202
+00001850: 332f 3036 2f32 310a 2d2d 2d2d 2d2d 2d2d  3/06/21.--------
+00001860: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001870: 2d0a 4669 7865 640a 7e7e 7e7e 7e0a 2a20  -.Fixed.~~~~~.* 
+00001880: 466f 7220 556b 7261 696e 6961 6e20 6261  For Ukrainian ba
+00001890: 6e6b 7320 6361 6c6c 696e 6720 6060 6962  nks calling ``ib
+000018a0: 616e 2e62 6963 6060 2064 6964 2072 6573  an.bic`` did res
+000018b0: 756c 7420 696e 2061 2060 6054 7970 6545  ult in a ``TypeE
+000018c0: 7272 6f72 6060 2e20 5468 616e 6b73 0a20  rror``. Thanks. 
+000018d0: 2060 4062 6572 6e6f 7265 6974 736d 6120   `@bernoreitsma 
+000018e0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+000018f0: 636f 6d2f 6265 726e 6f72 6569 7473 6d61  com/bernoreitsma
+00001900: 3e60 5f20 666f 7220 7265 706f 7274 696e  >`_ for reportin
+00001910: 672e 0a0a 4368 616e 6765 640a 7e7e 7e7e  g...Changed.~~~~
+00001920: 7e7e 7e0a 2a20 5570 6461 7465 6420 6765  ~~~.* Updated ge
+00001930: 6e65 7261 7465 6420 6261 6e6b 2072 6567  nerated bank reg
+00001940: 6973 7472 6965 7320 666f 7220 4175 7374  istries for Aust
+00001950: 7269 612c 2042 656c 6769 756d 2c20 437a  ria, Belgium, Cz
+00001960: 6563 6820 5265 7075 626c 6963 2c20 4765  ech Republic, Ge
+00001970: 726d 616e 792c 204e 6574 6865 726c 616e  rmany, Netherlan
+00001980: 6473 2c0a 2020 4875 6e67 6172 792c 204e  ds,.  Hungary, N
+00001990: 6f72 7761 792c 2050 6f6c 616e 6420 616e  orway, Poland an
+000019a0: 6420 556b 7261 696e 652e 0a0a 0a60 3230  d Ukraine....`20
+000019b0: 3233 2e30 332e 3060 5f20 2d20 3230 3233  23.03.0`_ - 2023
+000019c0: 2f30 332f 3134 0a2d 2d2d 2d2d 2d2d 2d2d  /03/14.---------
+000019d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000019e0: 0a43 6861 6e67 6564 0a7e 7e7e 7e7e 7e7e  .Changed.~~~~~~~
+000019f0: 0a2a 2055 7064 6174 6564 2067 656e 6572  .* Updated gener
+00001a00: 6174 6564 2062 616e 6b20 7265 6769 7374  ated bank regist
+00001a10: 7269 6573 2066 6f72 2041 7573 7472 6961  ries for Austria
+00001a20: 2c20 4265 6c67 6975 6d2c 2047 6572 6d61  , Belgium, Germa
+00001a30: 6e79 2c20 4e65 7468 6572 6c61 6e64 732c  ny, Netherlands,
+00001a40: 0a20 2048 756e 6761 7279 2c20 536c 6f76  .  Hungary, Slov
+00001a50: 656e 6961 2061 6e64 2055 6b72 6169 6e65  enia and Ukraine
+00001a60: 2e0a 0a41 6464 6564 0a7e 7e7e 7e7e 0a2a  ...Added.~~~~~.*
+00001a70: 204e 6577 2062 616e 6b20 7265 6769 7374   New bank regist
+00001a80: 7279 2066 6f72 204e 6f72 7761 7920 7468  ry for Norway th
+00001a90: 616e 6b73 2074 6f20 6040 657a 6574 203c  anks to `@ezet <
+00001aa0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001ab0: 6f6d 2f65 7a65 743e 605f 0a0a 6032 3032  om/ezet>`_..`202
+00001ac0: 332e 3032 2e31 605f 202d 2032 3032 332f  3.02.1`_ - 2023/
+00001ad0: 3032 2f32 380a 2d2d 2d2d 2d2d 2d2d 2d2d  02/28.----------
+00001ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00001af0: 4669 7865 640a 7e7e 7e7e 7e0a 2a20 5468  Fixed.~~~~~.* Th
+00001b00: 6520 646f 6d65 7374 6963 2063 6865 636b  e domestic check
+00001b10: 7375 6d20 6361 6c63 756c 6174 696f 6e20  sum calculation 
+00001b20: 666f 7220 4265 6c67 6975 6d20 6e6f 7720  for Belgium now 
+00001b30: 7265 7475 726e 7320 3937 2069 6e20 6361  returns 97 in ca
+00001b40: 7365 2074 6865 206d 6f64 756c 6f20 6f70  se the modulo op
+00001b50: 6572 6174 696f 6e0a 2020 7265 7375 6c74  eration.  result
+00001b60: 7320 696e 2030 2e20 6040 6d68 656d 6572  s in 0. `@mhemer
+00001b70: 7963 6b20 3c68 7474 7073 3a2f 2f67 6974  yck <https://git
+00001b80: 6875 622e 636f 6d2f 6d68 656d 6572 7963  hub.com/mhemeryc
+00001b90: 6b3e 605f 0a0a 4368 616e 6765 640a 7e7e  k>`_..Changed.~~
+00001ba0: 7e7e 7e7e 7e0a 2a20 5570 6461 7465 6420  ~~~~~.* Updated 
+00001bb0: 6765 6e65 7261 7465 6420 6261 6e6b 2072  generated bank r
+00001bc0: 6567 6973 7472 6965 7320 666f 7220 4175  egistries for Au
+00001bd0: 7374 7269 612c 2042 656c 6769 756d 2c20  stria, Belgium, 
+00001be0: 437a 6563 6820 5265 7075 626c 6963 2c20  Czech Republic, 
+00001bf0: 4765 726d 616e 792c 2053 7061 696e 2c0a  Germany, Spain,.
+00001c00: 2020 4875 6e67 6172 7920 616e 6420 4372    Hungary and Cr
+00001c10: 6f61 7469 612e 0a0a 6032 3032 332e 3032  oatia...`2023.02
+00001c20: 2e30 605f 202d 2032 3032 332f 3032 2f30  .0`_ - 2023/02/0
+00001c30: 360a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  6.--------------
+00001c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 4164 6465  -----------.Adde
+00001c50: 640a 7e7e 7e7e 7e0a 2a20 4e65 7720 6261  d.~~~~~.* New ba
+00001c60: 6e6b 7320 666f 7220 506f 7274 7567 616c  nks for Portugal
+00001c70: 2061 6e64 2049 7461 6c79 2060 4064 656e   and Italy `@den
+00001c80: 6e69 7378 7472 6961 203c 6874 7470 733a  nisxtria <https:
+00001c90: 2f2f 6769 7468 7562 2e63 6f6d 2f64 656e  //github.com/den
+00001ca0: 6e69 7378 7472 6961 3e60 5f0a 2a20 4164  nisxtria>`_.* Ad
+00001cb0: 6465 6420 7375 7070 6f72 7420 666f 7220  ded support for 
+00001cc0: 556b 7261 696e 6961 6e20 6261 6e6b 7320  Ukrainian banks 
+00001cd0: 6040 7368 7069 6775 6e6f 7620 3c68 7474  `@shpigunov <htt
+00001ce0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00001cf0: 7368 7069 6775 6e6f 763e 605f 0a0a 4669  shpigunov>`_..Fi
+00001d00: 7865 640a 7e7e 7e7e 7e0a 2a20 436f 7272  xed.~~~~~.* Corr
+00001d10: 6563 7465 6420 6261 6e6b 2063 6f64 6573  ected bank codes
+00001d20: 2066 6f72 2043 7970 7269 6f74 2062 616e   for Cypriot ban
+00001d30: 6b73 2060 404b 7279 7374 6f66 6565 203c  ks `@Krystofee <
+00001d40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001d50: 6f6d 2f4b 7279 7374 6f66 6565 3e60 5f0a  om/Krystofee>`_.
+00001d60: 0a60 3230 3232 2e30 392e 3060 5f20 2d20  .`2022.09.0`_ - 
+00001d70: 3230 3232 2f31 362f 3039 0a2d 2d2d 2d2d  2022/16/09.-----
+00001d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001d90: 2d2d 2d2d 0a41 6464 6564 0a7e 7e7e 7e7e  ----.Added.~~~~~
+00001da0: 0a2a 2049 4241 4e20 7661 6c69 6461 7469  .* IBAN validati
+00001db0: 6f6e 2066 6f72 2053 656e 6567 616c 2060  on for Senegal `
+00001dc0: 6d6b 6f70 6563 3837 203c 6874 7470 733a  mkopec87 <https:
+00001dd0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6b6f  //github.com/mko
+00001de0: 7065 6338 373e 605f 0a0a 4368 616e 6765  pec87>`_..Change
+00001df0: 640a 7e7e 7e7e 7e7e 7e0a 2a20 5265 6661  d.~~~~~~~.* Refa
+00001e00: 6374 6f72 6564 206d 6f73 7420 6f66 2074  ctored most of t
+00001e10: 6865 2073 6372 6970 7473 2074 6f20 6765  he scripts to ge
+00001e20: 6e65 7261 7465 2074 6865 2062 616e 6b20  nerate the bank 
+00001e30: 7265 6769 7374 7279 2074 6f20 7573 6520  registry to use 
+00001e40: 5061 6e64 6173 2060 4070 6562 6f73 6920  Pandas `@pebosi 
+00001e50: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+00001e60: 636f 6d2f 7065 626f 7369 3e60 5f0a 2a20  com/pebosi>`_.* 
+00001e70: 5570 6461 7465 6420 6261 6e6b 2072 6567  Updated bank reg
+00001e80: 6973 7472 7920 666f 7220 4175 7374 7269  istry for Austri
+00001e90: 612c 2042 656c 6769 756d 2c20 4765 726d  a, Belgium, Germ
+00001ea0: 616e 792c 2053 7061 696e 2c20 4875 6e67  any, Spain, Hung
+00001eb0: 6172 792c 204e 6574 6865 726c 616e 6473  ary, Netherlands
+00001ec0: 2061 6e64 2050 6f6c 616e 642e 0a0a 6032   and Poland...`2
+00001ed0: 3032 322e 3037 2e31 605f 202d 2032 3032  022.07.1`_ - 202
+00001ee0: 322f 3238 2f30 370a 2d2d 2d2d 2d2d 2d2d  2/28/07.--------
+00001ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001f00: 2d0a 4669 7865 640a 7e7e 7e7e 7e0a 2a20  -.Fixed.~~~~~.* 
+00001f10: 496e 2073 6f6d 6520 636f 756e 7472 6965  In some countrie
+00001f20: 7320 7468 6520 4242 414e 2064 6f65 7320  s the BBAN does 
+00001f30: 6e6f 7420 696e 636c 7564 6520 6120 6261  not include a ba
+00001f40: 6e6b 2063 6f64 652c 2062 7574 206f 6e6c  nk code, but onl
+00001f50: 7920 6120 6272 616e 6368 2063 6f64 6520  y a branch code 
+00001f60: 2865 2e67 2e20 506f 6c61 6e64 292e 2049  (e.g. Poland). I
+00001f70: 6e0a 2020 7468 6f73 6520 6361 7365 7320  n.  those cases 
+00001f80: 7468 6520 6272 616e 6368 2063 6f64 6520  the branch code 
+00001f90: 7368 6f75 6c64 2062 6520 7573 6564 2074  should be used t
+00001fa0: 6f20 6c6f 6f6b 7570 2074 6865 2062 616e  o lookup the ban
+00001fb0: 6b20 6173 736f 6369 6174 6564 2074 6f20  k associated to 
+00001fc0: 616e 2049 4241 4e20 696e 7374 6561 6420  an IBAN instead 
+00001fd0: 6f66 2074 6865 0a20 206f 6276 696f 7573  of the.  obvious
+00001fe0: 6c79 2065 6d70 7479 2062 616e 6b20 636f  ly empty bank co
+00001ff0: 6465 2e0a 0a60 3230 3232 2e30 372e 3060  de...`2022.07.0`
+00002000: 5f20 2d20 3230 3232 2f30 372f 3037 0a2d  _ - 2022/07/07.-
+00002010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002020: 2d2d 2d2d 2d2d 2d2d 0a46 6978 6564 0a7e  --------.Fixed.~
+00002030: 7e7e 7e7e 0a2a 2048 756e 6761 7269 616e  ~~~~.* Hungarian
+00002040: 2062 616e 6b20 7265 6769 7374 7279 2067   bank registry g
+00002050: 656e 6572 6174 6f72 2073 6372 6970 7420  enerator script 
+00002060: 7761 7320 6669 7865 6420 6279 2060 404b  was fixed by `@K
+00002070: 7279 7374 6f66 6565 203c 6874 7470 733a  rystofee <https:
+00002080: 2f2f 6769 7468 7562 2e63 6f6d 2f4b 7279  //github.com/Kry
+00002090: 7374 6f66 6565 3e60 5f0a 0a60 3230 3232  stofee>`_..`2022
+000020a0: 2e30 362e 3360 5f20 2d20 3230 3232 2f30  .06.3`_ - 2022/0
+000020b0: 362f 3239 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  6/29.-----------
+000020c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a41  --------------.A
+000020d0: 6464 6564 0a7e 7e7e 7e7e 0a2a 2047 656e  dded.~~~~~.* Gen
+000020e0: 6572 6174 6564 206c 6973 7420 6f66 204c  erated list of L
+000020f0: 6974 6875 616e 6961 6e20 4249 4373 2060  ithuanian BICs `
+00002100: 4044 7261 7567 656c 6973 203c 6874 7470  @Draugelis <http
+00002110: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f44  s://github.com/D
+00002120: 7261 7567 656c 6973 3e60 5f0a 2a20 5265  raugelis>`_.* Re
+00002130: 6d6f 7665 6420 6d61 6e75 616c 6c79 2063  moved manually c
+00002140: 7572 6174 6564 206c 6973 7420 6f66 204c  urated list of L
+00002150: 6974 6875 616e 6961 6e20 6261 6e6b 732e  ithuanian banks.
+00002160: 0a0a 6032 3032 322e 3036 2e32 605f 202d  ..`2022.06.2`_ -
+00002170: 2032 3032 322f 3036 2f32 320a 2d2d 2d2d   2022/06/22.----
+00002180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002190: 2d2d 2d2d 2d0a 4164 6465 640a 7e7e 7e7e  -----.Added.~~~~
+000021a0: 7e0a 2a20 4765 6e65 7261 7465 6420 6c69  ~.* Generated li
+000021b0: 7374 206f 6620 4772 6565 6b20 4249 4373  st of Greek BICs
+000021c0: 2060 406b 6f75 6e61 6269 2020 3c68 7474   `@kounabi  <htt
+000021d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000021e0: 6b6f 756e 6162 693e 605f 0a2a 2047 656e  kounabi>`_.* Gen
+000021f0: 6572 6174 6564 206c 6973 7420 6f66 2043  erated list of C
+00002200: 7970 7269 6f74 2042 4943 7320 6040 6b6f  ypriot BICs `@ko
+00002210: 756e 6162 6920 203c 6874 7470 733a 2f2f  unabi  <https://
+00002220: 6769 7468 7562 2e63 6f6d 2f6b 6f75 6e61  github.com/kouna
+00002230: 6269 3e60 5f0a 0a43 6861 6e67 6564 0a7e  bi>`_..Changed.~
+00002240: 7e7e 7e7e 7e7e 0a2a 2055 7064 6174 6564  ~~~~~~.* Updated
+00002250: 2062 616e 6b20 7265 6769 7374 7279 2066   bank registry f
+00002260: 6f72 2041 7573 7472 6961 2c20 4265 6c67  or Austria, Belg
+00002270: 6975 6d2c 2043 7a65 6368 2052 6570 7562  ium, Czech Repub
+00002280: 6c69 632c 2047 6572 6d61 6e79 2c20 4372  lic, Germany, Cr
+00002290: 6f61 7469 612c 204e 6574 6865 726c 616e  oatia, Netherlan
+000022a0: 6473 2c20 506f 6c61 6e64 0a20 2061 6e64  ds, Poland.  and
+000022b0: 2053 6c6f 7665 6e69 612e 0a0a 4669 7865   Slovenia...Fixe
+000022c0: 640a 7e7e 7e7e 7e0a 2a20 5468 6520 646f  d.~~~~~.* The do
+000022d0: 6d65 7374 6963 2062 616e 6b20 636f 6465  mestic bank code
+000022e0: 2066 6f72 2048 756e 6761 7269 616e 2062   for Hungarian b
+000022f0: 616e 6b73 2077 6173 2077 726f 6e67 6c79  anks was wrongly
+00002300: 2067 656e 6572 6174 6564 2060 404b 7279   generated `@Kry
+00002310: 7374 6f66 6565 203c 6874 7470 733a 2f2f  stofee <https://
+00002320: 6769 7468 7562 2e63 6f6d 2f4b 7279 7374  github.com/Kryst
+00002330: 6f66 6565 3e60 5f0a 0a60 3230 3232 2e30  ofee>`_..`2022.0
+00002340: 362e 3160 5f20 2d20 3230 3232 2f30 362f  6.1`_ - 2022/06/
+00002350: 3036 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  06.-------------
+00002360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4164  ------------..Ad
+00002370: 6465 640a 7e7e 7e7e 7e0a 2a20 4765 6e65  ded.~~~~~.* Gene
+00002380: 7261 7465 6420 6c69 7374 206f 6620 526f  rated list of Ro
+00002390: 6d61 6e69 616e 2042 4943 7320 6040 4b72  manian BICs `@Kr
+000023a0: 7973 746f 6665 6520 3c68 7474 7073 3a2f  ystofee <https:/
+000023b0: 2f67 6974 6875 622e 636f 6d2f 4b72 7973  /github.com/Krys
+000023c0: 746f 6665 653e 605f 0a2a 2047 656e 6572  tofee>`_.* Gener
+000023d0: 6174 6564 206c 6973 7420 6f66 2048 756e  ated list of Hun
+000023e0: 6761 7269 616e 2042 4943 7320 6040 4b72  garian BICs `@Kr
+000023f0: 7973 746f 6665 6520 3c68 7474 7073 3a2f  ystofee <https:/
+00002400: 2f67 6974 6875 622e 636f 6d2f 4b72 7973  /github.com/Krys
+00002410: 746f 6665 653e 605f 0a2a 2045 7874 656e  tofee>`_.* Exten
+00002420: 6465 6420 6d61 6e75 616c 6c79 2063 7572  ded manually cur
+00002430: 6174 6564 206c 6973 7420 6f66 2049 7269  ated list of Iri
+00002440: 7368 2042 4943 7320 6040 6465 6e6e 6973  sh BICs `@dennis
+00002450: 7874 7269 6120 3c68 7474 7073 3a2f 2f67  xtria <https://g
+00002460: 6974 6875 622e 636f 6d2f 6465 6e6e 6973  ithub.com/dennis
+00002470: 7874 7269 613e 605f 0a0a 0a60 3230 3232  xtria>`_...`2022
+00002480: 2e30 362e 3060 5f20 2d20 3230 3232 2f30  .06.0`_ - 2022/0
+00002490: 362f 3036 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  6/06.-----------
+000024a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+000024b0: 4164 6465 640a 7e7e 7e7e 7e0a 2a20 4d61  Added.~~~~~.* Ma
+000024c0: 6e75 616c 6c79 2063 7572 6174 6564 206c  nually curated l
+000024d0: 6973 7420 6f66 2042 756c 6761 7269 616e  ist of Bulgarian
+000024e0: 2042 4943 7320 6040 4b72 7973 746f 6665   BICs `@Krystofe
+000024f0: 6520 3c68 7474 7073 3a2f 2f67 6974 6875  e <https://githu
+00002500: 622e 636f 6d2f 4b72 7973 746f 6665 653e  b.com/Krystofee>
+00002510: 605f 0a2a 204d 616e 7561 6c6c 7920 6375  `_.* Manually cu
+00002520: 7261 7465 6420 6c69 7374 206f 6620 5361  rated list of Sa
+00002530: 7564 6920 4172 6162 6961 6e20 4249 4373  udi Arabian BICs
+00002540: 2060 4073 616d 697a 616d 616e 203c 6874   `@samizaman <ht
+00002550: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002560: 2f73 616d 697a 616d 616e 3e60 5f0a 2a20  /samizaman>`_.* 
+00002570: 5375 7070 6f72 7420 666f 7220 6050 7949  Support for `PyI
+00002580: 6e73 7461 6c6c 6572 203c 6874 7470 733a  nstaller <https:
+00002590: 2f2f 7079 696e 7374 616c 6c65 722e 6f72  //pyinstaller.or
+000025a0: 672f 656e 2f73 7461 626c 652f 3e60 5f20  g/en/stable/>`_ 
+000025b0: 6040 4c75 6b61 737a 3837 203c 6874 7470  `@Lukasz87 <http
+000025c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
+000025d0: 756b 6173 7a38 373e 605f 0a0a 496e 7465  ukasz87>`_..Inte
+000025e0: 726e 616c 0a7e 7e7e 7e7e 7e7e 7e0a 2a20  rnal.~~~~~~~~.* 
+000025f0: 5275 6e20 7465 7374 7320 6f6e 2050 7974  Run tests on Pyt
+00002600: 686f 6e20 332e 3130 2060 4061 6461 6d63  hon 3.10 `@adamc
+00002610: 6861 696e 7a20 3c68 7474 7073 3a2f 2f67  hainz <https://g
+00002620: 6974 6875 622e 636f 6d2f 6164 616d 6368  ithub.com/adamch
+00002630: 6169 6e7a 3e60 5f0a 2a20 5573 6520 7374  ainz>`_.* Use st
+00002640: 616e 6461 7264 206b 6579 7320 696e 2060  andard keys in `
+00002650: 6073 6574 7570 2e63 6667 6060 2060 4061  `setup.cfg`` `@a
+00002660: 6461 6d63 6861 696e 7a20 3c68 7474 7073  damchainz <https
+00002670: 3a2f 2f67 6974 6875 622e 636f 6d2f 6164  ://github.com/ad
+00002680: 616d 6368 6169 6e7a 3e60 5f0a 2a20 446f  amchainz>`_.* Do
+00002690: 6e27 7420 7265 6c79 206f 6e20 6060 6861  n't rely on ``ha
+000026a0: 636b 696e 6760 6020 696e 2074 6573 742d  cking`` in test-
+000026b0: 7365 7475 7020 6040 6164 616d 6368 6169  setup `@adamchai
+000026c0: 6e7a 203c 6874 7470 733a 2f2f 6769 7468  nz <https://gith
+000026d0: 7562 2e63 6f6d 2f61 6461 6d63 6861 696e  ub.com/adamchain
+000026e0: 7a3e 605f 0a0a 6032 3032 322e 3034 2e32  z>`_..`2022.04.2
+000026f0: 605f 202d 2032 3032 322f 3034 2f32 390a  `_ - 2022/04/29.
+00002700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002710: 2d2d 2d2d 2d2d 2d2d 2d0a 0a43 6861 6e67  ---------..Chang
+00002720: 6564 0a7e 7e7e 7e7e 7e7e 0a2a 2041 6c6c  ed.~~~~~~~.* All
+00002730: 6f77 2067 6574 7469 6e67 2062 616e 6b20  ow getting bank 
+00002740: 6e61 6d65 7320 6672 6f6d 2049 4241 4e2e  names from IBAN.
+00002750: 2050 7265 7669 6f75 736c 792c 2079 6f75   Previously, you
+00002760: 2063 6f75 6c64 2064 6f20 6060 6962 616e   could do ``iban
+00002770: 2e62 6963 2e62 616e 6b5f 6e61 6d65 735b  .bic.bank_names[
+00002780: 305d 6060 2c20 6275 7420 7369 6e63 650a  0]``, but since.
+00002790: 2020 6120 4249 4320 6361 6e20 6265 2061    a BIC can be a
+000027a0: 7373 6f63 6961 7465 6420 746f 206d 756c  ssociated to mul
+000027b0: 7469 706c 6520 6261 6e6b 2063 6f64 6573  tiple bank codes
+000027c0: 2074 6865 2063 6f6e 7465 7874 206f 6620   the context of 
+000027d0: 7468 6520 7370 6563 6966 6963 2062 616e  the specific ban
+000027e0: 6b20 6973 206c 6f73 7420 616e 6420 796f  k is lost and yo
+000027f0: 750a 2020 636f 756c 6420 656e 6420 7570  u.  could end up
+00002800: 2077 6974 6820 7468 6520 7772 6f6e 6720   with the wrong 
+00002810: 6261 6e6b 206e 616d 652e 2060 406a 6f73  bank name. `@jos
+00002820: 652d 7265 7665 6e69 203c 6874 7470 733a  e-reveni <https:
+00002830: 2f2f 6769 7468 7562 2e63 6f6d 2f6a 6f73  //github.com/jos
+00002840: 652d 7265 7665 6e69 3e60 5f0a 0a0a 6032  e-reveni>`_...`2
+00002850: 3032 322e 3034 2e31 605f 202d 2032 3032  022.04.1`_ - 202
+00002860: 322f 3034 2f32 390a 2d2d 2d2d 2d2d 2d2d  2/04/29.--------
+00002870: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002880: 2d0a 0a43 6861 6e67 6564 0a7e 7e7e 7e7e  -..Changed.~~~~~
+00002890: 7e7e 0a2a 2054 6865 2049 7461 6c69 616e  ~~.* The Italian
+000028a0: 2042 4241 4e20 6368 6563 6b73 756d 2061   BBAN checksum a
+000028b0: 6c67 6f72 6974 686d 2069 7320 6e6f 7720  lgorithm is now 
+000028c0: 616c 736f 2061 7070 6c69 6564 2066 6f72  also applied for
+000028d0: 2053 616e 204d 6172 696e 6f20 6040 6661   San Marino `@fa
+000028e0: 6269 656e 7065 203c 6874 7470 733a 2f2f  bienpe <https://
+000028f0: 6769 7468 7562 2e63 6f6d 2f66 6162 6965  github.com/fabie
+00002900: 6e70 653e 605f 0a0a 4669 7865 640a 7e7e  npe>`_..Fixed.~~
+00002910: 7e7e 7e0a 2a20 4669 7820 4974 616c 6961  ~~~.* Fix Italia
+00002920: 6e20 4242 414e 2063 6865 636b 7375 6d20  n BBAN checksum 
+00002930: 6361 6c63 756c 6174 696f 6e20 6023 3738  calculation `#78
+00002940: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
+00002950: 2e63 6f6d 2f6d 646f 6d6b 652f 7363 6877  .com/mdomke/schw
+00002960: 6966 7479 2f69 7373 7565 732f 3738 3e60  ifty/issues/78>`
+00002970: 5f0a 2a20 4669 7820 6261 6e6b 2063 6f64  _.* Fix bank cod
+00002980: 6520 706f 7369 7469 6f6e 2069 6e20 4242  e position in BB
+00002990: 414e 2066 6f72 204a 6f72 6461 6e20 6261  AN for Jordan ba
+000029a0: 6e6b 7320 6040 6661 6269 656e 7065 203c  nks `@fabienpe <
+000029b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000029c0: 6f6d 2f66 6162 6965 6e70 653e 605f 0a0a  om/fabienpe>`_..
+000029d0: 0a60 3230 3232 2e30 342e 3060 5f20 2d20  .`2022.04.0`_ - 
+000029e0: 3230 3232 2f30 342f 3131 0a2d 2d2d 2d2d  2022/04/11.-----
+000029f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002a00: 2d2d 2d2d 0a0a 4368 616e 6765 640a 7e7e  ----..Changed.~~
+00002a10: 7e7e 7e7e 7e0a 2a20 5570 6461 7465 2062  ~~~~~.* Update b
+00002a20: 616e 6b20 7265 6769 7374 7279 2066 6f72  ank registry for
+00002a30: 2041 7573 7472 6961 2c20 437a 6563 6820   Austria, Czech 
+00002a40: 5265 7075 626c 6963 2c20 4765 726d 616e  Republic, German
+00002a50: 792c 2053 7061 696e 2c20 506f 6c61 6e64  y, Spain, Poland
+00002a60: 2061 6e64 2053 6c6f 7661 6b69 612e 0a0a   and Slovakia...
+00002a70: 4669 7865 640a 7e7e 7e7e 7e0a 2a20 5265  Fixed.~~~~~.* Re
+00002a80: 6d6f 7665 6420 626f 6775 7320 6c69 6e65  moved bogus line
+00002a90: 2066 726f 6d20 6475 7463 6820 6261 6e6b   from dutch bank
+00002aa0: 2072 6567 6973 7472 792e 0a2a 204c 6f61   registry..* Loa
+00002ab0: 6469 6e67 2074 6865 2062 616e 6b20 7265  ding the bank re
+00002ac0: 6769 7374 7279 206e 6f77 2061 6c73 6f20  gistry now also 
+00002ad0: 776f 726b 7320 6f6e 206d 6163 6869 6e65  works on machine
+00002ae0: 7320 7468 6174 2064 6f6e 2774 2068 6176  s that don't hav
+00002af0: 6520 5554 462d 3820 6173 2074 6865 6972  e UTF-8 as their
+00002b00: 2064 6566 6175 6c74 0a20 2065 6e63 6f64   default.  encod
+00002b10: 696e 6720 6040 696d 6164 3376 203c 6874  ing `@imad3v <ht
+00002b20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00002b30: 2f69 6d61 6433 763e 605f 0a0a 0a60 3230  /imad3v>`_...`20
+00002b40: 3232 2e30 332e 3160 5f20 2d20 3230 3232  22.03.1`_ - 2022
+00002b50: 2f30 332f 3035 0a2d 2d2d 2d2d 2d2d 2d2d  /03/05.---------
+00002b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002b70: 0a0a 4164 6465 640a 7e7e 7e7e 7e0a 2a20  ..Added.~~~~~.* 
+00002b80: 436f 756e 7472 7920 7370 6563 6966 6320  Country specifc 
+00002b90: 6368 6563 6b73 756d 2076 616c 6964 6174  checksum validat
+00002ba0: 696f 6e20 666f 7220 4672 656e 6368 2062  ion for French b
+00002bb0: 616e 6b73 2028 6261 7365 6420 6f6e 2074  anks (based on t
+00002bc0: 6865 2077 6f72 6b20 6f66 0a20 2060 4073  he work of.  `@s
+00002bd0: 686f 6c61 6e20 3c68 7474 7073 3a2f 2f67  holan <https://g
+00002be0: 6974 6875 622e 636f 6d2f 7368 6f6c 616e  ithub.com/sholan
+00002bf0: 3e60 5f29 0a0a 0a60 3230 3232 2e30 332e  >`_)...`2022.03.
+00002c00: 3060 5f20 2d20 3230 3232 2f30 332f 3034  0`_ - 2022/03/04
+00002c10: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
+00002c20: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4164 6465  ----------..Adde
+00002c30: 640a 7e7e 7e7e 7e0a 2a20 5468 6520 3a63  d.~~~~~.* The :c
+00002c40: 6c61 7373 3a60 2e49 4241 4e60 2061 6e64  lass:`.IBAN` and
+00002c50: 203a 636c 6173 733a 602e 4249 4360 2063   :class:`.BIC` c
+00002c60: 6c61 7373 6573 206e 6f77 2073 7570 706f  lasses now suppo
+00002c70: 7274 2074 6865 2060 605f 5f6c 656e 5f5f  rt the ``__len__
+00002c80: 6060 206d 6574 686f 6420 746f 2061 6c6c  `` method to all
+00002c90: 6f77 2061 206d 6f72 650a 2020 5079 7468  ow a more.  Pyth
+00002ca0: 6f6e 6963 2063 616c 6375 6c61 7469 6f6e  onic calculation
+00002cb0: 206f 6620 7468 6520 6c65 6e67 7468 2e0a   of the length..
+00002cc0: 0a43 6861 6e67 6564 0a7e 7e7e 7e7e 7e7e  .Changed.~~~~~~~
+00002cd0: 0a2a 2055 7064 6174 6520 6261 6e6b 2072  .* Update bank r
+00002ce0: 6567 6973 7472 7920 666f 7220 437a 6563  egistry for Czec
+00002cf0: 6820 5265 7075 626c 6963 2c20 5370 6169  h Republic, Spai
+00002d00: 6e2c 2048 756e 6761 7279 2c20 506f 6c61  n, Hungary, Pola
+00002d10: 6e64 2061 6e64 2053 6c6f 7661 6b69 612e  nd and Slovakia.
+00002d20: 0a0a 0a60 3230 3232 2e30 322e 3060 5f20  ...`2022.02.0`_ 
+00002d30: 2d20 3230 3232 2f30 322f 3135 0a2d 2d2d  - 2022/02/15.---
+00002d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002d50: 2d2d 2d2d 2d2d 0a0a 4164 6465 640a 7e7e  ------..Added.~~
+00002d60: 7e7e 7e0a 2a20 4e32 3620 4249 4320 666f  ~~~.* N26 BIC fo
+00002d70: 7220 5370 6169 6e20 6040 6272 756e 6f76  r Spain `@brunov
+00002d80: 696c 6120 3c68 7474 7073 3a2f 2f67 6974  ila <https://git
+00002d90: 6875 622e 636f 6d2f 6272 756e 6f76 696c  hub.com/brunovil
+00002da0: 613e 605f 0a2a 204d 616e 7561 6c6c 7920  a>`_.* Manually 
+00002db0: 6375 7261 7465 6420 656e 7472 6965 7320  curated entries 
+00002dc0: 666f 7220 6261 6e6b 7320 6672 6f6d 2049  for banks from I
+00002dd0: 6365 6c61 6e64 2060 4067 6175 7469 6e69  celand `@gautini
+00002de0: 6c73 203c 6874 7470 733a 2f2f 6769 7468  ls <https://gith
+00002df0: 7562 2e63 6f6d 2f67 6175 7469 6e69 6c73  ub.com/gautinils
+00002e00: 3e60 5f0a 0a43 6861 6e67 6564 0a7e 7e7e  >`_..Changed.~~~
+00002e10: 7e7e 7e7e 0a2a 2052 656d 6f76 6564 206d  ~~~~.* Removed m
+00002e20: 616e 7561 6c6c 7920 6375 7261 7465 6420  anually curated 
+00002e30: 6261 6e6b 2065 6e74 7269 6573 2066 6f72  bank entries for
+00002e40: 2053 7061 696e 2073 696e 6365 2061 6c6c   Spain since all
+00002e50: 2076 616c 7565 7320 7765 7265 2061 6c72   values were alr
+00002e60: 6561 6479 2070 6172 7420 6f66 0a20 2074  eady part of.  t
+00002e70: 6865 2067 656e 6572 6174 6564 2072 6567  he generated reg
+00002e80: 6973 7472 792e 0a2a 2055 7064 6174 6564  istry..* Updated
+00002e90: 2062 616e 6b20 7265 6769 7374 7279 2066   bank registry f
+00002ea0: 6f72 2041 7573 7472 6961 2c20 4265 6c67  or Austria, Belg
+00002eb0: 6975 6d2c 2043 7a65 6368 2052 6570 7562  ium, Czech Repub
+00002ec0: 6c69 632c 2047 6572 6d61 6e79 2c20 5370  lic, Germany, Sp
+00002ed0: 6169 6e2c 204e 6574 6865 726c 616e 6473  ain, Netherlands
+00002ee0: 2061 6e64 2050 6f6c 616e 640a 2a20 4164   and Poland.* Ad
+00002ef0: 6465 6420 6f76 6572 7772 6974 6520 666f  ded overwrite fo
+00002f00: 7220 4942 414e 2073 7065 6320 6f66 2043  r IBAN spec of C
+00002f10: 7a65 6368 2052 6570 7562 6c69 6320 616e  zech Republic an
+00002f20: 6420 4672 616e 6365 2e20 5468 6520 6272  d France. The br
+00002f30: 616e 6368 2061 6e64 2061 6363 6f75 6e74  anch and account
+00002f40: 2063 6f64 6520 706f 7369 7469 6f6e 730a   code positions.
+00002f50: 2020 6172 6520 7772 6f6e 676c 7920 7072    are wrongly pr
+00002f60: 6f76 6964 6564 2069 6e20 7468 6520 6f66  ovided in the of
+00002f70: 6669 6369 616c 2049 4241 4e20 7265 6769  ficial IBAN regi
+00002f80: 7374 7279 2e0a 0a60 3230 3231 2e31 302e  stry...`2021.10.
+00002f90: 3260 5f20 2d20 3230 3231 2f31 302f 3132  2`_ - 2021/10/12
+00002fa0: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
+00002fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4164 6465  ----------..Adde
+00002fc0: 640a 7e7e 7e7e 7e0a 2a20 4164 6465 6420  d.~~~~~.* Added 
+00002fd0: 3434 3020 6164 6469 7469 6f6e 616c 2062  440 additional b
+00002fe0: 616e 6b20 7265 636f 7264 7320 666f 7220  ank records for 
+00002ff0: 5370 6169 6e2e 0a0a 6032 3032 312e 3130  Spain...`2021.10
+00003000: 2e31 605f 202d 2032 3032 312f 3130 2f31  .1`_ - 2021/10/1
+00003010: 310a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  1.--------------
+00003020: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a43 6861  -----------..Cha
+00003030: 6e67 6564 0a7e 7e7e 7e7e 7e7e 0a2a 2055  nged.~~~~~~~.* U
+00003040: 7365 2060 696d 706f 7274 6c69 622e 7265  se `importlib.re
+00003050: 736f 7572 6365 7320 3c68 7474 7073 3a2f  sources <https:/
+00003060: 2f64 6f63 732e 7079 7468 6f6e 2e6f 7267  /docs.python.org
+00003070: 2f33 2e39 2f6c 6962 7261 7279 2f69 6d70  /3.9/library/imp
+00003080: 6f72 746c 6962 2e68 746d 6c23 6d6f 6475  ortlib.html#modu
+00003090: 6c65 2d69 6d70 6f72 746c 6962 2e72 6573  le-importlib.res
+000030a0: 6f75 7263 6573 3e60 5f0a 2020 666f 7220  ources>`_.  for 
+000030b0: 6c6f 6164 696e 6720 696e 7465 726e 616c  loading internal
+000030c0: 2072 6567 6973 7472 6965 732e 2054 6869   registries. Thi
+000030d0: 7320 7265 6d6f 7665 7320 7468 6520 6e65  s removes the ne
+000030e0: 6564 2074 6f20 6861 7665 2060 6073 6574  ed to have ``set
+000030f0: 7570 746f 6f6c 7360 6020 696e 7374 616c  uptools`` instal
+00003100: 6c65 642e 0a20 2054 6861 6e6b 2079 6f75  led..  Thank you
+00003110: 2060 4061 2d72 6563 6b6e 6167 656c 203c   `@a-recknagel <
+00003120: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003130: 6f6d 2f61 2d72 6563 6b6e 6167 656c 3e60  om/a-recknagel>`
+00003140: 5f20 666f 7220 7468 6520 6964 6561 210a  _ for the idea!.
+00003150: 0a46 6978 6564 0a7e 7e7e 7e7e 0a2a 2045  .Fixed.~~~~~.* E
+00003160: 6e73 7572 6520 7468 6174 2042 656c 6769  nsure that Belgi
+00003170: 616e 2042 4241 4e20 6368 6563 6b73 756d  an BBAN checksum
+00003180: 7320 6172 6520 616c 7761 7973 2032 2064  s are always 2 d
+00003190: 6967 6974 7320 6c6f 6e67 2e0a 0a60 3230  igits long...`20
+000031a0: 3231 2e31 302e 3060 5f20 2d20 3230 3231  21.10.0`_ - 2021
+000031b0: 2f31 302f 3031 0a2d 2d2d 2d2d 2d2d 2d2d  /10/01.---------
+000031c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000031d0: 0a0a 4164 6465 640a 7e7e 7e7e 7e0a 2a20  ..Added.~~~~~.* 
+000031e0: 4164 6465 6420 4942 414e 2073 7065 6320  Added IBAN spec 
+000031f0: 666f 7220 5375 6461 6e20 2853 4429 2e0a  for Sudan (SD)..
+00003200: 2a20 4164 6465 6420 616e 6420 6578 7465  * Added and exte
+00003210: 6e64 6564 206d 616e 7561 6c6c 7920 6375  nded manually cu
+00003220: 7261 7465 6420 6261 6e6b 2065 6e74 7269  rated bank entri
+00003230: 6573 2066 6f72 2054 7572 6b65 792c 2049  es for Turkey, I
+00003240: 7461 6c79 2c20 4973 7261 656c 2c20 4972  taly, Israel, Ir
+00003250: 656c 616e 642c 2053 7061 696e 2c0a 2020  eland, Spain,.  
+00003260: 5377 6974 7a65 726c 616e 6420 616e 6420  Switzerland and 
+00003270: 4465 6e6d 6172 6b20 6040 686f 776f 726b  Denmark `@howork
+00003280: 6f6e 203c 6874 7470 733a 2f2f 6769 7468  on <https://gith
+00003290: 7562 2e63 6f6d 2f68 6f77 6f72 6b6f 6e3e  ub.com/howorkon>
+000032a0: 605f 2e0a 0a43 6861 6e67 6564 0a7e 7e7e  `_...Changed.~~~
+000032b0: 7e7e 7e7e 0a2a 2055 7064 6174 6564 2062  ~~~~.* Updated b
+000032c0: 616e 6b20 7265 6769 7374 7279 2066 6f72  ank registry for
+000032d0: 2041 7573 7472 6961 2c20 4265 6c67 6975   Austria, Belgiu
+000032e0: 6d2c 2043 7a65 6368 2052 6570 7562 6c69  m, Czech Republi
+000032f0: 632c 2047 6572 6d61 6e79 2c20 4e65 7468  c, Germany, Neth
+00003300: 6572 6c61 6e64 732c 2050 6f6c 616e 642c  erlands, Poland,
+00003310: 0a20 2053 6c6f 7665 6e69 6120 616e 6420  .  Slovenia and 
+00003320: 536c 6f76 616b 6961 2e0a 0a46 6978 6564  Slovakia...Fixed
+00003330: 0a7e 7e7e 7e7e 0a2a 2044 6973 616c 6c6f  .~~~~~.* Disallo
+00003340: 7720 6060 7363 6877 6966 7479 6060 2074  w ``schwifty`` t
+00003350: 6f20 6265 2069 6e73 7461 6c6c 6564 2066  o be installed f
+00003360: 6f72 2050 7974 686f 6e20 7665 7273 696f  or Python versio
+00003370: 6e73 206f 6c64 6572 2074 6861 6e20 332e  ns older than 3.
+00003380: 372e 2049 7420 7761 7320 756e 7375 7070  7. It was unsupp
+00003390: 6f72 7465 640a 2020 6265 666f 7265 2062  orted.  before b
+000033a0: 7574 2069 7320 6e6f 7720 7265 6a65 6374  ut is now reject
+000033b0: 6564 2075 706f 6e20 696e 7374 616c 6c61  ed upon installa
+000033c0: 7469 6f6e 2077 6974 6820 616e 2061 7070  tion with an app
+000033d0: 726f 7072 6961 7465 2065 7272 6f72 206d  ropriate error m
+000033e0: 6573 7361 6765 2e0a 2a20 4175 7374 7269  essage..* Austri
+000033f0: 616e 2062 616e 6b20 636f 6465 7320 6172  an bank codes ar
+00003400: 6520 6e6f 7720 636f 6e73 6973 7465 6e74  e now consistent
+00003410: 6c79 206c 6566 7420 7061 6464 6564 2077  ly left padded w
+00003420: 6974 6820 7a65 726f 732e 2054 6869 7320  ith zeros. This 
+00003430: 6669 7865 7320 7468 6520 6d61 7070 696e  fixes the mappin
+00003440: 6720 6672 6f6d 0a20 2049 4241 4e20 746f  g from.  IBAN to
+00003450: 2042 4943 2066 6f72 2074 6865 2041 7573   BIC for the Aus
+00003460: 7472 6961 6e20 6665 6465 7261 6c20 6261  trian federal ba
+00003470: 6e6b 2069 6e73 7469 7475 7465 732e 0a0a  nk institutes...
+00003480: 6032 3032 312e 3036 2e31 605f 202d 2032  `2021.06.1`_ - 2
+00003490: 3032 312f 3036 2f32 340a 2d2d 2d2d 2d2d  021/06/24.------
+000034a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000034b0: 2d2d 2d0a 0a41 6464 6564 0a7e 7e7e 7e7e  ---..Added.~~~~~
+000034c0: 0a2a 2045 6e61 626c 6520 746f 6f6c 2062  .* Enable tool b
+000034d0: 6173 6564 2074 7970 6520 6368 6563 6b69  ased type checki
+000034e0: 6e67 2061 7320 6465 7363 7269 6265 6420  ng as described 
+000034f0: 696e 2060 5045 502d 3035 3631 605f 2062  in `PEP-0561`_ b
+00003500: 7920 6164 6469 6e67 2074 6865 2060 6070  y adding the ``p
+00003510: 792e 7479 7065 6460 6020 6d61 726b 6572  y.typed`` marker
+00003520: 0a20 2060 406a 6d66 6564 6572 6963 6f20  .  `@jmfederico 
+00003530: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
+00003540: 636f 6d2f 6a6d 6665 6465 7269 636f 3e60  com/jmfederico>`
+00003550: 5f0a 0a0a 6032 3032 312e 3036 2e30 605f  _...`2021.06.0`_
+00003560: 202d 2032 3032 312f 3036 2f31 370a 2d2d   - 2021/06/17.--
+00003570: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003580: 2d2d 2d2d 2d2d 2d0a 0a41 6464 6564 0a7e  -------..Added.~
+00003590: 7e7e 7e7e 0a2a 2041 6464 6564 2062 616e  ~~~~.* Added ban
+000035a0: 6b20 7265 6769 7374 7279 2066 6f72 2053  k registry for S
+000035b0: 7765 6469 7368 2042 616e 6b73 2060 406a  wedish Banks `@j
+000035c0: 6d66 6564 6572 6963 6f20 3c68 7474 7073  mfederico <https
+000035d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a6d  ://github.com/jm
+000035e0: 6665 6465 7269 636f 3e60 5f0a 0a0a 6032  federico>`_...`2
+000035f0: 3032 312e 3035 2e32 605f 202d 2032 3032  021.05.2`_ - 202
+00003600: 312f 3035 2f32 330a 2d2d 2d2d 2d2d 2d2d  1/05/23.--------
+00003610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003620: 2d0a 0a41 6464 6564 0a7e 7e7e 7e7e 0a2a  -..Added.~~~~~.*
+00003630: 2043 6f75 6e74 7279 2073 7065 6369 6663   Country specifc
+00003640: 2063 6865 636b 7375 6d20 7661 6c69 6461   checksum valida
+00003650: 7469 6f6e 2066 6f72 2042 656c 6769 616e  tion for Belgian
+00003660: 2062 616e 6b73 2c20 6173 2077 656c 6c20   banks, as well 
+00003670: 6173 2073 7570 706f 7274 2066 6f72 2067  as support for g
+00003680: 656e 6572 6174 696e 6720 7468 650a 2020  enerating the.  
+00003690: 6368 6563 6b73 756d 2077 6865 6e20 7573  checksum when us
+000036a0: 696e 6720 7468 6520 3a6d 6574 683a 602e  ing the :meth:`.
+000036b0: 4942 414e 2e67 656e 6572 6174 6560 2d6d  IBAN.generate`-m
+000036c0: 6574 686f 642e 2060 406d 6865 6d65 7279  ethod. `@mhemery
+000036d0: 636b 203c 6874 7470 733a 2f2f 6769 7468  ck <https://gith
+000036e0: 7562 2e63 6f6d 2f6d 6865 6d65 7279 636b  ub.com/mhemeryck
+000036f0: 3e60 5f0a 0a60 3230 3231 2e30 352e 3160  >`_..`2021.05.1`
+00003700: 5f20 2d20 3230 3231 2f30 352f 3230 0a2d  _ - 2021/05/20.-
+00003710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003720: 2d2d 2d2d 2d2d 2d2d 0a0a 4164 6465 640a  --------..Added.
+00003730: 7e7e 7e7e 7e0a 2a20 5468 6520 4942 414e  ~~~~~.* The IBAN
+00003740: 2076 616c 6964 6174 696f 6e20 6e6f 7720   validation now 
+00003750: 6f70 7469 6f6e 616c 6c79 2069 6e63 6c75  optionally inclu
+00003760: 6465 7320 7468 6520 7665 7269 6669 6361  des the verifica
+00003770: 7469 6f6e 206f 6620 7468 6520 636f 756e  tion of the coun
+00003780: 7472 7920 7370 6563 6966 6963 2063 6865  try specific che
+00003790: 636b 7375 6d0a 2020 7769 7468 696e 2074  cksum.  within t
+000037a0: 6865 2042 4241 4e2e 2054 6869 7320 6375  he BBAN. This cu
+000037b0: 7272 656e 746c 7920 776f 726b 7320 666f  rrently works fo
+000037c0: 7220 4765 726d 616e 2061 6e64 2049 7461  r German and Ita
+000037d0: 6c69 616e 2062 616e 6b73 2e20 466f 7220  lian banks. For 
+000037e0: 4765 726d 616e 2062 616e 6b73 2074 6865  German banks the
+000037f0: 2063 6865 636b 7375 6d0a 2020 616c 676f   checksum.  algo
+00003800: 7269 7468 6d20 666f 7220 7468 6520 6163  rithm for the ac
+00003810: 636f 756e 7420 636f 6465 2069 7320 6368  count code is ch
+00003820: 6f73 656e 2062 7920 7468 6520 6261 6e6b  osen by the bank
+00003830: 2063 6f64 652e 2053 696e 6365 2074 6865   code. Since the
+00003840: 7265 2061 7265 206f 7665 7220 3135 3020  re are over 150 
+00003850: 6261 6e6b 2073 7065 6369 6669 630a 2020  bank specific.  
+00003860: 616c 676f 7269 7468 6d73 2069 6e20 4765  algorithms in Ge
+00003870: 726d 616e 7920 6e6f 7420 616c 6c20 6f66  rmany not all of
+00003880: 2074 6865 6d20 6172 6520 696d 706c 656d   them are implem
+00003890: 656e 7465 6420 6174 2074 6865 206d 6f6d  ented at the mom
+000038a0: 656e 742c 2062 7574 2074 6865 206d 616a  ent, but the maj
+000038b0: 6f72 6974 7920 6f66 2062 616e 6b73 0a20  ority of banks. 
+000038c0: 2073 686f 756c 6420 6265 2063 6f76 6572   should be cover
+000038d0: 6564 2e0a 0a43 6861 6e67 6564 0a7e 7e7e  ed...Changed.~~~
+000038e0: 7e7e 7e7e 0a2a 2055 7064 6174 6520 6261  ~~~~.* Update ba
 000038f0: 6e6b 2072 6567 6973 7472 7920 666f 7220  nk registry for 
-00003900: 4175 7374 7269 612c 2050 6f6c 616e 642c  Austria, Poland,
-00003910: 2047 6572 6d61 6e79 2c20 4265 6c67 6975   Germany, Belgiu
-00003920: 6d2c 2043 7a65 6368 2052 6570 7562 6c69  m, Czech Republi
-00003930: 632c 204e 6574 6865 726c 616e 6473 2c20  c, Netherlands, 
-00003940: 536c 6f76 656e 6961 0a20 2061 6e64 2053  Slovenia.  and S
-00003950: 6c6f 7661 6b69 612e 0a0a 6032 3032 312e  lovakia...`2021.
-00003960: 3031 2e30 605f 202d 2032 3032 312f 3031  01.0`_ - 2021/01
-00003970: 2f32 300a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /20.------------
-00003980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a43  -------------..C
-00003990: 6861 6e67 6564 0a7e 7e7e 7e7e 7e7e 0a2a  hanged.~~~~~~~.*
-000039a0: 2052 6573 7472 7563 7475 7265 2064 6f63   Restructure doc
-000039b0: 756d 656e 7461 7469 6f6e 2061 6e64 2063  umentation and c
-000039c0: 6861 6e67 6520 7468 656d 6520 746f 2060  hange theme to `
-000039d0: 6675 726f 203c 6874 7470 733a 2f2f 7072  furo <https://pr
-000039e0: 6164 7975 6e73 672e 6d65 2f66 7572 6f2f  adyunsg.me/furo/
-000039f0: 3e60 5f2e 0a2a 2041 6464 6564 2064 6564  >`_..* Added ded
-00003a00: 6963 6174 6564 2065 7863 6570 7469 6f6e  icated exception
-00003a10: 2063 6c61 7373 6573 2066 6f72 2076 6172   classes for var
-00003a20: 696f 7573 2076 616c 6964 6174 696f 6e20  ious validation 
-00003a30: 6572 726f 7273 2e0a 2a20 4472 6f70 2073  errors..* Drop s
-00003a40: 7570 706f 7274 2066 6f72 2050 7974 686f  upport for Pytho
-00003a50: 6e20 322e 204f 6e6c 7920 5079 7468 6f6e  n 2. Only Python
-00003a60: 2033 2e36 2b20 7769 6c6c 2062 6520 7375   3.6+ will be su
-00003a70: 7070 6f72 7465 6420 6672 6f6d 206e 6f77  pported from now
-00003a80: 206f 6e2e 0a2a 2055 7365 2050 4550 2035   on..* Use PEP 5
-00003a90: 3137 2f35 3138 2063 6f6d 706c 6961 6e74  17/518 compliant
-00003aa0: 2062 7569 6c64 2073 6574 7570 2e0a 0a60   build setup...`
-00003ab0: 3230 3230 2e31 312e 3060 5f20 2d20 3230  2020.11.0`_ - 20
-00003ac0: 3230 2f31 322f 3032 0a2d 2d2d 2d2d 2d2d  20/12/02.-------
-00003ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003ae0: 2d2d 0a0a 4368 616e 6765 640a 7e7e 7e7e  --..Changed.~~~~
-00003af0: 7e7e 7e0a 2a20 5570 6461 7465 6420 4942  ~~~.* Updated IB
-00003b00: 414e 2072 6567 6973 7472 7920 616e 6420  AN registry and 
-00003b10: 6261 6e6b 2072 6567 6973 7472 6965 7320  bank registries 
-00003b20: 6f66 2050 6f6c 616e 642c 2047 6572 6d61  of Poland, Germa
-00003b30: 6e79 2c20 4175 7374 7269 612c 2042 656c  ny, Austria, Bel
-00003b40: 6769 756d 2c20 4e65 7468 6572 6c61 6e64  gium, Netherland
-00003b50: 732c 0a20 2043 7a65 6368 2052 6570 7562  s,.  Czech Repub
-00003b60: 6c69 6320 616e 6420 536c 6f76 656e 6961  lic and Slovenia
-00003b70: 2e0a 0a41 6464 6564 0a7e 7e7e 7e7e 0a2a  ...Added.~~~~~.*
-00003b80: 2041 6464 6564 2067 656e 6572 6174 6564   Added generated
-00003b90: 2062 616e 6b73 2066 6f72 2053 6c6f 7661   banks for Slova
-00003ba0: 6b69 6120 6040 7065 7472 626f 726f 7320  kia `@petrboros 
-00003bb0: 3c68 7474 7073 3a2f 2f67 6974 6875 622e  <https://github.
-00003bc0: 636f 6d2f 7065 7472 626f 726f 733e 605f  com/petrboros>`_
-00003bd0: 2e0a 2a20 4164 6465 6420 6120 7465 7374  ..* Added a test
-00003be0: 2074 6f20 7661 6c69 6461 7465 2074 6865   to validate the
-00003bf0: 2063 6f72 7265 6374 6e65 7320 6f66 2042   correctnes of B
-00003c00: 4943 7320 696e 2074 6865 2072 6567 6973  ICs in the regis
-00003c10: 7472 7920 6040 636b 6f65 686e 203c 6874  try `@ckoehn <ht
-00003c20: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00003c30: 2f63 6b6f 6568 6e3e 605f 2e0a 0a46 6978  /ckoehn>`_...Fix
-00003c40: 6564 0a7e 7e7e 7e7e 0a2a 2046 6978 6564  ed.~~~~~.* Fixed
-00003c50: 2065 6e63 6f64 696e 6720 666f 7220 506f   encoding for Po
-00003c60: 6c69 7368 2062 616e 6b20 7265 6769 7374  lish bank regist
-00003c70: 7279 2060 406d 6963 6861 6c2d 6d69 6368  ry `@michal-mich
-00003c80: 616c 616b 203c 6874 7470 733a 2f2f 6769  alak <https://gi
-00003c90: 7468 7562 2e63 6f6d 2f6d 6963 6861 6c2d  thub.com/michal-
-00003ca0: 6d69 6368 616c 616b 3e60 5f2e 0a0a 6032  michalak>`_...`2
-00003cb0: 3032 302e 3039 2e30 605f 202d 2032 3032  020.09.0`_ - 202
-00003cc0: 302f 3039 2f30 370a 2d2d 2d2d 2d2d 2d2d  0/09/07.--------
-00003cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003ce0: 2d0a 0a43 6861 6e67 6564 0a7e 7e7e 7e7e  -..Changed.~~~~~
-00003cf0: 7e7e 0a2a 204d 6967 7261 7465 6420 6275  ~~.* Migrated bu
-00003d00: 696c 6420 616e 6420 7465 7374 2070 6970  ild and test pip
-00003d10: 656c 696e 6573 2074 6f20 4769 7448 7562  elines to GitHub
-00003d20: 2061 6374 696f 6e73 2e0a 0a41 6464 6564   actions...Added
-00003d30: 0a7e 7e7e 7e7e 0a2a 2041 6464 6564 2067  .~~~~~.* Added g
-00003d40: 656e 6572 6174 6564 2062 616e 6b73 2066  enerated banks f
-00003d50: 6f72 204e 6574 6865 726c 616e 6473 2060  or Netherlands `
-00003d60: 4069 6e73 656e 7369 7469 7665 636c 6f64  @insensitiveclod
-00003d70: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-00003d80: 2e63 6f6d 2f69 6e73 656e 7369 7469 7665  .com/insensitive
-00003d90: 636c 6f64 3e60 5f2e 0a2a 2041 6464 6564  clod>`_..* Added
-00003da0: 2067 656e 6572 6174 6564 2062 616e 6b73   generated banks
-00003db0: 2066 6f72 2053 7061 696e 2e0a 0a60 3230   for Spain...`20
-00003dc0: 3230 2e30 382e 3360 5f20 2d20 3230 3230  20.08.3`_ - 2020
-00003dd0: 2f30 382f 3331 0a2d 2d2d 2d2d 2d2d 2d2d  /08/31.---------
-00003de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00003df0: 0a0a 4669 7865 640a 7e7e 7e7e 7e0a 2a20  ..Fixed.~~~~~.* 
-00003e00: 4669 7865 6420 4942 414e 2067 656e 6572  Fixed IBAN gener
-00003e10: 6174 696f 6e20 666f 7220 636f 756e 7472  ation for countr
-00003e20: 6965 7320 7769 7468 2062 7261 6e63 682f  ies with branch/
-00003e30: 736f 7274 2063 6f64 650a 2a20 4164 6420  sort code.* Add 
-00003e40: 6765 6e65 7261 7465 6420 6261 6e6b 7320  generated banks 
-00003e50: 666f 7220 5370 6169 6e0a 0a60 3230 3230  for Spain..`2020
-00003e60: 2e30 382e 3260 5f20 2d20 3230 3230 2f30  .08.2`_ - 2020/0
-00003e70: 382f 3330 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  8/30.-----------
-00003e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
-00003e90: 4669 7865 640a 7e7e 7e7e 7e0a 2a20 506f  Fixed.~~~~~.* Po
-00003ea0: 6c61 6e64 2773 2049 4241 4e20 7370 6563  land's IBAN spec
-00003eb0: 206f 6e6c 7920 6861 7320 6120 6272 616e   only has a bran
-00003ec0: 6368 2d63 6f64 6520 6275 7420 6e6f 2062  ch-code but no b
-00003ed0: 616e 6b2d 636f 6465 0a2a 2046 6978 6564  ank-code.* Fixed
-00003ee0: 206c 6973 7469 6e67 206f 6620 7375 7070   listing of supp
-00003ef0: 6f72 7465 6420 636f 756e 7472 6965 7320  orted countries 
-00003f00: 666f 7220 4249 4320 6465 7269 7661 7469  for BIC derivati
-00003f10: 6f6e 2e0a 2a20 4669 7865 6420 6261 6e6b  on..* Fixed bank
-00003f20: 2072 6567 6973 7472 7920 666f 7220 4875   registry for Hu
-00003f30: 6e67 6172 792e 0a0a 4368 616e 6765 640a  ngary...Changed.
-00003f40: 7e7e 7e7e 7e7e 7e0a 2a20 5570 6461 7465  ~~~~~~~.* Update
-00003f50: 6420 6261 6e6b 2072 6567 6973 7472 7920  d bank registry 
-00003f60: 506f 6c61 6e64 2c20 4265 6c67 6975 6d20  Poland, Belgium 
-00003f70: 616e 6420 4175 7374 7269 612e 0a2a 2055  and Austria..* U
-00003f80: 7064 6174 6564 2049 4241 4e20 7370 6563  pdated IBAN spec
-00003f90: 2066 6f72 2053 616f 2054 6f6d 6520 616e   for Sao Tome an
-00003fa0: 6420 5072 696e 6369 7065 0a0a 6032 3032  d Principe..`202
-00003fb0: 302e 3038 2e31 605f 202d 2032 3032 302f  0.08.1`_ - 2020/
-00003fc0: 3038 2f32 380a 2d2d 2d2d 2d2d 2d2d 2d2d  08/28.----------
-00003fd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00003fe0: 0a41 6464 6564 0a7e 7e7e 7e7e 0a2a 204e  .Added.~~~~~.* N
-00003ff0: 6577 2061 7474 7269 6275 7465 203a 6174  ew attribute :at
-00004000: 7472 3a60 2e42 4943 2e69 735f 7661 6c69  tr:`.BIC.is_vali
-00004010: 6460 2061 6e64 203a 6174 7472 3a60 2e49  d` and :attr:`.I
-00004020: 4241 4e2e 6973 5f76 616c 6964 602e 0a0a  BAN.is_valid`...
-00004030: 6032 3032 302e 3038 2e30 605f 202d 2032  `2020.08.0`_ - 2
-00004040: 3032 302f 3038 2f30 360a 2d2d 2d2d 2d2d  020/08/06.------
-00004050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004060: 2d2d 2d0a 0a43 6861 6e67 6564 0a7e 7e7e  ---..Changed.~~~
-00004070: 7e7e 7e7e 0a2a 2055 7064 6174 6564 2062  ~~~~.* Updated b
-00004080: 616e 6b20 7265 6769 7374 7279 2066 6f72  ank registry for
-00004090: 2050 6f6c 616e 642e 0a0a 6032 3032 302e   Poland...`2020.
-000040a0: 3035 2e33 605f 202d 2032 3032 302f 3035  05.3`_ - 2020/05
-000040b0: 2f32 350a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  /25.------------
-000040c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a41  -------------..A
-000040d0: 6464 6564 0a7e 7e7e 7e7e 0a2a 2041 6464  dded.~~~~~.* Add
-000040e0: 6564 2062 616e 6b73 2066 6f72 2046 7261  ed banks for Fra
-000040f0: 6e63 652c 2053 7769 747a 6572 6c61 6e64  nce, Switzerland
-00004100: 2061 6e64 2047 7265 6174 2042 7269 7461   and Great Brita
-00004110: 696e 2e0a 0a60 3230 3230 2e30 352e 3260  in...`2020.05.2`
-00004120: 5f20 2d20 3230 3230 2f30 352f 3038 0a2d  _ - 2020/05/08.-
-00004130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004140: 2d2d 2d2d 2d2d 2d2d 0a0a 4164 6465 640a  --------..Added.
-00004150: 7e7e 7e7e 7e0a 2a20 4164 6465 6420 3a61  ~~~~~.* Added :a
-00004160: 7474 723a 602e 4249 432e 636f 756e 7472  ttr:`.BIC.countr
-00004170: 7960 2061 6e64 203a 6174 7472 3a60 2e49  y` and :attr:`.I
-00004180: 4241 4e2e 636f 756e 7472 7960 2e0a 0a0a  BAN.country`....
-00004190: 2e2e 205f 3230 3234 2e30 352e 303a 2068  .. _2024.05.0: h
-000041a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000041b0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000041c0: 792f 636f 6d70 6172 652f 3230 3234 2e30  y/compare/2024.0
-000041d0: 342e 302e 2e2e 3230 3234 2e30 352e 300a  4.0...2024.05.0.
-000041e0: 2e2e 205f 3230 3234 2e30 342e 303a 2068  .. _2024.04.0: h
-000041f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004200: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004210: 792f 636f 6d70 6172 652f 3230 3233 2e30  y/compare/2023.0
-00004220: 312e 312e 2e2e 3230 3234 2e30 342e 300a  1.1...2024.04.0.
-00004230: 2e2e 205f 3230 3234 2e30 312e 313a 2068  .. _2024.01.1: h
-00004240: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004250: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004260: 792f 636f 6d70 6172 652f 3230 3233 2e31  y/compare/2023.1
-00004270: 312e 322e 2e2e 3230 3234 2e30 312e 310a  1.2...2024.01.1.
-00004280: 2e2e 205f 3230 3233 2e31 312e 323a 2068  .. _2023.11.2: h
-00004290: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000042a0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000042b0: 792f 636f 6d70 6172 652f 3230 3233 2e31  y/compare/2023.1
-000042c0: 312e 312e 2e2e 3230 3233 2e31 312e 320a  1.1...2023.11.2.
-000042d0: 2e2e 205f 3230 3233 2e31 312e 313a 2068  .. _2023.11.1: h
-000042e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000042f0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004300: 792f 636f 6d70 6172 652f 3230 3233 2e31  y/compare/2023.1
-00004310: 312e 302e 2e2e 3230 3233 2e31 312e 310a  1.0...2023.11.1.
-00004320: 2e2e 205f 3230 3233 2e31 312e 303a 2068  .. _2023.11.0: h
-00004330: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004340: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004350: 792f 636f 6d70 6172 652f 3230 3233 2e31  y/compare/2023.1
-00004360: 302e 302e 2e2e 3230 3233 2e31 312e 300a  0.0...2023.11.0.
-00004370: 2e2e 205f 3230 3233 2e31 302e 303a 2068  .. _2023.10.0: h
-00004380: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004390: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000043a0: 792f 636f 6d70 6172 652f 3230 3233 2e30  y/compare/2023.0
-000043b0: 392e 302e 2e2e 3230 3233 2e31 302e 300a  9.0...2023.10.0.
-000043c0: 2e2e 205f 3230 3233 2e30 392e 303a 2068  .. _2023.09.0: h
-000043d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000043e0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000043f0: 792f 636f 6d70 6172 652f 3230 3233 2e30  y/compare/2023.0
-00004400: 362e 302e 2e2e 3230 3233 2e30 392e 300a  6.0...2023.09.0.
-00004410: 2e2e 205f 3230 3233 2e30 362e 303a 2068  .. _2023.06.0: h
-00004420: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004430: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004440: 792f 636f 6d70 6172 652f 3230 3233 2e30  y/compare/2023.0
-00004450: 332e 302e 2e2e 3230 3233 2e30 362e 300a  3.0...2023.06.0.
-00004460: 2e2e 205f 3230 3233 2e30 332e 303a 2068  .. _2023.03.0: h
-00004470: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004480: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004490: 792f 636f 6d70 6172 652f 3230 3233 2e30  y/compare/2023.0
-000044a0: 322e 312e 2e2e 3230 3233 2e30 332e 300a  2.1...2023.03.0.
-000044b0: 2e2e 205f 3230 3233 2e30 322e 313a 2068  .. _2023.02.1: h
-000044c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000044d0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000044e0: 792f 636f 6d70 6172 652f 3230 3233 2e30  y/compare/2023.0
-000044f0: 322e 302e 2e2e 3230 3233 2e30 322e 310a  2.0...2023.02.1.
-00004500: 2e2e 205f 3230 3233 2e30 322e 303a 2068  .. _2023.02.0: h
-00004510: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004520: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004530: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-00004540: 392e 302e 2e2e 3230 3233 2e30 322e 300a  9.0...2023.02.0.
-00004550: 2e2e 205f 3230 3232 2e30 392e 303a 2068  .. _2022.09.0: h
-00004560: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004570: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004580: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-00004590: 372e 312e 2e2e 3230 3232 2e30 392e 300a  7.1...2022.09.0.
-000045a0: 2e2e 205f 3230 3232 2e30 372e 313a 2068  .. _2022.07.1: h
-000045b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000045c0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000045d0: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-000045e0: 372e 302e 2e2e 3230 3232 2e30 372e 310a  7.0...2022.07.1.
-000045f0: 2e2e 205f 3230 3232 2e30 372e 303a 2068  .. _2022.07.0: h
-00004600: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004610: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004620: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-00004630: 362e 332e 2e2e 3230 3232 2e30 372e 300a  6.3...2022.07.0.
-00004640: 2e2e 205f 3230 3232 2e30 362e 333a 2068  .. _2022.06.3: h
-00004650: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004660: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004670: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-00004680: 362e 322e 2e2e 3230 3232 2e30 362e 330a  6.2...2022.06.3.
-00004690: 2e2e 205f 3230 3232 2e30 362e 323a 2068  .. _2022.06.2: h
-000046a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000046b0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000046c0: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-000046d0: 362e 312e 2e2e 3230 3232 2e30 362e 320a  6.1...2022.06.2.
-000046e0: 2e2e 205f 3230 3232 2e30 362e 313a 2068  .. _2022.06.1: h
-000046f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004700: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004710: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-00004720: 362e 302e 2e2e 3230 3232 2e30 362e 310a  6.0...2022.06.1.
-00004730: 2e2e 205f 3230 3232 2e30 362e 303a 2068  .. _2022.06.0: h
-00004740: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004750: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004760: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-00004770: 342e 322e 2e2e 3230 3232 2e30 362e 300a  4.2...2022.06.0.
-00004780: 2e2e 205f 3230 3232 2e30 342e 323a 2068  .. _2022.04.2: h
-00004790: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000047a0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000047b0: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-000047c0: 342e 312e 2e2e 3230 3232 2e30 342e 320a  4.1...2022.04.2.
-000047d0: 2e2e 205f 3230 3232 2e30 342e 313a 2068  .. _2022.04.1: h
-000047e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000047f0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004800: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-00004810: 342e 302e 2e2e 3230 3232 2e30 342e 310a  4.0...2022.04.1.
-00004820: 2e2e 205f 3230 3232 2e30 342e 303a 2068  .. _2022.04.0: h
-00004830: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004840: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004850: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-00004860: 332e 312e 2e2e 3230 3232 2e30 342e 300a  3.1...2022.04.0.
-00004870: 2e2e 205f 3230 3232 2e30 332e 313a 2068  .. _2022.03.1: h
-00004880: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004890: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000048a0: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-000048b0: 332e 302e 2e2e 3230 3232 2e30 332e 310a  3.0...2022.03.1.
-000048c0: 2e2e 205f 3230 3232 2e30 332e 303a 2068  .. _2022.03.0: h
-000048d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000048e0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000048f0: 792f 636f 6d70 6172 652f 3230 3232 2e30  y/compare/2022.0
-00004900: 322e 302e 2e2e 3230 3232 2e30 332e 300a  2.0...2022.03.0.
-00004910: 2e2e 205f 3230 3232 2e30 322e 303a 2068  .. _2022.02.0: h
-00004920: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004930: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004940: 792f 636f 6d70 6172 652f 3230 3231 2e31  y/compare/2021.1
-00004950: 302e 322e 2e2e 3230 3232 2e30 322e 300a  0.2...2022.02.0.
-00004960: 2e2e 205f 3230 3231 2e31 302e 323a 2068  .. _2021.10.2: h
-00004970: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004980: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004990: 792f 636f 6d70 6172 652f 3230 3231 2e31  y/compare/2021.1
-000049a0: 302e 312e 2e2e 3230 3231 2e31 302e 320a  0.1...2021.10.2.
-000049b0: 2e2e 205f 3230 3231 2e31 302e 313a 2068  .. _2021.10.1: h
-000049c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000049d0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-000049e0: 792f 636f 6d70 6172 652f 3230 3231 2e31  y/compare/2021.1
-000049f0: 302e 302e 2e2e 3230 3231 2e31 302e 310a  0.0...2021.10.1.
-00004a00: 2e2e 205f 3230 3231 2e31 302e 303a 2068  .. _2021.10.0: h
-00004a10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004a20: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004a30: 792f 636f 6d70 6172 652f 3230 3231 2e30  y/compare/2021.0
-00004a40: 362e 312e 2e2e 3230 3231 2e31 302e 300a  6.1...2021.10.0.
-00004a50: 2e2e 205f 3230 3231 2e30 362e 313a 2068  .. _2021.06.1: h
-00004a60: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004a70: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004a80: 792f 636f 6d70 6172 652f 3230 3231 2e30  y/compare/2021.0
-00004a90: 362e 302e 2e2e 3230 3231 2e30 362e 310a  6.0...2021.06.1.
-00004aa0: 2e2e 205f 3230 3231 2e30 362e 303a 2068  .. _2021.06.0: h
-00004ab0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004ac0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004ad0: 792f 636f 6d70 6172 652f 3230 3231 2e30  y/compare/2021.0
-00004ae0: 352e 322e 2e2e 3230 3231 2e30 362e 300a  5.2...2021.06.0.
-00004af0: 2e2e 205f 3230 3231 2e30 352e 323a 2068  .. _2021.05.2: h
-00004b00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004b10: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004b20: 792f 636f 6d70 6172 652f 3230 3231 2e30  y/compare/2021.0
-00004b30: 352e 312e 2e2e 3230 3231 2e30 352e 320a  5.1...2021.05.2.
-00004b40: 2e2e 205f 3230 3231 2e30 352e 313a 2068  .. _2021.05.1: h
-00004b50: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004b60: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004b70: 792f 636f 6d70 6172 652f 3230 3231 2e30  y/compare/2021.0
-00004b80: 352e 302e 2e2e 3230 3231 2e30 352e 310a  5.0...2021.05.1.
-00004b90: 2e2e 205f 3230 3231 2e30 352e 303a 2068  .. _2021.05.0: h
-00004ba0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004bb0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004bc0: 792f 636f 6d70 6172 652f 3230 3231 2e30  y/compare/2021.0
-00004bd0: 342e 302e 2e2e 3230 3231 2e30 352e 300a  4.0...2021.05.0.
-00004be0: 2e2e 205f 3230 3231 2e30 342e 303a 2068  .. _2021.04.0: h
-00004bf0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004c00: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004c10: 792f 636f 6d70 6172 652f 3230 3231 2e30  y/compare/2021.0
-00004c20: 312e 302e 2e2e 3230 3231 2e30 342e 300a  1.0...2021.04.0.
-00004c30: 2e2e 205f 3230 3231 2e30 312e 303a 2068  .. _2021.01.0: h
-00004c40: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004c50: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004c60: 792f 636f 6d70 6172 652f 3230 3230 2e31  y/compare/2020.1
-00004c70: 312e 302e 2e2e 3230 3231 2e30 312e 300a  1.0...2021.01.0.
-00004c80: 2e2e 205f 3230 3230 2e31 312e 303a 2068  .. _2020.11.0: h
-00004c90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004ca0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004cb0: 792f 636f 6d70 6172 652f 3230 3230 2e30  y/compare/2020.0
-00004cc0: 392e 302e 2e2e 3230 3230 2e31 312e 300a  9.0...2020.11.0.
-00004cd0: 2e2e 205f 3230 3230 2e30 392e 303a 2068  .. _2020.09.0: h
-00004ce0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004cf0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004d00: 792f 636f 6d70 6172 652f 3230 3230 2e30  y/compare/2020.0
-00004d10: 382e 332e 2e2e 3230 3230 2e30 392e 300a  8.3...2020.09.0.
-00004d20: 2e2e 205f 3230 3230 2e30 382e 333a 2068  .. _2020.08.3: h
-00004d30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004d40: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004d50: 792f 636f 6d70 6172 652f 3230 3230 2e30  y/compare/2020.0
-00004d60: 382e 322e 2e2e 3230 3230 2e30 382e 330a  8.2...2020.08.3.
-00004d70: 2e2e 205f 3230 3230 2e30 382e 323a 2068  .. _2020.08.2: h
-00004d80: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004d90: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004da0: 792f 636f 6d70 6172 652f 3230 3230 2e30  y/compare/2020.0
-00004db0: 382e 312e 2e2e 3230 3230 2e30 382e 320a  8.1...2020.08.2.
-00004dc0: 2e2e 205f 3230 3230 2e30 382e 313a 2068  .. _2020.08.1: h
-00004dd0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004de0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004df0: 792f 636f 6d70 6172 652f 3230 3230 2e30  y/compare/2020.0
-00004e00: 382e 302e 2e2e 3230 3230 2e30 382e 310a  8.0...2020.08.1.
-00004e10: 2e2e 205f 3230 3230 2e30 382e 303a 2068  .. _2020.08.0: h
-00004e20: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004e30: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004e40: 792f 636f 6d70 6172 652f 3230 3230 2e30  y/compare/2020.0
-00004e50: 352e 332e 2e2e 3230 3230 2e30 382e 300a  5.3...2020.08.0.
-00004e60: 2e2e 205f 3230 3230 2e30 352e 333a 2068  .. _2020.05.3: h
-00004e70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004e80: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004e90: 792f 636f 6d70 6172 652f 3230 3230 2e30  y/compare/2020.0
-00004ea0: 352e 322e 2e2e 3230 3230 2e30 352e 330a  5.2...2020.05.3.
-00004eb0: 2e2e 205f 3230 3230 2e30 352e 323a 2068  .. _2020.05.2: h
-00004ec0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004ed0: 6d2f 6d64 6f6d 6b65 2f73 6368 7769 6674  m/mdomke/schwift
-00004ee0: 792f 636f 6d70 6172 652f 3230 3230 2e30  y/compare/2020.0
-00004ef0: 352e 312e 2e2e 3230 3230 2e30 352e 320a  5.1...2020.05.2.
-00004f00: 0a2e 2e20 5f50 4550 2d30 3536 313a 2068  ... _PEP-0561: h
-00004f10: 7474 7073 3a2f 2f77 7777 2e70 7974 686f  ttps://www.pytho
-00004f20: 6e2e 6f72 672f 6465 762f 7065 7073 2f70  n.org/dev/peps/p
-00004f30: 6570 2d30 3536 312f 2370 6163 6b61 6769  ep-0561/#packagi
-00004f40: 6e67 2d74 7970 652d 696e 666f 726d 6174  ng-type-informat
-00004f50: 696f 6e0a                                ion.
+00003900: 4765 726d 616e 792c 2050 6f6c 616e 642c  Germany, Poland,
+00003910: 2043 7a65 6368 2052 6570 7562 6c69 632c   Czech Republic,
+00003920: 2041 7573 7472 6961 2061 6e64 204e 6574   Austria and Net
+00003930: 6865 726c 616e 6473 2e0a 0a60 3230 3231  herlands...`2021
+00003940: 2e30 352e 3060 5f20 2d20 3230 3231 2f30  .05.0`_ - 2021/0
+00003950: 352f 3032 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  5/02.-----------
+00003960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+00003970: 4164 6465 640a 7e7e 7e7e 7e0a 2a20 4164  Added.~~~~~.* Ad
+00003980: 6465 6420 6d61 6e75 616c 6c79 2063 7572  ded manually cur
+00003990: 6174 6564 206c 6973 7420 6f66 204c 6974  ated list of Lit
+000039a0: 6875 616e 6961 6e20 4261 6e6b 7320 2865  huanian Banks (e
+000039b0: 2e67 2052 6576 6f6c 7574 2050 6179 6d65  .g Revolut Payme
+000039c0: 6e74 7320 5541 4229 2e0a 0a60 3230 3231  nts UAB)...`2021
+000039d0: 2e30 342e 3060 5f20 2d20 3230 3231 2f30  .04.0`_ - 2021/0
+000039e0: 342f 3233 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d  4/23.-----------
+000039f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a  --------------..
+00003a00: 4368 616e 6765 640a 7e7e 7e7e 7e7e 7e0a  Changed.~~~~~~~.
+00003a10: 2a20 4164 6465 6420 7479 7065 2068 696e  * Added type hin
+00003a20: 7473 2074 6f20 7468 6520 656e 7469 7265  ts to the entire
+00003a30: 2063 6f64 6520 6261 7365 2e0a 2a20 4472   code base..* Dr
+00003a40: 6f70 7065 6420 7375 7070 6f72 7420 666f  opped support fo
+00003a50: 7220 5079 7468 6f6e 2033 2e36 0a2a 2055  r Python 3.6.* U
+00003a60: 7064 6174 6520 6261 6e6b 2072 6567 6973  pdate bank regis
+00003a70: 7472 7920 666f 7220 4175 7374 7269 612c  try for Austria,
+00003a80: 2050 6f6c 616e 642c 2047 6572 6d61 6e79   Poland, Germany
+00003a90: 2c20 4265 6c67 6975 6d2c 2043 7a65 6368  , Belgium, Czech
+00003aa0: 2052 6570 7562 6c69 632c 204e 6574 6865   Republic, Nethe
+00003ab0: 726c 616e 6473 2c20 536c 6f76 656e 6961  rlands, Slovenia
+00003ac0: 0a20 2061 6e64 2053 6c6f 7661 6b69 612e  .  and Slovakia.
+00003ad0: 0a0a 6032 3032 312e 3031 2e30 605f 202d  ..`2021.01.0`_ -
+00003ae0: 2032 3032 312f 3031 2f32 300a 2d2d 2d2d   2021/01/20.----
+00003af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003b00: 2d2d 2d2d 2d0a 0a43 6861 6e67 6564 0a7e  -----..Changed.~
+00003b10: 7e7e 7e7e 7e7e 0a2a 2052 6573 7472 7563  ~~~~~~.* Restruc
+00003b20: 7475 7265 2064 6f63 756d 656e 7461 7469  ture documentati
+00003b30: 6f6e 2061 6e64 2063 6861 6e67 6520 7468  on and change th
+00003b40: 656d 6520 746f 2060 6675 726f 203c 6874  eme to `furo <ht
+00003b50: 7470 733a 2f2f 7072 6164 7975 6e73 672e  tps://pradyunsg.
+00003b60: 6d65 2f66 7572 6f2f 3e60 5f2e 0a2a 2041  me/furo/>`_..* A
+00003b70: 6464 6564 2064 6564 6963 6174 6564 2065  dded dedicated e
+00003b80: 7863 6570 7469 6f6e 2063 6c61 7373 6573  xception classes
+00003b90: 2066 6f72 2076 6172 696f 7573 2076 616c   for various val
+00003ba0: 6964 6174 696f 6e20 6572 726f 7273 2e0a  idation errors..
+00003bb0: 2a20 4472 6f70 2073 7570 706f 7274 2066  * Drop support f
+00003bc0: 6f72 2050 7974 686f 6e20 322e 204f 6e6c  or Python 2. Onl
+00003bd0: 7920 5079 7468 6f6e 2033 2e36 2b20 7769  y Python 3.6+ wi
+00003be0: 6c6c 2062 6520 7375 7070 6f72 7465 6420  ll be supported 
+00003bf0: 6672 6f6d 206e 6f77 206f 6e2e 0a2a 2055  from now on..* U
+00003c00: 7365 2050 4550 2035 3137 2f35 3138 2063  se PEP 517/518 c
+00003c10: 6f6d 706c 6961 6e74 2062 7569 6c64 2073  ompliant build s
+00003c20: 6574 7570 2e0a 0a60 3230 3230 2e31 312e  etup...`2020.11.
+00003c30: 3060 5f20 2d20 3230 3230 2f31 322f 3032  0`_ - 2020/12/02
+00003c40: 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .---------------
+00003c50: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4368 616e  ----------..Chan
+00003c60: 6765 640a 7e7e 7e7e 7e7e 7e0a 2a20 5570  ged.~~~~~~~.* Up
+00003c70: 6461 7465 6420 4942 414e 2072 6567 6973  dated IBAN regis
+00003c80: 7472 7920 616e 6420 6261 6e6b 2072 6567  try and bank reg
+00003c90: 6973 7472 6965 7320 6f66 2050 6f6c 616e  istries of Polan
+00003ca0: 642c 2047 6572 6d61 6e79 2c20 4175 7374  d, Germany, Aust
+00003cb0: 7269 612c 2042 656c 6769 756d 2c20 4e65  ria, Belgium, Ne
+00003cc0: 7468 6572 6c61 6e64 732c 0a20 2043 7a65  therlands,.  Cze
+00003cd0: 6368 2052 6570 7562 6c69 6320 616e 6420  ch Republic and 
+00003ce0: 536c 6f76 656e 6961 2e0a 0a41 6464 6564  Slovenia...Added
+00003cf0: 0a7e 7e7e 7e7e 0a2a 2041 6464 6564 2067  .~~~~~.* Added g
+00003d00: 656e 6572 6174 6564 2062 616e 6b73 2066  enerated banks f
+00003d10: 6f72 2053 6c6f 7661 6b69 6120 6040 7065  or Slovakia `@pe
+00003d20: 7472 626f 726f 7320 3c68 7474 7073 3a2f  trboros <https:/
+00003d30: 2f67 6974 6875 622e 636f 6d2f 7065 7472  /github.com/petr
+00003d40: 626f 726f 733e 605f 2e0a 2a20 4164 6465  boros>`_..* Adde
+00003d50: 6420 6120 7465 7374 2074 6f20 7661 6c69  d a test to vali
+00003d60: 6461 7465 2074 6865 2063 6f72 7265 6374  date the correct
+00003d70: 6e65 7320 6f66 2042 4943 7320 696e 2074  nes of BICs in t
+00003d80: 6865 2072 6567 6973 7472 7920 6040 636b  he registry `@ck
+00003d90: 6f65 686e 203c 6874 7470 733a 2f2f 6769  oehn <https://gi
+00003da0: 7468 7562 2e63 6f6d 2f63 6b6f 6568 6e3e  thub.com/ckoehn>
+00003db0: 605f 2e0a 0a46 6978 6564 0a7e 7e7e 7e7e  `_...Fixed.~~~~~
+00003dc0: 0a2a 2046 6978 6564 2065 6e63 6f64 696e  .* Fixed encodin
+00003dd0: 6720 666f 7220 506f 6c69 7368 2062 616e  g for Polish ban
+00003de0: 6b20 7265 6769 7374 7279 2060 406d 6963  k registry `@mic
+00003df0: 6861 6c2d 6d69 6368 616c 616b 203c 6874  hal-michalak <ht
+00003e00: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00003e10: 2f6d 6963 6861 6c2d 6d69 6368 616c 616b  /michal-michalak
+00003e20: 3e60 5f2e 0a0a 6032 3032 302e 3039 2e30  >`_...`2020.09.0
+00003e30: 605f 202d 2032 3032 302f 3039 2f30 370a  `_ - 2020/09/07.
+00003e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003e50: 2d2d 2d2d 2d2d 2d2d 2d0a 0a43 6861 6e67  ---------..Chang
+00003e60: 6564 0a7e 7e7e 7e7e 7e7e 0a2a 204d 6967  ed.~~~~~~~.* Mig
+00003e70: 7261 7465 6420 6275 696c 6420 616e 6420  rated build and 
+00003e80: 7465 7374 2070 6970 656c 696e 6573 2074  test pipelines t
+00003e90: 6f20 4769 7448 7562 2061 6374 696f 6e73  o GitHub actions
+00003ea0: 2e0a 0a41 6464 6564 0a7e 7e7e 7e7e 0a2a  ...Added.~~~~~.*
+00003eb0: 2041 6464 6564 2067 656e 6572 6174 6564   Added generated
+00003ec0: 2062 616e 6b73 2066 6f72 204e 6574 6865   banks for Nethe
+00003ed0: 726c 616e 6473 2060 4069 6e73 656e 7369  rlands `@insensi
+00003ee0: 7469 7665 636c 6f64 203c 6874 7470 733a  tiveclod <https:
+00003ef0: 2f2f 6769 7468 7562 2e63 6f6d 2f69 6e73  //github.com/ins
+00003f00: 656e 7369 7469 7665 636c 6f64 3e60 5f2e  ensitiveclod>`_.
+00003f10: 0a2a 2041 6464 6564 2067 656e 6572 6174  .* Added generat
+00003f20: 6564 2062 616e 6b73 2066 6f72 2053 7061  ed banks for Spa
+00003f30: 696e 2e0a 0a60 3230 3230 2e30 382e 3360  in...`2020.08.3`
+00003f40: 5f20 2d20 3230 3230 2f30 382f 3331 0a2d  _ - 2020/08/31.-
+00003f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003f60: 2d2d 2d2d 2d2d 2d2d 0a0a 4669 7865 640a  --------..Fixed.
+00003f70: 7e7e 7e7e 7e0a 2a20 4669 7865 6420 4942  ~~~~~.* Fixed IB
+00003f80: 414e 2067 656e 6572 6174 696f 6e20 666f  AN generation fo
+00003f90: 7220 636f 756e 7472 6965 7320 7769 7468  r countries with
+00003fa0: 2062 7261 6e63 682f 736f 7274 2063 6f64   branch/sort cod
+00003fb0: 650a 2a20 4164 6420 6765 6e65 7261 7465  e.* Add generate
+00003fc0: 6420 6261 6e6b 7320 666f 7220 5370 6169  d banks for Spai
+00003fd0: 6e0a 0a60 3230 3230 2e30 382e 3260 5f20  n..`2020.08.2`_ 
+00003fe0: 2d20 3230 3230 2f30 382f 3330 0a2d 2d2d  - 2020/08/30.---
+00003ff0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004000: 2d2d 2d2d 2d2d 0a0a 4669 7865 640a 7e7e  ------..Fixed.~~
+00004010: 7e7e 7e0a 2a20 506f 6c61 6e64 2773 2049  ~~~.* Poland's I
+00004020: 4241 4e20 7370 6563 206f 6e6c 7920 6861  BAN spec only ha
+00004030: 7320 6120 6272 616e 6368 2d63 6f64 6520  s a branch-code 
+00004040: 6275 7420 6e6f 2062 616e 6b2d 636f 6465  but no bank-code
+00004050: 0a2a 2046 6978 6564 206c 6973 7469 6e67  .* Fixed listing
+00004060: 206f 6620 7375 7070 6f72 7465 6420 636f   of supported co
+00004070: 756e 7472 6965 7320 666f 7220 4249 4320  untries for BIC 
+00004080: 6465 7269 7661 7469 6f6e 2e0a 2a20 4669  derivation..* Fi
+00004090: 7865 6420 6261 6e6b 2072 6567 6973 7472  xed bank registr
+000040a0: 7920 666f 7220 4875 6e67 6172 792e 0a0a  y for Hungary...
+000040b0: 4368 616e 6765 640a 7e7e 7e7e 7e7e 7e0a  Changed.~~~~~~~.
+000040c0: 2a20 5570 6461 7465 6420 6261 6e6b 2072  * Updated bank r
+000040d0: 6567 6973 7472 7920 506f 6c61 6e64 2c20  egistry Poland, 
+000040e0: 4265 6c67 6975 6d20 616e 6420 4175 7374  Belgium and Aust
+000040f0: 7269 612e 0a2a 2055 7064 6174 6564 2049  ria..* Updated I
+00004100: 4241 4e20 7370 6563 2066 6f72 2053 616f  BAN spec for Sao
+00004110: 2054 6f6d 6520 616e 6420 5072 696e 6369   Tome and Princi
+00004120: 7065 0a0a 6032 3032 302e 3038 2e31 605f  pe..`2020.08.1`_
+00004130: 202d 2032 3032 302f 3038 2f32 380a 2d2d   - 2020/08/28.--
+00004140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004150: 2d2d 2d2d 2d2d 2d0a 0a41 6464 6564 0a7e  -------..Added.~
+00004160: 7e7e 7e7e 0a2a 204e 6577 2061 7474 7269  ~~~~.* New attri
+00004170: 6275 7465 203a 6174 7472 3a60 2e42 4943  bute :attr:`.BIC
+00004180: 2e69 735f 7661 6c69 6460 2061 6e64 203a  .is_valid` and :
+00004190: 6174 7472 3a60 2e49 4241 4e2e 6973 5f76  attr:`.IBAN.is_v
+000041a0: 616c 6964 602e 0a0a 6032 3032 302e 3038  alid`...`2020.08
+000041b0: 2e30 605f 202d 2032 3032 302f 3038 2f30  .0`_ - 2020/08/0
+000041c0: 360a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  6.--------------
+000041d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a43 6861  -----------..Cha
+000041e0: 6e67 6564 0a7e 7e7e 7e7e 7e7e 0a2a 2055  nged.~~~~~~~.* U
+000041f0: 7064 6174 6564 2062 616e 6b20 7265 6769  pdated bank regi
+00004200: 7374 7279 2066 6f72 2050 6f6c 616e 642e  stry for Poland.
+00004210: 0a0a 6032 3032 302e 3035 2e33 605f 202d  ..`2020.05.3`_ -
+00004220: 2032 3032 302f 3035 2f32 350a 2d2d 2d2d   2020/05/25.----
+00004230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004240: 2d2d 2d2d 2d0a 0a41 6464 6564 0a7e 7e7e  -----..Added.~~~
+00004250: 7e7e 0a2a 2041 6464 6564 2062 616e 6b73  ~~.* Added banks
+00004260: 2066 6f72 2046 7261 6e63 652c 2053 7769   for France, Swi
+00004270: 747a 6572 6c61 6e64 2061 6e64 2047 7265  tzerland and Gre
+00004280: 6174 2042 7269 7461 696e 2e0a 0a60 3230  at Britain...`20
+00004290: 3230 2e30 352e 3260 5f20 2d20 3230 3230  20.05.2`_ - 2020
+000042a0: 2f30 352f 3038 0a2d 2d2d 2d2d 2d2d 2d2d  /05/08.---------
+000042b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000042c0: 0a0a 4164 6465 640a 7e7e 7e7e 7e0a 2a20  ..Added.~~~~~.* 
+000042d0: 4164 6465 6420 3a61 7474 723a 602e 4249  Added :attr:`.BI
+000042e0: 432e 636f 756e 7472 7960 2061 6e64 203a  C.country` and :
+000042f0: 6174 7472 3a60 2e49 4241 4e2e 636f 756e  attr:`.IBAN.coun
+00004300: 7472 7960 2e0a 0a0a 2e2e 205f 3230 3234  try`...... _2024
+00004310: 2e30 352e 313a 2068 7474 7073 3a2f 2f67  .05.1: https://g
+00004320: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004330: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004340: 652f 3230 3234 2e30 352e 302e 2e2e 3230  e/2024.05.0...20
+00004350: 3234 2e30 352e 310a 2e2e 205f 3230 3234  24.05.1... _2024
+00004360: 2e30 352e 303a 2068 7474 7073 3a2f 2f67  .05.0: https://g
+00004370: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004380: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004390: 652f 3230 3234 2e30 342e 302e 2e2e 3230  e/2024.04.0...20
+000043a0: 3234 2e30 352e 300a 2e2e 205f 3230 3234  24.05.0... _2024
+000043b0: 2e30 342e 303a 2068 7474 7073 3a2f 2f67  .04.0: https://g
+000043c0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+000043d0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+000043e0: 652f 3230 3233 2e30 312e 312e 2e2e 3230  e/2023.01.1...20
+000043f0: 3234 2e30 342e 300a 2e2e 205f 3230 3234  24.04.0... _2024
+00004400: 2e30 312e 313a 2068 7474 7073 3a2f 2f67  .01.1: https://g
+00004410: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004420: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004430: 652f 3230 3233 2e31 312e 322e 2e2e 3230  e/2023.11.2...20
+00004440: 3234 2e30 312e 310a 2e2e 205f 3230 3233  24.01.1... _2023
+00004450: 2e31 312e 323a 2068 7474 7073 3a2f 2f67  .11.2: https://g
+00004460: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004470: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004480: 652f 3230 3233 2e31 312e 312e 2e2e 3230  e/2023.11.1...20
+00004490: 3233 2e31 312e 320a 2e2e 205f 3230 3233  23.11.2... _2023
+000044a0: 2e31 312e 313a 2068 7474 7073 3a2f 2f67  .11.1: https://g
+000044b0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+000044c0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+000044d0: 652f 3230 3233 2e31 312e 302e 2e2e 3230  e/2023.11.0...20
+000044e0: 3233 2e31 312e 310a 2e2e 205f 3230 3233  23.11.1... _2023
+000044f0: 2e31 312e 303a 2068 7474 7073 3a2f 2f67  .11.0: https://g
+00004500: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004510: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004520: 652f 3230 3233 2e31 302e 302e 2e2e 3230  e/2023.10.0...20
+00004530: 3233 2e31 312e 300a 2e2e 205f 3230 3233  23.11.0... _2023
+00004540: 2e31 302e 303a 2068 7474 7073 3a2f 2f67  .10.0: https://g
+00004550: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004560: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004570: 652f 3230 3233 2e30 392e 302e 2e2e 3230  e/2023.09.0...20
+00004580: 3233 2e31 302e 300a 2e2e 205f 3230 3233  23.10.0... _2023
+00004590: 2e30 392e 303a 2068 7474 7073 3a2f 2f67  .09.0: https://g
+000045a0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+000045b0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+000045c0: 652f 3230 3233 2e30 362e 302e 2e2e 3230  e/2023.06.0...20
+000045d0: 3233 2e30 392e 300a 2e2e 205f 3230 3233  23.09.0... _2023
+000045e0: 2e30 362e 303a 2068 7474 7073 3a2f 2f67  .06.0: https://g
+000045f0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004600: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004610: 652f 3230 3233 2e30 332e 302e 2e2e 3230  e/2023.03.0...20
+00004620: 3233 2e30 362e 300a 2e2e 205f 3230 3233  23.06.0... _2023
+00004630: 2e30 332e 303a 2068 7474 7073 3a2f 2f67  .03.0: https://g
+00004640: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004650: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004660: 652f 3230 3233 2e30 322e 312e 2e2e 3230  e/2023.02.1...20
+00004670: 3233 2e30 332e 300a 2e2e 205f 3230 3233  23.03.0... _2023
+00004680: 2e30 322e 313a 2068 7474 7073 3a2f 2f67  .02.1: https://g
+00004690: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+000046a0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+000046b0: 652f 3230 3233 2e30 322e 302e 2e2e 3230  e/2023.02.0...20
+000046c0: 3233 2e30 322e 310a 2e2e 205f 3230 3233  23.02.1... _2023
+000046d0: 2e30 322e 303a 2068 7474 7073 3a2f 2f67  .02.0: https://g
+000046e0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+000046f0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004700: 652f 3230 3232 2e30 392e 302e 2e2e 3230  e/2022.09.0...20
+00004710: 3233 2e30 322e 300a 2e2e 205f 3230 3232  23.02.0... _2022
+00004720: 2e30 392e 303a 2068 7474 7073 3a2f 2f67  .09.0: https://g
+00004730: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004740: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004750: 652f 3230 3232 2e30 372e 312e 2e2e 3230  e/2022.07.1...20
+00004760: 3232 2e30 392e 300a 2e2e 205f 3230 3232  22.09.0... _2022
+00004770: 2e30 372e 313a 2068 7474 7073 3a2f 2f67  .07.1: https://g
+00004780: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004790: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+000047a0: 652f 3230 3232 2e30 372e 302e 2e2e 3230  e/2022.07.0...20
+000047b0: 3232 2e30 372e 310a 2e2e 205f 3230 3232  22.07.1... _2022
+000047c0: 2e30 372e 303a 2068 7474 7073 3a2f 2f67  .07.0: https://g
+000047d0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+000047e0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+000047f0: 652f 3230 3232 2e30 362e 332e 2e2e 3230  e/2022.06.3...20
+00004800: 3232 2e30 372e 300a 2e2e 205f 3230 3232  22.07.0... _2022
+00004810: 2e30 362e 333a 2068 7474 7073 3a2f 2f67  .06.3: https://g
+00004820: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004830: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004840: 652f 3230 3232 2e30 362e 322e 2e2e 3230  e/2022.06.2...20
+00004850: 3232 2e30 362e 330a 2e2e 205f 3230 3232  22.06.3... _2022
+00004860: 2e30 362e 323a 2068 7474 7073 3a2f 2f67  .06.2: https://g
+00004870: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004880: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004890: 652f 3230 3232 2e30 362e 312e 2e2e 3230  e/2022.06.1...20
+000048a0: 3232 2e30 362e 320a 2e2e 205f 3230 3232  22.06.2... _2022
+000048b0: 2e30 362e 313a 2068 7474 7073 3a2f 2f67  .06.1: https://g
+000048c0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+000048d0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+000048e0: 652f 3230 3232 2e30 362e 302e 2e2e 3230  e/2022.06.0...20
+000048f0: 3232 2e30 362e 310a 2e2e 205f 3230 3232  22.06.1... _2022
+00004900: 2e30 362e 303a 2068 7474 7073 3a2f 2f67  .06.0: https://g
+00004910: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004920: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004930: 652f 3230 3232 2e30 342e 322e 2e2e 3230  e/2022.04.2...20
+00004940: 3232 2e30 362e 300a 2e2e 205f 3230 3232  22.06.0... _2022
+00004950: 2e30 342e 323a 2068 7474 7073 3a2f 2f67  .04.2: https://g
+00004960: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004970: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004980: 652f 3230 3232 2e30 342e 312e 2e2e 3230  e/2022.04.1...20
+00004990: 3232 2e30 342e 320a 2e2e 205f 3230 3232  22.04.2... _2022
+000049a0: 2e30 342e 313a 2068 7474 7073 3a2f 2f67  .04.1: https://g
+000049b0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+000049c0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+000049d0: 652f 3230 3232 2e30 342e 302e 2e2e 3230  e/2022.04.0...20
+000049e0: 3232 2e30 342e 310a 2e2e 205f 3230 3232  22.04.1... _2022
+000049f0: 2e30 342e 303a 2068 7474 7073 3a2f 2f67  .04.0: https://g
+00004a00: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004a10: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004a20: 652f 3230 3232 2e30 332e 312e 2e2e 3230  e/2022.03.1...20
+00004a30: 3232 2e30 342e 300a 2e2e 205f 3230 3232  22.04.0... _2022
+00004a40: 2e30 332e 313a 2068 7474 7073 3a2f 2f67  .03.1: https://g
+00004a50: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004a60: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004a70: 652f 3230 3232 2e30 332e 302e 2e2e 3230  e/2022.03.0...20
+00004a80: 3232 2e30 332e 310a 2e2e 205f 3230 3232  22.03.1... _2022
+00004a90: 2e30 332e 303a 2068 7474 7073 3a2f 2f67  .03.0: https://g
+00004aa0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004ab0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004ac0: 652f 3230 3232 2e30 322e 302e 2e2e 3230  e/2022.02.0...20
+00004ad0: 3232 2e30 332e 300a 2e2e 205f 3230 3232  22.03.0... _2022
+00004ae0: 2e30 322e 303a 2068 7474 7073 3a2f 2f67  .02.0: https://g
+00004af0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004b00: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004b10: 652f 3230 3231 2e31 302e 322e 2e2e 3230  e/2021.10.2...20
+00004b20: 3232 2e30 322e 300a 2e2e 205f 3230 3231  22.02.0... _2021
+00004b30: 2e31 302e 323a 2068 7474 7073 3a2f 2f67  .10.2: https://g
+00004b40: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004b50: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004b60: 652f 3230 3231 2e31 302e 312e 2e2e 3230  e/2021.10.1...20
+00004b70: 3231 2e31 302e 320a 2e2e 205f 3230 3231  21.10.2... _2021
+00004b80: 2e31 302e 313a 2068 7474 7073 3a2f 2f67  .10.1: https://g
+00004b90: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004ba0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004bb0: 652f 3230 3231 2e31 302e 302e 2e2e 3230  e/2021.10.0...20
+00004bc0: 3231 2e31 302e 310a 2e2e 205f 3230 3231  21.10.1... _2021
+00004bd0: 2e31 302e 303a 2068 7474 7073 3a2f 2f67  .10.0: https://g
+00004be0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004bf0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004c00: 652f 3230 3231 2e30 362e 312e 2e2e 3230  e/2021.06.1...20
+00004c10: 3231 2e31 302e 300a 2e2e 205f 3230 3231  21.10.0... _2021
+00004c20: 2e30 362e 313a 2068 7474 7073 3a2f 2f67  .06.1: https://g
+00004c30: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004c40: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004c50: 652f 3230 3231 2e30 362e 302e 2e2e 3230  e/2021.06.0...20
+00004c60: 3231 2e30 362e 310a 2e2e 205f 3230 3231  21.06.1... _2021
+00004c70: 2e30 362e 303a 2068 7474 7073 3a2f 2f67  .06.0: https://g
+00004c80: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004c90: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004ca0: 652f 3230 3231 2e30 352e 322e 2e2e 3230  e/2021.05.2...20
+00004cb0: 3231 2e30 362e 300a 2e2e 205f 3230 3231  21.06.0... _2021
+00004cc0: 2e30 352e 323a 2068 7474 7073 3a2f 2f67  .05.2: https://g
+00004cd0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004ce0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004cf0: 652f 3230 3231 2e30 352e 312e 2e2e 3230  e/2021.05.1...20
+00004d00: 3231 2e30 352e 320a 2e2e 205f 3230 3231  21.05.2... _2021
+00004d10: 2e30 352e 313a 2068 7474 7073 3a2f 2f67  .05.1: https://g
+00004d20: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004d30: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004d40: 652f 3230 3231 2e30 352e 302e 2e2e 3230  e/2021.05.0...20
+00004d50: 3231 2e30 352e 310a 2e2e 205f 3230 3231  21.05.1... _2021
+00004d60: 2e30 352e 303a 2068 7474 7073 3a2f 2f67  .05.0: https://g
+00004d70: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004d80: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004d90: 652f 3230 3231 2e30 342e 302e 2e2e 3230  e/2021.04.0...20
+00004da0: 3231 2e30 352e 300a 2e2e 205f 3230 3231  21.05.0... _2021
+00004db0: 2e30 342e 303a 2068 7474 7073 3a2f 2f67  .04.0: https://g
+00004dc0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004dd0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004de0: 652f 3230 3231 2e30 312e 302e 2e2e 3230  e/2021.01.0...20
+00004df0: 3231 2e30 342e 300a 2e2e 205f 3230 3231  21.04.0... _2021
+00004e00: 2e30 312e 303a 2068 7474 7073 3a2f 2f67  .01.0: https://g
+00004e10: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004e20: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004e30: 652f 3230 3230 2e31 312e 302e 2e2e 3230  e/2020.11.0...20
+00004e40: 3231 2e30 312e 300a 2e2e 205f 3230 3230  21.01.0... _2020
+00004e50: 2e31 312e 303a 2068 7474 7073 3a2f 2f67  .11.0: https://g
+00004e60: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004e70: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004e80: 652f 3230 3230 2e30 392e 302e 2e2e 3230  e/2020.09.0...20
+00004e90: 3230 2e31 312e 300a 2e2e 205f 3230 3230  20.11.0... _2020
+00004ea0: 2e30 392e 303a 2068 7474 7073 3a2f 2f67  .09.0: https://g
+00004eb0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004ec0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004ed0: 652f 3230 3230 2e30 382e 332e 2e2e 3230  e/2020.08.3...20
+00004ee0: 3230 2e30 392e 300a 2e2e 205f 3230 3230  20.09.0... _2020
+00004ef0: 2e30 382e 333a 2068 7474 7073 3a2f 2f67  .08.3: https://g
+00004f00: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004f10: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004f20: 652f 3230 3230 2e30 382e 322e 2e2e 3230  e/2020.08.2...20
+00004f30: 3230 2e30 382e 330a 2e2e 205f 3230 3230  20.08.3... _2020
+00004f40: 2e30 382e 323a 2068 7474 7073 3a2f 2f67  .08.2: https://g
+00004f50: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004f60: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004f70: 652f 3230 3230 2e30 382e 312e 2e2e 3230  e/2020.08.1...20
+00004f80: 3230 2e30 382e 320a 2e2e 205f 3230 3230  20.08.2... _2020
+00004f90: 2e30 382e 313a 2068 7474 7073 3a2f 2f67  .08.1: https://g
+00004fa0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00004fb0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00004fc0: 652f 3230 3230 2e30 382e 302e 2e2e 3230  e/2020.08.0...20
+00004fd0: 3230 2e30 382e 310a 2e2e 205f 3230 3230  20.08.1... _2020
+00004fe0: 2e30 382e 303a 2068 7474 7073 3a2f 2f67  .08.0: https://g
+00004ff0: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00005000: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00005010: 652f 3230 3230 2e30 352e 332e 2e2e 3230  e/2020.05.3...20
+00005020: 3230 2e30 382e 300a 2e2e 205f 3230 3230  20.08.0... _2020
+00005030: 2e30 352e 333a 2068 7474 7073 3a2f 2f67  .05.3: https://g
+00005040: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+00005050: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+00005060: 652f 3230 3230 2e30 352e 322e 2e2e 3230  e/2020.05.2...20
+00005070: 3230 2e30 352e 330a 2e2e 205f 3230 3230  20.05.3... _2020
+00005080: 2e30 352e 323a 2068 7474 7073 3a2f 2f67  .05.2: https://g
+00005090: 6974 6875 622e 636f 6d2f 6d64 6f6d 6b65  ithub.com/mdomke
+000050a0: 2f73 6368 7769 6674 792f 636f 6d70 6172  /schwifty/compar
+000050b0: 652f 3230 3230 2e30 352e 312e 2e2e 3230  e/2020.05.1...20
+000050c0: 3230 2e30 352e 320a 0a2e 2e20 5f50 4550  20.05.2.... _PEP
+000050d0: 2d30 3536 313a 2068 7474 7073 3a2f 2f77  -0561: https://w
+000050e0: 7777 2e70 7974 686f 6e2e 6f72 672f 6465  ww.python.org/de
+000050f0: 762f 7065 7073 2f70 6570 2d30 3536 312f  v/peps/pep-0561/
+00005100: 2370 6163 6b61 6769 6e67 2d74 7970 652d  #packaging-type-
+00005110: 696e 666f 726d 6174 696f 6e0a            information.
```

### Comparing `schwifty-2024.5.0/devbox.lock` & `schwifty-2024.5.1/devbox.lock`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/.github/workflows/lint-and-test.yml` & `schwifty-2024.5.1/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/.github/workflows/publish.yml` & `schwifty-2024.5.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/docs/Makefile` & `schwifty-2024.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/docs/source/api.rst` & `schwifty-2024.5.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/docs/source/conf.py` & `schwifty-2024.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/docs/source/examples.rst` & `schwifty-2024.5.1/docs/source/examples.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/docs/source/ilikewhatugot.png` & `schwifty-2024.5.1/docs/source/ilikewhatugot.png`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/docs/source/index.rst` & `schwifty-2024.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/docs/source/troubleshooting.rst` & `schwifty-2024.5.1/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bban.py` & `schwifty-2024.5.1/schwifty/bban.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bic.py` & `schwifty-2024.5.1/schwifty/bic.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/common.py` & `schwifty-2024.5.1/schwifty/common.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/exceptions.py` & `schwifty-2024.5.1/schwifty/exceptions.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/iban.py` & `schwifty-2024.5.1/schwifty/iban.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/registry.py` & `schwifty-2024.5.1/schwifty/registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from __future__ import annotations
 
 import itertools
 import json
-import pathlib
-import sys
 from collections import defaultdict
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Union
 
 
 try:
     from importlib.resources import files
-    from importlib.resources.abc import Traversable
 except ImportError:
     from importlib_resources import files  # type: ignore
-    from importlib_resources.abc import Traversable  # type: ignore
 
 
 Key = Union[str, tuple]
 Value = Union[Dict[Key, Any], List[Dict[Key, Any]]]
 
 _registry: dict[Key, Value] = {}
 
@@ -47,21 +43,16 @@
 
 
 def get(name: Key) -> Value:
     if has(name):
         return _registry[name]
 
     data = None
-    package_path: Traversable | Path
-    if getattr(sys, "frozen", False) and hasattr(sys, "_MEIPASS"):
-        package_path = Path(sys._MEIPASS)
-    else:
-        package_path = files(__package__)
-    directory = package_path / f"{name}_registry"
-    assert isinstance(directory, pathlib.Path)
+    directory = files(__package__) / f"{name}_registry"
+    assert isinstance(directory, Path)
     for entry in sorted(directory.glob("*.json")):
         with entry.open(encoding="utf-8") as fp:
             chunk = json.load(fp)
             if data is None:
                 data = chunk
             elif isinstance(data, list):
                 data.extend(chunk)
```

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/README.md` & `schwifty-2024.5.1/schwifty/bank_registry/README.md`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_at.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_at.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_ba.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_ba.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_be.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_be.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_ch.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_ch.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_cz.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_cz.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_de.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_de.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_ee.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_ee.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_es.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_es.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_fi.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_fi.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_ge.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_ge.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_hr.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_hr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_hu.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_hu.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_it.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_it.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_kz.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_kz.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_lt.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_lt.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_lv.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_lv.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_md.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_md.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_nl.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_nl.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_no.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_no.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_pl.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_pl.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_ro.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_ro.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_rs.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_rs.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_se.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_se.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_si.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_si.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_sk.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_sk.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/generated_ua.json` & `schwifty-2024.5.1/schwifty/bank_registry/generated_ua.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_ad.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_ad.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_ae.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_ae.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_bg.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_bg.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_cr.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_cr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_cy.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_cy.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_es.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_es.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_fr.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_fr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_gb.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_gb.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_gr.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_gr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_ie.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_ie.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_is.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_is.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_it.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_it.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_lu.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_lu.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_me.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_me.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_pt.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_pt.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_sa.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_sa.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/bank_registry/manual_tr.json` & `schwifty-2024.5.1/schwifty/bank_registry/manual_tr.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/__init__.py` & `schwifty-2024.5.1/schwifty/checksum/__init__.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/czech_republic.py` & `schwifty-2024.5.1/schwifty/checksum/czech_republic.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/estonia.py` & `schwifty-2024.5.1/schwifty/checksum/estonia.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/france.py` & `schwifty-2024.5.1/schwifty/checksum/france.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/germany.py` & `schwifty-2024.5.1/schwifty/checksum/germany.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/iceland.py` & `schwifty-2024.5.1/schwifty/checksum/iceland.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/italy.py` & `schwifty-2024.5.1/schwifty/checksum/italy.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/netherlands.py` & `schwifty-2024.5.1/schwifty/checksum/netherlands.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/norway.py` & `schwifty-2024.5.1/schwifty/checksum/norway.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/poland.py` & `schwifty-2024.5.1/schwifty/checksum/poland.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/checksum/spain.py` & `schwifty-2024.5.1/schwifty/checksum/spain.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/iban_registry/README.md` & `schwifty-2024.5.1/schwifty/iban_registry/README.md`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/iban_registry/generated.json` & `schwifty-2024.5.1/schwifty/iban_registry/generated.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/schwifty/iban_registry/overwrite.json` & `schwifty-2024.5.1/schwifty/iban_registry/overwrite.json`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_at.py` & `schwifty-2024.5.1/scripts/get_bank_registry_at.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_be.py` & `schwifty-2024.5.1/scripts/get_bank_registry_be.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_ch.py` & `schwifty-2024.5.1/scripts/get_bank_registry_ch.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_cz.py` & `schwifty-2024.5.1/scripts/get_bank_registry_cz.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_de.py` & `schwifty-2024.5.1/scripts/get_bank_registry_de.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_es.py` & `schwifty-2024.5.1/scripts/get_bank_registry_es.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_fi.py` & `schwifty-2024.5.1/scripts/get_bank_registry_fi.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_hr.py` & `schwifty-2024.5.1/scripts/get_bank_registry_hr.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_hu.py` & `schwifty-2024.5.1/scripts/get_bank_registry_hu.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_it.py` & `schwifty-2024.5.1/scripts/get_bank_registry_it.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_lt.py` & `schwifty-2024.5.1/scripts/get_bank_registry_lt.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_lv.py` & `schwifty-2024.5.1/scripts/get_bank_registry_lv.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_nl.py` & `schwifty-2024.5.1/scripts/get_bank_registry_nl.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_no.py` & `schwifty-2024.5.1/scripts/get_bank_registry_no.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_pl.py` & `schwifty-2024.5.1/scripts/get_bank_registry_pl.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_ro.py` & `schwifty-2024.5.1/scripts/get_bank_registry_ro.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_se.py` & `schwifty-2024.5.1/scripts/get_bank_registry_se.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_si.py` & `schwifty-2024.5.1/scripts/get_bank_registry_si.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_sk.py` & `schwifty-2024.5.1/scripts/get_bank_registry_sk.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_bank_registry_ua.py` & `schwifty-2024.5.1/scripts/get_bank_registry_ua.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/scripts/get_iban_registry.py` & `schwifty-2024.5.1/scripts/get_iban_registry.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/tests/test_bic.py` & `schwifty-2024.5.1/tests/test_bic.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/tests/test_checksum.py` & `schwifty-2024.5.1/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/tests/test_iban.py` & `schwifty-2024.5.1/tests/test_iban.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/tests/test_registry.py` & `schwifty-2024.5.1/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/LICENSE` & `schwifty-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/README.rst` & `schwifty-2024.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/hatch.toml` & `schwifty-2024.5.1/hatch.toml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/pyproject.toml` & `schwifty-2024.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `schwifty-2024.5.0/PKG-INFO` & `schwifty-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: schwifty
-Version: 2024.5.0
+Version: 2024.5.1
 Project-URL: Changelog, https://github.com/mdomke/schwifty/blob/main/CHANGELOG.rst
 Project-URL: Documentation, https://schwifty.readthedocs.io/en/latest/
 Project-URL: Homepage, http://github.com/mdomke/schwifty
 Author-email: Martin Domke <mail@martindomke.net>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

