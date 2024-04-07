# Comparing `tmp/fusion_stat-0.0.8.tar.gz` & `tmp/fusion_stat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fusion_stat-0.0.8.tar", max compression
+gzip compressed data, was "fusion_stat-0.0.9.tar", max compression
```

## Comparing `fusion_stat-0.0.8.tar` & `fusion_stat-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1067 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/LICENSE
--rw-r--r--   0        0        0     1750 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/README.md
--rw-r--r--   0        0        0      311 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/__init__.py
--rw-r--r--   0        0        0     5210 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/api.py
--rw-r--r--   0        0        0      953 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/config.py
--rw-r--r--   0        0        0    23111 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/models.py
--rw-r--r--   0        0        0        0 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/py.typed
--rw-r--r--   0        0        0     1613 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/scraper.py
--rw-r--r--   0        0        0      113 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/__init__.py
--rw-r--r--   0        0        0      151 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fbref/__init__.py
--rw-r--r--   0        0        0      514 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fbref/_common.py
--rw-r--r--   0        0        0     2148 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fbref/competition.py
--rw-r--r--   0        0        0     1876 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fbref/competitions.py
--rw-r--r--   0        0        0      722 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fbref/match.py
--rw-r--r--   0        0        0      597 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fbref/matches.py
--rw-r--r--   0        0        0     1132 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fbref/player.py
--rw-r--r--   0        0        0     3403 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fbref/team.py
--rw-r--r--   0        0        0      198 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fotmob/__init__.py
--rw-r--r--   0        0        0      349 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fotmob/_common.py
--rw-r--r--   0        0        0     3545 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fotmob/competition.py
--rw-r--r--   0        0        0     1240 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fotmob/competitions.py
--rw-r--r--   0        0        0      698 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fotmob/match.py
--rw-r--r--   0        0        0     2663 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fotmob/matches.py
--rw-r--r--   0        0        0      830 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fotmob/player.py
--rw-r--r--   0        0        0      563 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fotmob/staff.py
--rw-r--r--   0        0        0     2007 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/fotmob/team.py
--rw-r--r--   0        0        0       54 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/official/__init__.py
--rw-r--r--   0        0        0     1138 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/official/_common.py
--rw-r--r--   0        0        0    10510 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/official/competition.py
--rw-r--r--   0        0        0     1490 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/official/competitions.py
--rw-r--r--   0        0        0      149 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/__init__.py
--rw-r--r--   0        0        0      822 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/_common.py
--rw-r--r--   0        0        0     2190 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/competition.py
--rw-r--r--   0        0        0     1788 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/competitions.py
--rw-r--r--   0        0        0      990 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/player.py
--rw-r--r--   0        0        0      876 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/staff.py
--rw-r--r--   0        0        0     1017 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/staffs.py
--rw-r--r--   0        0        0     2526 2024-03-20 03:24:28.275631 fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/team.py
--rw-r--r--   0        0        0     1819 2024-03-20 03:24:28.279631 fusion_stat-0.0.8/fusion_stat/utils.py
--rw-r--r--   0        0        0      889 2024-03-20 03:24:28.279631 fusion_stat-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 fusion_stat-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-20 16:09:44.403435 fusion_stat-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1750 2024-03-20 16:09:44.403435 fusion_stat-0.0.9/README.md
+-rw-r--r--   0        0        0      311 2024-03-20 16:09:44.403435 fusion_stat-0.0.9/fusion_stat/__init__.py
+-rw-r--r--   0        0        0     5210 2024-03-20 16:09:44.403435 fusion_stat-0.0.9/fusion_stat/api.py
+-rw-r--r--   0        0        0      980 2024-03-20 16:09:44.403435 fusion_stat-0.0.9/fusion_stat/config.py
+-rw-r--r--   0        0        0    23103 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/models.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/py.typed
+-rw-r--r--   0        0        0     1613 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/scraper.py
+-rw-r--r--   0        0        0      113 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/__init__.py
+-rw-r--r--   0        0        0      151 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fbref/__init__.py
+-rw-r--r--   0        0        0      514 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fbref/_common.py
+-rw-r--r--   0        0        0     2148 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fbref/competition.py
+-rw-r--r--   0        0        0     1876 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fbref/competitions.py
+-rw-r--r--   0        0        0      722 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fbref/match.py
+-rw-r--r--   0        0        0      597 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fbref/matches.py
+-rw-r--r--   0        0        0     1132 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fbref/player.py
+-rw-r--r--   0        0        0     3403 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fbref/team.py
+-rw-r--r--   0        0        0      198 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fotmob/__init__.py
+-rw-r--r--   0        0        0      349 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fotmob/_common.py
+-rw-r--r--   0        0        0     3545 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fotmob/competition.py
+-rw-r--r--   0        0        0     1240 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fotmob/competitions.py
+-rw-r--r--   0        0        0      698 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fotmob/match.py
+-rw-r--r--   0        0        0     3065 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fotmob/matches.py
+-rw-r--r--   0        0        0      830 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fotmob/player.py
+-rw-r--r--   0        0        0      563 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fotmob/staff.py
+-rw-r--r--   0        0        0     2007 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/fotmob/team.py
+-rw-r--r--   0        0        0       54 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/official/__init__.py
+-rw-r--r--   0        0        0     1138 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/official/_common.py
+-rw-r--r--   0        0        0    10510 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/official/competition.py
+-rw-r--r--   0        0        0     1490 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/official/competitions.py
+-rw-r--r--   0        0        0      149 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/__init__.py
+-rw-r--r--   0        0        0      822 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/_common.py
+-rw-r--r--   0        0        0     2190 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/competition.py
+-rw-r--r--   0        0        0     1788 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/competitions.py
+-rw-r--r--   0        0        0      990 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/player.py
+-rw-r--r--   0        0        0      876 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/staff.py
+-rw-r--r--   0        0        0     1017 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/staffs.py
+-rw-r--r--   0        0        0     2526 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/team.py
+-rw-r--r--   0        0        0     1819 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/fusion_stat/utils.py
+-rw-r--r--   0        0        0      889 2024-03-20 16:09:44.407435 fusion_stat-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2587 1970-01-01 00:00:00.000000 fusion_stat-0.0.9/PKG-INFO
```

### Comparing `fusion_stat-0.0.8/LICENSE` & `fusion_stat-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/README.md` & `fusion_stat-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/api.py` & `fusion_stat-0.0.9/fusion_stat/api.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/config.py` & `fusion_stat-0.0.9/fusion_stat/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from fifacodes import Members
 
