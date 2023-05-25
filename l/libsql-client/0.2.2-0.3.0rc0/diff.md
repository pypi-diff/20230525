# Comparing `tmp/libsql-client-0.2.2.tar.gz` & `tmp/libsql_client-0.3.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsql-client-0.2.2.tar", max compression
+gzip compressed data, was "libsql_client-0.3.0rc0.tar", max compression
```

## Comparing `libsql-client-0.2.2.tar` & `libsql_client-0.3.0rc0.tar`

### file list

```diff
@@ -1,19 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-02-27 08:58:08.764134 libsql-client-0.2.2/LICENSE.md
--rw-r--r--   0        0        0     2912 2023-04-27 07:46:00.306317 libsql-client-0.2.2/README.md
--rw-r--r--   0        0        0      268 2023-04-19 10:43:28.755257 libsql-client-0.2.2/libsql_client/__init__.py
--rw-r--r--   0        0        0     3039 2023-04-17 12:00:30.657316 libsql-client-0.2.2/libsql_client/client.py
--rw-r--r--   0        0        0      993 2023-04-17 12:00:30.657316 libsql-client-0.2.2/libsql_client/config.py
--rw-r--r--   0        0        0      801 2023-04-17 12:00:30.657316 libsql-client-0.2.2/libsql_client/create_client.py
--rw-r--r--   0        0        0       85 2023-04-17 12:00:30.657316 libsql-client-0.2.2/libsql_client/hrana/__init__.py
--rw-r--r--   0        0        0     4254 2023-04-28 14:43:03.375368 libsql-client-0.2.2/libsql_client/hrana/client.py
--rw-r--r--   0        0        0    12135 2023-04-28 14:43:03.379368 libsql-client-0.2.2/libsql_client/hrana/conn.py
--rw-r--r--   0        0        0     4816 2023-04-20 09:18:36.654076 libsql-client-0.2.2/libsql_client/hrana/convert.py
--rw-r--r--   0        0        0     1610 2023-04-17 12:00:30.661316 libsql-client-0.2.2/libsql_client/hrana/id_alloc.py
--rw-r--r--   0        0        0     3974 2023-04-17 12:00:30.661316 libsql-client-0.2.2/libsql_client/hrana/proto.py
--rw-r--r--   0        0        0     3441 2023-04-17 12:00:30.661316 libsql-client-0.2.2/libsql_client/http.py
--rw-r--r--   0        0        0     3071 2023-04-28 14:52:18.017515 libsql-client-0.2.2/libsql_client/result.py
--rw-r--r--   0        0        0     4896 2023-04-20 09:19:13.406247 libsql-client-0.2.2/libsql_client/sqlite3.py
--rw-r--r--   0        0        0     7175 2023-05-02 07:53:42.957852 libsql-client-0.2.2/libsql_client/sync.py
--rw-r--r--   0        0        0      960 2023-05-02 08:27:39.682207 libsql-client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 libsql-client-0.2.2/setup.py
--rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 libsql-client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 20:47:51.106565 libsql_client-0.3.0rc0/LICENSE.md
+-rw-r--r--   0        0        0     2912 2023-05-04 20:47:51.106814 libsql_client-0.3.0rc0/README.md
+-rw-r--r--   0        0        0      268 2023-05-04 20:47:51.108622 libsql_client-0.3.0rc0/libsql_client/__init__.py
+-rw-r--r--   0        0        0     3215 2023-05-22 13:09:47.355780 libsql_client-0.3.0rc0/libsql_client/client.py
+-rw-r--r--   0        0        0      993 2023-05-04 20:47:51.108918 libsql_client-0.3.0rc0/libsql_client/config.py
+-rw-r--r--   0        0        0      801 2023-05-04 20:47:51.109050 libsql_client-0.3.0rc0/libsql_client/create_client.py
+-rw-r--r--   0        0        0     2986 2023-05-24 18:03:12.709676 libsql_client-0.3.0rc0/libsql_client/dbapi2/__init__.py
+-rw-r--r--   0        0        0      839 2023-05-24 18:03:12.710251 libsql_client-0.3.0rc0/libsql_client/dbapi2/__main__.py
+-rw-r--r--   0        0        0     6335 2023-05-24 18:03:12.711562 libsql_client-0.3.0rc0/libsql_client/dbapi2/_async_executor.py
+-rw-r--r--   0        0        0    13537 2023-05-24 18:03:12.712336 libsql_client-0.3.0rc0/libsql_client/dbapi2/_reexports.py
+-rw-r--r--   0        0        0       41 2023-05-24 18:03:12.712831 libsql_client-0.3.0rc0/libsql_client/dbapi2/_replace_modules_pythonpath/sqlite3/__init__.py
+-rw-r--r--   0        0        0      661 2023-05-24 18:03:12.713309 libsql_client-0.3.0rc0/libsql_client/dbapi2/_replace_modules_pythonpath/sqlite3/dbapi2.py
+-rw-r--r--   0        0        0     6261 2023-05-24 18:03:12.713933 libsql_client-0.3.0rc0/libsql_client/dbapi2/_utils.py
+-rw-r--r--   0        0        0    12432 2023-05-24 18:03:12.714427 libsql_client-0.3.0rc0/libsql_client/dbapi2/hrana.py
+-rw-r--r--   0        0        0    48342 2023-05-24 18:03:12.715290 libsql_client-0.3.0rc0/libsql_client/dbapi2/types.py
+-rw-r--r--   0        0        0       85 2023-05-04 20:47:51.109237 libsql_client-0.3.0rc0/libsql_client/hrana/__init__.py
+-rw-r--r--   0        0        0     4261 2023-05-22 14:41:16.889969 libsql_client-0.3.0rc0/libsql_client/hrana/client.py
+-rw-r--r--   0        0        0    14518 2023-05-22 14:41:16.890806 libsql_client-0.3.0rc0/libsql_client/hrana/conn.py
+-rw-r--r--   0        0        0     4853 2023-05-22 13:09:47.357397 libsql_client-0.3.0rc0/libsql_client/hrana/convert.py
+-rw-r--r--   0        0        0     1610 2023-05-04 20:47:51.109936 libsql_client-0.3.0rc0/libsql_client/hrana/id_alloc.py
+-rw-r--r--   0        0        0     4988 2023-05-22 14:41:16.891594 libsql_client-0.3.0rc0/libsql_client/hrana/proto.py
+-rw-r--r--   0        0        0     3631 2023-05-22 14:41:16.892225 libsql_client-0.3.0rc0/libsql_client/http.py
+-rw-r--r--   0        0        0     3071 2023-05-04 20:47:51.110394 libsql_client-0.3.0rc0/libsql_client/result.py
+-rw-r--r--   0        0        0     4896 2023-05-22 13:09:47.358497 libsql_client-0.3.0rc0/libsql_client/sqlite3.py
+-rw-r--r--   0        0        0     7175 2023-05-22 13:09:47.358757 libsql_client-0.3.0rc0/libsql_client/sync.py
+-rw-r--r--   0        0        0     1009 2023-05-25 14:16:00.085239 libsql_client-0.3.0rc0/pyproject.toml
+-rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 libsql_client-0.3.0rc0/PKG-INFO
```

### Comparing `libsql-client-0.2.2/LICENSE.md` & `libsql_client-0.3.0rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.2/README.md` & `libsql_client-0.3.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.2/libsql_client/client.py` & `libsql_client-0.3.0rc0/libsql_client/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from datetime import datetime
-from typing import Any, Dict, List, NamedTuple, Optional, Tuple, TypeVar, Union
-from typing_extensions import Protocol
+from typing import TYPE_CHECKING, Any, Dict, List, Tuple, TypeVar, Union
 
 from .result import ResultSet, Value
 
