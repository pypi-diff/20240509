# Comparing `tmp/glyphspkg-0.1.9.tar.gz` & `tmp/glyphspkg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glyphspkg-0.1.9.tar", last modified: Wed Aug 30 17:03:55 2023, max compression
+gzip compressed data, was "glyphspkg-0.2.0.tar", last modified: Thu May  9 12:19:27 2024, max compression
```

## Comparing `glyphspkg-0.1.9.tar` & `glyphspkg-0.2.0.tar`

### file list

```diff
@@ -1,1436 +1,1435 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.310554 glyphspkg-0.1.9/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.034553 glyphspkg-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.034553 glyphspkg-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (999)     1142 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (999)     1821 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.034553 glyphspkg-0.1.9/.vscode/
--rw-r--r--   0 runner    (1001) docker     (999)      356 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (999)     1069 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.034553 glyphspkg-0.1.9/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.038553 glyphspkg-0.1.9/Lib/glyphspkg/
--rw-r--r--   0 runner    (1001) docker     (999)      108 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/Lib/glyphspkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      160 2023-08-30 17:03:54.000000 glyphspkg-0.1.9/Lib/glyphspkg/_version.py
--rw-r--r--   0 runner    (1001) docker     (999)     1987 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/Lib/glyphspkg/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (999)     8506 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/Lib/glyphspkg/filenames.py
--rw-r--r--   0 runner    (1001) docker     (999)     2781 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/Lib/glyphspkg/package_to_single.py
--rw-r--r--   0 runner    (1001) docker     (999)     1291 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/Lib/glyphspkg/plist.py
--rw-r--r--   0 runner    (1001) docker     (999)      176 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/Lib/glyphspkg/single_to_package.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.038553 glyphspkg-0.1.9/Lib/glyphspkg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2040 2023-08-30 17:03:54.000000 glyphspkg-0.1.9/Lib/glyphspkg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)   104498 2023-08-30 17:03:55.000000 glyphspkg-0.1.9/Lib/glyphspkg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 17:03:54.000000 glyphspkg-0.1.9/Lib/glyphspkg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       53 2023-08-30 17:03:54.000000 glyphspkg-0.1.9/Lib/glyphspkg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       22 2023-08-30 17:03:54.000000 glyphspkg-0.1.9/Lib/glyphspkg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       10 2023-08-30 17:03:54.000000 glyphspkg-0.1.9/Lib/glyphspkg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-30 17:03:54.000000 glyphspkg-0.1.9/Lib/glyphspkg.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (999)     2040 2023-08-30 17:03:55.310554 glyphspkg-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1180 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (999)      257 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)     1173 2023-08-30 17:03:55.310554 glyphspkg-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)       69 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.038553 glyphspkg-0.1.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.038553 glyphspkg-0.1.9/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.038553 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/
--rw-r--r--   0 runner    (1001) docker     (999)      324 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/UIState.plist
--rw-r--r--   0 runner    (1001) docker     (999)    55322 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/fontinfo.plist
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-30 17:03:55.310554 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/
--rw-r--r--   0 runner    (1001) docker     (999)      386 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1458 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_E_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      515 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_E_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      348 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_P_L_iota.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1772 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_P_L_rho.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      549 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_P_L_tildedieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_breve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      499 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_breveacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      607 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevedotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      499 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevegrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      515 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevehookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      499 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevetilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      519 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      627 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexdotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      519 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexgrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      535 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      519 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflextilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      475 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_dotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_grave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_hookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      336 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_lpha.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      506 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_lphatonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      467 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_macron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1119 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_ogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      459 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_ring.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_tilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2020 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/B_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1317 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/B_e-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      335 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/B_eta.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1720 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      251 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_R_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1164 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_cedilla.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      531 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      527 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_dotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1162 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_he-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      660 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_hedescender-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      334 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_hi.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1381 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      574 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_croat.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1307 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_e-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      961 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_elta.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1727 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_je-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      388 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_ze-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      829 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_zhe-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1634 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1290 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      257 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_M_quad.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      556 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_breve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      519 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      627 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexdotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      519 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexgrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      535 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      519 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflextilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      475 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      479 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_dotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_dotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1957 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_f-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_grave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_hookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      974 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_l-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_m-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      467 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_macron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_n-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      684 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ndescender-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1319 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ng.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1167 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2024 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_open.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      338 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_psilon.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      524 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_psilontonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_r-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1642 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_reversed-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_s-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      334 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ta.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_tatonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      571 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_th.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      512 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_tilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      895 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/F_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1001 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/F_doubleS_truck.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1882 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      354 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_amma.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      556 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_breve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      531 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      487 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_commaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      527 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_dotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      867 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_e-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1619 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_ermandbls.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      615 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_hestroke-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      688 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_heupturn-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      532 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_je-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      961 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_a-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1317 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_ardsign-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      620 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_bar.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      531 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      386 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1283 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1390 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_a-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      556 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_breve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      475 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      527 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_dotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_dotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_e-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_grave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_hookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1249 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_i-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      581 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_ishort-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      467 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_macron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      474 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_o-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1118 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_ogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      335 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_ota.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      478 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_otadieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      505 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_otatonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_tilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1880 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_u-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1212 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/J_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      531 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/J_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/J_e-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1105 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1108 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_a-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      403 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_a-cy.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      685 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_adescender-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      686 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_adescender-cy.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      963 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_aiS_ymbol.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      932 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_aiS_ymbol.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      336 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_appa.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      353 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_appa.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      487 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_commaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_commaaccent.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      514 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_je-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      530 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_je-cy.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      840 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      867 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_ambda.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      460 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      487 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_commaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      539 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_dot.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1775 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_je-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      650 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_slash.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1584 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/M_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      333 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/M_u.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1226 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      233 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_U_L_L_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      520 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_commaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1227 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_doubleS_truck.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1620 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_je-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_tilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      333 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_u.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      386 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2368 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2077 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_E_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1826 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_barred-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      556 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_breve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      519 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      627 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexdotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      519 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexgrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      535 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      519 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflextilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      475 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_dotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_grave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1047 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horn.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      528 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hornacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      492 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horndotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      528 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horngrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      496 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hornhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      528 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horntilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      539 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hungarumlaut.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      515 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_macron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1833 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_mega.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      518 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_megatonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      338 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_micron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      508 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_microntonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2598 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_ogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2168 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_slash.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      531 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_slashacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_tilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1390 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      669 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_e-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      400 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_hi.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      351 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_i.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1308 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_si.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2012 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Q_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2466 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Q_doubleS_truck.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1636 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      520 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_commaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      334 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_ho.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2199 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      238 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_P_C_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1362 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_cedilla.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1730 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_chwa-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1763 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_chwa.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      531 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      520 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_commaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3657 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_doubleS_truck.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      829 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_ha-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      989 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_hcha-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      500 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_hha-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      825 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_igma.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1245 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_oftsign-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      924 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      334 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_au.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      610 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_bar.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1209 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_cedilla.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      520 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_commaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_e-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1818 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_heta.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1329 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_horn.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      836 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_se-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1385 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_she-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1066 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1652 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      556 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_breve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      475 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_dotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_grave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1079 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horn.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      528 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hornacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      492 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horndotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      528 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horngrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      496 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hornhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      528 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horntilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      539 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hungarumlaut.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      515 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_macron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2104 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_ogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      338 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_psilon.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      481 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_psilondieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      508 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_psilontonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      507 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_ring.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      577 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_short-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      394 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_straight-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      643 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_straightstroke-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_tilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1016 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/V_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/V_e-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1811 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      464 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      464 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_grave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1440 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/X_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      997 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/X_i.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1203 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      475 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_dotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1555 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_eru-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      464 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_grave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_hookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      522 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_i-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      467 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_macron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      512 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_tilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      886 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      511 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      527 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_dotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      984 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_doubleS_truck.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2030 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_e-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      335 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_eta.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1202 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_he-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1203 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_he-cy.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      908 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/_notdef.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1339 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/_similiar_tilda.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      386 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/a-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2214 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/a.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/aacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abreve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      484 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abreveacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      577 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abrevedotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      484 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abrevegrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      500 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abrevehookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      484 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abrevetilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      468 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      597 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexdotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexgrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      520 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflextilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      410 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acute.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      405 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      789 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acutecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      800 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acutecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      460 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/adieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/adotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3415 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ae.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      500 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/aeacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/agrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      465 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ahookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      336 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/alpha.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      533 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/alphatonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      452 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/amacron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2331 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     4342 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_ampersand.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     6403 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_ampersand_ampersand.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2788 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      403 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/anoteleia.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1079 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/aogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      545 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/apostrophemod.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      636 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/approxequal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      444 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/aring.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      897 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciicircum.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      985 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciicircum_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1338 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1860 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_asciitilde.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2825 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_asciitilde_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1332 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_at.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2052 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1407 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2350 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      788 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_asterisk_asterisk.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2636 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      560 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_slash.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3679 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asteriskoperator.circled.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      663 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asymptoticallyequal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2806 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/at.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2951 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/at_underscore.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/atilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1905 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/b.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      546 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/backslash.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      839 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ballotX_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      571 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1058 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_bar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1003 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_bar_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1126 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      729 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      965 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2032 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_braceright.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      958 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bracketright.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      867 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1193 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_equal_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1070 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      706 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      905 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_hyphen_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2054 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/be-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      913 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bell-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2775 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/beta.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2777 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bitcoin.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      859 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackC_ircle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      542 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackD_iamond.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      549 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackS_mallS_quare.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      526 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackS_quare.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1213 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      964 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      965 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      795 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1211 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      962 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      963 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      817 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_ertical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1628 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1223 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1224 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      889 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndH_orizontalS_ingle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      805 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndL_eftS_ingle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      806 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndR_ightS_ingle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      725 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndH_orizontalL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      641 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndL_eftL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      805 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndL_eftU_pL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      642 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndR_ightL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      806 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndR_ightU_pL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      889 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndU_pH_orizontalL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      725 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndH_orizontalH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      641 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndL_eftH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      805 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndL_eftU_pH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      642 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndR_ightH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      806 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndR_ightU_pH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      889 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndU_pH_orizontalH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      970 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndH_orizontalD_ouble.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      799 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndL_eftD_ouble.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      800 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndR_ightD_ouble.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      798 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_oubleD_ashH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      808 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_oubleD_ashV_ertical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      551 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_own.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      720 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      636 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      637 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      551 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      545 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      714 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyL_eftA_ndL_ightR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1287 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyQ_uadrupleD_ashH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1291 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyQ_uadrupleD_ashV_ertical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      546 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1041 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyT_ripleD_ashH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1051 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyT_ripleD_ashV_ertical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      549 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_p.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      718 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      634 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      723 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndL_ightD_own.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      635 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      561 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_ertical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      886 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      724 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      725 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      966 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftD_ownH_eavyA_ndR_ightU_pL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      802 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightD_ownL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      800 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightU_pL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      890 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightV_erticalL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      802 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightD_ownH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      800 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightU_pH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      890 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightV_erticalH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      966 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftU_pH_eavyA_ndR_ightD_ownL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      873 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcD_ownA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      880 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcD_ownA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      877 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcU_pA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      884 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcU_pA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1034 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalC_ross.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      654 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalU_pperL_eftT_oL_owerR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      654 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalU_pperR_ightT_oL_owerL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      798 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_oubleD_ashH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      808 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_oubleD_ashV_ertical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      551 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_own.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      720 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      636 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      637 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      551 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      545 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      714 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightL_eftA_ndH_eavyR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1287 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightQ_uadrupleD_ashH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1291 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightQ_uadrupleD_ashV_ertical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      546 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1041 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightT_ripleD_ashH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1051 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightT_ripleD_ashV_ertical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      549 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_p.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      723 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndH_eavyD_own.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      718 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      634 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      635 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      561 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_ertical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      886 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndH_orizontal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      724 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndL_eft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      725 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndR_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      966 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightD_ownH_eavyA_ndL_eftU_pL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      802 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftD_ownL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      800 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftU_pL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      890 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftV_erticalL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      802 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftD_ownH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      800 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftU_pH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      890 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftV_erticalH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      966 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightU_pH_eavyA_ndL_eftD_ownL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      887 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndH_orizontalS_ingle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      803 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndL_eftS_ingle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      804 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndR_ightS_ingle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      889 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndD_ownH_orizontalL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      723 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndH_orizontalL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      805 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndL_eftD_ownL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      639 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndL_eftL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      806 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndR_ightD_ownL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      640 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndR_ightL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      889 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndD_ownH_orizontalH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      723 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndH_orizontalH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      805 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndL_eftD_ownH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      639 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndL_eftH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      806 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndR_ightD_ownH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      640 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndR_ightH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      968 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndH_orizontalD_ouble.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      797 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndL_eftD_ouble.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      798 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndR_ightD_ouble.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1217 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndH_orizontalS_ingle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      986 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndL_eftS_ingle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      987 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndR_ightS_ingle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      891 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndH_orizontalL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      729 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndL_eftL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      730 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndR_ightL_ight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      891 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndH_orizontalH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      729 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndL_eftH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      730 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndR_ightH_eavy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1205 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndH_orizontalD_ouble.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      887 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndL_eftD_ouble.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      888 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndR_ightD_ouble.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1904 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceleft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2222 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceleft_bar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1897 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceright.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      702 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      953 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_bar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1693 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_bar_bar_bracketright.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      613 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_less.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      868 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleftwithquill.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      699 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketright.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1879 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketright_numbersign.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      868 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketrightwithquill.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      410 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/breve.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      405 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/breve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1268 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevebelowcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1107 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1210 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1222 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1567 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_acutecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1469 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_acutecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1570 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_gravecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1472 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_gravecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2185 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_hookabovecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2079 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_hookabovecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2427 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_tildecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2321 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_tildecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1218 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/breveinvertedcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      790 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brokenbar.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      863 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bullet.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      454 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bulletoperator.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2548 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bullseye.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1731 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/c.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      915 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cancel-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      410 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caron.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      405 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      795 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.alt.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      913 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      925 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      719 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/carriageR_eturn-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ccaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1314 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ccedilla.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      516 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ccircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      512 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cdotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      413 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cedilla.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1433 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cedillacomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1443 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cedillacomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      616 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1159 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/che-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      616 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/checkmark.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      658 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/chedescender-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      593 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/chi.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      430 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflex.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      425 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      920 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      930 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1174 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_acutecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1166 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_acutecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1181 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_gravecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1170 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_gravecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1725 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_hookabovecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1722 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_hookabovecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2046 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_tildecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2029 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_tildecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1407 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1415 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      587 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      749 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon_colon.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      755 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1980 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      601 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      589 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_less.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      601 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_question.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      670 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_question_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1885 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colonequals.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      540 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/comma.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      695 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.alt.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      819 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      831 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      809 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaturnedabovecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      811 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaturnedabovecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1655 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/complement.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      884 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/congruent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      654 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      863 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/coproduct.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2791 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/copyright.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      566 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/curlybracketextension.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1064 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/curlyor.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2671 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/currency.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1900 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/d.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      857 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dagger.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1166 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/daggerdbl.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      923 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dataL_inkE_scape-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1047 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dblgravecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1058 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dblgravecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2144 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dcaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2138 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dcroat.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2052 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/de-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1429 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/degree.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      915 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/delete-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3069 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/delta.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      935 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolF_our-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      931 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolO_ne-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      939 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolT_hree-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      931 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolT_wo-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      422 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresis.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      417 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1820 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresisbelowcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1723 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresiscomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1754 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresiscomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1679 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresistonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1656 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/divide.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      528 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/divides.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      414 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/divisionslash.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1918 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dje-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2570 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dollar.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3143 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dollar_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2383 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dong.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      426 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccent.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      421 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1144 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccentcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1154 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccentcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1185 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotbelowcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1195 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotbelowcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      973 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotminus.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     4358 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dottedC_ircle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      786 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/doubleprimemod.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2680 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/doublesubset.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1289 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      615 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downA_rrowH_ead.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downB_lackS_mallT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      508 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downB_lackT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      564 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downD_oubleA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downF_rombarA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      720 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downW_hiteS_mallT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      709 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downW_hiteT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1983 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downrightdiagonalellipsis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      388 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dze-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      829 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dzhe-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1633 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/e-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2111 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/e.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      496 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ebreve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      468 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      597 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexdotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexgrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      520 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflextilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      460 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/edieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      464 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/edotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/edotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2591 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ef-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/egrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      465 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ehookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2531 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eightinferior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2565 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eightsuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      974 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/el-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1319 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/element.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2188 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ellipsis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1988 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ellipsisvertical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1340 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/em-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      452 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/emacron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      531 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/emdash.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1623 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/emptyset.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      825 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/en-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      716 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fM_edium-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      918 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ext-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      926 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ransmission-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      931 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ransmissionB_lock-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      533 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endash.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1237 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endescender-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      531 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endofproof.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1568 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eng.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      916 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/enquiry-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2676 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2180 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/epsilon.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      553 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/epsilontonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      772 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1914 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_colon.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2500 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_colon_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      788 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1055 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1071 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_equal.liga.old.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      948 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1452 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_exclam_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      930 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1259 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_greater_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1256 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_less_less.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1202 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_slash_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1016 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equivalence.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/er-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1640 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ereversed-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      415 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/es-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      915 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/escape-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1709 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/estimated.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1243 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eta.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      537 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/etatonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2106 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eth.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      497 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/etilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2085 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/euro.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1663 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/excess.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1238 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1163 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1305 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1552 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal_equal.liga.old.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      595 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_exclam.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1277 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclamdown.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      834 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/existential.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1487 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/f.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      718 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fileS_eparator-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      419 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/firsttonechinese.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1747 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/five.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      470 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fiveinferior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1655 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fivesuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2996 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/flat-musical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1492 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/florin.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      713 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/formF_eed-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1568 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/four-gujarati.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      829 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/four.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      431 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fourinferior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      857 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/foursuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      526 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fraction.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      542 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fullB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2388 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/g.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      496 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1333 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gamma.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      496 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gbreve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      496 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gcaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      516 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gcircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      487 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gcommaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      512 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gdotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2368 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ge-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      358 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/germandbls.calt.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2286 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/germandbls.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1062 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ghestroke-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      689 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gheupturn-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      517 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gje-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      410 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/grave.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      404 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/grave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      792 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gravecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      802 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gravecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      886 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      626 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_bracketright.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      592 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_colon.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1189 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1279 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_equal_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      605 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1298 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      725 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1095 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      746 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      950 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_hyphen_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      679 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greaterequal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1397 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greaterorequivalent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      719 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/groupS_eparator-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      929 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guillemetleft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      927 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guillemetright.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      618 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guilsinglleft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      618 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guilsinglright.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1262 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/h.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ha-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1316 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hardsign-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      407 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hbar.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      554 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hcircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1418 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyC_ircle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      637 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyleftpointinganglebracketornament.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      643 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyleftpointinganglequotationmarkornament.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      572 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyrightpointinganglebracketornament.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      596 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyrightpointinganglequotationmarkornament.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      623 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/highV_oltageS_ign.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1398 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hookabovecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1412 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hookabovecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      725 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horizontalT_abulation-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1247 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horncomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1268 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horncomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      835 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/house.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      438 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlaut.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      433 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlaut.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1043 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlautcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1055 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlautcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      537 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1365 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_asciitilde.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      694 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_bar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      730 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1057 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_greater_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      778 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      743 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1046 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      728 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_less.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1055 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_less_less.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      404 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphentwo.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      482 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/i-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/i.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1388 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ia-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      469 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      517 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ibreve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      489 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/icircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      481 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      470 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      605 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1102 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idotless.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ie-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      469 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/igrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      486 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ihookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1486 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ii-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      521 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iishort-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      473 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/imacron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2778 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/infinity.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1177 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/integral.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      449 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/intersection.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      507 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/io-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1263 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1050 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iota.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      472 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iotadieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      531 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iotadieresistonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      445 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iotatonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      517 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/itilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1879 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iu-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/j.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      537 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/jcircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1085 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/jdotless.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      483 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/je-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1106 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/k.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1108 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/k.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1008 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ka-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1009 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ka-cy.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1031 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kadescender-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1032 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kadescender-cy.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1474 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kaiS_ymbol.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      354 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kappa.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      371 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kappa.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      472 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kcommaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      489 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kcommaaccent.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      409 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kgreenlandic.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      426 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kgreenlandic.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      517 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kje-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      533 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kje-cy.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1153 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/l.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      991 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/l.ss01.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      463 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lacute.ss01.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      906 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lambda.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      601 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lambdastroke.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1417 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/largeC_ircle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      460 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lcaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      477 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lcaron.ss01.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      472 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lcommaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      489 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lcommaaccent.ss01.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      584 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ldot.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      508 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ldot.ss01.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1286 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      489 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lackP_ointer.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      546 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lackS_mallT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      508 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lackT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      542 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      628 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftC_eiling.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      553 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftF_iveE_ighthsB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      624 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftF_loor.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      501 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftH_alfB_lackS_quare.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1279 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftL_ongA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      545 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftO_neE_ighthB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      552 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftO_neQ_uarterB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1999 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1641 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightD_oubleA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2004 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightL_ongA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3220 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightW_aveA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      554 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftS_evenE_ighthsB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      554 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftT_hreeE_ighthsB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      555 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftT_hreeQ_uartersB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      497 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftT_woheadedA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      489 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftW_hiteP_ointer.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      720 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftW_hiteS_mallT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      712 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftW_hiteT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      680 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftanglebracket-math.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      886 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketlowerhook.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1518 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketmiddlepiece.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      888 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketupperhook.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1205 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftdoubleanglebracket-math.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      571 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketextension.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      649 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketlowercorner.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      645 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketuppercorner.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      542 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftwhitesquarebracket-math.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      885 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2047 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2978 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde_asciitilde.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2182 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2487 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asterisk.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2799 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asterisk_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      819 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      705 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_bar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      965 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_bar_bar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1305 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      580 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_colon.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2765 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_dollar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3133 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_dollar_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1202 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1192 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_bar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      957 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1304 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_equal_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1273 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1271 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_less.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1603 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_exclam_hyphen_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1352 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      742 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      902 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_bar.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      944 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1017 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      942 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_less.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      579 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2694 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_asciitilde.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1289 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1086 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      734 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_less.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1211 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_numbersign_hyphen_hyphen.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      981 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_plus.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1174 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_plus_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      798 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_slash.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1116 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_slash_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      667 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lessequal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1381 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lessorequivalent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      713 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lineF_eed-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1877 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/literS_ign.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1774 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lje-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      644 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicaland.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      614 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicalnot.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      651 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicalor.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1181 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/longs.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      548 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerF_iveE_ighthsB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerH_alfB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerL_eftB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      552 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerO_neE_ighthB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerO_neQ_uarterB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      554 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerR_ightB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      746 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerR_ightD_iagonalH_alfB_lackS_quare.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      549 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerS_evenE_ighthsB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      549 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerT_hreeE_ighthsB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      550 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerT_hreeQ_uartersB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      363 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowernumeral-greek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      454 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowringmod.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1554 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowtildemod.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1547 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lozenge.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      628 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lslash.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      597 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lslash.ss01.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1923 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/m.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      414 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macron.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      409 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      825 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macronbelowcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      787 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macroncomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      797 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macroncomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      339 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/micro.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2594 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/midlinehorizontalellipsis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1836 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/minus.circled.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      400 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/minus.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      539 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/minute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1412 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/mu.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1669 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multimap.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      853 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiplicationX_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1518 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiply.circled.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      849 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiply.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1962 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multisetunion.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1472 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/n.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1996 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nA_ryC_ircledD_otO_perator.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      689 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nA_ryS_quareU_nionO_perator.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      573 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/napostrophe.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      278 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nbspace.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ncaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      472 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ncommaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      928 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/negativeA_cknowledge-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1159 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/neitherapproximatelynoractuallyequalto.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1663 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/neitherasubsetofnorequalto.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      712 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/newline-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1687 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nine.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      470 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nineinferior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1751 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ninesuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1621 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nje-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1291 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/northE_astA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1291 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/northW_estA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      881 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notalmostequalto.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      652 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notcontains.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      648 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notelement.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      640 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notequal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      600 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notgreater.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      881 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notgreaternorequal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      629 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notidentical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      588 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notless.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      871 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notlessnorequal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      644 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notsubset.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      652 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notsuperset.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ntilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      333 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nu.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      913 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/null-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1682 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3381 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_braceleft.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1891 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_bracketleft.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1594 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_colon.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      940 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1401 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_exclam.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2842 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     4041 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign_numbersign.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     5285 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign_numbersign_numbersign.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1887 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_parenleft.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3305 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_question.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1858 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_underscore.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2516 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_underscore_parenleft.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      547 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numeral-greek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2521 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numero.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      386 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/o-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2269 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/o.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1825 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/obarred-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      496 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/obreve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      468 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      597 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexdotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexgrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      520 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflextilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      460 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/odieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      461 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/odotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2883 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oe.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      409 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1268 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ogonekcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1278 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ogonekcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ograve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1047 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorn.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohornacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      477 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorndotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorngrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      481 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohornhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorntilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohungarumlaut.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      452 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omacron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3004 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omega.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      545 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omegatonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      338 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omicron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      439 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omicrontonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      781 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/one.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      409 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onedotenleader.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2256 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onehalf.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      469 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oneinferior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1591 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onequarter.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      816 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onesuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2597 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1971 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/operator.circled.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      919 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/optionK_ey.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2142 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ordfeminine.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1603 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ordmasculine.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2167 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oslash.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      516 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oslashacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/otilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      535 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/overline.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1921 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/p.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1073 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/paragraph.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      759 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parallel.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1016 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      563 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftextension.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      794 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftlowerhook.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      797 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftupperhook.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1011 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenright.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      402 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenrightextension.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      495 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenrightlowerhook.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      495 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenrightupperhook.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1972 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/partialdiff.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      669 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/pe-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3083 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/percent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      862 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      552 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      595 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      753 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period_less.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      760 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period_period.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      605 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_question.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      453 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/periodcentered.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      460 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/periodcentered.loclC_A_T_.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      455 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/periodcentered.loclC_A_T_.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     4178 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/perthousand.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1616 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/phi.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      358 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/phiS_ymbol.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1454 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/pi.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3914 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/piS_ymbol.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2139 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus.circled.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      837 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1014 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1177 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_plus.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1519 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_plus_plus.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      977 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plusminus.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      857 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plussuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2073 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerO_nO_ffS_ymbol.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      933 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerO_nS_ymbol.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1101 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerS_leepS_ymbol.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2452 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerS_ymbol.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1453 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/precedes.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      639 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/precedesorequalto.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      540 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/primemod.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      857 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/product.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      645 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/projective.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     5387 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/propellor.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2517 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/proportion.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1283 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/psi.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1918 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/q.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1762 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      599 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_colon.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1052 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      603 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_period.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      611 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_question.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1789 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/questiondown.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2229 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/questionedequalto.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      368 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/questiongreek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      938 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedbl.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      796 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblbase.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      787 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblleft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      788 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblright.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      491 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quoteleft.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      450 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quoteright.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      406 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotesinglbase.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      620 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotesingle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1481 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/r.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1465 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/r.ss03.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/racute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      465 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/racute.ss03.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      832 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/radical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1417 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ratio.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rcaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      465 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rcaron.ss03.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      472 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rcommaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      489 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rcommaaccent.ss03.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      720 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/recordS_eparator-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      672 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/reflexsubset.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      680 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/reflexsuperset.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2712 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/registered.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2957 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/replacement.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1768 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rho.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1284 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      499 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lackP_ointer.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      544 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lackS_mallT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      497 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lackT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      555 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      629 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightC_eiling.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1223 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightD_oubleA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2112 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightD_oubleP_airedA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      621 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightF_loor.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1423 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightF_rombarA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      772 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightH_alfB_lackS_quare.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2036 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightH_eavyR_oundT_ippedA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      564 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightO_neE_ighthB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1474 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_ailA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2352 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_woH_eadedA_rrowW_ithT_ail.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2163 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_woheadedA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1855 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      697 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteP_ointer.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      721 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteS_mallT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      695 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      681 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightanglebracket-math.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      523 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketlowerhook.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      763 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketmiddlepiece.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      523 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketupperhook.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      540 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightdoubleanglebracket-math.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1295 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightlongA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      434 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightsquarebracketextension.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      535 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightsquarebracketlowercorner.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      535 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightsquarebracketuppercorner.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      745 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/righttack.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      969 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightwhitesquarebracket-math.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      406 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ring.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      401 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ring.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1826 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringbelowcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1738 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringcomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1749 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      888 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringequalto.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1436 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringoperator.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1703 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ruble.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2364 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/s.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1164 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scedilla.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      480 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/schwa-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1762 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/schwa.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      516 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      520 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scommaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      781 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/second.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     3325 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/section.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1196 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      619 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon_semicolon.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      797 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon_semicolon_semicolon.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      717 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/seven.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/seveninferior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      741 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sevensuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      828 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sha-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)    12362 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shadedark.glyph
--rw-r--r--   0 runner    (1001) docker     (999)    13629 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shadelight.glyph
--rw-r--r--   0 runner    (1001) docker     (999)    26827 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shademedium.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1244 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sharp-musical.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      988 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shcha-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      712 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shiftI_n-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      713 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shiftO_ut-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1768 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sigma.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2527 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sigmafinal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      414 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/similar.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1676 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/six.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      856 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sixP_ointedB_lackS_tar.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      464 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sixinferior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1750 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sixsuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      539 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      603 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_asterisk.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      776 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_asterisk_asterisk.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      938 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      947 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_equal_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1048 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_greater.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      587 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1097 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash_equal.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      749 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash_slash.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      713 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slashlongcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      703 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slashshortcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      356 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/softhyphen.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1244 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/softsign-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1288 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/southE_astA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1288 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/southW_estA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      710 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/space-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      254 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/space.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      820 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/squarecap.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      458 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/squarecup.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      926 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/squareimageoforequalto.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      779 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/staroperator.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      923 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/startO_fH_eading-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      920 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/startO_fT_ext-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1741 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sterling.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      699 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/strokelongcomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1173 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/subset.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      919 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/substitute-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1318 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/suchthat.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      859 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/summation.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1190 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/summationdoubleS_truck.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1176 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/superset.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      924 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/synchronousI_dle-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1284 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/t.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      760 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tackdown.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      983 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tau.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      604 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tbar.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      628 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1314 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcedilla.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      520 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcommaaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      680 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/te-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1818 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/theta.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      634 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/thorn.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1551 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/three.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      493 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threeT_urned.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      477 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threeinferior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2151 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threequarters.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1496 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threesuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      423 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tilde.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      405 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1640 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tildecomb.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1657 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tildecomb.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      527 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tonos.case.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      684 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2006 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/trademark.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      607 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tripleprime.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1607 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tripletilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      836 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tse-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1538 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tshe-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1295 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tugrik.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1346 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/two.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      485 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/twoT_urned.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      469 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/twoinferior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1380 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/twosuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      386 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/u-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1653 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/u.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1793 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/u.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      465 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uacute.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      496 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ubreve.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ubreve.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      468 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ucircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      533 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ucircumflex.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      460 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      525 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udieresis.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      525 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udotbelow.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ugrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ugrave.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      465 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      529 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhookabove.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1689 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorn.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2157 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorn.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      529 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornacute.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      525 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorndotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorndotbelow.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorngrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      529 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorngrave.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      481 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      497 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornhookabove.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorntilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      529 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorntilde.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      476 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhungarumlaut.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhungarumlaut.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      452 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/umacron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      517 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/umacron.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      538 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      731 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore_bar_underscore.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      553 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore_underscore.liga.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1324 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/undertie.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1540 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_0.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1663 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_1.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2497 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_2.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      586 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_0.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      619 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_1.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      586 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_2.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      625 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_3.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1135 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/union.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      718 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/unitS_eparator-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1006 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/universal.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2105 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uogonek.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1136 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uogonek.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1275 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      514 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upB_lackS_mallT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      503 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upB_lackT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      957 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upD_oubleA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2011 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upD_ownA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1432 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upF_rombarA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1225 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteA_rrow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      718 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteS_mallT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      704 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteT_riangle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperH_alfB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      650 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndL_owerL_eftA_ndL_owerR_ightB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      803 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndL_owerR_ightB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      650 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndU_pperR_ightA_ndL_owerL_eftB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      663 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndU_pperR_ightA_ndL_owerR_ightB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      541 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      748 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftD_iagonalH_alfB_lackS_quare.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1300 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftW_hiteC_ircle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      546 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperO_neE_ighthB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      651 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightA_ndL_owerL_eftA_ndL_owerR_ightB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      803 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightA_ndL_owerL_eftB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1538 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightB_lackC_ircle.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      554 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightB_lock.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1981 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uprightdiagonalellipsis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      338 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upsilon.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      466 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upsilondieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      525 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upsilondieresistonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      439 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upsilontonos.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      452 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uptack.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      444 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uring.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      509 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uring.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      454 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ushort-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      358 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ustraight-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      589 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ustraightstroke-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      496 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/utilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      513 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/utilde.ss04.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      871 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/v.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1883 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ve-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1021 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/verticalB_isectingL_ineW_hiteS_quare.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      723 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/verticalT_abulation-control.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1706 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/w.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      449 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/wacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2032 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/warningS_ign.001.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1978 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/warningS_ign.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      468 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/wcircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      461 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/wdieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      449 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/wgrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1435 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteB_ullet.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      782 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteD_iamond.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      792 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteS_mallS_quare.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      763 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteS_quare.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1297 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/x.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2018 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/xi.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1742 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/y.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      468 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ycircumflex.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      460 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ydieresis.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      563 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ydotbelow.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      840 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yen.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1469 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yeru-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      449 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ygrave.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      465 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yhookabove.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      573 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yi-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      452 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ymacron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      497 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ytilde.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      887 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/z.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zacute.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zcaron.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      464 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zdotaccent.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2187 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ze-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     2142 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zero.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1804 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zero.zero.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      254 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zeroW_idthN_oB_reakS_pace.001.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      267 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zeroW_idthN_oB_reakS_pace.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      431 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zeroinferior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1604 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zerosuperior.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1796 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zeta.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1200 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zhe-cy.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1201 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zhe-cy.ss00.glyph
--rw-r--r--   0 runner    (1001) docker     (999)     1475 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/znotationleftimagebracket.glyph
--rw-r--r--   0 runner    (1001) docker     (999)      524 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/znotationrightimagebracket.glyph
--rw-r--r--   0 runner    (1001) docker     (999)    21710 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/order.plist
--rw-r--r--   0 runner    (1001) docker     (999)  1466790 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic_orig.glyphs
--rw-r--r--   0 runner    (1001) docker     (999)     1315 2023-08-30 17:03:45.000000 glyphspkg-0.1.9/tests/package_to_single_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:19:27.892323 glyphspkg-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:19:27.660322 glyphspkg-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:19:27.664322 glyphspkg-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:19:27.664322 glyphspkg-0.2.0/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:19:27.664322 glyphspkg-0.2.0/Lib/glyphspkg/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/Lib/glyphspkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 12:19:27.000000 glyphspkg-0.2.0/Lib/glyphspkg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/Lib/glyphspkg/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/Lib/glyphspkg/filenames.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/Lib/glyphspkg/package_to_single.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/Lib/glyphspkg/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/Lib/glyphspkg/plist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/Lib/glyphspkg/single_to_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:19:27.892323 glyphspkg-0.2.0/Lib/glyphspkg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-09 12:19:27.000000 glyphspkg-0.2.0/Lib/glyphspkg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)   104499 2024-05-09 12:19:27.000000 glyphspkg-0.2.0/Lib/glyphspkg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:19:27.000000 glyphspkg-0.2.0/Lib/glyphspkg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 12:19:27.000000 glyphspkg-0.2.0/Lib/glyphspkg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 12:19:27.000000 glyphspkg-0.2.0/Lib/glyphspkg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 12:19:27.000000 glyphspkg-0.2.0/Lib/glyphspkg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:19:27.000000 glyphspkg-0.2.0/Lib/glyphspkg.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-09 12:19:27.892323 glyphspkg-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-09 12:19:27.896323 glyphspkg-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:19:27.668322 glyphspkg-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:19:27.668322 glyphspkg-0.2.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:19:27.668322 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/UIState.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    55214 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/fontinfo.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:19:27.892323 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_E_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_E_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_P_L_iota.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_P_L_rho.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_P_L_tildedieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_breve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_breveacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevedotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevegrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevehookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevetilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexdotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexgrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflextilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_dotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_grave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_hookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_lpha.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_lphatonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_macron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_ogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_ring.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_tilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/B_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/B_e-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/B_eta.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_R_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_cedilla.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_dotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_he-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_hedescender-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_hi.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_croat.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_e-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_elta.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_je-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_ze-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_zhe-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_M_quad.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_breve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexdotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexgrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflextilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_dotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_dotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_f-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_grave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_hookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_l-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_m-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_macron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_n-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ndescender-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ng.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_open.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_psilon.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_psilontonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_r-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_reversed-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_s-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ta.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_tatonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_th.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_tilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/F_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/F_doubleS_truck.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_amma.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_breve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_commaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_dotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_e-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_ermandbls.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_hestroke-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_heupturn-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_je-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_a-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_ardsign-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_bar.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_a-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_breve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_dotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_dotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_e-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_grave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_hookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_i-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_ishort-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_macron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_o-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_ogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_ota.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_otadieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_otatonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_tilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_u-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/J_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/J_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/J_e-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_a-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_a-cy.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_adescender-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_adescender-cy.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_aiS_ymbol.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_aiS_ymbol.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_appa.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_appa.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_commaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_commaaccent.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_je-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_je-cy.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_ambda.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_commaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_dot.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_je-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_slash.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/M_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/M_u.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_U_L_L_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_commaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_doubleS_truck.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_je-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_tilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_u.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_E_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_barred-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_breve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexdotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexgrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflextilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_dotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_grave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horn.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hornacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horndotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horngrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hornhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horntilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hungarumlaut.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_macron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_mega.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_megatonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_micron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_microntonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_ogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_slash.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_slashacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_tilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_e-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_hi.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_i.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_si.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Q_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Q_doubleS_truck.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_commaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_ho.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_P_C_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_cedilla.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_chwa-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_chwa.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_commaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_doubleS_truck.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_ha-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_hcha-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_hha-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_igma.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_oftsign-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_au.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_bar.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_cedilla.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_commaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_e-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_heta.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_horn.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_se-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_she-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_breve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_dotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_grave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horn.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hornacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horndotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horngrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hornhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horntilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hungarumlaut.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_macron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_ogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_psilon.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_psilondieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_psilontonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_ring.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_short-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_straight-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_straightstroke-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_tilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/V_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/V_e-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_grave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/X_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/X_i.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_dotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_eru-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_grave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_hookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_i-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_macron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_tilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_dotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_doubleS_truck.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_e-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_eta.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_he-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_he-cy.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/_notdef.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/_similiar_tilda.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/a-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/a.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/aacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abreve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abreveacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abrevedotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abrevegrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abrevehookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abrevetilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexdotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexgrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflextilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acute.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acutecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acutecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/adieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/adotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ae.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/aeacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/agrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ahookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/alpha.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/alphatonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/amacron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_ampersand.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_ampersand_ampersand.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/anoteleia.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/aogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/apostrophemod.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/approxequal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/aring.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciicircum.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciicircum_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_asciitilde.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_asciitilde_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_at.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_asterisk_asterisk.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_slash.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asteriskoperator.circled.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asymptoticallyequal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/at.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/at_underscore.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/atilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/b.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/backslash.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ballotX_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_bar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_bar_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_braceright.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bracketright.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_equal_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_hyphen_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/be-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bell-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/beta.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bitcoin.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackC_ircle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackD_iamond.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackS_mallS_quare.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackS_quare.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_ertical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndH_orizontalS_ingle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndL_eftS_ingle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndR_ightS_ingle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndH_orizontalL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndL_eftL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndL_eftU_pL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndR_ightL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndR_ightU_pL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndU_pH_orizontalL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndH_orizontalH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndL_eftH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndL_eftU_pH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndR_ightH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndR_ightU_pH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndU_pH_orizontalH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndH_orizontalD_ouble.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndL_eftD_ouble.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndR_ightD_ouble.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_oubleD_ashH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_oubleD_ashV_ertical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_own.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyL_eftA_ndL_ightR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyQ_uadrupleD_ashH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyQ_uadrupleD_ashV_ertical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyT_ripleD_ashH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyT_ripleD_ashV_ertical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_p.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndL_ightD_own.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_ertical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftD_ownH_eavyA_ndR_ightU_pL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightD_ownL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightU_pL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightV_erticalL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightD_ownH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightU_pH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightV_erticalH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftU_pH_eavyA_ndR_ightD_ownL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcD_ownA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcD_ownA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcU_pA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcU_pA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalC_ross.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalU_pperL_eftT_oL_owerR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalU_pperR_ightT_oL_owerL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_oubleD_ashH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_oubleD_ashV_ertical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_own.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightL_eftA_ndH_eavyR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightQ_uadrupleD_ashH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightQ_uadrupleD_ashV_ertical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightT_ripleD_ashH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightT_ripleD_ashV_ertical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_p.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndH_eavyD_own.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_ertical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndH_orizontal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndL_eft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndR_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightD_ownH_eavyA_ndL_eftU_pL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftD_ownL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftU_pL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftV_erticalL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftD_ownH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftU_pH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftV_erticalH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightU_pH_eavyA_ndL_eftD_ownL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndH_orizontalS_ingle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndL_eftS_ingle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndR_ightS_ingle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndD_ownH_orizontalL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndH_orizontalL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndL_eftD_ownL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndL_eftL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndR_ightD_ownL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndR_ightL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndD_ownH_orizontalH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndH_orizontalH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndL_eftD_ownH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndL_eftH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndR_ightD_ownH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndR_ightH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndH_orizontalD_ouble.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndL_eftD_ouble.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndR_ightD_ouble.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndH_orizontalS_ingle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndL_eftS_ingle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndR_ightS_ingle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndH_orizontalL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndL_eftL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndR_ightL_ight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndH_orizontalH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndL_eftH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndR_ightH_eavy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndH_orizontalD_ouble.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndL_eftD_ouble.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndR_ightD_ouble.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceleft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceleft_bar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceright.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_bar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_bar_bar_bracketright.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_less.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleftwithquill.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketright.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketright_numbersign.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketrightwithquill.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/breve.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/breve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevebelowcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_acutecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_acutecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_gravecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_gravecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_hookabovecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_hookabovecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_tildecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_tildecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/breveinvertedcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brokenbar.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bullet.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bulletoperator.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bullseye.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/c.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cancel-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caron.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.alt.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/carriageR_eturn-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ccaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ccedilla.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ccircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cdotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cedilla.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cedillacomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cedillacomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/che-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/checkmark.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/chedescender-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/chi.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflex.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_acutecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_acutecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_gravecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_gravecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_hookabovecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_hookabovecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_tildecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_tildecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon_colon.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_less.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_question.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_question_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colonequals.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/comma.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.alt.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaturnedabovecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaturnedabovecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/complement.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/congruent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/coproduct.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/copyright.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/curlybracketextension.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/curlyor.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/currency.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/d.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dagger.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/daggerdbl.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dataL_inkE_scape-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dblgravecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dblgravecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dcaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dcroat.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/de-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/degree.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/delete-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/delta.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolF_our-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolO_ne-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolT_hree-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolT_wo-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresis.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresisbelowcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresiscomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresiscomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresistonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/divide.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/divides.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/divisionslash.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dje-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dollar.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dollar_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dong.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccent.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccentcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccentcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotbelowcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotbelowcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotminus.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dottedC_ircle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/doubleprimemod.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/doublesubset.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downA_rrowH_ead.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downB_lackS_mallT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downB_lackT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downD_oubleA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downF_rombarA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downW_hiteS_mallT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downW_hiteT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downrightdiagonalellipsis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dze-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dzhe-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/e-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/e.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ebreve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexdotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexgrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflextilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/edieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/edotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/edotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ef-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/egrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ehookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eightinferior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eightsuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/el-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/element.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ellipsis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ellipsisvertical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/em-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/emacron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/emdash.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/emptyset.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/en-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fM_edium-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ext-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ransmission-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ransmissionB_lock-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endash.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endescender-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endofproof.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eng.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/enquiry-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/epsilon.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/epsilontonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_colon.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_colon_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_equal.liga.old.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_exclam_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_greater_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_less_less.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_slash_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equivalence.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/er-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ereversed-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/es-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/escape-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/estimated.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eta.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/etatonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eth.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/etilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/euro.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/excess.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal_equal.liga.old.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_exclam.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclamdown.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/existential.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/f.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fileS_eparator-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/firsttonechinese.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/five.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fiveinferior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fivesuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/flat-musical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/florin.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/formF_eed-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/four-gujarati.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/four.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fourinferior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/foursuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fraction.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fullB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/g.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gamma.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gbreve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gcaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gcircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gcommaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gdotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ge-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/germandbls.calt.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/germandbls.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ghestroke-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gheupturn-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gje-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/grave.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/grave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gravecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gravecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_bracketright.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_colon.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_equal_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_hyphen_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greaterequal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greaterorequivalent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/groupS_eparator-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guillemetleft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guillemetright.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guilsinglleft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guilsinglright.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/h.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ha-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hardsign-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hbar.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hcircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyC_ircle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyleftpointinganglebracketornament.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyleftpointinganglequotationmarkornament.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyrightpointinganglebracketornament.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyrightpointinganglequotationmarkornament.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/highV_oltageS_ign.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hookabovecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hookabovecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horizontalT_abulation-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horncomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horncomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/house.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlaut.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlaut.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlautcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlautcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_asciitilde.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_bar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_greater_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_less.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_less_less.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphentwo.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/i-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/i.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ia-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ibreve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/icircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idotless.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ie-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/igrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ihookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ii-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iishort-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/imacron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/infinity.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/integral.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/intersection.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/io-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iota.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iotadieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iotadieresistonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iotatonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/itilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iu-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/j.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/jcircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/jdotless.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/je-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/k.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/k.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ka-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ka-cy.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kadescender-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kadescender-cy.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kaiS_ymbol.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kappa.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kappa.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kcommaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kcommaaccent.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kgreenlandic.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kgreenlandic.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kje-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kje-cy.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/l.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/l.ss01.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lacute.ss01.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lambda.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lambdastroke.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/largeC_ircle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lcaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lcaron.ss01.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lcommaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lcommaaccent.ss01.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ldot.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ldot.ss01.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lackP_ointer.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lackS_mallT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lackT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftC_eiling.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftF_iveE_ighthsB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftF_loor.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftH_alfB_lackS_quare.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftL_ongA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftO_neE_ighthB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftO_neQ_uarterB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightD_oubleA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightL_ongA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightW_aveA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftS_evenE_ighthsB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftT_hreeE_ighthsB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftT_hreeQ_uartersB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftT_woheadedA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftW_hiteP_ointer.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftW_hiteS_mallT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftW_hiteT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftanglebracket-math.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketlowerhook.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketmiddlepiece.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketupperhook.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftdoubleanglebracket-math.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketextension.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketlowercorner.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketuppercorner.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftwhitesquarebracket-math.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde_asciitilde.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asterisk.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asterisk_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_bar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_bar_bar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_colon.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_dollar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_dollar_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_bar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_equal_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_less.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_exclam_hyphen_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_bar.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_less.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_asciitilde.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_less.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_numbersign_hyphen_hyphen.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_plus.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_plus_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_slash.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_slash_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lessequal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lessorequivalent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lineF_eed-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/literS_ign.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lje-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicaland.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicalnot.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicalor.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/longs.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerF_iveE_ighthsB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerH_alfB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerL_eftB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerO_neE_ighthB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerO_neQ_uarterB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerR_ightB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerR_ightD_iagonalH_alfB_lackS_quare.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerS_evenE_ighthsB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerT_hreeE_ighthsB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerT_hreeQ_uartersB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowernumeral-greek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowringmod.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowtildemod.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lozenge.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lslash.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lslash.ss01.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/m.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macron.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macronbelowcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macroncomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macroncomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/micro.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/midlinehorizontalellipsis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/minus.circled.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/minus.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/minute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/mu.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multimap.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiplicationX_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiply.circled.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiply.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multisetunion.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/n.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nA_ryC_ircledD_otO_perator.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nA_ryS_quareU_nionO_perator.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/napostrophe.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nbspace.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ncaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ncommaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/negativeA_cknowledge-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/neitherapproximatelynoractuallyequalto.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/neitherasubsetofnorequalto.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/newline-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nine.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nineinferior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ninesuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nje-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/northE_astA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/northW_estA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notalmostequalto.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notcontains.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notelement.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notequal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notgreater.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notgreaternorequal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notidentical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notless.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notlessnorequal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notsubset.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notsuperset.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ntilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nu.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/null-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_braceleft.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_bracketleft.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_colon.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_exclam.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign_numbersign.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign_numbersign_numbersign.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_parenleft.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_question.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_underscore.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_underscore_parenleft.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numeral-greek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numero.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/o-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/o.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/obarred-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/obreve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexdotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexgrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflextilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/odieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/odotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oe.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ogonekcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ogonekcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ograve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorn.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohornacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorndotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorngrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohornhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorntilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohungarumlaut.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omacron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omega.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omegatonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omicron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omicrontonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/one.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onedotenleader.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onehalf.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oneinferior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onequarter.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onesuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/operator.circled.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/optionK_ey.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ordfeminine.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ordmasculine.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oslash.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oslashacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/otilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/overline.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/p.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/paragraph.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parallel.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftextension.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftlowerhook.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftupperhook.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenright.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenrightextension.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenrightlowerhook.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenrightupperhook.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/partialdiff.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/pe-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/percent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period_less.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period_period.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_question.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/periodcentered.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/periodcentered.loclC_A_T_.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/periodcentered.loclC_A_T_.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/perthousand.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/phi.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/phiS_ymbol.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/pi.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/piS_ymbol.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus.circled.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_plus.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_plus_plus.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plusminus.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plussuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerO_nO_ffS_ymbol.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerO_nS_ymbol.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerS_leepS_ymbol.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerS_ymbol.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/precedes.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/precedesorequalto.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/primemod.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/product.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/projective.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/propellor.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/proportion.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/psi.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/q.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_colon.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_period.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_question.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/questiondown.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/questionedequalto.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/questiongreek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedbl.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblbase.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblleft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblright.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quoteleft.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quoteright.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotesinglbase.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotesingle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/r.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/r.ss03.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/racute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/racute.ss03.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/radical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ratio.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rcaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rcaron.ss03.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rcommaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rcommaaccent.ss03.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/recordS_eparator-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/reflexsubset.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/reflexsuperset.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/registered.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/replacement.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rho.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lackP_ointer.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lackS_mallT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lackT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightC_eiling.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightD_oubleA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightD_oubleP_airedA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightF_loor.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightF_rombarA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightH_alfB_lackS_quare.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightH_eavyR_oundT_ippedA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightO_neE_ighthB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_ailA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_woH_eadedA_rrowW_ithT_ail.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_woheadedA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteP_ointer.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteS_mallT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightanglebracket-math.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketlowerhook.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketmiddlepiece.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketupperhook.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightdoubleanglebracket-math.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightlongA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightsquarebracketextension.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightsquarebracketlowercorner.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightsquarebracketuppercorner.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/righttack.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightwhitesquarebracket-math.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ring.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ring.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringbelowcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringcomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringequalto.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringoperator.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ruble.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/s.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scedilla.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/schwa-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/schwa.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scommaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/second.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/section.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon_semicolon.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon_semicolon_semicolon.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/seven.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/seveninferior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sevensuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sha-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shadedark.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shadelight.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)    26827 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shademedium.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sharp-musical.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shcha-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shiftI_n-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shiftO_ut-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sigma.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sigmafinal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/similar.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/six.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sixP_ointedB_lackS_tar.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sixinferior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sixsuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_asterisk.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_asterisk_asterisk.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_equal_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_greater.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash_equal.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash_slash.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slashlongcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slashshortcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/softhyphen.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/softsign-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/southE_astA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/southW_estA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/space-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/space.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/squarecap.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/squarecup.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/squareimageoforequalto.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/staroperator.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/startO_fH_eading-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/startO_fT_ext-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sterling.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/strokelongcomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/subset.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/substitute-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/suchthat.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/summation.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/summationdoubleS_truck.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/superset.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/synchronousI_dle-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/t.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tackdown.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tau.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tbar.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcedilla.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcommaaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/te-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/theta.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/thorn.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/three.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threeT_urned.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threeinferior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threequarters.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threesuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tilde.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tildecomb.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tildecomb.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tonos.case.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/trademark.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tripleprime.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tripletilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tse-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tshe-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tugrik.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/two.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/twoT_urned.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/twoinferior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/twosuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/u-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/u.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/u.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uacute.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ubreve.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ubreve.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ucircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ucircumflex.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udieresis.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udotbelow.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ugrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ugrave.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhookabove.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorn.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorn.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornacute.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorndotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorndotbelow.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorngrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorngrave.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornhookabove.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorntilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorntilde.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhungarumlaut.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhungarumlaut.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/umacron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/umacron.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore_bar_underscore.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore_underscore.liga.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/undertie.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_0.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_1.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_2.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_0.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_1.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_2.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_3.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/union.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/unitS_eparator-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/universal.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uogonek.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uogonek.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upB_lackS_mallT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upB_lackT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upD_oubleA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upD_ownA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upF_rombarA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteA_rrow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteS_mallT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteT_riangle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperH_alfB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndL_owerL_eftA_ndL_owerR_ightB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndL_owerR_ightB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndU_pperR_ightA_ndL_owerL_eftB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndU_pperR_ightA_ndL_owerR_ightB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftD_iagonalH_alfB_lackS_quare.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftW_hiteC_ircle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperO_neE_ighthB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightA_ndL_owerL_eftA_ndL_owerR_ightB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightA_ndL_owerL_eftB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightB_lackC_ircle.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightB_lock.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uprightdiagonalellipsis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upsilon.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upsilondieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upsilondieresistonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upsilontonos.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uptack.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uring.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uring.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ushort-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ustraight-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ustraightstroke-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/utilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/utilde.ss04.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/v.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ve-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/verticalB_isectingL_ineW_hiteS_quare.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/verticalT_abulation-control.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/w.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/wacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/warningS_ign.001.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/warningS_ign.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/wcircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/wdieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/wgrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteB_ullet.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteD_iamond.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteS_mallS_quare.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteS_quare.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/x.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/xi.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/y.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ycircumflex.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ydieresis.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ydotbelow.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yen.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yeru-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ygrave.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yhookabove.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yi-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ymacron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ytilde.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/z.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zacute.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zcaron.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zdotaccent.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ze-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zero.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zero.zero.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zeroW_idthN_oB_reakS_pace.001.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zeroW_idthN_oB_reakS_pace.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zeroinferior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zerosuperior.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zeta.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zhe-cy.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zhe-cy.ss00.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/znotationleftimagebracket.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/znotationrightimagebracket.glyph
+-rw-r--r--   0 runner    (1001) docker     (127)    21710 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/order.plist
+-rw-r--r--   0 runner    (1001) docker     (127)  1466085 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic_orig.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-09 12:19:22.000000 glyphspkg-0.2.0/tests/package_to_single_test.py
```

### Comparing `glyphspkg-0.1.9/.github/workflows/publish-to-test-pypi.yml` & `glyphspkg-0.2.0/.github/workflows/publish-to-test-pypi.yml`

 * *Files 23% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 on: push
 
 jobs:
   build-n-publish:
     name: Build and publish Python distributions to PyPI and TestPyPI
     runs-on: ubuntu-latest
     environment:
-      name: pypi
+      name: release
       url: https://pypi.org/p/glyphspkg
+    permissions:
+      id-token: write
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         fetch-depth: 0
-    - name: Set up Python 3.9
-      uses: actions/setup-python@v4
+    - name: Set up Python 3.12
+      uses: actions/setup-python@v5
       with:
-        python-version: 3.9
+        python-version: 3.12
 
     - name: Install pypa/build
       run: >-
         python -m
         pip install
         build
         --user
@@ -33,15 +35,12 @@
         --wheel
         --outdir dist/
         .
 
     - name: Publish distribution to Test PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
-        password: ${{ secrets.TEST_PYPI_API_TOKEN }}
         repository-url: https://test.pypi.org/legacy/
 
     - name: Publish distribution to PyPI
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `glyphspkg-0.1.9/.gitignore` & `glyphspkg-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/LICENSE` & `glyphspkg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/Lib/glyphspkg/cmdline.py` & `glyphspkg-0.2.0/Lib/glyphspkg/cmdline.py`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/Lib/glyphspkg/filenames.py` & `glyphspkg-0.2.0/Lib/glyphspkg/filenames.py`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/Lib/glyphspkg/package_to_single.py` & `glyphspkg-0.2.0/Lib/glyphspkg/package_to_single.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import logging
 
 from glyphspkg.filenames import userNameToFileName
