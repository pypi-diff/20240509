# Comparing `tmp/soccerdata-1.6.1.tar.gz` & `tmp/soccerdata-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soccerdata-1.6.1.tar", max compression
+gzip compressed data, was "soccerdata-1.7.0.tar", max compression
```

## Comparing `soccerdata-1.6.1.tar` & `soccerdata-1.7.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1384 2024-03-22 22:23:14.031880 soccerdata-1.6.1/LICENSE.rst
--rw-r--r--   0        0        0     3961 2024-03-22 22:23:14.031880 soccerdata-1.6.1/README.rst
--rw-r--r--   0        0        0     2339 2024-03-22 22:23:26.443882 soccerdata-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      548 2024-03-22 22:23:26.443882 soccerdata-1.6.1/soccerdata/__init__.py
--rw-r--r--   0        0        0    22016 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/_common.py
--rw-r--r--   0        0        0     5741 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/_config.py
--rw-r--r--   0        0        0     6349 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/clubelo.py
--rw-r--r--   0        0        0    13855 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/espn.py
--rw-r--r--   0        0        0    47226 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/fbref.py
--rw-r--r--   0        0        0     8537 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/fivethirtyeight.py
--rw-r--r--   0        0        0    17214 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/fotmob.py
--rw-r--r--   0        0        0     4658 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/match_history.py
--rw-r--r--   0        0        0    17504 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/sofifa.py
--rw-r--r--   0        0        0    25962 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/understat.py
--rw-r--r--   0        0        0    33035 2024-03-22 22:23:14.047880 soccerdata-1.6.1/soccerdata/whoscored.py
--rw-r--r--   0        0        0     5276 1970-01-01 00:00:00.000000 soccerdata-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1384 2024-05-09 20:04:25.002545 soccerdata-1.7.0/LICENSE.rst
+-rw-r--r--   0        0        0     4017 2024-05-09 20:04:25.002545 soccerdata-1.7.0/README.rst
+-rw-r--r--   0        0        0     2361 2024-05-09 20:04:36.218657 soccerdata-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      598 2024-05-09 20:04:36.218657 soccerdata-1.7.0/soccerdata/__init__.py
+-rw-r--r--   0        0        0    22163 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/_common.py
+-rw-r--r--   0        0        0     5910 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/_config.py
+-rw-r--r--   0        0        0     6349 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/clubelo.py
+-rw-r--r--   0        0        0    13855 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/espn.py
+-rw-r--r--   0        0        0    47579 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/fbref.py
+-rw-r--r--   0        0        0     8537 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/fivethirtyeight.py
+-rw-r--r--   0        0        0    17171 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/fotmob.py
+-rw-r--r--   0        0        0     4658 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/match_history.py
+-rw-r--r--   0        0        0    10406 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/sofascore.py
+-rw-r--r--   0        0        0    17504 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/sofifa.py
+-rw-r--r--   0        0        0    25962 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/understat.py
+-rw-r--r--   0        0        0    33035 2024-05-09 20:04:25.018546 soccerdata-1.7.0/soccerdata/whoscored.py
+-rw-r--r--   0        0        0     5332 1970-01-01 00:00:00.000000 soccerdata-1.7.0/PKG-INFO
```

### Comparing `soccerdata-1.6.1/LICENSE.rst` & `soccerdata-1.7.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.6.1/README.rst` & `soccerdata-1.7.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
    :target: https://github.com/psf/black
    :alt: Black
 
 .. badges-end
 
 SoccerData is a collection of scrapers to gather soccer data from popular
 websites, including `Club Elo`_, `ESPN`_, `FBref`_, `FiveThirtyEight`_,
-`Football-Data.co.uk`_, `FotMob`_, `SoFIFA`_, `Understat`_ and `WhoScored`_.
+`Football-Data.co.uk`_, `FotMob`_, `Sofascore`_, `SoFIFA`_, `Understat`_ and `WhoScored`_.
 You get Pandas DataFrames with sensible, matching column names and identifiers
 across datasets. Data is downloaded when needed and cached locally.
 
 .. code:: python
 
    import soccerdata as sd
 
@@ -62,14 +62,15 @@
 
 .. _Club Elo: https://www.clubelo.com/
 .. _ESPN: https://www.espn.com/soccer/
 .. _FBref: https://www.fbref.com/en/
 .. _FiveThirtyEight: https://fivethirtyeight.com/soccer-predictions/
 .. _Football-Data.co.uk: https://www.football-data.co.uk/
 .. _FotMob: https://fotmob.com/
