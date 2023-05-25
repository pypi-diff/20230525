# Comparing `tmp/bastion_api-0.2.5.tar.gz` & `tmp/bastion_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastion_api-0.2.5.tar", max compression
+gzip compressed data, was "bastion_api-0.3.0.tar", max compression
```

## Comparing `bastion_api-0.2.5.tar` & `bastion_api-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0      178 2023-04-10 12:05:00.739901 bastion_api-0.2.5/LICENSE
--rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 bastion_api-0.2.5/README.md
--rw-r--r--   0        0        0      311 2023-05-19 09:20:55.118369 bastion_api-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 09:32:45.417575 bastion_api-0.2.5/src/bastion_api/__init__.py
--rw-r--r--   0        0        0    34553 2023-05-19 09:19:28.207340 bastion_api-0.2.5/src/bastion_api/bastion.py
--rw-r--r--   0        0        0        0 2023-05-16 13:17:30.854465 bastion_api-0.2.5/src/bastion_api/dto/__init__.py
--rw-r--r--   0        0        0      173 2023-05-16 13:58:25.251623 bastion_api-0.2.5/src/bastion_api/dto/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      536 2023-05-17 12:02:03.938377 bastion_api-0.2.5/src/bastion_api/dto/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0      899 2023-05-17 12:02:03.910378 bastion_api-0.2.5/src/bastion_api/dto/__pycache__/device_dto.cpython-310.pyc
--rw-r--r--   0        0        0     1098 2023-05-17 12:02:03.910378 bastion_api-0.2.5/src/bastion_api/dto/__pycache__/organization_dto.cpython-310.pyc
--rw-r--r--   0        0        0     5532 2023-05-17 12:03:24.517481 bastion_api-0.2.5/src/bastion_api/dto/__pycache__/pass_dto.cpython-310.pyc
--rw-r--r--   0        0        0     1979 2023-05-17 12:02:03.914378 bastion_api-0.2.5/src/bastion_api/dto/__pycache__/person_dto.cpython-310.pyc
--rw-r--r--   0        0        0     2270 2023-05-17 12:02:03.914378 bastion_api-0.2.5/src/bastion_api/dto/__pycache__/points_dto.cpython-310.pyc
--rw-r--r--   0        0        0     4478 2023-05-17 12:02:03.922378 bastion_api-0.2.5/src/bastion_api/dto/__pycache__/support.cpython-310.pyc
--rw-r--r--   0        0        0      212 2023-05-18 13:24:55.942013 bastion_api-0.2.5/src/bastion_api/dto/config.py
--rw-r--r--   0        0        0      957 2023-05-16 14:23:37.380494 bastion_api-0.2.5/src/bastion_api/dto/device_dto.py
--rw-r--r--   0        0        0     2960 2023-05-16 14:20:20.754482 bastion_api-0.2.5/src/bastion_api/dto/old_dto.py
--rw-r--r--   0        0        0     1449 2023-05-16 13:27:28.275950 bastion_api-0.2.5/src/bastion_api/dto/organization_dto.py
--rw-r--r--   0        0        0     8763 2023-05-18 13:41:28.612882 bastion_api-0.2.5/src/bastion_api/dto/pass_dto.py
--rw-r--r--   0        0        0     2898 2023-05-16 13:27:28.295950 bastion_api-0.2.5/src/bastion_api/dto/person_dto.py
--rw-r--r--   0        0        0     2558 2023-05-16 14:17:31.752162 bastion_api-0.2.5/src/bastion_api/dto/points_dto.py
--rw-r--r--   0        0        0     4916 2023-05-17 12:18:28.396213 bastion_api-0.2.5/src/bastion_api/dto/support.py
--rw-r--r--   0        0        0      994 2023-05-17 12:18:28.360214 bastion_api-0.2.5/src/bastion_api/handlers.py
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 bastion_api-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      178 2023-04-10 12:05:00.739901 bastion_api-0.3.0/LICENSE
+-rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 bastion_api-0.3.0/README.md
+-rw-r--r--   0        0        0      311 2023-05-25 08:44:23.584258 bastion_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 09:32:45.417575 bastion_api-0.3.0/src/bastion_api/__init__.py
+-rw-r--r--   0        0        0    34986 2023-05-25 08:29:31.889757 bastion_api-0.3.0/src/bastion_api/bastion.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:17:30.854465 bastion_api-0.3.0/src/bastion_api/dto/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-16 13:58:25.251623 bastion_api-0.3.0/src/bastion_api/dto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      907 2023-05-24 14:24:44.899037 bastion_api-0.3.0/src/bastion_api/dto/__pycache__/device_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     1098 2023-05-17 12:02:03.910378 bastion_api-0.3.0/src/bastion_api/dto/__pycache__/organization_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     5533 2023-05-24 14:24:30.247151 bastion_api-0.3.0/src/bastion_api/dto/__pycache__/pass_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     1979 2023-05-17 12:02:03.914378 bastion_api-0.3.0/src/bastion_api/dto/__pycache__/person_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     2247 2023-05-24 14:24:30.251150 bastion_api-0.3.0/src/bastion_api/dto/__pycache__/points_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     4479 2023-05-24 14:24:30.255150 bastion_api-0.3.0/src/bastion_api/dto/__pycache__/support.cpython-310.pyc
+-rw-r--r--   0        0        0      964 2023-05-23 12:58:06.859649 bastion_api-0.3.0/src/bastion_api/dto/device_dto.py
+-rw-r--r--   0        0        0     2960 2023-05-16 14:20:20.754482 bastion_api-0.3.0/src/bastion_api/dto/old_dto.py
+-rw-r--r--   0        0        0     1449 2023-05-16 13:27:28.275950 bastion_api-0.3.0/src/bastion_api/dto/organization_dto.py
+-rw-r--r--   0        0        0     8763 2023-05-25 08:29:31.881758 bastion_api-0.3.0/src/bastion_api/dto/pass_dto.py
+-rw-r--r--   0        0        0     2898 2023-05-16 13:27:28.295950 bastion_api-0.3.0/src/bastion_api/dto/person_dto.py
+-rw-r--r--   0        0        0     2555 2023-05-23 09:04:17.397615 bastion_api-0.3.0/src/bastion_api/dto/points_dto.py
+-rw-r--r--   0        0        0     4916 2023-05-17 12:18:28.396213 bastion_api-0.3.0/src/bastion_api/dto/support.py
+-rw-r--r--   0        0        0      944 2023-05-25 07:47:42.262724 bastion_api-0.3.0/src/bastion_api/error_handler.py
+-rw-r--r--   0        0        0     1120 2023-05-25 08:41:53.767471 bastion_api-0.3.0/src/bastion_api/handlers.py
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 bastion_api-0.3.0/PKG-INFO
```

### Comparing `bastion_api-0.2.5/src/bastion_api/bastion.py` & `bastion_api-0.3.0/src/bastion_api/bastion.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,159 +2,165 @@
 from http.cookies import SimpleCookie
 from typing import Dict, List
 from datetime import datetime as dt, timedelta as td
 from pydantic import BaseModel
 from aiohttp import ClientResponse, ClientSession
 from loguru import logger
 
+
 from bastion_api.dto.device_dto import DeviceDto
 from bastion_api.dto.organization_dto import OrgDto, DepartDto
 from bastion_api.dto.pass_dto import CardEventDto, CardDto, AttendanceDto, PassDto, MatValuePassDto, CarPassDto
 from bastion_api.dto.person_dto import PersonDto
 from bastion_api.dto.points_dto import EntryPointDto, AccessLevelDto, ControlAreaDto, AccessPointDto
 from bastion_api.dto.support import DictValDto, PassBriefDto
-from bastion_api.dto.config import BastionConfig
-from bastion_api.handlers import BastionIntegrationError, _handle_response
+from bastion_api.error_handler import BastionIntegrationError
+from bastion_api.handlers import ResponseMethod, _handle_response, BastionDeviceType, BastionInfo, \
+    BastionConfig
 
 
-class Bastion:
-    session = ClientSession
-    config: BaseModel
-    bastion_servers: []
-    _code_for_url: str = ""
-    config: BastionConfig
-    cookies: SimpleCookie
+class Bastion(BastionInfo):
 
-    async def _wrap_response(self, method: str, url: str, data: BaseModel | None | Dict = None) -> ClientResponse:
+    async def _wrap_response(self, method: ResponseMethod, url: str,
+                             data: BaseModel | None | Dict = None) -> ClientResponse:
         if self.session:
-            async with self.session.request(method.upper(),
+            async with self.session.request(method=method.value,
                                             url=f"http://{self.config.iks_host}:{self.config.iks_port}{url}",
                                             json=data.dict() if isinstance(data, BaseModel) else data if isinstance(
                                                 data, Dict) else None) as response:
                 await response.read()
                 self.cookies = response.cookies
-                if "debug" in self.config.log:
-                    logger.debug(
-                        f"\nurl: {url}\nresponse_body: {bytes(await response.read()).decode()}\nresponse: {response}")
 
                 if response.cookies:
                     for cook in response.cookies.values():
                         cook["expires"] = (dt.now() + td(days=1)).strftime("%a, %d %b %Y %H:%M:%S GMT")
                     self.session.cookie_jar.update_cookies(response.cookies)
+
+                if self.log_debug:
+                    logger.debug(
+                        f"\nurl: {url}\nresponse_body: {bytes(await response.read()).decode()}\nresponse: {response} \nCookies: {self.cookies}")
+
                 if response.status != 200:
                     raise BastionIntegrationError(message=f"Bad response status:  {response.status}")
 
-        return response
+        else:
+            raise BastionIntegrationError(message='Session not exist')
 
-    def _set_config(self, config):
-        self.config = BastionConfig(**json.loads(config))
+        return response
 
     # ________________________________________________________________________________________________________
 
-    async def connect_to_bastion_iks(self, config, search_servers: str = None):
+    async def init_bastion_iks(self, config, search_servers: str = None) -> str:
         """Функция осуществляет подключение к Бастион ИКС согласно файлу конфигурации"""
-        self._set_config(config)
-        response = await(await self._wrap_response(method="POST", url="/api/Login",
+        self.session = ClientSession()
+        self.config = BastionConfig(**json.loads(config))
+        response = await(await self._wrap_response(method=ResponseMethod.POST,
+                                                   url="/api/Login",
                                                    data={"opername": f"{self.config.iks_operator_login}",
                                                          "password": f"{self.config.iks_operator_password}"})).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
 
-        self.bastion_servers = (await (await self._wrap_response(method="GET", url="/api/GetServers")).json())
+        self.bastion_servers = (await (await self._wrap_response(method=ResponseMethod.GET,
+                                                                 url="/api/GetServers")).json())
         if search_servers:
             if search_servers.lower() in self.bastion_servers.servers_code:
                 self.bastion_servers.servers_code = search_servers.lower()
             else:
                 raise BastionIntegrationError(message="Some server not found")
 
         for server_code in (
-                self.bastion_servers if self.bastion_servers.__class__ == "list" else [
-                    self.bastion_servers]):
+                self.bastion_servers if self.bastion_servers.__class__ == "list" else
+                self.bastion_servers):
             self._code_for_url = self._code_for_url + f"srvCode={server_code}&"
+        return response
 
     # ________________________________________________________________________________________________________
 
     async def logout_bastion_iks(self):
-        await self._wrap_response(method="POST", url="/api/LogOff")
+        await self._wrap_response(method=ResponseMethod.POST,
+                                  url="/api/LogOff")
 
     # ________________________________________________________________________________________________________
 
     async def get_bastion_version(self) -> str:
         """Метод, возвращающий строку с версией модуля"""
-        response = await (await self._wrap_response(method="GET", url="/api/GetVersion")).text()
-        if "info" in self.config.log:
+        response = await (await self._wrap_response(method=ResponseMethod.GET,
+                                                    url="/api/GetVersion")).text()
+        if self.log_info:
             logger.info(response)
         return response
 
     async def check_bastion_connection(self) -> str:
         """Метод предназначен для проверки связи с одним или несколькими серверами."""
         response = await (
-            await self._wrap_response(method="GET", url=f"/api/CheckConnection?{self._code_for_url}")).text()
-        if "info" in self.config.log:
+            await self._wrap_response(method=ResponseMethod.GET,
+                                      url=f"/api/CheckConnection?{self._code_for_url}")).text()
+        if self.log_info:
             logger.info(response)
         return response
 
     # ________________________________________________________________________________________________________
 
     async def get_bastion_entry_points(self) -> List[EntryPointDto]:
         """Метод, предназначенный для получения информации о точках прохода"""
         response = await (
-            await self._wrap_response(method="GET", url=f"/api/GetEntryPoints?{self._code_for_url}")).json()
+            await self._wrap_response(method=ResponseMethod.GET, url=f"/api/GetEntryPoints?{self._code_for_url}")).json()
         model_list = await _handle_response(response, EntryPointDto)
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return model_list
 
     async def get_bastion_access_level(self) -> List[AccessLevelDto]:
         """Метод, предназначенный для получения информации об уровнях доступа"""
         response = await (
-            await self._wrap_response(method="GET", url=f"/api/GetAccessLevels?{self._code_for_url}")).json()
+            await self._wrap_response(method=ResponseMethod.GET, url=f"/api/GetAccessLevels?{self._code_for_url}")).json()
         model_list = await _handle_response(response, AccessLevelDto)
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     # ________________________________________________________________________________________________________
 
     async def get_bastion_dict_value(self, category: int = "") -> List[DictValDto]:
         """Метод предназначен для запроса списка словарных значений с фильтрацией
         по категории.
         category = Категория словарных значений, информацию о которых требуется получить
         """