+from glyphspkg.paths import build_output_file_path
 from glyphspkg.plist import parse_plist_from_path, save_to_plist_path
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 
 logger = logging.getLogger(__name__)
 
 
-def package_to_single(
-    input_path: Path, output_path: Optional[Path] = None
-) -> Path:
+def package_to_single(input_path: Path, output_path: Optional[Path] = None) -> Path:
     # The main dict
     glyphs_file = convert_fontinfo(input_path)
 
     # Glyph order, is used to read individual glyphs files
     glyph_order = convert_order(input_path)
 
     # All glyphs files derived from the Glyph order list
@@ -40,39 +39,21 @@
     if uistate:
         # Why the different key casing?
         glyphs_file["DisplayStrings"] = uistate["displayStrings"]
 
     output_file_path = build_output_file_path(input_path, output_path)
     if input_path == output_file_path:
         logger.error(f"Saving would overwrite the input file {input_path}")
-        raise(FileExistsError)
+        raise FileExistsError
 
     logger.info(f"Saving: {output_file_path}")
     save_to_plist_path(glyphs_file, output_file_path)
     return output_file_path
 
 
-def build_output_file_path(
-    input_path: Path, output_path: Optional[Path] = None
-) -> Path:
-    file_name = input_path.with_suffix(".glyphs").name
-    if output_path is None:
-        # No path was specified, save next to original file
-        output_file_path = input_path.parent / file_name
-    elif output_path.is_dir():
-        # Output directory was specified, save to original file name with
-        # changed suffix in new dir
-        output_file_path = output_path / file_name
-    else:
-        # Full path with file name was specified, save there
-        output_file_path = output_path
-
-    return output_file_path
-
-
 def convert_fontinfo(input_path: Path) -> Union[Dict[Any, Any], List[Any]]:
     return parse_plist_from_path(input_path / "fontinfo.plist")
 
 
 def convert_order(input_path: Path) -> Union[Dict[Any, Any], List[Any]]:
     return parse_plist_from_path(input_path / "order.plist")
