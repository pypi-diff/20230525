# Comparing `tmp/pulumi_pulumiservice-0.7.1a1684512888.tar.gz` & `tmp/pulumi_pulumiservice-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_pulumiservice-0.7.1a1684512888.tar", last modified: Fri May 19 16:18:25 2023, max compression
+gzip compressed data, was "pulumi_pulumiservice-0.7.2.tar", last modified: Thu May 25 17:14:18 2023, max compression
```

## Comparing `pulumi_pulumiservice-0.7.1a1684512888.tar` & `pulumi_pulumiservice-0.7.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    28475 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/config/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/deployment_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/org_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/stack_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team_stack_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:18:25.000000 pulumi_pulumiservice-0.7.1a1684512888/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-19 16:18:23.000000 pulumi_pulumiservice-0.7.1a1684512888/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:14:18.644098 pulumi_pulumiservice-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-25 17:14:18.644098 pulumi_pulumiservice-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:14:18.640098 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28475 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:14:18.644098 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/deployment_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/org_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/stack_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team_stack_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17290 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:14:18.640098 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:14:18.644098 pulumi_pulumiservice-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-25 17:14:18.000000 pulumi_pulumiservice-0.7.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/PKG-INFO` & `pulumi_pulumiservice-0.7.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,108 +1,110 @@
 Metadata-Version: 2.1
 Name: pulumi_pulumiservice
