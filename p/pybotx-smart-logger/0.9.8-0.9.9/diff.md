# Comparing `tmp/pybotx_smart_logger-0.9.8.tar.gz` & `tmp/pybotx_smart_logger-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotx_smart_logger-0.9.8.tar", max compression
+gzip compressed data, was "pybotx_smart_logger-0.9.9.tar", max compression
```

## Comparing `pybotx_smart_logger-0.9.8.tar` & `pybotx_smart_logger-0.9.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6421 2023-01-26 07:34:33.469405 pybotx_smart_logger-0.9.8/LICENSE
--rw-r--r--   0        0        0     6484 2023-01-26 07:34:33.469405 pybotx_smart_logger-0.9.8/README.md
--rw-r--r--   0        0        0      164 2023-01-26 07:34:33.469405 pybotx_smart_logger-0.9.8/pybotx_smart_logger/__init__.py
--rw-r--r--   0        0        0      840 2023-01-26 07:34:33.469405 pybotx_smart_logger-0.9.8/pybotx_smart_logger/contextvars.py
--rw-r--r--   0        0        0      174 2023-01-26 07:34:33.469405 pybotx_smart_logger-0.9.8/pybotx_smart_logger/log_levels.py
--rw-r--r--   0        0        0     1543 2023-01-26 07:34:33.469405 pybotx_smart_logger-0.9.8/pybotx_smart_logger/logger.py
--rw-r--r--   0        0        0        0 2023-01-26 07:34:33.469405 pybotx_smart_logger-0.9.8/pybotx_smart_logger/py.typed
--rw-r--r--   0        0        0      320 2023-01-26 07:34:33.469405 pybotx_smart_logger-0.9.8/pybotx_smart_logger/schemas.py
--rw-r--r--   0        0        0      942 2023-01-26 07:34:33.469405 pybotx_smart_logger-0.9.8/pybotx_smart_logger/wrapper.py
--rw-r--r--   0        0        0      661 2023-01-26 07:34:33.469405 pybotx_smart_logger-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     7349 1970-01-01 00:00:00.000000 pybotx_smart_logger-0.9.8/setup.py
--rw-r--r--   0        0        0     7011 1970-01-01 00:00:00.000000 pybotx_smart_logger-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     6421 2023-02-21 09:38:16.146391 pybotx_smart_logger-0.9.9/LICENSE
+-rw-r--r--   0        0        0     6484 2023-02-21 09:38:16.146391 pybotx_smart_logger-0.9.9/README.md
+-rw-r--r--   0        0        0      164 2023-02-21 09:38:16.150391 pybotx_smart_logger-0.9.9/pybotx_smart_logger/__init__.py
+-rw-r--r--   0        0        0      840 2023-02-21 09:38:16.150391 pybotx_smart_logger-0.9.9/pybotx_smart_logger/contextvars.py
+-rw-r--r--   0        0        0      174 2023-02-21 09:38:16.150391 pybotx_smart_logger-0.9.9/pybotx_smart_logger/log_levels.py
+-rw-r--r--   0        0        0     1543 2023-02-21 09:38:16.150391 pybotx_smart_logger-0.9.9/pybotx_smart_logger/logger.py
+-rw-r--r--   0        0        0        0 2023-02-21 09:38:16.150391 pybotx_smart_logger-0.9.9/pybotx_smart_logger/py.typed
+-rw-r--r--   0        0        0      320 2023-02-21 09:38:16.150391 pybotx_smart_logger-0.9.9/pybotx_smart_logger/schemas.py
+-rw-r--r--   0        0        0      942 2023-02-21 09:38:16.150391 pybotx_smart_logger-0.9.9/pybotx_smart_logger/wrapper.py
+-rw-r--r--   0        0        0      699 2023-02-21 09:38:16.150391 pybotx_smart_logger-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     7347 1970-01-01 00:00:00.000000 pybotx_smart_logger-0.9.9/setup.py
+-rw-r--r--   0        0        0     7009 1970-01-01 00:00:00.000000 pybotx_smart_logger-0.9.9/PKG-INFO
```

### Comparing `pybotx_smart_logger-0.9.8/LICENSE` & `pybotx_smart_logger-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotx_smart_logger-0.9.8/README.md` & `pybotx_smart_logger-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pybotx_smart_logger-0.9.8/pybotx_smart_logger/contextvars.py` & `pybotx_smart_logger-0.9.9/pybotx_smart_logger/contextvars.py`

 * *Files identical despite different names*

### Comparing `pybotx_smart_logger-0.9.8/pybotx_smart_logger/logger.py` & `pybotx_smart_logger-0.9.9/pybotx_smart_logger/logger.py`

 * *Files identical despite different names*

### Comparing `pybotx_smart_logger-0.9.8/pybotx_smart_logger/wrapper.py` & `pybotx_smart_logger-0.9.9/pybotx_smart_logger/wrapper.py`

 * *Files identical despite different names*

### Comparing `pybotx_smart_logger-0.9.8/pyproject.toml` & `pybotx_smart_logger-0.9.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "pybotx-smart-logger"
-version = "0.9.8"
+version = "0.9.9"
 description = "Shows logs when you need it"
 authors = ["Alexander Samoylenko <alexandr.samojlenko@ccsteam.ru>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 
-pybotx = ">=0.44.1,<0.55.0"
-
-fastapi = ">=0.70.0,<0.75.0"
-
+loguru = "^0.6.0"
+pydantic = "^1.10.5"
 
 [tool.poetry.dev-dependencies]
 add-trailing-comma = "2.2.3"
 autoflake = "1.4.0"
 black = "22.3.0"
 isort = "5.10.1"
 mypy = "0.910.0"
 wemake-python-styleguide = "0.16.1"
 bandit = "1.7.2"
 
 pytest = "^7.2.1"
 pytest-asyncio = "^0.18.1"
-pytest-cov = "^3.0.0"
+pytest-cov = "^4.0.0"
 requests = "^2.27.1"
 
+fastapi = ">=0.70.0,<0.93.0"
+pybotx = ">=0.44.1,<0.56.0"
+
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `pybotx_smart_logger-0.9.8/setup.py` & `pybotx_smart_logger-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['pybotx_smart_logger']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.70.0,<0.75.0', 'pybotx>=0.44.1,<0.55.0']
+['loguru>=0.6.0,<0.7.0', 'pydantic>=1.10.5,<2.0.0']
 
 setup_kwargs = {
     'name': 'pybotx-smart-logger',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Shows logs when you need it',
     'long_description': '# pybotx-smart-logger\n\n_Shows logs when you need it_\n\n\n## Проблема/решение\n\nВ основном наши боты работают в закрытых контурах. Там невозможно использовать Sentry,\nпоэтому наш главный помощник в диагностике неполадок - логи контейнера.\n\nОднако, если сделать логи слишком подробными, то действительно важную информацию будет\nочень сложно найти. Также мы получим проблемы избыточного использования постоянной\nпамяти или слишком быструю ротацию логов. Но сделав логи слишком сжатыми, мы рискуем\nстолкнуться с ситуацией, когда их недостаточно для диагностики ошибки.\n\nТо есть хочется видеть как можно больше информации во время возникновения ошибок, и как\nможно меньше - когда всё хорошо.\n\n\n## Использование\n\nИспользуя функцию `smart_log(log_message: str, *args: Any, **kwargs: Any)` логируете всю\nинформацию, которая поможет в диагностике ошибки. Если во время обработки сообщения\nбудет выброшено исключение, в логи попадёт:\n\n1. Текущее сообщение от пользователя,\n2. Вся залогированная с помощью `smart_log` информация,\n3. Выброшенное исключение.\n\nЕсли обработка сообщения завершится успешно, накопленные логи будут "выброшены".\n\n## Настройка\n\n1. Устанавливаем библиотеку:  \n```bash\npoetry add pybotx-smart-logger\n```\n\n2. Подключим мидлварь для логирования входящих сообщений:\n\n**middlewares/smart_logger.py**\n```python #logger_init_middleware\nasync def smart_logger_middleware(\n    message: IncomingMessage,\n    bot: Bot,\n    call_next: IncomingMessageHandlerFunc,\n) -> None:\n    async with wrap_smart_logger(\n        log_source="Incoming message",\n        context_func=lambda: format_raw_command(message.raw_command),\n        debug=True,\n    ):\n        await call_next(message, bot)\n```\n\n**bot.py**\n```python #logger_init_bot\nBot(\n    collectors=[collector],\n    bot_accounts=[BOT_CREDENTIALS],\n    middlewares=[\n        smart_logger_middleware,\n    ],\n)\n```\n3. Для того чтобы логировать какие-то другие части приложения, необходимо обернуть в контекстный менджер:\n```python #logger_common_use\nasync def handler() -> None:\n    async with wrap_smart_logger(\n        log_source="Request to Server",\n        context_func=lambda: str(kwargs),\n        debug=False,\n    ):\n        await make_request(**kwargs)\n```\n\n4.  Также можно использовать smart_logger для логирования запросов к FastAPI приложению:\n```python #logger_fastapi_use\napp = FastAPI()\n\n\n@app.middleware("http")\nasync def smart_logger_middleware(request: Request, call_next: Callable) -> None:\n    async with wrap_smart_logger(\n        log_source="Incoming request",\n        context_func=lambda: pformat_str_request(request),\n        debug=DEBUG,\n    ):\n        return await call_next(request)\n```\n`log_source` определяет источник логов. `context_func` - пользовательская функция для форматирования логов.\n\n## Пример команд для включения отладки\n\n```python #logger_debug_enable\n@collector.command("/_debug:enable-for-huids", visible=False)\nasync def enable_debug_for_users(message: IncomingMessage, bot: Bot) -> None:\n    try:\n        huids = [UUID(huid) for huid in message.arguments]\n    except ValueError:\n        await bot.answer_message("Получен невалидный user_huid")\n        return\n\n    # TODO: Обновите список user_huid\n\n    await bot.answer_message(f"Список user_huid для отладки обновлён {huids}")\n```\n\n\n```python #logger_debug_enable_command\n@collector.command("/_debug:enable-for-tasks", visible=False)\nasync def enable_debug_for_tasks(message: IncomingMessage, bot: Bot) -> None:\n    # TODO: Обновите список имён задач\n\n    await bot.answer_message("Список задач для отладки обновлён")\n```\n\n\n## Где применять\n\n1. Проверка роли:\n\n```python #logger_check_role\n# TODO: Мидлварь для заполнения message.state.user\n\n\nasync def subscribed_users_only_middleware(\n    message: IncomingMessage,\n    bot: Bot,\n    call_next: IncomingMessageHandlerFunc,\n) -> None:\n    if not message.state.user.is_subscribed:\n        await bot.send(message=only_subscribed_users_allowed_message(message))\n\n        return\n\n    smart_log("This user is subscribed")\n\n    await call_next(message, bot)\n```\n\n2. Обращение в API:\n\n```python #logger_api_call\nasync def _perform_request(\n    method: Literal["GET", "POST"],\n    url: str,\n    query_params: Optional[Dict[str, Any]] = None,\n    body_dict: Optional[Dict[str, Any]] = None,\n) -> str:\n    smart_log("Performing request to YourAwesomeAPI")\n    smart_log("Method:", method)\n    smart_log("URL:", url)\n    smart_log("Query parameters:", query_params)\n    smart_log("Body dict:", body_dict)\n\n    try:\n        async with AsyncClient(base_url=base_url) as client:\n            response = await client.request(\n                method,\n                url,\n                params=query_params,\n                json=body_dict,\n            )\n    except HTTPError as exc:\n        raise RequestToAwesomeAPIError from exc\n\n    smart_log("Response text:", response.text)\n\n    try:\n        response.raise_for_status()\n    except HTTPStatusError as exc:  # noqa: WPS440\n        raise InvalidStatusCodeFromAwesomeAPIError from exc\n\n    return response.text\n```\n\nА также любые моменты, где что-то может пойти не так. Логируйте - не стестяйтесь.\n',
     'author': 'Alexander Samoylenko',
     'author_email': 'alexandr.samojlenko@ccsteam.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pybotx_smart_logger-0.9.8/PKG-INFO` & `pybotx_smart_logger-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pybotx-smart-logger
-Version: 0.9.8
+Version: 0.9.9
 Summary: Shows logs when you need it
 Author: Alexander Samoylenko
 Author-email: alexandr.samojlenko@ccsteam.ru
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: fastapi (>=0.70.0,<0.75.0)
-Requires-Dist: pybotx (>=0.44.1,<0.55.0)
+Requires-Dist: loguru (>=0.6.0,<0.7.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 # pybotx-smart-logger
 
 _Shows logs when you need it_
```