```

### Comparing `glyphspkg-0.1.9/Lib/glyphspkg.egg-info/PKG-INFO` & `glyphspkg-0.2.0/Lib/glyphspkg.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: glyphspkg
-Version: 0.1.9
-Summary: Converter from .glyphspackage to .glyphs files
+Version: 0.2.0
+Summary: Converter from .glyphspackage to .glyphs files and vice versa
 Home-page: https://github.com/jenskutilek/glyphspkg
 Author: Jens Kutilek
 License: MIT
 Project-URL: Documentation, https://github.com/jenskutilek/glyphspkg
 Project-URL: Source, https://github.com/jenskutilek/glyphspkg
 Project-URL: Tracker, https://github.com/jenskutilek/glyphspkg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
+Requires-Dist: openstep-plist>=0.3.1
 
 # glyphspkg
 
-Converter for GlyphsApp package to monolithic files.
+Converter for GlyphsApp package to monolithic files and vice versa.
 
 [Glyphs](https://glyphsapp.com) supports two different file formats, both of
 which are based on plist. One, using the suffix `.glyphs`, is a monolithic
 file, the other, using the suffix `.glyphspackage`, is a special folder that
 appears as one file on macOS.
 
 The _package_ variant has advantages when used in SCM systems, but some
@@ -48,12 +49,7 @@
   glyphsfile            Path to the glyphs file or package to be converted.
 
 options:
   -h, --help            show this help message and exit
   -o OUTPUT_PATH, --output OUTPUT_PATH
                         Output path for converted files. If omitted, the file is saved next to the original.
 ```
-
-
-## Known issues
-
-Only conversion from `.glyphspackage` to `.glyphs` is implemented at the moment.
```

### Comparing `glyphspkg-0.1.9/Lib/glyphspkg.egg-info/SOURCES.txt` & `glyphspkg-0.2.0/Lib/glyphspkg.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/publish-to-test-pypi.yml
-.vscode/settings.json
 Lib/glyphspkg/__init__.py
 Lib/glyphspkg/_version.py
 Lib/glyphspkg/cmdline.py
 Lib/glyphspkg/filenames.py
 Lib/glyphspkg/package_to_single.py
+Lib/glyphspkg/paths.py
 Lib/glyphspkg/plist.py
 Lib/glyphspkg/single_to_package.py
 Lib/glyphspkg.egg-info/PKG-INFO
 Lib/glyphspkg.egg-info/SOURCES.txt
 Lib/glyphspkg.egg-info/dependency_links.txt
 Lib/glyphspkg.egg-info/entry_points.txt
 Lib/glyphspkg.egg-info/requires.txt
```

### Comparing `glyphspkg-0.1.9/PKG-INFO` & `glyphspkg-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: glyphspkg
-Version: 0.1.9
-Summary: Converter from .glyphspackage to .glyphs files
+Version: 0.2.0
+Summary: Converter from .glyphspackage to .glyphs files and vice versa
 Home-page: https://github.com/jenskutilek/glyphspkg
 Author: Jens Kutilek
 License: MIT
 Project-URL: Documentation, https://github.com/jenskutilek/glyphspkg
 Project-URL: Source, https://github.com/jenskutilek/glyphspkg
 Project-URL: Tracker, https://github.com/jenskutilek/glyphspkg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: Topic :: Multimedia :: Graphics :: Editors :: Vector-Based
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
+Requires-Dist: openstep-plist>=0.3.1
 
 # glyphspkg
 
-Converter for GlyphsApp package to monolithic files.
+Converter for GlyphsApp package to monolithic files and vice versa.
 
 [Glyphs](https://glyphsapp.com) supports two different file formats, both of
 which are based on plist. One, using the suffix `.glyphs`, is a monolithic
 file, the other, using the suffix `.glyphspackage`, is a special folder that
 appears as one file on macOS.
 
 The _package_ variant has advantages when used in SCM systems, but some
@@ -48,12 +49,7 @@
   glyphsfile            Path to the glyphs file or package to be converted.
 
 options:
   -h, --help            show this help message and exit
   -o OUTPUT_PATH, --output OUTPUT_PATH
                         Output path for converted files. If omitted, the file is saved next to the original.
 ```
-
-
-## Known issues
-
-Only conversion from `.glyphspackage` to `.glyphs` is implemented at the moment.
```

### Comparing `glyphspkg-0.1.9/README.md` & `glyphspkg-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # glyphspkg
 
-Converter for GlyphsApp package to monolithic files.
+Converter for GlyphsApp package to monolithic files and vice versa.
 
 [Glyphs](https://glyphsapp.com) supports two different file formats, both of
 which are based on plist. One, using the suffix `.glyphs`, is a monolithic
 file, the other, using the suffix `.glyphspackage`, is a special folder that
 appears as one file on macOS.
 
 The _package_ variant has advantages when used in SCM systems, but some
@@ -26,13 +26,8 @@
 positional arguments:
   glyphsfile            Path to the glyphs file or package to be converted.
 
 options:
   -h, --help            show this help message and exit
   -o OUTPUT_PATH, --output OUTPUT_PATH
                         Output path for converted files. If omitted, the file is saved next to the original.
-```
-
-
-## Known issues
-
-Only conversion from `.glyphspackage` to `.glyphs` is implemented at the moment.
+```
```

### Comparing `glyphspkg-0.1.9/setup.cfg` & `glyphspkg-0.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = glyphspkg
-description = Converter from .glyphspackage to .glyphs files
+description = Converter from .glyphspackage to .glyphs files and vice versa
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/jenskutilek/glyphspkg
 author = Jens Kutilek
 license = MIT
 license_files = LICENSE
 classifiers = 
@@ -24,26 +24,33 @@
 zip_safe = True
 package_dir = 
 	=Lib
 packages = find:
 platforms = any
 include_package_data = True
 install_requires = 
-	openstep-plist >= 0.3.0
-python_requires = >=3.7
+	openstep-plist >= 0.3.1
+python_requires = >=3.8
 setup_requires = 
 	setuptools_scm
 
 [options.packages.find]
 where = Lib
 
 [bdist_wheel]
 universal = 1
 
 [options.entry_points]
 console_scripts = 
 	glyphspkg = glyphspkg.cmdline:main
 
+[flake8]
+select = B, C, E, F, W, T4, B9
+ignore = E203, E266, E501, W503, E741
+max-line-length = 88
+max-complexity = 19
+exclude = .git, __pycache__, build, dist, .eggs, .tox
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/fontinfo.plist` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/fontinfo.plist`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {
-.appVersion = "3124";
+.appVersion = "3306";
 .formatVersion = 3;
 axes = (
 {
 name = Weight;
 tag = wght;
 }
 );
@@ -68,23 +68,23 @@
 },
 {
 pos = 550;
 size = 10;
 },
 {
 pos = 0;
-size = "-10";
+size = -10;
 },
 {
-pos = "-110";
-size = "-10";
+pos = -110;
+size = -10;
 },
 {
-pos = "-180";
-size = "-10";
+pos = -180;
+size = -10;
 }
 );
 },
 {
 name = isFixedPitch;
 value = 1;
 },
@@ -1579,20 +1579,20 @@
 name = "Alignment Zones";
 value = (
 {
 pos = 830;
 size = 10;
 },
 {
-pos = "-110";
-size = "-10";
+pos = -110;
+size = -10;
 },
 {
-pos = "-180";
-size = "-10";
+pos = -180;
+size = -10;
 }
 );
 }
 );
 iconName = Light;
 id = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 metricValues = (
@@ -1691,20 +1691,20 @@
 name = "Alignment Zones";
 value = (
 {
 pos = 830;
 size = 10;
 },
 {
-pos = "-110";
-size = "-10";
+pos = -110;
+size = -10;
 },
 {
-pos = "-180";
-size = "-10";
+pos = -180;
+size = -10;
 }
 );
 }
 );
 id = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 metricValues = (
 {
@@ -1794,20 +1794,20 @@
 name = "Alignment Zones";
 value = (
 {
 pos = 830;
 size = 10;
 },
 {
-pos = "-110";
-size = "-10";
+pos = -110;
+size = -10;
 },
 {
-pos = "-180";
-size = "-10";
+pos = -180;
+size = -10;
 }
 );
 }
 );
 iconName = Bold;
 id = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 metricValues = (
@@ -2120,17 +2120,14 @@
 {
 customParameters = (
 {
 name = "Variable Font Origin";
 value = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 }
 );
-instanceInterpolations = {
-"EDF5EB54-295C-4C90-9A2F-67CD82979CFF" = 1;
-};
 name = Regular;
 type = variable;
 }
 );
 metrics = (
 {
 type = ascender;
@@ -2171,38 +2168,38 @@
 );
 },
 {
 key = designerURL;
 value = "https://www.jetbrains.com";
 },
 {
-key = manufacturers;
+key = licenses;
 values = (
 {
 language = dflt;
-value = JetBrains;
+value = "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license is available with a FAQ at: https://scripts.sil.org/OFL";
 }
 );
 },
 {
-key = manufacturerURL;
-value = "https://www.jetbrains.com";
+key = licenseURL;
+value = "https://scripts.sil.org/OFL";
 },
 {
-key = licenses;
+key = manufacturers;
 values = (
 {
 language = dflt;
-value = "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license is available with a FAQ at: https://scripts.sil.org/OFL";
+value = JetBrains;
 }
 );
 },
 {
-key = licenseURL;
-value = "https://scripts.sil.org/OFL";
+key = manufacturerURL;
+value = "https://www.jetbrains.com";
 },
 {
 key = trademarks;
 values = (
 {
 language = dflt;
 value = "JetBrains Mono is a trademark of JetBrains s.r.o.";
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_E_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_E_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_E_acute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_E_acute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_P_L_rho.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_P_L_rho.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_P_L_tildedieresis.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_P_L_tildedieresis.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevedotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevedotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevehookabove.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_brevehookabove.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexacute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexacute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexdotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexdotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexgrave.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexgrave.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexhookabove.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflexhookabove.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflextilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_circumflextilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_ogonek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/A_ogonek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/B_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/B_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/B_e-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/B_e-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_cedilla.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_cedilla.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_circumflex.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_circumflex.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_dotaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_dotaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_he-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_he-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_hedescender-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/C_hedescender-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_croat.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_croat.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_e-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_e-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_elta.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_elta.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_je-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_je-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_zhe-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/D_zhe-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_breve.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_breve.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexacute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexacute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexdotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexdotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexgrave.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexgrave.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexhookabove.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflexhookabove.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflextilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_circumflextilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_f-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_f-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_l-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_l-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ndescender-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ndescender-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ng.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ng.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ogonek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_ogonek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_open.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_open.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_psilontonos.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_psilontonos.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_reversed-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_reversed-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_th.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_th.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_tilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/E_tilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/F_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/F_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/F_doubleS_truck.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/F_doubleS_truck.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_breve.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_breve.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_circumflex.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_circumflex.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_dotaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_dotaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_e-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_e-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_ermandbls.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_ermandbls.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_hestroke-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_hestroke-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_heupturn-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_heupturn-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_je-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/G_je-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_ardsign-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_ardsign-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_bar.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_bar.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_circumflex.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/H_circumflex.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_a-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_a-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_breve.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_breve.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_dotaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_dotaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_i-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_i-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_ishort-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_ishort-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_ogonek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_ogonek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_u-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/I_u-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/J_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/J_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/J_circumflex.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/J_circumflex.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_.ss00.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_.ss00.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_adescender-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_adescender-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_adescender-cy.ss00.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_adescender-cy.ss00.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_aiS_ymbol.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_aiS_ymbol.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_aiS_ymbol.ss00.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_aiS_ymbol.ss00.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_je-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_je-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_je-cy.ss00.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/K_je-cy.ss00.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_ambda.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_ambda.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_dot.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_dot.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_je-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_je-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_slash.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/L_slash.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/M_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/M_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_commaaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_commaaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_doubleS_truck.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_doubleS_truck.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_je-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/N_je-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_E_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_E_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_barred-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_barred-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_breve.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_breve.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexacute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexacute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexdotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexdotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexgrave.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexgrave.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexhookabove.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflexhookabove.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflextilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_circumflextilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horn.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horn.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hornacute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hornacute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horngrave.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horngrave.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horntilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_horntilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hungarumlaut.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_hungarumlaut.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_macron.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_macron.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_mega.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_mega.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_megatonos.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_megatonos.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_ogonek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_ogonek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_slash.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_slash.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_slashacute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/O_slashacute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_e-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_e-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_si.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/P_si.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Q_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Q_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Q_doubleS_truck.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Q_doubleS_truck.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_commaaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/R_commaaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_cedilla.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_cedilla.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_chwa-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_chwa-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_chwa.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_chwa.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_circumflex.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_circumflex.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_commaaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_commaaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_doubleS_truck.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_doubleS_truck.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_ha-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_ha-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_hcha-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_hcha-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_igma.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_igma.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_oftsign-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/S_oftsign-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_bar.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_bar.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_cedilla.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_cedilla.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_commaaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_commaaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_heta.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_heta.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_horn.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_horn.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_se-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_se-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_she-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/T_she-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_breve.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_breve.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horn.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horn.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hornacute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hornacute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horngrave.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horngrave.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horntilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_horntilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hungarumlaut.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_hungarumlaut.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_macron.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_macron.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_ogonek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_ogonek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_short-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_short-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_straightstroke-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/U_straightstroke-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/V_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/V_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/W_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/X_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/X_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/X_i.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/X_i.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_eru-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_eru-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_i-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_i-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_tilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Y_tilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_dotaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_dotaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_doubleS_truck.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_doubleS_truck.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_e-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_e-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_he-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_he-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_he-cy.ss00.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/Z_he-cy.ss00.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/_notdef.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/_notdef.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/_similiar_tilda.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/_similiar_tilda.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/a.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/a.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abrevedotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/abrevedotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexdotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexdotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexhookabove.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acircumflexhookabove.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acutecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acutecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acutecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/acutecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ae.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ae.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/alphatonos.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/alphatonos.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_ampersand.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_ampersand.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_ampersand_ampersand.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_ampersand_ampersand.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ampersand_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/aogonek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/aogonek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/apostrophemod.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/apostrophemod.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/approxequal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/approxequal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciicircum.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciicircum.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciicircum_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciicircum_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_asciitilde.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_asciitilde.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_asciitilde_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_asciitilde_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_at.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_at.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asciitilde_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_asterisk_asterisk.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_asterisk_asterisk.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_slash.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asterisk_slash.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asteriskoperator.circled.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asteriskoperator.circled.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asymptoticallyequal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/asymptoticallyequal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/at.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/at.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/at_underscore.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/at_underscore.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/b.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/b.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/backslash.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/backslash.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ballotX_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ballotX_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_bar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_bar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_bar_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_bar_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bar_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_braceright.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_braceright.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bracketright.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_bracketright.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_equal_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_equal_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_hyphen_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bar_hyphen_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/be-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/be-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bell-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bell-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/beta.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/beta.glyph`

 * *Files 11% similar despite different names*

```diff
@@ -55,77 +55,65 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (20, 46);
-place = (20, 46);
+place = (20,46);
 type = Stem;
 },
 {
-place = (393, 51);
-place = (393, 51);
+place = (393,51);
 type = Stem;
 },
 {
-place = (380, 51);
-place = (380, 51);
+place = (380,51);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-54, 36);
-place = (-54, 36);
+place = (-54,36);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (281, 38);
-place = (281, 38);
+place = (281,38);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (606, 36);
-place = (606, 36);
+place = (606,36);
 type = Stem;
 },
 {
-place = (20, 46);
-place = (20, 46);
+place = (20,46);
 type = Stem;
 },
 {
-place = (393, 51);
-place = (393, 51);
+place = (393,51);
 type = Stem;
 },
 {
-place = (380, 51);
-place = (380, 51);
+place = (380,51);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-54, 36);
-place = (-54, 36);
+place = (-54,36);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (281, 38);
-place = (281, 38);
+place = (281,38);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (606, 36);
-place = (606, 36);
+place = (606,36);
 type = Stem;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
 closed = 1;
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bitcoin.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bitcoin.glyph`

 * *Files 8% similar despite different names*

```diff
@@ -68,44 +68,38 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (46, 45);
-place = (46, 45);
+place = (46,45);
 type = Stem;
 },
 {
-place = (380, 51);
-place = (380, 51);
+place = (380,51);
 type = Stem;
 },
 {
-place = (393, 51);
-place = (393, 51);
+place = (393,51);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-44, 38);
-place = (-44, 38);
+place = (-44,38);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (286, 34);
-place = (286, 34);
+place = (286,34);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (594, 38);
-place = (594, 38);
+place = (594,38);
 type = Stem;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
 closed = 1;
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackC_ircle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackC_ircle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackD_iamond.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackD_iamond.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackS_mallS_quare.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackS_mallS_quare.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackS_quare.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/blackS_quare.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleD_ownA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleU_pA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_ertical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_ertical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_oubleV_erticalA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndH_orizontalS_ingle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndH_orizontalS_ingle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndL_eftS_ingle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndL_eftS_ingle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndR_ightS_ingle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownD_oubleA_ndR_ightS_ingle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndH_orizontalL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndH_orizontalL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndL_eftL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndL_eftL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndL_eftU_pL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndL_eftU_pL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndR_ightL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndR_ightL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndR_ightU_pL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndR_ightU_pL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndU_pH_orizontalL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownH_eavyA_ndU_pH_orizontalL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndH_orizontalH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndH_orizontalH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndL_eftH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndL_eftH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndL_eftU_pH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndL_eftU_pH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndR_ightH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndR_ightH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndR_ightU_pH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndR_ightU_pH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndU_pH_orizontalH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownL_ightA_ndU_pH_orizontalH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndH_orizontalD_ouble.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndH_orizontalD_ouble.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndL_eftD_ouble.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndL_eftD_ouble.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndR_ightD_ouble.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxD_ownS_ingleA_ndR_ightD_ouble.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_oubleD_ashH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_oubleD_ashH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_oubleD_ashV_ertical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_oubleD_ashV_ertical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_own.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_own.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyD_ownA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyL_eftA_ndL_ightR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyL_eftA_ndL_ightR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyQ_uadrupleD_ashH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyQ_uadrupleD_ashH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyQ_uadrupleD_ashV_ertical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyQ_uadrupleD_ashV_ertical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyT_ripleD_ashH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyT_ripleD_ashH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyT_ripleD_ashV_ertical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyT_ripleD_ashV_ertical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_p.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_p.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndL_ightD_own.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndL_ightD_own.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyU_pA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_ertical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_ertical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxH_eavyV_erticalA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftD_ownH_eavyA_ndR_ightU_pL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftD_ownH_eavyA_ndR_ightU_pL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightD_ownL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightD_ownL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightU_pL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightU_pL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightV_erticalL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftH_eavyA_ndR_ightV_erticalL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightD_ownH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightD_ownH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightU_pH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightU_pH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightV_erticalH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftL_ightA_ndR_ightV_erticalH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftU_pH_eavyA_ndR_ightD_ownL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_eftU_pH_eavyA_ndR_ightD_ownL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcD_ownA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcD_ownA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcD_ownA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcD_ownA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcU_pA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcU_pA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcU_pA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightA_rcU_pA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalC_ross.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalC_ross.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalU_pperL_eftT_oL_owerR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalU_pperL_eftT_oL_owerR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalU_pperR_ightT_oL_owerL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_iagonalU_pperR_ightT_oL_owerL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_oubleD_ashH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_oubleD_ashH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_oubleD_ashV_ertical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_oubleD_ashV_ertical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_own.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_own.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightD_ownA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightL_eftA_ndH_eavyR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightL_eftA_ndH_eavyR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightQ_uadrupleD_ashH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightQ_uadrupleD_ashH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightQ_uadrupleD_ashV_ertical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightQ_uadrupleD_ashV_ertical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightT_ripleD_ashH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightT_ripleD_ashH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightT_ripleD_ashV_ertical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightT_ripleD_ashV_ertical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_p.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_p.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndH_eavyD_own.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndH_eavyD_own.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightU_pA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_ertical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_ertical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndH_orizontal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndH_orizontal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndL_eft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndL_eft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndR_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxL_ightV_erticalA_ndR_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightD_ownH_eavyA_ndL_eftU_pL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightD_ownH_eavyA_ndL_eftU_pL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftD_ownL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftD_ownL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftU_pL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftU_pL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftV_erticalL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightH_eavyA_ndL_eftV_erticalL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftD_ownH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftD_ownH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftU_pH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftU_pH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftV_erticalH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightL_ightA_ndL_eftV_erticalH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightU_pH_eavyA_ndL_eftD_ownL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxR_ightU_pH_eavyA_ndL_eftD_ownL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndH_orizontalS_ingle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndH_orizontalS_ingle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndL_eftS_ingle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndL_eftS_ingle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndR_ightS_ingle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pD_oubleA_ndR_ightS_ingle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndD_ownH_orizontalL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndD_ownH_orizontalL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndH_orizontalL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndH_orizontalL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndL_eftD_ownL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndL_eftD_ownL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndL_eftL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndL_eftL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndR_ightD_ownL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndR_ightD_ownL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndR_ightL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pH_eavyA_ndR_ightL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndD_ownH_orizontalH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndD_ownH_orizontalH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndH_orizontalH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndH_orizontalH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndL_eftD_ownH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndL_eftD_ownH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndL_eftH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndL_eftH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndR_ightD_ownH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndR_ightD_ownH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndR_ightH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pL_ightA_ndR_ightH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndH_orizontalD_ouble.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndH_orizontalD_ouble.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndL_eftD_ouble.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndL_eftD_ouble.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndR_ightD_ouble.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxU_pS_ingleA_ndR_ightD_ouble.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndH_orizontalS_ingle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndH_orizontalS_ingle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndL_eftS_ingle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndL_eftS_ingle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndR_ightS_ingle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalD_oubleA_ndR_ightS_ingle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndH_orizontalL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndH_orizontalL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndL_eftL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndL_eftL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndR_ightL_ight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalH_eavyA_ndR_ightL_ight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndH_orizontalH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndH_orizontalH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndL_eftH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndL_eftH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndR_ightH_eavy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalL_ightA_ndR_ightH_eavy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndH_orizontalD_ouble.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndH_orizontalD_ouble.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndL_eftD_ouble.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndL_eftD_ouble.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndR_ightD_ouble.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/boxV_erticalS_ingleA_ndR_ightD_ouble.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceleft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceleft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceleft_bar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceleft_bar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceright.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/braceright.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_bar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_bar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_bar_bar_bracketright.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_bar_bar_bracketright.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_less.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleft_less.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleftwithquill.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketleftwithquill.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketright.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketright.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketright_numbersign.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketright_numbersign.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketrightwithquill.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bracketrightwithquill.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevebelowcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevebelowcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_acutecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_acutecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_acutecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_acutecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_gravecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_gravecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_gravecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_gravecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_hookabovecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_hookabovecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_hookabovecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_hookabovecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_tildecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_tildecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_tildecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brevecomb_tildecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/breveinvertedcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/breveinvertedcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brokenbar.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/brokenbar.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bullet.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bullet.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bullseye.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/bullseye.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/c.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/c.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cancel-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cancel-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.alt.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.alt.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/caroncomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/carriageR_eturn-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/carriageR_eturn-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ccedilla.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ccedilla.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ccircumflex.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ccircumflex.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cdotaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cdotaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cedillacomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cedillacomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cedillacomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cedillacomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/cent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/che-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/che-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/checkmark.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/checkmark.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/chedescender-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/chedescender-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/chi.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/chi.glyph`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 );
 width = 600;
 },
 {
 hints = (
 {
 horizontal = 1;
-place = (550.803, -20);
+place = (550.803,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (-165, 21);
+place = (-165,21);
 target = up;
 type = BottomGhost;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_acutecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_acutecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_acutecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_acutecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_gravecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_gravecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_gravecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_gravecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_hookabovecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_hookabovecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_hookabovecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_hookabovecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_tildecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_tildecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_tildecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/circumflexcomb_tildecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon_colon.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon_colon.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_colon_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_less.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_less.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_question.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_question.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_question_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colon_question_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colonequals.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/colonequals.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/comma.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/comma.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.alt.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.alt.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaaccentcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaturnedabovecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaturnedabovecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaturnedabovecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/commaturnedabovecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/complement.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/complement.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/congruent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/congruent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/coproduct.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/coproduct.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/copyright.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/copyright.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/curlybracketextension.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/curlybracketextension.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/curlyor.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/curlyor.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/currency.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/currency.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/d.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/d.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dagger.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dagger.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/daggerdbl.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/daggerdbl.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dataL_inkE_scape-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dataL_inkE_scape-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dblgravecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dblgravecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dblgravecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dblgravecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dcaron.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dcaron.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dcroat.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dcroat.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/de-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/de-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/degree.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/degree.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/delete-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/delete-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/delta.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/delta.glyph`

 * *Files 7% similar despite different names*