-        response = await (await self._wrap_response(method="GET", url=f"/api/GetDictVals?{self._code_for_url}"
+        response = await (await self._wrap_response(method=ResponseMethod.GET, url=f"/api/GetDictVals?{self._code_for_url}"
                                                                       f"category={category}")).json()
         model_list = await _handle_response(response, DictValDto)
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return model_list
 
     async def get_bastion_card_events(self, card_info: CardDto) -> List[CardEventDto]:
         """Метод предназначен для получения списка событий, произошедших с конкретной картой доступа"""
 
-        response = await(await self._wrap_response(method="GET",
+        response = await(await self._wrap_response(method=ResponseMethod.GET,
                                                    url=f"/api/GetCardEvents?{self._code_for_url}"
                                                        f"cardCode={card_info.card_code}&"
                                                        f"dateFrom={card_info.date_from}&"
                                                        f"dateTo={card_info.date_to}")).json()
         model_list = await _handle_response(response, CardEventDto)
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     async def get_bastion_attendance(self, card_info: CardDto) -> List[AttendanceDto]:
         """Метод предназначен для получения списка посещений с конкретной картой доступа,
          либо со всеми катами доступа с сервера"""
 
-        response = await (await self._wrap_response(method="GET",
+        response = await (await self._wrap_response(method=ResponseMethod.GET,
                                                     url=f"/api/GetAttendance?{self._code_for_url}"
                                                         f"cardCode={card_info.card_code}&"
                                                         f"dateFrom={card_info.date_from}&"
                                                         f"dateTo={card_info.date_to}")).json()
         model_list = await _handle_response(response, AttendanceDto)
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     # ________________________________________________________________________________________________________
 
     async def create_or_update_bastion_pass(self, new_pass_card: PassDto.NewPassPerson, use_access_level: bool = ''):
         """
@@ -168,343 +174,347 @@
                                  По умолчанию значение флага – false,
                                   в этом случае используются данные поля EntryPoints модели Pass.
                                   стр. 29 документации пп 5.14
         """
         if not new_pass_card.entryPoints and not new_pass_card.accessLevels:
             raise BastionIntegrationError(message="Please input access level or entry points")
 
-        response = await (await self._wrap_response(method="PUT",
+        response = await (await self._wrap_response(method=ResponseMethod.PUT,
                                                     url=f"/api/PutPass?{self._code_for_url}"
                                                         f"useAccessLevelsInsteadOfEntryPoints={use_access_level}",
                                                     data=new_pass_card)).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response
 
     async def return_bastion_pass_for_card(self, _pass: PassDto.ReturnPassForCardCode, ) -> str:
         """Метод предназначен для создания или редактирования КД,
          а также для создания/редактирования заявки на пропуск"""
 
-        response = await (await self._wrap_response(method="PUT",
+        response = await (await self._wrap_response(method=ResponseMethod.PUT,
                                                     url=f"/api/PutPass?{self._code_for_url}"
                                                         f"useAccessLevelsInsteadOfEntryPoints=",
                                                     data=_pass)).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response
 
     async def get_bastion_pass(self, get_pass_info: PassDto.ReturnPass) -> List[PassDto]:
         """Метод предназначен для получения списка пропусков
         с фильтрацией по их статусу и типу с сервера"""
-        response = await (await self._wrap_response(method="GET",
+        response = await (await self._wrap_response(method=ResponseMethod.GET,
                                                     url=f"/api/GetPasses?{self._code_for_url}"
                                                         f"cardStatus={get_pass_info.card_status}&"
                                                         f"passType={get_pass_info.pass_type}&"
                                                         f"withoutPhoto={get_pass_info.without_photo}&"
                                                         f"startFrom={get_pass_info.start_numer}&"
                                                         f"maxCount={get_pass_info.max_count}")).json()
         model_list = await _handle_response(response, PassDto)
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     async def get_bastion_passes_by_person(self, person_info: PersonDto, without_photo: bool) -> List[PassDto]:
         """Метод предназначен для получения списка пропусков любых статусов"""
 
-        response = await (await self._wrap_response(method="GET",  # Dont change url parameters
+        response = await (await self._wrap_response(method=ResponseMethod.GET,  # Dont change url parameters
                                                     url=f"/api/GetPassesByPerson?{self._code_for_url}"
                                                         f"name={person_info.name}&"
                                                         f"firstname={person_info.firstName}&"
                                                         f"secondname={person_info.secondName}&"
                                                         f"birthDate={person_info.birthDate}&"
                                                         f"withoutPhoto={without_photo}")).json()
 
         model_list = await _handle_response(response, PassDto)
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     async def get_bastion_pass_by_card(self, card_code: str, without_photo: bool = "") -> List[PassDto]:
         """Метод предназначен для получения списка пропусков любых статусов, по которым когда-либо выдавалась карта
         without_photo: bool - true если фотографии возвращать не нужно"""
-        response = await (await self._wrap_response(method="GET",
+        response = await (await self._wrap_response(method=ResponseMethod.GET,
                                                     url=f"/api/GetPassesByCardCode?{self._code_for_url}"
                                                         f"cardCode={card_code}&"
                                                         f"withoutPhoto={without_photo}")).json()
         model_list = await _handle_response(response, PassDto)
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     async def get_bastion_pass_count(self, card_status: int = "", pass_type: int = "") -> str:
         """Метод предназначен для получения общего количества пропусков"""
-        response = await (await self._wrap_response(method="GET",
+        response = await (await self._wrap_response(method=ResponseMethod.GET,
                                                     url=f"/api/GetPassCount?{self._code_for_url}"
                                                         f"cardStatus={card_status}&"
                                                         f"passType={pass_type}")).text()
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>  <srvN> – код сервера, а <resultN> – результат выполнения операции.
 
     async def block_bastion_pass(self, card_code: str, block_reason: str) -> str:
         """Метод предназначен для блокировки КД"""
-        response = await (await self._wrap_response(method="GET",
+        response = await (await self._wrap_response(method=ResponseMethod.GET,
                                                     url=f"/api/BlockPass?{self._code_for_url}"
                                                         f"cardCode={card_code}&"
                                                         f"blockReason={block_reason}")).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>  <srvN> – код сервера, а <resultN> – результат выполнения операции.
 
     async def unblock_bastion_pass(self, card_code: str) -> str:
         """Метод предназначен для разблокировки КД"""
-        response = await (await self._wrap_response(method="GET", url=f"/api/UnblockPass?{self._code_for_url}"
+        response = await (await self._wrap_response(method=ResponseMethod.GET, url=f"/api/UnblockPass?{self._code_for_url}"
                                                                       f"cardCode={card_code}")).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>  <srvN> – код сервера, а <resultN> – результат выполнения операции.
 
     async def archive_bastion_pass(self, card_code: str) -> str:
         """Метод предназначен для переноса в архив карты доступа"""
-        response = await (await self._wrap_response(method="GET", url=f"/api/ReturnPass?{self._code_for_url}"
+        response = await (await self._wrap_response(method=ResponseMethod.GET, url=f"/api/ReturnPass?{self._code_for_url}"
                                                                       f"cardCode={card_code}")).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>  <srvN> – код сервера, а <resultN> – результат выполнения операции.
 
     async def issue_bastion_pass(self, person_info: PersonDto, pass_type: int, card_code: str) -> str:
         """Метод предназначен для выдачи КД по ранее созданной заявке на пропуск"""
-        response = await (await self._wrap_response(method="GET",
+        response = await (await self._wrap_response(method=ResponseMethod.GET,
                                                     url=f"/api/IssuePass?{self._code_for_url}"
                                                         f"name={person_info.name}&"
                                                         f"firstname={person_info.firstName}&"
                                                         f"secondname={person_info.secondName}&"
                                                         f"birthDate={person_info.birthDate}&"
                                                         f"passType={pass_type}&"
                                                         f"cardCode={card_code}")).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>  <srvN> – код сервера, а <resultN> – результат выполнения операции.
 
     async def get_bastion_material_pass_by_pass(self, pass_id: int) -> str:
         """Метод предназначен для выдачи материального пропуска по ранее созданной заявке на сервере"""
         response = await (
-            await self._wrap_response(method="GET",
+            await self._wrap_response(method=ResponseMethod.GET,
                                       url=f"/api/IssueMVPass?{self._code_for_url}passid={pass_id}")).json()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def ban_bastion_material_pass(self, pass_id: int) -> str:
         """Метод предназначен для изъятия материального пропуска на сервере"""
-        response = await (await self._wrap_response(method="GET",
+        response = await (await self._wrap_response(method=ResponseMethod.GET,
                                                     url=f"/api/WithdrawMVPass?{self._code_for_url}passid={pass_id}")).json()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     # ________________________________________________________________________________________________________
 
     async def get_bastion_organisation(self, org_filter: str = "") -> List[OrgDto]:
         """Метод предназначен для получения списка организаций"""
-        response = await (await self._wrap_response(method="GET", url=f"/api/GetOrgs?{self._code_for_url}"
+        response = await (await self._wrap_response(method=ResponseMethod.GET, url=f"/api/GetOrgs?{self._code_for_url}"
                                                                       f"filter={org_filter}")).json()
         model_list = await _handle_response(response, OrgDto)
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     async def create_bastion_organization(self, organization: OrgDto) -> str:
         """Метод предназначен для добавления организации """
         response = await (
-            await self._wrap_response(method="PUT", url=f"/api/PutOrg?{self._code_for_url}", data=organization)).text()
-        if "info" in self.config.log:
+            await self._wrap_response(method=ResponseMethod.PUT, url=f"/api/PutOrg?{self._code_for_url}", data=organization)).text()
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def update_bastion_organization(self, organization: OrgDto, organization_new_name: str) -> str:
         """Метод предназначен для переименования организации на всех серверах, добавленных в схему интеграции, либо на одном сервере, код которого передан в качестве входного параметра."""
-        response = await (await self._wrap_response(method="POST",
+        response = await (await self._wrap_response(method=ResponseMethod.POST,
                                                     url=f"/api/UpdateOrg?{self._code_for_url}"
                                                         f"orgNewName={organization_new_name}",
                                                     data=organization)).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def delete_bastion_organization(self, organization: OrgDto) -> str:
         """Метод предназначен для удаления организации (вместе со всеми дочерними организациями и подразделениями) на всех серверах, добавленных в схему интеграции, либо на одном сервере, код которого передан в качестве входного параметра."""
         response = await (
-            await self._wrap_response(method="POST", url=f"/api/DeleteOrg?{self._code_for_url}",
+            await self._wrap_response(method=ResponseMethod.POST, url=f"/api/DeleteOrg?{self._code_for_url}",
                                       data=organization)).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     # ________________________________________________________________________________________________________
 
     async def get_bastion_department(self, department_name: str = "") -> List[DepartDto]:
         """Метод предназначен для получения списка подразделений (всех, либо принадлежащих организации, имя которой передано в качестве входного параметра)"""
-        response = await (await self._wrap_response(method="GET",
+        response = await (await self._wrap_response(method=ResponseMethod.GET,
                                                     url=f"/api/GetDeparts?{self._code_for_url}parentOrgName={department_name}")).json()
         model_list = await _handle_response(response, DepartDto)
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     async def create_bastion_department(self, department: DepartDto) -> str:
         """Метод предназначен для добавления подразделения"""
         response = await (
-            await self._wrap_response(method="PUT", url=f"/api/PutDepart?{self._code_for_url}", data=department)).text()
-        if "info" in self.config.log:
+            await self._wrap_response(method=ResponseMethod.PUT, url=f"/api/PutDepart?{self._code_for_url}", data=department)).text()
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def update_bastion_department(self, department: DepartDto, new_department_name: str) -> str:
         """Метод предназначен для переименования подразделения"""
-        response = await (await self._wrap_response(method="POST",
+        response = await (await self._wrap_response(method=ResponseMethod.POST,
                                                     url=f"/api/UpdateDepart?{self._code_for_url}departNewName={new_department_name}",
                                                     data=department)).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def delete_bastion_department(self, department: DepartDto) -> str:
         """Метод предназначен для удаления подразделения"""
-        response = await (await self._wrap_response(method="POST", url=f"/api/DeleteDepart?{self._code_for_url}",
+        response = await (await self._wrap_response(method=ResponseMethod.POST, url=f"/api/DeleteDepart?{self._code_for_url}",
                                                     data=department)).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     # ________________________________________________________________________________________________________
 
     async def create_or_update_bastion_material_pass(self, mat_value: MatValuePassDto, claim: bool = "", ) -> str:
         """Метод предназначен для создания или редактирования материального пропуска, а также для создания/редактирования заявки на материальный пропуск
         claim - Флаг, определяющий, будет создан выданный материальный пропуск, либо же будет создана заявка на пропуск
             """
         response = await (
-            await self._wrap_response(method="PUT", url=f"/api/PutMVPass?{self._code_for_url}issuePass={claim}",
+            await self._wrap_response(method=ResponseMethod.PUT, url=f"/api/PutMVPass?{self._code_for_url}issuePass={claim}",
                                       data=mat_value)).text()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def get_bastion_material_pass(self, status: int = "") -> List[MatValuePassDto]:
         """Метод предназначен для получения списка материальных пропусков с фильтрацией по их статусу с сервера
         status: int - Статус возвращаемых материальных пропусков. Значение параметра может быть пустым, в этом случае будут возвращены пропуска с любым статусом
         """
-        response = await(await self._wrap_response(method="GET",
+        response = await(await self._wrap_response(method=ResponseMethod.GET,
                                                    url=f"/api/GetMVPasses?{self._code_for_url}status={status}")).json()
         model_list = await _handle_response(response, MatValuePassDto)
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     async def get_bastion_material_pass_by_person(self, pass_dto: PassBriefDto) -> List[MatValuePassDto]:
         """Метод предназначен для получения списка материальных пропусков с фильтрацией по персональному пропуску с сервера, код которого передан в качестве входного параметра"""
 
         response = await (
-            await self._wrap_response(method="POST", url=f"/api/GetMVPassesByPersonPass?{self._code_for_url}",
+            await self._wrap_response(method=ResponseMethod.POST, url=f"/api/GetMVPassesByPersonPass?{self._code_for_url}",
                                       data=pass_dto)).json()
 
         model_list = await _handle_response(response, MatValuePassDto)
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     # ________________________________________________________________________________________________________
 
     async def create_or_update_bastion_car_pass(self, car_pass: CarPassDto, claim: bool = "") -> str:
         """Метод предназначен для создания или редактирования транспортного пропуска, а также для создания/редактирования заявки на транспортный пропуск"""
         response = await (
-            await self._wrap_response(method="PUT", url=f"/api/PutCarPass?{self._code_for_url}issuePass={claim}",
+            await self._wrap_response(method=ResponseMethod.PUT, url=f"/api/PutCarPass?{self._code_for_url}issuePass={claim}",
                                       data=car_pass)).json()
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def get_bastion_car_passes(self, status: int = "") -> List[CarPassDto]:
         """Метод предназначен для получения списка транспортных пропусков с фильтрацией по их статусу
         status: int - Статус возвращаемых транспортных пропусков. Значение параметра может быть пустым, в этом случае будут возвращены пропуска с любым статусом"""
 
         response = await (
-            await self._wrap_response(method="GET",
+            await self._wrap_response(method=ResponseMethod.GET,
                                       url=f"/api/GetCarPasses?{self._code_for_url}status={status}")).json()
 
         model_list = await _handle_response(response, CarPassDto)
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     async def get_bastion_car_passes_by_person_pass(self, pass_dto: PassBriefDto) -> List[CarPassDto]:
         """Метод предназначен для получения списка транспортных пропусков с фильтрацией по персональному пропуску"""
 
         response = await (
-            await self._wrap_response(method="POST", url=f"/api/GetCarPassesByPersonPass?{self._code_for_url}",
+            await self._wrap_response(method=ResponseMethod.POST, url=f"/api/GetCarPassesByPersonPass?{self._code_for_url}",
                                       data=pass_dto)).json()
 
         model_list = await _handle_response(response, CarPassDto)
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     async def issue_bastion_car_pass_by_claim(self, pass_id: int) -> str:
         """Метод предназначен для выдачи транспортного пропуска по ранее созданной заявке"""
         response = await (
-            await self._wrap_response(method="GET",
+            await self._wrap_response(method=ResponseMethod.GET,
                                       url=f"/api/IssueCarPass?{self._code_for_url}passid={pass_id}")).json()
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def banned_bastion_car_pass(self, pass_id: int) -> str:
         """Метод предназначен для изъятия транспортного пропуска на сервере, код которого передан в качестве входного параметра."""
-        response = await (await self._wrap_response(method="GET",
+        response = await (await self._wrap_response(method=ResponseMethod.GET,
                                                     url=f"/api/WithdrawCarPass?{self._code_for_url}passid={pass_id}")).json()
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     # ________________________________________________________________________________________________________
 
-    async def get_bastion_devices(self, driver_id: int = "", device_type: int = "") -> List[DeviceDto]:
+    async def get_bastion_devices(self, driver_id: int = "",
+                                  device_type: BastionDeviceType = BastionDeviceType.All.value) -> List[DeviceDto]:
+
         """Метод предназначен для получения набора устройств, добавленных в систему на сервере
         driver_id: int - Код типа драйвера, устройства которого необходимо получить. Значение параметра может быть пустым, в таком случае будут возвращены устройства всех драйверов
         device_type: int - Код типа устройства. В случае передачи непустого значения параметра будут возвращены устройства только данного типа. Значение параметра может быть пустым."""
-        response = await ((await self._wrap_response(method="GET",
+
+        response = await ((await self._wrap_response(method=ResponseMethod.GET,
                                                      url=f"/api/GetDevices?{self._code_for_url}driverId={driver_id}&deviceType={device_type}"))).json()
 
         model_list = await _handle_response(response, DeviceDto)
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
+
         return model_list
 
     async def get_bastion_control_area(self) -> List[ControlAreaDto]:
         """Метод, предназначенный для получения информации об областях контроля"""
         response = await (
-            await self._wrap_response(method="GET", url=f"/api/GetControlAreas?{self._code_for_url}")).json()
+            await self._wrap_response(method=ResponseMethod.GET, url=f"/api/GetControlAreas?{self._code_for_url}")).json()
         model_list = await _handle_response(response, ControlAreaDto)
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
 
     async def get_bastion_access_point(self) -> List[AccessPointDto]:
         """Метод, предназначенный для получения информации об точках доступа"""
         response = await (
-            await self._wrap_response(method="GET", url=f"/api/GetAccessPoints?{self._code_for_url}")).json()
+            await self._wrap_response(method=ResponseMethod.GET, url=f"/api/GetAccessPoints?{self._code_for_url}")).json()
         model_list = await _handle_response(response, AccessPointDto)
 
-        if "info" in self.config.log:
+        if self.log_info:
             logger.info(model_list)
         return model_list
```

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/__pycache__/device_dto.cpython-310.pyc` & `bastion_api-0.3.0/src/bastion_api/dto/__pycache__/device_dto.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May 16 14:23:37 2023 UTC, .py size: 957 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e991 6364 bd03 0000  o.........cd....
+00000000: 6f0d 0d0a 0000 0000 5eb8 6c64 c403 0000  o.......^.ld....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0173 3800 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6505 8303  ..G.d.d...d.e...
 00000060: 5a06 6406 5300 2907 e900 0000 0029 01da  Z.d.S.)......)..
 00000070: 0b61 6e6e 6f74 6174 696f 6e73 2901 da04  .annotations)...
@@ -30,28 +30,28 @@
 000001d0: 20d1 83d1 81d1 82d1 80d0 bed0 b9d1 81d1   ...............
 000001e0: 82d0 b220 4765 7444 6576 6963 6573 da03  ... GetDevices..
 000001f0: 696e 74da 0373 646e 7a0a 696e 7420 7c20  int..sdnz.int | 
 00000200: 4e6f 6e65 da09 7061 7265 6e74 5364 6eda  None..parentSdn.
 00000210: 0864 7269 7665 7249 64da 0373 7472 da04  .driverId..str..
 00000220: 6e61 6d65 da0a 6465 7669 6365 5479 7065  name..deviceType
 00000230: da0e 6465 7669 6365 5479 7065 4e61 6d65  ..deviceTypeName
-00000240: 7a0f 4c69 7374 5b44 6576 6963 6544 746f  z.List[DeviceDto
-00000250: 5dda 0663 6869 6c64 734e 2905 da08 5f5f  ]..childsN)...__
-00000260: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000270: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000280: da07 5f5f 646f 635f 5fda 0f5f 5f61 6e6e  ..__doc__..__ann
-00000290: 6f74 6174 696f 6e73 5f5f a900 7214 0000  otations__..r...
-000002a0: 0072 1400 0000 fa52 2f68 6f6d 652f 646d  .r.....R/home/dm
-000002b0: 6974 7279 2f50 7963 6861 726d 5072 6f6a  itry/PycharmProj
-000002c0: 6563 7473 2f42 6173 7469 6f6e 5f69 6e74  ects/Bastion_int
-000002d0: 6567 7261 7469 6f6e 2f73 7263 2f62 6173  egration/src/bas
-000002e0: 7469 6f6e 5f61 7069 2f64 746f 2f64 6576  tion_api/dto/dev
-000002f0: 6963 655f 6474 6f2e 7079 7205 0000 0007  ice_dto.pyr.....
-00000300: 0000 0073 1200 0000 0a00 0401 0802 0801  ...s............
-00000310: 0801 0801 0801 0801 0c01 7205 0000 004e  ..........r....N
-00000320: 2907 da0a 5f5f 6675 7475 7265 5f5f 7202  )...__future__r.
-00000330: 0000 00da 0674 7970 696e 6772 0300 0000  .....typingr....
-00000340: da08 7079 6461 6e74 6963 7204 0000 0072  ..pydanticr....r
-00000350: 0500 0000 7214 0000 0072 1400 0000 7214  ....r....r....r.
-00000360: 0000 0072 1500 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000370: 653e 0100 0000 7308 0000 000c 000c 010c  e>....s.........
-00000380: 0214 03                                  ...
+00000240: 7a16 4c69 7374 5b44 6576 6963 6544 746f  z.List[DeviceDto
+00000250: 5d20 7c20 4e6f 6e65 da06 6368 696c 6473  ] | None..childs
+00000260: 4e29 05da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000270: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000280: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000290: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
+000002a0: 5fa9 0072 1400 0000 7214 0000 00fa 532f  _..r....r.....S/
+000002b0: 686f 6d65 2f6b 6f72 6f67 6f64 2f50 7963  home/korogod/Pyc
+000002c0: 6861 726d 5072 6f6a 6563 7473 2f42 6173  harmProjects/Bas
+000002d0: 7469 6f6e 5f69 6e74 6567 7261 7469 6f6e  tion_integration
+000002e0: 2f73 7263 2f62 6173 7469 6f6e 5f61 7069  /src/bastion_api
+000002f0: 2f64 746f 2f64 6576 6963 655f 6474 6f2e  /dto/device_dto.
+00000300: 7079 7205 0000 0007 0000 0073 1200 0000  pyr........s....
+00000310: 0a00 0401 0802 0801 0801 0801 0801 0801  ................
+00000320: 0c01 7205 0000 004e 2907 da0a 5f5f 6675  ..r....N)...__fu
+00000330: 7475 7265 5f5f 7202 0000 00da 0674 7970  ture__r......typ
+00000340: 696e 6772 0300 0000 da08 7079 6461 6e74  ingr......pydant
+00000350: 6963 7204 0000 0072 0500 0000 7214 0000  icr....r....r...
+00000360: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
+00000370: da08 3c6d 6f64 756c 653e 0100 0000 7308  ..<module>....s.
+00000380: 0000 000c 000c 010c 0214 03              ...........
```

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/__pycache__/organization_dto.cpython-310.pyc` & `bastion_api-0.3.0/src/bastion_api/dto/__pycache__/organization_dto.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/__pycache__/pass_dto.cpython-310.pyc` & `bastion_api-0.3.0/src/bastion_api/dto/__pycache__/pass_dto.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed May 17 12:03:24 2023 UTC, .py size: 8775 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 8cc2 6464 4722 0000  o.........ddG"..
+00000000: 6f0d 0d0a 0000 0000 1e1e 6e64 2c23 0000  o.........nd,#..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 ce00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 6d09 5a09 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  d.l.m.Z.m.Z.m.Z.
@@ -18,16 +18,16 @@
 00000110: 01da 044c 6973 7429 01da 0942 6173 654d  ...List)...BaseM
 00000120: 6f64 656c 2901 da09 5065 7273 6f6e 4474  odel)...PersonDt
 00000130: 6f29 02da 0d45 6e74 7279 506f 696e 7444  o)...EntryPointD
 00000140: 746f da0e 4163 6365 7373 4c65 7665 6c44  to..AccessLevelD
 00000150: 746f 2905 da0f 5469 6d65 496e 7465 7276  to)...TimeInterv
 00000160: 616c 4474 6fda 0e50 6572 736f 6e42 7269  alDto..PersonBri
 00000170: 6566 4474 6fda 0b4d 6174 5661 6c75 6544  efDto..MatValueD
-00000180: 746f da06 4361 7244 746f da0c 5061 7373  to..CarDto..Pass
-00000190: 4272 6965 6644 746f 6300 0000 0000 0000  BriefDtoc.......
+00000180: 746f da0c 5061 7373 4272 6965 6644 746f  to..PassBriefDto
+00000190: da06 4361 7244 746f 6300 0000 0000 0000  ..CarDtoc.......
 000001a0: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 000001b0: 0073 3c00 0000 6500 5a01 6400 5a02 4700  .s<...e.Z.d.Z.G.
 000001c0: 6401 6402 8400 6402 6503 8303 5a04 4700  d.d...d.e...Z.G.
 000001d0: 6403 6404 8400 6404 6503 8303 5a05 4700  d.d...d.e...Z.G.
 000001e0: 6405 6406 8400 6406 6503 8303 5a06 6407  d.d...d.e...Z.d.
 000001f0: 5300 2908 da07 5061 7373 4474 6f63 0000  S.)...PassDtoc..
 00000200: 0000 0000 0000 0000 0000 0000 0000 0300  ................
@@ -58,289 +58,289 @@
 00000390: 6d65 5f5f da07 5f5f 646f 635f 5f72 0500  me__..__doc__r..
 000003a0: 0000 da0f 5f5f 616e 6e6f 7461 7469 6f6e  ....__annotation
 000003b0: 735f 5f72 1100 0000 7203 0000 0072 0600  s__r....r....r..
 000003c0: 0000 7212 0000 0072 0700 0000 da03 7374  ..r....r......st
 000003d0: 72da 0369 6e74 7215 0000 0072 1600 0000  r..intr....r....
 000003e0: 7217 0000 0072 1900 0000 7208 0000 0072  r....r....r....r
 000003f0: 1a00 0000 7202 0000 0072 1b00 0000 a900  ....r....r......
-00000400: 7223 0000 0072 2300 0000 fa50 2f68 6f6d  r#...r#....P/hom
-00000410: 652f 646d 6974 7279 2f50 7963 6861 726d  e/dmitry/Pycharm
-00000420: 5072 6f6a 6563 7473 2f42 6173 7469 6f6e  Projects/Bastion
-00000430: 5f69 6e74 6567 7261 7469 6f6e 2f73 7263  _integration/src
-00000440: 2f62 6173 7469 6f6e 5f61 7069 2f64 746f  /bastion_api/dto
-00000450: 2f70 6173 735f 6474 6f2e 7079 da0d 4e65  /pass_dto.py..Ne
-00000460: 7750 6173 7350 6572 736f 6e0c 0000 0073  wPassPerson....s
-00000470: 1c00 0000 0a00 0401 0801 1001 1001 0801  ................
-00000480: 0801 0c01 0c01 0c01 0801 0c01 0c01 1001  ................
-00000490: 7225 0000 0063 0000 0000 0000 0000 0000  r%...c..........
-000004a0: 0000 0000 0000 0300 0000 4000 0000 7336  ..........@...s6
-000004b0: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-000004c0: 0364 025a 0465 0565 0664 033c 0065 0765  .d.Z.e.e.d.<.e.e
-000004d0: 0664 043c 0065 0865 0664 053c 0065 0565  .d.<.e.e.d.<.e.e
-000004e0: 0664 063c 0064 0753 0029 087a 1d50 6173  .d.<.d.S.).z.Pas
-000004f0: 7344 746f 2e52 6574 7572 6e50 6173 7346  sDto.ReturnPassF
-00000500: 6f72 4361 7264 436f 6465 da14 7265 7475  orCardCode..retu
-00000510: 726e 5f70 6173 735f 666f 725f 6361 7264  rn_pass_for_card
-00000520: 7210 0000 00da 0863 6172 6443 6f64 6572  r......cardCoder
-00000530: 0f00 0000 7214 0000 0072 1300 0000 4e29  ....r....r....N)
-00000540: 0972 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
-00000550: 721f 0000 0072 2700 0000 7221 0000 0072  r....r'...r!...r
-00000560: 2000 0000 7205 0000 0072 2200 0000 7223   ...r....r"...r#
-00000570: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
-00000580: 0000 da15 5265 7475 726e 5061 7373 466f  ....ReturnPassFo
-00000590: 7243 6172 6443 6f64 651b 0000 0073 0c00  rCardCode....s..
-000005a0: 0000 0a00 0401 0c01 0801 0801 0c01 7228  ..............r(
-000005b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-000005c0: 0000 0000 0300 0000 4000 0000 734e 0000  ........@...sN..
-000005d0: 0065 005a 0164 005a 0255 0064 015a 0364  .e.Z.d.Z.U.d.Z.d
-000005e0: 025a 0465 0565 0664 033c 0064 025a 0765  .Z.e.e.d.<.d.Z.e
-000005f0: 0565 0664 043c 0064 025a 0865 0965 0664  .e.d.<.d.Z.e.e.d
-00000600: 053c 0064 025a 0a65 0565 0664 063c 0064  .<.d.Z.e.e.d.<.d
-00000610: 025a 0b65 0565 0664 073c 0064 0853 0029  .Z.e.e.d.<.d.S.)
-00000620: 097a 1250 6173 7344 746f 2e52 6574 7572  .z.PassDto.Retur
-00000630: 6e50 6173 73da 0867 6574 5f70 6173 7372  nPass..get_passr
-00000640: 1000 0000 da0b 6361 7264 5f73 7461 7475  ......card_statu
-00000650: 73da 0970 6173 735f 7479 7065 da0d 7769  s..pass_type..wi
-00000660: 7468 6f75 745f 7068 6f74 6fda 0b73 7461  thout_photo..sta
-00000670: 7274 5f6e 756d 6572 da09 6d61 785f 636f  rt_numer..max_co
-00000680: 756e 744e 290c 721c 0000 0072 1d00 0000  untN).r....r....
-00000690: 721e 0000 0072 1f00 0000 722a 0000 0072  r....r....r*...r
-000006a0: 2200 0000 7220 0000 0072 2b00 0000 722c  "...r ...r+...r,
-000006b0: 0000 00da 0462 6f6f 6c72 2d00 0000 722e  .....boolr-...r.
-000006c0: 0000 0072 2300 0000 7223 0000 0072 2300  ...r#...r#...r#.
-000006d0: 0000 7224 0000 00da 0a52 6574 7572 6e50  ..r$.....ReturnP
-000006e0: 6173 7323 0000 0073 0e00 0000 0a00 0401  ass#...s........
-000006f0: 0c01 0c01 0c01 0c01 1001 7230 0000 004e  ..........r0...N
-00000700: 2907 721c 0000 0072 1d00 0000 721e 0000  ).r....r....r...
-00000710: 0072 0400 0000 7225 0000 0072 2800 0000  .r....r%...r(...
-00000720: 7230 0000 0072 2300 0000 7223 0000 0072  r0...r#...r#...r
-00000730: 2300 0000 7224 0000 0072 0d00 0000 0b00  #...r$...r......
-00000740: 0000 7308 0000 0008 0010 0110 0f14 0872  ..s............r
-00000750: 0d00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000760: 0000 0000 0003 0000 0040 0000 0073 3200  .........@...s2.
-00000770: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00000780: 6504 6505 6402 3c00 6506 6505 6403 3c00  e.e.d.<.e.e.d.<.
-00000790: 6507 6505 6404 3c00 6507 6505 6405 3c00  e.e.d.<.e.e.d.<.
-000007a0: 6406 5300 2907 da12 4765 7450 6173 7342  d.S.)...GetPassB
-000007b0: 7950 6572 736f 6e44 746f 75e5 0000 00d0  yPersonDtou.....
-000007c0: a2d0 b8d0 bf20 5061 7373 20d0 bfd1 80d0  ..... Pass .....
-000007d0: b5d0 b4d1 81d1 82d0 b0d0 b2d0 bbd1 8fd0  ................
-000007e0: b5d1 8220 d0ba d180 d0b0 d182 d0ba d0b8  ... ............
-000007f0: d0b9 20d0 bdd0 b0d0 b1d0 bed1 8020 d0b4  .. .......... ..
-00000800: d0b0 d0bd d0bd d18b d185 20d0 bfd0 b5d1  .......... .....
-00000810: 80d1 81d0 bed0 bdd0 b0d0 bbd1 8cd0 bdd0  ................
-00000820: bed0 b3d0 be20 d0bf d180 d0be d0bf d183  ..... ..........
-00000830: d181 d0ba d0b0 20d0 b8d0 bbd0 b820 d0b7  ...... ...... ..
-00000840: d0b0 d18f d0b2 d0ba d0b8 20d0 bdd0 b020  .......... .... 
-00000850: d0bf d180 d0be d0bf d183 d181 d0ba 2e0a  ................
-00000860: 2020 2020 6765 745f 6d61 7465 7269 616c      get_material
-00000870: 5f70 6173 735f 6279 5f70 6572 736f 6e0a  _pass_by_person.
-00000880: 2020 2020 6765 745f 6361 725f 7061 7373      get_car_pass
-00000890: 5f62 795f 7065 7273 6f6e 5f70 6173 730a  _by_person_pass.
-000008a0: 2020 2020 7227 0000 0072 0f00 0000 7218      r'...r....r.
-000008b0: 0000 00da 0a63 6172 6453 7461 7475 734e  .....cardStatusN
-000008c0: 2908 721c 0000 0072 1d00 0000 721e 0000  ).r....r....r...
-000008d0: 0072 1f00 0000 7221 0000 0072 2000 0000  .r....r!...r ...
-000008e0: 7209 0000 0072 2200 0000 7223 0000 0072  r....r"...r#...r
-000008f0: 2300 0000 7223 0000 0072 2400 0000 7231  #...r#...r$...r1
-00000900: 0000 002d 0000 0073 0c00 0000 0a00 0401  ...-...s........
-00000910: 0804 0801 0801 0c01 7231 0000 0063 0000  ........r1...c..
-00000920: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000930: 0000 4000 0000 733e 0000 0065 005a 0164  ..@...s>...e.Z.d
-00000940: 005a 0255 0064 015a 0365 0465 0564 023c  .Z.U.d.Z.e.e.d.<
-00000950: 0064 015a 0665 0765 0564 033c 0064 015a  .d.Z.e.e.d.<.d.Z
-00000960: 0865 0765 0564 043c 0064 015a 0965 0a65  .e.e.d.<.d.Z.e.e
-00000970: 0564 053c 0064 0653 0029 07da 0743 6172  .d.<.d.S.)...Car
-00000980: 6444 746f 7210 0000 00da 0963 6172 645f  dDtor......card_
-00000990: 636f 6465 da09 6461 7465 5f66 726f 6dda  code..date_from.
-000009a0: 0764 6174 655f 746f da0a 7769 7468 5f70  .date_to..with_p
-000009b0: 686f 746f 4e29 0b72 1c00 0000 721d 0000  hotoN).r....r...
-000009c0: 0072 1e00 0000 7234 0000 0072 2100 0000  .r....r4...r!...
-000009d0: 7220 0000 0072 3500 0000 7202 0000 0072  r ...r5...r....r
-000009e0: 3600 0000 7237 0000 0072 2f00 0000 7223  6...r7...r/...r#
-000009f0: 0000 0072 2300 0000 7223 0000 0072 2400  ...r#...r#...r$.
-00000a00: 0000 7233 0000 0038 0000 0073 0a00 0000  ..r3...8...s....
-00000a10: 0a00 0c01 0c01 0c01 1001 7233 0000 0063  ..........r3...c
-00000a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000a30: 0300 0000 4000 0000 739a 0000 0065 005a  ....@...s....e.Z
-00000a40: 0164 005a 0255 0064 015a 0364 025a 0465  .d.Z.U.d.Z.d.Z.e
-00000a50: 0565 0664 033c 0064 025a 0765 0865 0664  .e.d.<.d.Z.e.e.d
-00000a60: 043c 0064 025a 0965 0a65 0664 053c 0064  .<.d.Z.e.e.d.<.d
-00000a70: 025a 0b65 0c65 0664 063c 0065 0d65 0664  .Z.e.e.d.<.e.e.d
-00000a80: 073c 0065 0d65 0664 083c 0064 025a 0e65  .<.e.e.d.<.d.Z.e
-00000a90: 0565 0664 093c 0065 0f65 1019 0065 0664  .e.d.<.e.e...e.d
-00000aa0: 0a3c 0065 1165 0664 0b3c 0065 0865 0664  .<.e.e.d.<.e.e.d
-00000ab0: 0c3c 0065 0865 0664 0d3c 0064 025a 1265  .<.e.e.d.<.d.Z.e
-00000ac0: 0865 0664 0e3c 0064 025a 1365 0865 0664  .e.d.<.d.Z.e.e.d
-00000ad0: 0f3c 0064 0253 0029 10da 0f4d 6174 5661  .<.d.S.)...MatVa
-00000ae0: 6c75 6550 6173 7344 746f 75c3 0100 00d0  luePassDtou.....
-00000af0: a2d0 b8d0 bf20 4d61 7456 616c 7565 5061  ..... MatValuePa
-00000b00: 7373 20d0 bfd1 80d0 b5d0 b4d1 81d1 82d0  ss .............
-00000b10: b0d0 b2d0 bbd1 8fd0 b5d1 8220 d181 d0be  ........... ....
-00000b20: d0b1 d0be d0b9 20d0 bdd0 b0d0 b1d0 bed1  ...... .........
-00000b30: 8020 d0b4 d0b0 d0bd d0bd d18b d185 20d0  . ............ .
-00000b40: bcd0 b0d1 82d0 b5d1 80d0 b8d0 b0d0 bbd1  ................
-00000b50: 8cd0 bdd0 bed0 b3d0 be20 d0bf d180 d0be  ......... ......
-00000b60: d0bf d183 d181 d0ba d0b0 20d0 b8d0 bbd0  .......... .....
-00000b70: b820 d0b7 d0b0 d18f d0b2 d0ba d0b8 20d0  . ............ .
-00000b80: bdd0 b00a d0bf d180 d0be d0bf d183 d181  ................
-00000b90: d0ba 2e20 d09e d0b1 d18a d0b5 d0ba d182  ... ............
-00000ba0: 20d1 82d0 b8d0 bfd0 b020 4d61 7456 616c   ........ MatVal
-00000bb0: 7565 5061 7373 20d0 b8d1 81d0 bfd0 bed0  uePass .........
-00000bc0: bbd1 8cd0 b7d1 83d0 b5d1 82d1 81d1 8f20  ............... 
-00000bd0: d0b2 20d0 bcd0 b5d1 82d0 bed0 b4d0 b0d1  .. .............
-00000be0: 8520 d181 d0be d0b7 d0b4 d0b0 d0bd d0b8  . ..............
-00000bf0: d18f 20d0 b820 d180 d0b5 d0b4 d0b0 d0ba  .. .. ..........
-00000c00: d182 d0b8 d180 d0be d0b2 d0b0 d0bd d0b8  ................
-00000c10: d18f 2c20 d0b0 20d1 82d0 b0d0 bad0 b6d0  .., .. .........
-00000c20: b50a d0bf d0be d0bb d183 d187 d0b5 d0bd  ................
-00000c30: d0b8 d18f 20d1 81d0 bfd0 b8d1 81d0 bad0  .... ...........
-00000c40: bed0 b220 d0bc d0b0 d182 d0b5 d180 d0b8  ... ............
-00000c50: d0b0 d0bb d18c d0bd d18b d185 20d0 bfd1  ............ ...
-00000c60: 80d0 bed0 bfd1 83d1 81d0 bad0 bed0 b220  ............... 
-00000c70: d0b8 20d0 b7d0 b0d1 8fd0 b2d0 bed0 ba20  .. ............ 
-00000c80: 4765 744d 5650 6173 7365 732c 2047 6574  GetMVPasses, Get
-00000c90: 4d56 5061 7373 6573 4279 5065 7273 6f6e  MVPassesByPerson
-00000ca0: 5061 7373 20d0 b80a 5075 744d 5650 6173  Pass ...PutMVPas
-00000cb0: 732e 4eda 0269 64da 0770 6173 734e 756d  s.N..id..passNum
-00000cc0: 721a 0000 00da 096d 6174 5065 7273 6f6e  r......matPerson
-00000cd0: da08 746f 4578 706f 7274 da08 746f 496d  ..toExport..toIm
-00000ce0: 706f 7274 da06 7374 6174 7573 da09 6d61  port..status..ma
-00000cf0: 7456 616c 7565 73da 0450 6173 73da 0973  tValues..Pass..s
-00000d00: 7461 7274 4461 7465 da07 656e 6444 6174  tartDate..endDat
-00000d10: 65da 1067 6f61 6c4f 7267 616e 697a 6174  e..goalOrganizat
-00000d20: 696f 6eda 0e67 6f61 6c44 6570 6172 746d  ion..goalDepartm
-00000d30: 656e 7429 1472 1c00 0000 721d 0000 0072  ent).r....r....r
-00000d40: 1e00 0000 721f 0000 0072 3900 0000 7222  ....r....r9...r"
-00000d50: 0000 0072 2000 0000 723a 0000 0072 2100  ...r ...r:...r!.
-00000d60: 0000 721a 0000 0072 0200 0000 723b 0000  ..r....r....r;..
-00000d70: 0072 0900 0000 722f 0000 0072 3e00 0000  .r....r/...r>...
-00000d80: 7203 0000 0072 0a00 0000 720c 0000 0072  r....r....r....r
-00000d90: 4300 0000 7244 0000 0072 2300 0000 7223  C...rD...r#...r#
-00000da0: 0000 0072 2300 0000 7224 0000 0072 3800  ...r#...r$...r8.
-00000db0: 0000 3f00 0000 731e 0000 000a 0004 010c  ..?...s.........
-00000dc0: 050c 010c 010c 0108 0108 010c 010c 0108  ................
-00000dd0: 0108 0108 010c 0110 0172 3800 0000 6300  .........r8...c.
-00000de0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
-00000df0: 0000 0040 0000 0073 6600 0000 6500 5a01  ...@...sf...e.Z.
-00000e00: 6400 5a02 5500 6401 5a03 6402 5a04 6505  d.Z.U.d.Z.d.Z.e.
-00000e10: 6506 6403 3c00 6402 5a07 6508 6506 6404  e.d.<.d.Z.e.e.d.
-00000e20: 3c00 6402 5a09 6508 6506 6405 3c00 6402  <.d.Z.e.e.d.<.d.
-00000e30: 5a0a 6505 6506 6406 3c00 650b 650c 1900  Z.e.e.d.<.e.e...
-00000e40: 6506 6407 3c00 650d 6506 6408 3c00 6508  e.d.<.e.e.d.<.e.
-00000e50: 6506 6409 3c00 6508 6506 640a 3c00 6402  e.d.<.e.e.d.<.d.
-00000e60: 5300 290b da0a 4361 7250 6173 7344 746f  S.)...CarPassDto
-00000e70: 75bb 0100 00d0 a2d0 b8d0 bf20 4361 7250  u.......... CarP
-00000e80: 6173 7320 d0bf d180 d0b5 d0b4 d181 d182  ass ............
-00000e90: d0b0 d0b2 d0bb d18f d0b5 d182 20d1 81d0  ............ ...
-00000ea0: bed0 b1d0 bed0 b920 d0bd d0b0 d0b1 d0be  ....... ........
-00000eb0: d180 20d0 b4d0 b0d0 bdd0 bdd1 8bd1 8520  .. ............ 
-00000ec0: d182 d180 d0b0 d0bd d181 d0bf d0be d180  ................
-00000ed0: d182 d0bd d0be d0b3 d0be 20d0 bfd1 80d0  .......... .....
-00000ee0: bed0 bfd1 83d1 81d0 bad0 b020 d0b8 d0bb  ........... ....
-00000ef0: d0b8 20d0 b7d0 b0d1 8fd0 b2d0 bad0 b820  .. ............ 
-00000f00: d0bd d0b0 20d0 bfd1 80d0 bed0 bfd1 83d1  .... ...........
-00000f10: 81d0 ba2e 0ad0 9ed0 b1d1 8ad0 b5d0 bad1  ................
-00000f20: 8220 d182 d0b8 d0bf d0b0 2043 6172 5061  . ........ CarPa
-00000f30: 7373 20d0 b8d1 81d0 bfd0 bed0 bbd1 8cd0  ss .............
-00000f40: b7d1 83d0 b5d1 82d1 81d1 8f20 d0b2 20d0  ........... .. .
-00000f50: bcd0 b5d1 82d0 bed0 b4d0 b0d1 8520 d181  ............. ..
-00000f60: d0be d0b7 d0b4 d0b0 d0bd d0b8 d18f 20d0  .............. .
-00000f70: b820 d180 d0b5 d0b4 d0b0 d0ba d182 d0b8  . ..............
-00000f80: d180 d0be d0b2 d0b0 d0bd d0b8 d18f 2c20  .............., 
-00000f90: d0b0 20d1 82d0 b0d0 bad0 b6d0 b520 d0bf  .. .......... ..
-00000fa0: d0be d0bb d183 d187 d0b5 d0bd d0b8 d18f  ................
-00000fb0: 0ad1 81d0 bfd0 b8d1 81d0 bad0 bed0 b220  ............... 
-00000fc0: d182 d180 d0b0 d0bd d181 d0bf d0be d180  ................
-00000fd0: d182 d0bd d18b d185 20d0 bfd1 80d0 bed0  ........ .......
-00000fe0: bfd1 83d1 81d0 bad0 bed0 b220 d0b8 20d0  ........... .. .
-00000ff0: b7d0 b0d1 8fd0 b2d0 bed0 ba20 4765 7443  ........... GetC
-00001000: 6172 5061 7373 6573 2c20 4765 7443 6172  arPasses, GetCar
-00001010: 5061 7373 6573 4279 5065 7273 6f6e 5061  PassesByPersonPa
-00001020: 7373 20d0 b820 5075 7443 6172 5061 7373  ss .. PutCarPass
-00001030: 4e72 3900 0000 723a 0000 00da 0a64 6174  Nr9...r:.....dat
-00001040: 6543 7265 6174 6572 3e00 0000 da04 6361  eCreater>.....ca
-00001050: 7273 7240 0000 0072 4100 0000 7242 0000  rsr@...rA...rB..
-00001060: 0029 0e72 1c00 0000 721d 0000 0072 1e00  .).r....r....r..
-00001070: 0000 721f 0000 0072 3900 0000 7222 0000  ..r....r9...r"..
-00001080: 0072 2000 0000 723a 0000 0072 2100 0000  .r ...r:...r!...
-00001090: 7246 0000 0072 3e00 0000 7203 0000 0072  rF...r>...r....r
-000010a0: 0b00 0000 720c 0000 0072 2300 0000 7223  ....r....r#...r#
-000010b0: 0000 0072 2300 0000 7224 0000 0072 4500  ...r#...r$...rE.
-000010c0: 0000 5400 0000 7314 0000 000a 0004 010c  ..T...s.........
-000010d0: 030c 010c 010c 010c 0108 0108 010c 0172  ...............r
-000010e0: 4500 0000 6300 0000 0000 0000 0000 0000  E...c...........
-000010f0: 0000 0000 0003 0000 0040 0000 0073 5200  .........@...sR.
-00001100: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00001110: 6504 6505 6402 3c00 6506 6505 6403 3c00  e.e.d.<.e.e.d.<.
-00001120: 6507 6505 6404 3c00 6504 6505 6405 3c00  e.e.d.<.e.e.d.<.
-00001130: 6508 6505 6406 3c00 6508 6505 6407 3c00  e.e.d.<.e.e.d.<.
-00001140: 6504 6505 6408 3c00 6504 6505 6409 3c00  e.e.d.<.e.e.d.<.
-00001150: 640a 5300 290b da0c 4361 7264 4576 656e  d.S.)...CardEven
-00001160: 7444 746f 7509 0100 00d0 a2d0 b8d0 bf20  tDtou.......... 
-00001170: 4361 7264 4576 656e 7420 d0bf d180 d0b5  CardEvent ......
-00001180: d0b4 d181 d182 d0b0 d0b2 d0bb d18f d0b5  ................
-00001190: d182 20d1 81d0 bed0 b1d0 bed0 b920 d0bd  .. .......... ..
-000011a0: d0b0 d0b1 d0be d180 20d0 b4d0 b0d0 bdd0  ........ .......
-000011b0: bdd1 8bd1 8520 d0be 20d1 81d0 bed0 b1d1  ..... .. .......
-000011c0: 8bd1 82d0 b8d0 b82c 20d0 bfd1 80d0 bed0  ......., .......
-000011d0: b8d0 b7d0 bed1 88d0 b5d0 b4d1 88d0 b5d0  ................
-000011e0: bc20 d181 20d0 bad0 b0d1 80d1 82d0 bed0  . .. ...........
-000011f0: b920 d0b4 d0be d181 d182 d183 d0bf d0b0  . ..............
-00001200: 2e0a 2020 2020 2020 2020 d098 d181 d0bf  ..        ......
-00001210: d0be d0bb d18c d0b7 d183 d0b5 d182 d181  ................
-00001220: d18f 20d0 b220 d0bc d0b5 d182 d0be d0b4  .. .. ..........
-00001230: d0b5 20d0 bfd0 bed0 bbd1 83d1 87d0 b5d0  .. .............
-00001240: bdd0 b8d1 8f20 d181 d0be d0b1 d18b d182  ..... ..........
-00001250: d0b8 d18f 20d1 8120 d0ba d0b0 d180 d182  .... .. ........
-00001260: d0be d0b9 2047 6574 4361 7264 4576 656e  .... GetCardEven
-00001270: 7473 7227 0000 00da 0a65 6e74 7279 506f  tsr'.....entryPo
-00001280: 696e 74da 0864 6174 6554 696d 65da 076d  int..dateTime..m
-00001290: 7367 5465 7874 da07 6d73 6743 6f64 65da  sgText..msgCode.
-000012a0: 076d 7367 5479 7065 da08 636f 6d6d 656e  .msgType..commen
-000012b0: 7473 da05 7068 6f74 6f4e 2909 721c 0000  ts..photoN).r...
-000012c0: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-000012d0: 7221 0000 0072 2000 0000 7206 0000 0072  r!...r ...r....r
-000012e0: 0200 0000 7222 0000 0072 2300 0000 7223  ....r"...r#...r#
-000012f0: 0000 0072 2300 0000 7224 0000 0072 4800  ...r#...r$...rH.
-00001300: 0000 6200 0000 7314 0000 000a 0004 0108  ..b...s.........
-00001310: 0208 0108 0108 0108 0108 0108 010c 0172  ...............r
-00001320: 4800 0000 6300 0000 0000 0000 0000 0000  H...c...........
-00001330: 0000 0000 0003 0000 0040 0000 0073 4200  .........@...sB.
-00001340: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-00001350: 6504 6505 6402 3c00 6506 6505 6403 3c00  e.e.d.<.e.e.d.<.
-00001360: 6507 6505 6404 3c00 6504 6505 6405 3c00  e.e.d.<.e.e.d.<.
-00001370: 6504 6505 6406 3c00 6504 6505 6407 3c00  e.e.d.<.e.e.d.<.
-00001380: 6408 5300 2909 da0d 4174 7465 6e64 616e  d.S.)...Attendan
-00001390: 6365 4474 6f75 6500 0000 d0bf d180 d0b5  ceDtoue.........
-000013a0: d0b4 d181 d182 d0b0 d0b2 d0bb d18f d0b5  ................
-000013b0: d182 20d1 81d0 bed0 b1d0 bed0 b920 d0b4  .. .......... ..
-000013c0: d0b0 d0bd d0bd d18b d0b5 20d0 be20 d0bf  .......... .. ..
-000013d0: d0be d181 d0b5 d189 d0b5 d0bd d0b8 d0b8  ................
-000013e0: 20d1 8120 d0ba d0b0 d180 d182 d0be d0b9   .. ............
-000013f0: 20d0 b4d0 bed1 81d1 82d1 83d0 bfd0 b072   ..............r
-00001400: 2700 0000 da0a 6973 456e 7472 616e 6365  '.....isEntrance
-00001410: 724a 0000 0072 4e00 0000 da08 6374 726c  rJ...rN.....ctrl
-00001420: 4172 6561 da07 7461 626c 656e 6f4e 2908  Area..tablenoN).
-00001430: 721c 0000 0072 1d00 0000 721e 0000 0072  r....r....r....r
-00001440: 1f00 0000 7221 0000 0072 2000 0000 722f  ....r!...r ...r/
-00001450: 0000 0072 0200 0000 7223 0000 0072 2300  ...r....r#...r#.
-00001460: 0000 7223 0000 0072 2400 0000 7250 0000  ..r#...r$...rP..
-00001470: 006f 0000 0073 1000 0000 0a00 0401 0801  .o...s..........
-00001480: 0801 0801 0801 0801 0c01 7250 0000 004e  ..........rP...N
-00001490: 2917 7202 0000 00da 0674 7970 696e 6772  ).r......typingr
-000014a0: 0300 0000 da08 7079 6461 6e74 6963 7204  ......pydanticr.
-000014b0: 0000 00da 1e73 7263 2e62 6173 7469 6f6e  .....src.bastion
-000014c0: 5f61 7069 2e64 746f 2e70 6572 736f 6e5f  _api.dto.person_
-000014d0: 6474 6f72 0500 0000 da1e 7372 632e 6261  dtor......src.ba
-000014e0: 7374 696f 6e5f 6170 692e 6474 6f2e 706f  stion_api.dto.po
-000014f0: 696e 7473 5f64 746f 7206 0000 0072 0700  ints_dtor....r..
-00001500: 0000 da1b 7372 632e 6261 7374 696f 6e5f  ....src.bastion_
-00001510: 6170 692e 6474 6f2e 7375 7070 6f72 7472  api.dto.supportr
-00001520: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
-00001530: 0000 0072 0c00 0000 720d 0000 0072 3100  ...r....r....r1.
-00001540: 0000 7233 0000 0072 3800 0000 7245 0000  ..r3...r8...rE..
-00001550: 0072 4800 0000 7250 0000 0072 2300 0000  .rH...rP...r#...
-00001560: 7223 0000 0072 2300 0000 7224 0000 00da  r#...r#...r$....
-00001570: 083c 6d6f 6475 6c65 3e01 0000 0073 1a00  .<module>....s..
-00001580: 0000 0c00 0c01 0c02 0c02 1001 1c01 0e03  ................
-00001590: 1022 100b 1007 1015 100e 140d            ."..........
+00000400: 7223 0000 0072 2300 0000 fa51 2f68 6f6d  r#...r#....Q/hom
+00000410: 652f 6b6f 726f 676f 642f 5079 6368 6172  e/korogod/Pychar
+00000420: 6d50 726f 6a65 6374 732f 4261 7374 696f  mProjects/Bastio
+00000430: 6e5f 696e 7465 6772 6174 696f 6e2f 7372  n_integration/sr
+00000440: 632f 6261 7374 696f 6e5f 6170 692f 6474  c/bastion_api/dt
+00000450: 6f2f 7061 7373 5f64 746f 2e70 79da 0d4e  o/pass_dto.py..N
+00000460: 6577 5061 7373 5065 7273 6f6e 1100 0000  ewPassPerson....
+00000470: 731c 0000 000a 0004 0108 0110 0110 0108  s...............
+00000480: 0108 010c 010c 010c 0108 010c 010c 0110  ................
+00000490: 0172 2500 0000 6300 0000 0000 0000 0000  .r%...c.........
+000004a0: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+000004b0: 3600 0000 6500 5a01 6400 5a02 5500 6401  6...e.Z.d.Z.U.d.
+000004c0: 5a03 6402 5a04 6505 6506 6403 3c00 6507  Z.d.Z.e.e.d.<.e.
+000004d0: 6506 6404 3c00 6508 6506 6405 3c00 6505  e.d.<.e.e.d.<.e.
+000004e0: 6506 6406 3c00 6407 5300 2908 7a1d 5061  e.d.<.d.S.).z.Pa
+000004f0: 7373 4474 6f2e 5265 7475 726e 5061 7373  ssDto.ReturnPass
+00000500: 466f 7243 6172 6443 6f64 65da 1472 6574  ForCardCode..ret
+00000510: 7572 6e5f 7061 7373 5f66 6f72 5f63 6172  urn_pass_for_car
+00000520: 6472 1000 0000 da08 6361 7264 436f 6465  dr......cardCode
+00000530: 720f 0000 0072 1400 0000 7213 0000 004e  r....r....r....N
+00000540: 2909 721c 0000 0072 1d00 0000 721e 0000  ).r....r....r...
+00000550: 0072 1f00 0000 7227 0000 0072 2100 0000  .r....r'...r!...
+00000560: 7220 0000 0072 0500 0000 7222 0000 0072  r ...r....r"...r
+00000570: 2300 0000 7223 0000 0072 2300 0000 7224  #...r#...r#...r$
+00000580: 0000 00da 1552 6574 7572 6e50 6173 7346  .....ReturnPassF
+00000590: 6f72 4361 7264 436f 6465 2000 0000 730c  orCardCode ...s.
+000005a0: 0000 000a 0004 010c 0108 0108 010c 0172  ...............r
+000005b0: 2800 0000 6300 0000 0000 0000 0000 0000  (...c...........
+000005c0: 0000 0000 0003 0000 0040 0000 0073 4e00  .........@...sN.
+000005d0: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+000005e0: 6402 5a04 6505 6506 6403 3c00 6402 5a07  d.Z.e.e.d.<.d.Z.
+000005f0: 6505 6506 6404 3c00 6402 5a08 6509 6506  e.e.d.<.d.Z.e.e.
+00000600: 6405 3c00 6402 5a0a 6505 6506 6406 3c00  d.<.d.Z.e.e.d.<.
+00000610: 6402 5a0b 6505 6506 6407 3c00 6408 5300  d.Z.e.e.d.<.d.S.
+00000620: 2909 7a12 5061 7373 4474 6f2e 5265 7475  ).z.PassDto.Retu
+00000630: 726e 5061 7373 da08 6765 745f 7061 7373  rnPass..get_pass
+00000640: 7210 0000 00da 0b63 6172 645f 7374 6174  r......card_stat
+00000650: 7573 da09 7061 7373 5f74 7970 65da 0d77  us..pass_type..w
+00000660: 6974 686f 7574 5f70 686f 746f da0b 7374  ithout_photo..st
+00000670: 6172 745f 6e75 6d65 72da 096d 6178 5f63  art_numer..max_c
+00000680: 6f75 6e74 4e29 0c72 1c00 0000 721d 0000  ountN).r....r...
+00000690: 0072 1e00 0000 721f 0000 0072 2a00 0000  .r....r....r*...
+000006a0: 7222 0000 0072 2000 0000 722b 0000 0072  r"...r ...r+...r
+000006b0: 2c00 0000 da04 626f 6f6c 722d 0000 0072  ,.....boolr-...r
+000006c0: 2e00 0000 7223 0000 0072 2300 0000 7223  ....r#...r#...r#
+000006d0: 0000 0072 2400 0000 da0a 5265 7475 726e  ...r$.....Return
+000006e0: 5061 7373 2800 0000 730e 0000 000a 0004  Pass(...s.......
+000006f0: 010c 010c 010c 010c 0110 0172 3000 0000  ...........r0...
+00000700: 4e29 0772 1c00 0000 721d 0000 0072 1e00  N).r....r....r..
+00000710: 0000 7204 0000 0072 2500 0000 7228 0000  ..r....r%...r(..
+00000720: 0072 3000 0000 7223 0000 0072 2300 0000  .r0...r#...r#...
+00000730: 7223 0000 0072 2400 0000 720d 0000 0010  r#...r$...r.....
+00000740: 0000 0073 0800 0000 0800 1001 100f 1408  ...s............
+00000750: 720d 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00000760: 0000 0000 0000 0300 0000 4000 0000 7332  ..........@...s2
+00000770: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+00000780: 0365 0465 0564 023c 0065 0665 0564 033c  .e.e.d.<.e.e.d.<
+00000790: 0065 0765 0564 043c 0065 0765 0564 053c  .e.e.d.<.e.e.d.<
+000007a0: 0064 0653 0029 07da 1247 6574 5061 7373  .d.S.)...GetPass
+000007b0: 4279 5065 7273 6f6e 4474 6f75 e500 0000  ByPersonDtou....
+000007c0: d0a2 d0b8 d0bf 2050 6173 7320 d0bf d180  ...... Pass ....
+000007d0: d0b5 d0b4 d181 d182 d0b0 d0b2 d0bb d18f  ................
+000007e0: d0b5 d182 20d0 bad1 80d0 b0d1 82d0 bad0  .... ...........
+000007f0: b8d0 b920 d0bd d0b0 d0b1 d0be d180 20d0  ... .......... .
+00000800: b4d0 b0d0 bdd0 bdd1 8bd1 8520 d0bf d0b5  ........... ....
+00000810: d180 d181 d0be d0bd d0b0 d0bb d18c d0bd  ................
+00000820: d0be d0b3 d0be 20d0 bfd1 80d0 bed0 bfd1  ...... .........
+00000830: 83d1 81d0 bad0 b020 d0b8 d0bb d0b8 20d0  ....... ...... .
+00000840: b7d0 b0d1 8fd0 b2d0 bad0 b820 d0bd d0b0  ........... ....
+00000850: 20d0 bfd1 80d0 bed0 bfd1 83d1 81d0 ba2e   ...............
+00000860: 0a20 2020 2067 6574 5f6d 6174 6572 6961  .    get_materia
+00000870: 6c5f 7061 7373 5f62 795f 7065 7273 6f6e  l_pass_by_person
+00000880: 0a20 2020 2067 6574 5f63 6172 5f70 6173  .    get_car_pas
+00000890: 735f 6279 5f70 6572 736f 6e5f 7061 7373  s_by_person_pass
+000008a0: 0a20 2020 2072 2700 0000 720f 0000 0072  .    r'...r....r
+000008b0: 1800 0000 da0a 6361 7264 5374 6174 7573  ......cardStatus
+000008c0: 4e29 0872 1c00 0000 721d 0000 0072 1e00  N).r....r....r..
+000008d0: 0000 721f 0000 0072 2100 0000 7220 0000  ..r....r!...r ..
+000008e0: 0072 0900 0000 7222 0000 0072 2300 0000  .r....r"...r#...
+000008f0: 7223 0000 0072 2300 0000 7224 0000 0072  r#...r#...r$...r
+00000900: 3100 0000 3200 0000 730c 0000 000a 0004  1...2...s.......
+00000910: 0108 0408 0108 010c 0172 3100 0000 6300  .........r1...c.
+00000920: 0000 0000 0000 0000 0000 0000 0000 0003  ................
+00000930: 0000 0040 0000 0073 3e00 0000 6500 5a01  ...@...s>...e.Z.
+00000940: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
+00000950: 3c00 6401 5a06 6507 6505 6403 3c00 6401  <.d.Z.e.e.d.<.d.
+00000960: 5a08 6507 6505 6404 3c00 6401 5a09 650a  Z.e.e.d.<.d.Z.e.
+00000970: 6505 6405 3c00 6406 5300 2907 da07 4361  e.d.<.d.S.)...Ca
+00000980: 7264 4474 6f72 1000 0000 da09 6361 7264  rdDtor......card
+00000990: 5f63 6f64 65da 0964 6174 655f 6672 6f6d  _code..date_from
+000009a0: da07 6461 7465 5f74 6fda 0a77 6974 685f  ..date_to..with_
+000009b0: 7068 6f74 6f4e 290b 721c 0000 0072 1d00  photoN).r....r..
+000009c0: 0000 721e 0000 0072 3400 0000 7221 0000  ..r....r4...r!..
+000009d0: 0072 2000 0000 7235 0000 0072 0200 0000  .r ...r5...r....
+000009e0: 7236 0000 0072 3700 0000 722f 0000 0072  r6...r7...r/...r
+000009f0: 2300 0000 7223 0000 0072 2300 0000 7224  #...r#...r#...r$
+00000a00: 0000 0072 3300 0000 3d00 0000 730a 0000  ...r3...=...s...
+00000a10: 000a 000c 010c 010c 0110 0172 3300 0000  ...........r3...
+00000a20: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000a30: 0003 0000 0040 0000 0073 9a00 0000 6500  .....@...s....e.
+00000a40: 5a01 6400 5a02 5500 6401 5a03 6402 5a04  Z.d.Z.U.d.Z.d.Z.
+00000a50: 6505 6506 6403 3c00 6402 5a07 6508 6506  e.e.d.<.d.Z.e.e.
+00000a60: 6404 3c00 6402 5a09 650a 6506 6405 3c00  d.<.d.Z.e.e.d.<.
+00000a70: 6402 5a0b 650c 6506 6406 3c00 650d 6506  d.Z.e.e.d.<.e.e.
+00000a80: 6407 3c00 650d 6506 6408 3c00 6402 5a0e  d.<.e.e.d.<.d.Z.
+00000a90: 6505 6506 6409 3c00 650f 6510 1900 6506  e.e.d.<.e.e...e.
+00000aa0: 640a 3c00 6511 6506 640b 3c00 6508 6506  d.<.e.e.d.<.e.e.
+00000ab0: 640c 3c00 6508 6506 640d 3c00 6402 5a12  d.<.e.e.d.<.d.Z.
+00000ac0: 6508 6506 640e 3c00 6402 5a13 6508 6506  e.e.d.<.d.Z.e.e.
+00000ad0: 640f 3c00 6402 5300 2910 da0f 4d61 7456  d.<.d.S.)...MatV
+00000ae0: 616c 7565 5061 7373 4474 6f75 c301 0000  aluePassDtou....
+00000af0: d0a2 d0b8 d0bf 204d 6174 5661 6c75 6550  ...... MatValueP
+00000b00: 6173 7320 d0bf d180 d0b5 d0b4 d181 d182  ass ............
+00000b10: d0b0 d0b2 d0bb d18f d0b5 d182 20d1 81d0  ............ ...
+00000b20: bed0 b1d0 bed0 b920 d0bd d0b0 d0b1 d0be  ....... ........
+00000b30: d180 20d0 b4d0 b0d0 bdd0 bdd1 8bd1 8520  .. ............ 
+00000b40: d0bc d0b0 d182 d0b5 d180 d0b8 d0b0 d0bb  ................
+00000b50: d18c d0bd d0be d0b3 d0be 20d0 bfd1 80d0  .......... .....
+00000b60: bed0 bfd1 83d1 81d0 bad0 b020 d0b8 d0bb  ........... ....
+00000b70: d0b8 20d0 b7d0 b0d1 8fd0 b2d0 bad0 b820  .. ............ 
+00000b80: d0bd d0b0 0ad0 bfd1 80d0 bed0 bfd1 83d1  ................
+00000b90: 81d0 ba2e 20d0 9ed0 b1d1 8ad0 b5d0 bad1  .... ...........
+00000ba0: 8220 d182 d0b8 d0bf d0b0 204d 6174 5661  . ........ MatVa
+00000bb0: 6c75 6550 6173 7320 d0b8 d181 d0bf d0be  luePass ........
+00000bc0: d0bb d18c d0b7 d183 d0b5 d182 d181 d18f  ................
+00000bd0: 20d0 b220 d0bc d0b5 d182 d0be d0b4 d0b0   .. ............
+00000be0: d185 20d1 81d0 bed0 b7d0 b4d0 b0d0 bdd0  .. .............
+00000bf0: b8d1 8f20 d0b8 20d1 80d0 b5d0 b4d0 b0d0  ... .. .........
+00000c00: bad1 82d0 b8d1 80d0 bed0 b2d0 b0d0 bdd0  ................
+00000c10: b8d1 8f2c 20d0 b020 d182 d0b0 d0ba d0b6  ..., .. ........
+00000c20: d0b5 0ad0 bfd0 bed0 bbd1 83d1 87d0 b5d0  ................
+00000c30: bdd0 b8d1 8f20 d181 d0bf d0b8 d181 d0ba  ..... ..........
+00000c40: d0be d0b2 20d0 bcd0 b0d1 82d0 b5d1 80d0  .... ...........
+00000c50: b8d0 b0d0 bbd1 8cd0 bdd1 8bd1 8520 d0bf  ............. ..
+00000c60: d180 d0be d0bf d183 d181 d0ba d0be d0b2  ................
+00000c70: 20d0 b820 d0b7 d0b0 d18f d0b2 d0be d0ba   .. ............
+00000c80: 2047 6574 4d56 5061 7373 6573 2c20 4765   GetMVPasses, Ge
+00000c90: 744d 5650 6173 7365 7342 7950 6572 736f  tMVPassesByPerso
+00000ca0: 6e50 6173 7320 d0b8 0a50 7574 4d56 5061  nPass ...PutMVPa
+00000cb0: 7373 2e4e da02 6964 da07 7061 7373 4e75  ss.N..id..passNu
+00000cc0: 6d72 1a00 0000 da09 6d61 7450 6572 736f  mr......matPerso
+00000cd0: 6eda 0874 6f45 7870 6f72 74da 0874 6f49  n..toExport..toI
+00000ce0: 6d70 6f72 74da 0673 7461 7475 73da 096d  mport..status..m
+00000cf0: 6174 5661 6c75 6573 da04 5061 7373 da09  atValues..Pass..
+00000d00: 7374 6172 7444 6174 65da 0765 6e64 4461  startDate..endDa
+00000d10: 7465 da10 676f 616c 4f72 6761 6e69 7a61  te..goalOrganiza
+00000d20: 7469 6f6e da0e 676f 616c 4465 7061 7274  tion..goalDepart
+00000d30: 6d65 6e74 2914 721c 0000 0072 1d00 0000  ment).r....r....
+00000d40: 721e 0000 0072 1f00 0000 7239 0000 0072  r....r....r9...r
+00000d50: 2200 0000 7220 0000 0072 3a00 0000 7221  "...r ...r:...r!
+00000d60: 0000 0072 1a00 0000 7202 0000 0072 3b00  ...r....r....r;.
+00000d70: 0000 7209 0000 0072 2f00 0000 723e 0000  ..r....r/...r>..
+00000d80: 0072 0300 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00000d90: 7243 0000 0072 4400 0000 7223 0000 0072  rC...rD...r#...r
+00000da0: 2300 0000 7223 0000 0072 2400 0000 7238  #...r#...r$...r8
+00000db0: 0000 0044 0000 0073 1e00 0000 0a00 0401  ...D...s........
+00000dc0: 0c05 0c01 0c01 0c01 0801 0801 0c01 0c01  ................
+00000dd0: 0801 0801 0801 0c01 1001 7238 0000 0063  ..........r8...c
+00000de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000df0: 0300 0000 4000 0000 7366 0000 0065 005a  ....@...sf...e.Z
+00000e00: 0164 005a 0255 0064 015a 0364 025a 0465  .d.Z.U.d.Z.d.Z.e
+00000e10: 0565 0664 033c 0064 025a 0765 0865 0664  .e.d.<.d.Z.e.e.d
+00000e20: 043c 0064 025a 0965 0865 0664 053c 0064  .<.d.Z.e.e.d.<.d
+00000e30: 025a 0a65 0565 0664 063c 0065 0b65 0c19  .Z.e.e.d.<.e.e..
+00000e40: 0065 0664 073c 0065 0d65 0664 083c 0065  .e.d.<.e.e.d.<.e
+00000e50: 0865 0664 093c 0065 0865 0664 0a3c 0064  .e.d.<.e.e.d.<.d
+00000e60: 0253 0029 0bda 0a43 6172 5061 7373 4474  .S.)...CarPassDt
+00000e70: 6f75 bb01 0000 d0a2 d0b8 d0bf 2043 6172  ou.......... Car
+00000e80: 5061 7373 20d0 bfd1 80d0 b5d0 b4d1 81d1  Pass ...........
+00000e90: 82d0 b0d0 b2d0 bbd1 8fd0 b5d1 8220 d181  ............. ..
+00000ea0: d0be d0b1 d0be d0b9 20d0 bdd0 b0d0 b1d0  ........ .......
+00000eb0: bed1 8020 d0b4 d0b0 d0bd d0bd d18b d185  ... ............
+00000ec0: 20d1 82d1 80d0 b0d0 bdd1 81d0 bfd0 bed1   ...............
+00000ed0: 80d1 82d0 bdd0 bed0 b3d0 be20 d0bf d180  ........... ....
+00000ee0: d0be d0bf d183 d181 d0ba d0b0 20d0 b8d0  ............ ...
+00000ef0: bbd0 b820 d0b7 d0b0 d18f d0b2 d0ba d0b8  ... ............
+00000f00: 20d0 bdd0 b020 d0bf d180 d0be d0bf d183   .... ..........
+00000f10: d181 d0ba 2e0a d09e d0b1 d18a d0b5 d0ba  ................
+00000f20: d182 20d1 82d0 b8d0 bfd0 b020 4361 7250  .. ........ CarP
+00000f30: 6173 7320 d0b8 d181 d0bf d0be d0bb d18c  ass ............
+00000f40: d0b7 d183 d0b5 d182 d181 d18f 20d0 b220  ............ .. 
+00000f50: d0bc d0b5 d182 d0be d0b4 d0b0 d185 20d1  .............. .
+00000f60: 81d0 bed0 b7d0 b4d0 b0d0 bdd0 b8d1 8f20  ............... 
+00000f70: d0b8 20d1 80d0 b5d0 b4d0 b0d0 bad1 82d0  .. .............
+00000f80: b8d1 80d0 bed0 b2d0 b0d0 bdd0 b8d1 8f2c  ...............,
+00000f90: 20d0 b020 d182 d0b0 d0ba d0b6 d0b5 20d0   .. .......... .
+00000fa0: bfd0 bed0 bbd1 83d1 87d0 b5d0 bdd0 b8d1  ................
+00000fb0: 8f0a d181 d0bf d0b8 d181 d0ba d0be d0b2  ................
+00000fc0: 20d1 82d1 80d0 b0d0 bdd1 81d0 bfd0 bed1   ...............
+00000fd0: 80d1 82d0 bdd1 8bd1 8520 d0bf d180 d0be  ......... ......
+00000fe0: d0bf d183 d181 d0ba d0be d0b2 20d0 b820  ............ .. 
+00000ff0: d0b7 d0b0 d18f d0b2 d0be d0ba 2047 6574  ............ Get
+00001000: 4361 7250 6173 7365 732c 2047 6574 4361  CarPasses, GetCa
+00001010: 7250 6173 7365 7342 7950 6572 736f 6e50  rPassesByPersonP
+00001020: 6173 7320 d0b8 2050 7574 4361 7250 6173  ass .. PutCarPas
+00001030: 734e 7239 0000 0072 3a00 0000 da0a 6461  sNr9...r:.....da
+00001040: 7465 4372 6561 7465 723e 0000 00da 0463  teCreater>.....c
+00001050: 6172 7372 4000 0000 7241 0000 0072 4200  arsr@...rA...rB.
+00001060: 0000 290e 721c 0000 0072 1d00 0000 721e  ..).r....r....r.
+00001070: 0000 0072 1f00 0000 7239 0000 0072 2200  ...r....r9...r".
+00001080: 0000 7220 0000 0072 3a00 0000 7221 0000  ..r ...r:...r!..
+00001090: 0072 4600 0000 723e 0000 0072 0300 0000  .rF...r>...r....
+000010a0: 720c 0000 0072 0b00 0000 7223 0000 0072  r....r....r#...r
+000010b0: 2300 0000 7223 0000 0072 2400 0000 7245  #...r#...r$...rE
+000010c0: 0000 0059 0000 0073 1400 0000 0a00 0401  ...Y...s........
+000010d0: 0c03 0c01 0c01 0c01 0c01 0801 0801 0c01  ................
+000010e0: 7245 0000 0063 0000 0000 0000 0000 0000  rE...c..........
+000010f0: 0000 0000 0000 0300 0000 4000 0000 7352  ..........@...sR
+00001100: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+00001110: 0365 0465 0564 023c 0065 0665 0564 033c  .e.e.d.<.e.e.d.<
+00001120: 0065 0765 0564 043c 0065 0465 0564 053c  .e.e.d.<.e.e.d.<
+00001130: 0065 0865 0564 063c 0065 0865 0564 073c  .e.e.d.<.e.e.d.<
+00001140: 0065 0465 0564 083c 0065 0465 0564 093c  .e.e.d.<.e.e.d.<
+00001150: 0064 0a53 0029 0bda 0c43 6172 6445 7665  .d.S.)...CardEve
+00001160: 6e74 4474 6f75 0901 0000 d0a2 d0b8 d0bf  ntDtou..........
+00001170: 2043 6172 6445 7665 6e74 20d0 bfd1 80d0   CardEvent .....
+00001180: b5d0 b4d1 81d1 82d0 b0d0 b2d0 bbd1 8fd0  ................
+00001190: b5d1 8220 d181 d0be d0b1 d0be d0b9 20d0  ... .......... .
+000011a0: bdd0 b0d0 b1d0 bed1 8020 d0b4 d0b0 d0bd  ......... ......
+000011b0: d0bd d18b d185 20d0 be20 d181 d0be d0b1  ...... .. ......
+000011c0: d18b d182 d0b8 d0b8 2c20 d0bf d180 d0be  ........, ......
+000011d0: d0b8 d0b7 d0be d188 d0b5 d0b4 d188 d0b5  ................
+000011e0: d0bc 20d1 8120 d0ba d0b0 d180 d182 d0be  .. .. ..........
+000011f0: d0b9 20d0 b4d0 bed1 81d1 82d1 83d0 bfd0  .. .............
+00001200: b02e 0a20 2020 2020 2020 20d0 98d1 81d0  ...        .....
+00001210: bfd0 bed0 bbd1 8cd0 b7d1 83d0 b5d1 82d1  ................
+00001220: 81d1 8f20 d0b2 20d0 bcd0 b5d1 82d0 bed0  ... .. .........
+00001230: b4d0 b520 d0bf d0be d0bb d183 d187 d0b5  ... ............
+00001240: d0bd d0b8 d18f 20d1 81d0 bed0 b1d1 8bd1  ...... .........
+00001250: 82d0 b8d1 8f20 d181 20d0 bad0 b0d1 80d1  ..... .. .......
+00001260: 82d0 bed0 b920 4765 7443 6172 6445 7665  ..... GetCardEve
+00001270: 6e74 7372 2700 0000 da0a 656e 7472 7950  ntsr'.....entryP
+00001280: 6f69 6e74 da08 6461 7465 5469 6d65 da07  oint..dateTime..
+00001290: 6d73 6754 6578 74da 076d 7367 436f 6465  msgText..msgCode
+000012a0: da07 6d73 6754 7970 65da 0863 6f6d 6d65  ..msgType..comme
+000012b0: 6e74 73da 0570 686f 746f 4e29 0972 1c00  nts..photoN).r..
+000012c0: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+000012d0: 0072 2100 0000 7220 0000 0072 0600 0000  .r!...r ...r....
+000012e0: 7202 0000 0072 2200 0000 7223 0000 0072  r....r"...r#...r
+000012f0: 2300 0000 7223 0000 0072 2400 0000 7248  #...r#...r$...rH
+00001300: 0000 0067 0000 0073 1400 0000 0a00 0401  ...g...s........
+00001310: 0802 0801 0801 0801 0801 0801 0801 0c01  ................
+00001320: 7248 0000 0063 0000 0000 0000 0000 0000  rH...c..........
+00001330: 0000 0000 0000 0300 0000 4000 0000 7342  ..........@...sB
+00001340: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+00001350: 0365 0465 0564 023c 0065 0665 0564 033c  .e.e.d.<.e.e.d.<
+00001360: 0065 0765 0564 043c 0065 0465 0564 053c  .e.e.d.<.e.e.d.<
+00001370: 0065 0465 0564 063c 0065 0465 0564 073c  .e.e.d.<.e.e.d.<
+00001380: 0064 0853 0029 09da 0d41 7474 656e 6461  .d.S.)...Attenda
+00001390: 6e63 6544 746f 7565 0000 00d0 bfd1 80d0  nceDtoue........
+000013a0: b5d0 b4d1 81d1 82d0 b0d0 b2d0 bbd1 8fd0  ................
+000013b0: b5d1 8220 d181 d0be d0b1 d0be d0b9 20d0  ... .......... .
+000013c0: b4d0 b0d0 bdd0 bdd1 8bd0 b520 d0be 20d0  ........... .. .
+000013d0: bfd0 bed1 81d0 b5d1 89d0 b5d0 bdd0 b8d0  ................
+000013e0: b820 d181 20d0 bad0 b0d1 80d1 82d0 bed0  . .. ...........
+000013f0: b920 d0b4 d0be d181 d182 d183 d0bf d0b0  . ..............
+00001400: 7227 0000 00da 0a69 7345 6e74 7261 6e63  r'.....isEntranc
+00001410: 6572 4a00 0000 724e 0000 00da 0863 7472  erJ...rN.....ctr
+00001420: 6c41 7265 61da 0774 6162 6c65 6e6f 4e29  lArea..tablenoN)
+00001430: 0872 1c00 0000 721d 0000 0072 1e00 0000  .r....r....r....
+00001440: 721f 0000 0072 2100 0000 7220 0000 0072  r....r!...r ...r
+00001450: 2f00 0000 7202 0000 0072 2300 0000 7223  /...r....r#...r#
+00001460: 0000 0072 2300 0000 7224 0000 0072 5000  ...r#...r$...rP.
+00001470: 0000 7400 0000 7310 0000 000a 0004 0108  ..t...s.........
+00001480: 0108 0108 0108 0108 010c 0172 5000 0000  ...........rP...
+00001490: 4e29 1772 0200 0000 da06 7479 7069 6e67  N).r......typing
+000014a0: 7203 0000 00da 0870 7964 616e 7469 6372  r......pydanticr
+000014b0: 0400 0000 da1e 7372 632e 6261 7374 696f  ......src.bastio
+000014c0: 6e5f 6170 692e 6474 6f2e 7065 7273 6f6e  n_api.dto.person
+000014d0: 5f64 746f 7205 0000 00da 1e73 7263 2e62  _dtor......src.b
+000014e0: 6173 7469 6f6e 5f61 7069 2e64 746f 2e70  astion_api.dto.p
+000014f0: 6f69 6e74 735f 6474 6f72 0600 0000 7207  oints_dtor....r.
+00001500: 0000 00da 1b73 7263 2e62 6173 7469 6f6e  .....src.bastion
+00001510: 5f61 7069 2e64 746f 2e73 7570 706f 7274  _api.dto.support
+00001520: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00001530: 0b00 0000 720c 0000 0072 0d00 0000 7231  ....r....r....r1
+00001540: 0000 0072 3300 0000 7238 0000 0072 4500  ...r3...r8...rE.
+00001550: 0000 7248 0000 0072 5000 0000 7223 0000  ..rH...rP...r#..
+00001560: 0072 2300 0000 7223 0000 0072 2400 0000  .r#...r#...r$...
+00001570: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
+00001580: 0000 000c 000c 010c 020c 0210 011c 010e  ................
+00001590: 0810 2210 0b10 0710 1510 0e14 0d         .."..........
```

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/__pycache__/person_dto.cpython-310.pyc` & `bastion_api-0.3.0/src/bastion_api/dto/__pycache__/person_dto.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/__pycache__/points_dto.cpython-310.pyc` & `bastion_api-0.3.0/src/bastion_api/dto/__pycache__/points_dto.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May 16 14:17:31 2023 UTC, .py size: 2558 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7b90 6364 fe09 0000  o.......{.cd....
+00000000: 6f0d 0d0a 0000 0000 9181 6c64 fb09 0000  o.........ld....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 4700 6404 6405  ..d.e...Z.G.d.d.
 00000050: 8400 6405 6501 8303 5a03 4700 6406 6407  ..d.e...Z.G.d.d.
 00000060: 8400 6407 6501 8303 5a04 4700 6408 6409  ..d.e...Z.G.d.d.
 00000070: 8400 6409 6501 8303 5a05 640a 5300 290b  ..d.e...Z.d.S.).
@@ -22,121 +22,120 @@
 00000150: 4944 da0b 7375 6244 6576 6963 654e 6fda  ID..subDeviceNo.
 00000160: 0d73 7562 4465 7669 6365 4e61 6d65 4ea9  .subDeviceNameN.
 00000170: 07da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
 00000180: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
 00000190: 616d 655f 5fda 075f 5f64 6f63 5f5f da03  ame__..__doc__..
 000001a0: 7374 72da 0f5f 5f61 6e6e 6f74 6174 696f  str..__annotatio
 000001b0: 6e73 5f5f da03 696e 74a9 0072 1000 0000  ns__..int..r....
-000001c0: 7210 0000 00fa 522f 686f 6d65 2f64 6d69  r.....R/home/dmi
-000001d0: 7472 792f 5079 6368 6172 6d50 726f 6a65  try/PycharmProje
-000001e0: 6374 732f 4261 7374 696f 6e5f 696e 7465  cts/Bastion_inte
-000001f0: 6772 6174 696f 6e2f 7372 632f 6261 7374  gration/src/bast
-00000200: 696f 6e5f 6170 692f 6474 6f2f 706f 696e  ion_api/dto/poin
-00000210: 7473 5f64 746f 2e70 7972 0400 0000 0400  ts_dto.pyr......
-00000220: 0000 730a 0000 000a 0004 0108 0108 010c  ..s.............
-00000230: 0172 0400 0000 6300 0000 0000 0000 0000  .r....c.........
-00000240: 0000 0000 0000 0003 0000 0040 0000 0072  ...........@...r
-00000250: 0300 0000 2906 da0e 4163 6365 7373 4c65  ....)...AccessLe
-00000260: 7665 6c44 746f 75e3 0100 00d0 a2d0 b8d0  velDtou.........
-00000270: bf20 4163 6365 7373 4c65 7665 6c20 d0bf  . AccessLevel ..
-00000280: d180 d0b5 d0b4 d181 d182 d0b0 d0b2 d0bb  ................
-00000290: d18f d0b5 d182 20d1 81d0 bed0 b1d0 bed0  ...... .........
-000002a0: b920 d0bd d0b0 d0b1 d0be d180 20d0 b4d0  . .......... ...
-000002b0: b0d0 bdd0 bdd1 8bd1 8520 d183 d180 d0be  ......... ......
-000002c0: d0b2 d0bd d18f 20d0 b4d0 bed1 81d1 82d1  ...... .........
-000002d0: 83d0 bfd0 b02e 20d0 9ed0 b1d1 8ad0 b5d0  ...... .........
-000002e0: bad1 8220 d182 d0b8 d0bf d0b0 2041 6363  ... ........ Acc
-000002f0: 6573 734c 6576 656c 0a20 2020 20d0 b8d1  essLevel.    ...
-00000300: 81d0 bfd0 bed0 bbd1 8cd0 b7d1 83d0 b5d1  ................
-00000310: 82d1 81d1 8f20 d0b2 20d0 bcd0 b5d1 82d0  ..... .. .......
-00000320: bed0 b4d0 b520 d181 d0be d0b7 d0b4 d0b0  ..... ..........
-00000330: d0bd d0b8 d18f 2fd1 80d0 b5d0 b4d0 b0d0  ....../.........
-00000340: bad1 82d0 b8d1 80d0 bed0 b2d0 b0d0 bdd0  ................
-00000350: b8d1 8f20 d0bf d180 d0be d0bf d183 d181  ... ............
-00000360: d0ba d0b0 2fd0 b7d0 b0d1 8fd0 b2d0 bad0  ..../...........
-00000370: b820 d0bd d0b0 20d0 bfd1 80d0 bed0 bfd1  . .... .........
-00000380: 83d1 81d0 ba20 5075 7450 6173 732c 20d0  ..... PutPass, .
-00000390: b220 d0bc d0b5 d182 d0be d0b4 d0b5 0a20  . ............. 
-000003a0: 2020 20d0 bfd0 bed0 bbd1 83d1 87d0 b5d0     .............
-000003b0: bdd0 b8d1 8f20 d181 d0bf d0b8 d181 d0ba  ..... ..........
-000003c0: d0b0 20d0 bfd1 80d0 bed0 bfd1 83d1 81d0  .. .............
-000003d0: bad0 bed0 b220 4765 7450 6173 7365 732c  ..... GetPasses,
-000003e0: 20d1 82d0 b0d0 bad0 b6d0 b520 d0b2 20d0   .......... .. .
-000003f0: bcd0 b5d1 82d0 bed0 b4d0 b520 d0bf d0be  ........... ....
-00000400: d0bb d183 d187 d0b5 d0bd d0b8 d18f 20d1  .............. .
-00000410: 81d0 bfd0 b8d1 81d0 bad0 b020 d183 d180  ........... ....
-00000420: d0be d0b2 d0bd d0b5 d0b9 20d0 b4d0 bed1  .......... .....
-00000430: 81d1 82d1 83d0 bfd0 b00a 2020 2020 4765  ..........    Ge
-00000440: 7441 6363 6573 734c 6576 656c 7320 7205  tAccessLevels r.
-00000450: 0000 00da 0269 64da 046e 616d 654e 7208  .....id..nameNr.
-00000460: 0000 0072 1000 0000 7210 0000 0072 1000  ...r....r....r..
-00000470: 0000 7211 0000 0072 1200 0000 0b00 0000  ..r....r........
-00000480: 730a 0000 000a 0004 0108 0408 010c 0172  s..............r
-00000490: 1200 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000004a0: 0000 0000 0003 0000 0040 0000 0072 0300  .........@...r..
-000004b0: 0000 2906 da0e 436f 6e74 726f 6c41 7265  ..)...ControlAre
-000004c0: 6144 746f 757f 0100 00d0 a2d0 b8d0 bf20  aDtou.......... 
-000004d0: 436f 6e74 726f 6c41 7265 6120 d0bf d180  ControlArea ....
-000004e0: d0b5 d0b4 d181 d182 d0b0 d0b2 d0bb d18f  ................
-000004f0: d0b5 d182 20d1 81d0 bed0 b1d0 bed0 b920  .... .......... 
-00000500: d0bd d0b0 d0b1 d0be d180 20d0 b4d0 b0d0  .......... .....
-00000510: bdd0 bdd1 8bd1 8520 d0be d0b1 d0bb d0b0  ....... ........
-00000520: d181 d182 d0b5 d0b9 20d0 bad0 bed0 bdd1  ........ .......
-00000530: 82d1 80d0 bed0 bbd1 8f2e 20d0 98d1 81d0  .......... .....
-00000540: bfd0 bed0 bbd1 8cd0 b7d1 83d0 b5d1 82d1  ................
-00000550: 81d1 8f20 d0b2 20d0 bad0 b0d1 87d0 b5d1  ... .. .........
-00000560: 81d1 82d0 b2d0 b50a d0b2 d18b d185 d0be  ................
-00000570: d0b4 d0bd d0be d0b3 d0be 20d0 bfd0 b0d1  .......... .....
-00000580: 80d0 b0d0 bcd0 b5d1 82d1 80d0 b020 d0bc  ............. ..
-00000590: d0b5 d182 d0be d0b4 d0b0 2047 6574 436f  .......... GetCo
-000005a0: 6e74 726f 6c41 7265 6173 2c20 d0b2 d0be  ntrolAreas, ....
-000005b0: d0b7 d0b2 d180 d0b0 d189 d0b0 d18e d189  ................
-000005c0: d0b5 d0b3 d0be 20d0 bad0 bed0 bbd0 bbd0  ...... .........
-000005d0: b5d0 bad1 86d0 b8d1 8e20 d0be d0b1 d0bb  ......... ......
-000005e0: d0b0 d181 d182 d0b5 d0b9 20d0 bad0 bed0  .......... .....
-000005f0: bdd1 82d1 80d0 bed0 bbd1 8f2c 20d0 b00a  ..........., ...
-00000600: d182 d0b0 d0ba d0b6 d0b5 20d1 8fd0 b2d0  .......... .....
-00000610: bbd1 8fd0 b5d1 82d1 81d1 8f20 d0bf d0be  ........... ....
-00000620: d0bb d0b5 d0bc 20d1 82d0 b8d0 bfd0 b020  ...... ........ 
-00000630: d0b4 d0b0 d0bd d0bd d18b d185 2041 7474  ............ Att
-00000640: 656e 6461 6e63 652e da06 7365 7276 4964  endance...servId
-00000650: 7213 0000 0072 1400 0000 4e72 0800 0000  r....r....Nr....
-00000660: 7210 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-00000670: 1100 0000 7215 0000 0015 0000 00f3 0a00  ....r...........
-00000680: 0000 0a00 0401 0803 0801 0c01 7215 0000  ............r...
-00000690: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-000006a0: 0000 0300 0000 4000 0000 7203 0000 0029  ......@...r....)
-000006b0: 06da 0e41 6363 6573 7350 6f69 6e74 4474  ...AccessPointDt
-000006c0: 6f75 6d01 0000 4163 6365 7373 506f 696e  oum...AccessPoin
-000006d0: 7420 e280 9320 d0be d0b1 d18a d0b5 d0ba  t ... ..........
-000006e0: d182 2c20 d0bf d180 d0b5 d0b4 d181 d182  .., ............
-000006f0: d0b0 d0b2 d0bb d18f d18e d189 d0b8 d0b9  ................
-00000700: 20d1 82d0 bed1 87d0 bad1 8320 d0b4 d0be   .......... ....
-00000710: d181 d182 d183 d0bf d0b0 2028 d0b4 d0b2  .......... (....
-00000720: d0b5 d180 d18c 2c20 d0b2 d0be d180 d0be  ......, ........
-00000730: d182 d0b0 2c20 d182 d183 d180 d0bd d0b8  ...., ..........
-00000740: d0ba d0b5 d182 2920 d0b2 20d0 a1d0 9ad0  ......) .. .....
-00000750: a3d0 9420 d090 d09f d09a 0a20 2020 20c2  ... .......    .
-00000760: abd0 91d0 b0d1 81d1 82d0 b8d0 bed0 bd2d  ...............-
-00000770: 32c2 bb2e 20d0 98d1 81d0 bfd0 bed0 bbd1  2... ...........
-00000780: 8cd0 b7d1 83d0 b5d1 82d1 81d1 8f20 d0b2  ............. ..
-00000790: 20d0 bad0 b0d1 87d0 b5d1 81d1 82d0 b2d0   ...............
-000007a0: b520 d0b2 d18b d185 d0be d0b4 d0bd d0be  . ..............
-000007b0: d0b3 d0be 20d0 bfd0 b0d1 80d0 b0d0 bcd0  .... ...........
-000007c0: b5d1 82d1 80d0 b020 d0b2 20d0 bcd0 b5d1  ....... .. .....
-000007d0: 82d0 bed0 b4d0 b520 4765 7441 6363 6573  ....... GetAcces
-000007e0: 7350 6f69 6e74 732c 0a20 2020 20d0 b2d0  sPoints,.    ...
-000007f0: bed0 b7d0 b2d1 80d0 b0d1 89d0 b0d1 8ed1  ................
-00000800: 89d0 b5d0 bc20 d0ba d0be d0bb d0bb d0b5  ..... ..........
-00000810: d0ba d186 d0b8 d18e 20d1 82d0 bed1 87d0  ........ .......
-00000820: b5d0 ba20 d0b4 d0be d181 d182 d183 d0bf  ... ............
-00000830: d0b0 2eda 0773 5365 7276 4944 da0c 7353  .....sServID..sS
-00000840: 7562 4465 7669 6365 4e6f da0e 7353 7562  ubDeviceNo..sSub
-00000850: 4465 7669 6365 4e61 6d65 4e72 0800 0000  DeviceNameNr....
-00000860: 7210 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
-00000870: 1100 0000 7218 0000 001e 0000 0072 1700  ....r........r..
-00000880: 0000 7218 0000 004e 2906 da08 7079 6461  ..r....N)...pyda
-00000890: 6e74 6963 7202 0000 0072 0400 0000 7212  nticr....r....r.
-000008a0: 0000 0072 1500 0000 7218 0000 0072 1000  ...r....r....r..
-000008b0: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
-000008c0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000008d0: 0a00 0000 0c00 1003 1007 100a 1409       ..............
+000001c0: 7210 0000 00fa 532f 686f 6d65 2f6b 6f72  r.....S/home/kor
+000001d0: 6f67 6f64 2f50 7963 6861 726d 5072 6f6a  ogod/PycharmProj
+000001e0: 6563 7473 2f42 6173 7469 6f6e 5f69 6e74  ects/Bastion_int
+000001f0: 6567 7261 7469 6f6e 2f73 7263 2f62 6173  egration/src/bas
+00000200: 7469 6f6e 5f61 7069 2f64 746f 2f70 6f69  tion_api/dto/poi
+00000210: 6e74 735f 6474 6f2e 7079 7204 0000 0004  nts_dto.pyr.....
+00000220: 0000 0073 0a00 0000 0a00 0401 0801 0801  ...s............
+00000230: 0c01 7204 0000 0063 0000 0000 0000 0000  ..r....c........
+00000240: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000250: 7203 0000 0029 06da 0e41 6363 6573 734c  r....)...AccessL
+00000260: 6576 656c 4474 6f75 e301 0000 d0a2 d0b8  evelDtou........
+00000270: d0bf 2041 6363 6573 734c 6576 656c 20d0  .. AccessLevel .
+00000280: bfd1 80d0 b5d0 b4d1 81d1 82d0 b0d0 b2d0  ................
+00000290: bbd1 8fd0 b5d1 8220 d181 d0be d0b1 d0be  ....... ........
+000002a0: d0b9 20d0 bdd0 b0d0 b1d0 bed1 8020 d0b4  .. .......... ..
+000002b0: d0b0 d0bd d0bd d18b d185 20d1 83d1 80d0  .......... .....
+000002c0: bed0 b2d0 bdd1 8f20 d0b4 d0be d181 d182  ....... ........
+000002d0: d183 d0bf d0b0 2e20 d09e d0b1 d18a d0b5  ....... ........
+000002e0: d0ba d182 20d1 82d0 b8d0 bfd0 b020 4163  .... ........ Ac
+000002f0: 6365 7373 4c65 7665 6c0a 2020 2020 d0b8  cessLevel.    ..
+00000300: d181 d0bf d0be d0bb d18c d0b7 d183 d0b5  ................
+00000310: d182 d181 d18f 20d0 b220 d0bc d0b5 d182  ...... .. ......
+00000320: d0be d0b4 d0b5 20d1 81d0 bed0 b7d0 b4d0  ...... .........
+00000330: b0d0 bdd0 b8d1 8f2f d180 d0b5 d0b4 d0b0  ......./........
+00000340: d0ba d182 d0b8 d180 d0be d0b2 d0b0 d0bd  ................
+00000350: d0b8 d18f 20d0 bfd1 80d0 bed0 bfd1 83d1  .... ...........
+00000360: 81d0 bad0 b02f d0b7 d0b0 d18f d0b2 d0ba  ...../..........
+00000370: d0b8 20d0 bdd0 b020 d0bf d180 d0be d0bf  .. .... ........
+00000380: d183 d181 d0ba 2050 7574 5061 7373 2c20  ...... PutPass, 
+00000390: d0b2 20d0 bcd0 b5d1 82d0 bed0 b4d0 b50a  .. .............
+000003a0: 2020 2020 d0bf d0be d0bb d183 d187 d0b5      ............
+000003b0: d0bd d0b8 d18f 20d1 81d0 bfd0 b8d1 81d0  ...... .........
+000003c0: bad0 b020 d0bf d180 d0be d0bf d183 d181  ... ............
+000003d0: d0ba d0be d0b2 2047 6574 5061 7373 6573  ...... GetPasses
+000003e0: 2c20 d182 d0b0 d0ba d0b6 d0b5 20d0 b220  , .......... .. 
+000003f0: d0bc d0b5 d182 d0be d0b4 d0b5 20d0 bfd0  ............ ...
+00000400: bed0 bbd1 83d1 87d0 b5d0 bdd0 b8d1 8f20  ............... 
+00000410: d181 d0bf d0b8 d181 d0ba d0b0 20d1 83d1  ............ ...
+00000420: 80d0 bed0 b2d0 bdd0 b5d0 b920 d0b4 d0be  ........... ....
+00000430: d181 d182 d183 d0bf d0b0 0a20 2020 2047  ...........    G
+00000440: 6574 4163 6365 7373 4c65 7665 6c73 2072  etAccessLevels r
+00000450: 0500 0000 da02 6964 da04 6e61 6d65 4e72  ......id..nameNr
+00000460: 0800 0000 7210 0000 0072 1000 0000 7210  ....r....r....r.
+00000470: 0000 0072 1100 0000 7212 0000 000b 0000  ...r....r.......
+00000480: 0073 0a00 0000 0a00 0401 0804 0801 0c01  .s..............
+00000490: 7212 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000004a0: 0000 0000 0000 0300 0000 4000 0000 7203  ..........@...r.
+000004b0: 0000 0029 06da 0e43 6f6e 7472 6f6c 4172  ...)...ControlAr
+000004c0: 6561 4474 6f75 7f01 0000 d0a2 d0b8 d0bf  eaDtou..........
+000004d0: 2043 6f6e 7472 6f6c 4172 6561 20d0 bfd1   ControlArea ...
+000004e0: 80d0 b5d0 b4d1 81d1 82d0 b0d0 b2d0 bbd1  ................
+000004f0: 8fd0 b5d1 8220 d181 d0be d0b1 d0be d0b9  ..... ..........
+00000500: 20d0 bdd0 b0d0 b1d0 bed1 8020 d0b4 d0b0   .......... ....
+00000510: d0bd d0bd d18b d185 20d0 bed0 b1d0 bbd0  ........ .......
+00000520: b0d1 81d1 82d0 b5d0 b920 d0ba d0be d0bd  ......... ......
+00000530: d182 d180 d0be d0bb d18f 2e20 d098 d181  ........... ....
+00000540: d0bf d0be d0bb d18c d0b7 d183 d0b5 d182  ................
+00000550: d181 d18f 20d0 b220 d0ba d0b0 d187 d0b5  .... .. ........
+00000560: d181 d182 d0b2 d0b5 0ad0 b2d1 8bd1 85d0  ................
+00000570: bed0 b4d0 bdd0 bed0 b3d0 be20 d0bf d0b0  ........... ....
+00000580: d180 d0b0 d0bc d0b5 d182 d180 d0b0 20d0  .............. .
+00000590: bcd0 b5d1 82d0 bed0 b4d0 b020 4765 7443  ........... GetC
+000005a0: 6f6e 7472 6f6c 4172 6561 732c 20d0 b2d0  ontrolAreas, ...
+000005b0: bed0 b7d0 b2d1 80d0 b0d1 89d0 b0d1 8ed1  ................
+000005c0: 89d0 b5d0 b3d0 be20 d0ba d0be d0bb d0bb  ....... ........
+000005d0: d0b5 d0ba d186 d0b8 d18e 20d0 bed0 b1d0  .......... .....
+000005e0: bbd0 b0d1 81d1 82d0 b5d0 b920 d0ba d0be  ........... ....
+000005f0: d0bd d182 d180 d0be d0bb d18f 2c20 d0b0  ............, ..
+00000600: 0ad1 82d0 b0d0 bad0 b6d0 b520 d18f d0b2  ........... ....
+00000610: d0bb d18f d0b5 d182 d181 d18f 20d0 bfd0  ............ ...
+00000620: bed0 bbd0 b5d0 bc20 d182 d0b8 d0bf d0b0  ....... ........
+00000630: 20d0 b4d0 b0d0 bdd0 bdd1 8bd1 8520 4174   ............ At
+00000640: 7465 6e64 616e 6365 2eda 0673 6572 7649  tendance...servI
+00000650: 6472 1300 0000 7214 0000 004e 7208 0000  dr....r....Nr...
+00000660: 0072 1000 0000 7210 0000 0072 1000 0000  .r....r....r....
+00000670: 7211 0000 0072 1500 0000 1500 0000 f30a  r....r..........
+00000680: 0000 000a 0004 0108 0308 010c 0172 1500  .............r..
+00000690: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+000006a0: 0000 0003 0000 0040 0000 0072 0300 0000  .......@...r....
+000006b0: 2906 da0e 4163 6365 7373 506f 696e 7444  )...AccessPointD
+000006c0: 746f 756d 0100 0041 6363 6573 7350 6f69  toum...AccessPoi
+000006d0: 6e74 20e2 8093 20d0 bed0 b1d1 8ad0 b5d0  nt ... .........
+000006e0: bad1 822c 20d0 bfd1 80d0 b5d0 b4d1 81d1  ..., ...........
+000006f0: 82d0 b0d0 b2d0 bbd1 8fd1 8ed1 89d0 b8d0  ................
+00000700: b920 d182 d0be d187 d0ba d183 20d0 b4d0  . .......... ...
+00000710: bed1 81d1 82d1 83d0 bfd0 b020 28d0 b4d0  ........... (...
+00000720: b2d0 b5d1 80d1 8c2c 20d0 b2d0 bed1 80d0  ......., .......
+00000730: bed1 82d0 b02c 20d1 82d1 83d1 80d0 bdd0  ....., .........
+00000740: b8d0 bad0 b5d1 8229 20d0 b220 d0a1 d09a  .......) .. ....
+00000750: d0a3 d094 20d0 90d0 9fd0 9a0a 2020 2020  .... .......    
+00000760: c2ab d091 d0b0 d181 d182 d0b8 d0be d0bd  ................
+00000770: 2d32 c2bb 2e20 d098 d181 d0bf d0be d0bb  -2... ..........
+00000780: d18c d0b7 d183 d0b5 d182 d181 d18f 20d0  .............. .
+00000790: b220 d0ba d0b0 d187 d0b5 d181 d182 d0b2  . ..............
+000007a0: d0b5 20d0 b2d1 8bd1 85d0 bed0 b4d0 bdd0  .. .............
+000007b0: bed0 b3d0 be20 d0bf d0b0 d180 d0b0 d0bc  ..... ..........
+000007c0: d0b5 d182 d180 d0b0 20d0 b220 d0bc d0b5  ........ .. ....
+000007d0: d182 d0be d0b4 d0b5 2047 6574 4163 6365  ........ GetAcce
+000007e0: 7373 506f 696e 7473 2c0a 2020 2020 d0b2  ssPoints,.    ..
+000007f0: d0be d0b7 d0b2 d180 d0b0 d189 d0b0 d18e  ................
+00000800: d189 d0b5 d0bc 20d0 bad0 bed0 bbd0 bbd0  ...... .........
+00000810: b5d0 bad1 86d0 b8d1 8e20 d182 d0be d187  ......... ......
+00000820: d0b5 d0ba 20d0 b4d0 bed1 81d1 82d1 83d0  .... ...........
+00000830: bfd0 b02e 7205 0000 0072 0600 0000 7207  ....r....r....r.
+00000840: 0000 004e 7208 0000 0072 1000 0000 7210  ...Nr....r....r.
+00000850: 0000 0072 1000 0000 7211 0000 0072 1800  ...r....r....r..
+00000860: 0000 1e00 0000 7217 0000 0072 1800 0000  ......r....r....
+00000870: 4e29 06da 0870 7964 616e 7469 6372 0200  N)...pydanticr..
+00000880: 0000 7204 0000 0072 1200 0000 7215 0000  ..r....r....r...
+00000890: 0072 1800 0000 7210 0000 0072 1000 0000  .r....r....r....
+000008a0: 7210 0000 0072 1100 0000 da08 3c6d 6f64  r....r......<mod
+000008b0: 756c 653e 0100 0000 730a 0000 000c 0010  ule>....s.......
+000008c0: 0310 0710 0a14 09                        .......
```

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/__pycache__/support.cpython-310.pyc` & `bastion_api-0.3.0/src/bastion_api/dto/__pycache__/support.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May 16 14:20:20 2023 UTC, .py size: 4916 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2491 6364 3413 0000  o.......$.cd4...
+00000000: 6f0d 0d0a 0000 0000 14c6 6464 3413 0000  o.........dd4...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 4700 6404 6405  ..d.e...Z.G.d.d.
 00000050: 8400 6405 6501 8303 5a03 4700 6406 6407  ..d.e...Z.G.d.d.
 00000060: 8400 6407 6501 8303 5a04 4700 6408 6409  ..d.e...Z.G.d.d.
 00000070: 8400 6409 6501 8303 5a05 4700 640a 640b  ..d.e...Z.G.d.d.
@@ -29,252 +29,252 @@
 000001c0: d0b8 d0b9 2047 6574 4469 6374 5661 6c73  .... GetDictVals
 000001d0: da08 6361 7465 676f 7279 da05 7661 6c75  ..category..valu
 000001e0: 654e 2907 da08 5f5f 6e61 6d65 5f5f da0a  eN)...__name__..
 000001f0: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
 00000200: 616c 6e61 6d65 5f5f da07 5f5f 646f 635f  alname__..__doc_
 00000210: 5fda 0369 6e74 da0f 5f5f 616e 6e6f 7461  _..int..__annota
 00000220: 7469 6f6e 735f 5fda 0373 7472 a900 720d  tions__..str..r.
-00000230: 0000 0072 0d00 0000 fa4f 2f68 6f6d 652f  ...r.....O/home/
-00000240: 646d 6974 7279 2f50 7963 6861 726d 5072  dmitry/PycharmPr
-00000250: 6f6a 6563 7473 2f42 6173 7469 6f6e 5f69  ojects/Bastion_i
-00000260: 6e74 6567 7261 7469 6f6e 2f73 7263 2f62  ntegration/src/b
-00000270: 6173 7469 6f6e 5f61 7069 2f64 746f 2f73  astion_api/dto/s
-00000280: 7570 706f 7274 2e70 7972 0300 0000 0400  upport.pyr......
-00000290: 0000 7308 0000 000a 0004 0108 020c 0172  ..s............r
-000002a0: 0300 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000002b0: 0000 0000 0003 0000 0040 0000 0073 3a00  .........@...s:.
-000002c0: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
-000002d0: 6504 6505 6402 3c00 6504 6505 6403 3c00  e.e.d.<.e.e.d.<.
-000002e0: 6506 6505 6404 3c00 6506 6505 6405 3c00  e.e.d.<.e.e.d.<.
-000002f0: 6506 6505 6406 3c00 6407 5300 2908 da0f  e.e.d.<.d.S.)...
-00000300: 5469 6d65 496e 7465 7276 616c 4474 6f75  TimeIntervalDtou
-00000310: 4702 0000 d09e d0b1 d18a d0b5 d0ba d182  G...............
-00000320: 20d1 82d0 b8d0 bfd0 b020 5469 6d65 496e   ........ TimeIn
-00000330: 7465 7276 616c 20d0 bfd1 80d0 b5d0 b4d1  terval .........
-00000340: 81d1 82d0 b0d0 b2d0 bbd1 8fd0 b5d1 8220  ............... 
-00000350: d181 d0be d0b1 d0be d0b9 20d0 b2d1 80d0  .......... .....
-00000360: b5d0 bcd0 b5d0 bdd0 bdd0 bed0 b920 d0bf  ............. ..
-00000370: d180 d0be d0bc d0b5 d0b6 d183 d182 d0be  ................
-00000380: d0ba 2c20 d184 d0b8 d0b3 d183 d180 d0b8  .., ............
-00000390: d180 d183 d18e d189 d0b8 d0b9 20d0 b220  ............ .. 
-000003a0: d183 d180 d0be d0b2 d0bd d0b5 0ad0 b4d0  ................
-000003b0: bed1 81d1 82d1 83d0 bfd0 b02c 20d0 bfd1  ..........., ...
-000003c0: 80d0 b8d0 b2d1 8fd0 b7d0 b0d0 bdd0 bdd0  ................
-000003d0: bed0 bcd1 8320 d0ba 20d0 bfd1 80d0 bed0  ..... .. .......
-000003e0: bfd1 83d1 81d0 bad1 8320 d0b2 20d0 a1d0  ......... .. ...
-000003f0: 9ad0 a3d0 9420 d090 d09f d09a 20c2 abd0  ..... ...... ...
-00000400: 91d0 b0d1 81d1 82d0 b8d0 bed0 bd2d 32c2  .............-2.
-00000410: bb2e 20d0 9ed0 b1d1 8ad0 b5d0 bad1 8220  .. ............ 
-00000420: d182 d0b8 d0bf d0b0 2054 696d 6549 6e74  ........ TimeInt
-00000430: 6572 7661 6c20 d18f d0b2 d0bb d18f d0b5  erval ..........
-00000440: d182 d181 d18f 0ad0 bfd0 bed0 bbd0 b5d0  ................
-00000450: bc20 d0b2 20d1 82d0 b8d0 bfd0 b520 d0b4  . .. ........ ..
-00000460: d0b0 d0bd d0bd d18b d185 2050 6173 732c  .......... Pass,
-00000470: 20d0 b8d1 81d0 bfd0 bed0 bbd1 8cd0 b7d1   ...............
-00000480: 83d1 8ed1 89d0 b5d0 bcd1 81d1 8f20 d0b2  ............. ..
-00000490: 20d0 bcd0 b5d1 82d0 bed0 b4d0 b520 d181   ............ ..
-000004a0: d0be d0b7 d0b4 d0b0 d0bd d0b8 d18f 2fd1  ............../.
-000004b0: 80d0 b5d0 b4d0 b0d0 bad1 82d0 b8d1 80d0  ................
-000004c0: bed0 b2d0 b0d0 bdd0 b8d1 8f20 d0bf d180  ........... ....
-000004d0: d0be d0bf d183 d181 d0ba d0b0 2fd0 b7d0  ............/...
-000004e0: b0d1 8fd0 b2d0 bad0 b80a d0bd d0b0 20d0  .............. .
-000004f0: bfd1 80d0 bed0 bfd1 83d1 81d0 ba20 5075  ............. Pu
-00000500: 7450 6173 7320 d0b8 20d0 b220 d0bc d0b5  tPass .. .. ....
-00000510: d182 d0be d0b4 d0b5 20d0 bfd0 bed0 bbd1  ........ .......
-00000520: 83d1 87d0 b5d0 bdd0 b8d1 8f20 d0ba d0be  ........... ....
-00000530: d0bb d0bb d0b5 d0ba d186 d0b8 d0b8 20d0  .............. .
-00000540: bfd1 80d0 bed0 bfd1 83d1 81d0 bad0 bed0  ................
-00000550: b220 4765 7450 6173 7365 73da 0974 696d  . GetPasses..tim
-00000560: 6553 7461 7274 da07 7469 6d65 456e 64da  eStart..timeEnd.
-00000570: 0a69 6e53 6174 7572 6461 79da 0869 6e53  .inSaturday..inS
-00000580: 756e 6461 79da 0a69 6e48 6f6c 6964 6179  unday..inHoliday
-00000590: 734e 2907 7206 0000 0072 0700 0000 7208  sN).r....r....r.
-000005a0: 0000 0072 0900 0000 720c 0000 0072 0b00  ...r....r....r..
-000005b0: 0000 720a 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-000005c0: 0072 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-000005d0: 0d00 0000 730e 0000 000a 0004 0108 0408  ....s...........
-000005e0: 0108 0108 010c 0172 0f00 0000 6300 0000  .......r....c...
-000005f0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00000600: 0040 0000 0073 1601 0000 6500 5a01 6400  .@...s....e.Z.d.
-00000610: 5a02 5500 6401 5a03 6504 6505 6402 3c00  Z.U.d.Z.e.e.d.<.
-00000620: 6403 5a06 6504 6505 6404 3c00 6403 5a07  d.Z.e.e.d.<.d.Z.
-00000630: 6504 6505 6405 3c00 6403 5a08 6504 6505  e.e.d.<.d.Z.e.e.
-00000640: 6406 3c00 6403 5a09 6504 6505 6407 3c00  d.<.d.Z.e.e.d.<.
-00000650: 6403 5a0a 6504 6505 6408 3c00 6403 5a0b  d.Z.e.e.d.<.d.Z.
-00000660: 6504 6505 6409 3c00 6403 5a0c 6504 6505  e.e.d.<.d.Z.e.e.
-00000670: 640a 3c00 6403 5a0d 6504 6505 640b 3c00  d.<.d.Z.e.e.d.<.
-00000680: 6403 5a0e 6504 6505 640c 3c00 6403 5a0f  d.Z.e.e.d.<.d.Z.
-00000690: 6504 6505 640d 3c00 6403 5a10 6504 6505  e.e.d.<.d.Z.e.e.
-000006a0: 640e 3c00 6403 5a11 6504 6505 640f 3c00  d.<.d.Z.e.e.d.<.
-000006b0: 6403 5a12 6504 6505 6410 3c00 6403 5a13  d.Z.e.e.d.<.d.Z.
-000006c0: 6504 6505 6411 3c00 6403 5a14 6504 6505  e.e.d.<.d.Z.e.e.
-000006d0: 6412 3c00 6403 5a15 6504 6505 6413 3c00  d.<.d.Z.e.e.d.<.
-000006e0: 6403 5a16 6504 6505 6414 3c00 6403 5a17  d.Z.e.e.d.<.d.Z.
-000006f0: 6504 6505 6415 3c00 6403 5a18 6504 6505  e.e.d.<.d.Z.e.e.
-00000700: 6416 3c00 6403 5a19 6504 6505 6417 3c00  d.<.d.Z.e.e.d.<.
-00000710: 6403 5a1a 651b 6505 6418 3c00 6403 5300  d.Z.e.e.d.<.d.S.
-00000720: 2919 da0b 4d61 7456 616c 7565 4474 6f75  )...MatValueDtou
-00000730: cf01 0000 d0a2 d0b8 d0bf 204d 6174 5661  .......... MatVa
-00000740: 6c75 6520 d0bf d180 d0b5 d0b4 d181 d182  lue ............
-00000750: d0b0 d0b2 d0bb d18f d0b5 d182 20d1 81d0  ............ ...
-00000760: bed0 b1d0 bed0 b920 d0bd d0b0 d0b1 d0be  ....... ........
-00000770: d180 20d0 b4d0 b0d0 bdd0 bdd1 8bd1 8520  .. ............ 
-00000780: d0bc d0b0 d182 d0b5 d180 d0b8 d0b0 d0bb  ................
-00000790: d18c d0bd d0be d0b9 20d1 86d0 b5d0 bdd0  ........ .......
-000007a0: bdd0 bed1 81d1 82d0 b82e 20d0 9ed0 b1d1  .......... .....
-000007b0: 8ad0 b5d0 bad1 8220 d182 d0b8 d0bf d0b0  ....... ........
-000007c0: 204d 6174 5661 6c75 650a d18f d0b2 d0bb   MatValue.......
-000007d0: d18f d0b5 d182 d181 d18f 20d0 bfd0 bed0  .......... .....
-000007e0: bbd0 b5d0 bc20 d0be d0b1 d18a d0b5 d0ba  ..... ..........
-000007f0: d182 d0b0 204d 6174 5661 6c75 6550 6173  .... MatValuePas
-00000800: 732c 20d0 b8d1 81d0 bfd0 bed0 bbd1 8cd0  s, .............
-00000810: b7d1 83d1 8ed1 89d0 b5d0 b3d0 bed1 81d1  ................
-00000820: 8f20 d0b2 20d0 bcd0 b5d1 82d0 bed0 b4d0  . .. ...........
-00000830: b0d1 8520 d181 d0be d0b7 d0b4 d0b0 d0bd  ... ............
-00000840: d0b8 d18f 20d0 b820 d180 d0b5 d0b4 d0b0  .... .. ........
-00000850: d0ba d182 d0b8 d180 d0be d0b2 d0b0 d0bd  ................
-00000860: d0b8 d18f 2c20 d0b0 0ad1 82d0 b0d0 bad0  ...., ..........
-00000870: b6d0 b520 d0bf d0be d0bb d183 d187 d0b5  ... ............
-00000880: d0bd d0b8 d18f 20d1 81d0 bfd0 b8d1 81d0  ...... .........
-00000890: bad0 bed0 b220 d0bc d0b0 d182 d0b5 d180  ..... ..........
-000008a0: d0b8 d0b0 d0bb d18c d0bd d18b d185 20d0  .............. .
-000008b0: bfd1 80d0 bed0 bfd1 83d1 81d0 bad0 bed0  ................
-000008c0: b220 d0b8 20d0 b7d0 b0d1 8fd0 b2d0 bed0  . .. ...........
-000008d0: ba20 4765 744d 5650 6173 7365 732c 0a47  . GetMVPasses,.G
-000008e0: 6574 4d56 5061 7373 6573 4279 5065 7273  etMVPassesByPers
-000008f0: 6f6e 5061 7373 20d0 b820 5075 744d 5650  onPass .. PutMVP
-00000900: 6173 73da 0474 7970 654e da07 7661 6c46  ass..typeN..valF
-00000910: 6c64 31da 0776 616c 466c 6432 da07 7661  ld1..valFld2..va
-00000920: 6c46 6c64 33da 0776 616c 466c 6434 da07  lFld3..valFld4..
-00000930: 7661 6c46 6c64 35da 0776 616c 466c 6436  valFld5..valFld6
-00000940: da07 7661 6c46 6c64 37da 0776 616c 466c  ..valFld7..valFl
-00000950: 6438 da07 7661 6c46 6c64 39da 0876 616c  d8..valFld9..val
-00000960: 466c 6431 30da 0876 616c 466c 6431 31da  Fld10..valFld11.
-00000970: 0876 616c 466c 6431 32da 0876 616c 466c  .valFld12..valFl
-00000980: 6431 33da 0876 616c 466c 6431 34da 0876  d13..valFld14..v
-00000990: 616c 466c 6431 35da 0876 616c 466c 6431  alFld15..valFld1
-000009a0: 36da 0876 616c 466c 6431 37da 0876 616c  6..valFld17..val
-000009b0: 466c 6431 38da 0876 616c 466c 6431 39da  Fld18..valFld19.
-000009c0: 0876 616c 466c 6432 30da 086f 7264 6572  .valFld20..order
-000009d0: 4e75 6d29 1c72 0600 0000 7207 0000 0072  Num).r....r....r
-000009e0: 0800 0000 7209 0000 0072 0c00 0000 720b  ....r....r....r.
-000009f0: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
-00000a00: 0000 721a 0000 0072 1b00 0000 721c 0000  ..r....r....r...
-00000a10: 0072 1d00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00000a20: 7220 0000 0072 2100 0000 7222 0000 0072  r ...r!...r"...r
-00000a30: 2300 0000 7224 0000 0072 2500 0000 7226  #...r$...r%...r&
-00000a40: 0000 0072 2700 0000 7228 0000 0072 2900  ...r'...r(...r).
-00000a50: 0000 722a 0000 0072 2b00 0000 720a 0000  ..r*...r+...r...
-00000a60: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-00000a70: 720e 0000 0072 1500 0000 1900 0000 7330  r....r........s0
-00000a80: 0000 000a 0004 0108 040c 010c 010c 010c  ................
-00000a90: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000aa0: 010c 010c 010c 010c 010c 010c 010c 010c  ................
-00000ab0: 0110 0172 1500 0000 6300 0000 0000 0000  ...r....c.......
-00000ac0: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00000ad0: 0073 8600 0000 6500 5a01 6400 5a02 5500  .s....e.Z.d.Z.U.
-00000ae0: 6401 5a03 6504 6505 6402 3c00 6403 5a06  d.Z.e.e.d.<.d.Z.
-00000af0: 6504 6505 6404 3c00 6403 5a07 6504 6505  e.e.d.<.d.Z.e.e.
-00000b00: 6405 3c00 6403 5a08 6504 6505 6406 3c00  d.<.d.Z.e.e.d.<.
-00000b10: 6403 5a09 650a 6505 6407 3c00 6403 5a0b  d.Z.e.e.d.<.d.Z.
-00000b20: 6504 6505 6408 3c00 6403 5a0c 6504 6505  e.e.d.<.d.Z.e.e.
-00000b30: 6409 3c00 6403 5a0d 6504 6505 640a 3c00  d.<.d.Z.e.e.d.<.
-00000b40: 6403 5a0e 6504 6505 640b 3c00 6403 5a0f  d.Z.e.e.d.<.d.Z.
-00000b50: 6504 6505 640c 3c00 6403 5300 290d da06  e.e.d.<.d.S.)...
-00000b60: 4361 7244 746f 75c6 0100 00d0 a2d0 b8d0  CarDtou.........
-00000b70: bf20 4361 7220 d0bf d180 d0b5 d0b4 d181  . Car ..........
-00000b80: d182 d0b0 d0b2 d0bb d18f d0b5 d182 20d1  .............. .
-00000b90: 81d0 bed0 b1d0 bed0 b920 d0bd d0b0 d0b1  ......... ......
-00000ba0: d0be d180 20d0 b4d0 b0d0 bdd0 bdd1 8bd1  .... ...........
-00000bb0: 8520 d182 d180 d0b0 d0bd d181 d0bf d0be  . ..............
-00000bc0: d180 d182 d0bd d0be d0b3 d0be 20d1 81d1  ............ ...
-00000bd0: 80d0 b5d0 b4d1 81d1 82d0 b2d0 b02e 20d0  .............. .
-00000be0: 9ed0 b1d1 8ad0 b5d0 bad1 8220 d182 d0b8  ........... ....
-00000bf0: d0bf d0b0 2043 6172 20d1 8fd0 b2d0 bbd1  .... Car .......
-00000c00: 8fd0 b5d1 82d1 81d1 8f20 d0bf d0be d0bb  ......... ......
-00000c10: d0b5 d0bc 0ad0 bed0 b1d1 8ad0 b5d0 bad1  ................
-00000c20: 82d0 b020 4361 7250 6173 732c 20d0 b8d1  ... CarPass, ...
-00000c30: 81d0 bfd0 bed0 bbd1 8cd0 b7d1 83d1 8ed1  ................
-00000c40: 89d0 b5d0 b3d0 bed1 81d1 8f20 d0b2 20d0  ........... .. .
-00000c50: bcd0 b5d1 82d0 bed0 b4d0 b0d1 8520 d181  ............. ..
-00000c60: d0be d0b7 d0b4 d0b0 d0bd d0b8 d18f 20d0  .............. .
-00000c70: b820 d180 d0b5 d0b4 d0b0 d0ba d182 d0b8  . ..............
-00000c80: d180 d0be d0b2 d0b0 d0bd d0b8 d18f 2c20  .............., 
-00000c90: d0b0 20d1 82d0 b0d0 ba20 d0b6 d0b5 20d0  .. ...... .... .
-00000ca0: bfd0 bed0 bbd1 83d1 87d0 b5d0 bdd0 b8d1  ................
-00000cb0: 8f0a d181 d0bf d0b8 d181 d0ba d0be d0b2  ................
-00000cc0: 20d1 82d1 80d0 b0d0 bdd1 81d0 bfd0 bed1   ...............
-00000cd0: 80d1 82d0 bdd1 8bd1 8520 d0bf d180 d0be  ......... ......
-00000ce0: d0bf d183 d181 d0ba d0be d0b2 20d0 b820  ............ .. 
-00000cf0: d0b7 d0b0 d18f d0b2 d0be d0ba 2047 6574  ............ Get
-00000d00: 4361 7250 6173 7365 732c 2047 6574 4361  CarPasses, GetCa
-00000d10: 7250 6173 7365 7342 7950 6572 736f 6e50  rPassesByPersonP
-00000d20: 6173 7320 d0b8 2050 7574 4361 7250 6173  ass .. PutCarPas
-00000d30: 73da 0572 6567 4e6f 4eda 0863 6172 4d6f  s..regNoN..carMo
-00000d40: 6465 6cda 0e63 6172 4465 7363 7269 7074  del..carDescript
-00000d50: 696f 6eda 0863 6172 5068 6f74 6fda 0763  ion..carPhoto..c
-00000d60: 6172 5965 6172 da0b 6361 7243 6f6c 6f72  arYear..carColor
-00000d70: 5374 72da 0963 6172 5765 6967 6874 da09  Str..carWeight..
-00000d80: 6361 7256 6f6c 756d 65da 0b63 6172 4f77  carVolume..carOw
-00000d90: 6e65 7253 7472 da0a 6361 7254 7970 6553  nerStr..carTypeS
-00000da0: 7472 2910 7206 0000 0072 0700 0000 7208  tr).r....r....r.
-00000db0: 0000 0072 0900 0000 720c 0000 0072 0b00  ...r....r....r..
-00000dc0: 0000 722e 0000 0072 2f00 0000 7230 0000  ..r....r/...r0..
-00000dd0: 0072 3100 0000 720a 0000 0072 3200 0000  .r1...r....r2...
-00000de0: 7233 0000 0072 3400 0000 7235 0000 0072  r3...r4...r5...r
-00000df0: 3600 0000 720d 0000 0072 0d00 0000 720d  6...r....r....r.
-00000e00: 0000 0072 0e00 0000 722c 0000 0036 0000  ...r....r,...6..
-00000e10: 0073 1800 0000 0a00 0401 0803 0c01 0c01  .s..............
-00000e20: 0c01 0c01 0c01 0c01 0c01 0c01 1001 722c  ..............r,
-00000e30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000e40: 0000 0000 0300 0000 4000 0000 733e 0000  ........@...s>..
-00000e50: 0065 005a 0164 005a 0255 0064 015a 0365  .e.Z.d.Z.U.d.Z.e
-00000e60: 0465 0564 023c 0064 035a 0665 0465 0564  .e.d.<.d.Z.e.e.d
-00000e70: 043c 0064 035a 0765 0465 0564 053c 0064  .<.d.Z.e.e.d.<.d
-00000e80: 035a 0865 0465 0564 063c 0064 0353 0029  .Z.e.e.d.<.d.S.)
-00000e90: 07da 0e50 6572 736f 6e42 7269 6566 4474  ...PersonBriefDt
-00000ea0: 6f75 5900 0000 d0bf d180 d0b5 d0b4 d181  ouY.............
-00000eb0: d182 d0b0 d0b2 d0bb d18f d0b5 d182 20d1  .............. .
-00000ec0: 81d0 bed0 b1d0 bed0 b920 d0ba d180 d0b0  ......... ......
-00000ed0: d182 d0ba d0b8 d0b9 20d0 bdd0 b0d0 b1d0  ........ .......
-00000ee0: bed1 8020 d0b4 d0b0 d0bd d0bd d18b d185  ... ............
-00000ef0: 20d0 bfd0 b5d1 80d1 81d0 bed0 bdd1 8bda   ...............
-00000f00: 046e 616d 654e da09 6669 7273 744e 616d  .nameN..firstNam
-00000f10: 65da 0a73 6563 6f6e 644e 616d 65da 0962  e..secondName..b
-00000f20: 6972 7468 4461 7465 2909 7206 0000 0072  irthDate).r....r
-00000f30: 0700 0000 7208 0000 0072 0900 0000 720c  ....r....r....r.
-00000f40: 0000 0072 0b00 0000 7239 0000 0072 3a00  ...r....r9...r:.
-00000f50: 0000 723b 0000 0072 0d00 0000 720d 0000  ..r;...r....r...
-00000f60: 0072 0d00 0000 720e 0000 0072 3700 0000  .r....r....r7...
-00000f70: 4500 0000 730c 0000 000a 0004 0108 010c  E...s...........
-00000f80: 010c 0110 0172 3700 0000 6300 0000 0000  .....r7...c.....
-00000f90: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00000fa0: 0000 0073 3200 0000 6500 5a01 6400 5a02  ...s2...e.Z.d.Z.
-00000fb0: 5500 6401 5a03 6504 6505 6402 3c00 6506  U.d.Z.e.e.d.<.e.
-00000fc0: 6505 6403 3c00 6507 6505 6404 3c00 6507  e.d.<.e.e.d.<.e.
-00000fd0: 6505 6405 3c00 6406 5300 2907 da0c 5061  e.d.<.d.S.)...Pa
-00000fe0: 7373 4272 6965 6644 746f 75a0 0000 00d0  ssBriefDtou.....
-00000ff0: a2d0 b8d0 bf20 5061 7373 20d0 bfd1 80d0  ..... Pass .....
-00001000: b5d0 b4d1 81d1 82d0 b0d0 b2d0 bbd1 8fd0  ................
-00001010: b5d1 8220 d0ba d180 d0b0 d182 d0ba d0b8  ... ............
-00001020: d0b9 20d0 bdd0 b0d0 b1d0 bed1 8020 d0b4  .. .......... ..
-00001030: d0b0 d0bd d0bd d18b d185 20d0 bfd0 b5d1  .......... .....
-00001040: 80d1 81d0 bed0 bdd0 b0d0 bbd1 8cd0 bdd0  ................
-00001050: bed0 b3d0 be20 d0bf d180 d0be d0bf d183  ..... ..........
-00001060: d181 d0ba d0b0 20d0 b8d0 bbd0 b820 d0b7  ...... ...... ..
-00001070: d0b0 d18f d0b2 d0ba d0b8 20d0 bdd0 b020  .......... .... 
-00001080: d0bf d180 d0be d0bf d183 d181 d0ba 2eda  ................
-00001090: 0843 6172 6443 6f64 65da 0a50 6572 736f  .CardCode..Perso
-000010a0: 6e44 6174 61da 0850 6173 7354 7970 65da  nData..PassType.
-000010b0: 0a43 6172 6453 7461 7475 734e 2908 7206  .CardStatusN).r.
-000010c0: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-000010d0: 0000 720c 0000 0072 0b00 0000 7237 0000  ..r....r....r7..
-000010e0: 0072 0a00 0000 720d 0000 0072 0d00 0000  .r....r....r....
-000010f0: 720d 0000 0072 0e00 0000 723c 0000 004c  r....r....r<...L
-00001100: 0000 0073 0c00 0000 0a00 0401 0801 0801  ...s............
-00001110: 0801 0c01 723c 0000 004e 2908 da08 7079  ....r<...N)...py
-00001120: 6461 6e74 6963 7202 0000 0072 0300 0000  danticr....r....
-00001130: 720f 0000 0072 1500 0000 722c 0000 0072  r....r....r,...r
-00001140: 3700 0000 723c 0000 0072 0d00 0000 720d  7...r<...r....r.
-00001150: 0000 0072 0d00 0000 720e 0000 00da 083c  ...r....r......<
-00001160: 6d6f 6475 6c65 3e01 0000 0073 0e00 0000  module>....s....
-00001170: 0c01 1002 1009 100c 101d 100f 1407       ..............
+00000230: 0000 0072 0d00 0000 fa50 2f68 6f6d 652f  ...r.....P/home/
+00000240: 6b6f 726f 676f 642f 5079 6368 6172 6d50  korogod/PycharmP
+00000250: 726f 6a65 6374 732f 4261 7374 696f 6e5f  rojects/Bastion_
+00000260: 696e 7465 6772 6174 696f 6e2f 7372 632f  integration/src/
+00000270: 6261 7374 696f 6e5f 6170 692f 6474 6f2f  bastion_api/dto/
+00000280: 7375 7070 6f72 742e 7079 7203 0000 0004  support.pyr.....
+00000290: 0000 0073 0800 0000 0a00 0401 0802 0c01  ...s............
+000002a0: 7203 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000002b0: 0000 0000 0000 0300 0000 4000 0000 733a  ..........@...s:
+000002c0: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+000002d0: 0365 0465 0564 023c 0065 0465 0564 033c  .e.e.d.<.e.e.d.<
+000002e0: 0065 0665 0564 043c 0065 0665 0564 053c  .e.e.d.<.e.e.d.<
+000002f0: 0065 0665 0564 063c 0064 0753 0029 08da  .e.e.d.<.d.S.)..
+00000300: 0f54 696d 6549 6e74 6572 7661 6c44 746f  .TimeIntervalDto
+00000310: 7547 0200 00d0 9ed0 b1d1 8ad0 b5d0 bad1  uG..............
+00000320: 8220 d182 d0b8 d0bf d0b0 2054 696d 6549  . ........ TimeI
+00000330: 6e74 6572 7661 6c20 d0bf d180 d0b5 d0b4  nterval ........
+00000340: d181 d182 d0b0 d0b2 d0bb d18f d0b5 d182  ................
+00000350: 20d1 81d0 bed0 b1d0 bed0 b920 d0b2 d180   .......... ....
+00000360: d0b5 d0bc d0b5 d0bd d0bd d0be d0b9 20d0  .............. .
+00000370: bfd1 80d0 bed0 bcd0 b5d0 b6d1 83d1 82d0  ................
+00000380: bed0 ba2c 20d1 84d0 b8d0 b3d1 83d1 80d0  ..., ...........
+00000390: b8d1 80d1 83d1 8ed1 89d0 b8d0 b920 d0b2  ............. ..
+000003a0: 20d1 83d1 80d0 bed0 b2d0 bdd0 b50a d0b4   ...............
+000003b0: d0be d181 d182 d183 d0bf d0b0 2c20 d0bf  ............, ..
+000003c0: d180 d0b8 d0b2 d18f d0b7 d0b0 d0bd d0bd  ................
+000003d0: d0be d0bc d183 20d0 ba20 d0bf d180 d0be  ...... .. ......
+000003e0: d0bf d183 d181 d0ba d183 20d0 b220 d0a1  .......... .. ..
+000003f0: d09a d0a3 d094 20d0 90d0 9fd0 9a20 c2ab  ...... ...... ..
+00000400: d091 d0b0 d181 d182 d0b8 d0be d0bd 2d32  ..............-2
+00000410: c2bb 2e20 d09e d0b1 d18a d0b5 d0ba d182  ... ............
+00000420: 20d1 82d0 b8d0 bfd0 b020 5469 6d65 496e   ........ TimeIn
+00000430: 7465 7276 616c 20d1 8fd0 b2d0 bbd1 8fd0  terval .........
+00000440: b5d1 82d1 81d1 8f0a d0bf d0be d0bb d0b5  ................
+00000450: d0bc 20d0 b220 d182 d0b8 d0bf d0b5 20d0  .. .. ........ .
+00000460: b4d0 b0d0 bdd0 bdd1 8bd1 8520 5061 7373  ........... Pass
+00000470: 2c20 d0b8 d181 d0bf d0be d0bb d18c d0b7  , ..............
+00000480: d183 d18e d189 d0b5 d0bc d181 d18f 20d0  .............. .
+00000490: b220 d0bc d0b5 d182 d0be d0b4 d0b5 20d1  . ............ .
+000004a0: 81d0 bed0 b7d0 b4d0 b0d0 bdd0 b8d1 8f2f  .............../
+000004b0: d180 d0b5 d0b4 d0b0 d0ba d182 d0b8 d180  ................
+000004c0: d0be d0b2 d0b0 d0bd d0b8 d18f 20d0 bfd1  ............ ...
+000004d0: 80d0 bed0 bfd1 83d1 81d0 bad0 b02f d0b7  ............./..
+000004e0: d0b0 d18f d0b2 d0ba d0b8 0ad0 bdd0 b020  ............... 
+000004f0: d0bf d180 d0be d0bf d183 d181 d0ba 2050  .............. P
+00000500: 7574 5061 7373 20d0 b820 d0b2 20d0 bcd0  utPass .. .. ...
+00000510: b5d1 82d0 bed0 b4d0 b520 d0bf d0be d0bb  ......... ......
+00000520: d183 d187 d0b5 d0bd d0b8 d18f 20d0 bad0  ............ ...
+00000530: bed0 bbd0 bbd0 b5d0 bad1 86d0 b8d0 b820  ............... 
+00000540: d0bf d180 d0be d0bf d183 d181 d0ba d0be  ................
+00000550: d0b2 2047 6574 5061 7373 6573 da09 7469  .. GetPasses..ti
+00000560: 6d65 5374 6172 74da 0774 696d 6545 6e64  meStart..timeEnd
+00000570: da0a 696e 5361 7475 7264 6179 da08 696e  ..inSaturday..in
+00000580: 5375 6e64 6179 da0a 696e 486f 6c69 6461  Sunday..inHolida
+00000590: 7973 4e29 0772 0600 0000 7207 0000 0072  ysN).r....r....r
+000005a0: 0800 0000 7209 0000 0072 0c00 0000 720b  ....r....r....r.
+000005b0: 0000 0072 0a00 0000 720d 0000 0072 0d00  ...r....r....r..
+000005c0: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+000005d0: 000b 0000 0073 0e00 0000 0a00 0401 0804  .....s..........
+000005e0: 0801 0801 0801 0c01 720f 0000 0063 0000  ........r....c..
+000005f0: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000600: 0000 4000 0000 7316 0100 0065 005a 0164  ..@...s....e.Z.d
+00000610: 005a 0255 0064 015a 0365 0465 0564 023c  .Z.U.d.Z.e.e.d.<
+00000620: 0064 035a 0665 0465 0564 043c 0064 035a  .d.Z.e.e.d.<.d.Z
+00000630: 0765 0465 0564 053c 0064 035a 0865 0465  .e.e.d.<.d.Z.e.e
+00000640: 0564 063c 0064 035a 0965 0465 0564 073c  .d.<.d.Z.e.e.d.<
+00000650: 0064 035a 0a65 0465 0564 083c 0064 035a  .d.Z.e.e.d.<.d.Z
+00000660: 0b65 0465 0564 093c 0064 035a 0c65 0465  .e.e.d.<.d.Z.e.e
+00000670: 0564 0a3c 0064 035a 0d65 0465 0564 0b3c  .d.<.d.Z.e.e.d.<
+00000680: 0064 035a 0e65 0465 0564 0c3c 0064 035a  .d.Z.e.e.d.<.d.Z
+00000690: 0f65 0465 0564 0d3c 0064 035a 1065 0465  .e.e.d.<.d.Z.e.e
+000006a0: 0564 0e3c 0064 035a 1165 0465 0564 0f3c  .d.<.d.Z.e.e.d.<
+000006b0: 0064 035a 1265 0465 0564 103c 0064 035a  .d.Z.e.e.d.<.d.Z
+000006c0: 1365 0465 0564 113c 0064 035a 1465 0465  .e.e.d.<.d.Z.e.e
+000006d0: 0564 123c 0064 035a 1565 0465 0564 133c  .d.<.d.Z.e.e.d.<
+000006e0: 0064 035a 1665 0465 0564 143c 0064 035a  .d.Z.e.e.d.<.d.Z
+000006f0: 1765 0465 0564 153c 0064 035a 1865 0465  .e.e.d.<.d.Z.e.e
+00000700: 0564 163c 0064 035a 1965 0465 0564 173c  .d.<.d.Z.e.e.d.<
+00000710: 0064 035a 1a65 1b65 0564 183c 0064 0353  .d.Z.e.e.d.<.d.S
+00000720: 0029 19da 0b4d 6174 5661 6c75 6544 746f  .)...MatValueDto
+00000730: 75cf 0100 00d0 a2d0 b8d0 bf20 4d61 7456  u.......... MatV
+00000740: 616c 7565 20d0 bfd1 80d0 b5d0 b4d1 81d1  alue ...........
+00000750: 82d0 b0d0 b2d0 bbd1 8fd0 b5d1 8220 d181  ............. ..
+00000760: d0be d0b1 d0be d0b9 20d0 bdd0 b0d0 b1d0  ........ .......
+00000770: bed1 8020 d0b4 d0b0 d0bd d0bd d18b d185  ... ............
+00000780: 20d0 bcd0 b0d1 82d0 b5d1 80d0 b8d0 b0d0   ...............
+00000790: bbd1 8cd0 bdd0 bed0 b920 d186 d0b5 d0bd  ......... ......
+000007a0: d0bd d0be d181 d182 d0b8 2e20 d09e d0b1  ........... ....
+000007b0: d18a d0b5 d0ba d182 20d1 82d0 b8d0 bfd0  ........ .......
+000007c0: b020 4d61 7456 616c 7565 0ad1 8fd0 b2d0  . MatValue......
+000007d0: bbd1 8fd0 b5d1 82d1 81d1 8f20 d0bf d0be  ........... ....
+000007e0: d0bb d0b5 d0bc 20d0 bed0 b1d1 8ad0 b5d0  ...... .........
+000007f0: bad1 82d0 b020 4d61 7456 616c 7565 5061  ..... MatValuePa
+00000800: 7373 2c20 d0b8 d181 d0bf d0be d0bb d18c  ss, ............
+00000810: d0b7 d183 d18e d189 d0b5 d0b3 d0be d181  ................
+00000820: d18f 20d0 b220 d0bc d0b5 d182 d0be d0b4  .. .. ..........
+00000830: d0b0 d185 20d1 81d0 bed0 b7d0 b4d0 b0d0  .... ...........
+00000840: bdd0 b8d1 8f20 d0b8 20d1 80d0 b5d0 b4d0  ..... .. .......
+00000850: b0d0 bad1 82d0 b8d1 80d0 bed0 b2d0 b0d0  ................
+00000860: bdd0 b8d1 8f2c 20d0 b00a d182 d0b0 d0ba  ....., .........
+00000870: d0b6 d0b5 20d0 bfd0 bed0 bbd1 83d1 87d0  .... ...........
+00000880: b5d0 bdd0 b8d1 8f20 d181 d0bf d0b8 d181  ....... ........
+00000890: d0ba d0be d0b2 20d0 bcd0 b0d1 82d0 b5d1  ...... .........
+000008a0: 80d0 b8d0 b0d0 bbd1 8cd0 bdd1 8bd1 8520  ............... 
+000008b0: d0bf d180 d0be d0bf d183 d181 d0ba d0be  ................
+000008c0: d0b2 20d0 b820 d0b7 d0b0 d18f d0b2 d0be  .. .. ..........
+000008d0: d0ba 2047 6574 4d56 5061 7373 6573 2c0a  .. GetMVPasses,.
+000008e0: 4765 744d 5650 6173 7365 7342 7950 6572  GetMVPassesByPer
+000008f0: 736f 6e50 6173 7320 d0b8 2050 7574 4d56  sonPass .. PutMV
+00000900: 5061 7373 da04 7479 7065 4eda 0776 616c  Pass..typeN..val
+00000910: 466c 6431 da07 7661 6c46 6c64 32da 0776  Fld1..valFld2..v
+00000920: 616c 466c 6433 da07 7661 6c46 6c64 34da  alFld3..valFld4.
+00000930: 0776 616c 466c 6435 da07 7661 6c46 6c64  .valFld5..valFld
+00000940: 36da 0776 616c 466c 6437 da07 7661 6c46  6..valFld7..valF
+00000950: 6c64 38da 0776 616c 466c 6439 da08 7661  ld8..valFld9..va
+00000960: 6c46 6c64 3130 da08 7661 6c46 6c64 3131  lFld10..valFld11
+00000970: da08 7661 6c46 6c64 3132 da08 7661 6c46  ..valFld12..valF
+00000980: 6c64 3133 da08 7661 6c46 6c64 3134 da08  ld13..valFld14..
+00000990: 7661 6c46 6c64 3135 da08 7661 6c46 6c64  valFld15..valFld
+000009a0: 3136 da08 7661 6c46 6c64 3137 da08 7661  16..valFld17..va
+000009b0: 6c46 6c64 3138 da08 7661 6c46 6c64 3139  lFld18..valFld19
+000009c0: da08 7661 6c46 6c64 3230 da08 6f72 6465  ..valFld20..orde
+000009d0: 724e 756d 291c 7206 0000 0072 0700 0000  rNum).r....r....
+000009e0: 7208 0000 0072 0900 0000 720c 0000 0072  r....r....r....r
+000009f0: 0b00 0000 7217 0000 0072 1800 0000 7219  ....r....r....r.
+00000a00: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00000a10: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00000a20: 0072 2000 0000 7221 0000 0072 2200 0000  .r ...r!...r"...
+00000a30: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
+00000a40: 2600 0000 7227 0000 0072 2800 0000 7229  &...r'...r(...r)
+00000a50: 0000 0072 2a00 0000 722b 0000 0072 0a00  ...r*...r+...r..
+00000a60: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000a70: 0072 0e00 0000 7215 0000 0017 0000 0073  .r....r........s
+00000a80: 3000 0000 0a00 0401 0804 0c01 0c01 0c01  0...............
+00000a90: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000aa0: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
+00000ab0: 0c01 1001 7215 0000 0063 0000 0000 0000  ....r....c......
+00000ac0: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
+00000ad0: 0000 7386 0000 0065 005a 0164 005a 0255  ..s....e.Z.d.Z.U
+00000ae0: 0064 015a 0365 0465 0564 023c 0064 035a  .d.Z.e.e.d.<.d.Z
+00000af0: 0665 0465 0564 043c 0064 035a 0765 0465  .e.e.d.<.d.Z.e.e
+00000b00: 0564 053c 0064 035a 0865 0465 0564 063c  .d.<.d.Z.e.e.d.<
+00000b10: 0064 035a 0965 0a65 0564 073c 0064 035a  .d.Z.e.e.d.<.d.Z
+00000b20: 0b65 0465 0564 083c 0064 035a 0c65 0465  .e.e.d.<.d.Z.e.e
+00000b30: 0564 093c 0064 035a 0d65 0465 0564 0a3c  .d.<.d.Z.e.e.d.<
+00000b40: 0064 035a 0e65 0465 0564 0b3c 0064 035a  .d.Z.e.e.d.<.d.Z
+00000b50: 0f65 0465 0564 0c3c 0064 0353 0029 0dda  .e.e.d.<.d.S.)..
+00000b60: 0643 6172 4474 6f75 c601 0000 d0a2 d0b8  .CarDtou........
+00000b70: d0bf 2043 6172 20d0 bfd1 80d0 b5d0 b4d1  .. Car .........
+00000b80: 81d1 82d0 b0d0 b2d0 bbd1 8fd0 b5d1 8220  ............... 
+00000b90: d181 d0be d0b1 d0be d0b9 20d0 bdd0 b0d0  .......... .....
+00000ba0: b1d0 bed1 8020 d0b4 d0b0 d0bd d0bd d18b  ..... ..........
+00000bb0: d185 20d1 82d1 80d0 b0d0 bdd1 81d0 bfd0  .. .............
+00000bc0: bed1 80d1 82d0 bdd0 bed0 b3d0 be20 d181  ............. ..
+00000bd0: d180 d0b5 d0b4 d181 d182 d0b2 d0b0 2e20  ............... 
+00000be0: d09e d0b1 d18a d0b5 d0ba d182 20d1 82d0  ............ ...
+00000bf0: b8d0 bfd0 b020 4361 7220 d18f d0b2 d0bb  ..... Car ......
+00000c00: d18f d0b5 d182 d181 d18f 20d0 bfd0 bed0  .......... .....
+00000c10: bbd0 b5d0 bc0a d0be d0b1 d18a d0b5 d0ba  ................
+00000c20: d182 d0b0 2043 6172 5061 7373 2c20 d0b8  .... CarPass, ..
+00000c30: d181 d0bf d0be d0bb d18c d0b7 d183 d18e  ................
+00000c40: d189 d0b5 d0b3 d0be d181 d18f 20d0 b220  ............ .. 
+00000c50: d0bc d0b5 d182 d0be d0b4 d0b0 d185 20d1  .............. .
+00000c60: 81d0 bed0 b7d0 b4d0 b0d0 bdd0 b8d1 8f20  ............... 
+00000c70: d0b8 20d1 80d0 b5d0 b4d0 b0d0 bad1 82d0  .. .............
+00000c80: b8d1 80d0 bed0 b2d0 b0d0 bdd0 b8d1 8f2c  ...............,
+00000c90: 20d0 b020 d182 d0b0 d0ba 20d0 b6d0 b520   .. ...... .... 
+00000ca0: d0bf d0be d0bb d183 d187 d0b5 d0bd d0b8  ................
+00000cb0: d18f 0ad1 81d0 bfd0 b8d1 81d0 bad0 bed0  ................
+00000cc0: b220 d182 d180 d0b0 d0bd d181 d0bf d0be  . ..............
+00000cd0: d180 d182 d0bd d18b d185 20d0 bfd1 80d0  .......... .....
+00000ce0: bed0 bfd1 83d1 81d0 bad0 bed0 b220 d0b8  ............. ..
+00000cf0: 20d0 b7d0 b0d1 8fd0 b2d0 bed0 ba20 4765   ............ Ge
+00000d00: 7443 6172 5061 7373 6573 2c20 4765 7443  tCarPasses, GetC
+00000d10: 6172 5061 7373 6573 4279 5065 7273 6f6e  arPassesByPerson
+00000d20: 5061 7373 20d0 b820 5075 7443 6172 5061  Pass .. PutCarPa
+00000d30: 7373 da05 7265 674e 6f4e da08 6361 724d  ss..regNoN..carM
+00000d40: 6f64 656c da0e 6361 7244 6573 6372 6970  odel..carDescrip
+00000d50: 7469 6f6e da08 6361 7250 686f 746f da07  tion..carPhoto..
+00000d60: 6361 7259 6561 72da 0b63 6172 436f 6c6f  carYear..carColo
+00000d70: 7253 7472 da09 6361 7257 6569 6768 74da  rStr..carWeight.
+00000d80: 0963 6172 566f 6c75 6d65 da0b 6361 724f  .carVolume..carO
+00000d90: 776e 6572 5374 72da 0a63 6172 5479 7065  wnerStr..carType
+00000da0: 5374 7229 1072 0600 0000 7207 0000 0072  Str).r....r....r
+00000db0: 0800 0000 7209 0000 0072 0c00 0000 720b  ....r....r....r.
+00000dc0: 0000 0072 2e00 0000 722f 0000 0072 3000  ...r....r/...r0.
+00000dd0: 0000 7231 0000 0072 0a00 0000 7232 0000  ..r1...r....r2..
+00000de0: 0072 3300 0000 7234 0000 0072 3500 0000  .r3...r4...r5...
+00000df0: 7236 0000 0072 0d00 0000 720d 0000 0072  r6...r....r....r
+00000e00: 0d00 0000 720e 0000 0072 2c00 0000 3400  ....r....r,...4.
+00000e10: 0000 7318 0000 000a 0004 0108 030c 010c  ..s.............
+00000e20: 010c 010c 010c 010c 010c 010c 0110 0172  ...............r
+00000e30: 2c00 0000 6300 0000 0000 0000 0000 0000  ,...c...........
+00000e40: 0000 0000 0003 0000 0040 0000 0073 3e00  .........@...s>.
+00000e50: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
+00000e60: 6504 6505 6402 3c00 6403 5a06 6504 6505  e.e.d.<.d.Z.e.e.
+00000e70: 6404 3c00 6403 5a07 6504 6505 6405 3c00  d.<.d.Z.e.e.d.<.
+00000e80: 6403 5a08 6504 6505 6406 3c00 6403 5300  d.Z.e.e.d.<.d.S.
+00000e90: 2907 da0e 5065 7273 6f6e 4272 6965 6644  )...PersonBriefD
+00000ea0: 746f 7559 0000 00d0 bfd1 80d0 b5d0 b4d1  touY............
+00000eb0: 81d1 82d0 b0d0 b2d0 bbd1 8fd0 b5d1 8220  ............... 
+00000ec0: d181 d0be d0b1 d0be d0b9 20d0 bad1 80d0  .......... .....
+00000ed0: b0d1 82d0 bad0 b8d0 b920 d0bd d0b0 d0b1  ......... ......
+00000ee0: d0be d180 20d0 b4d0 b0d0 bdd0 bdd1 8bd1  .... ...........
+00000ef0: 8520 d0bf d0b5 d180 d181 d0be d0bd d18b  . ..............
+00000f00: da04 6e61 6d65 4eda 0966 6972 7374 4e61  ..nameN..firstNa
+00000f10: 6d65 da0a 7365 636f 6e64 4e61 6d65 da09  me..secondName..
+00000f20: 6269 7274 6844 6174 6529 0972 0600 0000  birthDate).r....
+00000f30: 7207 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
+00000f40: 0c00 0000 720b 0000 0072 3900 0000 723a  ....r....r9...r:
+00000f50: 0000 0072 3b00 0000 720d 0000 0072 0d00  ...r;...r....r..
+00000f60: 0000 720d 0000 0072 0e00 0000 7237 0000  ..r....r....r7..
+00000f70: 0044 0000 0073 0c00 0000 0a00 0401 0801  .D...s..........
+00000f80: 0c01 0c01 1001 7237 0000 0063 0000 0000  ......r7...c....
+00000f90: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00000fa0: 4000 0000 7332 0000 0065 005a 0164 005a  @...s2...e.Z.d.Z
+00000fb0: 0255 0064 015a 0365 0465 0564 023c 0065  .U.d.Z.e.e.d.<.e
+00000fc0: 0665 0564 033c 0065 0765 0564 043c 0065  .e.d.<.e.e.d.<.e
+00000fd0: 0765 0564 053c 0064 0653 0029 07da 0c50  .e.d.<.d.S.)...P
+00000fe0: 6173 7342 7269 6566 4474 6f75 a000 0000  assBriefDtou....
+00000ff0: d0a2 d0b8 d0bf 2050 6173 7320 d0bf d180  ...... Pass ....
+00001000: d0b5 d0b4 d181 d182 d0b0 d0b2 d0bb d18f  ................
+00001010: d0b5 d182 20d0 bad1 80d0 b0d1 82d0 bad0  .... ...........
+00001020: b8d0 b920 d0bd d0b0 d0b1 d0be d180 20d0  ... .......... .
+00001030: b4d0 b0d0 bdd0 bdd1 8bd1 8520 d0bf d0b5  ........... ....
+00001040: d180 d181 d0be d0bd d0b0 d0bb d18c d0bd  ................
+00001050: d0be d0b3 d0be 20d0 bfd1 80d0 bed0 bfd1  ...... .........
+00001060: 83d1 81d0 bad0 b020 d0b8 d0bb d0b8 20d0  ....... ...... .
+00001070: b7d0 b0d1 8fd0 b2d0 bad0 b820 d0bd d0b0  ........... ....
+00001080: 20d0 bfd1 80d0 bed0 bfd1 83d1 81d0 ba2e   ...............
+00001090: da08 4361 7264 436f 6465 da0a 5065 7273  ..CardCode..Pers
+000010a0: 6f6e 4461 7461 da08 5061 7373 5479 7065  onData..PassType
+000010b0: da0a 4361 7264 5374 6174 7573 4e29 0872  ..CardStatusN).r
+000010c0: 0600 0000 7207 0000 0072 0800 0000 7209  ....r....r....r.
+000010d0: 0000 0072 0c00 0000 720b 0000 0072 3700  ...r....r....r7.
+000010e0: 0000 720a 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+000010f0: 0072 0d00 0000 720e 0000 0072 3c00 0000  .r....r....r<...
+00001100: 4c00 0000 730c 0000 000a 0004 0108 0108  L...s...........
+00001110: 0108 010c 0172 3c00 0000 4e29 08da 0870  .....r<...N)...p
+00001120: 7964 616e 7469 6372 0200 0000 7203 0000  ydanticr....r...
+00001130: 0072 0f00 0000 7215 0000 0072 2c00 0000  .r....r....r,...
+00001140: 7237 0000 0072 3c00 0000 720d 0000 0072  r7...r<...r....r
+00001150: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
+00001160: 3c6d 6f64 756c 653e 0100 0000 730e 0000  <module>....s...
+00001170: 000c 0010 0310 0710 0c10 1d10 1014 08    ...............
```

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/device_dto.py` & `bastion_api-0.3.0/src/bastion_api/dto/device_dto.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 получения набора устройств GetDevices"""
     sdn: int  # Идентификатор устройства
     parentSdn: int | None  # Идентификатор родительского устройства
     driverId: int  # Идентификатор типа драйвера, которому принадлежит устройство
     name: str  # Наименование устройства
     deviceType: int  # Код типа устройства
     deviceTypeName: str  # Текстовое имя типа устройства
-    childs: List[DeviceDto]  # Коллекция дочерних устройств
+    childs: List[DeviceDto] | None  # Коллекция дочерних устройств
```

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/old_dto.py` & `bastion_api-0.3.0/src/bastion_api/dto/old_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/organization_dto.py` & `bastion_api-0.3.0/src/bastion_api/dto/organization_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/pass_dto.py` & `bastion_api-0.3.0/src/bastion_api/dto/pass_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 from typing import List
 
 from pydantic import BaseModel
 
 from bastion_api.dto.person_dto import PersonDto
 from bastion_api.dto.points_dto import EntryPointDto, AccessLevelDto