-InValue = Union[Value, bool, datetime]
+if TYPE_CHECKING:
+    from _typeshed import ReadableBuffer
+else:
+    ReadableBuffer = bytes
+
+InValue = Union[Value, bool, datetime, ReadableBuffer]
 InArgs = Union[List[InValue], Tuple[InValue, ...], Dict[str, InValue], None]
 InStatement = Union["Statement", str, Tuple[str], Tuple[str, InArgs]]
 
 class Statement:
     sql: str
     args: InArgs
 
@@ -93,8 +97,10 @@
         self.close()
 
 def _normalize_value(in_value: InValue) -> Value:
     if isinstance(in_value, datetime):
         return int(in_value.timestamp() * 1000)
     elif isinstance(in_value, bool):
         return int(in_value)
-    return in_value
+    elif isinstance(in_value, (str, int, float)) or in_value is None:
+        return in_value
+    return bytes(memoryview(in_value))
```

### Comparing `libsql-client-0.2.2/libsql_client/config.py` & `libsql_client-0.3.0rc0/libsql_client/config.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.2/libsql_client/create_client.py` & `libsql_client-0.3.0rc0/libsql_client/create_client.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.2/libsql_client/hrana/client.py` & `libsql_client-0.3.0rc0/libsql_client/hrana/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import List, Optional, Set
+from typing import List, Optional, Set, Union
 import aiohttp
 import asyncio
 import urllib.parse
 
 from ..client import Client, InArgs, InStatement, LibsqlError, Transaction
 from ..config import _Config
 from ..result import ResultSet