```diff
@@ -55,101 +55,93 @@
 );
 width = 600;
 },
 {
 hints = (
 {
 horizontal = 1;
-place = (727, -20);
+place = (727,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (652, 21);
+place = (652,21);
 target = up;
 type = BottomGhost;
 },
 {
 horizontal = 1;
-place = (727, -20);
+place = (727,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (652, 21);
+place = (652,21);
 target = up;
 type = BottomGhost;
 },
 {
-place = (27, 47);
-place = (27, 47);
+place = (27,47);
 type = Stem;
 },
 {
-place = (397, 47);
-place = (397, 47);
+place = (397,47);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-53, 37);
-place = (-53, 37);
+place = (-53,37);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (317, 33);
-place = (317, 33);
+place = (317,33);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (717, -20);
+place = (717,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (642, 21);
+place = (642,21);
 target = up;
 type = BottomGhost;
 },
 {
-place = (27, 47);
-place = (27, 47);
+place = (27,47);
 type = Stem;
 },
 {
-place = (397, 47);
-place = (397, 47);
+place = (397,47);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-53, 37);
-place = (-53, 37);
+place = (-53,37);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (317, 33);
-place = (317, 33);
+place = (317,33);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (727, -20);
+place = (727,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (652, 21);
+place = (652,21);
 target = up;
 type = BottomGhost;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolF_our-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolF_our-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolO_ne-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolO_ne-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolT_hree-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolT_hree-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolT_wo-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/deviceC_ontrolT_wo-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresisbelowcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresisbelowcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresiscomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresiscomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresiscomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresiscomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresistonos.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dieresistonos.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/divide.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/divide.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/divides.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/divides.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dje-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dje-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dollar.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dollar.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dollar_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dollar_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dong.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dong.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccentcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccentcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccentcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotaccentcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotbelowcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotbelowcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotbelowcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotbelowcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotminus.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dotminus.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dottedC_ircle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dottedC_ircle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/doubleprimemod.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/doubleprimemod.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/doublesubset.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/doublesubset.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downA_rrowH_ead.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downA_rrowH_ead.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downD_oubleA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downD_oubleA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downW_hiteS_mallT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downW_hiteS_mallT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downW_hiteT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downW_hiteT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downrightdiagonalellipsis.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/downrightdiagonalellipsis.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dzhe-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/dzhe-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/e-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/e-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/e.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/e.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexdotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexdotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexhookabove.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ecircumflexhookabove.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ef-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ef-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eightsuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eightsuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/el-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/el-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/element.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/element.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ellipsis.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ellipsis.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ellipsisvertical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ellipsisvertical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/em-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/em-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/emdash.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/emdash.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/emptyset.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/emptyset.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/en-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/en-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fM_edium-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fM_edium-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ext-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ext-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ransmission-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ransmission-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ransmissionB_lock-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endO_fT_ransmissionB_lock-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endash.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endash.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endescender-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endescender-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endofproof.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/endofproof.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eng.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eng.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/enquiry-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/enquiry-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eogonek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eogonek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/epsilon.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/epsilon.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/epsilontonos.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/epsilontonos.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_colon.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_colon.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_colon_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_colon_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_equal.liga.old.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_equal.liga.old.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_equal_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_exclam_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_exclam_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_greater_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_greater_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_less_less.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_less_less.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_slash_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equal_slash_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equivalence.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/equivalence.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ereversed-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ereversed-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/escape-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/escape-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/estimated.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/estimated.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eta.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eta.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/etatonos.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/etatonos.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eth.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/eth.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/euro.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/euro.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/excess.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/excess.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal_equal.liga.old.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_equal_equal.liga.old.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_exclam.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclam_exclam.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclamdown.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/exclamdown.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/existential.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/existential.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/f.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/f.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fileS_eparator-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fileS_eparator-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/five.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/five.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fivesuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fivesuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/flat-musical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/flat-musical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/florin.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/florin.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/formF_eed-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/formF_eed-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/four-gujarati.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/four-gujarati.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/four.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/four.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/foursuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/foursuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fraction.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fraction.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fullB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/fullB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/g.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/g.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gamma.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gamma.glyph`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 {
 glyphname = gamma;
 layers = (
 {
 hints = (
 {
 horizontal = 1;
-place = (-43, 21);
+place = (-43,21);
 target = up;
 type = BottomGhost;
 },
 {
 horizontal = 1;
-place = (507, -20);
+place = (507,-20);
 target = down;
 type = TopGhost;
 }
 );
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
@@ -40,27 +40,26 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (212, 47);
-place = (212, 47);
+place = (212,47);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (677, -20);
+place = (677,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (-43, 21);
+place = (-43,21);
 target = up;
 type = BottomGhost;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gcircumflex.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gcircumflex.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gdotaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gdotaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ge-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ge-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/germandbls.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/germandbls.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ghestroke-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ghestroke-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gheupturn-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gheupturn-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gje-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gje-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gravecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gravecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gravecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/gravecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_bracketright.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_bracketright.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_colon.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_colon.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_equal_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_equal_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_greater_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_hyphen_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greater_hyphen_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greaterequal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greaterequal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greaterorequivalent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/greaterorequivalent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/groupS_eparator-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/groupS_eparator-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guillemetleft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guillemetleft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guillemetright.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guillemetright.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guilsinglleft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guilsinglleft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guilsinglright.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/guilsinglright.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/h.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/h.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hardsign-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hardsign-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hcircumflex.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hcircumflex.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyC_ircle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyC_ircle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyleftpointinganglebracketornament.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyleftpointinganglebracketornament.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyleftpointinganglequotationmarkornament.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyleftpointinganglequotationmarkornament.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyrightpointinganglebracketornament.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyrightpointinganglebracketornament.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyrightpointinganglequotationmarkornament.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/heavyrightpointinganglequotationmarkornament.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/highV_oltageS_ign.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/highV_oltageS_ign.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hookabovecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hookabovecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hookabovecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hookabovecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horizontalT_abulation-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horizontalT_abulation-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horncomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horncomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horncomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/horncomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/house.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/house.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlautcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlautcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlautcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hungarumlautcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_asciitilde.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_asciitilde.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_bar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_bar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_greater_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_greater_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_hyphen_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_less.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_less.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_less_less.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/hyphen_less_less.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ia-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ia-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ibreve.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ibreve.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idotless.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/idotless.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ii-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ii-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iishort-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iishort-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/infinity.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/infinity.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/integral.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/integral.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iogonek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iogonek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iota.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iota.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iotadieresistonos.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iotadieresistonos.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/itilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/itilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iu-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/iu-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/jcircumflex.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/jcircumflex.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/jdotless.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/jdotless.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/k.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/k.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/k.ss00.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/k.ss00.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ka-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ka-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ka-cy.ss00.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ka-cy.ss00.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kadescender-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kadescender-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kadescender-cy.ss00.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kadescender-cy.ss00.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kaiS_ymbol.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kaiS_ymbol.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kje-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kje-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kje-cy.ss00.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/kje-cy.ss00.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/l.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/l.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/l.ss01.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/l.ss01.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lambda.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lambda.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lambdastroke.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lambdastroke.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/largeC_ircle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/largeC_ircle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ldot.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ldot.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lackS_mallT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lackS_mallT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftC_eiling.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftC_eiling.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftF_iveE_ighthsB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftF_iveE_ighthsB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftF_loor.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftF_loor.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftL_ongA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftL_ongA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftO_neE_ighthB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftO_neE_ighthB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftO_neQ_uarterB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftO_neQ_uarterB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightD_oubleA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightD_oubleA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightL_ongA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightL_ongA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightW_aveA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftR_ightW_aveA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftS_evenE_ighthsB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftS_evenE_ighthsB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftT_hreeE_ighthsB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftT_hreeE_ighthsB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftT_hreeQ_uartersB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftT_hreeQ_uartersB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftW_hiteS_mallT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftW_hiteS_mallT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftW_hiteT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftW_hiteT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftanglebracket-math.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftanglebracket-math.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketlowerhook.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketlowerhook.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketmiddlepiece.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketmiddlepiece.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketupperhook.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftcurlybracketupperhook.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftdoubleanglebracket-math.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftdoubleanglebracket-math.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketextension.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketextension.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketlowercorner.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketlowercorner.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketuppercorner.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftsquarebracketuppercorner.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftwhitesquarebracket-math.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/leftwhitesquarebracket-math.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde_asciitilde.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde_asciitilde.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asciitilde_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asterisk.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asterisk.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asterisk_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_asterisk_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_bar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_bar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_bar_bar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_bar_bar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_bar_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_colon.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_colon.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_dollar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_dollar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_dollar_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_dollar_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_bar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_bar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_equal_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_equal_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_less.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_equal_less.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_exclam_hyphen_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_exclam_hyphen_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_bar.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_bar.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_less.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_hyphen_less.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_asciitilde.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_asciitilde.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_less.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_less_less.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_numbersign_hyphen_hyphen.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_numbersign_hyphen_hyphen.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_plus.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_plus.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_plus_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_plus_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_slash.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_slash.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_slash_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/less_slash_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lessequal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lessequal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lessorequivalent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lessorequivalent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lineF_eed-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lineF_eed-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/literS_ign.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/literS_ign.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lje-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lje-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicaland.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicaland.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicalnot.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicalnot.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicalor.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/logicalor.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/longs.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/longs.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerF_iveE_ighthsB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerF_iveE_ighthsB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerH_alfB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerH_alfB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerL_eftB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerL_eftB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerO_neE_ighthB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerO_neE_ighthB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerO_neQ_uarterB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerO_neQ_uarterB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerR_ightB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerR_ightB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerR_ightD_iagonalH_alfB_lackS_quare.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerR_ightD_iagonalH_alfB_lackS_quare.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerS_evenE_ighthsB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerS_evenE_ighthsB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerT_hreeE_ighthsB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerT_hreeE_ighthsB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerT_hreeQ_uartersB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowerT_hreeQ_uartersB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowtildemod.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lowtildemod.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lozenge.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lozenge.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lslash.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lslash.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lslash.ss01.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/lslash.ss01.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/m.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/m.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macronbelowcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macronbelowcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macroncomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macroncomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macroncomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/macroncomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/midlinehorizontalellipsis.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/midlinehorizontalellipsis.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/minus.circled.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/minus.circled.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/minute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/minute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/mu.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/mu.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multimap.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multimap.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiplicationX_.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiplicationX_.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiply.circled.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiply.circled.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiply.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multiply.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multisetunion.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/multisetunion.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/n.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/n.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nA_ryC_ircledD_otO_perator.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nA_ryC_ircledD_otO_perator.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nA_ryS_quareU_nionO_perator.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nA_ryS_quareU_nionO_perator.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/napostrophe.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/napostrophe.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/negativeA_cknowledge-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/negativeA_cknowledge-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/neitherapproximatelynoractuallyequalto.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/neitherapproximatelynoractuallyequalto.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/neitherasubsetofnorequalto.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/neitherasubsetofnorequalto.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/newline-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/newline-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nine.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nine.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ninesuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ninesuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nje-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/nje-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/northE_astA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/northE_astA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/northW_estA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/northW_estA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notalmostequalto.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notalmostequalto.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notcontains.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notcontains.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notelement.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notelement.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notequal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notequal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notgreater.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notgreater.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notgreaternorequal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notgreaternorequal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notidentical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notidentical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notless.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notless.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notlessnorequal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notlessnorequal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notsubset.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notsubset.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notsuperset.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/notsuperset.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/null-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/null-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_braceleft.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_braceleft.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_bracketleft.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_bracketleft.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_colon.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_colon.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_exclam.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_exclam.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign_numbersign.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign_numbersign.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign_numbersign_numbersign.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_numbersign_numbersign_numbersign.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_parenleft.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_parenleft.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_question.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_question.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_underscore.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_underscore.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_underscore_parenleft.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numbersign_underscore_parenleft.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numeral-greek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numeral-greek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numero.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/numero.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/o.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/o.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/obarred-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/obarred-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexdotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexdotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexhookabove.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ocircumflexhookabove.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oe.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oe.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ogonekcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ogonekcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ogonekcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ogonekcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohookabove.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohookabove.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorn.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorn.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohornacute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohornacute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorngrave.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorngrave.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorntilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ohorntilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omega.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omega.glyph`

 * *Files 20% similar despite different names*

```diff
@@ -57,79 +57,67 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (-24, -43);
-place = (-24, -43);
+place = (-24,-43);
 type = Stem;
 },
 {
-place = (-24, -43);
-place = (-24, -43);
+place = (-24,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (464, -43);
-place = (464, -43);
+place = (464,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (464, -43);
-place = (464, -43);
+place = (464,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (464, -43);
-place = (464, -43);
+place = (464,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (464, -43);
-place = (464, -43);
+place = (464,-43);
 type = Stem;
 },
 {
-place = (-28, -43);
-place = (-28, -43);
+place = (-28,-43);
 type = Stem;
 },
 {
-place = (-28, -43);
-place = (-28, -43);
+place = (-28,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (454, -43);
-place = (454, -43);
+place = (454,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (454, -43);
-place = (454, -43);
+place = (454,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (454, -43);
-place = (454, -43);
+place = (454,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (454, -43);
-place = (454, -43);
+place = (454,-43);
 type = Stem;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
 closed = 1;
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omegatonos.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/omegatonos.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/one.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/one.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onehalf.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onehalf.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onequarter.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onequarter.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onesuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/onesuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oogonek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oogonek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/operator.circled.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/operator.circled.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/optionK_ey.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/optionK_ey.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ordfeminine.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ordfeminine.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ordmasculine.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ordmasculine.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oslash.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oslash.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oslashacute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/oslashacute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/overline.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/overline.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/p.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/p.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/paragraph.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/paragraph.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parallel.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parallel.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftextension.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftextension.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftlowerhook.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftlowerhook.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftupperhook.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenleftupperhook.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenright.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/parenright.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/partialdiff.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/partialdiff.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/pe-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/pe-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/percent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/percent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period_less.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period_less.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period_period.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_period_period.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_question.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/period_question.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/perthousand.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/perthousand.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/phi.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/phi.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/pi.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/pi.glyph`

 * *Files 17% similar despite different names*

```diff
@@ -31,38 +31,33 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (57, 47);
-place = (57, 47);
+place = (57,47);
 type = Stem;
 },
 {
-place = (342, 47);
-place = (342, 47);
+place = (342,47);
 type = Stem;
 },
 {
-place = (342, 147);
-place = (342, 147);
+place = (342,147);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-48, 41);
-place = (-48, 41);
+place = (-48,41);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (425, 39);
-place = (425, 39);
+place = (425,39);
 type = Stem;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
 closed = 1;
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/piS_ymbol.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/piS_ymbol.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus.circled.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus.circled.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_plus.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_plus.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_plus_plus.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plus_plus_plus.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plusminus.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plusminus.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plussuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/plussuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerO_nO_ffS_ymbol.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerO_nO_ffS_ymbol.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerO_nS_ymbol.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerO_nS_ymbol.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerS_leepS_ymbol.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerS_leepS_ymbol.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerS_ymbol.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/powerS_ymbol.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/precedes.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/precedes.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/precedesorequalto.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/precedesorequalto.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/primemod.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/primemod.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/product.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/product.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/projective.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/projective.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/propellor.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/propellor.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/proportion.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/proportion.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/psi.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/psi.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/q.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/q.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_colon.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_colon.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_period.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_period.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_question.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/question_question.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/questiondown.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/questiondown.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/questionedequalto.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/questionedequalto.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedbl.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedbl.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblbase.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblbase.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblleft.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblleft.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblright.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotedblright.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotesingle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/quotesingle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/r.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/r.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/r.ss03.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/r.ss03.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/radical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/radical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ratio.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ratio.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/recordS_eparator-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/recordS_eparator-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/reflexsubset.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/reflexsubset.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/reflexsuperset.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/reflexsuperset.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/registered.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/registered.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/replacement.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/replacement.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rho.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rho.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lackS_mallT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lackS_mallT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightC_eiling.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightC_eiling.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightD_oubleA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightD_oubleA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightD_oubleP_airedA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightD_oubleP_airedA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightF_loor.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightF_loor.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightF_rombarA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightF_rombarA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightH_alfB_lackS_quare.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightH_alfB_lackS_quare.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightH_eavyR_oundT_ippedA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightH_eavyR_oundT_ippedA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightO_neE_ighthB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightO_neE_ighthB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_ailA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_ailA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_woH_eadedA_rrowW_ithT_ail.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_woH_eadedA_rrowW_ithT_ail.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_woheadedA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightT_woheadedA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteP_ointer.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteP_ointer.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteS_mallT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteS_mallT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightW_hiteT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightanglebracket-math.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightanglebracket-math.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketlowerhook.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketlowerhook.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketmiddlepiece.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketmiddlepiece.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketupperhook.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightcurlybracketupperhook.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightdoubleanglebracket-math.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightdoubleanglebracket-math.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightlongA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightlongA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightsquarebracketlowercorner.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightsquarebracketlowercorner.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightsquarebracketuppercorner.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightsquarebracketuppercorner.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/righttack.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/righttack.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightwhitesquarebracket-math.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/rightwhitesquarebracket-math.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringbelowcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringbelowcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringcomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringcomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringequalto.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringequalto.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringoperator.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ringoperator.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ruble.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ruble.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/s.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/s.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scedilla.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scedilla.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/schwa.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/schwa.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scircumflex.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scircumflex.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scommaaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/scommaaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/second.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/second.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/section.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/section.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon_semicolon.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon_semicolon.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon_semicolon_semicolon.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/semicolon_semicolon_semicolon.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/seven.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/seven.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sevensuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sevensuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sha-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sha-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shadedark.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shadedark.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shadelight.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shadelight.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shademedium.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shademedium.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sharp-musical.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sharp-musical.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shcha-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shcha-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shiftI_n-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shiftI_n-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shiftO_ut-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/shiftO_ut-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sigma.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sigma.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sigmafinal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sigmafinal.glyph`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 {
 horizontal = 1;
 origin = (0,0);
 target = (0,0);
 type = Stem;
 },
 {
-place = (407, -43);
-place = (407, -43);
+place = (407,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-223, 21);
+place = (-223,21);
 target = up;
 type = BottomGhost;
 }
 );
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
@@ -62,44 +61,39 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (45, 47);
-place = (45, 47);
+place = (45,47);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-53, 37);
-place = (-53, 37);
+place = (-53,37);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (437, 37);
-place = (437, 37);
+place = (437,37);
 type = Stem;
 },
 {
-place = (142, 42);
-place = (142, 42);
+place = (142,42);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (27, 37);
-place = (27, 37);
+place = (27,37);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-223, -20);
+place = (-223,-20);
 target = down;
 type = TopGhost;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
@@ -153,21 +147,20 @@
 {
 origin = (0,1);
 target = (0,4);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-223, -43);
-place = (-223, -43);
+place = (-223,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-223, 21);
+place = (-223,21);
 target = up;
 type = BottomGhost;
 }
 );
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/six.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/six.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sixP_ointedB_lackS_tar.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sixP_ointedB_lackS_tar.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sixsuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sixsuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_asterisk.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_asterisk.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_asterisk_asterisk.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_asterisk_asterisk.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_equal_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_equal_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_greater.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_greater.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash_equal.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash_equal.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash_slash.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slash_slash_slash.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slashlongcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slashlongcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slashshortcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/slashshortcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/softsign-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/softsign-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/southE_astA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/southE_astA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/southW_estA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/southW_estA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/space-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/space-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/squarecap.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/squarecap.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/squareimageoforequalto.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/squareimageoforequalto.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/staroperator.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/staroperator.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/startO_fH_eading-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/startO_fH_eading-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/startO_fT_ext-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/startO_fT_ext-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sterling.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/sterling.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/strokelongcomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/strokelongcomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/subset.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/subset.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/substitute-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/substitute-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/suchthat.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/suchthat.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/summation.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/summation.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/summationdoubleS_truck.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/summationdoubleS_truck.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/superset.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/superset.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/synchronousI_dle-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/synchronousI_dle-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/t.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/t.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tackdown.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tackdown.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tau.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tau.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tbar.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tbar.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcaron.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcaron.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcedilla.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcedilla.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcommaaccent.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tcommaaccent.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/te-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/te-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/theta.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/theta.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/thorn.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/thorn.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/three.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/three.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threequarters.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threequarters.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threesuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/threesuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tildecomb.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tildecomb.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tildecomb.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tildecomb.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tonos.case.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tonos.case.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tonos.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tonos.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/trademark.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/trademark.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tripleprime.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tripleprime.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tripletilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tripletilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tse-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tse-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tshe-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tshe-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tugrik.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/tugrik.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/two.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/two.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/twosuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/twosuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/u.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/u.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/u.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/u.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ubreve.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ubreve.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ucircumflex.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ucircumflex.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udieresis.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udieresis.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udotbelow.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/udotbelow.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ugrave.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ugrave.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhookabove.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhookabove.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorn.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorn.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorn.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorn.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornacute.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornacute.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornacute.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhornacute.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorndotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorndotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorndotbelow.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorndotbelow.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorngrave.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorngrave.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorngrave.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorngrave.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorntilde.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorntilde.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorntilde.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhorntilde.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhungarumlaut.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uhungarumlaut.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/umacron.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/umacron.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore_bar_underscore.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore_bar_underscore.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore_underscore.liga.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/underscore_underscore.liga.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/undertie.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/undertie.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_0.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_0.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_1.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_1.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_2.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0A_2.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_0.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_0.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_1.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_1.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_2.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_2.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_3.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uniE_0B_3.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/union.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/union.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/unitS_eparator-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/unitS_eparator-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/universal.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/universal.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uogonek.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uogonek.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uogonek.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uogonek.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upB_lackS_mallT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upB_lackS_mallT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upD_oubleA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upD_oubleA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upD_ownA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upD_ownA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upF_rombarA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upF_rombarA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteA_rrow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteA_rrow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteS_mallT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteS_mallT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteT_riangle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upW_hiteT_riangle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperH_alfB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperH_alfB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndL_owerL_eftA_ndL_owerR_ightB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndL_owerL_eftA_ndL_owerR_ightB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndL_owerR_ightB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndL_owerR_ightB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndU_pperR_ightA_ndL_owerL_eftB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndU_pperR_ightA_ndL_owerL_eftB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndU_pperR_ightA_ndL_owerR_ightB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftA_ndU_pperR_ightA_ndL_owerR_ightB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftD_iagonalH_alfB_lackS_quare.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftD_iagonalH_alfB_lackS_quare.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftW_hiteC_ircle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperL_eftW_hiteC_ircle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperO_neE_ighthB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperO_neE_ighthB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightA_ndL_owerL_eftA_ndL_owerR_ightB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightA_ndL_owerL_eftA_ndL_owerR_ightB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightA_ndL_owerL_eftB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightA_ndL_owerL_eftB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightB_lackC_ircle.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightB_lackC_ircle.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightB_lock.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upperR_ightB_lock.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uprightdiagonalellipsis.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/uprightdiagonalellipsis.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upsilondieresistonos.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/upsilondieresistonos.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ustraightstroke-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ustraightstroke-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/utilde.ss04.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/utilde.ss04.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/v.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/v.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ve-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ve-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/verticalB_isectingL_ineW_hiteS_quare.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/verticalB_isectingL_ineW_hiteS_quare.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/verticalT_abulation-control.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/verticalT_abulation-control.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/w.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/w.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/warningS_ign.001.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/warningS_ign.001.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/warningS_ign.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/warningS_ign.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteB_ullet.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteB_ullet.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteD_iamond.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteD_iamond.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteS_mallS_quare.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteS_mallS_quare.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteS_quare.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/whiteS_quare.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/x.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/x.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/xi.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/xi.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/y.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/y.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ydotbelow.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ydotbelow.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yen.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yen.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yeru-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yeru-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yi-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/yi-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/z.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/z.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ze-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/ze-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zero.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zero.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zero.zero.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zero.zero.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zerosuperior.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zerosuperior.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zeta.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zeta.glyph`

 * *Files 11% similar despite different names*

```diff
@@ -81,34 +81,30 @@
 );
 width = 600;
 },
 {
 hints = (
 {
 horizontal = 1;
-place = (-43, 36);
-place = (-43, 36);
+place = (-43,36);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (598, 36);
-place = (598, 36);
+place = (598,36);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-43, 36);
-place = (-43, 36);
+place = (-43,36);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (598, 36);
-place = (598, 36);
+place = (598,36);
 type = Stem;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
 closed = 1;
```

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zhe-cy.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zhe-cy.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zhe-cy.ss00.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/zhe-cy.ss00.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/znotationleftimagebracket.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/znotationleftimagebracket.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/znotationrightimagebracket.glyph` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/glyphs/znotationrightimagebracket.glyph`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic.glyphspackage/order.plist` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic.glyphspackage/order.plist`

 * *Files identical despite different names*

### Comparing `glyphspkg-0.1.9/tests/data/JetBrainsMono-Italic_orig.glyphs` & `glyphspkg-0.2.0/tests/data/JetBrainsMono-Italic_orig.glyphs`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {
-.appVersion = "3124";
+.appVersion = "3306";
 .formatVersion = 3;
 DisplayStrings = (
 "ΐΐΐΐΐΐΰΰΰΰΰΰώώώώώώάάάάάάέέέέέέήήήήήή/periodcentered.loclCAT.case/periodcentered.loclCAT.case/periodcentered.loclCAT.case/periodcentered.loclCAT/periodcentered.loclCAT/periodcentered.loclCAT ↊↊↊/commaaccentcomb.alt/commaaccentcomb.alt/commaaccentcomb.alt"
 );
 axes = (
 {
 name = Weight;
@@ -71,23 +71,23 @@
 },
 {
 pos = 550;
 size = 10;
 },
 {
 pos = 0;
-size = "-10";
+size = -10;
 },
 {
-pos = "-110";
-size = "-10";
+pos = -110;
+size = -10;
 },
 {
-pos = "-180";
-size = "-10";
+pos = -180;
+size = -10;
 }
 );
 },
 {
 name = isFixedPitch;
 value = 1;
 },
@@ -1582,20 +1582,20 @@
 name = "Alignment Zones";
 value = (
 {
 pos = 830;
 size = 10;
 },
 {
-pos = "-110";
-size = "-10";
+pos = -110;
+size = -10;
 },
 {
-pos = "-180";
-size = "-10";
+pos = -180;
+size = -10;
 }
 );
 }
 );
 iconName = Light;
 id = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 metricValues = (
@@ -1694,20 +1694,20 @@
 name = "Alignment Zones";
 value = (
 {
 pos = 830;
 size = 10;
 },
 {
-pos = "-110";
-size = "-10";
+pos = -110;
+size = -10;
 },
 {
-pos = "-180";
-size = "-10";
+pos = -180;
+size = -10;
 }
 );
 }
 );
 id = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 metricValues = (
 {
@@ -1797,20 +1797,20 @@
 name = "Alignment Zones";
 value = (
 {
 pos = 830;
 size = 10;
 },
 {
-pos = "-110";
-size = "-10";
+pos = -110;
+size = -10;
 },
 {
-pos = "-180";
-size = "-10";
+pos = -180;
+size = -10;
 }
 );
 }
 );
 iconName = Bold;
 id = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 metricValues = (
@@ -42836,77 +42836,65 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (20, 46);
-place = (20, 46);
+place = (20,46);
 type = Stem;
 },
 {
-place = (393, 51);
-place = (393, 51);
+place = (393,51);
 type = Stem;
 },
 {
-place = (380, 51);
-place = (380, 51);
+place = (380,51);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-54, 36);
-place = (-54, 36);
+place = (-54,36);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (281, 38);
-place = (281, 38);
+place = (281,38);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (606, 36);
-place = (606, 36);
+place = (606,36);
 type = Stem;
 },
 {
-place = (20, 46);
-place = (20, 46);
+place = (20,46);
 type = Stem;
 },
 {
-place = (393, 51);
-place = (393, 51);
+place = (393,51);
 type = Stem;
 },
 {
-place = (380, 51);
-place = (380, 51);
+place = (380,51);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-54, 36);
-place = (-54, 36);
+place = (-54,36);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (281, 38);
-place = (281, 38);
+place = (281,38);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (606, 36);
-place = (606, 36);
+place = (606,36);
 type = Stem;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
 closed = 1;
@@ -43021,21 +43009,21 @@
 {
 glyphname = gamma;
 layers = (
 {
 hints = (
 {
 horizontal = 1;
-place = (-43, 21);
+place = (-43,21);
 target = up;
 type = BottomGhost;
 },
 {
 horizontal = 1;
-place = (507, -20);
+place = (507,-20);
 target = down;
 type = TopGhost;
 }
 );
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
@@ -43060,27 +43048,26 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (212, 47);
-place = (212, 47);
+place = (212,47);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (677, -20);
+place = (677,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (-43, 21);
+place = (-43,21);
 target = up;
 type = BottomGhost;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
@@ -43192,101 +43179,93 @@
 );
 width = 600;
 },
 {
 hints = (
 {
 horizontal = 1;
-place = (727, -20);
+place = (727,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (652, 21);
+place = (652,21);
 target = up;
 type = BottomGhost;
 },
 {
 horizontal = 1;
-place = (727, -20);
+place = (727,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (652, 21);
+place = (652,21);
 target = up;
 type = BottomGhost;
 },
 {
-place = (27, 47);
-place = (27, 47);
+place = (27,47);
 type = Stem;
 },
 {
-place = (397, 47);
-place = (397, 47);
+place = (397,47);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-53, 37);
-place = (-53, 37);
+place = (-53,37);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (317, 33);
-place = (317, 33);
+place = (317,33);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (717, -20);
+place = (717,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (642, 21);
+place = (642,21);
 target = up;
 type = BottomGhost;
 },
 {
-place = (27, 47);
-place = (27, 47);
+place = (27,47);
 type = Stem;
 },
 {
-place = (397, 47);
-place = (397, 47);
+place = (397,47);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-53, 37);
-place = (-53, 37);
+place = (-53,37);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (317, 33);
-place = (317, 33);
+place = (317,33);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (727, -20);
+place = (727,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (652, 21);
+place = (652,21);
 target = up;
 type = BottomGhost;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
@@ -43657,34 +43636,30 @@
 );
 width = 600;
 },
 {
 hints = (
 {
 horizontal = 1;
-place = (-43, 36);
-place = (-43, 36);
+place = (-43,36);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (598, 36);
-place = (598, 36);
+place = (598,36);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-43, 36);
-place = (-43, 36);
+place = (-43,36);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (598, 36);
-place = (598, 36);
+place = (598,36);
 type = Stem;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
 closed = 1;
@@ -44593,38 +44568,33 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (57, 47);
-place = (57, 47);
+place = (57,47);
 type = Stem;
 },
 {
-place = (342, 47);
-place = (342, 47);
+place = (342,47);
 type = Stem;
 },
 {
-place = (342, 147);
-place = (342, 147);
+place = (342,147);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-48, 41);
-place = (-48, 41);
+place = (-48,41);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (425, 39);
-place = (425, 39);
+place = (425,39);
 type = Stem;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
 closed = 1;
@@ -44849,21 +44819,20 @@
 {
 horizontal = 1;
 origin = (0,0);
 target = (0,0);
 type = Stem;
 },
 {
-place = (407, -43);
-place = (407, -43);
+place = (407,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-223, 21);
+place = (-223,21);
 target = up;
 type = BottomGhost;
 }
 );
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
@@ -44905,44 +44874,39 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (45, 47);
-place = (45, 47);
+place = (45,47);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-53, 37);
-place = (-53, 37);
+place = (-53,37);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (437, 37);
-place = (437, 37);
+place = (437,37);
 type = Stem;
 },
 {
-place = (142, 42);
-place = (142, 42);
+place = (142,42);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (27, 37);
-place = (27, 37);
+place = (27,37);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-223, -20);
+place = (-223,-20);
 target = down;
 type = TopGhost;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
@@ -44996,21 +44960,20 @@
 {
 origin = (0,1);
 target = (0,4);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-223, -43);
-place = (-223, -43);
+place = (-223,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-223, 21);
+place = (-223,21);
 target = up;
 type = BottomGhost;
 }
 );
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
@@ -45487,21 +45450,21 @@
 );
 width = 600;
 },
 {
 hints = (
 {
 horizontal = 1;
-place = (550.803, -20);
+place = (550.803,-20);
 target = down;
 type = TopGhost;
 },
 {
 horizontal = 1;
-place = (-165, 21);
+place = (-165,21);
 target = up;
 type = BottomGhost;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
@@ -45696,79 +45659,67 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (-24, -43);
-place = (-24, -43);
+place = (-24,-43);
 type = Stem;
 },
 {
-place = (-24, -43);
-place = (-24, -43);
+place = (-24,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (464, -43);
-place = (464, -43);
+place = (464,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (464, -43);
-place = (464, -43);
+place = (464,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (464, -43);
-place = (464, -43);
+place = (464,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (464, -43);
-place = (464, -43);
+place = (464,-43);
 type = Stem;
 },
 {
-place = (-28, -43);
-place = (-28, -43);
+place = (-28,-43);
 type = Stem;
 },
 {
-place = (-28, -43);
-place = (-28, -43);
+place = (-28,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (454, -43);
-place = (454, -43);
+place = (454,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (454, -43);
-place = (454, -43);
+place = (454,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (454, -43);
-place = (454, -43);
+place = (454,-43);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (454, -43);
-place = (454, -43);
+place = (454,-43);
 type = Stem;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
 closed = 1;
@@ -63570,44 +63521,38 @@
 }
 );
 width = 600;
 },
 {
 hints = (
 {
-place = (46, 45);
-place = (46, 45);
+place = (46,45);
 type = Stem;
 },
 {
-place = (380, 51);
-place = (380, 51);
+place = (380,51);
 type = Stem;
 },
 {
-place = (393, 51);
-place = (393, 51);
+place = (393,51);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (-44, 38);
-place = (-44, 38);
+place = (-44,38);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (286, 34);
-place = (286, 34);
+place = (286,34);
 type = Stem;
 },
 {
 horizontal = 1;
-place = (594, 38);
-place = (594, 38);
+place = (594,38);
 type = Stem;
 }
 );
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
 closed = 1;
@@ -124874,34 +124819,37 @@
 {
 glyphname = dieresis.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = dieresiscomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = dieresiscomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = dieresiscomb.case;
 }
 );
 width = 600;
 }
 );
@@ -124909,34 +124857,37 @@
 {
 glyphname = dotaccent.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = dotaccentcomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = dotaccentcomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = dotaccentcomb.case;
 }
 );
 width = 600;
 }
 );
@@ -124944,34 +124895,37 @@
 {
 glyphname = grave.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = gravecomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = gravecomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = gravecomb.case;
 }
 );
 width = 600;
 }
 );
@@ -124979,34 +124933,37 @@
 {
 glyphname = acute.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = acutecomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = acutecomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = acutecomb.case;
 }
 );
 width = 600;
 }
 );
@@ -125014,34 +124971,37 @@
 {
 glyphname = hungarumlaut.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = hungarumlautcomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = hungarumlautcomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = hungarumlautcomb.case;
 }
 );
 width = 600;
 }
 );
