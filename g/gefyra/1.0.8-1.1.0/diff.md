# Comparing `tmp/gefyra-1.0.8.tar.gz` & `tmp/gefyra-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gefyra-1.0.8.tar", max compression
+gzip compressed data, was "gefyra-1.1.0.tar", max compression
```

## Comparing `gefyra-1.0.8.tar` & `gefyra-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     2151 2023-05-03 18:49:11.805759 gefyra-1.0.8/README.md
--rw-r--r--   0        0        0        0 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/__init__.py
--rw-r--r--   0        0        0    13357 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/__main__.py
--rw-r--r--   0        0        0      169 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/api/__init__.py
--rw-r--r--   0        0        0     9037 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/api/bridge.py
--rw-r--r--   0        0        0     1306 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/api/down.py
--rw-r--r--   0        0        0     1605 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/api/list.py
--rw-r--r--   0        0        0     6142 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/api/run.py
--rw-r--r--   0        0        0     6277 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/api/status.py
--rw-r--r--   0        0        0     2917 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/api/up.py
--rw-r--r--   0        0        0     1264 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/api/utils.py
--rw-r--r--   0        0        0        0 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/cluster/__init__.py
--rw-r--r--   0        0        0     5507 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/cluster/manager.py
--rw-r--r--   0        0        0     8850 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/cluster/resources.py
--rw-r--r--   0        0        0     1608 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/cluster/utils.py
--rw-r--r--   0        0        0     8959 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/configuration.py
--rw-r--r--   0        0        0      260 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/local/__init__.py
--rw-r--r--   0        0        0     6677 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/local/bridge.py
--rw-r--r--   0        0        0     4609 2023-05-03 18:49:11.805759 gefyra-1.0.8/gefyra/local/cargo.py
--rw-r--r--   0        0        0        0 2023-05-03 18:49:11.809759 gefyra-1.0.8/gefyra/local/cargoimage/__init__.py
--rw-r--r--   0        0        0     1037 2023-05-03 18:49:11.809759 gefyra-1.0.8/gefyra/local/cargoimage/cargo_dockerfile.py
--rw-r--r--   0        0        0      945 2023-05-03 18:49:11.809759 gefyra-1.0.8/gefyra/local/check.py
--rw-r--r--   0        0        0     2150 2023-05-03 18:49:11.809759 gefyra-1.0.8/gefyra/local/minikube.py
--rw-r--r--   0        0        0     4300 2023-05-03 18:49:11.809759 gefyra-1.0.8/gefyra/local/networking.py
--rw-r--r--   0        0        0     3948 2023-05-03 18:49:11.809759 gefyra-1.0.8/gefyra/local/telemetry.py
--rw-r--r--   0        0        0     8109 2023-05-03 18:49:11.809759 gefyra-1.0.8/gefyra/local/utils.py
--rw-r--r--   0        0        0     1326 2023-05-03 18:49:11.809759 gefyra-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2151 2023-05-25 13:38:51.145910 gefyra-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/__init__.py
+-rw-r--r--   0        0        0    15368 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/__main__.py
+-rw-r--r--   0        0        0      200 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/__init__.py
+-rw-r--r--   0        0        0     9037 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/bridge.py
+-rw-r--r--   0        0        0     1306 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/down.py
+-rw-r--r--   0        0        0     1605 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/list.py
+-rw-r--r--   0        0        0     2523 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/reflect.py
+-rw-r--r--   0        0        0     6142 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/run.py
+-rw-r--r--   0        0        0     6277 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/status.py
+-rw-r--r--   0        0        0     2917 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/up.py
+-rw-r--r--   0        0        0     1562 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/api/utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/cluster/__init__.py
+-rw-r--r--   0        0        0     7090 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/cluster/manager.py
+-rw-r--r--   0        0        0     8850 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/cluster/resources.py
+-rw-r--r--   0        0        0     3016 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/cluster/utils.py
+-rw-r--r--   0        0        0     8959 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/configuration.py
+-rw-r--r--   0        0        0      260 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/__init__.py
+-rw-r--r--   0        0        0     6677 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/bridge.py
+-rw-r--r--   0        0        0     4609 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/cargo.py
+-rw-r--r--   0        0        0        0 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/cargoimage/__init__.py
+-rw-r--r--   0        0        0     1037 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/cargoimage/cargo_dockerfile.py
+-rw-r--r--   0        0        0     1121 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/check.py
+-rw-r--r--   0        0        0     2150 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/minikube.py
+-rw-r--r--   0        0        0     4300 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/networking.py
+-rw-r--r--   0        0        0     3948 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/telemetry.py
+-rw-r--r--   0        0        0     8109 2023-05-25 13:38:51.145910 gefyra-1.1.0/gefyra/local/utils.py
+-rw-r--r--   0        0        0     1326 2023-05-25 13:38:51.145910 gefyra-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3338 1970-01-01 00:00:00.000000 gefyra-1.1.0/PKG-INFO
```

### Comparing `gefyra-1.0.8/README.md` & `gefyra-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/__main__.py` & `gefyra-1.1.0/gefyra/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 parser = argparse.ArgumentParser(
     prog="gefyra",
     description="The Gefyra client. For more help please visit: https://gefyra.dev/reference/cli/",
 )
 action = parser.add_subparsers(dest="action", help="the action to be performed")
 parser.add_argument("-d", "--debug", action="store_true", help="add debug output")
 