```

### Comparing `libsql-client-0.2.2/libsql_client/hrana/conn.py` & `libsql_client-0.3.0rc0/libsql_client/hrana/conn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 from dataclasses import dataclass
-from typing import Any, Callable, Dict, Optional, TypeVar, cast
+from typing import Any, Callable, Dict, Optional, TypeVar, Union, cast
 import aiohttp
 import asyncio
 import json
 
 from ..client import LibsqlError
 from . import proto
 from .convert import _error_from_proto
@@ -25,42 +25,51 @@
     _receive_task: Optional[asyncio.Task[None]]
     _send_task: Optional[asyncio.Task[None]]
 
     _socket: Optional[aiohttp.ClientWebSocketResponse]
     _send_msg_queue: asyncio.Queue[str]
 
     _recvd_hello: bool
+    _finished_handshake: asyncio.Event
     _response_map: Dict[int, _ResponseState]
     _request_id_alloc: IdAlloc
     _stream_id_alloc: IdAlloc
+    _sql_id_alloc: IdAlloc
 
     exception: Optional[BaseException]
 
     def __init__(self, session: aiohttp.ClientSession, url: str, auth_token: Optional[str] = None):
         self._connect_task = asyncio.create_task(self._do_connect(session, url))
         self._connect_task.add_done_callback(self._done_connect)
         self._receive_task = None
         self._send_task = None
 
         self._socket = None
         self._send_msg_queue = asyncio.Queue()
 
         self._recvd_hello = False
+        self._finished_handshake = asyncio.Event()
         self._response_map = {}
         self._request_id_alloc = IdAlloc()
         self._stream_id_alloc = IdAlloc()
+        self._sql_id_alloc = IdAlloc()
 
         self.exception = None
 
         self._send({"type": "hello", "jwt": auth_token})
 
+    async def wait_connected(self) -> None:
+        await self._finished_handshake.wait()
+        if self.exception:
+            raise self.exception
+
     async def _do_connect(self, session: aiohttp.ClientSession, url: str) -> aiohttp.ClientWebSocketResponse:
         return await session.ws_connect(
             url,
-            protocols=["hrana1"],
+            protocols=["hrana2"],
             autoclose=False,
             autoping=True,
         )
 
     def _done_connect(self, task: asyncio.Task[aiohttp.ClientWebSocketResponse]) -> None:
         e: Optional[BaseException]
         if task.cancelled():
@@ -153,14 +162,15 @@
         assert self.exception is None
         self._send_msg_queue.put_nowait(json.dumps(msg))
 
     def _set_exception(self, e: BaseException) -> None:
         if self.exception is not None:
             return
         self.exception = e
+        self._finished_handshake.set()
 
         for task in (self._connect_task, self._receive_task, self._send_task):
             if task is not None:
                 task.cancel()
 
         for request_id, response_state in self._response_map.items():
             response_state.future.set_exception(e)