@@ -125049,34 +125009,37 @@
 {
 glyphname = circumflex.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = circumflexcomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = circumflexcomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = circumflexcomb.case;
 }
 );
 width = 600;
 }
 );
@@ -125084,34 +125047,37 @@
 {
 glyphname = caron.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = caroncomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = caroncomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = caroncomb.case;
 }
 );
 width = 600;
 }
 );
@@ -125119,34 +125085,37 @@
 {
 glyphname = breve.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = brevecomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = brevecomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = brevecomb.case;
 }
 );
 width = 600;
 }
 );
@@ -125154,34 +125123,37 @@
 {
 glyphname = ring.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = ringcomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = ringcomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = ringcomb.case;
 }
 );
 width = 600;
 }
 );
@@ -125189,34 +125161,37 @@
 {
 glyphname = tilde.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = tildecomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = tildecomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = tildecomb.case;
 }
 );
 visible = 1;
 width = 600;
 }
@@ -125225,34 +125200,37 @@
 {
 glyphname = macron.case;
 layers = (
 {
 layerId = "9ADF6715-3D0F-493D-8567-18A6FBCFC567";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = macroncomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = macroncomb.case;
 }
 );
 width = 600;
 },
 {
 layerId = "EDF5EB54-295C-4C90-9A2F-67CD82979CFF";
 shapes = (
 {
+alignment = -1;
 pos = (600,0);
 ref = macroncomb.case;
 }
 );
 width = 600;
 }
 );