+.. _Sofascore: https://www.sofascore.com/
 .. _SoFIFA: https://sofifa.com/
 .. _Understat: https://understat.com/
 .. _WhoScored: https://www.whoscored.com/
 
 **Usage Notice:** Please use this web scraping tool responsibly and in compliance with the terms of service of the
 websites you intend to scrape. The software is provided as-is, without any warranty or guarantees of any kind. The
 developers disclaim any responsibility for misuse, legal consequences, or damages resulting from its use. It is
```

### Comparing `soccerdata-1.6.1/pyproject.toml` & `soccerdata-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "soccerdata"
-version = "1.6.1"
+version = "1.7.0"
 description = "A collection of wrappers over soccer data from various websites / APIs."
 authors = ["Pieter Robberechts <pieter.robberechts@kuleuven.be>"]
 license = "Apache-2.0"
 readme = 'README.rst'
 homepage = "https://github.com/probberechts/soccerdata"
 repository = "https://github.com/probberechts/soccerdata"
 keywords = ["soccer", "football", "soccer data", "web scraping", "soccer analytics"]
@@ -70,14 +70,15 @@
 
 [tool.coverage.paths]
 source = ["soccerdata", "*/site-packages"]
 
 [tool.coverage.run]
 branch = true
 source = ["soccerdata"]
+relative_files = true
 
 [tool.coverage.report]
 show_missing = true
 ignore_errors = true
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `soccerdata-1.6.1/soccerdata/__init__.py` & `soccerdata-1.7.0/soccerdata/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """A collection of tools to read and process soccer data from various sources."""
 
-__version__ = '1.6.1'
+__version__ = '1.7.0'
 
 __all__ = [
     'ClubElo',
     'ESPN',
     'FBref',
     'FiveThirtyEight',
     'FotMob',
     'MatchHistory',
+    'Sofascore',
     'SoFIFA',
     'Understat',
     'WhoScored',
 ]
 
 from .clubelo import ClubElo
 from .espn import ESPN
 from .fbref import FBref
 from .fivethirtyeight import FiveThirtyEight
 from .fotmob import FotMob
 from .match_history import MatchHistory
+from .sofascore import Sofascore
 from .sofifa import SoFIFA
 from .understat import Understat
 from .whoscored import WhoScored
```

### Comparing `soccerdata-1.6.1/soccerdata/_common.py` & `soccerdata-1.7.0/soccerdata/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,15 +245,15 @@
                 ids = [ids]
             tmp_league_dict = {}
             for i in ids:
                 if i not in self._all_leagues():
                     raise ValueError(
                         f"""
                         Invalid league '{i}'. Valid leagues are:
-                        { pprint.pformat(self.available_leagues()) }
+                        {pprint.pformat(self.available_leagues())}
                         """
                     )
                 tmp_league_dict[i] = self._all_leagues()[i]
             self._leagues_dict = tmp_league_dict
 
     def _is_complete(self, league: str, season: str) -> bool:
         """Check if a season is complete."""
@@ -286,15 +286,15 @@
         return self._season_ids
 
     @seasons.setter
     def seasons(self, seasons: Optional[Union[str, int, Iterable[Union[str, int]]]]) -> None:
         if seasons is None:
             logger.info("No seasons provided. Will retrieve data for the last 5 seasons.")
             year = datetime.today().year
-            seasons = [f"{y-1}-{y}" for y in range(year, year - 6, -1)]
+            seasons = [f"{y - 1}-{y}" for y in range(year, year - 6, -1)]
         if isinstance(seasons, str) or isinstance(seasons, int):
             seasons = [seasons]
         self._season_ids = [season_code(s) for s in seasons]
 
 
 class BaseRequestsReader(BaseReader):
     """Base class for readers that use the Python requests module."""
@@ -478,14 +478,15 @@
     season = str(season)
     pat1 = re.compile(r"^[0-9]{4}$")  # 1994 | 9495
     pat2 = re.compile(r"^[0-9]{2}$")  # 94
     pat3 = re.compile(r"^[0-9]{4}-[0-9]{4}$")  # 1994-1995
     pat4 = re.compile(r"^[0-9]{4}/[0-9]{4}$")  # 1994/1995
     pat5 = re.compile(r"^[0-9]{4}-[0-9]{2}$")  # 1994-95
     pat6 = re.compile(r"^[0-9]{2}-[0-9]{2}$")  # 94-95
