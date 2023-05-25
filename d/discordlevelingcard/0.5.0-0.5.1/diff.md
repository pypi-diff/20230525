# Comparing `tmp/discordlevelingcard-0.5.0.tar.gz` & `tmp/discordlevelingcard-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordlevelingcard-0.5.0.tar", max compression
+gzip compressed data, was "discordlevelingcard-0.5.1.tar", max compression
```

## Comparing `discordlevelingcard-0.5.0.tar` & `discordlevelingcard-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       71 2023-01-08 10:51:38.071812 discordlevelingcard-0.5.0/DiscordLevelingCard/__init__.py
--rw-r--r--   0        0        0      842 2023-01-08 10:51:38.071812 discordlevelingcard-0.5.0/DiscordLevelingCard/assets/curveborder.png
--rw-r--r--   0        0        0     2596 2023-01-08 10:51:38.071812 discordlevelingcard-0.5.0/DiscordLevelingCard/assets/curvedoverlay.png
--rw-r--r--   0        0        0    60288 2023-01-08 10:51:38.103076 discordlevelingcard-0.5.0/DiscordLevelingCard/assets/levelfont.otf
--rw-r--r--   0        0        0     9742 2023-01-08 10:51:38.118707 discordlevelingcard-0.5.0/DiscordLevelingCard/assets/mask_circle.jpg
--rw-r--r--   0        0        0     6394 2023-01-08 10:51:38.118707 discordlevelingcard-0.5.0/DiscordLevelingCard/assets/overlay1.png
--rw-r--r--   0        0        0     2590 2023-01-24 08:45:29.025994 discordlevelingcard-0.5.0/DiscordLevelingCard/card_settings.py
--rw-r--r--   0        0        0    11232 2023-04-25 07:23:06.420282 discordlevelingcard-0.5.0/DiscordLevelingCard/discord_card.py
--rw-r--r--   0        0        0      531 2023-01-08 10:51:38.212709 discordlevelingcard-0.5.0/DiscordLevelingCard/error.py
--rw-r--r--   0        0        0     1083 2023-01-08 11:22:52.135512 discordlevelingcard-0.5.0/LICENSE
--rw-r--r--   0        0        0      888 2023-04-25 07:23:44.291549 discordlevelingcard-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4387 2023-04-25 07:22:29.870410 discordlevelingcard-0.5.0/README.md
--rw-r--r--   0        0        0     5189 2023-04-25 07:26:46.867985 discordlevelingcard-0.5.0/setup.py
--rw-r--r--   0        0        0     5127 2023-04-25 07:26:46.867985 discordlevelingcard-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-04-25 08:29:49.128624 discordlevelingcard-0.5.1/DiscordLevelingCard/__init__.py
+-rw-r--r--   0        0        0      842 2023-04-25 08:29:49.129344 discordlevelingcard-0.5.1/DiscordLevelingCard/assets/curveborder.png
+-rw-r--r--   0        0        0     2596 2023-04-25 08:29:49.129826 discordlevelingcard-0.5.1/DiscordLevelingCard/assets/curvedoverlay.png
+-rw-r--r--   0        0        0    60288 2023-04-25 08:29:49.131350 discordlevelingcard-0.5.1/DiscordLevelingCard/assets/levelfont.otf
+-rw-r--r--   0        0        0     9742 2023-04-25 08:29:49.132354 discordlevelingcard-0.5.1/DiscordLevelingCard/assets/mask_circle.jpg
+-rw-r--r--   0        0        0     6394 2023-04-25 08:29:49.133294 discordlevelingcard-0.5.1/DiscordLevelingCard/assets/overlay1.png
+-rw-r--r--   0        0        0     2590 2023-04-25 08:29:49.133788 discordlevelingcard-0.5.1/DiscordLevelingCard/card_settings.py
+-rw-r--r--   0        0        0    11379 2023-05-25 16:51:31.035219 discordlevelingcard-0.5.1/DiscordLevelingCard/discord_card.py
+-rw-r--r--   0        0        0      531 2023-04-25 08:29:49.134664 discordlevelingcard-0.5.1/DiscordLevelingCard/error.py
+-rw-r--r--   0        0        0     1083 2023-04-25 08:29:49.135173 discordlevelingcard-0.5.1/LICENSE
+-rw-r--r--   0        0        0      888 2023-05-25 16:42:13.533780 discordlevelingcard-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4528 2023-05-25 16:47:49.247493 discordlevelingcard-0.5.1/README.md
+-rw-r--r--   0        0        0     5330 2023-05-25 17:00:53.936697 discordlevelingcard-0.5.1/setup.py
+-rw-r--r--   0        0        0     5264 2023-05-25 17:00:53.936697 discordlevelingcard-0.5.1/PKG-INFO
```

### Comparing `discordlevelingcard-0.5.0/DiscordLevelingCard/assets/curveborder.png` & `discordlevelingcard-0.5.1/DiscordLevelingCard/assets/curveborder.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.0/DiscordLevelingCard/assets/curvedoverlay.png` & `discordlevelingcard-0.5.1/DiscordLevelingCard/assets/curvedoverlay.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.0/DiscordLevelingCard/assets/levelfont.otf` & `discordlevelingcard-0.5.1/DiscordLevelingCard/assets/levelfont.otf`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.0/DiscordLevelingCard/assets/mask_circle.jpg` & `discordlevelingcard-0.5.1/DiscordLevelingCard/assets/mask_circle.jpg`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.0/DiscordLevelingCard/assets/overlay1.png` & `discordlevelingcard-0.5.1/DiscordLevelingCard/assets/overlay1.png`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.0/DiscordLevelingCard/card_settings.py` & `discordlevelingcard-0.5.1/DiscordLevelingCard/card_settings.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.0/DiscordLevelingCard/discord_card.py` & `discordlevelingcard-0.5.1/DiscordLevelingCard/discord_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,15 +159,16 @@
             print(e)
             new.paste(self.avatar, (0,0))
         self.background.paste(new, (13, 65), mask_im)
 
         im = Image.new("RGB", (490, 51), (0, 0, 0))
         draw = ImageDraw.Draw(im, "RGBA")
         draw.rounded_rectangle((0, 0, 420, 50), 30, fill=(255,255,255,50))
-        draw.rounded_rectangle((0, 0, bar_exp, 50), 30, fill=self.bar_color)
+        if self.current_exp != 0:
+            draw.rounded_rectangle((0, 0, bar_exp, 50), 30, fill=self.bar_color)
         self.background.paste(im, (190, 235))
         new = Image.new("RGBA", self.background.size)
         new.paste(self.background,(0, 0), Image.open(path + "/assets/curvedoverlay.png").convert("L"))
         self.background = new.resize((505, 259))
 
         image = BytesIO()
         self.background.save(image, 'PNG')
@@ -224,15 +225,18 @@
         bar_exp = (self.current_exp/self.max_exp)*619
         if bar_exp <= 50:
             bar_exp = 50  
 
         im = Image.new("RGB", (620, 51), "#2f3136")
         draw = ImageDraw.Draw(im, "RGBA")
         draw.rounded_rectangle((0, 0, 619, 50), 30, fill=(255,255,255,50))
-        draw.rounded_rectangle((0, 0, bar_exp, 50), 30, fill=self.bar_color)
+        
+        if self.current_exp != 0:
+            draw.rounded_rectangle((0, 0, bar_exp, 50), 30, fill=self.bar_color)
+        
         background.paste(im, (330, 235))
 
         image = BytesIO()
         background.save(image, 'PNG')
         image.seek(0)
         return image
 
@@ -285,14 +289,16 @@
         bar_exp = (self.current_exp/self.max_exp)*619
         if bar_exp <= 50:
             bar_exp = 50  
 
         im = Image.new("RGBA", (620, 51))
         draw = ImageDraw.Draw(im, "RGBA")
         draw.rounded_rectangle((0, 0, 619, 50), 30, fill=(255,255,255,225))
-        draw.rounded_rectangle((0, 0, bar_exp, 50), 30, fill=self.bar_color)
+        if self.current_exp != 0:
+            draw.rounded_rectangle((0, 0, bar_exp, 50), 30, fill=self.bar_color)
+        
         background.paste(im, (330, 235), im.convert("RGBA"))
 
         image = BytesIO()
         background.save(image, 'PNG')
         image.seek(0)
         return image
```