@@ -188,14 +198,15 @@
         except ValueError as e:
             raise LibsqlError("Server message is not valid JSON", "HRANA_PROTO_ERROR") from e
 
         if msg["type"] in ("hello_ok", "hello_error"):
             if self._recvd_hello:
                 raise LibsqlError("Received a duplicated error response", "HRANA_PROTO_ERROR")
             self._recvd_hello = True
+            self._finished_handshake.set()
 
             if msg["type"] == "hello_error":
                 raise _error_from_proto(msg["error"])
             return
         elif not self._recvd_hello:
             raise LibsqlError("Received a non-hello message before hello response", "HRANA_PROTO_ERROR")
 
@@ -246,28 +257,66 @@
         return HranaStream(self, stream_state)
 
     def _close_stream(self, stream_state: _StreamState, e: BaseException) -> None:
         if stream_state.closed is not None or self.exception is not None:
             return
         stream_state.closed = e
 
-        def close_done(_fut: asyncio.Future[proto.Response]) -> None:
+        def close_done(fut: asyncio.Future[proto.Response]) -> None:
             self._stream_id_alloc.free(stream_state.stream_id)
+            if not fut.cancelled():
+                fut.exception()
 
         close_fut = self.send_request({
             "type": "close_stream",
             "stream_id": stream_state.stream_id,
         })
         close_fut.add_done_callback(close_done)
 
     async def close(self) -> None:
         self._set_exception(LibsqlError("Client was manually closed", "CLIENT_CLOSED"))
         if self._socket is not None:
             await self._socket.close()
 
+    def store_sql(self, sql: str) -> int:
+        sql_id = self._sql_id_alloc.alloc()
+
+        def store_sql_done(fut: asyncio.Future[proto.Response]) -> None:
+            e: Optional[BaseException]
+            if fut.cancelled():
+                e = asyncio.CancelledError("store_sql was cancelled")
+            else:
+                e = fut.exception()
+            if e is not None:
+                self._sql_id_alloc.free(sql_id)
+
+        store_sql_fut = self.send_request({
+            "type": "store_sql",
+            "sql_id": sql_id,
+            "sql": sql,
+        })
+        store_sql_fut.add_done_callback(store_sql_done)
+        return sql_id
+
+    def close_sql(self, sql_id: int) -> None:
+        if self.exception is not None:
+            return
+
+        def close_sql_done(fut: asyncio.Future[proto.Response]) -> None:
+            self._sql_id_alloc.free(sql_id)
+            if not fut.cancelled():
+                fut.exception()
+
+        close_sql_fut = self.send_request( {
+            "type": "close_sql",
+            "sql_id": sql_id,
+        })
+        close_sql_fut.add_done_callback(close_sql_done)
+
+
 class HranaStream:
     _conn: HranaConn
     _state: _StreamState
 
     def __init__(self, conn: HranaConn, state: _StreamState):
         self._conn = conn
         self._state = state
@@ -283,14 +332,38 @@
         }
         response_fut = self._conn.send_request(request)
 
         def get_result(response: proto.Response) -> proto.StmtResult:
             return cast(proto.ExecuteResp, response)["result"]
         return _map_future(response_fut, get_result)
 
