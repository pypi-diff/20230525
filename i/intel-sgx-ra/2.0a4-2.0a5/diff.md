# Comparing `tmp/intel_sgx_ra-2.0a4.tar.gz` & `tmp/intel_sgx_ra-2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intel_sgx_ra-2.0a4.tar", last modified: Wed May 24 14:32:20 2023, max compression
+gzip compressed data, was "intel_sgx_ra-2.0a5.tar", last modified: Thu May 25 16:15:41 2023, max compression
```

## Comparing `intel_sgx_ra-2.0a4.tar` & `intel_sgx_ra-2.0a5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.190170 intel_sgx_ra-2.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-24 14:32:20.190170 intel_sgx_ra-2.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-24 14:32:20.190170 intel_sgx_ra-2.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.186170 intel_sgx_ra-2.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.186170 intel_sgx_ra-2.0a4/src/intel_sgx_ra/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/attest.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/base64url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.186170 intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/error.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/ratls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra/signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.186170 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 14:32:20.000000 intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 14:32:20.186170 intel_sgx_ra-2.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/tests/test_pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/tests/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-24 14:31:43.000000 intel_sgx_ra-2.0a4/tests/test_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.358536 intel_sgx_ra-2.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-25 16:15:41.358536 intel_sgx_ra-2.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-25 16:15:41.358536 intel_sgx_ra-2.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.354536 intel_sgx_ra-2.0a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.354536 intel_sgx_ra-2.0a5/src/intel_sgx_ra/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/attest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/base64url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.358536 intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/ratls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/signer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.354536 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.358536 intel_sgx_ra-2.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/tests/test_pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/tests/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/tests/test_regex.py
```

### Comparing `intel_sgx_ra-2.0a4/PKG-INFO` & `intel_sgx_ra-2.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel_sgx_ra
-Version: 2.0a4
+Version: 2.0a5
 Summary: Intel SGX Remote Attestation verification library
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intel_sgx_ra-2.0a4/README.md` & `intel_sgx_ra-2.0a5/README.md`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/setup.py` & `intel_sgx_ra-2.0a5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,15 +27,19 @@
     author_email="tech@cosmian.com",
     description="Intel SGX Remote Attestation verification library",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     zip_safe=False,
-    install_requires=["requests>=2.28.1,<3.0.0", "cryptography>=40.0.2,<40.1.0"],
+    install_requires=[
+        "requests>=2.28.1,<3.0.0",
+        "cryptography>=40.0.2,<40.1.0",
+        "sgx-pck-extension>=0.1.2,<0.2.0",
+    ],
     entry_points={
         "console_scripts": [
             "sgx-ra-verify = intel_sgx_ra.cli.verify:run",
             "sgx-ra-utils = intel_sgx_ra.cli.utils:run",
         ],
     },
     classifiers=[
```

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra/attest.py` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra/attest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """intel_ra_sgx.attest module."""
 
+import json
 import logging
 from datetime import datetime
 from hashlib import sha256
-from typing import Literal, Optional, Tuple, Union, cast
+from typing import Any, Dict, Literal, Optional, Tuple, Union, cast
 
 import cryptography.exceptions
 from cryptography import x509
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.hazmat.primitives.asymmetric.utils import encode_dss_signature
 from cryptography.hazmat.primitives.hashes import SHA256, HashAlgorithm
+from sgx_pck_extension import sgx_pck_extension_from_cert
 
 from intel_sgx_ra import globs
 from intel_sgx_ra.error import (
     CertificateError,
     CertificateRevokedError,
     CollateralsError,
     SGXDebugModeError,
     SGXVerificationError,
 )
-from intel_sgx_ra.pccs import get_pck_cert_crl, get_root_ca_crl
+from intel_sgx_ra.pccs import get_pck_cert_crl, get_root_ca_crl, get_tcbinfo
 from intel_sgx_ra.quote import Quote
 
 # define SGX_FLAGS_DEBUG 0x0000000000000002ULL
 SGX_FLAGS_DEBUG: int = 2
 
 
 def verify_pck_chain(
@@ -94,28 +96,85 @@
         raise exc
 
     logging.info("%s Certification chain", globs.OK)
 
     return True
 
 
+def verify_tcb(
+    tcb_info: bytes, tcb_cert: x509.Certificate, root_ca_cert: x509.Certificate
+) -> bool:
+    """Verify TCB information."""
+    now: datetime = datetime.utcnow()
+
+    tcb: Dict[str, Any] = json.loads(tcb_info)
+
+    assert tcb["tcbInfo"]["version"] == 3
+    assert tcb["tcbInfo"]["id"] == "SGX"
+    assert now < datetime.strptime(tcb["tcbInfo"]["nextUpdate"], "%Y-%m-%dT%H:%M:%SZ")
+
+    root_ca_pk = cast(ec.EllipticCurvePublicKey, root_ca_cert.public_key())
+
+    # Check issuers
+    root_ca_cert.verify_directly_issued_by(root_ca_cert)
+    tcb_cert.verify_directly_issued_by(root_ca_cert)
+
+    # Check expiration date of certificates
+    if not root_ca_cert.not_valid_before <= now <= root_ca_cert.not_valid_after:
+        raise CertificateError("Intel Root CA certificate has expired")
+    if not tcb_cert.not_valid_before <= now <= tcb_cert.not_valid_after:
+        raise CertificateError("Intel TCB certificate has expired")
+
+    try:
+        # 1) Check Intel Root CA is self-signed
+        root_ca_pk.verify(
+            root_ca_cert.signature,
+            root_ca_cert.tbs_certificate_bytes,
+            ec.ECDSA(cast(HashAlgorithm, root_ca_cert.signature_hash_algorithm)),
+        )
+        # 2) Check Intel Root CA signed Intel TCB certificate
+        root_ca_pk.verify(
+            tcb_cert.signature,
+            tcb_cert.tbs_certificate_bytes,
+            ec.ECDSA(cast(HashAlgorithm, tcb_cert.signature_hash_algorithm)),
+        )
+    except cryptography.exceptions.InvalidSignature as exc:
+        logging.info("%s TCB verification", globs.FAIL)
+        raise exc
+
+    logging.info("%s TCB verification", globs.OK)
+
+    return True
+
+
 def retrieve_collaterals(
-    pccs_url: str, ca: Literal["processor", "platform"]
-) -> Tuple[x509.CertificateRevocationList, x509.CertificateRevocationList]:
+    fmspc: bytes, pccs_url: str, ca: Literal["processor", "platform"]
+) -> Tuple[
+    bytes,
+    x509.Certificate,
+    x509.CertificateRevocationList,
+    x509.CertificateRevocationList,
+]:
     """Retrive collaterals from PCCS URL and PCK CA type."""
     root_ca_crl: x509.CertificateRevocationList = get_root_ca_crl(pccs_url)
     pck_ca_crl: x509.CertificateRevocationList = get_pck_cert_crl(pccs_url, ca)
+    tcb_info, tcb_cert = get_tcbinfo(pccs_url, fmspc)
 
-    return root_ca_crl, pck_ca_crl
+    return tcb_info, tcb_cert, root_ca_crl, pck_ca_crl
 
 
 def verify_quote(
     quote: Union[Quote, bytes],
     collaterals: Optional[
-        Tuple[x509.CertificateRevocationList, x509.CertificateRevocationList]
+        Tuple[
+            bytes,
+            x509.Certificate,
+            x509.CertificateRevocationList,
+            x509.CertificateRevocationList,
+        ]
     ] = None,
     pccs_url: Optional[str] = None,
 ):
     """Process DCAP remote attestation with `quote`."""
     quote = cast(Quote, Quote.from_bytes(quote) if isinstance(quote, bytes) else quote)
 
     # If set, then the enclave is in debug mode
@@ -126,34 +185,44 @@
     if debug:
         raise SGXDebugModeError
 
     pck_cert, pck_ca_cert, root_ca_cert = [
         x509.load_pem_x509_certificate(raw_cert) for raw_cert in quote.certs()
     ]  # type: x509.Certificate, x509.Certificate, x509.Certificate
 
+    sgx_pck_ext: Dict[str, Any] = sgx_pck_extension_from_cert(pck_cert)
+    fmspc: bytes = sgx_pck_ext["fmspc"]
+
+    tcb_info: bytes
+    tcb_cert: x509.Certificate
     root_ca_crl: x509.CertificateRevocationList
     pck_ca_crl: x509.CertificateRevocationList
     if pccs_url is not None:
         common_name, *_ = pck_ca_cert.subject.get_attributes_for_oid(
             x509.NameOID.COMMON_NAME
         )
         if common_name.value == "Intel SGX PCK Platform CA":
-            root_ca_crl, pck_ca_crl = retrieve_collaterals(pccs_url, "platform")
+            (tcb_info, tcb_cert, root_ca_crl, pck_ca_crl) = retrieve_collaterals(
+                fmspc, pccs_url, "platform"
+            )
         elif common_name.value == "Intel SGX PCK Processor CA":
-            root_ca_crl, pck_ca_crl = retrieve_collaterals(pccs_url, "processor")
+            (tcb_info, tcb_cert, root_ca_crl, pck_ca_crl) = retrieve_collaterals(
+                fmspc, pccs_url, "processor"
+            )
         else:
             raise CertificateError("Unknown CN in Intel SGX PCK Platform/Processor CA")
     elif collaterals is not None:
-        root_ca_crl, pck_ca_crl = collaterals
+        tcb_info, tcb_cert, root_ca_crl, pck_ca_crl = collaterals
     else:
         raise CollateralsError("Collaterals or PCCS URL missing")
 
     assert verify_pck_chain(
         root_ca_cert, pck_ca_cert, pck_cert, root_ca_crl, pck_ca_crl
     )
+    assert verify_tcb(tcb_info, tcb_cert, root_ca_cert)
 
     ecdsa_attestation_pk = ec.EllipticCurvePublicNumbers(
         curve=ec.SECP256R1(),
         x=int.from_bytes(quote.auth_data.public_key[:32], byteorder="big"),
         y=int.from_bytes(quote.auth_data.public_key[32:], byteorder="big"),
     ).public_key()
```

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra/base64url.py` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra/base64url.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/utils.py` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/utils.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra/cli/verify.py` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/verify.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra/error.py` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra/error.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra/pccs.py` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra/pccs.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,33 +69,34 @@
         params={"ca": ca, "encoding": "der"},
         timeout=30,
     )
 
     return load_der_x509_crl(response.content)
 
 
-def get_tcbinfo(
-    pccs_url: str, fmscp: str
-) -> Tuple[Tuple[Certificate, Certificate], Dict[str, Any]]:
+def get_tcbinfo(pccs_url: str, fmscp: bytes) -> Tuple[bytes, Certificate]:
     """Retrieve TCB info from `fmscp`."""
     response = requests.get(
-        url=f"{pccs_url}/sgx/certification/v4/tcb", params={"fmspc": fmscp}, timeout=30
+        url=f"{pccs_url}/sgx/certification/v4/tcb",
+        params={"fmspc": fmscp.hex()},
+        timeout=30,
     )
-    cert_chain = unquote(response.headers["SGX-TCB-Info-Issuer-Chain"])
-    tcb_cert, root_ca_cert, *others = [
+
+    cert_chain = unquote(response.headers["TCB-Info-Issuer-Chain"])
+    tcb_cert, _root_ca_cert, *others = [
         load_pem_x509_certificate(raw_cert)
         for raw_cert in re.findall(RE_CERT, cert_chain.encode("utf-8"))
     ]
 
     if others:
         raise PCCSResponseError(
-            "More than 2 certifices in header SGX-TCB-Info-Issuer-Chain"
+            "More than 2 certifices in header TCB-Info-Issuer-Chain"
         )
 
-    return (tcb_cert, root_ca_cert), response.json()
+    return response.content, tcb_cert
 
 
 def get_qe_identity(
     pccs_url: str,
 ) -> Tuple[Tuple[Certificate, Certificate], Dict[str, Any]]:
     """Retrieve Quoting Enclave Identity."""
     response = requests.get(
```

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra/quote.py` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra/quote.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra/ratls.py` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra/ratls.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra/signer.py` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra/signer.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/PKG-INFO` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel-sgx-ra
-Version: 2.0a4
+Version: 2.0a5
 Summary: Intel SGX Remote Attestation verification library
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intel_sgx_ra-2.0a4/src/intel_sgx_ra.egg-info/SOURCES.txt` & `intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/tests/test_pccs.py` & `intel_sgx_ra-2.0a5/tests/test_pccs.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/tests/test_quote.py` & `intel_sgx_ra-2.0a5/tests/test_quote.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a4/tests/test_regex.py` & `intel_sgx_ra-2.0a5/tests/test_regex.py`

 * *Files identical despite different names*

