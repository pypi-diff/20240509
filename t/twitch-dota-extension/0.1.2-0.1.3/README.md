# Comparing `tmp/twitch_dota_extension-0.1.2.tar.gz` & `tmp/twitch_dota_extension-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch_dota_extension-0.1.2.tar", max compression
+gzip compressed data, was "twitch_dota_extension-0.1.3.tar", max compression
```

## Comparing `twitch_dota_extension-0.1.2.tar` & `twitch_dota_extension-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       58 2024-04-17 16:20:11.616674 twitch_dota_extension-0.1.2/README.md
--rw-r--r--   0        0        0      480 2024-04-26 13:49:47.571251 twitch_dota_extension-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7727 2024-04-25 15:56:25.054341 twitch_dota_extension-0.1.2/twitch_dota_extension/lib.py
--rw-r--r--   0        0        0     2527 2024-04-18 19:25:34.069698 twitch_dota_extension-0.1.2/twitch_dota_extension/tooltips.py
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 twitch_dota_extension-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       58 2024-04-17 16:20:11.616674 twitch_dota_extension-0.1.3/README.md
+-rw-r--r--   0        0        0      480 2024-05-09 17:44:37.606257 twitch_dota_extension-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6796 2024-05-09 17:00:39.841479 twitch_dota_extension-0.1.3/twitch_dota_extension/lib.py
+-rw-r--r--   0        0        0     4546 2024-05-09 17:42:34.346097 twitch_dota_extension-0.1.3/twitch_dota_extension/tooltips.py
+-rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 twitch_dota_extension-0.1.3/PKG-INFO
```

### Comparing `twitch_dota_extension-0.1.2/twitch_dota_extension/lib.py` & `twitch_dota_extension-0.1.3/twitch_dota_extension/lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import enum
 import json
-import dataclasses
 from dataclasses import dataclass
 from typing import Optional, Any
-from pathlib import Path
 
 import dacite
 import httpx
 
 from twitch_dota_extension.tooltips import Hero, Ability, Item
 
 
@@ -39,15 +37,15 @@
 class HeroData:
     t: list[int]
     items: dict[str, HDItem]
     # base_ability_count: int
 
 @dataclass
 class TournamentHeroData(HeroData):
-    p: str # playername
+    p: str
     lvl: int
     aghs: list[int]
 
 @dataclass
 class TalentEntry:
     name: str
     picked: bool
@@ -69,15 +67,21 @@
 @dataclass
 class ProcessedHeroData:
     n: str
     name: str
     talent_tree: TalentTree
     abilities: list[Ability]
     inventory: Inventory
+
+@dataclass
+class TourProcessedHeroData(ProcessedHeroData):
     player: Optional[str] = None
+    level: Optional[int] = None
+    has_aghs: Optional[bool] = False
+    has_shard: Optional[bool] = False
 
 
 @dataclass
 class Playing:
     selected_hero: str
     selected_hero_data: HeroData
 
@@ -115,22 +119,24 @@
     hero_data: dict[str, HeroData]
 
 
 @dataclass
 class SpectatingTournament:
     hero_data: dict[str, TournamentHeroData]
 
-    def process_data(self, heroes: dict[str, Hero], items) -> list[ProcessedHeroData]:
+    def process_data(self, heroes: dict[str, Hero], items) -> list[TourProcessedHeroData]:
         ret = []
         for hero_name, hero_state in self.hero_data.items():
             hero = heroes[hero_name]
             talents = TalentTree.from_parts(hero.talents, hero_state.t)
             inv = Inventory.from_parts(hero_state.items, items)
 
-            phd = ProcessedHeroData(hero.n, hero_name, talents, hero.abilities, inv, player=hero_state.p)
+            phd = TourProcessedHeroData(hero.n, hero.name, talents, hero.abilities, inv,
+                                    player=hero_state.p, level=hero_state.lvl,
+                                    has_aghs=bool(hero_state.aghs[0]), has_shard=bool(hero_state.aghs[1]))
             ret.append(phd)
         return ret
 
 @dataclass
 class InvalidResponse:
     r: dict[str, Any]
 
@@ -212,43 +218,7 @@
             return dacite.from_dict(data_class=Playing, data=game)
         elif state == "spectating" and game.get('matchid'):  # Tournament
             return dacite.from_dict(data_class=SpectatingTournament, data=game)
         elif state == "spectating":
             return dacite.from_dict(data_class=Spectating, data=game)
 
         return InvalidResponse(r=data)
-
-
-
-class EnhancedJSONEncoder(json.JSONEncoder):
-        def default(self, o):
-            if dataclasses.is_dataclass(o):
-                return dataclasses.asdict(o)
-            return super().default(o)
-
-
-if __name__ == "__main__":
-
-    async def f():
-        api = API()
-        with Path("./data/playing-2.json").open() as fd:
-        #with Path("./data/spectating-tournament.json").open() as fd:
-            # with Path('./data/spectating.json').open() as fd:
-            # with Path('./data/full-heroes.json').open() as fd:
-            data = json.load(fd)
-
-        heroes = await api.fetch_heroes()
-        items = await api.fetch_items()
-        game_state = api._from_json(data)
-        match game_state:
-            case Playing():
-                phd = game_state.process_data(heroes, items)
-                fd = open("data/output/playing.json", 'w')
-                print(json.dumps(phd, cls=EnhancedJSONEncoder), file=fd)
-
-            case SpectatingTournament():
-                phd = game_state.process_data(heroes, items)
-
-                fd = open("data/output/tournament.json", 'w')
-                print(json.dumps(phd, cls=EnhancedJSONEncoder), file=fd)
-    import asyncio
-    asyncio.run(f())
```

### Comparing `twitch_dota_extension-0.1.2/PKG-INFO` & `twitch_dota_extension-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitch-dota-extension
-Version: 0.1.2
+Version: 0.1.3
 Summary: Interact with the Dota2 Extension API for a given Twitch channel ID
 License: MIT
 Author: David Ventura
 Author-email: davidventura27@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