+    def sequence(self, stmt: Union[str, int]) -> asyncio.Future[None]:
+        if self._state.closed is not None:
+            raise LibsqlError("Stream was closed", "STREAM_CLOSED") from self._state.closed
+
+        request: proto.SequenceReq
+        if isinstance(stmt, str):
+            request = {
+                "type": "sequence",
+                "stream_id": self._state.stream_id,
+                "sql": stmt,
+            }
+        else:
+            request = {
+                "type": "sequence",
+                "stream_id": self._state.stream_id,
+                "sql_id": stmt,
+            }
+
+        response_fut = self._conn.send_request(request)
+
+        def get_result(response: proto.Response) -> None:
+            return None
+        return _map_future(response_fut, get_result)
+
     def batch(self, batch: proto.Batch) -> asyncio.Future[proto.BatchResult]:
         if self._state.closed is not None:
             raise LibsqlError("Stream was closed", "STREAM_CLOSED") from self._state.closed
 
         request: proto.BatchReq = {
             "type": "batch",
             "stream_id": self._state.stream_id,
```

### Comparing `libsql-client-0.2.2/libsql_client/hrana/convert.py` & `libsql_client-0.3.0rc0/libsql_client/hrana/convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,18 +101,20 @@
         if value < _MIN_INTEGER or value > _MAX_INTEGER:
             raise OverflowError("Integer exceeds the range of SQLite integers (64 bits, signed)")
         return {"type": "integer", "value": str(value)}
     elif isinstance(value, float):
         if not math.isfinite(value):
             raise ValueError("Only finite floats (not Infinity or NaN) are supported")
         return {"type": "float", "value": value}
-    elif isinstance(value, bytes):
-        return {"type": "blob", "base64": base64.b64encode(value).decode()}
     else:
-        raise TypeError(f"Unsupported value of type {type(value)}")
+        try:
+            data = base64.b64encode(value).decode()
+            return {"type": "blob", "base64": data }
+        except TypeError:
+            raise TypeError(f"Unsupported value of type {type(value)}")
 
 _MIN_INTEGER = -2**63
 _MAX_INTEGER = 2**63-1
 
 def _value_from_proto(value: proto.Value) -> Value:
     if value["type"] == "null":
         return None
```

### Comparing `libsql-client-0.2.2/libsql_client/hrana/id_alloc.py` & `libsql_client-0.3.0rc0/libsql_client/hrana/id_alloc.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.2/libsql_client/hrana/proto.py` & `libsql_client-0.3.0rc0/libsql_client/hrana/proto.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,22 +22,25 @@
 
 NamedArg = TypedDict("NamedArg", {
     "name": str,
     "value": Value,
 })
 
 Stmt = TypedDict("Stmt", {
-    "sql": str,
+    # NOTE: must provide one of sql or sql_id
+    "sql":  NotRequired[str],
+    "sql_id": NotRequired[int],
     "args": NotRequired[List[Value]],
     "named_args": NotRequired[List[NamedArg]],
     "want_rows": bool,
 })
 
 Col = TypedDict("Col", {
     "name": Optional[str],
+    "decltype": NotRequired[Optional[str]],
 })
 
 StmtResult = TypedDict("StmtResult", {
     "cols": List[Col],
     "rows": List[List[Value]],
     "affected_row_count": int,
     "last_insert_rowid": NotRequired[Optional[str]],
@@ -50,14 +53,30 @@
 })
 
 ExecuteResp = TypedDict("ExecuteResp", {
     "type": Literal["execute"],
     "result": StmtResult,
 })
 
+
+### Execute a sequence of SQL statements
+
+SequenceReq = TypedDict("SequenceReq", {
+    "type": Literal["sequence"],
+    "stream_id": int,
+    # NOTE: must provide one of sql or sql_id
+    "sql":  NotRequired[str],
+    "sql_id": NotRequired[int],
+})
+
+SequenceResp = TypedDict("SequenceResp", {
+    "type": Literal["sequence"],
+})
+
+
 ### Execute a batch
 
 BatchCondOk = TypedDict("BatchCondOk", {"type": Literal["ok"], "step": int})
 BatchCondError = TypedDict("BatchCondError", {"type": Literal["error"], "step": int})
 BatchCondNot = TypedDict("BatchCondNot", {"type": Literal["not"], "cond": "BatchCond"})
 BatchCondAnd = TypedDict("BatchCondAnd", {"type": Literal["and"], "conds": List["BatchCond"]})
 BatchCondOr = TypedDict("BatchCondOr", {"type": Literal["or"], "conds": List["BatchCond"]})
@@ -122,34 +141,64 @@
 })
 
 HelloErrorMsg = TypedDict("HelloErrorMsg", {
     "type": Literal["hello_error"],
     "error": Error,
 })
 