+port_mapping_help_text = "Add port mapping in form of <container_port>:<host_port>"
+namespace_help_text = "The namespace for this container to run in"
 
 up_parser = action.add_parser("up")
 up_parser.add_argument(
     "-e",
     "--endpoint",
     dest="cargo_endpoint",
     help="the Wireguard endpoint in the form <IP>:<Port> for Gefyra to connect to",
@@ -104,14 +106,71 @@
 up_parser.add_argument(
     "--context",
     dest="kube_context",
     required=False,
     help="The context name from kubeconfig",
 )
 
+reflect_parser = action.add_parser("reflect")
+reflect_parser.add_argument(
+    "-w", "--workload", help="Workload to reflect locally", required=True
+)
+reflect_parser.add_argument(
+    "-e",
+    "--expose",
+    help="Exposes ports from k8s container spec to host",
+    required=False,
+    default=True,
+    action="store_false",
+)
+reflect_parser.add_argument(
+    "-i", "--image", help="The docker image to run in Gefyra", required=True
+)
+reflect_parser.add_argument(
+    "-v",
+    "--volume",
+    action="append",
+    help="Bind mount a volume into the container in notation src:dest, allowed multiple times",
+    required=False,
+)
+reflect_parser.add_argument(
+    "-p",
+    "--port",
+    help=port_mapping_help_text,
+    required=False,
+    action=PortMappingParser,
+)
+reflect_parser.add_argument(
+    "-b",
+    "--bridge",
+    help="Bridge workload and make local container accessible to k8s workloads",
+    required=False,
+    default=False,
+    action="store_true",
+)
+
+reflect_parser.add_argument(
+    "-c",
+    "--command",
+    help="The command for this container to in Gefyra",
+    nargs="+",
+    required=False,
+)
+reflect_parser.add_argument(
+    "-n",
+    "--namespace",
+    help=namespace_help_text,
+    default="default",
+)
+reflect_parser.add_argument(
+    "--env",
+    action="append",
+    help="Set or override environment variables in the form ENV=value, allowed multiple times",
+    required=False,
+)
 
 run_parser = action.add_parser("run")
 run_parser.add_argument(
     "-i", "--image", help="The docker image to run in Gefyra", required=True
 )
 run_parser.add_argument(
     "-N", "--name", help="The name of the container running in Gefyra", required=True
@@ -122,15 +181,15 @@
     help="The command for this container to in Gefyra",
     nargs="+",
     required=False,
 )
 run_parser.add_argument(
     "-n",
     "--namespace",
-    help="The namespace for this container to run in",
+    help=namespace_help_text,
 )
 run_parser.add_argument(
     "--env",
     action="append",
     help="Set or override environment variables in the form ENV=value, allowed multiple times",
     required=False,
 )
@@ -145,15 +204,15 @@
     "--env-from",
     help="Copy the environment from the container in the notation 'Pod/Container'",
     required=False,
 )
 run_parser.add_argument(
     "-p",
     "--expose",
-    help="Add port mapping in form of <container_port>:<host_port>",
+    help=port_mapping_help_text,
     required=False,
     action=IpPortMappingParser,
 )
 run_parser.add_argument(
     "--rm",
     help="Automatically remove the container when it exits",
     dest="auto_remove",
@@ -172,22 +231,22 @@
 bridge_parser = action.add_parser("bridge")
 bridge_parser.add_argument(
     "-N", "--name", help="The name of the container running in Gefyra", required=True
 )
 bridge_parser.add_argument(
     "-p",
     "--port",
-    help="Add port mapping in form of <container_port>:<host_port>",
+    help=port_mapping_help_text,
     required=True,
     action=PortMappingParser,
 )
 bridge_parser.add_argument(
     "-n",
     "--namespace",
-    help="The namespace for this container to run in",
+    help=namespace_help_text,
     default="default",
 )
 bridge_parser.add_argument(
     "-P",
     "--no-probe-handling",
     action="store_true",
     help="Make Carrier to not handle probes during switch operation",
@@ -338,35 +397,47 @@
     from gefyra.api import up
 
     success = up(config=configuration)
     if not success:
         raise RuntimeError("Failed to start Gefyra")
 
 
+def setup_logger(args, configuration_package):
+    if args.debug:
+        logger.setLevel(logging.DEBUG)
+    else:
+        logger.setLevel(logging.INFO)
+    logger.addHandler(configuration_package.console)
+
+
 def main():
     try:
         from gefyra import configuration as configuration_package
-        from gefyra.api import bridge, down, run, unbridge, unbridge_all, status
+        from gefyra.api import (
+            bridge,
+            down,
+            run,
+            unbridge,
+            unbridge_all,
+            status,
+            reflect,
+        )
         from gefyra.local.check import probe_kubernetes, probe_docker
 
         args = parser.parse_args()
-        if args.debug:
-            logger.setLevel(logging.DEBUG)
-        else:
-            logger.setLevel(logging.INFO)
-        logger.addHandler(configuration_package.console)
+
+        setup_logger(args, configuration_package)
+
+        configuration = get_client_configuration(args)
 
         if args.action == "version":
             check = not args.no_check
             version(configuration_package, check)
             exit(0)
-
-        configuration = get_client_configuration(args)
-
-        if args.action == "up":
+        elif args.action == "up":
             cli_up(configuration=configuration)
         elif args.action == "run":
             run(
                 image=args.image,
                 name=args.name,
                 command=" ".join(args.command) if args.command else None,
                 namespace=args.namespace,
@@ -374,14 +445,25 @@
                 env=args.env,
                 ports=args.expose,
                 auto_remove=args.auto_remove,
                 volumes=args.volume,
                 config=configuration,
                 detach=args.detach,
             )
+        elif args.action == "reflect":
+            reflect(
+                workload=args.workload,
+                expose_ports=args.expose,
+                volumes=args.volume,
+                command=args.command,
+                namespace=args.namespace,
+                do_bridge=args.bridge,
+                ports=args.port,
+                image=args.image,
+            )
         elif args.action == "bridge":
             bridge(
                 args.name,
                 args.port,
                 namespace=args.namespace,
                 handle_probes=not args.no_probe_handling,
                 config=configuration,
```

### Comparing `gefyra-1.0.8/gefyra/api/bridge.py` & `gefyra-1.1.0/gefyra/api/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/api/down.py` & `gefyra-1.1.0/gefyra/api/down.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/api/list.py` & `gefyra-1.1.0/gefyra/api/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/api/run.py` & `gefyra-1.1.0/gefyra/api/run.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/api/status.py` & `gefyra-1.1.0/gefyra/api/status.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/api/up.py` & `gefyra-1.1.0/gefyra/api/up.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/cluster/manager.py` & `gefyra-1.1.0/gefyra/cluster/manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,30 +21,90 @@
     create_operator_serviceaccount,
 )
 from .utils import decode_secret
 
 logger = logging.getLogger(__name__)
 
 
-def handle_serviceaccount(
-    config: ClientConfiguration, serviceaccount: V1ServiceAccount
-):
+def _handle_duplicate_namespace(config: ClientConfiguration):
+    active = False
     try:
-        config.K8S_CORE_API.create_namespaced_service_account(
-            body=serviceaccount, namespace=config.NAMESPACE
-        )
+        namespace = config.K8S_CORE_API.read_namespace(config.NAMESPACE)
     except ApiException as e:
-        if e.status == 409:
-            pass
-        elif e.status == 403:
-            raise RuntimeError(
-                f"You're not allowed to create a serviceaccount in namespace {config.NAMESPACE}."
-            )
+        if e.status == 404:
+            logger.warning(f"NS {config.NAMESPACE} after 409. Retrying.")
         else:
             raise e
+    if namespace.status.phase == "Active":
+        active = True
+    return active
+
+
+def handle_create_namespace(config: ClientConfiguration, retries=10, wait=3):
+    counter = 0
+    created = False
+    while counter < retries:
+        try:
+            config.K8S_CORE_API.create_namespace(
+                body=V1Namespace(
+                    metadata=V1ObjectMeta(
+                        name=config.NAMESPACE,
+                        labels={
+                            "pod-security.kubernetes.io/enforce": "privileged",
+                        },
+                    )
+                )
+            )
+            created = True
+            break
+        except ApiException as e:
+            if e.status == 409:
+                active = _handle_duplicate_namespace(config)
+                if active:
+                    created = True
+                    break
+            else:
+                raise e
+        logger.warning(f"Could not create namespace {config.NAMESPACE}. Retrying.")
+        counter += 1
+        time.sleep(wait)
+    if not created:
+        raise RuntimeError(
+            f"Could not create namespace. Retried {retries} times. API returned HTTP 409."
+        )
+
+
+def handle_serviceaccount(
+    config: ClientConfiguration, serviceaccount: V1ServiceAccount
+):
+    retries = 5
+    wait = 5
+    counter = 0
+    while counter < retries:
+        try:
+            config.K8S_CORE_API.create_namespaced_service_account(
+                body=serviceaccount, namespace=config.NAMESPACE
+            )
+            break
+        except ApiException as e:
+            if e.status == 409:
+                break
+            elif e.status == 403:
+                # this sometimes happens when to cluster in terminating the gefyra namespace
+                # due to a previous `gefyra down`. As long as it is terminating this error occurs.
+                if counter > retries:
+                    raise RuntimeError(
+                        f"You're not allowed to create a serviceaccount in namespace {config.NAMESPACE}."
+                    )
+                else:
+                    counter += 1
+                    time.sleep(wait)
+                    continue
+            else:
+                raise e
 
 
 def handle_clusterrole(config: ClientConfiguration, clusterrole: V1ClusterRole):
     try:
         config.K8S_RBAC_API.create_cluster_role(body=clusterrole)
     except ApiException as e:
         if e.status == 409:
@@ -84,31 +144,15 @@
     """
     Installs Gefyra Operator to the configured cluster, waits for the installation to complete and returns the
     connection secrets for Cargo
     :param config: a ClientConfiguration install
     :return: Cargo connection details
     """
     tic = time.perf_counter()
-    try:
-        config.K8S_CORE_API.create_namespace(
-            body=V1Namespace(
-                metadata=V1ObjectMeta(
-                    name=config.NAMESPACE,
-                    labels={
-                        "pod-security.kubernetes.io/enforce": "privileged",
-                    },
-                )
-            )
-        )
-    except ApiException as e:
-        if e.status == 409:
-            # namespace does already exist
-            pass
-        else:
-            raise e
+    handle_create_namespace(config=config)
 
     serviceaccount = create_operator_serviceaccount(config.NAMESPACE)
     clusterrole = create_operator_clusterrole()
     clusterrolebinding = create_operator_clusterrolebinding(
         serviceaccount, clusterrole, config.NAMESPACE
     )
     operator_deployment = create_operator_deployment(
```

### Comparing `gefyra-1.0.8/gefyra/cluster/resources.py` & `gefyra-1.1.0/gefyra/cluster/resources.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/configuration.py` & `gefyra-1.1.0/gefyra/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 console = logging.StreamHandler(sys.stdout)
 formatter = logging.Formatter("[%(levelname)s] %(message)s")
 console.setFormatter(formatter)
 
 logger = logging.getLogger("gefyra")
 logger.addHandler(console)
 
-__VERSION__ = "1.0.8"
+__VERSION__ = "1.1.0"
 
 
 def fix_pywin32_in_frozen_build() -> None:  # pragma: no cover
     import os
     import site
 
     if sys.platform != "win32" or not getattr(sys, "frozen", False):
```

### Comparing `gefyra-1.0.8/gefyra/local/bridge.py` & `gefyra-1.1.0/gefyra/local/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/local/cargo.py` & `gefyra-1.1.0/gefyra/local/cargo.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/local/cargoimage/cargo_dockerfile.py` & `gefyra-1.1.0/gefyra/local/cargoimage/cargo_dockerfile.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/local/check.py` & `gefyra-1.1.0/gefyra/local/check.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 
 from gefyra.configuration import default_configuration, ClientConfiguration
 
 logger = logging.getLogger("gefyra")
 
 
 def probe_docker(config: ClientConfiguration = default_configuration):
-    logger.debug("Probing: Docker")
+    logger.info("Checking Docker client.")
     try:
         config.DOCKER.containers.list()
+        logger.info("Docker client: Ok")
+        logger.info("Checking availability of Gefyra Cargo image...")
         config.DOCKER.images.pull("quay.io/gefyra/cargo:latest")
+        logger.info("Gefyra Cargo: Available")
     except Exception:
         logger.error("Docker does not seem to be not working for Gefyra")
         return False
     else:
         logger.info("Docker: Ok")
         return True
 
 
 def probe_kubernetes(config: ClientConfiguration = default_configuration):
-    logger.debug("Probing: Kubernetes")
+    logger.info("Checking Kubernetes connection.")
     try:
         config.K8S_CORE_API.list_namespace()
     except Exception:
         logger.error(
             "Kubernetes is not connected to a cluster or does not seem to be working for Gefyra"
         )
         return False
```

### Comparing `gefyra-1.0.8/gefyra/local/minikube.py` & `gefyra-1.1.0/gefyra/local/minikube.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/local/networking.py` & `gefyra-1.1.0/gefyra/local/networking.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/local/telemetry.py` & `gefyra-1.1.0/gefyra/local/telemetry.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/gefyra/local/utils.py` & `gefyra-1.1.0/gefyra/local/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-1.0.8/pyproject.toml` & `gefyra-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Gefyra"
-version = "1.0.8"
+version = "1.1.0"
 description = "Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure"
 authors = ["Michael Schilonka <michael@unikube.io>"]
 readme = "README.md"
 homepage = "https://gefyra.dev"
 repository = "https://github.com/gefyrahq/gefyra"
 documentation = "https://gefyra.dev"
 keywords = [
```

### Comparing `gefyra-1.0.8/PKG-INFO` & `gefyra-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gefyra
-Version: 1.0.8
+Version: 1.1.0
 Summary: Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure
 Home-page: https://gefyra.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@unikube.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

