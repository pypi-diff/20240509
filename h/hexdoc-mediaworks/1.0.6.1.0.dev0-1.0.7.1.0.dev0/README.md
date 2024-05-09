# Comparing `tmp/hexdoc_mediaworks-1.0.6.1.0.dev0.tar.gz` & `tmp/hexdoc_mediaworks-1.0.7.1.0.dev0.tar.gz`

## Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0.tar` & `hexdoc_mediaworks-1.0.7.1.0.dev0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/gradle.properties
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/__gradle_version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/__init__.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/__version__.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_hooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/py.typed
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/__init__.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/mediaworks.hexdoc.json
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/mediaworks.patterns.hexdoc.json
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
--rw-r--r--   0        0        0    20385 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/lang/en_us.json
--rw-r--r--   0        0        0    30576 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/lang/zh_cn.json
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/models/item/magic_cloak.json
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak.png
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak_default.png
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak_overlay.png
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/mob_effect/astral_projection.png
--rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/models/armor/magic_cloak.png
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/models/armor/magic_cloak_overlay.png
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/minecraft/lang/en_us.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/lang/en_us.json
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/models/block/sack_closed.json
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/models/item/sack.json
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_bottom.png
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_bottom1.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_bottom2.png
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_bottom_r.png
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_closed.png
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_closed1.png
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_closed_r.png
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_front.png
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_front1.png
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_front_r.png
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top.png
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top1.png
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top2.png
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top_r.png
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/book.json
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/categories/patterns/macula.json
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/basics/mediaworks_tweaks.json
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/greatwork/astral_self.json
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/interop/mediaworks_containers.json
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/interop/mediaworks_moreiotas.json
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/items/magic_cloak.json
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/astral_utils.json
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/cloak_patterns.json
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/media_patterns.json
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/great_spells/astral_projection.json
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/black_eye.json
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/macula_concepts.json
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/macula_patterns.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/text_visages.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_templates/__init__.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/.gitignore
--rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/LICENSE.md
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/doc/README.md
--rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.6.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/gradle.properties
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/__gradle_version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/__version__.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_hooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/py.typed
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/__init__.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/mediaworks.hexdoc.json
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/mediaworks.patterns.hexdoc.json
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/hexcasting/lang/en_us.flatten.json5
+-rw-r--r--   0        0        0    20385 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/lang/en_us.json
+-rw-r--r--   0        0        0    30576 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/lang/zh_cn.json
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/models/item/magic_cloak.json
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak.png
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak_default.png
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak_overlay.png
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/mob_effect/astral_projection.png
+-rw-r--r--   0        0        0     5261 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/models/armor/magic_cloak.png
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/models/armor/magic_cloak_overlay.png
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/minecraft/lang/en_us.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/lang/en_us.json
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/models/block/sack_closed.json
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/models/item/sack.json
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_bottom.png
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_bottom1.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_bottom2.png
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_bottom_r.png
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_closed.png
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_closed1.png
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_closed_r.png
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_front.png
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_front1.png
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_front_r.png
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top.png
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top1.png
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top2.png
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top_r.png
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/book.json
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/categories/patterns/macula.json
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/basics/mediaworks_tweaks.json
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/greatwork/astral_self.json
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/interop/mediaworks_containers.json
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/interop/mediaworks_moreiotas.json
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/items/magic_cloak.json
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/astral_utils.json
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/cloak_patterns.json
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/media_patterns.json
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/great_spells/astral_projection.json
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/black_eye.json
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/macula_concepts.json
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/macula_patterns.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/text_visages.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_templates/__init__.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/.gitignore
+-rw-r--r--   0        0        0     7487 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/LICENSE.md
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/doc/README.md
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 hexdoc_mediaworks-1.0.7.1.0.dev0/PKG-INFO
```

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/gradle.properties` & `hexdoc_mediaworks-1.0.7.1.0.dev0/gradle.properties`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 jetbrainsAnnotationsVersion=23.0.0
 # gradle kotlin jvm plugin breaks without this
 kotlin.stdlib.default.dependency=false
 # needed for mixins to work for forge
 asmVersion=9.4
 # mod info
 modId=mediaworks