-from bastion_api.dto.support import TimeIntervalDto, PersonBriefDto, MatValueDto, CarDto, PassBriefDto
+from bastion_api.dto.support import TimeIntervalDto, PersonBriefDto, MatValueDto, PassBriefDto, CarDto
 
 
 class PassDto:
     class NewPassPerson(BaseModel):
         """create_or_update_pass"""
         personData: PersonDto  # Набор персональных данных пропуска
         entryPoints: List[EntryPointDto] = ""  # Массив точек прохода
```

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/person_dto.py` & `bastion_api-0.3.0/src/bastion_api/dto/person_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/points_dto.py` & `bastion_api-0.3.0/src/bastion_api/dto/points_dto.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,10 +27,10 @@
     name: str  # Имя области контроля
 
 
 class AccessPointDto(BaseModel):
     """AccessPoint – объект, представляющий точку доступа (дверь, ворота, турникет) в СКУД АПК
     «Бастион-2». Используется в качестве выходного параметра в методе GetAccessPoints,
     возвращающем коллекцию точек доступа."""
-    sServID: str  # Идентификатор сервера – владельца точки прохода
-    sSubDeviceNo: int  # Идентификатор устройства на сервере
-    sSubDeviceName: str  # Имя точки прохода
+    servID: str  # Идентификатор сервера – владельца точки прохода
+    subDeviceNo: int  # Идентификатор устройства на сервере
+    subDeviceName: str  # Имя точки прохода
```

### Comparing `bastion_api-0.2.5/src/bastion_api/dto/support.py` & `bastion_api-0.3.0/src/bastion_api/dto/support.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.5/src/bastion_api/handlers.py` & `bastion_api-0.3.0/src/bastion_api/error_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+from enum import Enum
 from typing import Dict
 
 
-
-
 class BastionIntegrationError(Exception):
     error_type: str = "C"
     default_class: int = 999
     default_subclass: int = 999
     context: Dict[str, str | int] = None
 
     def __init__(self, ex=None, message=None, context=None):
@@ -27,12 +26,14 @@
             "code": f"{self.error_type}-{self.default_class}-{self.default_subclass}",
             "class": self.default_class,
             "subclass": self.default_subclass,
             "comment": self.message
         }
 
 
-async def _handle_response(response, dto):
-    model_list = []
-    for info in response:
-        model_list.append(dto(**info))
-    return model_list
+
+class ErrorCodeClass(Enum):
+    pass
+
+
+class ErrorCodeSubClass(Enum):
+    pass
```

### Comparing `bastion_api-0.2.5/PKG-INFO` & `bastion_api-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastion-api
-Version: 0.2.5
+Version: 0.3.0
 Summary: Модуль интеграции с API Бастоин ИКС
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

