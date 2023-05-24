# Comparing `tmp/netius-1.9.8.tar.gz` & `tmp/netius-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/netius-1.9.8.tar", last modified: Sat Aug 13 00:09:56 2016, max compression
+gzip compressed data, was "dist/netius-1.9.9.tar", last modified: Sat Aug 13 00:19:24 2016, max compression
```

## Comparing `netius-1.9.8.tar` & `netius-1.9.9.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/adapters/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1460 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/adapters/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3259 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/adapters/base.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3943 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/adapters/fs.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3348 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/adapters/memory.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1452 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/adapters/mongo.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1359 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/adapters/null.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/auth/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1615 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/auth/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2138 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/auth/address.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1484 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/auth/allow.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     6613 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/auth/base.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1484 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/auth/deny.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1801 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/auth/dummy.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2251 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/auth/memory.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2765 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/auth/passwd.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2008 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/auth/simple.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/base/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/base/extras/
--rw-rw-r--   0 travis    (1000) travis    (1000)      424 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/extras/dh.pem
--rw-rw-r--   0 travis    (1000) travis    (1000)   250607 2016-08-13 00:09:49.000000 netius-1.9.8/src/netius/base/extras/net.ca
--rw-rw-r--   0 travis    (1000) travis    (1000)      989 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/extras/net.cer
--rw-rw-r--   0 travis    (1000) travis    (1000)      720 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/extras/net.csr
--rw-rw-r--   0 travis    (1000) travis    (1000)      887 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/extras/net.key
--rw-rw-r--   0 travis    (1000) travis    (1000)      272 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/extras/net.pub
--rw-rw-r--   0 travis    (1000) travis    (1000)     2433 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3730 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/async.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2010 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/async_neo.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    37668 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/client.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    85106 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/common.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     7404 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/config.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    30690 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/conn.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     7688 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/container.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2652 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/diag.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3808 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/errors.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    11136 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/legacy.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2865 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/log.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2838 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/observer.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    17342 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/poll.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2913 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/request.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    37142 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/server.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2750 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/stream.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3330 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/base/tls.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/clients/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1857 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     7282 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/apn.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5413 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/dht.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    12055 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/dns.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    34923 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/http.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4852 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/mjpg.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2243 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/raw.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    20303 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/smtp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3746 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/ssdp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     9214 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/torrent.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     8515 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/clients/ws.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/common/
--rw-rw-r--   0 travis    (1000) travis    (1000)     3975 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     7521 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/asn.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    10328 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/calc.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5268 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/dhcp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     6811 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/dkim.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5600 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/ftp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4989 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/geo.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    33217 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/http.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    48697 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/http2.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     8369 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/mime.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2379 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/parser.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4720 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/pop.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    14790 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/rsa.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2145 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/setup.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5603 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/smtp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    10057 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/socks.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     9128 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/stream.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2567 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/structures.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1518 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/tftp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2895 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/tls.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    11668 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/torrent.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    12286 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/util.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     6867 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/common/ws.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/examples/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1316 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/examples/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1748 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/examples/http.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3790 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/examples/upnp.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/extra/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/extra/extras/
--rw-rw-r--   0 travis    (1000) travis    (1000)       19 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/extras/htpasswd
--rw-rw-r--   0 travis    (1000) travis    (1000)     1686 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1804 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/desktop.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4128 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/dhcp_s.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    18262 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/file.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3478 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/filea.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3090 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/hello.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1744 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/hello_w.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4002 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/proxy_f.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    20975 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/proxy_r.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     7846 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/extra/smtp_r.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/mock/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1222 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/mock/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1430 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/mock/appier.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/pool/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1438 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/pool/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     7572 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/pool/common.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3397 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/pool/file.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1935 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/pool/task.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/servers/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/servers/extras/
--rw-rw-r--   0 travis    (1000) travis    (1000)    11271 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/extras/boy_0.jpg
--rw-rw-r--   0 travis    (1000) travis    (1000)    11096 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/extras/boy_1.jpg
--rw-rw-r--   0 travis    (1000) travis    (1000)     2138 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    12498 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/dhcp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1565 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/echo.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    18527 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/ftp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    26853 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/http.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    41577 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/http2.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4170 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/mjpg.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    12706 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/pop.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    23141 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/proxy.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    16621 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/smtp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     8619 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/socks.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     8066 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/tftp.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    34626 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/torrent.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     7997 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/ws.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    18665 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/servers/wsgi.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/sh/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1279 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/sh/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1436 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/sh/auth.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1533 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/sh/base.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2100 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/sh/dkim.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1886 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/sh/rsa.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1924 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/sh/smtp.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius/test/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1198 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/test/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1333 2016-08-13 00:09:37.000000 netius-1.9.8/src/netius/__init__.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)      925 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)     3390 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-08-13 00:09:49.000000 netius-1.9.8/src/netius.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (1000) travis    (1000)        7 2016-08-13 00:09:56.000000 netius-1.9.8/src/netius.egg-info/top_level.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      108 2016-08-13 00:09:37.000000 netius-1.9.8/MANIFEST.in
--rw-rw-r--   0 travis    (1000) travis    (1000)     1459 2016-08-13 00:09:37.000000 netius-1.9.8/README.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)     3175 2016-08-13 00:09:37.000000 netius-1.9.8/setup.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      925 2016-08-13 00:09:56.000000 netius-1.9.8/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)       88 2016-08-13 00:09:56.000000 netius-1.9.8/setup.cfg
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/adapters/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1460 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/adapters/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3259 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/adapters/base.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3943 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/adapters/fs.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3348 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/adapters/memory.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1452 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/adapters/mongo.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1359 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/adapters/null.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/auth/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1615 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/auth/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2138 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/auth/address.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1484 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/auth/allow.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     6613 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/auth/base.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1484 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/auth/deny.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1801 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/auth/dummy.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2251 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/auth/memory.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2765 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/auth/passwd.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2008 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/auth/simple.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/base/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/base/extras/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      424 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/extras/dh.pem
+-rw-rw-r--   0 travis    (1000) travis    (1000)   250607 2016-08-13 00:19:17.000000 netius-1.9.9/src/netius/base/extras/net.ca
+-rw-rw-r--   0 travis    (1000) travis    (1000)      989 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/extras/net.cer
+-rw-rw-r--   0 travis    (1000) travis    (1000)      720 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/extras/net.csr
+-rw-rw-r--   0 travis    (1000) travis    (1000)      887 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/extras/net.key
+-rw-rw-r--   0 travis    (1000) travis    (1000)      272 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/extras/net.pub
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2433 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3730 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/async.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2010 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/async_neo.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    37668 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/client.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    85106 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/common.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     7404 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/config.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    30690 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/conn.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     7688 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/container.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2652 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/diag.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3808 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/errors.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    11136 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/legacy.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2865 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/log.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2838 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/observer.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    17342 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/poll.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2913 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/request.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    37142 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/server.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2750 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/stream.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3330 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/base/tls.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/clients/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1857 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     7282 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/apn.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5413 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/dht.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    12055 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/dns.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    34923 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/http.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4852 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/mjpg.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2243 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/raw.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    20303 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/smtp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3746 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/ssdp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     9214 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/torrent.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     8515 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/clients/ws.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/common/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3975 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     7521 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/asn.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    10328 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/calc.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5268 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/dhcp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     6811 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/dkim.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5600 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/ftp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4989 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/geo.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    33217 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/http.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    48701 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/http2.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     8369 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/mime.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2379 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/parser.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4720 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/pop.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    14790 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/rsa.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2145 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/setup.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5603 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/smtp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    10057 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/socks.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     9128 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/stream.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2567 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/structures.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1518 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/tftp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2895 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/tls.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    11668 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/torrent.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    12286 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/util.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     6867 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/common/ws.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/examples/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1316 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/examples/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1748 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/examples/http.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3790 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/examples/upnp.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/extra/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/extra/extras/
+-rw-rw-r--   0 travis    (1000) travis    (1000)       19 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/extras/htpasswd
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1686 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1804 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/desktop.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4128 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/dhcp_s.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    18262 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/file.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3478 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/filea.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3090 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/hello.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1744 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/hello_w.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4002 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/proxy_f.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    20975 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/proxy_r.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     7846 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/extra/smtp_r.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/mock/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1222 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/mock/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1430 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/mock/appier.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/pool/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1438 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/pool/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     7572 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/pool/common.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3397 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/pool/file.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1935 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/pool/task.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/servers/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/servers/extras/
+-rw-rw-r--   0 travis    (1000) travis    (1000)    11271 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/extras/boy_0.jpg
+-rw-rw-r--   0 travis    (1000) travis    (1000)    11096 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/extras/boy_1.jpg
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2138 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    12498 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/dhcp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1565 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/echo.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    18527 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/ftp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    26853 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/http.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    41205 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/http2.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4170 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/mjpg.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    12706 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/pop.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    23141 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/proxy.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    16621 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/smtp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     8619 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/socks.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     8066 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/tftp.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    34626 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/torrent.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     7997 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/ws.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    18665 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/servers/wsgi.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/sh/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1279 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/sh/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1436 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/sh/auth.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1533 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/sh/base.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2100 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/sh/dkim.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1886 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/sh/rsa.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1924 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/sh/smtp.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius/test/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1198 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/test/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1333 2016-08-13 00:19:07.000000 netius-1.9.9/src/netius/__init__.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius.egg-info/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      925 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3390 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-08-13 00:19:17.000000 netius-1.9.9/src/netius.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (1000) travis    (1000)        7 2016-08-13 00:19:24.000000 netius-1.9.9/src/netius.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)      108 2016-08-13 00:19:07.000000 netius-1.9.9/MANIFEST.in
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1459 2016-08-13 00:19:07.000000 netius-1.9.9/README.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3175 2016-08-13 00:19:07.000000 netius-1.9.9/setup.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      925 2016-08-13 00:19:24.000000 netius-1.9.9/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)       88 2016-08-13 00:19:24.000000 netius-1.9.9/setup.cfg
```

### Comparing `netius-1.9.8/src/netius/adapters/__init__.py` & `netius-1.9.9/src/netius/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/adapters/base.py` & `netius-1.9.9/src/netius/adapters/base.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/adapters/fs.py` & `netius-1.9.9/src/netius/adapters/fs.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/adapters/memory.py` & `netius-1.9.9/src/netius/adapters/memory.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/adapters/mongo.py` & `netius-1.9.9/src/netius/adapters/mongo.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/adapters/null.py` & `netius-1.9.9/src/netius/adapters/null.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/auth/__init__.py` & `netius-1.9.9/src/netius/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/auth/address.py` & `netius-1.9.9/src/netius/auth/address.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/auth/allow.py` & `netius-1.9.9/src/netius/auth/allow.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/auth/base.py` & `netius-1.9.9/src/netius/auth/base.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/auth/deny.py` & `netius-1.9.9/src/netius/auth/deny.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/auth/dummy.py` & `netius-1.9.9/src/netius/auth/dummy.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/auth/memory.py` & `netius-1.9.9/src/netius/auth/memory.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/auth/passwd.py` & `netius-1.9.9/src/netius/auth/passwd.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/auth/simple.py` & `netius-1.9.9/src/netius/auth/simple.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/extras/net.ca` & `netius-1.9.9/src/netius/base/extras/net.ca`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/extras/net.cer` & `netius-1.9.9/src/netius/base/extras/net.cer`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/extras/net.csr` & `netius-1.9.9/src/netius/base/extras/net.csr`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/extras/net.key` & `netius-1.9.9/src/netius/base/extras/net.key`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/__init__.py` & `netius-1.9.9/src/netius/base/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/async.py` & `netius-1.9.9/src/netius/base/async.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/async_neo.py` & `netius-1.9.9/src/netius/base/async_neo.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/client.py` & `netius-1.9.9/src/netius/base/client.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/common.py` & `netius-1.9.9/src/netius/base/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 from .async import * #@UnusedWildImport
 
 NAME = "netius"
 """ The global infra-structure name to be used in the
 identification of both the clients and the services this
 value may be prefixed or suffixed """
 