### Comparing `discordlevelingcard-0.5.0/DiscordLevelingCard/error.py` & `discordlevelingcard-0.5.1/DiscordLevelingCard/error.py`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.0/LICENSE` & `discordlevelingcard-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discordlevelingcard-0.5.0/pyproject.toml` & `discordlevelingcard-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "discordlevelingcard"
-version = "0.5.0"
+version = "0.5.1"
 readme = "README.md"
 description = "A library with leveling cards for your discord bot."
 repository = "https://github.com/krishsharma0413/DiscordLevelingCard"
 authors = ["Reset <krishsharma0413@gmail.com>"]
 license = "MIT"
 keywords = [
     "discord", "leveling", "card",
```

### Comparing `discordlevelingcard-0.5.0/README.md` & `discordlevelingcard-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -199,8 +199,12 @@
 ![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)
 
 <br>
 
 </details>
 
 <br><br>
+
+if you want to see changelog then click [here](https://github.com/krishsharma0413/DiscordLevelingCard/blob/main/CHANGELOG.md)
+
+<br><br>
 please star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D
```

### Comparing `discordlevelingcard-0.5.0/setup.py` & `discordlevelingcard-0.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'DiscordLevelingCard': ['assets/*']}
 
 install_requires = \
 ['Pillow>=9.2.0,<10.0.0', 'aiohttp>=3.8.1,<4.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'discordlevelingcard',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'A library with leveling cards for your discord bot.',
-    'long_description': '# DiscordLevelingCard\nA library with Rank cards for your discord bot.\n\n[![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)\n\n## card preview\n\n`card1`\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n\n`card2`\n![card2](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n\n`card3` *same as card2 but with background*\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n## installation\n\n`for pypi version`\n```sh\npip install discordlevelingcard\n```\n\n`for github developement version`\n```sh\npip install git+https://github.com/krishsharma0413/DiscordLevelingCard\n```\n\n## How To Use\n\nIf you don\'t provide `path` then the method will return `bytes` which can directly be used in discord.py/disnake/pycord/nextcord \'s `File class`.\n\n\n<br>\n\n\n## Example\n\n`since no path was provided, it returns bytes which can directly be used in discord.py and its fork\'s File class.`\n\n```py\nfrom disnake.ext import commands\nfrom DiscordLevelingCard import RankCard, Settings\nimport disnake\n\nclient = commands.Bot()\n# define background, bar_color, text_color at one place\ncard_settings = Settings(\n    background="url or path to background image",\n    text_color="white",\n    bar_color="#000000"\n)\n\n@client.slash_command(name="rank")\nasync def user_rank_card(ctx, user:disnake.Member):\n    await ctx.response.defer()\n    a = RankCard(\n        settings=card_settings,\n        avatar=user.display_avatar.url,\n        level=1,\n        current_exp=1,\n        max_exp=1,\n        username="cool username"\n    )\n    image = await a.card1()\n    await ctx.edit_original_message(file=disnake.File(image, filename="rank.png")) # providing filename is very important\n\n```\n\n<br>\n\n## Documentation\n\n\n<details>\n\n<summary> <span style="color:yellow">RankCard</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">Settings</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nSettings(\n    background: Union[PathLike, BufferedIOBase, str],\n    bar_color: Optional[str] = \'white\',\n    text_color: Optional[str] = \'white\',\n    background_color: Optional[str]= "#36393f"\n\n)\n```\n\n- `background` - background image url or file-object in `rb` mode.\n  - `4:1` aspect ratio recommended.\n\n- `bar_color` - color of the bar [example: "white" or "#000000"]\n\n- `text_color` - color of the text [example: "white" or "#000000"]\n\n- `background_color` - color of the background [example: "white" or "#000000"]\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card1</span> method</summary>\n\n\n```py\nRankCard.card1()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card2</span> method</summary>\n\n\n```py\nRankCard.card2()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card3</span> method</summary>\n\n\n```py\nRankCard.card3()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n</details>\n\n<br><br>\nplease star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D\n',
+    'long_description': '# DiscordLevelingCard\nA library with Rank cards for your discord bot.\n\n[![Downloads](https://pepy.tech/badge/discordlevelingcard)](https://pepy.tech/project/discordlevelingcard)\n\n## card preview\n\n`card1`\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n\n`card2`\n![card2](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n\n`card3` *same as card2 but with background*\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n## installation\n\n`for pypi version`\n```sh\npip install discordlevelingcard\n```\n\n`for github developement version`\n```sh\npip install git+https://github.com/krishsharma0413/DiscordLevelingCard\n```\n\n## How To Use\n\nIf you don\'t provide `path` then the method will return `bytes` which can directly be used in discord.py/disnake/pycord/nextcord \'s `File class`.\n\n\n<br>\n\n\n## Example\n\n`since no path was provided, it returns bytes which can directly be used in discord.py and its fork\'s File class.`\n\n```py\nfrom disnake.ext import commands\nfrom DiscordLevelingCard import RankCard, Settings\nimport disnake\n\nclient = commands.Bot()\n# define background, bar_color, text_color at one place\ncard_settings = Settings(\n    background="url or path to background image",\n    text_color="white",\n    bar_color="#000000"\n)\n\n@client.slash_command(name="rank")\nasync def user_rank_card(ctx, user:disnake.Member):\n    await ctx.response.defer()\n    a = RankCard(\n        settings=card_settings,\n        avatar=user.display_avatar.url,\n        level=1,\n        current_exp=1,\n        max_exp=1,\n        username="cool username"\n    )\n    image = await a.card1()\n    await ctx.edit_original_message(file=disnake.File(image, filename="rank.png")) # providing filename is very important\n\n```\n\n<br>\n\n## Documentation\n\n\n<details>\n\n<summary> <span style="color:yellow">RankCard</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nRankCard(\n    settings: Settings,\n    avatar:str,\n    level:int,\n    current_exp:int,\n    max_exp:int,\n    username:str,\n    rank: Optional[int] = None\n)\n```\n\n- `settings` - Settings class from DiscordLevelingCard.\n\n- `avatar` - avatar image url.\n\n- `level` - level of the user.\n\n- `current_exp` - current exp of the user.\n\n- `max_exp` - max exp of the user.\n\n- `username` - username of the user.\n\n- `rank` - rank of the user. (optional)\n\n</details>\n\n<details>\n\n<summary> <span style="color:yellow">Settings</span> class</summary>\n\n<br>\n\n`__init__` method\n\n```py\nSettings(\n    background: Union[PathLike, BufferedIOBase, str],\n    bar_color: Optional[str] = \'white\',\n    text_color: Optional[str] = \'white\',\n    background_color: Optional[str]= "#36393f"\n\n)\n```\n\n- `background` - background image url or file-object in `rb` mode.\n  - `4:1` aspect ratio recommended.\n\n- `bar_color` - color of the bar [example: "white" or "#000000"]\n\n- `text_color` - color of the text [example: "white" or "#000000"]\n\n- `background_color` - color of the background [example: "white" or "#000000"]\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card1</span> method</summary>\n\n\n```py\nRankCard.card1()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card1](https://user-images.githubusercontent.com/77439837/234198272-3dcaabb0-0f38-4d51-9938-de4b0ad42123.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card2</span> method</summary>\n\n\n```py\nRankCard.card2()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card](https://user-images.githubusercontent.com/77439837/234198354-315e9420-9bd7-47bd-87ed-b21c3772646c.png)\n\n<br>\n\n</details>\n\n\n<details>\n\n<summary> <span style="color:yellow">card3</span> method</summary>\n\n\n```py\nRankCard.card3()\n```\n\n`returns` - `bytes` which can directly be used within `discord.File` class.\n\n\n\n![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)\n\n<br>\n\n</details>\n\n<br><br>\n\nif you want to see changelog then click [here](https://github.com/krishsharma0413/DiscordLevelingCard/blob/main/CHANGELOG.md)\n\n<br><br>\nplease star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D\n',
     'author': 'Reset',
     'author_email': 'krishsharma0413@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/krishsharma0413/DiscordLevelingCard',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `discordlevelingcard-0.5.0/PKG-INFO` & `discordlevelingcard-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordlevelingcard
-Version: 0.5.0
+Version: 0.5.1
 Summary: A library with leveling cards for your discord bot.
 Home-page: https://github.com/krishsharma0413/DiscordLevelingCard
 License: MIT
 Keywords: discord,leveling,card,image,discord.py,disnake,nextcord,rank,ranking,level,discord-bot,bot,discord-leveling,level-card,discord-leveling-card,discord-rank-card
 Author: Reset
 Author-email: krishsharma0413@gmail.com
 Requires-Python: >=3.8,<4
@@ -220,9 +220,13 @@
 ![card3](https://user-images.githubusercontent.com/77439837/234203410-a6a970ef-c01c-454b-be67-6dc7c1b2c807.png)
 
 <br>
 
 </details>
 
 <br><br>
+
+if you want to see changelog then click [here](https://github.com/krishsharma0413/DiscordLevelingCard/blob/main/CHANGELOG.md)
+
+<br><br>
 please star the <a href="https://github.com/krishsharma0413/DiscordLevelingCard">repository</a> if you like it :D
```