-Version: 0.7.1a1684512888
+Version: 0.7.2
 Summary: A native Pulumi package for creating and managing Pulumi Service constructs
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
-Description: # Pulumi Service Provider
-        
-        [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-        [![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
-        [![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
-        [![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
-        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
-        [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
-        
-        A Pulumi Resource Provider for The Pulumi Service.
-        
-        The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
-        
-        #### Supported Resources
-        
-        - [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
-        - [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
-          - You can grant a team access to stacks via the `TeamStackPermission` resource
-        - [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
-        - [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
-        
-        For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
-        
-        ## Installing
-        
-        This package is available in many languages in the standard packaging formats.
-        
-        ### Node.js (Java/TypeScript)
-        
-        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-        
-            $ npm install @pulumi/pulumiservice
-        
-        or `yarn`:
-        
-            $ yarn add @pulumi/pulumiservice
-        
-        ### Python
-        
-        To use from Python, install using `pip`:
-        
-            $ pip install pulumi_pulumiservice
-        
-        ### Go
-        
-        To use from Go, use `go get` to grab the latest version of the library
-        
-            $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
-        
-        ### .NET
-        
-        To use from .NET, install using `dotnet add package`:
-        
-            $ dotnet add package Pulumi.PulumiService
-        
-        ## Setup
-        
-        Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
-        
-        ### Configuration Options
-        
-        Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
-        
-        | Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
-        | ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-        | `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
-        | `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
-        
-        ## Examples
-        
-        ```typescript
-        import * as aws from "@pulumi/awsx"
-        import * as pulumi from "@pulumi/pulumi";
-        import * as service from "@pulumi/pulumiservice";
-        
-        const team = new service.Team("team", {
-            name: "pulumi-service-team",
-            displayName: "Pulumi Service",
-            description: "The Pulumi Service Team",
-            organizationName: "pulumi",
-            teamType: "pulumi",
-            members: [
-                "piers",
-                "bryce",
-                "casey"
-                "evan",
-                "devon",
-                "meagan"
-                "myles",
-                "steve"
-            ],
-        });
-        
-        export const members = team.members;
-        ```
-        
-        Check out the [examples/](examples/) directory for more examples.
-        
 Keywords: pulumi kind/native category/infrastructure
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# Pulumi Service Provider
+
+[![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+[![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
+[![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
+[![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
+[![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
+
+A Pulumi Resource Provider for The Pulumi Service.
+
+The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
+
+#### Supported Resources
+
+- [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
+- [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
+  - You can grant a team access to stacks via the `TeamStackPermission` resource
+- [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
+- [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
+
+For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
+
+## Installing
+
+This package is available in many languages in the standard packaging formats.
+
+### Node.js (Java/TypeScript)
+
+To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+
+    $ npm install @pulumi/pulumiservice
+
+or `yarn`:
+
+    $ yarn add @pulumi/pulumiservice
+
+### Python
+
+To use from Python, install using `pip`:
+
+    $ pip install pulumi_pulumiservice
+
+### Go
+
+To use from Go, use `go get` to grab the latest version of the library
+
+    $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
+
+### .NET
+
+To use from .NET, install using `dotnet add package`:
+
+    $ dotnet add package Pulumi.PulumiService
+
+## Setup
+
+Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
+
+### Configuration Options
+
+Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
+
+| Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
+| ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
+| `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
+
+## Examples
+
+```typescript
+import * as aws from "@pulumi/awsx"
+import * as pulumi from "@pulumi/pulumi";
+import * as service from "@pulumi/pulumiservice";
+
+const team = new service.Team("team", {
+    name: "pulumi-service-team",
+    displayName: "Pulumi Service",
+    description: "The Pulumi Service Team",
+    organizationName: "pulumi",
+    teamType: "pulumi",
+    members: [
+        "piers",
+        "bryce",
+        "casey"
+        "evan",
+        "devon",
+        "meagan"
+        "myles",
+        "steve"
+    ],
+});
+
+export const members = team.members;
+```
+
+Check out the [examples/](examples/) directory for more examples.
+
+
```

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/README.md` & `pulumi_pulumiservice-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/__init__.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_enums.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_inputs.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/_utilities.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/access_token.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/config/vars.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/deployment_settings.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/deployment_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,18 +142,18 @@
                  stack: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Deployment settings configure Pulumi Deployments for a stack.
 
         ### Import
 
-        Deployment settings can be imported using the `id`, which for deployment settings is {org}/{project}/{stack} e.g.,
+        Deployment settings can be imported using the `id`, which for deployment settings is `{org}/{project}/{stack}` e.g.,
 
         ```sh
-         $ pulumi import pulumiservice:index:DeploymentSettings my_settings `my-org/my-project/my-stack`
+         $ pulumi import pulumiservice:index:DeploymentSettings my_settings my-org/my-project/my-stack
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['DeploymentSettingsExecutorContextArgs']] executor_context: Settings related to the deployment executor.
         :param pulumi.Input[pulumi.InputType['DeploymentSettingsGithubArgs']] github: GitHub settings for the deployment.
         :param pulumi.Input[pulumi.InputType['DeploymentSettingsOperationContextArgs']] operation_context: Settings related to the Pulumi operation environment during the deployment.
@@ -169,18 +169,18 @@
                  args: DeploymentSettingsArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Deployment settings configure Pulumi Deployments for a stack.
 
         ### Import
 
-        Deployment settings can be imported using the `id`, which for deployment settings is {org}/{project}/{stack} e.g.,
+        Deployment settings can be imported using the `id`, which for deployment settings is `{org}/{project}/{stack}` e.g.,
 
         ```sh
-         $ pulumi import pulumiservice:index:DeploymentSettings my_settings `my-org/my-project/my-stack`
+         $ pulumi import pulumiservice:index:DeploymentSettings my_settings my-org/my-project/my-stack
         ```
 
         :param str resource_name: The name of the resource.
         :param DeploymentSettingsArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
```

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/org_access_token.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/org_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/provider.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/stack_tag.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/stack_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team_access_token.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/team_stack_permission.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/team_stack_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice/webhook.py` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/PKG-INFO` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,108 +1,110 @@
 Metadata-Version: 2.1
 Name: pulumi-pulumiservice
-Version: 0.7.1a1684512888
+Version: 0.7.2
 Summary: A native Pulumi package for creating and managing Pulumi Service constructs
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-pulumiservice
-Description: # Pulumi Service Provider
-        
-        [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-        [![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
-        [![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
-        [![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
-        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
-        [![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
-        
-        A Pulumi Resource Provider for The Pulumi Service.
-        
-        The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
-        
-        #### Supported Resources
-        
-        - [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
-        - [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
-          - You can grant a team access to stacks via the `TeamStackPermission` resource
-        - [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
-        - [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
-        
-        For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
-        
-        ## Installing
-        
-        This package is available in many languages in the standard packaging formats.
-        
-        ### Node.js (Java/TypeScript)
-        
-        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-        
-            $ npm install @pulumi/pulumiservice
-        
-        or `yarn`:
-        
-            $ yarn add @pulumi/pulumiservice
-        
-        ### Python
-        
-        To use from Python, install using `pip`:
-        
-            $ pip install pulumi_pulumiservice
-        
-        ### Go
-        
-        To use from Go, use `go get` to grab the latest version of the library
-        
-            $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
-        
-        ### .NET
-        
-        To use from .NET, install using `dotnet add package`:
-        
-            $ dotnet add package Pulumi.PulumiService
-        
-        ## Setup
-        
-        Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
-        
-        ### Configuration Options
-        
-        Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
-        
-        | Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
-        | ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-        | `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
-        | `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
-        
-        ## Examples
-        
-        ```typescript
-        import * as aws from "@pulumi/awsx"
-        import * as pulumi from "@pulumi/pulumi";
-        import * as service from "@pulumi/pulumiservice";
-        
-        const team = new service.Team("team", {
-            name: "pulumi-service-team",
-            displayName: "Pulumi Service",
-            description: "The Pulumi Service Team",
-            organizationName: "pulumi",
-            teamType: "pulumi",
-            members: [
-                "piers",
-                "bryce",
-                "casey"
-                "evan",
-                "devon",
-                "meagan"
-                "myles",
-                "steve"
-            ],
-        });
-        
-        export const members = team.members;
-        ```
-        
-        Check out the [examples/](examples/) directory for more examples.
-        
 Keywords: pulumi kind/native category/infrastructure
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# Pulumi Service Provider
+
+[![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+[![NPM version](https://badge.fury.io/js/%40pulumi%2Fpulumiservice.svg)](https://www.npmjs.com/package/@pulumi/pulumiservice)
+[![Python version](https://badge.fury.io/py/pulumi-pulumiservice.svg)](https://pypi.org/project/pulumi-pulumiservice)
+[![NuGet version](https://badge.fury.io/nu/pulumi.pulumiservice.svg)](https://badge.fury.io/nu/pulumi.pulumiservice)
+[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-pulumiservice/sdk/go/pulumiservice)](https://pkg.go.dev/github.com/pulumi/pulumi-pulumiservice/sdk/go)
+[![License](https://img.shields.io/npm/l/%40pulumi%2Fpulumiservice.svg)](https://github.com/pulumi/pulumi-pulumiservice/blob/main/LICENSE)
+
+A Pulumi Resource Provider for The Pulumi Service.
+
+The Pulumi Service Provider is built on top of the [Pulumi Service REST API](https://pulumi.com/docs/reference/service-rest-api) which is another feature available to our customers to programmatically configuring the Pulumi Service. The Pulumi Service REST API includes functionality to interact with and manipulate any kind of metadata managed by Pulumi. That includes Projects and Stacks, Previews and Updates, Organizations and Audit Logs. We have already seen Cloud Engineering teams using the Pulumi REST API to build all sorts of custom functionality. These new capabilities are especially powerful when used in combination with the [Automation API](https://pulumi.com/automation).
+
+#### Supported Resources
+
+- [Webhooks](https://pulumi.com/docs/intro/pulumi-service/webhooks)
+- [Teams](https://pulumi.com/docs/intro/pulumi-service/teams)
+  - You can grant a team access to stacks via the `TeamStackPermission` resource
+- [StackTags](https://pulumi.com/docs/reference/cli/pulumi_stack_tag)
+- [AccessTokens](https://pulumi.com/docs/intro/pulumi-service/accounts)
+
+For reference documentation, visit the [Pulumi Service API Documentation](https://www.pulumi.com/registry/packages/pulumiservice/api-docs/) on the [Pulumi Registry](https://www.pulumi.com/registry/packages/pulumiservice/)
+
+## Installing
+
+This package is available in many languages in the standard packaging formats.
+
+### Node.js (Java/TypeScript)
+
+To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+
+    $ npm install @pulumi/pulumiservice
+
+or `yarn`:
+
+    $ yarn add @pulumi/pulumiservice
+
+### Python
+
+To use from Python, install using `pip`:
+
+    $ pip install pulumi_pulumiservice
+
+### Go
+
+To use from Go, use `go get` to grab the latest version of the library
+
+    $ go get github.com/pulumi/pulumi-pulumiservice/sdk/go
+
+### .NET
+
+To use from .NET, install using `dotnet add package`:
+
+    $ dotnet add package Pulumi.PulumiService
+
+## Setup
+
+Ensure that you have ran `pulumi login`. Run `pulumi whoami` to verify that you are logged in.
+
+### Configuration Options
+
+Use `pulumi config set pulumiservice:<option>` or pass options to the [constructor of `new pulumiservice.Provider`](https://pulumi.com/registry/packages/pulumiservice/api-docs/provider).
+
+| Option        | Environment Variable Name | Required/Optional | Description                                                                                                                                                                              |
+| ------------- | ------------------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `accessToken` | `PULUMI_ACCESS_TOKEN`     | Optional          | Overrides [Pulumi Service Access Tokens](https://www.pulumi.com/docs/intro/pulumi-service/accounts/#access-tokens)                                                                       |
+| `apiUrl`      | `PULUMI_BACKEND_URL`      | Optional          | Allows overriding default [Pulumi Service API URL](https://www.pulumi.com/docs/reference/service-rest-api) for [self hosted customers](https://www.pulumi.com/docs/guides/self-hosted/). |
+
+## Examples
+
+```typescript
+import * as aws from "@pulumi/awsx"
+import * as pulumi from "@pulumi/pulumi";
+import * as service from "@pulumi/pulumiservice";
+
+const team = new service.Team("team", {
+    name: "pulumi-service-team",
+    displayName: "Pulumi Service",
+    description: "The Pulumi Service Team",
+    organizationName: "pulumi",
+    teamType: "pulumi",
+    members: [
+        "piers",
+        "bryce",
+        "casey"
+        "evan",
+        "devon",
+        "meagan"
+        "myles",
+        "steve"
+    ],
+});
+
+export const members = team.members;
+```
+
+Check out the [examples/](examples/) directory for more examples.
+
+
```

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/pulumi_pulumiservice.egg-info/SOURCES.txt` & `pulumi_pulumiservice-0.7.2/pulumi_pulumiservice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_pulumiservice-0.7.1a1684512888/setup.py` & `pulumi_pulumiservice-0.7.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.7.1a1684512888"
-PLUGIN_VERSION = "0.7.1-alpha.1684512888+4fa1a7d9"
+VERSION = "0.7.2"
+PLUGIN_VERSION = "0.7.2"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'pulumiservice', PLUGIN_VERSION])
         except OSError as error:
```