-modVersion=1.0.6
+modVersion=1.0.7
 modName=Mediaworks
 modDescription=A Hex Casting addon focusing on diverse casting utilities and quality-of-life tweaks
 modAuthor=artynova
 modPage=https://modrinth.com/mod/mediaworks
 modSource=https://github.com/artynova/mediaworks
 modIssueTracker=https://github.com/artynova/mediaworks/issues
 modLicense=MIT
```

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/__gradle_version__.py` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/__gradle_version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This file is auto-generated by hatch-gradle-version. Do not edit.
 
-GRADLE_VERSION = "1.0.6"
-FULL_VERSION = "1.0.6.1.0.dev0"
+GRADLE_VERSION = "1.0.7"
+FULL_VERSION = "1.0.7.1.0.dev0"
 
 ARCHITECTURY_VERSION = "6.5.85"
 ASM_VERSION = "9.4"
 CARDINAL_COMPONENTS_VERSION = "5.0.2"
 CURIOS_VERSION = "5.1.4.1"
 CURSEFORGE_ID = ""
 ENABLED_PLATFORMS = "fabric,forge"
@@ -30,15 +30,15 @@
 MOD_ID = "mediaworks"
 MOD_ISSUE_TRACKER = "https://github.com/artynova/mediaworks/issues"
 MOD_LICENSE = "MIT"
 MOD_NAME = "Mediaworks"
 MOD_PACK_FORMAT = "10"
 MOD_PAGE = "https://modrinth.com/mod/mediaworks"
 MOD_SOURCE = "https://github.com/artynova/mediaworks"
-MOD_VERSION = "1.0.6"
+MOD_VERSION = "1.0.7"
 MODRINTH_ID = "2kZJcMa9"
 MORE_IOTAS_FABRIC_VERSION = "0.0.4"
 ORG_GRADLE_JVMARGS = "-Xmx2048M"
 PATCHOULI_VERSION = "77"
 PAUCAL_VERSION = "0.5.0"
 SERIALIZATION_HOOKS_VERSION = "0.3.24"
 TRINKETS_VERSION = "3.4.1"
```

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_hooks.py` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_hooks.py`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/mediaworks.patterns.hexdoc.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/mediaworks.patterns.hexdoc.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/lang/en_us.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/lang/en_us.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/lang/zh_cn.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/lang/zh_cn.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak_default.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak_default.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak_overlay.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/item/magic_cloak_overlay.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/mob_effect/astral_projection.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/mob_effect/astral_projection.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/models/armor/magic_cloak.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/models/armor/magic_cloak.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/models/armor/magic_cloak_overlay.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/mediaworks/textures/models/armor/magic_cloak_overlay.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/models/block/sack_closed.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/models/block/sack_closed.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_bottom1.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_bottom1.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_closed1.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_closed1.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_front.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_front.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_front1.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_front1.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top1.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top1.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top2.png` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/assets/supplementaries/textures/blocks/sack_top2.png`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/items/magic_cloak.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/items/magic_cloak.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/astral_utils.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/astral_utils.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/media_patterns.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/media_patterns.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/great_spells/astral_projection.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/great_spells/astral_projection.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/macula_concepts.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/macula_concepts.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/macula_patterns.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/macula_patterns.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/text_visages.json` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/src/hexdoc_mediaworks/_export/generated/data/mediaworks/patchouli_books/mediaworksbook/en_us/entries/patterns/macula/text_visages.json`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/.gitignore` & `hexdoc_mediaworks-1.0.7.1.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/LICENSE.md` & `hexdoc_mediaworks-1.0.7.1.0.dev0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/pyproject.toml` & `hexdoc_mediaworks-1.0.7.1.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/doc/README.md` & `hexdoc_mediaworks-1.0.7.1.0.dev0/doc/README.md`

 * *Files identical despite different names*

### Comparing `hexdoc_mediaworks-1.0.6.1.0.dev0/PKG-INFO` & `hexdoc_mediaworks-1.0.7.1.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hexdoc-mediaworks
-Version: 1.0.6.1.0.dev0
+Version: 1.0.7.1.0.dev0
 Summary: Python web book docgen and hexdoc plugin for Mediaworks.
 Project-URL: Homepage, https://artynova.github.io/mediaworks/
 Project-URL: Source, https://github.com/artynova/mediaworks
 Author: artynova
 License-File: LICENSE.md
 Keywords: hexdoc
 Requires-Python: >=3.11
```

