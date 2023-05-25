# Comparing `tmp/spotify_codegen-0.3.2.tar.gz` & `tmp/spotify_codegen-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_codegen-0.3.2.tar", max compression
+gzip compressed data, was "spotify_codegen-0.3.3.tar", max compression
```

## Comparing `spotify_codegen-0.3.2.tar` & `spotify_codegen-0.3.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-01-11 19:59:53.784615 spotify_codegen-0.3.2/LICENSE
--rw-r--r--   0        0        0     3253 2023-01-11 19:59:53.784615 spotify_codegen-0.3.2/README.md
--rw-r--r--   0        0        0     2174 2023-01-11 20:00:04.880557 spotify_codegen-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       23 2023-01-11 19:59:53.788615 spotify_codegen-0.3.2/src/spotifycodegen/__init__.py
--rw-r--r--   0        0        0     3142 2023-01-11 19:59:53.788615 spotify_codegen-0.3.2/src/spotifycodegen/cli.py
--rw-r--r--   0        0        0     7876 2023-01-11 19:59:53.788615 spotify_codegen-0.3.2/src/spotifycodegen/main.py
--rw-r--r--   0        0        0        0 2023-01-11 19:59:53.788615 spotify_codegen-0.3.2/src/spotifycodegen/py.typed
--rw-r--r--   0        0        0     4295 1970-01-01 00:00:00.000000 spotify_codegen-0.3.2/setup.py
--rw-r--r--   0        0        0     4308 1970-01-01 00:00:00.000000 spotify_codegen-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-25 16:44:36.705545 spotify_codegen-0.3.3/LICENSE
+-rw-r--r--   0        0        0     3253 2023-05-25 16:44:36.705545 spotify_codegen-0.3.3/README.md
+-rw-r--r--   0        0        0     2174 2023-05-25 16:45:01.570654 spotify_codegen-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-25 16:44:36.709545 spotify_codegen-0.3.3/src/spotifycodegen/__init__.py
+-rw-r--r--   0        0        0     3166 2023-05-25 16:44:36.709545 spotify_codegen-0.3.3/src/spotifycodegen/cli.py
+-rw-r--r--   0        0        0     7876 2023-05-25 16:44:36.709545 spotify_codegen-0.3.3/src/spotifycodegen/main.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:44:36.709545 spotify_codegen-0.3.3/src/spotifycodegen/py.typed
+-rw-r--r--   0        0        0     4308 1970-01-01 00:00:00.000000 spotify_codegen-0.3.3/PKG-INFO
```

### Comparing `spotify_codegen-0.3.2/LICENSE` & `spotify_codegen-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_codegen-0.3.2/README.md` & `spotify_codegen-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `spotify_codegen-0.3.2/pyproject.toml` & `spotify_codegen-0.3.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotify-codegen"
-version = "0.3.2"
+version = "0.3.3"
 description = "spotify-codegen"
 authors = ["Til Schünemann <til.schuenemann@mailbox.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tilschuenemann/spotify-codegen"
 repository = "https://github.com/tilschuenemann/spotify-codegen"
 documentation = "https://spotify-codegen.readthedocs.io"
```

### Comparing `spotify_codegen-0.3.2/src/spotifycodegen/cli.py` & `spotify_codegen-0.3.3/src/spotifycodegen/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         path_type=Path,
         exists=True,
         file_okay=False,
         dir_okay=True,
         writable=True,
         readable=True,
     ),
+    default=Path.cwd(),
     help="Output directory where files get written to.",
 )
 @click.pass_context
 def cli(ctx: Context, output_dir: Path) -> None:
     """Used for passing context."""
     ctx.ensure_object(dict)
     ctx.obj["output_dir"] = output_dir
