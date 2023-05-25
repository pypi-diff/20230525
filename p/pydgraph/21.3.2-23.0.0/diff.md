# Comparing `tmp/pydgraph-21.3.2.tar.gz` & `tmp/pydgraph-23.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydgraph-21.3.2.tar", last modified: Thu Aug  5 16:18:29 2021, max compression
+gzip compressed data, was "pydgraph-23.0.0.tar", last modified: Thu May 25 17:44:20 2023, max compression
```

## Comparing `pydgraph-21.3.2.tar` & `pydgraph-23.0.0.tar`

### file list

```diff
@@ -1,28 +1,38 @@
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2021-08-05 16:18:29.592094 pydgraph-21.3.2/
--rwxr-xr-x   0 dmai      (1000) dmai      (1000)    10172 2018-12-12 21:47:13.000000 pydgraph-21.3.2/LICENSE
--rwxr-xr-x   0 dmai      (1000) dmai      (1000)       32 2018-12-12 21:47:13.000000 pydgraph-21.3.2/MANIFEST.in
--rw-rw-r--   0 dmai      (1000) dmai      (1000)    20652 2021-08-05 16:18:29.592094 pydgraph-21.3.2/PKG-INFO
--rw-rw-r--   0 dmai      (1000) dmai      (1000)    15843 2021-08-04 20:49:35.000000 pydgraph-21.3.2/README.md
--rw-rw-r--   0 dmai      (1000) dmai      (1000)       62 2021-08-04 19:59:42.000000 pydgraph-21.3.2/publishing-requirements.txt
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2021-08-05 16:18:29.592094 pydgraph-21.3.2/pydgraph/
--rwxr-xr-x   0 dmai      (1000) dmai      (1000)      849 2019-09-05 19:07:28.000000 pydgraph-21.3.2/pydgraph/__init__.py
--rwxrwxr-x   0 dmai      (1000) dmai      (1000)     6648 2021-07-27 17:23:19.000000 pydgraph-21.3.2/pydgraph/client.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     4640 2021-08-05 16:06:50.000000 pydgraph-21.3.2/pydgraph/client_stub.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     1755 2021-07-27 17:23:19.000000 pydgraph-21.3.2/pydgraph/errors.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)      636 2021-08-05 16:18:02.000000 pydgraph-21.3.2/pydgraph/meta.py
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2021-08-05 16:18:29.592094 pydgraph-21.3.2/pydgraph/proto/
--rw-r--r--   0 dmai      (1000) dmai      (1000)        0 2018-12-12 21:47:13.000000 pydgraph-21.3.2/pydgraph/proto/__init__.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)    53769 2021-07-27 17:48:53.000000 pydgraph-21.3.2/pydgraph/proto/api_pb2.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     4076 2021-07-27 17:48:53.000000 pydgraph-21.3.2/pydgraph/proto/api_pb2_grpc.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)    12606 2021-07-27 17:23:19.000000 pydgraph-21.3.2/pydgraph/txn.py
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     1952 2021-07-27 17:23:19.000000 pydgraph-21.3.2/pydgraph/util.py
-drwxrwxr-x   0 dmai      (1000) dmai      (1000)        0 2021-08-05 16:18:29.592094 pydgraph-21.3.2/pydgraph.egg-info/
--rw-r--r--   0 dmai      (1000) dmai      (1000)    20652 2021-08-05 16:18:29.000000 pydgraph-21.3.2/pydgraph.egg-info/PKG-INFO
--rw-r--r--   0 dmai      (1000) dmai      (1000)      475 2021-08-05 16:18:29.000000 pydgraph-21.3.2/pydgraph.egg-info/SOURCES.txt
--rw-r--r--   0 dmai      (1000) dmai      (1000)        1 2021-08-05 16:18:29.000000 pydgraph-21.3.2/pydgraph.egg-info/dependency_links.txt
--rw-r--r--   0 dmai      (1000) dmai      (1000)       31 2021-08-05 16:18:29.000000 pydgraph-21.3.2/pydgraph.egg-info/requires.txt
--rw-r--r--   0 dmai      (1000) dmai      (1000)        9 2021-08-05 16:18:29.000000 pydgraph-21.3.2/pydgraph.egg-info/top_level.txt
--rw-rw-r--   0 dmai      (1000) dmai      (1000)     2534 2021-08-04 18:16:43.000000 pydgraph-21.3.2/r.txt
--rwxrwxr-x   0 dmai      (1000) dmai      (1000)       31 2019-08-30 23:31:40.000000 pydgraph-21.3.2/requirements.txt
--rw-r--r--   0 dmai      (1000) dmai      (1000)      108 2021-08-05 16:18:29.596094 pydgraph-21.3.2/setup.cfg
--rwxrwxr-x   0 dmai      (1000) dmai      (1000)     1691 2021-07-27 17:23:19.000000 pydgraph-21.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:44:20.046277 pydgraph-23.0.0/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10172 2023-05-25 17:42:30.000000 pydgraph-23.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    29505 2023-05-25 17:44:20.046277 pydgraph-23.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    17322 2023-05-25 17:42:30.000000 pydgraph-23.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:44:20.042277 pydgraph-23.0.0/pydgraph/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      849 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6648 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/client_stub.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2876 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1754 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:44:20.046277 pydgraph-23.0.0/pydgraph/proto/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7961 2023-05-25 17:44:13.000000 pydgraph-23.0.0/pydgraph/proto/api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7821 2023-05-25 17:44:13.000000 pydgraph-23.0.0/pydgraph/proto/api_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12606 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/txn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pydgraph/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:44:20.046277 pydgraph-23.0.0/pydgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    29505 2023-05-25 17:44:20.000000 pydgraph-23.0.0/pydgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-05-25 17:44:20.000000 pydgraph-23.0.0/pydgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 17:44:20.000000 pydgraph-23.0.0/pydgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-05-25 17:44:20.000000 pydgraph-23.0.0/pydgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-25 17:44:20.000000 pydgraph-23.0.0/pydgraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      915 2023-05-25 17:42:30.000000 pydgraph-23.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 17:44:20.046277 pydgraph-23.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 17:44:20.046277 pydgraph-23.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     7787 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_acct_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5185 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_acl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2984 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_client_stub.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16449 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1946 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_essentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3882 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18545 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_txn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2980 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_type_system.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5986 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_upsert_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1300 2023-05-25 17:42:30.000000 pydgraph-23.0.0/tests/test_util.py
```

### Comparing `pydgraph-21.3.2/LICENSE` & `pydgraph-23.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydgraph-21.3.2/PKG-INFO` & `pydgraph-23.0.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,533 +1,552 @@
-Metadata-Version: 2.1
-Name: pydgraph
-Version: 21.3.2
-Summary: Official Dgraph client implementation for Python
-Home-page: https://github.com/dgraph-io/pydgraph
-Author: Dgraph Labs
-Author-email: contact@dgraph.io
-License: Apache License, Version 2.0
-Description: # pydgraph
-        
-        This is the official Dgraph database client implementation for Python (Python >= v2.7 and >= v3.5), using [gRPC][grpc].
-        
-        [grpc]: https://grpc.io/
-        
-        This client follows the [Dgraph Go client][goclient] closely.
-        
-        **Use [Discuss Issues](https://discuss.dgraph.io/c/issues/35/clients/46) to report issues about this repository.**
-        
-        [goclient]: https://github.com/dgraph-io/dgo
-        
-        Before using this client, we highly recommend that you read the [Dgraph Python
-        Client docs](https://dgraph.io/docs/clients/python/), as well as reviewing
-        the product documentation at [docs.dgraph.io].
-        
-        [docs.dgraph.io]:https://docs.dgraph.io
-        
-        ## Table of contents
-        
-        - [Install](#install)
-        - [Supported Versions](#supported-versions)
-        - [Quickstart](#quickstart)
-        - [Using a Client](#using-a-client)
-          - [Creating a Client](#creating-a-client)
-          - [Altering the Database](#altering-the-database)
-          - [Creating a Transaction](#creating-a-transaction)
-          - [Running a Mutation](#running-a-mutation)
-          - [Committing a Transaction](#committing-a-transaction)
-          * [Running a Query](#running-a-query)
-          * [Running an Upsert: Query + Mutation](#running-an-upsert-query--mutation)
-          * [Running a Conditional Upsert](#running-a-conditional-upsert)
-          - [Cleaning up Resources](#cleaning-up-resources)
-          - [Setting Metadata Headers](#setting-metadata-headers)
-        - [Examples](#examples)
-        - [Development](#development)
-          - [Building the source](#building-the-source)
-          - [Running tests](#running-tests)
-        
-        ## Install
-        
-        Install using pip:
-        
-        ```sh
-        pip install pydgraph
-        ```
-        
-        ### Install Notes
-        
-        To avoid issues when adding composite credentials or when using client authorization, please install gRPC version 1.19.0:
-        
-        ```sh
-        pip install grpcio==1.19.0
-        ```
-        
-        ## Supported Versions
-        
-        Depending on the version of Dgraph that you are connecting to, you will have to
-        use a different version of this client.
-        
-        | Dgraph version |   pydgraph version   |
-        |:--------------:|:--------------------:|
-        |     1.0.X      |      <= *1.2.0*      |
-        |     1.1.X      |      >= *2.0.0*      |
-        |     1.2.X      |      >= *2.0.0*      |
-        
-        ## Quickstart
-        
-        Build and run the [simple project][simple] in the `examples` folder, which
-        contains an end-to-end example of using the Dgraph python client. For additional details, follow the
-        instructions in the project's [README](./examples/simple/README.md).
-        
-        [simple]: ./examples/simple
-        
-        ## Using a client
-        
-        ### Creating a Client
-        
-        You can initialize a `DgraphClient` object by passing it a list of
-        `DgraphClientStub` clients as variadic arguments. Connecting to multiple Dgraph
-        servers in the same cluster allows for better distribution of workload.
-        
-        The following code snippet shows just one connection.
-        
-        ```python
-        import pydgraph
-        
-        client_stub = pydgraph.DgraphClientStub('localhost:9080')
-        client = pydgraph.DgraphClient(client_stub)
-        ```
-        
-        ### Altering the Database
-        
-        To set the schema, create an `Operation` object, set the schema and pass it to
-        `DgraphClient#alter(Operation)` method.
-        
-        ```python
-        schema = 'name: string @index(exact) .'
-        op = pydgraph.Operation(schema=schema)
-        client.alter(op)
-        ```
-        
-        Starting with Dgraph version 20.03.0, indexes can be computed in the background.
-        You can set the `run_in_background` field of `pydgraph.Operation` to `True`
-        before passing it to the `Alter` function. You can find more details
-        [here](https://docs.dgraph.io/master/query-language/#indexes-in-background).
-        
-        ```python
-        schema = 'name: string @index(exact) .'
-        op = pydgraph.Operation(schema=schema, run_in_background=True)
-        client.alter(op)
-        ```
-        
-        `Operation` contains other fields as well, including the `drop` predicate and `drop all`.
-        Drop all is useful if you wish to discard all the data, and start with a clean
-        slate, without bringing the instance down.
-        
-        ```python
-        # Drop all data including schema from the Dgraph instance. This is a useful
-        # for small examples such as this since it puts Dgraph into a clean state.
-        op = pydgraph.Operation(drop_all=True)
-        client.alter(op)
-        ```
-        
-        ### Creating a Transaction
-        
-        To create a transaction, call the `DgraphClient#txn()` method, which returns a
-        new `Txn` object. This operation incurs no network overhead.
-        
-        It is good practice to call `Txn#discard()` in a `finally` block after running
-        the transaction. Calling `Txn#discard()` after `Txn#commit()` is a no-op
-        and you can call `Txn#discard()` multiple times with no additional side-effects.
-        
-        ```python
-        txn = client.txn()
-        try:
-          # Do something here
-          # ...
-        finally:
-          txn.discard()
-          # ...
-        ```
-        
-        To create a read-only transaction, call `DgraphClient#txn(read_only=True)`.
-        Read-only transactions are ideal for transactions which only involve queries.
-        Mutations and commits are not allowed.
-        
-        ```python
-        txn = client.txn(read_only=True)
-        try:
-          # Do some queries here
-          # ...
-        finally:
-          txn.discard()
-          # ...
-        ```
-        
-        To create a read-only transaction that executes best-effort queries, call
-        `DgraphClient#txn(read_only=True, best_effort=True)`. Best-effort queries are
-        faster than normal queries because they bypass the normal consensus protocol.
-        For this same reason, best-effort queries cannot guarantee to return the latest
-        data. Best-effort queries are only supported by read-only transactions.
-        
-        ### Running a Mutation
-        
-        `Txn#mutate(mu=Mutation)` runs a mutation. It takes in a `Mutation` object,
-        which provides two main ways to set data: JSON and RDF N-Quad. You can choose
-        whichever way is convenient.
-        
-        `Txn#mutate()` provides convenience keyword arguments `set_obj` and `del_obj`
-        for setting JSON values and `set_nquads` and `del_nquads` for setting N-Quad
-        values. See examples below for usage.
-        
-        We define a person object to represent a person and use it in a transaction.
-        
-        ```python
-        # Create data.
-        p = {
-            'name': 'Alice',
-        }
-        
-        # Run mutation.
-        txn.mutate(set_obj=p)
-        
-        # If you want to use a mutation object, use this instead:
-        # mu = pydgraph.Mutation(set_json=json.dumps(p).encode('utf8'))
-        # txn.mutate(mu)
-        
-        # If you want to use N-Quads, use this instead:
-        # txn.mutate(set_nquads='_:alice <name> "Alice" .')
-        ```
-        
-        ```python
-        # Delete data.
-        
-        query = """query all($a: string)
-         {
-           all(func: eq(name, $a))
-            {
-              uid
-            }
-          }"""
-        
-        variables = {'$a': 'Bob'}
-        
-        res = txn.query(query, variables=variables)
-        ppl = json.loads(res.json)
-        
-        # For a mutation to delete a node, use this:
-        txn.mutate(del_obj=person)
-        ```
-        
-        For a complete example with multiple fields and relationships, look at the
-        [simple project][simple] in the `examples` folder.
-        
-        Sometimes, you only want to commit a mutation, without querying anything further.
-        In such cases, you can set the keyword argument `commit_now=True` to indicate
-        that the mutation must be immediately committed.
-        
-        A mutation can be executed using `txn.do_request` as well.
-        
-        ```python
-        mutation = txn.create_mutation(set_nquads='_:alice <name> "Alice" .')
-        request = txn.create_request(mutations=[mutation], commit_now=True)
-        txn.do_request(request)
-        ```
-        
-        ### Committing a Transaction
-        
-        A transaction can be committed using the `Txn#commit()` method. If your transaction
-        consist solely of `Txn#query` or `Txn#queryWithVars` calls, and no calls to
-        `Txn#mutate`, then calling `Txn#commit()` is not necessary.
-        
-        An error is raised if another transaction(s) modify the same data concurrently that was
-        modified in the current transaction. It is up to the user to retry transactions
-        when they fail.
-        
-        ```python
-        txn = client.txn()
-        try:
-          # ...
-          # Perform any number of queries and mutations
-          # ...
-          # and finally...
-          txn.commit()
-        except pydgraph.AbortedError:
-          # Retry or handle exception.
-        finally:
-          # Clean up. Calling this after txn.commit() is a no-op
-          # and hence safe.
-          txn.discard()
-        ```
-        
-        ### Running a Query
-        
-        You can run a query by calling `Txn#query(string)`. You will need to pass in a
-        [DQL](https://dgraph.io/docs/query-language/) query string. If you want to pass an additional dictionary of any
-        variables that you might want to set in the query, call
-        `Txn#query(string, variables=d)` with the variables dictionary `d`.
-        
-        The query response contains the `json` field, which returns the JSON response.
-        
-        Let’s run a query with a variable `$a`, deserialize the result from JSON and
-        print it out:
-        
-        ```python
-        # Run query.
-        query = """query all($a: string) {
-          all(func: eq(name, $a))
-          {
-            name
-          }
-        }"""
-        variables = {'$a': 'Alice'}
-        
-        res = txn.query(query, variables=variables)
-        
-        # If not doing a mutation in the same transaction, simply use:
-        # res = client.txn(read_only=True).query(query, variables=variables)
-        
-        ppl = json.loads(res.json)
-        
-        # Print results.
-        print('Number of people named "Alice": {}'.format(len(ppl['all'])))
-        for person in ppl['all']:
-          print(person)
-        ```
-        
-        This should print:
-        
-        ```console
-        Number of people named "Alice": 1
-        Alice
-        ```
-        
-        You can also use `txn.do_request` function to run the query.
-        
-        ```python
-        request = txn.create_request(query=query)
-        txn.do_request(request)
-        ```
-        
-        ### Running an Upsert: Query + Mutation
-        
-        The `txn.do_request` function allows you to use upsert blocks. An upsert block
-        contains one query block and one or more mutation blocks, so it lets you perform
-        queries and mutations in a single request. Variables defined in the query block
-        can be used in the mutation blocks using the `uid` and `val` functions
-        implemented by DQL.
-        
-        To learn more about upsert blocks, see the
-        [Upsert Block documentation](https://dgraph.io/docs/mutations/upsert-block/).
-        
-        ```python
-        query = """{
-          u as var(func: eq(name, "Alice"))
-        }"""
-        nquad = """
-          uid(u) <name> "Alice" .
-          uid(u) <age> "25" .
-        """
-        mutation = txn.create_mutation(set_nquads=nquad)
-        request = txn.create_request(query=query, mutations=[mutation], commit_now=True)
-        txn.do_request(request)
-        ```
-        
-        ### Running a Conditional Upsert
-        
-        The upsert block also allows specifying a conditional mutation block using an `@if` directive. The mutation is executed
-        only when the specified condition is true. If the condition is false, the mutation is silently ignored.
-        
-        See more about Conditional Upserts [here](https://docs.dgraph.io/mutations/#conditional-upsert).
-        
-        ```python
-        query = """
-          {
-            user as var(func: eq(email, "wrong_email@dgraph.io"))
-          }
-        """
-        cond = "@if(eq(len(user), 1))"
-        nquads = """
-          uid(user) <email> "correct_email@dgraph.io" .
-        """
-        mutation = txn.create_mutation(cond=cond, set_nquads=nquads)
-        request = txn.create_request(mutations=[mutation], query=query, commit_now=True)
-        txn.do_request(request)
-        ```
-        
-        ### Cleaning Up Resources
-        
-        To clean up resources, you have to call `DgraphClientStub#close()` individually for
-        all the instances of `DgraphClientStub`.
-        
-        ```python
-        SERVER_ADDR = "localhost:9080"
-        
-        # Create instances of DgraphClientStub.
-        stub1 = pydgraph.DgraphClientStub(SERVER_ADDR)
-        stub2 = pydgraph.DgraphClientStub(SERVER_ADDR)
-        
-        # Create an instance of DgraphClient.
-        client = pydgraph.DgraphClient(stub1, stub2)
-        
-        # ...
-        # Use client
-        # ...
-        
-        # Clean up resources by closing all client stubs.
-        stub1.close()
-        stub2.close()
-        ```
-        
-        ### Setting Metadata Headers
-        
-        Metadata headers such as authentication tokens can be set through the metadata of gRPC methods. Below is an example of how to set a header named "auth-token".
-        
-        ```python
-        # The following piece of code shows how one can set metadata with
-        # auth-token, to allow Alter operation, if the server requires it.
-        # metadata is a list of arbitrary key-value pairs.
-        metadata = [("auth-token", "the-auth-token-value")]
-        dg.alter(op, metadata=metadata)
-        ```
-        
-        ### Setting a timeout
-        
-        A timeout value representing the number of seconds can be passed to the `login`,
-        `alter`, `query`, and `mutate` methods using the `timeout` keyword argument.
-        
-        For example, the following alters the schema with a timeout of ten seconds:
-        `dg.alter(op, timeout=10)`
-        
-        ### Passing credentials
-        
-        A `CallCredentials` object can be passed to the `login`, `alter`, `query`, and
-        `mutate` methods using the `credentials` keyword argument.
-        
-        ### Authenticating to a reverse TLS proxy
-        
-        If the Dgraph instance is behind a reverse TLS proxy, credentials can also be
-        passed through the methods available in the gRPC library. Note that in this case
-        every request will need to include the credentials. In the example below, we are
-        trying to add authentication to a proxy that requires an API key. This value is
-        expected to be included in the metadata using the key "authorization".
-        
-        ```python
-        creds = grpc.ssl_channel_credentials()
-        call_credentials = grpc.metadata_call_credentials(
-            lambda context, callback: callback((("authorization", "<api-key>"),), None))
-        composite_credentials = grpc.composite_channel_credentials(creds, call_credentials)
-        client_stub = pydgraph.DgraphClientStub(
-            '{host}:{port}'.format(host=GRPC_HOST, port=GRPC_PORT), composite_credentials)
-        client = pydgraph.DgraphClient(client_stub)
-        ```
-        
-        ### Async methods
-        
-        The `alter` method in the client has an asynchronous version called
-        `async_alter`. The async methods return a future. You can directly call the
-        `result` method on the future. However. The DgraphClient class provides a static
-        method `handle_alter_future` to handle any possible exception.
-        
-        ```python
-        alter_future = self.client.async_alter(pydgraph.Operation(
-        	schema="name: string @index(term) ."))
-        response = pydgraph.DgraphClient.handle_alter_future(alter_future)
-        ```
-        
-        The `query` and `mutate` methods int the `Txn` class also have async versions
-        called `async_query` and `async_mutation` respectively. These functions work
-        just like `async_alter`.
-        
-        You can use the `handle_query_future` and `handle_mutate_future` static methods
-        in the `Txn` class to retrieve the result. A short example is given below:
-        
-        ```python
-        txn = client.txn()
-        query = "query body here"
-        future = txn.async_query()
-        response = pydgraph.Txn.handle_query_future(future)
-        ```
-        
-        A working example can be found in the `test_asycn.py` test file.
-        
-        Keep in mind that due to the nature of async calls, the async functions cannot
-        retry the request if the login is invalid. You will have to check for this error
-        and retry the login (with the function `retry_login` in both the `Txn` and
-        `Client` classes). A short example is given below:
-        
-        ```python
-        client = DgraphClient(client_stubs) # client_stubs is a list of gRPC stubs.
-        alter_future = client.async_alter()
-        try:
-            response = alter_future.result()
-        except Exception as e:
-        	# You can use this function in the util package to check for JWT
-            # expired errors.
-            if pydgraph.util.is_jwt_expired(e):
-                # retry your request here.
-        ```
-        
-        ## Examples
-        
-        - [simple][]: Quickstart example of using pydgraph.
-        
-        ## Development
-        
-        ### Building the source
-        
-        ```sh
-        python setup.py install
-        # To install for the current user, use this instead:
-        # python setup.py install --user
-        ```
-        
-        If you have made changes to the `pydgraph/proto/api.proto` file, you need need
-        to regenerate the source files generated by Protocol Buffer tools. To do that,
-        install the [grpcio-tools][grpcio-tools] library and then run the following
-        command:
-        
-        [grpcio-tools]: https://pypi.python.org/pypi/grpcio-tools
-        
-        ```sh
-        python scripts/protogen.py
-        ```
-        
-        The generated file `api_pb2_grpc.py` needs to be changed in recent versions of python.
-        The required change is outlined below as a diff.
-        
-        ```diff
-        -import api_pb2 as api__pb2
-        +from . import api_pb2 as api__pb2
-        ```
-        
-        ### Running tests
-        
-        To run the tests in your local machine, install and run `tox`:
-        
-        ```bash
-        pip install tox
-        tox
-        ```
-        
-        This script assumes Dgraph and [dgo](https://github.com/dgraph-io/dgo) (Go
-        client) are already built on the local machine and that their code is in
-        `$GOPATH/src`. It also requires that docker and docker-compose are installed in
-        your machine.
-        
-        The script will take care of bringing up a Dgraph cluster and bringing it down
-        after the tests are executed. The script connects to randomly selected ports for
-        HTTP and gRPC requests to prevent interference with clusters running on the
-        default port. Docker and docker-compose need to be installed before running the
-        script. Refer to the official [Docker documentation](https://docs.docker.com/)
-        for instructions on how to install those packages.
-        
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Database
-Classifier: Topic :: Software Development
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Description-Content-Type: text/markdown
+# pydgraph
+
+This is the official Dgraph database client implementation for Python (Python >= v3.7), using [gRPC][grpc].
+
+[grpc]: https://grpc.io/
+
+This client follows the [Dgraph Go client][goclient] closely.
+
+[goclient]: https://github.com/dgraph-io/dgo
+
+Before using this client, we highly recommend that you read the
+the product documentation at [dgraph.io/docs].
+
+[dgraph.io/docs]:https://dgraph.io/docs
+
+## Table of contents
+- [pydgraph](#pydgraph)
+  - [Table of contents](#table-of-contents)
+  - [Install](#install)
+  - [Supported Versions](#supported-versions)
+  - [Quickstart](#quickstart)
+  - [Using a client](#using-a-client)
+    - [Creating a Client](#creating-a-client)
+    - [Login into a Namespace](#login-into-a-namespace)
+    - [Connecting To Dgraph Cloud](#connecting-to-dgraph-cloud)
+    - [Altering the Database](#altering-the-database)
+    - [Creating a Transaction](#creating-a-transaction)
+    - [Running a Mutation](#running-a-mutation)
+    - [Running a Query](#running-a-query)
+    - [Query with RDF response](#query-with-rdf-response)
+    - [Running an Upsert: Query + Mutation](#running-an-upsert-query--mutation)
+    - [Running a Conditional Upsert](#running-a-conditional-upsert)
+    - [Committing a Transaction](#committing-a-transaction)
+    - [Cleaning Up Resources](#cleaning-up-resources)
+    - [Setting Metadata Headers](#setting-metadata-headers)
+    - [Setting a timeout](#setting-a-timeout)
+    - [Async methods](#async-methods)
+  - [Examples](#examples)
+  - [Development](#development)
+    - [Setting up environment](#setting-up-environment)
+    - [Build from source](#build-from-source)
+    - [Running tests](#running-tests)
+
+## Install
+
+Install using pip:
+
+```sh
+pip install pydgraph
+```
+
+## Supported Versions
+
+Depending on the version of Dgraph that you are connecting to, you will have to
+use a different version of this client.
+
+| Dgraph version |   pydgraph version   |
+|:--------------:|:--------------------:|
+|    20.3.X      |      *20.3.0*        |
+|    20.7.X      |      *20.7.0*        |
+|    20.11.X     |      *20.7.0*        |
+|    21.03.X     |      *21.3.0*        |
+|    22.0.X      |      *21.3.0*        |
+|    23.0.X      |      *23.0.0*        |
+
+## Quickstart
+
+Build and run the [simple project][simple] in the `examples` folder, which
+contains an end-to-end example of using the Dgraph python client. For additional details, follow the
+instructions in the project's [README](./examples/simple/README.md).
+
+[simple]: ./examples/simple
+
+## Using a client
+
+### Creating a Client
+
+You can initialize a `DgraphClient` object by passing it a list of
+`DgraphClientStub` clients as variadic arguments. Connecting to multiple Dgraph
+servers in the same cluster allows for better distribution of workload.
+
+The following code snippet shows just one connection.
+
+```python3
+import pydgraph
+
+client_stub = pydgraph.DgraphClientStub('localhost:9080')
+client = pydgraph.DgraphClient(client_stub)
+```
+
+### Login into a Namespace
+
+If your server has Access Control Lists enabled (Dgraph v1.1 or above), the client must be
+logged in for accessing data. Use `login` endpoint:
+
+Calling login will obtain and remember the access and refresh JWT tokens. All subsequent operations
+via the logged in client will send along the stored access token.
+
+```python3
+client.login("groot", "password")
+```
+
+If your server additionally has namespaces (Dgraph v21.03 or above), use the
+`login_into_namespace` API.
+
+```python3
+client.login_into_namespace("groot", "password", "123")
+```
+
+### Connecting To Dgraph Cloud
+
+If you want to connect to Dgraph running on [Dgraph Cloud](https://cloud.dgraph.io) instance, then
+get the gRPC endpoint of your cluster that you can find in the
+[Settings section](https://cloud.dgraph.io/_/settings) of Dgraph Cloud console and obtain a Client
+or Admin API key (created in the [API key tab](https://cloud.dgraph.io/_/settings?tab=api-keys)
+of the Setting section). Create the `client_stub` using the gRPC endpoint and the API key:
+
+```python3
+client_stub = pydgraph.DgraphClientStub.from_cloud(
+    "https://morning-glade.grpc.us-east-1.aws.cloud.dgraph.io:443", "<api-key>")
+client = pydgraph.DgraphClient(client_stub)
+```
+
+The `DgraphClientStub.from_slash_endpoint()` method has been removed v23.0.
+Please use `DgraphClientStub.from_cloud()` instead.
+
+### Altering the Database
+
+To set the schema, create an `Operation` object, set the schema and pass it to
+`DgraphClient#alter(Operation)` method.
+
+```python3
+schema = 'name: string @index(exact) .'
+op = pydgraph.Operation(schema=schema)
+client.alter(op)
+```
+
+`Operation` contains other fields as well, including `DropAttr` and `DropAll`. `DropAll` is
+useful if you wish to discard all the data, and start from a clean slate, without bringing
+the instance down. `DropAttr` is used to drop all the data related to a predicate.
+
+```python3
+# Drop all data including schema from the Dgraph instance. This is a useful
+# for small examples such as this since it puts Dgraph into a clean state.
+op = pydgraph.Operation(drop_all=True)
+client.alter(op)
+```
+
+Indexes can be computed in the background.
+You can set the `run_in_background` field of `pydgraph.Operation` to `True`
+before passing it to the `Alter` function. You can find more details
+[here](https://docs.dgraph.io/master/query-language/#indexes-in-background).
+
+```python3
+schema = 'name: string @index(exact) .'
+op = pydgraph.Operation(schema=schema, run_in_background=True)
+client.alter(op)
+```
+
+### Creating a Transaction
+
+To create a transaction, call the `DgraphClient#txn()` method, which returns a
+new `Txn` object. This operation incurs no network overhead.
+
+It is good practice to call `Txn#discard()` in a `finally` block after running
+the transaction. Calling `Txn#discard()` after `Txn#commit()` is a no-op
+and you can call `Txn#discard()` multiple times with no additional side-effects.
+
+```python3
+txn = client.txn()
+try:
+  # Do something here
+  # ...
+finally:
+  txn.discard()
+  # ...
+```
+
+To create a read-only transaction, call `DgraphClient#txn(read_only=True)`.
+Read-only transactions are ideal for transactions which only involve queries.
+Mutations and commits are not allowed.
+
+```python3
+txn = client.txn(read_only=True)
+try:
+  # Do some queries here
+  # ...
+finally:
+  txn.discard()
+  # ...
+```
+
+To create a read-only transaction that executes best-effort queries, call
+`DgraphClient#txn(read_only=True, best_effort=True)`. Best-effort queries are
+faster than normal queries because they bypass the normal consensus protocol.
+For this same reason, best-effort queries cannot guarantee to return the latest
+data. Best-effort queries are only supported by read-only transactions.
+
+### Running a Mutation
+
+`Txn#mutate(mu=Mutation)` runs a mutation. It takes in a `Mutation` object,
+which provides two main ways to set data: JSON and RDF N-Quad. You can choose
+whichever way is convenient.
+
+`Txn#mutate()` provides convenience keyword arguments `set_obj` and `del_obj`
+for setting JSON values and `set_nquads` and `del_nquads` for setting N-Quad
+values. See examples below for usage.
+
+We define a person object to represent a person and use it in a transaction.
+
+```python3
+# Create data.
+p = { 'name': 'Alice' }
+
+# Run mutation.
+txn.mutate(set_obj=p)
+
+# If you want to use a mutation object, use this instead:
+# mu = pydgraph.Mutation(set_json=json.dumps(p).encode('utf8'))
+# txn.mutate(mu)
+
+# If you want to use N-Quads, use this instead:
+# txn.mutate(set_nquads='_:alice <name> "Alice" .')
+```
+
+```python3
+# Delete data
+
+query = """query all($a: string)
+ {
+   all(func: eq(name, $a))
+    {
+      uid
+    }
+  }"""
+variables = {'$a': 'Bob'}
+
+res = txn.query(query, variables=variables)
+ppl = json.loads(res.json)
+
+# For a mutation to delete a node, use this:
+txn.mutate(del_obj=person)
+```
+
+For a complete example with multiple fields and relationships, look at the
+[simple project][simple] in the `examples` folder.
+
+Sometimes, you only want to commit a mutation, without querying anything further.
+In such cases, you can set the keyword argument `commit_now=True` to indicate
+that the mutation must be immediately committed.
+
+A mutation can be executed using `txn.do_request` as well.
+
+```python3
+mutation = txn.create_mutation(set_nquads='_:alice <name> "Alice" .')
+request = txn.create_request(mutations=[mutation], commit_now=True)
+txn.do_request(request)
+```
+
+### Running a Query
+
+You can run a query by calling `Txn#query(string)`. You will need to pass in a
+[DQL](https://dgraph.io/docs/query-language/) query string. If you want to pass
+an additional dictionary of any variables that you might want to set in the query,
+call `Txn#query(string, variables=d)` with the variables dictionary `d`.
+
+The query response contains the `json` field, which returns the JSON response.
+Let’s run a query with a variable `$a`, deserialize the result from JSON and
+print it out:
+
+```python3
+# Run query.
+query = """query all($a: string) {
+  all(func: eq(name, $a))
+  {
+    name
+  }
+}"""
+variables = {'$a': 'Alice'}
+
+res = txn.query(query, variables=variables)
+
+# If not doing a mutation in the same transaction, simply use:
+# res = client.txn(read_only=True).query(query, variables=variables)
+
+ppl = json.loads(res.json)
+
+# Print results.
+print('Number of people named "Alice": {}'.format(len(ppl['all'])))
+for person in ppl['all']:
+  print(person)
+```
+
+This should print:
+
+```console
+Number of people named "Alice": 1
+Alice
+```
+
+You can also use `txn.do_request` function to run the query.
+
+```python3
+request = txn.create_request(query=query)
+txn.do_request(request)
+```
+
+### Query with RDF response
+
+You can get query result as a RDF response by calling `Txn#query(string)` with `resp_format` set
+to `RDF`. The response would contain a `rdf` field, which has the RDF encoded result.
+
+**Note:** If you are querying only for `uid` values, use a JSON format response.
+
+```python3
+res = txn.query(query, variables=variables, resp_format="RDF")
+print(res.rdf)
+```
+
+### Running an Upsert: Query + Mutation
+
+The `txn.do_request` function allows you to use upsert blocks. An upsert block
+contains one query block and one or more mutation blocks, so it lets you perform
+queries and mutations in a single request. Variables defined in the query block
+can be used in the mutation blocks using the `uid` and `val` functions
+implemented by DQL.
+
+To learn more about upsert blocks, see the
+[Upsert Block documentation](https://dgraph.io/docs/mutations/upsert-block/).
+
+```python3
+query = """{
+  u as var(func: eq(name, "Alice"))
+}"""
+
+nquad = """
+  uid(u) <name> "Alice" .
+  uid(u) <age> "25" .
+"""
+
+mutation = txn.create_mutation(set_nquads=nquad)
+request = txn.create_request(query=query, mutations=[mutation], commit_now=True)
+txn.do_request(request)
+```
+
+### Running a Conditional Upsert
+
+The upsert block also allows specifying a conditional mutation block using an `@if` directive.
+The mutation is executed only when the specified condition is true. If the condition is false,
+the mutation is silently ignored.
+
+See more about Conditional Upserts [here](https://docs.dgraph.io/mutations/#conditional-upsert).
+
+```python3
+query = """
+  {
+    user as var(func: eq(email, "wrong_email@dgraph.io"))
+  }
+"""
+
+cond = "@if(eq(len(user), 1))"
+nquads = """
+  uid(user) <email> "correct_email@dgraph.io" .
+"""
+
+mutation = txn.create_mutation(cond=cond, set_nquads=nquads)
+request = txn.create_request(mutations=[mutation], query=query, commit_now=True)
+txn.do_request(request)
+```
+
+### Committing a Transaction
+
+A transaction can be committed using the `Txn#commit()` method. If your transaction
+consist solely of `Txn#query` or `Txn#queryWithVars` calls, and no calls to
+`Txn#mutate`, then calling `Txn#commit()` is not necessary.
+
+An error is raised if another transaction(s) modify the same data concurrently that was
+modified in the current transaction. It is up to the user to retry transactions
+when they fail.
+
+```python3
+txn = client.txn()
+try:
+  # ...
+  # Perform any number of queries and mutations
+  # ...
+  # and finally...
+  txn.commit()
+except pydgraph.AbortedError:
+  # Retry or handle exception.
+finally:
+  # Clean up. Calling this after txn.commit() is a no-op
+  # and hence safe.
+  txn.discard()
+```
+
+### Cleaning Up Resources
+
+To clean up resources, you have to call `DgraphClientStub#close()` individually for
+all the instances of `DgraphClientStub`.
+
+```python3
+SERVER_ADDR1 = "localhost:9080"
+SERVER_ADDR2 = "localhost:9080"
+
+# Create instances of DgraphClientStub.
+stub1 = pydgraph.DgraphClientStub(SERVER_ADDR1)
+stub2 = pydgraph.DgraphClientStub(SERVER_ADDR2)
+
+# Create an instance of DgraphClient.
+client = pydgraph.DgraphClient(stub1, stub2)
+
+# Use client
+...
+
+# Clean up resources by closing all client stubs.
+stub1.close()
+stub2.close()
+```
+
+### Setting Metadata Headers
+
+Metadata headers such as authentication tokens can be set through the metadata of gRPC methods.
+Below is an example of how to set a header named "auth-token".
+
+```python3
+# The following piece of code shows how one can set metadata with
+# auth-token, to allow Alter operation, if the server requires it.
+# metadata is a list of arbitrary key-value pairs.
+metadata = [("auth-token", "the-auth-token-value")]
+dg.alter(op, metadata=metadata)
+```
+
+### Setting a timeout
+
+A timeout value representing the number of seconds can be passed to the `login`,
+`alter`, `query`, and `mutate` methods using the `timeout` keyword argument.
+
+For example, the following alters the schema with a timeout of ten seconds:
+`dg.alter(op, timeout=10)`
+
+### Async methods
+
+The `alter` method in the client has an asynchronous version called
+`async_alter`. The async methods return a future. You can directly call the
+`result` method on the future. However. The DgraphClient class provides a static
+method `handle_alter_future` to handle any possible exception.
+
+```python3
+alter_future = self.client.async_alter(pydgraph.Operation(
+	schema="name: string @index(term) ."))
+response = pydgraph.DgraphClient.handle_alter_future(alter_future)
+```
+
+The `query` and `mutate` methods int the `Txn` class also have async versions
+called `async_query` and `async_mutation` respectively. These functions work
+just like `async_alter`.
+
+You can use the `handle_query_future` and `handle_mutate_future` static methods
+in the `Txn` class to retrieve the result. A short example is given below:
+
+```python3
+txn = client.txn()
+query = "query body here"
+future = txn.async_query()
+response = pydgraph.Txn.handle_query_future(future)
+```
+
+Keep in mind that due to the nature of async calls, the async functions cannot
+retry the request if the login is invalid. You will have to check for this error
+and retry the login (with the function `retry_login` in both the `Txn` and
+`Client` classes). A short example is given below:
+
+```python3
+client = DgraphClient(client_stubs) # client_stubs is a list of gRPC stubs.
+alter_future = client.async_alter()
+try:
+    response = alter_future.result()
+except Exception as e:
+	# You can use this function in the util package to check for JWT
+    # expired errors.
+    if pydgraph.util.is_jwt_expired(e):
+        # retry your request here.
+```
+
+## Examples
+
+[tls]: ./examples/tls
+[parse_datetime]: ./examples/parse_datetime
+
+- [simple][]: Quickstart example of using pydgraph.
+- [tls][]: Quickstart example that uses TLS.
+- [parse_datetime]: Demonstration of converting Dgraph's DateTime strings to native python datetime.
+
+## Development
+
+### Setting up environment
+
+There are many ways to set up your local Python environment. We suggest some sane defaults here.
+
+- Use [pyenv](https://github.com/pyenv/pyenv) to manage your Python installations.
+- Most recent versions of Python should work, but the version of Python officially supported is located in
+`.python-version`
+- Create a Python virtual environment using `python -m venv .venv`
+- Activate virtual environment via `source .venv/bin/activate`
+
+### Build from source
+
+To build and install pydgraph locally, run
+
+```sh
+pip install -e ".[dev]"
+```
+
+If you have made changes to the `pydgraph/proto/api.proto` file, you need need
+to regenerate the source files generated by Protocol Buffer tools. To do that,
+install the [grpcio-tools][grpcio-tools] library and then run the following
+command:
+
+[grpcio-tools]: https://pypi.python.org/pypi/grpcio-tools
+
+```sh
+python scripts/protogen.py
+```
+
+The generated file `api_pb2_grpc.py` needs to be changed in recent versions of python.
+The required change is outlined below as a diff.
+
+```diff
+-import api_pb2 as api__pb2
++from . import api_pb2 as api__pb2
+```
+
+### Running tests
+
+To run the tests in your local machine, run:
+
+```bash
+bash scripts/local-test.sh
+```
+
+This script assumes dgraph is located on your path. Dgraph release binaries can
+be found [here](https://github.com/dgraph-io/dgraph/releases).
+The test script also requires that `docker` and `docker compose` are installed on
+your machine.
+
+The script will take care of bringing up a Dgraph cluster and bringing it down
+after the tests are executed. The script connects to randomly selected ports for
+HTTP and gRPC requests to prevent interference with clusters running on the
+default port. Docker and docker-compose need to be installed before running the
+script. Refer to the official [Docker documentation](https://docs.docker.com/)
+for instructions on how to install those packages.
```

### Comparing `pydgraph-21.3.2/pydgraph/__init__.py` & `pydgraph-23.0.0/pydgraph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Dgraph Labs, Inc.
+# Copyright 2023 Dgraph Labs, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pydgraph-21.3.2/pydgraph/client.py` & `pydgraph-23.0.0/pydgraph/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2016 Dgraph Labs, Inc.
+# Copyright 2023 Dgraph Labs, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pydgraph-21.3.2/pydgraph/client_stub.py` & `pydgraph-23.0.0/pydgraph/client_stub.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Dgraph Labs, Inc.
+# Copyright 2023 Dgraph Labs, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -83,30 +83,29 @@
         try:
             self.channel.close()
         except:
             pass
         del self.channel
         del self.stub
 
-    # from_slash_endpoint is deprecated and will be removed in v21.07 release.
-    # Use from_cloud method to connect to dgraph cloud backend.
-    @staticmethod
-    def from_slash_endpoint(cloud_endpoint, api_key):
-        return from_cloud(cloud_endpoint, api_key)
-
+    # accepts grpc endpoint as copied in cloud console as well as graphql endpoint
     # Usage:
     # import pydgraph
     # client_stub = pydgraph.DgraphClientStub.from_cloud("cloud_endpoint", "api-key")
     # client = pydgraph.DgraphClient(client_stub)
     @staticmethod
     def from_cloud(cloud_endpoint, api_key):
-        """Returns Dgraph Client stub for the Slash GraphQL endpoint"""
-        url = urlparse(cloud_endpoint)
-        url_parts = url.netloc.split(".", 1)
-        host = url_parts[0] + ".grpc." + url_parts[1]
+        """Returns Dgraph Client stub for the Dgraph Cloud endpoint"""
+        if cloud_endpoint.startswith("http"): # catch http:// and https://
+            host = urlparse(cloud_endpoint).netloc
+        else:
+            host = cloud_endpoint.split(":",1)[0] # remove port if any
+        if not ".grpc." in host:
+            url_parts = host.split(".", 1)
+            host = url_parts[0] + ".grpc." + url_parts[1]
         creds = grpc.ssl_channel_credentials()
         call_credentials = grpc.metadata_call_credentials(
             lambda context, callback: callback((("authorization", api_key),), None))
         composite_credentials = grpc.composite_channel_credentials(
             creds, call_credentials)
         client_stub = DgraphClientStub('{host}:{port}'.format(
             host=host, port="443"), composite_credentials, options=(('grpc.enable_http_proxy', 0),))
```

### Comparing `pydgraph-21.3.2/pydgraph/errors.py` & `pydgraph-23.0.0/pydgraph/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Dgraph Labs, Inc.
+# Copyright 2023 Dgraph Labs, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -46,8 +46,7 @@
     def __str__(self):
         return str(self.exception)
 
 class TransactionError(Exception):
     """Error thrown when the transaction is invalid (e.g trying to mutate in read-only mode)."""
     def __init__(self, msg):
         super(TransactionError, self).__init__(msg)
-
```

### Comparing `pydgraph-21.3.2/pydgraph/meta.py` & `pydgraph-23.0.0/pydgraph/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Dgraph Labs, Inc.
+# Copyright 2023 Dgraph Labs, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Metadata about this package."""
 
-VERSION = '21.3.2'
+VERSION = '23.0.0'
```

### Comparing `pydgraph-21.3.2/pydgraph/txn.py` & `pydgraph-23.0.0/pydgraph/txn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Dgraph Labs, Inc.
+# Copyright 2023 Dgraph Labs, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `pydgraph-21.3.2/pydgraph/util.py` & `pydgraph-23.0.0/pydgraph/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Dgraph Labs, Inc.
+# Copyright 2023 Dgraph Labs, Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
```