-MEMBERS_SIMILARITY_SCORE = 80
+COMPETITIONS_SCORE_CUTOFF = 90
+MEMBERS_SCORE_CUFOFF = 80
 
 
 class CompetitionsConfig:
     data = (
         ("ENG", "Premier League"),
         ("ESP", "La Liga"),
         ("GER", "Bundesliga"),
```

### Comparing `fusion_stat-0.0.8/fusion_stat/models.py` & `fusion_stat-0.0.9/fusion_stat/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 
 from rapidfuzz import process
 
 from . import spiders
-from .config import MEMBERS_SIMILARITY_SCORE
+from .config import MEMBERS_SCORE_CUFOFF
 from .scraper import BaseItem
 from .utils import mean_scorer
 
 
 class CompetitionItemTypes(typing.Protocol):
     name: str
     country_code: str
@@ -450,15 +450,15 @@
             choices,
             scorer=mean_scorer,
             processor=lambda x: [
                 x.name,
                 x.country_code,
                 x.position,
             ],
-            score_cutoff=MEMBERS_SIMILARITY_SCORE,
+            score_cutoff=MEMBERS_SCORE_CUFOFF,
         )[0]
         return result
 
     @property
     def info(self) -> dict[str, typing.Any]:
         return {
             "id": self._fotmob.id,
```

### Comparing `fusion_stat-0.0.8/fusion_stat/scraper.py` & `fusion_stat-0.0.9/fusion_stat/scraper.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fbref/_common.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fbref/_common.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fbref/competition.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fbref/competition.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fbref/competitions.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fbref/competitions.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fbref/match.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fbref/match.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fbref/matches.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fbref/matches.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fbref/player.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fbref/player.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fbref/team.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fbref/team.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fotmob/competition.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fotmob/competition.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fotmob/competitions.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fotmob/competitions.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fotmob/match.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fotmob/match.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fotmob/matches.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fotmob/matches.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 
 import httpx
 from rapidfuzz import process
 
-from ...config import CompetitionsConfig
+from ...config import COMPETITIONS_SCORE_CUTOFF, CompetitionsConfig
 from ...scraper import BaseItem, BaseSpider
 from ._common import BASE_URL, parse_score
 
 
 class TeamItem(BaseItem):
     score: int | None
 
@@ -47,22 +47,30 @@
             if (country_code := com["ccode"]) in CompetitionsConfig.countries:
                 choices.append(
                     (country_code, com["name"], str(com["id"]), com["matches"])
                 )
 
         matches: list[Item] = []
         for query in CompetitionsConfig.data:
+            # 暂时用 .replace(" ", "") 消除了
+            # 'Premier League', 'Premier League U18'
+            # 所引发的匹配错误，后续会更新更好的方法
             result = process.extractOne(
                 query,
                 choices,
-                processor=lambda x: x[1],
-            )[0]
-            for node in result[3]:
-                match = self._parse_match(result[0], result[1], result[2], node)
-                matches.append(match)
+                processor=lambda x: x[1].replace(" ", ""),
+                score_cutoff=COMPETITIONS_SCORE_CUTOFF,
+            )
+            if result is not None:
+                choice = result[0]
+                for node in choice[3]:
+                    match = self._parse_match(
+                        choice[0], choice[1], choice[2], node
+                    )
+                    matches.append(match)
         return matches
 
     def _parse_match(
         self,
         competition_country_code: str,
         competition_name: str,
         competition_id: str,
```

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fotmob/player.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fotmob/player.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fotmob/staff.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fotmob/staff.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/fotmob/team.py` & `fusion_stat-0.0.9/fusion_stat/spiders/fotmob/team.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/official/_common.py` & `fusion_stat-0.0.9/fusion_stat/spiders/official/_common.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/official/competition.py` & `fusion_stat-0.0.9/fusion_stat/spiders/official/competition.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/official/competitions.py` & `fusion_stat-0.0.9/fusion_stat/spiders/official/competitions.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/_common.py` & `fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/_common.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/competition.py` & `fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/competition.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/competitions.py` & `fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/competitions.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/player.py` & `fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/player.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/staff.py` & `fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/staff.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/staffs.py` & `fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/staffs.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/spiders/transfermarkt/team.py` & `fusion_stat-0.0.9/fusion_stat/spiders/transfermarkt/team.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/fusion_stat/utils.py` & `fusion_stat-0.0.9/fusion_stat/utils.py`

 * *Files identical despite different names*

### Comparing `fusion_stat-0.0.8/pyproject.toml` & `fusion_stat-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fusion-stat"
-version = "0.0.8"
+version = "0.0.9"
 description = "Scrape football data from multiple sources simultaneously."
 authors = ["tanzhijian <tanzhijianorg@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "fusion_stat"}]
 homepage = "https://github.com/tanzhijian/fusion-stat"
 repository = "https://github.com/tanzhijian/fusion-stat"
```

### Comparing `fusion_stat-0.0.8/PKG-INFO` & `fusion_stat-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fusion-stat
-Version: 0.0.8
+Version: 0.0.9
 Summary: Scrape football data from multiple sources simultaneously.
 Home-page: https://github.com/tanzhijian/fusion-stat
 License: MIT
 Author: tanzhijian
 Author-email: tanzhijianorg@outlook.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
```