```

### Comparing `spotify_codegen-0.3.2/src/spotifycodegen/main.py` & `spotify_codegen-0.3.3/src/spotifycodegen/main.py`

 * *Files identical despite different names*

### Comparing `spotify_codegen-0.3.2/setup.py` & `spotify_codegen-0.3.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: spotify-codegen
+Version: 0.3.3
+Summary: spotify-codegen
+Home-page: https://github.com/tilschuenemann/spotify-codegen
+License: MIT
+Keywords: spotify-codegen,spoticode,spotify,spotipy,art,code,qr,album,track,song,album,generator
+Author: Til Schünemann
+Author-email: til.schuenemann@mailbox.org
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.0.1)
+Requires-Dist: colorthief (>=0.2.1,<0.3.0)
+Requires-Dist: pillow (>=9.3.0,<10.0.0)
+Requires-Dist: spotipy (>=2.21.0,<3.0.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Project-URL: Changelog, https://github.com/tilschuenemann/spotify-codegen/releases
+Project-URL: Documentation, https://spotify-codegen.readthedocs.io
+Project-URL: Repository, https://github.com/tilschuenemann/spotify-codegen
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# spotify-codegen
 
-packages = \
-['spotifycodegen']
+[![PyPI](https://img.shields.io/pypi/v/spotify-codegen.svg)][pypi_]
+[![Status](https://img.shields.io/pypi/status/spotify-codegen.svg)][status]
+[![Python Version](https://img.shields.io/pypi/pyversions/spotify-codegen)][python version]
+[![License](https://img.shields.io/pypi/l/spotify-codegen)][license]
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.0.1',
- 'colorthief>=0.2.1,<0.3.0',
- 'pillow>=9.3.0,<10.0.0',
- 'spotipy>=2.21.0,<3.0.0',
- 'tqdm>=4.64.1,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['spotifycodegen = spotifycodegen.cli:cli']}
-
-setup_kwargs = {
-    'name': 'spotify-codegen',
-    'version': '0.3.2',
-    'description': 'spotify-codegen',
-    'long_description': '# spotify-codegen\n\n[![PyPI](https://img.shields.io/pypi/v/spotify-codegen.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/spotify-codegen.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/spotify-codegen)][python version]\n[![License](https://img.shields.io/pypi/l/spotify-codegen)][license]\n\n[![Read the documentation at https://spotify-codegen.readthedocs.io/](https://img.shields.io/readthedocs/spotify-codegen/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/tilschuenemann/spotify-codegen/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/tilschuenemann/spotify-codegen/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/spotify-codegen/\n[status]: https://pypi.org/project/spotify-codegen/\n[python version]: https://pypi.org/project/spotify-codegen\n[read the docs]: https://spotify-codegen.readthedocs.io/\n[tests]: https://github.com/tilschuenemann/spotify-codegen/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/tilschuenemann/spotify-codegen\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\nSpotify removed the feature to get a stitched image of an album / artist / track cover with their own Spotify Code. This package mimicks that behaviour and creates stitches, based on supplied\n\n- URL\n- URI\n- query\n\nIt\'s also possible to use create stitches for:\n\n- all saved albums\n- 50 followed artists (limit imposed by Spotify API)\n\n[You can also try the Streamlit showcase here.](https://tilschuenemann-showcase-showcasesstart-0ndtb3.streamlit.app/spotify_codegen)\n\n## Requirements\n\nYou\'ll need to have a Spotify Client ID & Secret in order to make API requests. Specify as environment variable like this:\n\n```console\n$ export SPOTIPY_CLIENT_ID="your_client_id"\n$ export SPOTIPY_CLIENT_ID="your_client_secret"\n```\n\n## Installation\n\nYou can install _spotify-codegen_ via [pip] from [PyPI]:\n\n```console\n$ pip install spotify-codegen\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_spotify-codegen_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/tilschuenemann/spotify-codegen/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/tilschuenemann/spotify-codegen/blob/main/LICENSE\n[contributor guide]: https://github.com/tilschuenemann/spotify-codegen/blob/main/CONTRIBUTING.md\n[command-line reference]: https://spotify-codegen.readthedocs.io/en/latest/usage.html\n',
-    'author': 'Til Schünemann',
-    'author_email': 'til.schuenemann@mailbox.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/tilschuenemann/spotify-codegen',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+[![Read the documentation at https://spotify-codegen.readthedocs.io/](https://img.shields.io/readthedocs/spotify-codegen/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/tilschuenemann/spotify-codegen/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/tilschuenemann/spotify-codegen/branch/main/graph/badge.svg)][codecov]
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi_]: https://pypi.org/project/spotify-codegen/
+[status]: https://pypi.org/project/spotify-codegen/
+[python version]: https://pypi.org/project/spotify-codegen
+[read the docs]: https://spotify-codegen.readthedocs.io/
+[tests]: https://github.com/tilschuenemann/spotify-codegen/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/tilschuenemann/spotify-codegen
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
+
+## Features
+
+Spotify removed the feature to get a stitched image of an album / artist / track cover with their own Spotify Code. This package mimicks that behaviour and creates stitches, based on supplied
+
+- URL
+- URI
+- query
+
+It's also possible to use create stitches for:
+
+- all saved albums
+- 50 followed artists (limit imposed by Spotify API)
+
+[You can also try the Streamlit showcase here.](https://tilschuenemann-showcase-showcasesstart-0ndtb3.streamlit.app/spotify_codegen)
+
+## Requirements
+
+You'll need to have a Spotify Client ID & Secret in order to make API requests. Specify as environment variable like this:
+
+```console
+$ export SPOTIPY_CLIENT_ID="your_client_id"
+$ export SPOTIPY_CLIENT_ID="your_client_secret"
+```
+
+## Installation
+
+You can install _spotify-codegen_ via [pip] from [PyPI]:
+
+```console
+$ pip install spotify-codegen
+```
+
+## Usage
+
+Please see the [Command-line Reference] for details.
+
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## License
+
+Distributed under the terms of the [MIT license][license],
+_spotify-codegen_ is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+
+[@cjolowicz]: https://github.com/cjolowicz
+[pypi]: https://pypi.org/
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[file an issue]: https://github.com/tilschuenemann/spotify-codegen/issues
+[pip]: https://pip.pypa.io/
+
+<!-- github-only -->
+
+[license]: https://github.com/tilschuenemann/spotify-codegen/blob/main/LICENSE
+[contributor guide]: https://github.com/tilschuenemann/spotify-codegen/blob/main/CONTRIBUTING.md
+[command-line reference]: https://spotify-codegen.readthedocs.io/en/latest/usage.html
 
-setup(**setup_kwargs)
```