+### Store an SQL text on the server
+
+StoreSqlReq = TypedDict("StoreSqlReq", {
+    "type": Literal["store_sql"],
+    "sql_id": int,
+    "sql": str,
+})
+
+StoreSqlResp = TypedDict("StoreSqlResp", {
+    "type": Literal["store_sql"],
+})
+
+### Close a stored SQL text
+
+CloseSqlReq = TypedDict("CloseSqlReq", {
+    "type": Literal["close_sql"],
+    "sql_id": int,
+})
+
+CloseSqlResp = TypedDict("CloseSqlResp", {
+    "type": Literal["close_sql"],
+})
+
+
 ### Request/response
 
 Request = Union[
     OpenStreamReq,
     CloseStreamReq,
     ExecuteReq,
     BatchReq,
+    StoreSqlReq,
+    CloseSqlReq,
+    SequenceReq,
 ]
 
 RequestMsg = TypedDict("RequestMsg", {
     "type": Literal["request"],
     "request_id": int,
     "request": Request,
 })
 
 Response = Union[
     OpenStreamResp,
     CloseStreamResp,
     ExecuteResp,
     BatchResp,
+    StoreSqlResp,
+    CloseSqlResp,
+    SequenceResp,
 ]
 
 ResponseOkMsg = TypedDict("ResponseOkMsg", {
     "type": Literal["response_ok"],
     "request_id": int,
     "response": Response,
 })
```

### Comparing `libsql-client-0.2.2/libsql_client/http.py` & `libsql_client-0.3.0rc0/libsql_client/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Any, List, Optional, cast
+from typing import Any, List, Optional, Union, cast
 from typing_extensions import TypedDict
 import aiohttp
 import urllib.parse
 
 from .client import Client, InArgs, InStatement, LibsqlError, Transaction
 from .config import _Config
 from .hrana import proto
@@ -34,14 +34,20 @@
         request: _ExecuteReq = {
             "stmt": _stmt_to_proto(stmt, args),
         }
         response = await self._send("POST", "v1/execute", request)
         proto_res = cast(_ExecuteResp, response)["result"]
         return _result_set_from_proto(proto_res)
 
+    async def sequence(self, stmt: str) -> None:
+        raise LibsqlError(
+            "The HTTP client does not support sequence.",
+            "SEQUENCE_NOT_SUPPORTED",
+        )
+
     async def batch(self, stmts: List[InStatement]) -> List[ResultSet]:
         request: _BatchReq = {
             "batch": _batch_to_proto(stmts),
         }
         response = await self._send("POST", "v1/batch", request)
         proto_res = cast(_BatchResp, response)["result"]
         return _batch_results_from_proto(proto_res, len(stmts))
```

### Comparing `libsql-client-0.2.2/libsql_client/result.py` & `libsql_client-0.3.0rc0/libsql_client/result.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.2/libsql_client/sqlite3.py` & `libsql_client-0.3.0rc0/libsql_client/sqlite3.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.2/libsql_client/sync.py` & `libsql_client-0.3.0rc0/libsql_client/sync.py`

 * *Files identical despite different names*

### Comparing `libsql-client-0.2.2/pyproject.toml` & `libsql_client-0.3.0rc0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "libsql-client"
-version = "0.2.2"
+version = "0.3.0-pre"
 authors = [
+    "Gustavo Barbieri <barbieri@gmail.com>",
     "Jan Špaček <honza@chiselstrike.com>",
     "ChiselStrike",
 ]
 description = "Python SDK for libSQL"
 homepage = "https://github.com/libsql/libsql-client-py"
 repository = "https://github.com/libsql/libsql-client-py"
 documentation = "https://libsql.org/libsql-client-py/"
```

### Comparing `libsql-client-0.2.2/PKG-INFO` & `libsql_client-0.3.0rc0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: libsql-client
-Version: 0.2.2
+Version: 0.3.0rc0
 Summary: Python SDK for libSQL
 Home-page: https://github.com/libsql/libsql-client-py
 License: MIT
-Author: Jan Špaček
-Author-email: honza@chiselstrike.com
+Author: Gustavo Barbieri
+Author-email: barbieri@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.0,<4.0)
 Requires-Dist: typing-extensions (>=4.5,<5.0)
 Project-URL: Documentation, https://libsql.org/libsql-client-py/
 Project-URL: Repository, https://github.com/libsql/libsql-client-py
 Description-Content-Type: text/markdown
 
 # Python SDK for libSQL
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

