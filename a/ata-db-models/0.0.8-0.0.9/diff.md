# Comparing `tmp/ata-db-models-0.0.8.tar.gz` & `tmp/ata-db-models-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ata-db-models-0.0.8.tar", max compression
+gzip compressed data, was "ata-db-models-0.0.9.tar", max compression
```

## Comparing `ata-db-models-0.0.8.tar` & `ata-db-models-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2022-12-01 20:58:47.527310 ata-db-models-0.0.8/LICENSE
--rw-r--r--   0        0        0     5087 2022-12-01 20:58:47.527310 ata-db-models-0.0.8/README.md
--rw-r--r--   0        0        0        0 2022-12-01 20:58:47.527310 ata-db-models-0.0.8/ata_db_models/__init__.py
--rw-r--r--   0        0        0     5224 2022-12-01 20:58:47.527310 ata-db-models-0.0.8/ata_db_models/helpers.py
--rw-r--r--   0        0        0     3067 2022-12-01 20:58:47.527310 ata-db-models-0.0.8/ata_db_models/init_db.py
--rw-r--r--   0        0        0     3395 2022-12-01 20:58:47.527310 ata-db-models-0.0.8/ata_db_models/models.py
--rw-r--r--   0        0        0     1114 2022-12-01 20:58:47.531310 ata-db-models-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5951 2022-12-01 20:58:57.719951 ata-db-models-0.0.8/setup.py
--rw-r--r--   0        0        0     5733 2022-12-01 20:58:57.720596 ata-db-models-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-12-01 21:13:15.085053 ata-db-models-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5087 2022-12-01 21:13:15.085053 ata-db-models-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2022-12-01 21:13:15.085053 ata-db-models-0.0.9/ata_db_models/__init__.py
+-rw-r--r--   0        0        0     5224 2022-12-01 21:13:15.085053 ata-db-models-0.0.9/ata_db_models/helpers.py
+-rw-r--r--   0        0        0     3067 2022-12-01 21:13:15.085053 ata-db-models-0.0.9/ata_db_models/init_db.py
+-rw-r--r--   0        0        0     3425 2022-12-01 21:13:15.085053 ata-db-models-0.0.9/ata_db_models/models.py
+-rw-r--r--   0        0        0     1114 2022-12-01 21:13:15.085053 ata-db-models-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5951 2022-12-01 21:13:23.362026 ata-db-models-0.0.9/setup.py
+-rw-r--r--   0        0        0     5733 2022-12-01 21:13:23.362360 ata-db-models-0.0.9/PKG-INFO
```

### Comparing `ata-db-models-0.0.8/LICENSE` & `ata-db-models-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ata-db-models-0.0.8/README.md` & `ata-db-models-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ata-db-models-0.0.8/ata_db_models/helpers.py` & `ata-db-models-0.0.9/ata_db_models/helpers.py`

 * *Files identical despite different names*

### Comparing `ata-db-models-0.0.8/ata_db_models/init_db.py` & `ata-db-models-0.0.9/ata_db_models/init_db.py`

 * *Files identical despite different names*

### Comparing `ata-db-models-0.0.8/ata_db_models/models.py` & `ata-db-models-0.0.9/ata_db_models/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 from typing import Optional, Union
 from uuid import UUID
 
 from pydantic import HttpUrl
-from sqlmodel import Column, Field, JSON, SQLModel, String
+from sqlmodel import JSON, Column, Field, SQLModel, String
 
 
 class Event(SQLModel, table=True):
     # TODO make enum
     site_name: str = Field(primary_key=True)
     # Timestamp making allowance for inaccurate device clock
     derived_tstamp: datetime
@@ -42,18 +42,18 @@
     # TODO consider making this an enum
     refr_medium: str
     # Name of referer if recognised, e.g., "Google" or "Bing"
     refr_source: Optional[str] = None
     # Data/attributes of HTML input and its form in JSON format. Only present if event_name == "change_form"
     # (read: https://github.com/snowplow/iglu-central/blob/master/schemas/com.snowplowanalytics.snowplow/change_form/jsonschema/1-0-0)
     # TODO probably optional and json