@@ -129217,17 +129195,14 @@
 {
 customParameters = (
 {
 name = "Variable Font Origin";
 value = "CCC0BD40-BA8C-414E-B576-CF0B94E6C996";
 }
 );
-instanceInterpolations = {
-"EDF5EB54-295C-4C90-9A2F-67CD82979CFF" = 1;
-};
 name = Regular;
 type = variable;
 }
 );
 metrics = (
 {
 type = ascender;
@@ -129268,38 +129243,38 @@
 );
 },
 {
 key = designerURL;
 value = "https://www.jetbrains.com";
 },
 {
-key = manufacturers;
+key = licenses;
 values = (
 {
 language = dflt;
-value = JetBrains;
+value = "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license is available with a FAQ at: https://scripts.sil.org/OFL";
 }
 );
 },
 {
-key = manufacturerURL;
-value = "https://www.jetbrains.com";
+key = licenseURL;
+value = "https://scripts.sil.org/OFL";
 },
 {
-key = licenses;
+key = manufacturers;
 values = (
 {
 language = dflt;
-value = "This Font Software is licensed under the SIL Open Font License, Version 1.1. This license is available with a FAQ at: https://scripts.sil.org/OFL";
+value = JetBrains;
 }
 );
 },
 {
-key = licenseURL;
-value = "https://scripts.sil.org/OFL";
+key = manufacturerURL;
+value = "https://www.jetbrains.com";
 },
 {
 key = trademarks;
 values = (
 {
 language = dflt;
 value = "JetBrains Mono is a trademark of JetBrains s.r.o.";
```

### Comparing `glyphspkg-0.1.9/tests/package_to_single_test.py` & `glyphspkg-0.2.0/tests/package_to_single_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
 import unittest
 
 from glyphspkg.package_to_single import package_to_single
+from glyphspkg.paths import rmdir
 from pathlib import Path
 
 
 def get_mono_path():
     return (
         Path(__file__).parent / "data" / "JetBrainsMono-Italic.glyphspackage"
     )
@@ -35,13 +36,8 @@
         out_dir.mkdir(exist_ok=True)
         out_file = out_dir / "custom.glyphs"
         package_to_single(get_mono_path(), out_file)
         assert out_file.is_file()
 
     @classmethod
     def tearDownClass(cls):
-        for entry in get_tmp_path().iterdir():
-            if entry.is_dir():
-                entry.rmdir()
-            else:
-                entry.unlink()
-        get_tmp_path().rmdir()
+        rmdir(get_tmp_path())
```