+    pat7 = re.compile(r"^[0-9]{2}/[0-9]{2}$")  # 94/95
 
     if re.match(pat1, season):
         if int(season[2:]) == int(season[:2]) + 1:
             if season == "2021":
                 msg = 'Season id "{}" is ambiguous: interpreting as "{}-{}"'.format(
                     season, season[:2], season[-2:]
                 )
@@ -504,14 +505,16 @@
         return "".join([season[2:4], season[-2:]])  # 1994-1995
     elif re.match(pat4, season):
         return "".join([season[2:4], season[-2:]])  # 1994/1995
     elif re.match(pat5, season):
         return "".join([season[2:4], season[-2:]])  # 1994-95
     elif re.match(pat6, season):
         return "".join([season[:2], season[-2:]])  # 94-95
+    elif re.match(pat7, season):
+        return "".join([season[:2], season[-2:]])  # 94/95
     else:
         return season
 
 
 def make_game_id(row: pd.Series) -> str:
     """Return a game id based on date, home and away team."""
     if pd.isnull(row["date"]):
```

### Comparing `soccerdata-1.6.1/soccerdata/_config.py` & `soccerdata-1.7.0/soccerdata/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,66 +95,71 @@
     "ENG-Premier League": {
         "ClubElo": "ENG_1",
         "MatchHistory": "E0",
         "FiveThirtyEight": "premier-league",
         "FBref": "Premier League",
         "FotMob": "ENG-Premier League",
         "ESPN": "eng.1",
+        "Sofascore": "Premier League",
         "SoFIFA": "[England] Premier League",
         "Understat": "EPL",
         "WhoScored": "England - Premier League",
         "season_start": "Aug",
         "season_end": "May",
     },
     "ESP-La Liga": {
         "ClubElo": "ESP_1",
         "MatchHistory": "SP1",
         "FiveThirtyEight": "la-liga",
         "FBref": "La Liga",
         "FotMob": "ESP-LaLiga",
         "ESPN": "esp.1",
+        "Sofascore": "LaLiga",
         "SoFIFA": "[Spain] La Liga",
         "Understat": "La liga",
         "WhoScored": "Spain - LaLiga",
         "season_start": "Aug",
         "season_end": "May",
     },
     "ITA-Serie A": {
         "ClubElo": "ITA_1",
         "MatchHistory": "I1",
         "FiveThirtyEight": "serie-a",
         "FBref": "Serie A",
         "FotMob": "ITA-Serie A",
         "ESPN": "ita.1",
+        "Sofascore": "Serie A",
         "SoFIFA": "[Italy] Serie A",
         "Understat": "Serie A",
         "WhoScored": "Italy - Serie A",
         "season_start": "Aug",
         "season_end": "May",
     },
     "GER-Bundesliga": {
         "ClubElo": "GER_1",
         "MatchHistory": "D1",
         "FiveThirtyEight": "bundesliga",
         "FBref": "Fußball-Bundesliga",
         "FotMob": "GER-Bundesliga",
         "ESPN": "ger.1",
+        "Sofascore": "Bundesliga",
         "SoFIFA": "[Germany] Bundesliga",
         "Understat": "Bundesliga",
         "WhoScored": "Germany - Bundesliga",
         "season_start": "Aug",
         "season_end": "May",
     },
     "FRA-Ligue 1": {
         "ClubElo": "FRA_1",
         "MatchHistory": "F1",
         "FiveThirtyEight": "ligue-1",
         "FBref": "Ligue 1",
         "FotMob": "FRA-Ligue 1",
         "ESPN": "fra.1",
+        "Sofascore": "Ligue 1",
         "SoFIFA": "[France] Ligue 1",
         "Understat": "Ligue 1",
         "WhoScored": "France - Ligue 1",
         "season_start": "Aug",
         "season_end": "May",
     },
     "INT-World Cup": {
```

### Comparing `soccerdata-1.6.1/soccerdata/clubelo.py` & `soccerdata-1.7.0/soccerdata/clubelo.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.6.1/soccerdata/espn.py` & `soccerdata-1.7.0/soccerdata/espn.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.6.1/soccerdata/fbref.py` & `soccerdata-1.7.0/soccerdata/fbref.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,15 @@
         return df
 
     def read_team_match_stats(  # noqa: C901
         self,
         stat_type: str = "schedule",
         opponent_stats: bool = False,
         team: Optional[Union[str, List[str]]] = None,
+        force_cache: bool = False,
     ) -> pd.DataFrame:
         """Retrieve the match logs for all teams in the selected leagues and seasons.
 
         The following stat types are available:
             * 'schedule'
             * 'keeper'
             * 'shooting'
@@ -355,14 +356,17 @@
         ----------
         stat_type: str
             Type of stats to retrieve.
         opponent_stats: bool
             If True, will retrieve opponent stats.
         team: str or list of str, optional
             Team(s) to retrieve. If None, will retrieve all teams.
+        force_cache: bool
+            By default no cached data is used for the current season.
+            If True, will force the use of cached data anyway.
 
         Raises
         ------
         ValueError
             If ``stat_type`` is not valid.
 
         Returns
@@ -415,15 +419,15 @@
             if len(iterator) == 0:
                 raise ValueError("No data found for the given teams in the selected seasons.")
         else:
             iterator = df_teams
 
         # collect match logs for each team
         stats = []
-        for (_, skey, team), team_url in iterator.url.items():
+        for (lkey, skey, team), team_url in iterator.url.items():
             # read html page
             filepath = self.data_dir / filemask.format(team, skey, stat_type)
             if len(team_url.split('/')) == 6:  # already have season in the url
                 url = (
                     FBREF_API
                     + team_url.rsplit("/", 1)[0]
                     + "/matchlogs"
@@ -439,15 +443,17 @@
                     FBREF_API
                     + team_url.rsplit("/", 1)[0]
                     + f"/{season_format}"
                     + "/matchlogs"
                     + "/all_comps"
                     + f"/{stat_type}"
                 )
-            reader = self.get(url, filepath)
+
+            current_season = not self._is_complete(lkey, skey)
+            reader = self.get(url, filepath, no_cache=current_season and not force_cache)
 
             # parse HTML and select table
             tree = html.parse(reader)
             (html_table,) = tree.xpath(f"//table[@id='matchlogs_{opp_type}']")
             # remove for / against header
             for elem in html_table.xpath("//th[@data-stat='header_for_against']"):
                 elem.text = ""
@@ -467,16 +473,15 @@
                     if mlink.xpath("./a") and mlink.xpath("./a")[0].text == "Match Report"
                     else None
                 )
                 for mlink in html_table.xpath(".//td[@data-stat='match_report']")
             ]
             nb_levels = df_table.columns.nlevels
             if nb_levels == 2:
-                df_table = df_table.drop("Match Report", axis=1, level=1)
-                df_table = df_table.drop("Time", axis=1, level=1)
+                df_table = df_table.drop(["Match Report", "Time"], axis=1, level=1)
             stats.append(df_table)
 
         # return data frame
         df = (
             _concat(stats, key=['league', 'season', 'team'])
             .replace(
                 {
@@ -975,15 +980,15 @@
             tree = html.parse(reader)
             teams = self._parse_teams(tree)
             for team, tid in zip(teams, ["a", "b"]):
                 html_events = tree.xpath(f"////*[@id='events_wrap']/div/div[@class='event {tid}']")
                 for e in html_events:
                     minute = e.xpath("./div[1]")[0].text.replace("&rsquor;", "").strip()
                     score = e.xpath("./div[1]/small/span")[0].text
-                    player1 = e.xpath("./div[2]/div[2]/div/a")[0].text
+                    player1 = e.xpath("./div[2]/div[2]/div")[0].text_content().strip()
                     if e.xpath("./div[2]/div[2]/small/a"):
                         player2 = e.xpath("./div[2]/div[2]/small/a")[0].text
                     else:
                         player2 = None
                     event_type = e.xpath("./div[2]/div[1]/@class")[0].split(" ")[1]
                     match_events.append(
                         {
@@ -991,18 +996,20 @@
                             "minute": minute,
                             "score": score,
                             "player1": player1,
                             "player2": player2,
                             "event_type": event_type,
                         }
                     )
-            df_match_events = pd.DataFrame(match_events).sort_values(by="minute")
+            df_match_events = pd.DataFrame(match_events)
             df_match_events["game"] = game["game"]
             df_match_events["league"] = game["league"]
             df_match_events["season"] = game["season"]
+            if len(df_match_events) > 0:
+                df_match_events.sort_values(by="minute", inplace=True)
             events.append(df_match_events)
 
         if len(events) == 0:
             return pd.DataFrame()
 
         df = (
             pd.concat(events)
```

### Comparing `soccerdata-1.6.1/soccerdata/fivethirtyeight.py` & `soccerdata-1.7.0/soccerdata/fivethirtyeight.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.6.1/soccerdata/fotmob.py` & `soccerdata-1.7.0/soccerdata/fotmob.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,34 +405,30 @@
             try:
                 selected_stats = next(stat for stat in all_stats if stat["title"] == stat_type)
             except StopIteration:
                 raise ValueError(f"Invalid stat type: {stat_type}")
 
             df_raw_stats = pd.DataFrame(selected_stats['stats'])
             game_teams = [game.home_team, game.away_team]
-            if opponent_stats:
-                game_teams = [game.away_team, game.home_team]
             for i, team in enumerate(game_teams):
                 df_team_stats = df_raw_stats.copy()
                 df_team_stats['stat'] = df_team_stats['stats'].apply(lambda x: x[i])  # noqa: B023
                 df_team_stats["league"] = lkey
                 df_team_stats["season"] = skey
                 df_team_stats["game"] = gkey
                 df_team_stats['team'] = team
+                if not opponent_stats:
+                    df_team_stats = df_team_stats[df_team_stats.team.isin(teams_to_check)]
                 df_team_stats.set_index(['league', 'season', 'game', 'team'], inplace=True)
                 df_team_stats = df_team_stats[df_team_stats['type'] != 'title']
                 df_team_stats = df_team_stats.pivot(columns='title', values='stat').reset_index()
                 df_team_stats.columns.name = None
                 stats.append(df_team_stats)
 
         df = pd.concat(stats, axis=0)
-        df = (
-            df[df.team.isin(teams_to_check)]
-            .set_index(['league', 'season', 'game', 'team'])
-            .sort_index()
-        )
+        df = df.set_index(['league', 'season', 'game', 'team']).sort_index()
         # Split percentage values
         pct_cols = [col for col in df.columns if df[col].astype(str).str.contains('%').any()]
         for col in pct_cols:
             df[[col, col + ' (%)']] = df[col].str.split(expand=True)
             df[col + ' (%)'] = df[col + ' (%)'].str.extract(r'(\d+)').astype(float).div(100)
         return df
```

### Comparing `soccerdata-1.6.1/soccerdata/match_history.py` & `soccerdata-1.7.0/soccerdata/match_history.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.6.1/soccerdata/sofifa.py` & `soccerdata-1.7.0/soccerdata/sofifa.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.6.1/soccerdata/understat.py` & `soccerdata-1.7.0/soccerdata/understat.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.6.1/soccerdata/whoscored.py` & `soccerdata-1.7.0/soccerdata/whoscored.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.6.1/PKG-INFO` & `soccerdata-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soccerdata
-Version: 1.6.1
+Version: 1.7.0
 Summary: A collection of wrappers over soccer data from various websites / APIs.
 Home-page: https://github.com/probberechts/soccerdata
 License: Apache-2.0
 Keywords: soccer,football,soccer data,web scraping,soccer analytics
 Author: Pieter Robberechts
 Author-email: pieter.robberechts@kuleuven.be
 Requires-Python: >=3.9,<3.13
@@ -66,15 +66,15 @@
    :target: https://github.com/psf/black
    :alt: Black
 
 .. badges-end
 
 SoccerData is a collection of scrapers to gather soccer data from popular
 websites, including `Club Elo`_, `ESPN`_, `FBref`_, `FiveThirtyEight`_,
-`Football-Data.co.uk`_, `FotMob`_, `SoFIFA`_, `Understat`_ and `WhoScored`_.
+`Football-Data.co.uk`_, `FotMob`_, `Sofascore`_, `SoFIFA`_, `Understat`_ and `WhoScored`_.
 You get Pandas DataFrames with sensible, matching column names and identifiers
 across datasets. Data is downloaded when needed and cached locally.
 
 .. code:: python
 
    import soccerdata as sd
 
@@ -93,14 +93,15 @@
 
 .. _Club Elo: https://www.clubelo.com/
 .. _ESPN: https://www.espn.com/soccer/
 .. _FBref: https://www.fbref.com/en/
 .. _FiveThirtyEight: https://fivethirtyeight.com/soccer-predictions/
 .. _Football-Data.co.uk: https://www.football-data.co.uk/
 .. _FotMob: https://fotmob.com/
+.. _Sofascore: https://www.sofascore.com/
 .. _SoFIFA: https://sofifa.com/
 .. _Understat: https://understat.com/
 .. _WhoScored: https://www.whoscored.com/
 
 **Usage Notice:** Please use this web scraping tool responsibly and in compliance with the terms of service of the
 websites you intend to scrape. The software is provided as-is, without any warranty or guarantees of any kind. The
 developers disclaim any responsibility for misuse, legal consequences, or damages resulting from its use. It is
```