-    unstruct_event_com_snowplowanalytics_snowplow_change_form_1: Union[list, dict] = Field(sa_column=Column(JSON))  # type: ignore
+    unstruct_event_com_snowplowanalytics_snowplow_change_form_1: Optional[Union[list, dict]] = Field(sa_column=Column(JSON))  # type: ignore
     # Data/attributes of HTML input and its form in JSON format. Only present if event_name == "focus_form"
     # (read: https://github.com/snowplow/iglu-central/blob/master/schemas/com.snowplowanalytics.snowplow/focus_form/jsonschema/1-0-0)
     # TODO probably optional and json
-    unstruct_event_com_snowplowanalytics_snowplow_focus_form_1: Union[list, dict] = Field(sa_column=Column(JSON))  # type: ignore
+    unstruct_event_com_snowplowanalytics_snowplow_focus_form_1: Optional[Union[list, dict]] = Field(sa_column=Column(JSON))  # type: ignore
     # Data/attributes of HTML form and all its inputs in JSON format. Only present if event_name == "submit_form"
     # (read: https://github.com/snowplow/iglu-central/blob/master/schemas/com.snowplowanalytics.snowplow/submit_form/jsonschema/1-0-0)
     # TODO probably optional and json
-    unstruct_event_com_snowplowanalytics_snowplow_submit_form_1: Union[list, dict] = Field(sa_column=Column(JSON))  # type: ignore
+    unstruct_event_com_snowplowanalytics_snowplow_submit_form_1: Optional[Union[list, dict]] = Field(sa_column=Column(JSON))  # type: ignore
     # Raw useragent
     useragent: str
```

### Comparing `ata-db-models-0.0.8/pyproject.toml` & `ata-db-models-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ata-db-models"
-version = "0.0.8"
+version = "0.0.9"
 description = "Database models and migrations for Automating the Ask."
 authors = ["Raaid Arshad <raaid@protonmail.com>"]
 repository = "https://github.com/LocalAtBrown/ata-models"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.10"