-VERSION = "1.9.8"
+VERSION = "1.9.9"
 """ The version value that identifies the version of the
 current infra-structure, all of the services and clients
 may share this value """
 
 PLATFORM = "%s %d.%d.%d.%s %s" % (
     sys.subversion[0] if hasattr(sys, "subversion") else "CPython",
     sys.version_info[0],
```

### Comparing `netius-1.9.8/src/netius/base/config.py` & `netius-1.9.9/src/netius/base/config.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/conn.py` & `netius-1.9.9/src/netius/base/conn.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/container.py` & `netius-1.9.9/src/netius/base/container.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/diag.py` & `netius-1.9.9/src/netius/base/diag.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/errors.py` & `netius-1.9.9/src/netius/base/errors.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/legacy.py` & `netius-1.9.9/src/netius/base/legacy.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/log.py` & `netius-1.9.9/src/netius/base/log.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/observer.py` & `netius-1.9.9/src/netius/base/observer.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/poll.py` & `netius-1.9.9/src/netius/base/poll.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/request.py` & `netius-1.9.9/src/netius/base/request.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/server.py` & `netius-1.9.9/src/netius/base/server.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/stream.py` & `netius-1.9.9/src/netius/base/stream.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/base/tls.py` & `netius-1.9.9/src/netius/base/tls.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/__init__.py` & `netius-1.9.9/src/netius/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/apn.py` & `netius-1.9.9/src/netius/clients/apn.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/dht.py` & `netius-1.9.9/src/netius/clients/dht.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/dns.py` & `netius-1.9.9/src/netius/clients/dns.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/http.py` & `netius-1.9.9/src/netius/clients/http.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/mjpg.py` & `netius-1.9.9/src/netius/clients/mjpg.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/raw.py` & `netius-1.9.9/src/netius/clients/raw.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/smtp.py` & `netius-1.9.9/src/netius/clients/smtp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/ssdp.py` & `netius-1.9.9/src/netius/clients/ssdp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/torrent.py` & `netius-1.9.9/src/netius/clients/torrent.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/clients/ws.py` & `netius-1.9.9/src/netius/clients/ws.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/__init__.py` & `netius-1.9.9/src/netius/common/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/asn.py` & `netius-1.9.9/src/netius/common/asn.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/calc.py` & `netius-1.9.9/src/netius/common/calc.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/dhcp.py` & `netius-1.9.9/src/netius/common/dhcp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/dkim.py` & `netius-1.9.9/src/netius/common/dkim.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/ftp.py` & `netius-1.9.9/src/netius/common/ftp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/geo.py` & `netius-1.9.9/src/netius/common/geo.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/http.py` & `netius-1.9.9/src/netius/common/http.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/http2.py` & `netius-1.9.9/src/netius/common/http2.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,16 +643,16 @@
         # going to be used as the basis for the header decoding
         fragment = data[index:data_l - padded_l]
 
         # retrieves the value of the window initial size from the owner
         # connections this is the value to be set in the new stream
         # and then retrieves the (maximum) frame size allowed to be passed
         # to the new stream instance for proper data frame fragmentation
-        window = self.owner.settings[SETTINGS_INITIAL_WINDOW_SIZE]
-        frame_size = self.owner.settings[SETTINGS_MAX_FRAME_SIZE]
+        window = self.owner.settings_r[SETTINGS_INITIAL_WINDOW_SIZE]
+        frame_size = self.owner.settings_r[SETTINGS_MAX_FRAME_SIZE]
 
         # tries to retrieve a previously opened stream and, this may be
         # the case it has been opened by a previous frame operation
         stream = self._get_stream(self.stream, strict = False, closed_s = True)
 
         if stream:
             # runs the headers assertion operation and then updated the
```

### Comparing `netius-1.9.8/src/netius/common/mime.py` & `netius-1.9.9/src/netius/common/mime.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/parser.py` & `netius-1.9.9/src/netius/common/parser.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/pop.py` & `netius-1.9.9/src/netius/common/pop.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/rsa.py` & `netius-1.9.9/src/netius/common/rsa.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/setup.py` & `netius-1.9.9/src/netius/common/setup.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/smtp.py` & `netius-1.9.9/src/netius/common/smtp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/socks.py` & `netius-1.9.9/src/netius/common/socks.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/stream.py` & `netius-1.9.9/src/netius/common/stream.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/structures.py` & `netius-1.9.9/src/netius/common/structures.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/tftp.py` & `netius-1.9.9/src/netius/common/tftp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/tls.py` & `netius-1.9.9/src/netius/common/tls.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/torrent.py` & `netius-1.9.9/src/netius/common/torrent.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/util.py` & `netius-1.9.9/src/netius/common/util.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/common/ws.py` & `netius-1.9.9/src/netius/common/ws.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/examples/__init__.py` & `netius-1.9.9/src/netius/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/examples/http.py` & `netius-1.9.9/src/netius/examples/http.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/examples/upnp.py` & `netius-1.9.9/src/netius/examples/upnp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/extra/__init__.py` & `netius-1.9.9/src/netius/extra/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/extra/desktop.py` & `netius-1.9.9/src/netius/extra/desktop.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/extra/dhcp_s.py` & `netius-1.9.9/src/netius/extra/dhcp_s.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/extra/file.py` & `netius-1.9.9/src/netius/extra/file.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/extra/filea.py` & `netius-1.9.9/src/netius/extra/filea.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/extra/hello.py` & `netius-1.9.9/src/netius/extra/hello.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/extra/hello_w.py` & `netius-1.9.9/src/netius/extra/hello_w.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/extra/proxy_f.py` & `netius-1.9.9/src/netius/extra/proxy_f.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/extra/proxy_r.py` & `netius-1.9.9/src/netius/extra/proxy_r.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/extra/smtp_r.py` & `netius-1.9.9/src/netius/extra/smtp_r.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/mock/__init__.py` & `netius-1.9.9/src/netius/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/mock/appier.py` & `netius-1.9.9/src/netius/mock/appier.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/pool/__init__.py` & `netius-1.9.9/src/netius/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/pool/common.py` & `netius-1.9.9/src/netius/pool/common.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/pool/file.py` & `netius-1.9.9/src/netius/pool/file.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/pool/task.py` & `netius-1.9.9/src/netius/pool/task.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/extras/boy_0.jpg` & `netius-1.9.9/src/netius/servers/extras/boy_0.jpg`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/extras/boy_1.jpg` & `netius-1.9.9/src/netius/servers/extras/boy_1.jpg`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/__init__.py` & `netius-1.9.9/src/netius/servers/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/dhcp.py` & `netius-1.9.9/src/netius/servers/dhcp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/echo.py` & `netius-1.9.9/src/netius/servers/echo.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/ftp.py` & `netius-1.9.9/src/netius/servers/ftp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/http.py` & `netius-1.9.9/src/netius/servers/http.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/http2.py` & `netius-1.9.9/src/netius/servers/http2.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,18 +55,20 @@
         **kwargs
     ):
         http.HTTPConnection.__init__(self, *args, **kwargs)
         self.legacy = legacy
         self.settings = dict(settings)
         self.settings_r = dict(settings_r)
         self.window = window