```

### Comparing `ata-db-models-0.0.8/setup.py` & `ata-db-models-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'boto3-stubs[ssm]==1.26.13',
  'boto3==1.26.13',
  'psycopg2==2.9.5',
  'sqlmodel==0.0.8']
 
 setup_kwargs = {
     'name': 'ata-db-models',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Database models and migrations for Automating the Ask.',
     'long_description': "# ata-db-models\n\n<!-- [![Release](https://img.shields.io/github/v/release/LocalAtBrown/ata-db-models)](https://img.shields.io/github/v/release/LocalAtBrown/ata-db-models) -->\n<!-- [![Build status](https://img.shields.io/github/workflow/status/LocalAtBrown/ata-db-models/merge-to-main)](https://img.shields.io/github/workflow/status/LocalAtBrown/ata-db-models/merge-to-main) -->\n\n[![Python version](https://img.shields.io/badge/python_version-3.9-blue)](https://github.com/psf/black)\n[![Code style with black](https://img.shields.io/badge/code_style-black-000000.svg)](https://github.com/psf/black)\n[![More style with flake8](https://img.shields.io/badge/code_style-flake8-blue)](https://flake8.pycqa.org)\n[![Imports with isort](https://img.shields.io/badge/%20imports-isort-blue)](https://pycqa.github.io/isort/)\n[![Type checking with mypy](https://img.shields.io/badge/type_checker-mypy-blue)](https://mypy.readthedocs.io)\n[![License](https://img.shields.io/github/license/LocalAtBrown/ata-db-models)](https://img.shields.io/github/license/LocalAtBrown/ata-db-models)\n\nDatabase models and migrations for Automating the Ask.\n\n## Usage\n\n### As a package\n\nWe use [SQLModel](https://sqlmodel.tiangolo.com/), a layer on top of SQLAlchemy with Pydantic, to define our tables.\nThis is useful because we can import this package to interact with the tables AND have Pydantic objects in Python\nthat correspond to a row in the table.\n\nTo install the package from PyPi, run: `pip install ata-db-models`. Check existing versions \n[here](https://pypi.org/project/ata-db-models/).\n\n### Initialize a new cluster\n\nIf you want to initialize a fresh database cluster, pass in the env vars to connect to the cluster and run `init_db`.\nIf the target cluster has IP restrictions, make sure your IP address is a valid access point.\n\nAn example run with fake credentials (from the root dir of this project with the virtual env\nactivated):\n`HOST=fakehost USER=fakeuser PASSWORD=fakepw DB_NAME=postgres python src/init_db.py`\n\nNo `PORT` is passed because the default port is 5432, the standard for Postgres.\n\n### Migrations\n\nSo you made some changes to what tables there are, what columns there are, indices, etc. and you'd like to\nupdate the databases. This is what alembic is for!\n\n TODO ALEMBIC INSTRUCTIONS\n\n## Development\n\nThis project uses [Poetry](https://python-poetry.org/) to manage dependencies. It also helps with pinning dependency and python\nversions. We also use [pre-commit](https://pre-commit.com/) with hooks for [isort](https://pycqa.github.io/isort/),\n[black](https://github.com/psf/black), and [flake8](https://flake8.pycqa.org/en/latest/) for consistent code style and\nreadability. Note that this means code that doesn't meet the rules will fail to commit until it is fixed.\n\nWe use [mypy](https://mypy.readthedocs.io/en/stable/index.html) for static type checking. This can be run [manually](#run-static-type-checking),\nand the CI runs it on PRs to the `main` branch. We also use [pytest](https://docs.pytest.org/en/7.2.x/) to run our tests.\nThis can be run [manually](#run-tests) and the CI runs it on PRs to the `main` branch.\n\n### Setup\n\n1. [Install Poetry](https://python-poetry.org/docs/#installation).\n2. Run `poetry install --no-root`\n3. Run `source $(poetry env list --full-path)/bin/activate && pre-commit install && deactivate` to set up `pre-commit`\n\nYou're all set up! Your local environment should include all dependencies, including dev dependencies like `black`.\nThis is done with Poetry via the `poetry.lock` file.\n\n### Run Code Format and Linting\n\nTo manually run isort, black, and flake8 all in one go, simply run `pre-commit run --all-files`. Explore the `pre-commit` docs (linked above)\nto see more options.\n\n### Run Static Type Checking\n\nTo manually run mypy, simply run `mypy` from the root directory of the project. It will use the default configuration\nspecified in `pyproject.toml`.\n\n### Update Dependencies\n\nTo update dependencies in your local environment, make changes to the `pyproject.toml` file then run `poetry update` from the root directory of the project.\n\n### Run Tests\n\nTo manually run rests, you need to have a Postgres instance running locally on port 5432. One way to do this\nis to run a Docker container, then run the tests while it is active.\n\n1. (If you don't already have the image locally) Run `docker pull postgres`\n2. Run `docker run --rm --name postgres -e POSTGRES_PASSWORD=postgres -e POSTGRES_HOST_AUTH_METHOD=trust -p 127.0.0.1:5432:5432/tcp postgres`\n3. Run `DB_NAME=postgres pytest tests` from the root directory of the project. Explore the `pytest` docs (linked above)\nto see more options.\n\nNote that if you decide to run the Postgres container with different credentials (a different password, port, etc.) or\nvia a different method, you will likely need to update the test file to point to the correct Postgres instance.\n\nAdditionally, if you want to re-run the tests, you want to make sure you start over from a fresh Postgres\ninstance. If you run Postgres via Docker, you can simply `ctrl-C` to stop the image and start a new one.\n",
     'author': 'Raaid Arshad',
     'author_email': 'raaid@protonmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/LocalAtBrown/ata-models',
```

### Comparing `ata-db-models-0.0.8/PKG-INFO` & `ata-db-models-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ata-db-models
-Version: 0.0.8
+Version: 0.0.9
 Summary: Database models and migrations for Automating the Ask.
 Home-page: https://github.com/LocalAtBrown/ata-models
 Author: Raaid Arshad
 Author-email: raaid@protonmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