+        self.window_o = self.settings[netius.common.http2.SETTINGS_INITIAL_WINDOW_SIZE]
+        self.window_l = self.window_o
+        self.window_t = self.window_o // 2
         self.preface = False
         self.preface_b = b""
         self.frames = []
-        self._build_windows()
 
     def open(self, *args, **kwargs):
         http.HTTPConnection.open(self, *args, **kwargs)
         if not self.legacy: self.set_h2()
 
     def set_h2(self):
         self.legacy = False
@@ -878,28 +880,14 @@
     @property
     def parser_ctx(self):
         if self.legacy: return super(HTTP2Connection, self).parser_ctx
         if not self.parser: return None
         if not self.parser.stream_o: return self.parser
         return self.parser.stream_o
 
-    def _build_windows(self):
-        """
-        Builds the various values to be used as part of the
-        output stream flow window management.
-
-        This operation should be performed whenever the remote
-        settings are updated as the initial window size value
-        for the remote peer may change.
-        """
-
-        self.window_o = self.settings_r[netius.common.http2.SETTINGS_INITIAL_WINDOW_SIZE]
-        self.window_l = self.window_o
-        self.window_t = self.window_o // 2
-
     def _build_c(self, callback, stream, data_l):
         stream = self.parser._get_stream(stream, strict = False)
         if not stream: return callback
 
         stream.pending_s += data_l
         old_callback = callback
```

### Comparing `netius-1.9.8/src/netius/servers/mjpg.py` & `netius-1.9.9/src/netius/servers/mjpg.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/pop.py` & `netius-1.9.9/src/netius/servers/pop.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/proxy.py` & `netius-1.9.9/src/netius/servers/proxy.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/smtp.py` & `netius-1.9.9/src/netius/servers/smtp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/socks.py` & `netius-1.9.9/src/netius/servers/socks.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/tftp.py` & `netius-1.9.9/src/netius/servers/tftp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/torrent.py` & `netius-1.9.9/src/netius/servers/torrent.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/ws.py` & `netius-1.9.9/src/netius/servers/ws.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/servers/wsgi.py` & `netius-1.9.9/src/netius/servers/wsgi.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/sh/__init__.py` & `netius-1.9.9/src/netius/sh/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/sh/auth.py` & `netius-1.9.9/src/netius/sh/auth.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/sh/base.py` & `netius-1.9.9/src/netius/sh/base.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/sh/dkim.py` & `netius-1.9.9/src/netius/sh/dkim.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/sh/rsa.py` & `netius-1.9.9/src/netius/sh/rsa.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/sh/smtp.py` & `netius-1.9.9/src/netius/sh/smtp.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/test/__init__.py` & `netius-1.9.9/src/netius/test/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius/__init__.py` & `netius-1.9.9/src/netius/__init__.py`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/src/netius.egg-info/PKG-INFO` & `netius-1.9.9/src/netius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: netius
-Version: 1.9.8
+Version: 1.9.9
 Summary: Netius System
 Home-page: http://netius.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: netius net infrastructure wsgi
```

### Comparing `netius-1.9.8/src/netius.egg-info/SOURCES.txt` & `netius-1.9.9/src/netius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/README.rst` & `netius-1.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `netius-1.9.8/setup.py` & `netius-1.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 sys.path.insert(0, NETIUS_DIR)
 
 import netius.common
 
 netius.common.ensure_setup()
 setuptools.setup(
     name = "netius",
-    version = "1.9.8",
+    version = "1.9.9",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Netius System",
     license = "Apache License, Version 2.0",
     keywords = "netius net infrastructure wsgi",
     url = "http://netius.hive.pt",
     zip_safe = False,
```

### Comparing `netius-1.9.8/PKG-INFO` & `netius-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: netius
-Version: 1.9.8
+Version: 1.9.9
 Summary: Netius System
 Home-page: http://netius.hive.pt
 Author: Hive Solutions Lda.
 Author-email: development@hive.pt
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Keywords: netius net infrastructure wsgi
```

