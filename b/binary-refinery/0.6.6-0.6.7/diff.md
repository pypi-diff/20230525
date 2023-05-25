# Comparing `tmp/binary-refinery-0.6.6.tar.gz` & `tmp/binary-refinery-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-jllhhbmv/binary-refinery-0.6.6.tar", last modified: Wed May 10 11:25:31 2023, max compression
+gzip compressed data, was "/home/runner/work/refinery/refinery/dist/.tmp-nue5hsdn/binary-refinery-0.6.7.tar", last modified: Thu May 25 16:52:04 2023, max compression
```

## Comparing `binary-refinery-0.6.6.tar` & `binary-refinery-0.6.7.tar`

### file list

```diff
@@ -1,381 +1,383 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/binary_refinery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/__init__.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49846 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/data/rich.json
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/explore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59048 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/argformats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/decompression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/deobfuscation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/lib/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dotnet/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dotnet/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dotnet/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/dotnet/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/java.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)    34515 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/mime.py
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/mscrypto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/murmur.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/lib/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    16925 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/patterns/tlds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/powershell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/ripemd128.py
--rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/suffixtree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/acefile.py
--rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/batch_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/pcode2code.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/thirdparty/xxhash.py
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/vfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/lib/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/
--rw-r--r--   0 runner    (1001) docker     (123)    70717 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/blockwise/
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/alu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/bitrev.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/byteswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/neg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/rev.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/rotl.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/rotr.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/shl.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/shr.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/terminate.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/blockwise/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/compression/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/ap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/blz.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/bz2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/decompress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/jcalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lz4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lzf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lzg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lzjb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lznt1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/lzo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/mscf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/qlz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/szdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/compression/zl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/crypto/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/blowfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/camellia.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/cast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/chacha.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/des.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/des3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/gost.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/hc128.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/isaac.py
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rc2.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rc4mod.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rc5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rc6.py
--rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rijndael.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rncrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rot.py
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/rsakey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/salsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/seal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/secstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/serpent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/tea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/vigenere.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/xtea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/cipher/xxtea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/checksums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/cryptographic.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/imphash.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/murmur.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/password_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/hash/xxhash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/CryptDeriveKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/DESDerive.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/hmac.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/kblob.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/pbkdf1.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/pbkdf2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/crypto/keyderive/unixcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/encoding/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/atbash.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/b32.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/b58.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/b64.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/b85.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/cp1252.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/esc.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/htmlesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/netbios.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/ps1str.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/recode.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/u16.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/url.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/uuenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/encoding/wshenc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/a3x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xt7z.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtasar.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtcab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtcpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtiso.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtnode.py
--rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtnsis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtpyi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xttar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/archive/xtzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/bat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/deserialize_php.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/dexstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/evtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/exe/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/vaddr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/vmemref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/vsect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/vsnip.py
--rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/exe/vstack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/hexload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/httpresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/ifps.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/ifpsstr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/java/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/java/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/java/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/java/jvdasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/java/jvstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/msi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/office/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/doctxt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/officecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/vbapc.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/vbastr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xlmdeobf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xlxtr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xtdoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xtone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xtrtf.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/office/xtvba.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pcap_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/pe/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnblob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dncfx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnds.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnfields.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnhdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnrc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnstr.py
--rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/pemeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/peoverlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/perc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/pesig.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pe/pestrip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pkcs7.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/pkcs7sig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/stego.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/tnetmtm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/winreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/formats/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/malware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/malware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/malware/n40.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/chop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/cm.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/cull.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/dedup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/eat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/ef.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/emit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/iff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/iffp.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/iffs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/iffx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/min.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/mvc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/mvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/pick.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/pop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/put.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/sep.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/sorted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/swap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/meta/xfcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/autoxor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/couple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/datefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/drp.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/nop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/urlfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/misc/xkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/obfuscation/
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/obfuscation/js/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/js/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/js/arrays.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/js/getattr.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/js/tuples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/securestring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/typecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/ps1/uncurly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/brackets.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/char.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/dummies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/stringreplace.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/stringreverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/obfuscation/vba/vba.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_7z.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_pe.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/carve_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/defang.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/dnsdomain.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/mimewords.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/resplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/resub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/rex.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/struct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/subfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/urlguards.py
--rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/xtp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/pattern/xtw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/asm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/iemap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/peek.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/ppjscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/ppjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/sinks/ppxml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/refinery/units/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/cca.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/ccp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/cfmt.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/clower.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/cswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/cupper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/rep.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/snip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/stretch.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/termfit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/refinery/units/strings/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 11:25:31.000000 binary-refinery-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-10 11:25:11.000000 binary-refinery-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17628 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15242 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/binary_refinery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/__init__.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50050 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/data/rich.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/explore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59048 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/argformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16375 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/decompression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/deobfuscation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/lib/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dotnet/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30549 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dotnet/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dotnet/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10738 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/dotnet/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23050 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23540 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/java.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34707 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/mime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/mscrypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/murmur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/lib/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    17558 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/patterns/tlds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/powershell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/ripemd128.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23138 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/suffixtree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   163388 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/acefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/batch_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127576 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/pcode2code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/thirdparty/xxhash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/lib/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    70717 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/blockwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/alu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/bitrev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/byteswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/rev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/rotl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/rotr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/shl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/shr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/terminate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/blockwise/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/compression/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/ap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/blz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/bz2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/decompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/jcalg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lz4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lzf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lzg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lzjb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lznt1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/lzo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/mscf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/qlz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/szdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/compression/zl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/camellia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/chacha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/chaskey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/des3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/gost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/hc128.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/isaac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rc2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rc4mod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rc5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rc6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48363 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rijndael.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rncrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/rsakey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/salsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/seal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/secstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/serpent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/tea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/vigenere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/xtea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/cipher/xxtea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/checksums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/cryptographic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/imphash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/murmur.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/password_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/hash/xxhash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/CryptDeriveKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/DESDerive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/PasswordDeriveBytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/kblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/pbkdf1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/pbkdf2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/crypto/keyderive/unixcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/encoding/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/atbash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/b32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/b58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/b64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/b85.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/cp1252.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/esc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/htmlesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/netbios.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/ps1str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/recode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/u16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/uuenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/encoding/wshenc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/a3x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xt7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtasar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtcab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtcpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtgz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtiso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46989 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtnsis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20487 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtpyi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xttar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/archive/xtzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/bat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/deserialize_php.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/dexstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/evtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/exe/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/vaddr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/vmemref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/vsect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/vsnip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11318 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/exe/vstack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/hexload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/httpresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30158 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/ifps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/ifpsstr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/java/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/java/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/java/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/java/jvdasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/java/jvstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/msi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/office/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/doctxt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/officecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/vbapc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/vbastr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xlmdeobf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xlxtr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xtdoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xtone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xtrtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/office/xtvba.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pcap_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/pe/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnblob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dncfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnfields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnhdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnrc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/pemeta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/peoverlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/perc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/pesig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pe/pestrip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pkcs7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/pkcs7sig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/stego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/tnetmtm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/winreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/formats/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/malware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/malware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/malware/n40.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/chop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/cm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/cull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/dedup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/eat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/ef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/emit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/iff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/iffp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/iffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/iffx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/min.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/mvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/mvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/pick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/pop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/put.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/sorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/swap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/meta/xfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/autoxor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/couple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/datefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/urlfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/misc/xkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/obfuscation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/obfuscation/js/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/js/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/js/arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/js/getattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/js/tuples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/securestring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/typecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/ps1/uncurly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/brackets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/char.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/dummies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/stringreplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/stringreverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/obfuscation/vba/vba.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_7z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/carve_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/defang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/dnsdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/mimewords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/resplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/resub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/rex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/struct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/subfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/urlguards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14200 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/xtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/pattern/xtw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/asm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/iemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10573 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/peek.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/ppjscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/ppjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/sinks/ppxml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/refinery/units/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/ccp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/cfmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/clower.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/cswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/cupper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/snip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/stretch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/termfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/refinery/units/strings/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 16:52:04.000000 binary-refinery-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-25 16:51:44.000000 binary-refinery-0.6.7/setup.py
```

### Comparing `binary-refinery-0.6.6/LICENSE` & `binary-refinery-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/PKG-INFO` & `binary-refinery-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.6
+Version: 0.6.7
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `binary-refinery-0.6.6/README.md` & `binary-refinery-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/binary_refinery.egg-info/PKG-INFO` & `binary-refinery-0.6.7/binary_refinery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binary-refinery
-Version: 0.6.6
+Version: 0.6.7
 Summary: A toolkit to transform and refine (mostly) binary data.
 Home-page: https://github.com/binref/refinery/
 Author: Jesko Huettenhain
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `binary-refinery-0.6.6/binary_refinery.egg-info/SOURCES.txt` & `binary-refinery-0.6.7/binary_refinery.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 refinery/units/crypto/__init__.py
 refinery/units/crypto/cipher/__init__.py
 refinery/units/crypto/cipher/aes.py
 refinery/units/crypto/cipher/blowfish.py
 refinery/units/crypto/cipher/camellia.py
 refinery/units/crypto/cipher/cast.py
 refinery/units/crypto/cipher/chacha.py
+refinery/units/crypto/cipher/chaskey.py
 refinery/units/crypto/cipher/des.py
 refinery/units/crypto/cipher/des3.py
 refinery/units/crypto/cipher/gost.py
 refinery/units/crypto/cipher/hc128.py
 refinery/units/crypto/cipher/isaac.py
 refinery/units/crypto/cipher/rabbit.py
 refinery/units/crypto/cipher/rc2.py
@@ -187,14 +188,15 @@
 refinery/units/formats/archive/__init__.py
 refinery/units/formats/archive/xt.py
 refinery/units/formats/archive/xt7z.py
 refinery/units/formats/archive/xtace.py
 refinery/units/formats/archive/xtasar.py
 refinery/units/formats/archive/xtcab.py
 refinery/units/formats/archive/xtcpio.py
+refinery/units/formats/archive/xtgz.py
 refinery/units/formats/archive/xtiso.py
 refinery/units/formats/archive/xtiss.py
 refinery/units/formats/archive/xtnode.py
 refinery/units/formats/archive/xtnsis.py
 refinery/units/formats/archive/xtpyi.py
 refinery/units/formats/archive/xttar.py
 refinery/units/formats/archive/xtzip.py
```

### Comparing `binary-refinery-0.6.6/binary_refinery.egg-info/entry_points.txt` & `binary-refinery-0.6.7/binary_refinery.egg-info/entry_points.txt`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 carve-zip = refinery.units.pattern.carve_zip:carve_zip.run
 cast = refinery.units.crypto.cipher.cast:cast.run
 cca = refinery.units.strings.cca:cca.run
 ccp = refinery.units.strings.ccp:ccp.run
 cfmt = refinery.units.strings.cfmt:cfmt.run
 chacha = refinery.units.crypto.cipher.chacha:chacha.run
 chacha20 = refinery.units.crypto.cipher.chacha:chacha20.run
+chaskey = refinery.units.crypto.cipher.chaskey:chaskey.run
 chop = refinery.units.meta.chop:chop.run
 clower = refinery.units.strings.clower:clower.run
 cm = refinery.units.meta.cm:cm.run
 couple = refinery.units.misc.couple:couple.run
 cp1252 = refinery.units.encoding.cp1252:cp1252.run
 crc32 = refinery.units.crypto.hash.checksums:crc32.run
 csv = refinery.units.formats.csv:csv.run
@@ -258,14 +259,15 @@
 xt7z = refinery.units.formats.archive.xt7z:xt7z.run
 xtace = refinery.units.formats.archive.xtace:xtace.run
 xtasar = refinery.units.formats.archive.xtasar:xtasar.run
 xtcab = refinery.units.formats.archive.xtcab:xtcab.run
 xtcpio = refinery.units.formats.archive.xtcpio:xtcpio.run
 xtdoc = refinery.units.formats.office.xtdoc:xtdoc.run
 xtea = refinery.units.crypto.cipher.xtea:xtea.run
+xtgz = refinery.units.formats.archive.xtgz:xtgz.run
 xthtml = refinery.units.formats.html:xthtml.run
 xtiso = refinery.units.formats.archive.xtiso:xtiso.run
 xtiss = refinery.units.formats.archive.xtiss:xtiss.run
 xtjson = refinery.units.formats.json:xtjson.run
 xtmail = refinery.units.formats.email:xtmail.run
 xtmsi = refinery.units.formats.msi:xtmsi.run
 xtnode = refinery.units.formats.archive.xtnode:xtnode.run
```

### Comparing `binary-refinery-0.6.6/binary_refinery.egg-info/requires.txt` & `binary-refinery-0.6.7/binary_refinery.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -5,56 +5,56 @@
 pefile
 pycryptodomex
 pyelftools
 setuptools
 toml
 wheel
 python-magic
-phpserialize
-msoffcrypto-tool
 asn1crypto
-Pillow
-pyperclip
 openpyxl
+decompyle3
+Pillow
+pycdlib
+msoffcrypto-tool
+python-registry
+uncompyle6
 javaobj-py3>=0.4.0.1
-cabarchive
-py7zr
-extract-msg
+pyonenote
 olefile
-capstone
-XLMMacroDeobfuscator
-decompyle3
 LnkParse3
-xlrd2
-pyonenote
-pycdlib
 xdis
-uncompyle6
-chardet
-python-registry
 PyPDF2>=3.0.0
 pyxlsb2
+XLMMacroDeobfuscator
+cabarchive
+py7zr
+capstone
+phpserialize
+extract-msg
+chardet
+pyperclip
+xlrd2
 
 [add]
 numpy
 
 [all]
-mitmproxy
-unicorn
-python-evtx
-pyzipper
 angr
+numpy
+pyzipper
 pypcapkit[scapy]<0.16.0
-colorama
 intervaltree
+colorama
+oletools
 jsbeautifier
 capstone
-numpy
+mitmproxy
 chardet
-oletools
+python-evtx
+unicorn
 
 [alu]
 numpy
 
 [asm]
 angr
 
@@ -128,16 +128,16 @@
 oletools
 
 [vmemref]
 angr
 
 [vstack]
 unicorn
-intervaltree
 capstone
+intervaltree
 
 [xor]
 numpy
 
 [xtrtf]
 oletools
```

### Comparing `binary-refinery-0.6.6/refinery/__init__.pkl` & `binary-refinery-0.6.7/refinery/__init__.pkl`

 * *Files 4% similar despite different names*

```diff
@@ -108,817 +108,824 @@
 000006b0: 0000 0063 6173 7471 4758 2100 0000 7265  ...castqGX!...re
 000006c0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
 000006d0: 7074 6f2e 6369 7068 6572 2e63 6173 7471  pto.cipher.castq
 000006e0: 4858 0600 0000 6368 6163 6861 7149 5823  HX....chachaqIX#
 000006f0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
 00000700: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
 00000710: 6368 6163 6861 714a 5808 0000 0063 6861  chachaqJX....cha
-00000720: 6368 6132 3071 4b68 4a58 0300 0000 6465  cha20qKhJX....de
-00000730: 7371 4c58 2000 0000 7265 6669 6e65 7279  sqLX ...refinery
-00000740: 2e75 6e69 7473 2e63 7279 7074 6f2e 6369  .units.crypto.ci
-00000750: 7068 6572 2e64 6573 714d 5804 0000 0064  pher.desqMX....d
-00000760: 6573 3371 4e58 2100 0000 7265 6669 6e65  es3qNX!...refine
-00000770: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00000780: 6369 7068 6572 2e64 6573 3371 4f58 0400  cipher.des3qOX..
-00000790: 0000 676f 7374 7150 5821 0000 0072 6566  ..gostqPX!...ref
-000007a0: 696e 6572 792e 756e 6974 732e 6372 7970  inery.units.cryp
-000007b0: 746f 2e63 6970 6865 722e 676f 7374 7151  to.cipher.gostqQ
-000007c0: 5805 0000 0068 6331 3238 7152 5822 0000  X....hc128qRX"..
-000007d0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000007e0: 6372 7970 746f 2e63 6970 6865 722e 6863  crypto.cipher.hc
-000007f0: 3132 3871 5358 0500 0000 6973 6161 6371  128qSX....isaacq
-00000800: 5458 2200 0000 7265 6669 6e65 7279 2e75  TX"...refinery.u
-00000810: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
-00000820: 6572 2e69 7361 6163 7155 5806 0000 0072  er.isaacqUX....r
-00000830: 6162 6269 7471 5658 2300 0000 7265 6669  abbitqVX#...refi
-00000840: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
-00000850: 6f2e 6369 7068 6572 2e72 6162 6269 7471  o.cipher.rabbitq
-00000860: 5758 0300 0000 7263 3271 5858 2000 0000  WX....rc2qXX ...
-00000870: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-00000880: 7279 7074 6f2e 6369 7068 6572 2e72 6332  rypto.cipher.rc2
-00000890: 7159 5803 0000 0072 6334 715a 5820 0000  qYX....rc4qZX ..
-000008a0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000008b0: 6372 7970 746f 2e63 6970 6865 722e 7263  crypto.cipher.rc
-000008c0: 3471 5b58 0600 0000 7263 346d 6f64 715c  4q[X....rc4modq\
-000008d0: 5823 0000 0072 6566 696e 6572 792e 756e  X#...refinery.un
-000008e0: 6974 732e 6372 7970 746f 2e63 6970 6865  its.crypto.ciphe
-000008f0: 722e 7263 346d 6f64 715d 5803 0000 0072  r.rc4modq]X....r
-00000900: 6335 715e 5820 0000 0072 6566 696e 6572  c5q^X ...refiner
-00000910: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
-00000920: 6970 6865 722e 7263 3571 5f58 0300 0000  ipher.rc5q_X....
-00000930: 7263 3671 6058 2000 0000 7265 6669 6e65  rc6q`X ...refine
-00000940: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00000950: 6369 7068 6572 2e72 6336 7161 5808 0000  cipher.rc6qaX...
-00000960: 0072 696a 6e64 6165 6c71 6258 2500 0000  .rijndaelqbX%...
-00000970: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-00000980: 7279 7074 6f2e 6369 7068 6572 2e72 696a  rypto.cipher.rij
-00000990: 6e64 6165 6c71 6358 0700 0000 726e 6372  ndaelqcX....rncr
-000009a0: 7970 7471 6458 2400 0000 7265 6669 6e65  yptqdX$...refine
-000009b0: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-000009c0: 6369 7068 6572 2e72 6e63 7279 7074 7165  cipher.rncryptqe
-000009d0: 5803 0000 0072 6f74 7166 5820 0000 0072  X....rotqfX ...r
-000009e0: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
-000009f0: 7970 746f 2e63 6970 6865 722e 726f 7471  ypto.cipher.rotq
-00000a00: 6758 0300 0000 7273 6171 6858 2000 0000  gX....rsaqhX ...
-00000a10: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-00000a20: 7279 7074 6f2e 6369 7068 6572 2e72 7361  rypto.cipher.rsa
-00000a30: 7169 5806 0000 0072 7361 6b65 7971 6a58  qiX....rsakeyqjX
-00000a40: 2300 0000 7265 6669 6e65 7279 2e75 6e69  #...refinery.uni
-00000a50: 7473 2e63 7279 7074 6f2e 6369 7068 6572  ts.crypto.cipher
-00000a60: 2e72 7361 6b65 7971 6b58 0500 0000 7361  .rsakeyqkX....sa
-00000a70: 6c73 6171 6c58 2200 0000 7265 6669 6e65  lsaqlX"...refine
-00000a80: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
-00000a90: 6369 7068 6572 2e73 616c 7361 716d 5807  cipher.salsaqmX.
-00000aa0: 0000 0073 616c 7361 3230 716e 686d 5804  ...salsa20qnhmX.
-00000ab0: 0000 0073 6561 6c71 6f58 2100 0000 7265  ...sealqoX!...re
-00000ac0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
-00000ad0: 7074 6f2e 6369 7068 6572 2e73 6561 6c71  pto.cipher.sealq
-00000ae0: 7058 0600 0000 7365 6373 7472 7171 5823  pX....secstrqqX#
-00000af0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00000b00: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
-00000b10: 7365 6373 7472 7172 5807 0000 0073 6572  secstrqrX....ser
-00000b20: 7065 6e74 7173 5824 0000 0072 6566 696e  pentqsX$...refin
-00000b30: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
-00000b40: 2e63 6970 6865 722e 7365 7270 656e 7471  .cipher.serpentq
-00000b50: 7458 0300 0000 7465 6171 7558 2000 0000  tX....teaquX ...
-00000b60: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-00000b70: 7279 7074 6f2e 6369 7068 6572 2e74 6561  rypto.cipher.tea
-00000b80: 7176 5808 0000 0076 6967 656e 6572 6571  qvX....vigenereq
-00000b90: 7758 2500 0000 7265 6669 6e65 7279 2e75  wX%...refinery.u
-00000ba0: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
-00000bb0: 6572 2e76 6967 656e 6572 6571 7858 0400  er.vigenereqxX..
-00000bc0: 0000 7874 6561 7179 5821 0000 0072 6566  ..xteaqyX!...ref
-00000bd0: 696e 6572 792e 756e 6974 732e 6372 7970  inery.units.cryp
-00000be0: 746f 2e63 6970 6865 722e 7874 6561 717a  to.cipher.xteaqz
-00000bf0: 5805 0000 0078 7874 6561 717b 5822 0000  X....xxteaq{X"..
-00000c00: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00000c10: 6372 7970 746f 2e63 6970 6865 722e 7878  crypto.cipher.xx
-00000c20: 7465 6171 7c58 0700 0000 6164 6c65 7233  teaq|X....adler3
-00000c30: 3271 7d58 2400 0000 7265 6669 6e65 7279  2q}X$...refinery
-00000c40: 2e75 6e69 7473 2e63 7279 7074 6f2e 6861  .units.crypto.ha
-00000c50: 7368 2e63 6865 636b 7375 6d73 717e 5805  sh.checksumsq~X.
-00000c60: 0000 0063 7263 3332 717f 687e 5806 0000  ...crc32q.h~X...
-00000c70: 0062 6c6b 3232 3471 8058 2800 0000 7265  .blk224q.X(...re
-00000c80: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
-00000c90: 7074 6f2e 6861 7368 2e63 7279 7074 6f67  pto.hash.cryptog
-00000ca0: 7261 7068 6963 7181 5806 0000 0062 6c6b  raphicq.X....blk
-00000cb0: 3235 3671 8268 8158 0600 0000 626c 6b33  256q.h.X....blk3
-00000cc0: 3834 7183 6881 5806 0000 0062 6c6b 3531  84q.h.X....blk51
-00000cd0: 3271 8468 8158 0300 0000 6d64 3271 8568  2q.h.X....md2q.h
-00000ce0: 8158 0300 0000 6d64 3471 8668 8158 0300  .X....md4q.h.X..
-00000cf0: 0000 6d64 3571 8768 8158 0900 0000 7269  ..md5q.h.X....ri
-00000d00: 7065 6d64 3132 3871 8868 8158 0900 0000  pemd128q.h.X....
-00000d10: 7269 7065 6d64 3136 3071 8968 8158 0400  ripemd160q.h.X..
-00000d20: 0000 7368 6131 718a 6881 5806 0000 0073  ..sha1q.h.X....s
-00000d30: 6861 3232 3471 8b68 8158 0600 0000 7368  ha224q.h.X....sh
-00000d40: 6132 3536 718c 6881 5806 0000 0073 6861  a256q.h.X....sha
-00000d50: 3338 3471 8d68 8158 0600 0000 7368 6135  384q.h.X....sha5
-00000d60: 3132 718e 6881 5807 0000 0069 6d70 6861  12q.h.X....impha
-00000d70: 7368 718f 5822 0000 0072 6566 696e 6572  shq.X"...refiner
-00000d80: 792e 756e 6974 732e 6372 7970 746f 2e68  y.units.crypto.h
-00000d90: 6173 682e 696d 7068 6173 6871 9058 0900  ash.imphashq.X..
-00000da0: 0000 6d6d 6831 3238 7833 3271 9158 2100  ..mmh128x32q.X!.
+00000720: 6368 6132 3071 4b68 4a58 0700 0000 6368  cha20qKhJX....ch
+00000730: 6173 6b65 7971 4c58 2400 0000 7265 6669  askeyqLX$...refi
+00000740: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
+00000750: 6f2e 6369 7068 6572 2e63 6861 736b 6579  o.cipher.chaskey
+00000760: 714d 5803 0000 0064 6573 714e 5820 0000  qMX....desqNX ..
+00000770: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00000780: 6372 7970 746f 2e63 6970 6865 722e 6465  crypto.cipher.de
+00000790: 7371 4f58 0400 0000 6465 7333 7150 5821  sqOX....des3qPX!
+000007a0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000007b0: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
+000007c0: 6465 7333 7151 5804 0000 0067 6f73 7471  des3qQX....gostq
+000007d0: 5258 2100 0000 7265 6669 6e65 7279 2e75  RX!...refinery.u
+000007e0: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
+000007f0: 6572 2e67 6f73 7471 5358 0500 0000 6863  er.gostqSX....hc
+00000800: 3132 3871 5458 2200 0000 7265 6669 6e65  128qTX"...refine
+00000810: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+00000820: 6369 7068 6572 2e68 6331 3238 7155 5805  cipher.hc128qUX.
+00000830: 0000 0069 7361 6163 7156 5822 0000 0072  ...isaacqVX"...r
+00000840: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
+00000850: 7970 746f 2e63 6970 6865 722e 6973 6161  ypto.cipher.isaa
+00000860: 6371 5758 0600 0000 7261 6262 6974 7158  cqWX....rabbitqX
+00000870: 5823 0000 0072 6566 696e 6572 792e 756e  X#...refinery.un
+00000880: 6974 732e 6372 7970 746f 2e63 6970 6865  its.crypto.ciphe
+00000890: 722e 7261 6262 6974 7159 5803 0000 0072  r.rabbitqYX....r
+000008a0: 6332 715a 5820 0000 0072 6566 696e 6572  c2qZX ...refiner
+000008b0: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
+000008c0: 6970 6865 722e 7263 3271 5b58 0300 0000  ipher.rc2q[X....
+000008d0: 7263 3471 5c58 2000 0000 7265 6669 6e65  rc4q\X ...refine
+000008e0: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+000008f0: 6369 7068 6572 2e72 6334 715d 5806 0000  cipher.rc4q]X...
+00000900: 0072 6334 6d6f 6471 5e58 2300 0000 7265  .rc4modq^X#...re
+00000910: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+00000920: 7074 6f2e 6369 7068 6572 2e72 6334 6d6f  pto.cipher.rc4mo
+00000930: 6471 5f58 0300 0000 7263 3571 6058 2000  dq_X....rc5q`X .
+00000940: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00000950: 2e63 7279 7074 6f2e 6369 7068 6572 2e72  .crypto.cipher.r
+00000960: 6335 7161 5803 0000 0072 6336 7162 5820  c5qaX....rc6qbX 
+00000970: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00000980: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
+00000990: 7263 3671 6358 0800 0000 7269 6a6e 6461  rc6qcX....rijnda
+000009a0: 656c 7164 5825 0000 0072 6566 696e 6572  elqdX%...refiner
+000009b0: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
+000009c0: 6970 6865 722e 7269 6a6e 6461 656c 7165  ipher.rijndaelqe
+000009d0: 5807 0000 0072 6e63 7279 7074 7166 5824  X....rncryptqfX$
+000009e0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000009f0: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
+00000a00: 726e 6372 7970 7471 6758 0300 0000 726f  rncryptqgX....ro
+00000a10: 7471 6858 2000 0000 7265 6669 6e65 7279  tqhX ...refinery
+00000a20: 2e75 6e69 7473 2e63 7279 7074 6f2e 6369  .units.crypto.ci
+00000a30: 7068 6572 2e72 6f74 7169 5803 0000 0072  pher.rotqiX....r
+00000a40: 7361 716a 5820 0000 0072 6566 696e 6572  saqjX ...refiner
+00000a50: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
+00000a60: 6970 6865 722e 7273 6171 6b58 0600 0000  ipher.rsaqkX....
+00000a70: 7273 616b 6579 716c 5823 0000 0072 6566  rsakeyqlX#...ref
+00000a80: 696e 6572 792e 756e 6974 732e 6372 7970  inery.units.cryp
+00000a90: 746f 2e63 6970 6865 722e 7273 616b 6579  to.cipher.rsakey
+00000aa0: 716d 5805 0000 0073 616c 7361 716e 5822  qmX....salsaqnX"
+00000ab0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00000ac0: 732e 6372 7970 746f 2e63 6970 6865 722e  s.crypto.cipher.
+00000ad0: 7361 6c73 6171 6f58 0700 0000 7361 6c73  salsaqoX....sals
+00000ae0: 6132 3071 7068 6f58 0400 0000 7365 616c  a20qphoX....seal
+00000af0: 7171 5821 0000 0072 6566 696e 6572 792e  qqX!...refinery.
+00000b00: 756e 6974 732e 6372 7970 746f 2e63 6970  units.crypto.cip
+00000b10: 6865 722e 7365 616c 7172 5806 0000 0073  her.sealqrX....s
+00000b20: 6563 7374 7271 7358 2300 0000 7265 6669  ecstrqsX#...refi
+00000b30: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
+00000b40: 6f2e 6369 7068 6572 2e73 6563 7374 7271  o.cipher.secstrq
+00000b50: 7458 0700 0000 7365 7270 656e 7471 7558  tX....serpentquX
+00000b60: 2400 0000 7265 6669 6e65 7279 2e75 6e69  $...refinery.uni
+00000b70: 7473 2e63 7279 7074 6f2e 6369 7068 6572  ts.crypto.cipher
+00000b80: 2e73 6572 7065 6e74 7176 5803 0000 0074  .serpentqvX....t
+00000b90: 6561 7177 5820 0000 0072 6566 696e 6572  eaqwX ...refiner
+00000ba0: 792e 756e 6974 732e 6372 7970 746f 2e63  y.units.crypto.c
+00000bb0: 6970 6865 722e 7465 6171 7858 0800 0000  ipher.teaqxX....
+00000bc0: 7669 6765 6e65 7265 7179 5825 0000 0072  vigenereqyX%...r
+00000bd0: 6566 696e 6572 792e 756e 6974 732e 6372  efinery.units.cr
+00000be0: 7970 746f 2e63 6970 6865 722e 7669 6765  ypto.cipher.vige
+00000bf0: 6e65 7265 717a 5804 0000 0078 7465 6171  nereqzX....xteaq
+00000c00: 7b58 2100 0000 7265 6669 6e65 7279 2e75  {X!...refinery.u
+00000c10: 6e69 7473 2e63 7279 7074 6f2e 6369 7068  nits.crypto.ciph
+00000c20: 6572 2e78 7465 6171 7c58 0500 0000 7878  er.xteaq|X....xx
+00000c30: 7465 6171 7d58 2200 0000 7265 6669 6e65  teaq}X"...refine
+00000c40: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+00000c50: 6369 7068 6572 2e78 7874 6561 717e 5807  cipher.xxteaq~X.
+00000c60: 0000 0061 646c 6572 3332 717f 5824 0000  ...adler32q.X$..
+00000c70: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00000c80: 6372 7970 746f 2e68 6173 682e 6368 6563  crypto.hash.chec
+00000c90: 6b73 756d 7371 8058 0500 0000 6372 6333  ksumsq.X....crc3
+00000ca0: 3271 8168 8058 0600 0000 626c 6b32 3234  2q.h.X....blk224
+00000cb0: 7182 5828 0000 0072 6566 696e 6572 792e  q.X(...refinery.
+00000cc0: 756e 6974 732e 6372 7970 746f 2e68 6173  units.crypto.has
+00000cd0: 682e 6372 7970 746f 6772 6170 6869 6371  h.cryptographicq
+00000ce0: 8358 0600 0000 626c 6b32 3536 7184 6883  .X....blk256q.h.
+00000cf0: 5806 0000 0062 6c6b 3338 3471 8568 8358  X....blk384q.h.X
+00000d00: 0600 0000 626c 6b35 3132 7186 6883 5803  ....blk512q.h.X.
+00000d10: 0000 006d 6432 7187 6883 5803 0000 006d  ...md2q.h.X....m
+00000d20: 6434 7188 6883 5803 0000 006d 6435 7189  d4q.h.X....md5q.
+00000d30: 6883 5809 0000 0072 6970 656d 6431 3238  h.X....ripemd128
+00000d40: 718a 6883 5809 0000 0072 6970 656d 6431  q.h.X....ripemd1
+00000d50: 3630 718b 6883 5804 0000 0073 6861 3171  60q.h.X....sha1q
+00000d60: 8c68 8358 0600 0000 7368 6132 3234 718d  .h.X....sha224q.
+00000d70: 6883 5806 0000 0073 6861 3235 3671 8e68  h.X....sha256q.h
+00000d80: 8358 0600 0000 7368 6133 3834 718f 6883  .X....sha384q.h.
+00000d90: 5806 0000 0073 6861 3531 3271 9068 8358  X....sha512q.h.X
+00000da0: 0700 0000 696d 7068 6173 6871 9158 2200  ....imphashq.X".
 00000db0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000dc0: 2e63 7279 7074 6f2e 6861 7368 2e6d 7572  .crypto.hash.mur
-00000dd0: 6d75 7271 9258 0900 0000 6d6d 6831 3238  murq.X....mmh128
-00000de0: 7836 3471 9368 9258 0500 0000 6d6d 6833  x64q.h.X....mmh3
-00000df0: 3271 9468 9258 0400 0000 6e74 6c6d 7195  2q.h.X....ntlmq.
-00000e00: 582a 0000 0072 6566 696e 6572 792e 756e  X*...refinery.un
-00000e10: 6974 732e 6372 7970 746f 2e68 6173 682e  its.crypto.hash.
-00000e20: 7061 7373 776f 7264 5f68 6173 6865 7371  password_hashesq
-00000e30: 9658 0300 0000 7878 6871 9758 2100 0000  .X....xxhq.X!...
-00000e40: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
-00000e50: 7279 7074 6f2e 6861 7368 2e78 7868 6173  rypto.hash.xxhas
-00000e60: 6871 9858 0e00 0000 4372 7970 7444 6572  hq.X....CryptDer
-00000e70: 6976 654b 6579 7199 582e 0000 0072 6566  iveKeyq.X....ref
-00000e80: 696e 6572 792e 756e 6974 732e 6372 7970  inery.units.cryp
-00000e90: 746f 2e6b 6579 6465 7269 7665 2e43 7279  to.keyderive.Cry
-00000ea0: 7074 4465 7269 7665 4b65 7971 9a58 0900  ptDeriveKeyq.X..
-00000eb0: 0000 4445 5344 6572 6976 6571 9b58 2900  ..DESDeriveq.X).
-00000ec0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00000ed0: 2e63 7279 7074 6f2e 6b65 7964 6572 6976  .crypto.keyderiv
-00000ee0: 652e 4445 5344 6572 6976 6571 9c58 1300  e.DESDeriveq.X..
-00000ef0: 0000 5061 7373 776f 7264 4465 7269 7665  ..PasswordDerive
-00000f00: 4279 7465 7371 9d58 3300 0000 7265 6669  Bytesq.X3...refi
-00000f10: 6e65 7279 2e75 6e69 7473 2e63 7279 7074  nery.units.crypt
-00000f20: 6f2e 6b65 7964 6572 6976 652e 5061 7373  o.keyderive.Pass
-00000f30: 776f 7264 4465 7269 7665 4279 7465 7371  wordDeriveBytesq
-00000f40: 9e58 0400 0000 484b 4446 719f 5824 0000  .X....HKDFq.X$..
-00000f50: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00000f60: 6372 7970 746f 2e6b 6579 6465 7269 7665  crypto.keyderive
-00000f70: 2e68 6b64 6671 a058 0400 0000 686d 6163  .hkdfq.X....hmac
-00000f80: 71a1 5824 0000 0072 6566 696e 6572 792e  q.X$...refinery.
-00000f90: 756e 6974 732e 6372 7970 746f 2e6b 6579  units.crypto.key
-00000fa0: 6465 7269 7665 2e68 6d61 6371 a258 0500  derive.hmacq.X..
-00000fb0: 0000 6b62 6c6f 6271 a358 2500 0000 7265  ..kblobq.X%...re
-00000fc0: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
-00000fd0: 7074 6f2e 6b65 7964 6572 6976 652e 6b62  pto.keyderive.kb
-00000fe0: 6c6f 6271 a458 0600 0000 7062 6b64 6631  lobq.X....pbkdf1
-00000ff0: 71a5 5826 0000 0072 6566 696e 6572 792e  q.X&...refinery.
+00000dc0: 2e63 7279 7074 6f2e 6861 7368 2e69 6d70  .crypto.hash.imp
+00000dd0: 6861 7368 7192 5809 0000 006d 6d68 3132  hashq.X....mmh12
+00000de0: 3878 3332 7193 5821 0000 0072 6566 696e  8x32q.X!...refin
+00000df0: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
+00000e00: 2e68 6173 682e 6d75 726d 7572 7194 5809  .hash.murmurq.X.
+00000e10: 0000 006d 6d68 3132 3878 3634 7195 6894  ...mmh128x64q.h.
+00000e20: 5805 0000 006d 6d68 3332 7196 6894 5804  X....mmh32q.h.X.
+00000e30: 0000 006e 746c 6d71 9758 2a00 0000 7265  ...ntlmq.X*...re
+00000e40: 6669 6e65 7279 2e75 6e69 7473 2e63 7279  finery.units.cry
+00000e50: 7074 6f2e 6861 7368 2e70 6173 7377 6f72  pto.hash.passwor
+00000e60: 645f 6861 7368 6573 7198 5803 0000 0078  d_hashesq.X....x
+00000e70: 7868 7199 5821 0000 0072 6566 696e 6572  xhq.X!...refiner
+00000e80: 792e 756e 6974 732e 6372 7970 746f 2e68  y.units.crypto.h
+00000e90: 6173 682e 7878 6861 7368 719a 580e 0000  ash.xxhashq.X...
+00000ea0: 0043 7279 7074 4465 7269 7665 4b65 7971  .CryptDeriveKeyq
+00000eb0: 9b58 2e00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00000ec0: 6e69 7473 2e63 7279 7074 6f2e 6b65 7964  nits.crypto.keyd
+00000ed0: 6572 6976 652e 4372 7970 7444 6572 6976  erive.CryptDeriv
+00000ee0: 654b 6579 719c 5809 0000 0044 4553 4465  eKeyq.X....DESDe
+00000ef0: 7269 7665 719d 5829 0000 0072 6566 696e  riveq.X)...refin
+00000f00: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
+00000f10: 2e6b 6579 6465 7269 7665 2e44 4553 4465  .keyderive.DESDe
+00000f20: 7269 7665 719e 5813 0000 0050 6173 7377  riveq.X....Passw
+00000f30: 6f72 6444 6572 6976 6542 7974 6573 719f  ordDeriveBytesq.
+00000f40: 5833 0000 0072 6566 696e 6572 792e 756e  X3...refinery.un
+00000f50: 6974 732e 6372 7970 746f 2e6b 6579 6465  its.crypto.keyde
+00000f60: 7269 7665 2e50 6173 7377 6f72 6444 6572  rive.PasswordDer
+00000f70: 6976 6542 7974 6573 71a0 5804 0000 0048  iveBytesq.X....H
+00000f80: 4b44 4671 a158 2400 0000 7265 6669 6e65  KDFq.X$...refine
+00000f90: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+00000fa0: 6b65 7964 6572 6976 652e 686b 6466 71a2  keyderive.hkdfq.
+00000fb0: 5804 0000 0068 6d61 6371 a358 2400 0000  X....hmacq.X$...
+00000fc0: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
+00000fd0: 7279 7074 6f2e 6b65 7964 6572 6976 652e  rypto.keyderive.
+00000fe0: 686d 6163 71a4 5805 0000 006b 626c 6f62  hmacq.X....kblob
+00000ff0: 71a5 5825 0000 0072 6566 696e 6572 792e  q.X%...refinery.
 00001000: 756e 6974 732e 6372 7970 746f 2e6b 6579  units.crypto.key
-00001010: 6465 7269 7665 2e70 626b 6466 3171 a658  derive.pbkdf1q.X
-00001020: 0600 0000 7062 6b64 6632 71a7 5826 0000  ....pbkdf2q.X&..
-00001030: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00001040: 6372 7970 746f 2e6b 6579 6465 7269 7665  crypto.keyderive
-00001050: 2e70 626b 6466 3271 a858 0600 0000 7563  .pbkdf2q.X....uc
-00001060: 7279 7074 71a9 5829 0000 0072 6566 696e  ryptq.X)...refin
-00001070: 6572 792e 756e 6974 732e 6372 7970 746f  ery.units.crypto
-00001080: 2e6b 6579 6465 7269 7665 2e75 6e69 7863  .keyderive.unixc
-00001090: 7279 7074 71aa 5806 0000 0061 7462 6173  ryptq.X....atbas
-000010a0: 6871 ab58 1e00 0000 7265 6669 6e65 7279  hq.X....refinery
-000010b0: 2e75 6e69 7473 2e65 6e63 6f64 696e 672e  .units.encoding.
-000010c0: 6174 6261 7368 71ac 5803 0000 0062 3332  atbashq.X....b32
-000010d0: 71ad 581b 0000 0072 6566 696e 6572 792e  q.X....refinery.
-000010e0: 756e 6974 732e 656e 636f 6469 6e67 2e62  units.encoding.b
-000010f0: 3332 71ae 5803 0000 0062 3538 71af 581b  32q.X....b58q.X.
-00001100: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00001110: 732e 656e 636f 6469 6e67 2e62 3538 71b0  s.encoding.b58q.
-00001120: 5803 0000 0062 3634 71b1 581b 0000 0072  X....b64q.X....r
-00001130: 6566 696e 6572 792e 756e 6974 732e 656e  efinery.units.en
-00001140: 636f 6469 6e67 2e62 3634 71b2 5803 0000  coding.b64q.X...
-00001150: 0062 3835 71b3 581b 0000 0072 6566 696e  .b85q.X....refin
-00001160: 6572 792e 756e 6974 732e 656e 636f 6469  ery.units.encodi
-00001170: 6e67 2e62 3835 71b4 5804 0000 0062 6173  ng.b85q.X....bas
-00001180: 6571 b558 1c00 0000 7265 6669 6e65 7279  eq.X....refinery
-00001190: 2e75 6e69 7473 2e65 6e63 6f64 696e 672e  .units.encoding.
-000011a0: 6261 7365 71b6 5806 0000 0063 7031 3235  baseq.X....cp125
-000011b0: 3271 b758 1e00 0000 7265 6669 6e65 7279  2q.X....refinery
-000011c0: 2e75 6e69 7473 2e65 6e63 6f64 696e 672e  .units.encoding.
-000011d0: 6370 3132 3532 71b8 5803 0000 0065 7363  cp1252q.X....esc
-000011e0: 71b9 581b 0000 0072 6566 696e 6572 792e  q.X....refinery.
-000011f0: 756e 6974 732e 656e 636f 6469 6e67 2e65  units.encoding.e
-00001200: 7363 71ba 5803 0000 0068 6578 71bb 581b  scq.X....hexq.X.
-00001210: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00001220: 732e 656e 636f 6469 6e67 2e68 6578 71bc  s.encoding.hexq.
-00001230: 5807 0000 0068 746d 6c65 7363 71bd 581f  X....htmlescq.X.
-00001240: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00001250: 732e 656e 636f 6469 6e67 2e68 746d 6c65  s.encoding.htmle
-00001260: 7363 71be 5807 0000 006e 6574 6269 6f73  scq.X....netbios
-00001270: 71bf 581f 0000 0072 6566 696e 6572 792e  q.X....refinery.
-00001280: 756e 6974 732e 656e 636f 6469 6e67 2e6e  units.encoding.n
-00001290: 6574 6269 6f73 71c0 5806 0000 0070 7331  etbiosq.X....ps1
-000012a0: 7374 7271 c158 1e00 0000 7265 6669 6e65  strq.X....refine
-000012b0: 7279 2e75 6e69 7473 2e65 6e63 6f64 696e  ry.units.encodin
-000012c0: 672e 7073 3173 7472 71c2 5806 0000 0072  g.ps1strq.X....r
-000012d0: 6563 6f64 6571 c358 1e00 0000 7265 6669  ecodeq.X....refi
-000012e0: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
-000012f0: 696e 672e 7265 636f 6465 71c4 5803 0000  ing.recodeq.X...
-00001300: 0075 3136 71c5 581b 0000 0072 6566 696e  .u16q.X....refin
-00001310: 6572 792e 756e 6974 732e 656e 636f 6469  ery.units.encodi
-00001320: 6e67 2e75 3136 71c6 5803 0000 0075 726c  ng.u16q.X....url
-00001330: 71c7 581b 0000 0072 6566 696e 6572 792e  q.X....refinery.
-00001340: 756e 6974 732e 656e 636f 6469 6e67 2e75  units.encoding.u
-00001350: 726c 71c8 5805 0000 0075 7565 6e63 71c9  rlq.X....uuencq.
-00001360: 581d 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00001370: 6974 732e 656e 636f 6469 6e67 2e75 7565  its.encoding.uue
-00001380: 6e63 71ca 5806 0000 0077 7368 656e 6371  ncq.X....wshencq
-00001390: cb58 1e00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-000013a0: 6e69 7473 2e65 6e63 6f64 696e 672e 7773  nits.encoding.ws
-000013b0: 6865 6e63 71cc 5803 0000 0061 3378 71cd  hencq.X....a3xq.
-000013c0: 581a 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000013d0: 6974 732e 666f 726d 6174 732e 6133 7871  its.formats.a3xq
-000013e0: ce58 0200 0000 7874 71cf 5821 0000 0072  .X....xtq.X!...r
-000013f0: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00001400: 726d 6174 732e 6172 6368 6976 652e 7874  rmats.archive.xt
-00001410: 71d0 5804 0000 0078 7437 7a71 d158 2300  q.X....xt7zq.X#.
-00001420: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00001430: 2e66 6f72 6d61 7473 2e61 7263 6869 7665  .formats.archive
-00001440: 2e78 7437 7a71 d258 0500 0000 7874 6163  .xt7zq.X....xtac
-00001450: 6571 d358 2400 0000 7265 6669 6e65 7279  eq.X$...refinery
-00001460: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
-00001470: 7263 6869 7665 2e78 7461 6365 71d4 5806  rchive.xtaceq.X.
-00001480: 0000 0078 7461 7361 7271 d558 2500 0000  ...xtasarq.X%...
-00001490: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
-000014a0: 6f72 6d61 7473 2e61 7263 6869 7665 2e78  ormats.archive.x
-000014b0: 7461 7361 7271 d658 0500 0000 7874 6361  tasarq.X....xtca
-000014c0: 6271 d758 2400 0000 7265 6669 6e65 7279  bq.X$...refinery
-000014d0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
-000014e0: 7263 6869 7665 2e78 7463 6162 71d8 5806  rchive.xtcabq.X.
-000014f0: 0000 0078 7463 7069 6f71 d958 2500 0000  ...xtcpioq.X%...
-00001500: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
-00001510: 6f72 6d61 7473 2e61 7263 6869 7665 2e78  ormats.archive.x
-00001520: 7463 7069 6f71 da58 0500 0000 7874 6973  tcpioq.X....xtis
-00001530: 6f71 db58 2400 0000 7265 6669 6e65 7279  oq.X$...refinery
-00001540: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
-00001550: 7263 6869 7665 2e78 7469 736f 71dc 5805  rchive.xtisoq.X.
-00001560: 0000 0078 7469 7373 71dd 5824 0000 0072  ...xtissq.X$...r
-00001570: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00001580: 726d 6174 732e 6172 6368 6976 652e 7874  rmats.archive.xt
-00001590: 6973 7371 de58 0600 0000 7874 6e6f 6465  issq.X....xtnode
-000015a0: 71df 5825 0000 0072 6566 696e 6572 792e  q.X%...refinery.
-000015b0: 756e 6974 732e 666f 726d 6174 732e 6172  units.formats.ar
-000015c0: 6368 6976 652e 7874 6e6f 6465 71e0 5806  chive.xtnodeq.X.
-000015d0: 0000 0078 746e 7369 7371 e158 2500 0000  ...xtnsisq.X%...
-000015e0: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
-000015f0: 6f72 6d61 7473 2e61 7263 6869 7665 2e78  ormats.archive.x
-00001600: 746e 7369 7371 e258 0500 0000 7874 7079  tnsisq.X....xtpy
-00001610: 6971 e358 2400 0000 7265 6669 6e65 7279  iq.X$...refinery
-00001620: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
-00001630: 7263 6869 7665 2e78 7470 7969 71e4 5805  rchive.xtpyiq.X.
-00001640: 0000 0078 7474 6172 71e5 5824 0000 0072  ...xttarq.X$...r
-00001650: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00001660: 726d 6174 732e 6172 6368 6976 652e 7874  rmats.archive.xt
-00001670: 7461 7271 e658 0500 0000 7874 7a69 7071  tarq.X....xtzipq
+00001010: 6465 7269 7665 2e6b 626c 6f62 71a6 5806  derive.kblobq.X.
+00001020: 0000 0070 626b 6466 3171 a758 2600 0000  ...pbkdf1q.X&...
+00001030: 7265 6669 6e65 7279 2e75 6e69 7473 2e63  refinery.units.c
+00001040: 7279 7074 6f2e 6b65 7964 6572 6976 652e  rypto.keyderive.
+00001050: 7062 6b64 6631 71a8 5806 0000 0070 626b  pbkdf1q.X....pbk
+00001060: 6466 3271 a958 2600 0000 7265 6669 6e65  df2q.X&...refine
+00001070: 7279 2e75 6e69 7473 2e63 7279 7074 6f2e  ry.units.crypto.
+00001080: 6b65 7964 6572 6976 652e 7062 6b64 6632  keyderive.pbkdf2
+00001090: 71aa 5806 0000 0075 6372 7970 7471 ab58  q.X....ucryptq.X
+000010a0: 2900 0000 7265 6669 6e65 7279 2e75 6e69  )...refinery.uni
+000010b0: 7473 2e63 7279 7074 6f2e 6b65 7964 6572  ts.crypto.keyder
+000010c0: 6976 652e 756e 6978 6372 7970 7471 ac58  ive.unixcryptq.X
+000010d0: 0600 0000 6174 6261 7368 71ad 581e 0000  ....atbashq.X...
+000010e0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000010f0: 656e 636f 6469 6e67 2e61 7462 6173 6871  encoding.atbashq
+00001100: ae58 0300 0000 6233 3271 af58 1b00 0000  .X....b32q.X....
+00001110: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
+00001120: 6e63 6f64 696e 672e 6233 3271 b058 0300  ncoding.b32q.X..
+00001130: 0000 6235 3871 b158 1b00 0000 7265 6669  ..b58q.X....refi
+00001140: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
+00001150: 696e 672e 6235 3871 b258 0300 0000 6236  ing.b58q.X....b6
+00001160: 3471 b358 1b00 0000 7265 6669 6e65 7279  4q.X....refinery
+00001170: 2e75 6e69 7473 2e65 6e63 6f64 696e 672e  .units.encoding.
+00001180: 6236 3471 b458 0300 0000 6238 3571 b558  b64q.X....b85q.X
+00001190: 1b00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+000011a0: 7473 2e65 6e63 6f64 696e 672e 6238 3571  ts.encoding.b85q
+000011b0: b658 0400 0000 6261 7365 71b7 581c 0000  .X....baseq.X...
+000011c0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000011d0: 656e 636f 6469 6e67 2e62 6173 6571 b858  encoding.baseq.X
+000011e0: 0600 0000 6370 3132 3532 71b9 581e 0000  ....cp1252q.X...
+000011f0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001200: 656e 636f 6469 6e67 2e63 7031 3235 3271  encoding.cp1252q
+00001210: ba58 0300 0000 6573 6371 bb58 1b00 0000  .X....escq.X....
+00001220: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
+00001230: 6e63 6f64 696e 672e 6573 6371 bc58 0300  ncoding.escq.X..
+00001240: 0000 6865 7871 bd58 1b00 0000 7265 6669  ..hexq.X....refi
+00001250: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
+00001260: 696e 672e 6865 7871 be58 0700 0000 6874  ing.hexq.X....ht
+00001270: 6d6c 6573 6371 bf58 1f00 0000 7265 6669  mlescq.X....refi
+00001280: 6e65 7279 2e75 6e69 7473 2e65 6e63 6f64  nery.units.encod
+00001290: 696e 672e 6874 6d6c 6573 6371 c058 0700  ing.htmlescq.X..
+000012a0: 0000 6e65 7462 696f 7371 c158 1f00 0000  ..netbiosq.X....
+000012b0: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
+000012c0: 6e63 6f64 696e 672e 6e65 7462 696f 7371  ncoding.netbiosq
+000012d0: c258 0600 0000 7073 3173 7472 71c3 581e  .X....ps1strq.X.
+000012e0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000012f0: 732e 656e 636f 6469 6e67 2e70 7331 7374  s.encoding.ps1st
+00001300: 7271 c458 0600 0000 7265 636f 6465 71c5  rq.X....recodeq.
+00001310: 581e 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+00001320: 6974 732e 656e 636f 6469 6e67 2e72 6563  its.encoding.rec
+00001330: 6f64 6571 c658 0300 0000 7531 3671 c758  odeq.X....u16q.X
+00001340: 1b00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00001350: 7473 2e65 6e63 6f64 696e 672e 7531 3671  ts.encoding.u16q
+00001360: c858 0300 0000 7572 6c71 c958 1b00 0000  .X....urlq.X....
+00001370: 7265 6669 6e65 7279 2e75 6e69 7473 2e65  refinery.units.e
+00001380: 6e63 6f64 696e 672e 7572 6c71 ca58 0500  ncoding.urlq.X..
+00001390: 0000 7575 656e 6371 cb58 1d00 0000 7265  ..uuencq.X....re
+000013a0: 6669 6e65 7279 2e75 6e69 7473 2e65 6e63  finery.units.enc
+000013b0: 6f64 696e 672e 7575 656e 6371 cc58 0600  oding.uuencq.X..
+000013c0: 0000 7773 6865 6e63 71cd 581e 0000 0072  ..wshencq.X....r
+000013d0: 6566 696e 6572 792e 756e 6974 732e 656e  efinery.units.en
+000013e0: 636f 6469 6e67 2e77 7368 656e 6371 ce58  coding.wshencq.X
+000013f0: 0300 0000 6133 7871 cf58 1a00 0000 7265  ....a3xq.X....re
+00001400: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+00001410: 6d61 7473 2e61 3378 71d0 5802 0000 0078  mats.a3xq.X....x
+00001420: 7471 d158 2100 0000 7265 6669 6e65 7279  tq.X!...refinery
+00001430: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e61  .units.formats.a
+00001440: 7263 6869 7665 2e78 7471 d258 0400 0000  rchive.xtq.X....
+00001450: 7874 377a 71d3 5823 0000 0072 6566 696e  xt7zq.X#...refin
+00001460: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+00001470: 732e 6172 6368 6976 652e 7874 377a 71d4  s.archive.xt7zq.
+00001480: 5805 0000 0078 7461 6365 71d5 5824 0000  X....xtaceq.X$..
+00001490: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000014a0: 666f 726d 6174 732e 6172 6368 6976 652e  formats.archive.
+000014b0: 7874 6163 6571 d658 0600 0000 7874 6173  xtaceq.X....xtas
+000014c0: 6172 71d7 5825 0000 0072 6566 696e 6572  arq.X%...refiner
+000014d0: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+000014e0: 6172 6368 6976 652e 7874 6173 6172 71d8  archive.xtasarq.
+000014f0: 5805 0000 0078 7463 6162 71d9 5824 0000  X....xtcabq.X$..
+00001500: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001510: 666f 726d 6174 732e 6172 6368 6976 652e  formats.archive.
+00001520: 7874 6361 6271 da58 0600 0000 7874 6370  xtcabq.X....xtcp
+00001530: 696f 71db 5825 0000 0072 6566 696e 6572  ioq.X%...refiner
+00001540: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+00001550: 6172 6368 6976 652e 7874 6370 696f 71dc  archive.xtcpioq.
+00001560: 5804 0000 0078 7467 7a71 dd58 2300 0000  X....xtgzq.X#...
+00001570: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+00001580: 6f72 6d61 7473 2e61 7263 6869 7665 2e78  ormats.archive.x
+00001590: 7467 7a71 de58 0500 0000 7874 6973 6f71  tgzq.X....xtisoq
+000015a0: df58 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
+000015b0: 6e69 7473 2e66 6f72 6d61 7473 2e61 7263  nits.formats.arc
+000015c0: 6869 7665 2e78 7469 736f 71e0 5805 0000  hive.xtisoq.X...
+000015d0: 0078 7469 7373 71e1 5824 0000 0072 6566  .xtissq.X$...ref
+000015e0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
+000015f0: 6174 732e 6172 6368 6976 652e 7874 6973  ats.archive.xtis
+00001600: 7371 e258 0600 0000 7874 6e6f 6465 71e3  sq.X....xtnodeq.
+00001610: 5825 0000 0072 6566 696e 6572 792e 756e  X%...refinery.un
+00001620: 6974 732e 666f 726d 6174 732e 6172 6368  its.formats.arch
+00001630: 6976 652e 7874 6e6f 6465 71e4 5806 0000  ive.xtnodeq.X...
+00001640: 0078 746e 7369 7371 e558 2500 0000 7265  .xtnsisq.X%...re
+00001650: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+00001660: 6d61 7473 2e61 7263 6869 7665 2e78 746e  mats.archive.xtn
+00001670: 7369 7371 e658 0500 0000 7874 7079 6971  sisq.X....xtpyiq
 00001680: e758 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
 00001690: 6e69 7473 2e66 6f72 6d61 7473 2e61 7263  nits.formats.arc
-000016a0: 6869 7665 2e78 747a 6970 71e8 5803 0000  hive.xtzipq.X...
-000016b0: 0062 6174 71e9 581a 0000 0072 6566 696e  .batq.X....refin
-000016c0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-000016d0: 732e 6261 7471 ea58 0300 0000 6373 7671  s.batq.X....csvq
-000016e0: eb58 1a00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-000016f0: 6e69 7473 2e66 6f72 6d61 7473 2e63 7376  nits.formats.csv
-00001700: 71ec 5805 0000 0064 7370 6870 71ed 5826  q.X....dsphpq.X&
-00001710: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00001720: 732e 666f 726d 6174 732e 6465 7365 7269  s.formats.deseri
-00001730: 616c 697a 655f 7068 7071 ee58 0600 0000  alize_phpq.X....
-00001740: 6465 7873 7472 71ef 581d 0000 0072 6566  dexstrq.X....ref
-00001750: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
-00001760: 6174 732e 6465 7873 7472 71f0 5806 0000  ats.dexstrq.X...
-00001770: 0078 746d 6169 6c71 f158 1c00 0000 7265  .xtmailq.X....re
-00001780: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
-00001790: 6d61 7473 2e65 6d61 696c 71f2 5804 0000  mats.emailq.X...
-000017a0: 0065 7674 7871 f358 1b00 0000 7265 6669  .evtxq.X....refi
-000017b0: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
-000017c0: 7473 2e65 7674 7871 f458 0500 0000 7661  ts.evtxq.X....va
-000017d0: 6464 7271 f558 2000 0000 7265 6669 6e65  ddrq.X ...refine
-000017e0: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
-000017f0: 2e65 7865 2e76 6164 6472 71f6 5807 0000  .exe.vaddrq.X...
-00001800: 0076 6d65 6d72 6566 71f7 5822 0000 0072  .vmemrefq.X"...r
-00001810: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00001820: 726d 6174 732e 6578 652e 766d 656d 7265  rmats.exe.vmemre
-00001830: 6671 f858 0500 0000 7673 6563 7471 f958  fq.X....vsectq.X
-00001840: 2000 0000 7265 6669 6e65 7279 2e75 6e69   ...refinery.uni
-00001850: 7473 2e66 6f72 6d61 7473 2e65 7865 2e76  ts.formats.exe.v
-00001860: 7365 6374 71fa 5805 0000 0076 736e 6970  sectq.X....vsnip
-00001870: 71fb 5820 0000 0072 6566 696e 6572 792e  q.X ...refinery.
-00001880: 756e 6974 732e 666f 726d 6174 732e 6578  units.formats.ex
-00001890: 652e 7673 6e69 7071 fc58 0600 0000 7673  e.vsnipq.X....vs
-000018a0: 7461 636b 71fd 5821 0000 0072 6566 696e  tackq.X!...refin
-000018b0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-000018c0: 732e 6578 652e 7673 7461 636b 71fe 5807  s.exe.vstackq.X.
-000018d0: 0000 0068 6578 6c6f 6164 71ff 581e 0000  ...hexloadq.X...
-000018e0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000018f0: 666f 726d 6174 732e 6865 786c 6f61 6472  formats.hexloadr
-00001900: 0001 0000 5806 0000 0078 7468 746d 6c72  ....X....xthtmlr
-00001910: 0101 0000 581b 0000 0072 6566 696e 6572  ....X....refiner
-00001920: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001930: 6874 6d6c 7202 0100 0058 0c00 0000 6874  htmlr....X....ht
-00001940: 7470 7265 7370 6f6e 7365 7203 0100 0058  tpresponser....X
-00001950: 2300 0000 7265 6669 6e65 7279 2e75 6e69  #...refinery.uni
-00001960: 7473 2e66 6f72 6d61 7473 2e68 7474 7072  ts.formats.httpr
-00001970: 6573 706f 6e73 6572 0401 0000 5804 0000  esponser....X...
-00001980: 0069 6670 7372 0501 0000 581b 0000 0072  .ifpsr....X....r
-00001990: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-000019a0: 726d 6174 732e 6966 7073 7206 0100 0058  rmats.ifpsr....X
-000019b0: 0700 0000 6966 7073 7374 7272 0701 0000  ....ifpsstrr....
-000019c0: 581e 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000019d0: 6974 732e 666f 726d 6174 732e 6966 7073  its.formats.ifps
-000019e0: 7374 7272 0801 0000 5806 0000 0064 736a  strr....X....dsj
-000019f0: 6176 6172 0901 0000 5827 0000 0072 6566  avar....X'...ref
-00001a00: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
-00001a10: 6174 732e 6a61 7661 2e64 6573 6572 6961  ats.java.deseria
-00001a20: 6c69 7a65 720a 0100 0058 0600 0000 6a76  lizer....X....jv
-00001a30: 6461 736d 720b 0100 0058 2200 0000 7265  dasmr....X"...re
-00001a40: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
-00001a50: 6d61 7473 2e6a 6176 612e 6a76 6461 736d  mats.java.jvdasm
-00001a60: 720c 0100 0058 0500 0000 6a76 7374 7272  r....X....jvstrr
-00001a70: 0d01 0000 5821 0000 0072 6566 696e 6572  ....X!...refiner
-00001a80: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001a90: 6a61 7661 2e6a 7673 7472 720e 0100 0058  java.jvstrr....X
-00001aa0: 0300 0000 786a 3072 0f01 0000 581b 0000  ....xj0r....X...
-00001ab0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00001ac0: 666f 726d 6174 732e 6a73 6f6e 7210 0100  formats.jsonr...
-00001ad0: 0058 0300 0000 786a 6c72 1101 0000 6a10  .X....xjlr....j.
-00001ae0: 0100 0058 0600 0000 7874 6a73 6f6e 7212  ...X....xtjsonr.
-00001af0: 0100 006a 1001 0000 5803 0000 006c 6e6b  ...j....X....lnk
-00001b00: 7213 0100 0058 1a00 0000 7265 6669 6e65  r....X....refine
-00001b10: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
-00001b20: 2e6c 6e6b 7214 0100 0058 0700 0000 6d73  .lnkr....X....ms
-00001b30: 6770 6163 6b72 1501 0000 581e 0000 0072  gpackr....X....r
-00001b40: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00001b50: 726d 6174 732e 6d73 6770 6163 6b72 1601  rmats.msgpackr..
-00001b60: 0000 5805 0000 0078 746d 7369 7217 0100  ..X....xtmsir...
-00001b70: 0058 1a00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00001b80: 6e69 7473 2e66 6f72 6d61 7473 2e6d 7369  nits.formats.msi
-00001b90: 7218 0100 0058 0600 0000 646f 6374 7874  r....X....doctxt
-00001ba0: 7219 0100 0058 2400 0000 7265 6669 6e65  r....X$...refine
-00001bb0: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
-00001bc0: 2e6f 6666 6963 652e 646f 6374 7874 721a  .office.doctxtr.
-00001bd0: 0100 0058 0b00 0000 6f66 6669 6365 6372  ...X....officecr
-00001be0: 7970 7472 1b01 0000 5829 0000 0072 6566  yptr....X)...ref
-00001bf0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
-00001c00: 6174 732e 6f66 6669 6365 2e6f 6666 6963  ats.office.offic
-00001c10: 6563 7279 7074 721c 0100 0058 0500 0000  ecryptr....X....
-00001c20: 7662 6170 6372 1d01 0000 5823 0000 0072  vbapcr....X#...r
-00001c30: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00001c40: 726d 6174 732e 6f66 6669 6365 2e76 6261  rmats.office.vba
-00001c50: 7063 721e 0100 0058 0600 0000 7662 6173  pcr....X....vbas
-00001c60: 7472 721f 0100 0058 2400 0000 7265 6669  trr....X$...refi
-00001c70: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
-00001c80: 7473 2e6f 6666 6963 652e 7662 6173 7472  ts.office.vbastr
-00001c90: 7220 0100 0058 0800 0000 786c 6d64 656f  r ...X....xlmdeo
-00001ca0: 6266 7221 0100 0058 2600 0000 7265 6669  bfr!...X&...refi
-00001cb0: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
-00001cc0: 7473 2e6f 6666 6963 652e 786c 6d64 656f  ts.office.xlmdeo
-00001cd0: 6266 7222 0100 0058 0500 0000 786c 7874  bfr"...X....xlxt
-00001ce0: 7272 2301 0000 5823 0000 0072 6566 696e  rr#...X#...refin
-00001cf0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00001d00: 732e 6f66 6669 6365 2e78 6c78 7472 7224  s.office.xlxtrr$
-00001d10: 0100 0058 0500 0000 7874 646f 6372 2501  ...X....xtdocr%.
-00001d20: 0000 5823 0000 0072 6566 696e 6572 792e  ..X#...refinery.
-00001d30: 756e 6974 732e 666f 726d 6174 732e 6f66  units.formats.of
-00001d40: 6669 6365 2e78 7464 6f63 7226 0100 0058  fice.xtdocr&...X
-00001d50: 0500 0000 7874 6f6e 6572 2701 0000 5823  ....xtoner'...X#
-00001d60: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00001d70: 732e 666f 726d 6174 732e 6f66 6669 6365  s.formats.office
-00001d80: 2e78 746f 6e65 7228 0100 0058 0500 0000  .xtoner(...X....
-00001d90: 7874 7274 6672 2901 0000 5823 0000 0072  xtrtfr)...X#...r
-00001da0: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00001db0: 726d 6174 732e 6f66 6669 6365 2e78 7472  rmats.office.xtr
-00001dc0: 7466 722a 0100 0058 0500 0000 7874 7662  tfr*...X....xtvb
-00001dd0: 6172 2b01 0000 5823 0000 0072 6566 696e  ar+...X#...refin
-00001de0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00001df0: 732e 6f66 6669 6365 2e78 7476 6261 722c  s.office.xtvbar,
-00001e00: 0100 0058 0400 0000 7063 6170 722d 0100  ...X....pcapr-..
-00001e10: 0058 1b00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00001e20: 6e69 7473 2e66 6f72 6d61 7473 2e70 6361  nits.formats.pca
-00001e30: 7072 2e01 0000 5809 0000 0070 6361 705f  pr....X....pcap_
-00001e40: 6874 7470 722f 0100 0058 2000 0000 7265  httpr/...X ...re
-00001e50: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
-00001e60: 6d61 7473 2e70 6361 705f 6874 7470 7230  mats.pcap_httpr0
-00001e70: 0100 0058 0500 0000 7874 7064 6672 3101  ...X....xtpdfr1.
-00001e80: 0000 581a 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00001e90: 756e 6974 732e 666f 726d 6174 732e 7064  units.formats.pd
-00001ea0: 6672 3201 0000 5806 0000 0064 6e62 6c6f  fr2...X....dnblo
-00001eb0: 6272 3301 0000 5827 0000 0072 6566 696e  br3...X'...refin
-00001ec0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00001ed0: 732e 7065 2e64 6f74 6e65 742e 646e 626c  s.pe.dotnet.dnbl
-00001ee0: 6f62 7234 0100 0058 0500 0000 646e 6366  obr4...X....dncf
-00001ef0: 7872 3501 0000 5826 0000 0072 6566 696e  xr5...X&...refin
-00001f00: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
-00001f10: 732e 7065 2e64 6f74 6e65 742e 646e 6366  s.pe.dotnet.dncf
-00001f20: 7872 3601 0000 5804 0000 0064 6e64 7372  xr6...X....dndsr
-00001f30: 3701 0000 5825 0000 0072 6566 696e 6572  7...X%...refiner
-00001f40: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
-00001f50: 7065 2e64 6f74 6e65 742e 646e 6473 7238  pe.dotnet.dndsr8
-00001f60: 0100 0058 0800 0000 646e 6669 656c 6473  ...X....dnfields
-00001f70: 7239 0100 0058 2900 0000 7265 6669 6e65  r9...X)...refine
-00001f80: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
-00001f90: 2e70 652e 646f 746e 6574 2e64 6e66 6965  .pe.dotnet.dnfie
-00001fa0: 6c64 7372 3a01 0000 5805 0000 0064 6e68  ldsr:...X....dnh
-00001fb0: 6472 723b 0100 0058 2600 0000 7265 6669  drr;...X&...refi
-00001fc0: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
-00001fd0: 7473 2e70 652e 646f 746e 6574 2e64 6e68  ts.pe.dotnet.dnh
-00001fe0: 6472 723c 0100 0058 0400 0000 646e 6d72  drr<...X....dnmr
-00001ff0: 723d 0100 0058 2500 0000 7265 6669 6e65  r=...X%...refine
-00002000: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
-00002010: 2e70 652e 646f 746e 6574 2e64 6e6d 7272  .pe.dotnet.dnmrr
-00002020: 3e01 0000 5804 0000 0064 6e72 6372 3f01  >...X....dnrcr?.
-00002030: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
-00002040: 756e 6974 732e 666f 726d 6174 732e 7065  units.formats.pe
-00002050: 2e64 6f74 6e65 742e 646e 7263 7240 0100  .dotnet.dnrcr@..
-00002060: 0058 0500 0000 646e 7374 7272 4101 0000  .X....dnstrrA...
-00002070: 5826 0000 0072 6566 696e 6572 792e 756e  X&...refinery.un
-00002080: 6974 732e 666f 726d 6174 732e 7065 2e64  its.formats.pe.d
-00002090: 6f74 6e65 742e 646e 7374 7272 4201 0000  otnet.dnstrrB...
-000020a0: 5806 0000 0070 656d 6574 6172 4301 0000  X....pemetarC...
-000020b0: 5820 0000 0072 6566 696e 6572 792e 756e  X ...refinery.un
-000020c0: 6974 732e 666f 726d 6174 732e 7065 2e70  its.formats.pe.p
-000020d0: 656d 6574 6172 4401 0000 5809 0000 0070  emetarD...X....p
-000020e0: 656f 7665 726c 6179 7245 0100 0058 2300  eoverlayrE...X#.
-000020f0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002100: 2e66 6f72 6d61 7473 2e70 652e 7065 6f76  .formats.pe.peov
-00002110: 6572 6c61 7972 4601 0000 5804 0000 0070  erlayrF...X....p
-00002120: 6572 6372 4701 0000 581e 0000 0072 6566  ercrG...X....ref
-00002130: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
-00002140: 6174 732e 7065 2e70 6572 6372 4801 0000  ats.pe.percrH...
-00002150: 5805 0000 0070 6573 6967 7249 0100 0058  X....pesigrI...X
-00002160: 1f00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00002170: 7473 2e66 6f72 6d61 7473 2e70 652e 7065  ts.formats.pe.pe
-00002180: 7369 6772 4a01 0000 5807 0000 0070 6573  sigrJ...X....pes
-00002190: 7472 6970 724b 0100 0058 2100 0000 7265  triprK...X!...re
-000021a0: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
-000021b0: 6d61 7473 2e70 652e 7065 7374 7269 7072  mats.pe.pestripr
-000021c0: 4c01 0000 5805 0000 0070 6b63 7337 724d  L...X....pkcs7rM
-000021d0: 0100 0058 1c00 0000 7265 6669 6e65 7279  ...X....refinery
-000021e0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e70  .units.formats.p
-000021f0: 6b63 7337 724e 0100 0058 0800 0000 706b  kcs7rN...X....pk
-00002200: 6373 3773 6967 724f 0100 0058 1f00 0000  cs7sigrO...X....
-00002210: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
-00002220: 6f72 6d61 7473 2e70 6b63 7337 7369 6772  ormats.pkcs7sigr
-00002230: 5001 0000 5805 0000 0073 7465 676f 7251  P...X....stegorQ
-00002240: 0100 0058 1c00 0000 7265 6669 6e65 7279  ...X....refinery
-00002250: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e73  .units.formats.s
-00002260: 7465 676f 7252 0100 0058 0700 0000 746e  tegorR...X....tn
-00002270: 6574 6d74 6d72 5301 0000 581e 0000 0072  etmtmrS...X....r
-00002280: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
-00002290: 726d 6174 732e 746e 6574 6d74 6d72 5401  rmats.tnetmtmrT.
-000022a0: 0000 5806 0000 0077 696e 7265 6772 5501  ..X....winregrU.
-000022b0: 0000 581d 0000 0072 6566 696e 6572 792e  ..X....refinery.
-000022c0: 756e 6974 732e 666f 726d 6174 732e 7769  units.formats.wi
-000022d0: 6e72 6567 7256 0100 0058 0500 0000 7874  nregrV...X....xt
-000022e0: 786d 6c72 5701 0000 581a 0000 0072 6566  xmlrW...X....ref
-000022f0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
-00002300: 6174 732e 786d 6c72 5801 0000 5803 0000  ats.xmlrX...X...
-00002310: 006e 3430 7259 0100 0058 1a00 0000 7265  .n40rY...X....re
-00002320: 6669 6e65 7279 2e75 6e69 7473 2e6d 616c  finery.units.mal
-00002330: 7761 7265 2e6e 3430 725a 0100 0058 0400  ware.n40rZ...X..
-00002340: 0000 6368 6f70 725b 0100 0058 1800 0000  ..chopr[...X....
-00002350: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
-00002360: 6574 612e 6368 6f70 725c 0100 0058 0200  eta.chopr\...X..
-00002370: 0000 636d 725d 0100 0058 1600 0000 7265  ..cmr]...X....re
-00002380: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
-00002390: 612e 636d 725e 0100 0058 0400 0000 6375  a.cmr^...X....cu
-000023a0: 6c6c 725f 0100 0058 1800 0000 7265 6669  llr_...X....refi
-000023b0: 6e65 7279 2e75 6e69 7473 2e6d 6574 612e  nery.units.meta.
-000023c0: 6375 6c6c 7260 0100 0058 0500 0000 6465  cullr`...X....de
-000023d0: 6475 7072 6101 0000 5819 0000 0072 6566  dupra...X....ref
-000023e0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
-000023f0: 2e64 6564 7570 7262 0100 0058 0300 0000  .deduprb...X....
-00002400: 6561 7472 6301 0000 5817 0000 0072 6566  eatrc...X....ref
-00002410: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
-00002420: 2e65 6174 7264 0100 0058 0200 0000 6566  .eatrd...X....ef
-00002430: 7265 0100 0058 1600 0000 7265 6669 6e65  re...X....refine
-00002440: 7279 2e75 6e69 7473 2e6d 6574 612e 6566  ry.units.meta.ef
-00002450: 7266 0100 0058 0400 0000 656d 6974 7267  rf...X....emitrg
-00002460: 0100 0058 1800 0000 7265 6669 6e65 7279  ...X....refinery
-00002470: 2e75 6e69 7473 2e6d 6574 612e 656d 6974  .units.meta.emit
-00002480: 7268 0100 0058 0500 0000 6772 6f75 7072  rh...X....groupr
-00002490: 6901 0000 5819 0000 0072 6566 696e 6572  i...X....refiner
-000024a0: 792e 756e 6974 732e 6d65 7461 2e67 726f  y.units.meta.gro
-000024b0: 7570 726a 0100 0058 0700 0000 6772 6f75  uprj...X....grou
-000024c0: 7062 7972 6b01 0000 581b 0000 0072 6566  pbyrk...X....ref
-000024d0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
-000024e0: 2e67 726f 7570 6279 726c 0100 0058 0300  .groupbyrl...X..
-000024f0: 0000 6966 6672 6d01 0000 5817 0000 0072  ..iffrm...X....r
-00002500: 6566 696e 6572 792e 756e 6974 732e 6d65  efinery.units.me
-00002510: 7461 2e69 6666 726e 0100 0058 0400 0000  ta.iffrn...X....
-00002520: 6966 6670 726f 0100 0058 1800 0000 7265  iffpro...X....re
-00002530: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
-00002540: 612e 6966 6670 7270 0100 0058 0400 0000  a.iffprp...X....
-00002550: 6966 6673 7271 0100 0058 1800 0000 7265  iffsrq...X....re
-00002560: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
-00002570: 612e 6966 6673 7272 0100 0058 0400 0000  a.iffsrr...X....
-00002580: 6966 6678 7273 0100 0058 1800 0000 7265  iffxrs...X....re
-00002590: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
-000025a0: 612e 6966 6678 7274 0100 0058 0400 0000  a.iffxrt...X....
-000025b0: 6d61 785f 7275 0100 0058 1700 0000 7265  max_ru...X....re
-000025c0: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
-000025d0: 612e 6d61 7872 7601 0000 5804 0000 006d  a.maxrv...X....m
-000025e0: 696e 5f72 7701 0000 5817 0000 0072 6566  in_rw...X....ref
-000025f0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
-00002600: 2e6d 696e 7278 0100 0058 0300 0000 6d76  .minrx...X....mv
-00002610: 6372 7901 0000 5817 0000 0072 6566 696e  cry...X....refin
-00002620: 6572 792e 756e 6974 732e 6d65 7461 2e6d  ery.units.meta.m
-00002630: 7663 727a 0100 0058 0300 0000 6d76 6772  vcrz...X....mvgr
-00002640: 7b01 0000 5817 0000 0072 6566 696e 6572  {...X....refiner
-00002650: 792e 756e 6974 732e 6d65 7461 2e6d 7667  y.units.meta.mvg
-00002660: 727c 0100 0058 0300 0000 7061 6472 7d01  r|...X....padr}.
-00002670: 0000 5817 0000 0072 6566 696e 6572 792e  ..X....refinery.
-00002680: 756e 6974 732e 6d65 7461 2e70 6164 727e  units.meta.padr~
-00002690: 0100 0058 0400 0000 7069 636b 727f 0100  ...X....pickr...
-000026a0: 0058 1800 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-000026b0: 6e69 7473 2e6d 6574 612e 7069 636b 7280  nits.meta.pickr.
-000026c0: 0100 0058 0300 0000 706f 7072 8101 0000  ...X....popr....
-000026d0: 5817 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000026e0: 6974 732e 6d65 7461 2e70 6f70 7282 0100  its.meta.popr...
-000026f0: 0058 0400 0000 7075 7368 7283 0100 0058  .X....pushr....X
-00002700: 1800 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00002710: 7473 2e6d 6574 612e 7075 7368 7284 0100  ts.meta.pushr...
-00002720: 0058 0300 0000 7075 7472 8501 0000 5817  .X....putr....X.
-00002730: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00002740: 732e 6d65 7461 2e70 7574 7286 0100 0058  s.meta.putr....X
-00002750: 0500 0000 7175 6575 6572 8701 0000 5819  ....queuer....X.
-00002760: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00002770: 732e 6d65 7461 2e71 7565 7565 7288 0100  s.meta.queuer...
-00002780: 0058 0600 0000 7265 6475 6365 7289 0100  .X....reducer...
-00002790: 0058 1a00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-000027a0: 6e69 7473 2e6d 6574 612e 7265 6475 6365  nits.meta.reduce
-000027b0: 728a 0100 0058 0500 0000 7363 6f70 6572  r....X....scoper
-000027c0: 8b01 0000 5819 0000 0072 6566 696e 6572  ....X....refiner
-000027d0: 792e 756e 6974 732e 6d65 7461 2e73 636f  y.units.meta.sco
-000027e0: 7065 728c 0100 0058 0300 0000 7365 7072  per....X....sepr
-000027f0: 8d01 0000 5817 0000 0072 6566 696e 6572  ....X....refiner
-00002800: 792e 756e 6974 732e 6d65 7461 2e73 6570  y.units.meta.sep
-00002810: 728e 0100 0058 0600 0000 736f 7274 6564  r....X....sorted
-00002820: 728f 0100 0058 1a00 0000 7265 6669 6e65  r....X....refine
-00002830: 7279 2e75 6e69 7473 2e6d 6574 612e 736f  ry.units.meta.so
-00002840: 7274 6564 7290 0100 0058 0400 0000 7377  rtedr....X....sw
-00002850: 6170 7291 0100 0058 1800 0000 7265 6669  apr....X....refi
-00002860: 6e65 7279 2e75 6e69 7473 2e6d 6574 612e  nery.units.meta.
-00002870: 7377 6170 7292 0100 0058 0900 0000 7472  swapr....X....tr
-00002880: 616e 7370 6f73 6572 9301 0000 581d 0000  ansposer....X...
-00002890: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000028a0: 6d65 7461 2e74 7261 6e73 706f 7365 7294  meta.transposer.
-000028b0: 0100 0058 0400 0000 7866 6363 7295 0100  ...X....xfccr...
-000028c0: 0058 1800 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-000028d0: 6e69 7473 2e6d 6574 612e 7866 6363 7296  nits.meta.xfccr.
-000028e0: 0100 0058 0700 0000 6175 746f 786f 7272  ...X....autoxorr
-000028f0: 9701 0000 581b 0000 0072 6566 696e 6572  ....X....refiner
-00002900: 792e 756e 6974 732e 6d69 7363 2e61 7574  y.units.misc.aut
-00002910: 6f78 6f72 7298 0100 0058 0600 0000 636f  oxorr....X....co
-00002920: 7570 6c65 7299 0100 0058 1a00 0000 7265  upler....X....re
-00002930: 6669 6e65 7279 2e75 6e69 7473 2e6d 6973  finery.units.mis
-00002940: 632e 636f 7570 6c65 729a 0100 0058 0700  c.coupler....X..
-00002950: 0000 6461 7465 6669 7872 9b01 0000 581b  ..datefixr....X.
-00002960: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00002970: 732e 6d69 7363 2e64 6174 6566 6978 729c  s.misc.datefixr.
-00002980: 0100 0058 0300 0000 6472 7072 9d01 0000  ...X....drpr....
-00002990: 5817 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000029a0: 6974 732e 6d69 7363 2e64 7270 729e 0100  its.misc.drpr...
-000029b0: 0058 0300 0000 6e6f 7072 9f01 0000 5817  .X....nopr....X.
-000029c0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-000029d0: 732e 6d69 7363 2e6e 6f70 72a0 0100 0058  s.misc.nopr....X
-000029e0: 0600 0000 7572 6c66 6978 72a1 0100 0058  ....urlfixr....X
-000029f0: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-00002a00: 7473 2e6d 6973 632e 7572 6c66 6978 72a2  ts.misc.urlfixr.
-00002a10: 0100 0058 0400 0000 786b 6579 72a3 0100  ...X....xkeyr...
-00002a20: 0058 1800 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00002a30: 6e69 7473 2e6d 6973 632e 786b 6579 72a4  nits.misc.xkeyr.
-00002a40: 0100 0058 0e00 0000 6465 6f62 5f6a 735f  ...X....deob_js_
-00002a50: 6172 7261 7973 72a5 0100 0058 2400 0000  arraysr....X$...
-00002a60: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
-00002a70: 6266 7573 6361 7469 6f6e 2e6a 732e 6172  bfuscation.js.ar
-00002a80: 7261 7973 72a6 0100 0058 0f00 0000 6465  raysr....X....de
-00002a90: 6f62 5f6a 735f 6765 7461 7474 7272 a701  ob_js_getattrr..
-00002aa0: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
-00002ab0: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
-00002ac0: 6e2e 6a73 2e67 6574 6174 7472 72a8 0100  n.js.getattrr...
-00002ad0: 0058 0e00 0000 6465 6f62 5f6a 735f 7475  .X....deob_js_tu
-00002ae0: 706c 6573 72a9 0100 0058 2400 0000 7265  plesr....X$...re
-00002af0: 6669 6e65 7279 2e75 6e69 7473 2e6f 6266  finery.units.obf
-00002b00: 7573 6361 7469 6f6e 2e6a 732e 7475 706c  uscation.js.tupl
-00002b10: 6573 72aa 0100 0058 0800 0000 6465 6f62  esr....X....deob
-00002b20: 5f70 7331 72ab 0100 0058 2200 0000 7265  _ps1r....X"...re
-00002b30: 6669 6e65 7279 2e75 6e69 7473 2e6f 6266  finery.units.obf
-00002b40: 7573 6361 7469 6f6e 2e70 7331 2e61 6c6c  uscation.ps1.all
-00002b50: 72ac 0100 0058 1100 0000 6465 6f62 5f70  r....X....deob_p
-00002b60: 7331 5f62 7261 636b 6574 7372 ad01 0000  s1_bracketsr....
-00002b70: 5827 0000 0072 6566 696e 6572 792e 756e  X'...refinery.un
-00002b80: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
-00002b90: 7073 312e 6272 6163 6b65 7473 72ae 0100  ps1.bracketsr...
-00002ba0: 0058 0e00 0000 6465 6f62 5f70 7331 5f63  .X....deob_ps1_c
-00002bb0: 6173 6573 72af 0100 0058 2400 0000 7265  asesr....X$...re
-00002bc0: 6669 6e65 7279 2e75 6e69 7473 2e6f 6266  finery.units.obf
-00002bd0: 7573 6361 7469 6f6e 2e70 7331 2e63 6173  uscation.ps1.cas
-00002be0: 6573 72b0 0100 0058 0f00 0000 6465 6f62  esr....X....deob
-00002bf0: 5f70 7331 5f63 6f6e 6361 7472 b101 0000  _ps1_concatr....
-00002c00: 5825 0000 0072 6566 696e 6572 792e 756e  X%...refinery.un
-00002c10: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
-00002c20: 7073 312e 636f 6e63 6174 72b2 0100 0058  ps1.concatr....X
-00002c30: 0f00 0000 6465 6f62 5f70 7331 5f65 7363  ....deob_ps1_esc
-00002c40: 6170 6572 b301 0000 5825 0000 0072 6566  aper....X%...ref
-00002c50: 696e 6572 792e 756e 6974 732e 6f62 6675  inery.units.obfu
-00002c60: 7363 6174 696f 6e2e 7073 312e 6573 6361  scation.ps1.esca
-00002c70: 7065 72b4 0100 0058 0f00 0000 6465 6f62  per....X....deob
-00002c80: 5f70 7331 5f66 6f72 6d61 7472 b501 0000  _ps1_formatr....
-00002c90: 5825 0000 0072 6566 696e 6572 792e 756e  X%...refinery.un
-00002ca0: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
-00002cb0: 7073 312e 666f 726d 6174 72b6 0100 0058  ps1.formatr....X
-00002cc0: 0f00 0000 6465 6f62 5f70 7331 5f69 6e76  ....deob_ps1_inv
-00002cd0: 6f6b 6572 b701 0000 5825 0000 0072 6566  oker....X%...ref
-00002ce0: 696e 6572 792e 756e 6974 732e 6f62 6675  inery.units.obfu
-00002cf0: 7363 6174 696f 6e2e 7073 312e 696e 766f  scation.ps1.invo
-00002d00: 6b65 72b8 0100 0058 0f00 0000 6465 6f62  ker....X....deob
-00002d10: 5f70 7331 5f73 6563 7374 7272 b901 0000  _ps1_secstrr....
-00002d20: 582b 0000 0072 6566 696e 6572 792e 756e  X+...refinery.un
-00002d30: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
-00002d40: 7073 312e 7365 6375 7265 7374 7269 6e67  ps1.securestring
-00002d50: 72ba 0100 0058 1600 0000 6465 6f62 5f70  r....X....deob_p
-00002d60: 7331 5f73 7472 696e 6772 6570 6c61 6365  s1_stringreplace
-00002d70: 72bb 0100 0058 2c00 0000 7265 6669 6e65  r....X,...refine
-00002d80: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
-00002d90: 7469 6f6e 2e70 7331 2e73 7472 696e 6772  tion.ps1.stringr
-00002da0: 6570 6c61 6365 72bc 0100 0058 1100 0000  eplacer....X....
-00002db0: 6465 6f62 5f70 7331 5f74 7970 6563 6173  deob_ps1_typecas
-00002dc0: 7472 bd01 0000 5827 0000 0072 6566 696e  tr....X'...refin
-00002dd0: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
-00002de0: 6174 696f 6e2e 7073 312e 7479 7065 6361  ation.ps1.typeca
-00002df0: 7374 72be 0100 0058 1000 0000 6465 6f62  str....X....deob
-00002e00: 5f70 7331 5f75 6e63 7572 6c79 72bf 0100  _ps1_uncurlyr...
-00002e10: 0058 2600 0000 7265 6669 6e65 7279 2e75  .X&...refinery.u
-00002e20: 6e69 7473 2e6f 6266 7573 6361 7469 6f6e  nits.obfuscation
-00002e30: 2e70 7331 2e75 6e63 7572 6c79 72c0 0100  .ps1.uncurlyr...
-00002e40: 0058 0800 0000 6465 6f62 5f76 6261 72c1  .X....deob_vbar.
-00002e50: 0100 0058 2200 0000 7265 6669 6e65 7279  ...X"...refinery
-00002e60: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
-00002e70: 6f6e 2e76 6261 2e61 6c6c 72c2 0100 0058  on.vba.allr....X
-00002e80: 1300 0000 6465 6f62 5f76 6261 5f61 7269  ....deob_vba_ari
-00002e90: 7468 6d65 7469 6372 c301 0000 5829 0000  thmeticr....X)..
-00002ea0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00002eb0: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
-00002ec0: 6172 6974 686d 6574 6963 72c4 0100 0058  arithmeticr....X
-00002ed0: 1100 0000 6465 6f62 5f76 6261 5f62 7261  ....deob_vba_bra
-00002ee0: 636b 6574 7372 c501 0000 5827 0000 0072  cketsr....X'...r
-00002ef0: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
-00002f00: 6675 7363 6174 696f 6e2e 7662 612e 6272  fuscation.vba.br
-00002f10: 6163 6b65 7473 72c6 0100 0058 1600 0000  acketsr....X....
-00002f20: 6465 6f62 5f76 6261 5f63 6861 725f 6675  deob_vba_char_fu
-00002f30: 6e63 7469 6f6e 72c7 0100 0058 2300 0000  nctionr....X#...
-00002f40: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
-00002f50: 6266 7573 6361 7469 6f6e 2e76 6261 2e63  bfuscation.vba.c
-00002f60: 6861 7272 c801 0000 5811 0000 0064 656f  harr....X....deo
-00002f70: 625f 7662 615f 636f 6d6d 656e 7473 72c9  b_vba_commentsr.
-00002f80: 0100 0058 2700 0000 7265 6669 6e65 7279  ...X'...refinery
-00002f90: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
-00002fa0: 6f6e 2e76 6261 2e63 6f6d 6d65 6e74 7372  on.vba.commentsr
-00002fb0: ca01 0000 580f 0000 0064 656f 625f 7662  ....X....deob_vb
-00002fc0: 615f 636f 6e63 6174 72cb 0100 0058 2500  a_concatr....X%.
-00002fd0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00002fe0: 2e6f 6266 7573 6361 7469 6f6e 2e76 6261  .obfuscation.vba
-00002ff0: 2e63 6f6e 6361 7472 cc01 0000 5812 0000  .concatr....X...
-00003000: 0064 656f 625f 7662 615f 636f 6e73 7461  .deob_vba_consta
-00003010: 6e74 7372 cd01 0000 5828 0000 0072 6566  ntsr....X(...ref
-00003020: 696e 6572 792e 756e 6974 732e 6f62 6675  inery.units.obfu
-00003030: 7363 6174 696f 6e2e 7662 612e 636f 6e73  scation.vba.cons
-00003040: 7461 6e74 7372 ce01 0000 5818 0000 0064  tantsr....X....d
-00003050: 656f 625f 7662 615f 6475 6d6d 795f 7661  eob_vba_dummy_va
-00003060: 7269 6162 6c65 7372 cf01 0000 5826 0000  riablesr....X&..
-00003070: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00003080: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
-00003090: 6475 6d6d 6965 7372 d001 0000 5816 0000  dummiesr....X...
-000030a0: 0064 656f 625f 7662 615f 7374 7269 6e67  .deob_vba_string
-000030b0: 7265 706c 6163 6572 d101 0000 582c 0000  replacer....X,..
-000030c0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-000030d0: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
-000030e0: 7374 7269 6e67 7265 706c 6163 6572 d201  stringreplacer..
-000030f0: 0000 5816 0000 0064 656f 625f 7662 615f  ..X....deob_vba_
-00003100: 7374 7269 6e67 7265 7665 7273 6572 d301  stringreverser..
-00003110: 0000 582c 0000 0072 6566 696e 6572 792e  ..X,...refinery.
-00003120: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
-00003130: 6e2e 7662 612e 7374 7269 6e67 7265 7665  n.vba.stringreve
-00003140: 7273 6572 d401 0000 5815 0000 0064 656f  rser....X....deo
-00003150: 625f 7662 615f 6368 725f 6c69 7465 7261  b_vba_chr_litera
-00003160: 6c73 72d5 0100 0058 2200 0000 7265 6669  lsr....X"...refi
-00003170: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
-00003180: 6361 7469 6f6e 2e76 6261 2e76 6261 72d6  cation.vba.vbar.
-00003190: 0100 0058 0500 0000 6361 7276 6572 d701  ...X....carver..
-000031a0: 0000 581c 0000 0072 6566 696e 6572 792e  ..X....refinery.
-000031b0: 756e 6974 732e 7061 7474 6572 6e2e 6361  units.pattern.ca
-000031c0: 7276 6572 d801 0000 5808 0000 0063 6172  rver....X....car
-000031d0: 7665 5f37 7a72 d901 0000 581f 0000 0072  ve_7zr....X....r
-000031e0: 6566 696e 6572 792e 756e 6974 732e 7061  efinery.units.pa
-000031f0: 7474 6572 6e2e 6361 7276 655f 377a 72da  ttern.carve_7zr.
-00003200: 0100 0058 0a00 0000 6361 7276 655f 6a73  ...X....carve_js
-00003210: 6f6e 72db 0100 0058 2100 0000 7265 6669  onr....X!...refi
-00003220: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
-00003230: 726e 2e63 6172 7665 5f6a 736f 6e72 dc01  rn.carve_jsonr..
-00003240: 0000 5809 0000 0063 6172 7665 5f6c 6e6b  ..X....carve_lnk
-00003250: 72dd 0100 0058 2000 0000 7265 6669 6e65  r....X ...refine
-00003260: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
-00003270: 2e63 6172 7665 5f6c 6e6b 72de 0100 0058  .carve_lnkr....X
-00003280: 0800 0000 6361 7276 655f 7065 72df 0100  ....carve_per...
-00003290: 0058 1f00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+000016a0: 6869 7665 2e78 7470 7969 71e8 5805 0000  hive.xtpyiq.X...
+000016b0: 0078 7474 6172 71e9 5824 0000 0072 6566  .xttarq.X$...ref
+000016c0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
+000016d0: 6174 732e 6172 6368 6976 652e 7874 7461  ats.archive.xtta
+000016e0: 7271 ea58 0500 0000 7874 7a69 7071 eb58  rq.X....xtzipq.X
+000016f0: 2400 0000 7265 6669 6e65 7279 2e75 6e69  $...refinery.uni
+00001700: 7473 2e66 6f72 6d61 7473 2e61 7263 6869  ts.formats.archi
+00001710: 7665 2e78 747a 6970 71ec 5803 0000 0062  ve.xtzipq.X....b
+00001720: 6174 71ed 581a 0000 0072 6566 696e 6572  atq.X....refiner
+00001730: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+00001740: 6261 7471 ee58 0300 0000 6373 7671 ef58  batq.X....csvq.X
+00001750: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00001760: 7473 2e66 6f72 6d61 7473 2e63 7376 71f0  ts.formats.csvq.
+00001770: 5805 0000 0064 7370 6870 71f1 5826 0000  X....dsphpq.X&..
+00001780: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001790: 666f 726d 6174 732e 6465 7365 7269 616c  formats.deserial
+000017a0: 697a 655f 7068 7071 f258 0600 0000 6465  ize_phpq.X....de
+000017b0: 7873 7472 71f3 581d 0000 0072 6566 696e  xstrq.X....refin
+000017c0: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+000017d0: 732e 6465 7873 7472 71f4 5806 0000 0078  s.dexstrq.X....x
+000017e0: 746d 6169 6c71 f558 1c00 0000 7265 6669  tmailq.X....refi
+000017f0: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
+00001800: 7473 2e65 6d61 696c 71f6 5804 0000 0065  ts.emailq.X....e
+00001810: 7674 7871 f758 1b00 0000 7265 6669 6e65  vtxq.X....refine
+00001820: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
+00001830: 2e65 7674 7871 f858 0500 0000 7661 6464  .evtxq.X....vadd
+00001840: 7271 f958 2000 0000 7265 6669 6e65 7279  rq.X ...refinery
+00001850: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e65  .units.formats.e
+00001860: 7865 2e76 6164 6472 71fa 5807 0000 0076  xe.vaddrq.X....v
+00001870: 6d65 6d72 6566 71fb 5822 0000 0072 6566  memrefq.X"...ref
+00001880: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
+00001890: 6174 732e 6578 652e 766d 656d 7265 6671  ats.exe.vmemrefq
+000018a0: fc58 0500 0000 7673 6563 7471 fd58 2000  .X....vsectq.X .
+000018b0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000018c0: 2e66 6f72 6d61 7473 2e65 7865 2e76 7365  .formats.exe.vse
+000018d0: 6374 71fe 5805 0000 0076 736e 6970 71ff  ctq.X....vsnipq.
+000018e0: 5820 0000 0072 6566 696e 6572 792e 756e  X ...refinery.un
+000018f0: 6974 732e 666f 726d 6174 732e 6578 652e  its.formats.exe.
+00001900: 7673 6e69 7072 0001 0000 5806 0000 0076  vsnipr....X....v
+00001910: 7374 6163 6b72 0101 0000 5821 0000 0072  stackr....X!...r
+00001920: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00001930: 726d 6174 732e 6578 652e 7673 7461 636b  rmats.exe.vstack
+00001940: 7202 0100 0058 0700 0000 6865 786c 6f61  r....X....hexloa
+00001950: 6472 0301 0000 581e 0000 0072 6566 696e  dr....X....refin
+00001960: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+00001970: 732e 6865 786c 6f61 6472 0401 0000 5806  s.hexloadr....X.
+00001980: 0000 0078 7468 746d 6c72 0501 0000 581b  ...xthtmlr....X.
+00001990: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000019a0: 732e 666f 726d 6174 732e 6874 6d6c 7206  s.formats.htmlr.
+000019b0: 0100 0058 0c00 0000 6874 7470 7265 7370  ...X....httpresp
+000019c0: 6f6e 7365 7207 0100 0058 2300 0000 7265  onser....X#...re
+000019d0: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+000019e0: 6d61 7473 2e68 7474 7072 6573 706f 6e73  mats.httprespons
+000019f0: 6572 0801 0000 5804 0000 0069 6670 7372  er....X....ifpsr
+00001a00: 0901 0000 581b 0000 0072 6566 696e 6572  ....X....refiner
+00001a10: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+00001a20: 6966 7073 720a 0100 0058 0700 0000 6966  ifpsr....X....if
+00001a30: 7073 7374 7272 0b01 0000 581e 0000 0072  psstrr....X....r
+00001a40: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00001a50: 726d 6174 732e 6966 7073 7374 7272 0c01  rmats.ifpsstrr..
+00001a60: 0000 5806 0000 0064 736a 6176 6172 0d01  ..X....dsjavar..
+00001a70: 0000 5827 0000 0072 6566 696e 6572 792e  ..X'...refinery.
+00001a80: 756e 6974 732e 666f 726d 6174 732e 6a61  units.formats.ja
+00001a90: 7661 2e64 6573 6572 6961 6c69 7a65 720e  va.deserializer.
+00001aa0: 0100 0058 0600 0000 6a76 6461 736d 720f  ...X....jvdasmr.
+00001ab0: 0100 0058 2200 0000 7265 6669 6e65 7279  ...X"...refinery
+00001ac0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e6a  .units.formats.j
+00001ad0: 6176 612e 6a76 6461 736d 7210 0100 0058  ava.jvdasmr....X
+00001ae0: 0500 0000 6a76 7374 7272 1101 0000 5821  ....jvstrr....X!
+00001af0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00001b00: 732e 666f 726d 6174 732e 6a61 7661 2e6a  s.formats.java.j
+00001b10: 7673 7472 7212 0100 0058 0300 0000 786a  vstrr....X....xj
+00001b20: 3072 1301 0000 581b 0000 0072 6566 696e  0r....X....refin
+00001b30: 6572 792e 756e 6974 732e 666f 726d 6174  ery.units.format
+00001b40: 732e 6a73 6f6e 7214 0100 0058 0300 0000  s.jsonr....X....
+00001b50: 786a 6c72 1501 0000 6a14 0100 0058 0600  xjlr....j....X..
+00001b60: 0000 7874 6a73 6f6e 7216 0100 006a 1401  ..xtjsonr....j..
+00001b70: 0000 5803 0000 006c 6e6b 7217 0100 0058  ..X....lnkr....X
+00001b80: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00001b90: 7473 2e66 6f72 6d61 7473 2e6c 6e6b 7218  ts.formats.lnkr.
+00001ba0: 0100 0058 0700 0000 6d73 6770 6163 6b72  ...X....msgpackr
+00001bb0: 1901 0000 581e 0000 0072 6566 696e 6572  ....X....refiner
+00001bc0: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+00001bd0: 6d73 6770 6163 6b72 1a01 0000 5805 0000  msgpackr....X...
+00001be0: 0078 746d 7369 721b 0100 0058 1a00 0000  .xtmsir....X....
+00001bf0: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+00001c00: 6f72 6d61 7473 2e6d 7369 721c 0100 0058  ormats.msir....X
+00001c10: 0600 0000 646f 6374 7874 721d 0100 0058  ....doctxtr....X
+00001c20: 2400 0000 7265 6669 6e65 7279 2e75 6e69  $...refinery.uni
+00001c30: 7473 2e66 6f72 6d61 7473 2e6f 6666 6963  ts.formats.offic
+00001c40: 652e 646f 6374 7874 721e 0100 0058 0b00  e.doctxtr....X..
+00001c50: 0000 6f66 6669 6365 6372 7970 7472 1f01  ..officecryptr..
+00001c60: 0000 5829 0000 0072 6566 696e 6572 792e  ..X)...refinery.
+00001c70: 756e 6974 732e 666f 726d 6174 732e 6f66  units.formats.of
+00001c80: 6669 6365 2e6f 6666 6963 6563 7279 7074  fice.officecrypt
+00001c90: 7220 0100 0058 0500 0000 7662 6170 6372  r ...X....vbapcr
+00001ca0: 2101 0000 5823 0000 0072 6566 696e 6572  !...X#...refiner
+00001cb0: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+00001cc0: 6f66 6669 6365 2e76 6261 7063 7222 0100  office.vbapcr"..
+00001cd0: 0058 0600 0000 7662 6173 7472 7223 0100  .X....vbastrr#..
+00001ce0: 0058 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
+00001cf0: 6e69 7473 2e66 6f72 6d61 7473 2e6f 6666  nits.formats.off
+00001d00: 6963 652e 7662 6173 7472 7224 0100 0058  ice.vbastrr$...X
+00001d10: 0800 0000 786c 6d64 656f 6266 7225 0100  ....xlmdeobfr%..
+00001d20: 0058 2600 0000 7265 6669 6e65 7279 2e75  .X&...refinery.u
+00001d30: 6e69 7473 2e66 6f72 6d61 7473 2e6f 6666  nits.formats.off
+00001d40: 6963 652e 786c 6d64 656f 6266 7226 0100  ice.xlmdeobfr&..
+00001d50: 0058 0500 0000 786c 7874 7272 2701 0000  .X....xlxtrr'...
+00001d60: 5823 0000 0072 6566 696e 6572 792e 756e  X#...refinery.un
+00001d70: 6974 732e 666f 726d 6174 732e 6f66 6669  its.formats.offi
+00001d80: 6365 2e78 6c78 7472 7228 0100 0058 0500  ce.xlxtrr(...X..
+00001d90: 0000 7874 646f 6372 2901 0000 5823 0000  ..xtdocr)...X#..
+00001da0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001db0: 666f 726d 6174 732e 6f66 6669 6365 2e78  formats.office.x
+00001dc0: 7464 6f63 722a 0100 0058 0500 0000 7874  tdocr*...X....xt
+00001dd0: 6f6e 6572 2b01 0000 5823 0000 0072 6566  oner+...X#...ref
+00001de0: 696e 6572 792e 756e 6974 732e 666f 726d  inery.units.form
+00001df0: 6174 732e 6f66 6669 6365 2e78 746f 6e65  ats.office.xtone
+00001e00: 722c 0100 0058 0500 0000 7874 7274 6672  r,...X....xtrtfr
+00001e10: 2d01 0000 5823 0000 0072 6566 696e 6572  -...X#...refiner
+00001e20: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+00001e30: 6f66 6669 6365 2e78 7472 7466 722e 0100  office.xtrtfr...
+00001e40: 0058 0500 0000 7874 7662 6172 2f01 0000  .X....xtvbar/...
+00001e50: 5823 0000 0072 6566 696e 6572 792e 756e  X#...refinery.un
+00001e60: 6974 732e 666f 726d 6174 732e 6f66 6669  its.formats.offi
+00001e70: 6365 2e78 7476 6261 7230 0100 0058 0400  ce.xtvbar0...X..
+00001e80: 0000 7063 6170 7231 0100 0058 1b00 0000  ..pcapr1...X....
+00001e90: 7265 6669 6e65 7279 2e75 6e69 7473 2e66  refinery.units.f
+00001ea0: 6f72 6d61 7473 2e70 6361 7072 3201 0000  ormats.pcapr2...
+00001eb0: 5809 0000 0070 6361 705f 6874 7470 7233  X....pcap_httpr3
+00001ec0: 0100 0058 2000 0000 7265 6669 6e65 7279  ...X ...refinery
+00001ed0: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e70  .units.formats.p
+00001ee0: 6361 705f 6874 7470 7234 0100 0058 0500  cap_httpr4...X..
+00001ef0: 0000 7874 7064 6672 3501 0000 581a 0000  ..xtpdfr5...X...
+00001f00: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00001f10: 666f 726d 6174 732e 7064 6672 3601 0000  formats.pdfr6...
+00001f20: 5806 0000 0064 6e62 6c6f 6272 3701 0000  X....dnblobr7...
+00001f30: 5827 0000 0072 6566 696e 6572 792e 756e  X'...refinery.un
+00001f40: 6974 732e 666f 726d 6174 732e 7065 2e64  its.formats.pe.d
+00001f50: 6f74 6e65 742e 646e 626c 6f62 7238 0100  otnet.dnblobr8..
+00001f60: 0058 0500 0000 646e 6366 7872 3901 0000  .X....dncfxr9...
+00001f70: 5826 0000 0072 6566 696e 6572 792e 756e  X&...refinery.un
+00001f80: 6974 732e 666f 726d 6174 732e 7065 2e64  its.formats.pe.d
+00001f90: 6f74 6e65 742e 646e 6366 7872 3a01 0000  otnet.dncfxr:...
+00001fa0: 5804 0000 0064 6e64 7372 3b01 0000 5825  X....dndsr;...X%
+00001fb0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00001fc0: 732e 666f 726d 6174 732e 7065 2e64 6f74  s.formats.pe.dot
+00001fd0: 6e65 742e 646e 6473 723c 0100 0058 0800  net.dndsr<...X..
+00001fe0: 0000 646e 6669 656c 6473 723d 0100 0058  ..dnfieldsr=...X
+00001ff0: 2900 0000 7265 6669 6e65 7279 2e75 6e69  )...refinery.uni
+00002000: 7473 2e66 6f72 6d61 7473 2e70 652e 646f  ts.formats.pe.do
+00002010: 746e 6574 2e64 6e66 6965 6c64 7372 3e01  tnet.dnfieldsr>.
+00002020: 0000 5805 0000 0064 6e68 6472 723f 0100  ..X....dnhdrr?..
+00002030: 0058 2600 0000 7265 6669 6e65 7279 2e75  .X&...refinery.u
+00002040: 6e69 7473 2e66 6f72 6d61 7473 2e70 652e  nits.formats.pe.
+00002050: 646f 746e 6574 2e64 6e68 6472 7240 0100  dotnet.dnhdrr@..
+00002060: 0058 0400 0000 646e 6d72 7241 0100 0058  .X....dnmrrA...X
+00002070: 2500 0000 7265 6669 6e65 7279 2e75 6e69  %...refinery.uni
+00002080: 7473 2e66 6f72 6d61 7473 2e70 652e 646f  ts.formats.pe.do
+00002090: 746e 6574 2e64 6e6d 7272 4201 0000 5804  tnet.dnmrrB...X.
+000020a0: 0000 0064 6e72 6372 4301 0000 5825 0000  ...dnrcrC...X%..
+000020b0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000020c0: 666f 726d 6174 732e 7065 2e64 6f74 6e65  formats.pe.dotne
+000020d0: 742e 646e 7263 7244 0100 0058 0500 0000  t.dnrcrD...X....
+000020e0: 646e 7374 7272 4501 0000 5826 0000 0072  dnstrrE...X&...r
+000020f0: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00002100: 726d 6174 732e 7065 2e64 6f74 6e65 742e  rmats.pe.dotnet.
+00002110: 646e 7374 7272 4601 0000 5806 0000 0070  dnstrrF...X....p
+00002120: 656d 6574 6172 4701 0000 5820 0000 0072  emetarG...X ...r
+00002130: 6566 696e 6572 792e 756e 6974 732e 666f  efinery.units.fo
+00002140: 726d 6174 732e 7065 2e70 656d 6574 6172  rmats.pe.pemetar
+00002150: 4801 0000 5809 0000 0070 656f 7665 726c  H...X....peoverl
+00002160: 6179 7249 0100 0058 2300 0000 7265 6669  ayrI...X#...refi
+00002170: 6e65 7279 2e75 6e69 7473 2e66 6f72 6d61  nery.units.forma
+00002180: 7473 2e70 652e 7065 6f76 6572 6c61 7972  ts.pe.peoverlayr
+00002190: 4a01 0000 5804 0000 0070 6572 6372 4b01  J...X....percrK.
+000021a0: 0000 581e 0000 0072 6566 696e 6572 792e  ..X....refinery.
+000021b0: 756e 6974 732e 666f 726d 6174 732e 7065  units.formats.pe
+000021c0: 2e70 6572 6372 4c01 0000 5805 0000 0070  .percrL...X....p
+000021d0: 6573 6967 724d 0100 0058 1f00 0000 7265  esigrM...X....re
+000021e0: 6669 6e65 7279 2e75 6e69 7473 2e66 6f72  finery.units.for
+000021f0: 6d61 7473 2e70 652e 7065 7369 6772 4e01  mats.pe.pesigrN.
+00002200: 0000 5807 0000 0070 6573 7472 6970 724f  ..X....pestriprO
+00002210: 0100 0058 2100 0000 7265 6669 6e65 7279  ...X!...refinery
+00002220: 2e75 6e69 7473 2e66 6f72 6d61 7473 2e70  .units.formats.p
+00002230: 652e 7065 7374 7269 7072 5001 0000 5805  e.pestriprP...X.
+00002240: 0000 0070 6b63 7337 7251 0100 0058 1c00  ...pkcs7rQ...X..
+00002250: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00002260: 2e66 6f72 6d61 7473 2e70 6b63 7337 7252  .formats.pkcs7rR
+00002270: 0100 0058 0800 0000 706b 6373 3773 6967  ...X....pkcs7sig
+00002280: 7253 0100 0058 1f00 0000 7265 6669 6e65  rS...X....refine
+00002290: 7279 2e75 6e69 7473 2e66 6f72 6d61 7473  ry.units.formats
+000022a0: 2e70 6b63 7337 7369 6772 5401 0000 5805  .pkcs7sigrT...X.
+000022b0: 0000 0073 7465 676f 7255 0100 0058 1c00  ...stegorU...X..
+000022c0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000022d0: 2e66 6f72 6d61 7473 2e73 7465 676f 7256  .formats.stegorV
+000022e0: 0100 0058 0700 0000 746e 6574 6d74 6d72  ...X....tnetmtmr
+000022f0: 5701 0000 581e 0000 0072 6566 696e 6572  W...X....refiner
+00002300: 792e 756e 6974 732e 666f 726d 6174 732e  y.units.formats.
+00002310: 746e 6574 6d74 6d72 5801 0000 5806 0000  tnetmtmrX...X...
+00002320: 0077 696e 7265 6772 5901 0000 581d 0000  .winregrY...X...
+00002330: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00002340: 666f 726d 6174 732e 7769 6e72 6567 725a  formats.winregrZ
+00002350: 0100 0058 0500 0000 7874 786d 6c72 5b01  ...X....xtxmlr[.
+00002360: 0000 581a 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00002370: 756e 6974 732e 666f 726d 6174 732e 786d  units.formats.xm
+00002380: 6c72 5c01 0000 5803 0000 006e 3430 725d  lr\...X....n40r]
+00002390: 0100 0058 1a00 0000 7265 6669 6e65 7279  ...X....refinery
+000023a0: 2e75 6e69 7473 2e6d 616c 7761 7265 2e6e  .units.malware.n
+000023b0: 3430 725e 0100 0058 0400 0000 6368 6f70  40r^...X....chop
+000023c0: 725f 0100 0058 1800 0000 7265 6669 6e65  r_...X....refine
+000023d0: 7279 2e75 6e69 7473 2e6d 6574 612e 6368  ry.units.meta.ch
+000023e0: 6f70 7260 0100 0058 0200 0000 636d 7261  opr`...X....cmra
+000023f0: 0100 0058 1600 0000 7265 6669 6e65 7279  ...X....refinery
+00002400: 2e75 6e69 7473 2e6d 6574 612e 636d 7262  .units.meta.cmrb
+00002410: 0100 0058 0400 0000 6375 6c6c 7263 0100  ...X....cullrc..
+00002420: 0058 1800 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00002430: 6e69 7473 2e6d 6574 612e 6375 6c6c 7264  nits.meta.cullrd
+00002440: 0100 0058 0500 0000 6465 6475 7072 6501  ...X....dedupre.
+00002450: 0000 5819 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00002460: 756e 6974 732e 6d65 7461 2e64 6564 7570  units.meta.dedup
+00002470: 7266 0100 0058 0300 0000 6561 7472 6701  rf...X....eatrg.
+00002480: 0000 5817 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00002490: 756e 6974 732e 6d65 7461 2e65 6174 7268  units.meta.eatrh
+000024a0: 0100 0058 0200 0000 6566 7269 0100 0058  ...X....efri...X
+000024b0: 1600 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+000024c0: 7473 2e6d 6574 612e 6566 726a 0100 0058  ts.meta.efrj...X
+000024d0: 0400 0000 656d 6974 726b 0100 0058 1800  ....emitrk...X..
+000024e0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000024f0: 2e6d 6574 612e 656d 6974 726c 0100 0058  .meta.emitrl...X
+00002500: 0500 0000 6772 6f75 7072 6d01 0000 5819  ....grouprm...X.
+00002510: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002520: 732e 6d65 7461 2e67 726f 7570 726e 0100  s.meta.grouprn..
+00002530: 0058 0700 0000 6772 6f75 7062 7972 6f01  .X....groupbyro.
+00002540: 0000 581b 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00002550: 756e 6974 732e 6d65 7461 2e67 726f 7570  units.meta.group
+00002560: 6279 7270 0100 0058 0300 0000 6966 6672  byrp...X....iffr
+00002570: 7101 0000 5817 0000 0072 6566 696e 6572  q...X....refiner
+00002580: 792e 756e 6974 732e 6d65 7461 2e69 6666  y.units.meta.iff
+00002590: 7272 0100 0058 0400 0000 6966 6670 7273  rr...X....iffprs
+000025a0: 0100 0058 1800 0000 7265 6669 6e65 7279  ...X....refinery
+000025b0: 2e75 6e69 7473 2e6d 6574 612e 6966 6670  .units.meta.iffp
+000025c0: 7274 0100 0058 0400 0000 6966 6673 7275  rt...X....iffsru
+000025d0: 0100 0058 1800 0000 7265 6669 6e65 7279  ...X....refinery
+000025e0: 2e75 6e69 7473 2e6d 6574 612e 6966 6673  .units.meta.iffs
+000025f0: 7276 0100 0058 0400 0000 6966 6678 7277  rv...X....iffxrw
+00002600: 0100 0058 1800 0000 7265 6669 6e65 7279  ...X....refinery
+00002610: 2e75 6e69 7473 2e6d 6574 612e 6966 6678  .units.meta.iffx
+00002620: 7278 0100 0058 0400 0000 6d61 785f 7279  rx...X....max_ry
+00002630: 0100 0058 1700 0000 7265 6669 6e65 7279  ...X....refinery
+00002640: 2e75 6e69 7473 2e6d 6574 612e 6d61 7872  .units.meta.maxr
+00002650: 7a01 0000 5804 0000 006d 696e 5f72 7b01  z...X....min_r{.
+00002660: 0000 5817 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00002670: 756e 6974 732e 6d65 7461 2e6d 696e 727c  units.meta.minr|
+00002680: 0100 0058 0300 0000 6d76 6372 7d01 0000  ...X....mvcr}...
+00002690: 5817 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000026a0: 6974 732e 6d65 7461 2e6d 7663 727e 0100  its.meta.mvcr~..
+000026b0: 0058 0300 0000 6d76 6772 7f01 0000 5817  .X....mvgr....X.
+000026c0: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+000026d0: 732e 6d65 7461 2e6d 7667 7280 0100 0058  s.meta.mvgr....X
+000026e0: 0300 0000 7061 6472 8101 0000 5817 0000  ....padr....X...
+000026f0: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00002700: 6d65 7461 2e70 6164 7282 0100 0058 0400  meta.padr....X..
+00002710: 0000 7069 636b 7283 0100 0058 1800 0000  ..pickr....X....
+00002720: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
+00002730: 6574 612e 7069 636b 7284 0100 0058 0300  eta.pickr....X..
+00002740: 0000 706f 7072 8501 0000 5817 0000 0072  ..popr....X....r
+00002750: 6566 696e 6572 792e 756e 6974 732e 6d65  efinery.units.me
+00002760: 7461 2e70 6f70 7286 0100 0058 0400 0000  ta.popr....X....
+00002770: 7075 7368 7287 0100 0058 1800 0000 7265  pushr....X....re
+00002780: 6669 6e65 7279 2e75 6e69 7473 2e6d 6574  finery.units.met
+00002790: 612e 7075 7368 7288 0100 0058 0300 0000  a.pushr....X....
+000027a0: 7075 7472 8901 0000 5817 0000 0072 6566  putr....X....ref
+000027b0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
+000027c0: 2e70 7574 728a 0100 0058 0500 0000 7175  .putr....X....qu
+000027d0: 6575 6572 8b01 0000 5819 0000 0072 6566  euer....X....ref
+000027e0: 696e 6572 792e 756e 6974 732e 6d65 7461  inery.units.meta
+000027f0: 2e71 7565 7565 728c 0100 0058 0600 0000  .queuer....X....
+00002800: 7265 6475 6365 728d 0100 0058 1a00 0000  reducer....X....
+00002810: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
+00002820: 6574 612e 7265 6475 6365 728e 0100 0058  eta.reducer....X
+00002830: 0500 0000 7363 6f70 6572 8f01 0000 5819  ....scoper....X.
+00002840: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002850: 732e 6d65 7461 2e73 636f 7065 7290 0100  s.meta.scoper...
+00002860: 0058 0300 0000 7365 7072 9101 0000 5817  .X....sepr....X.
+00002870: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002880: 732e 6d65 7461 2e73 6570 7292 0100 0058  s.meta.sepr....X
+00002890: 0600 0000 736f 7274 6564 7293 0100 0058  ....sortedr....X
+000028a0: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+000028b0: 7473 2e6d 6574 612e 736f 7274 6564 7294  ts.meta.sortedr.
+000028c0: 0100 0058 0400 0000 7377 6170 7295 0100  ...X....swapr...
+000028d0: 0058 1800 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+000028e0: 6e69 7473 2e6d 6574 612e 7377 6170 7296  nits.meta.swapr.
+000028f0: 0100 0058 0900 0000 7472 616e 7370 6f73  ...X....transpos
+00002900: 6572 9701 0000 581d 0000 0072 6566 696e  er....X....refin
+00002910: 6572 792e 756e 6974 732e 6d65 7461 2e74  ery.units.meta.t
+00002920: 7261 6e73 706f 7365 7298 0100 0058 0400  ransposer....X..
+00002930: 0000 7866 6363 7299 0100 0058 1800 0000  ..xfccr....X....
+00002940: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
+00002950: 6574 612e 7866 6363 729a 0100 0058 0700  eta.xfccr....X..
+00002960: 0000 6175 746f 786f 7272 9b01 0000 581b  ..autoxorr....X.
+00002970: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00002980: 732e 6d69 7363 2e61 7574 6f78 6f72 729c  s.misc.autoxorr.
+00002990: 0100 0058 0600 0000 636f 7570 6c65 729d  ...X....coupler.
+000029a0: 0100 0058 1a00 0000 7265 6669 6e65 7279  ...X....refinery
+000029b0: 2e75 6e69 7473 2e6d 6973 632e 636f 7570  .units.misc.coup
+000029c0: 6c65 729e 0100 0058 0700 0000 6461 7465  ler....X....date
+000029d0: 6669 7872 9f01 0000 581b 0000 0072 6566  fixr....X....ref
+000029e0: 696e 6572 792e 756e 6974 732e 6d69 7363  inery.units.misc
+000029f0: 2e64 6174 6566 6978 72a0 0100 0058 0300  .datefixr....X..
+00002a00: 0000 6472 7072 a101 0000 5817 0000 0072  ..drpr....X....r
+00002a10: 6566 696e 6572 792e 756e 6974 732e 6d69  efinery.units.mi
+00002a20: 7363 2e64 7270 72a2 0100 0058 0300 0000  sc.drpr....X....
+00002a30: 6e6f 7072 a301 0000 5817 0000 0072 6566  nopr....X....ref
+00002a40: 696e 6572 792e 756e 6974 732e 6d69 7363  inery.units.misc
+00002a50: 2e6e 6f70 72a4 0100 0058 0600 0000 7572  .nopr....X....ur
+00002a60: 6c66 6978 72a5 0100 0058 1a00 0000 7265  lfixr....X....re
+00002a70: 6669 6e65 7279 2e75 6e69 7473 2e6d 6973  finery.units.mis
+00002a80: 632e 7572 6c66 6978 72a6 0100 0058 0400  c.urlfixr....X..
+00002a90: 0000 786b 6579 72a7 0100 0058 1800 0000  ..xkeyr....X....
+00002aa0: 7265 6669 6e65 7279 2e75 6e69 7473 2e6d  refinery.units.m
+00002ab0: 6973 632e 786b 6579 72a8 0100 0058 0e00  isc.xkeyr....X..
+00002ac0: 0000 6465 6f62 5f6a 735f 6172 7261 7973  ..deob_js_arrays
+00002ad0: 72a9 0100 0058 2400 0000 7265 6669 6e65  r....X$...refine
+00002ae0: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
+00002af0: 7469 6f6e 2e6a 732e 6172 7261 7973 72aa  tion.js.arraysr.
+00002b00: 0100 0058 0f00 0000 6465 6f62 5f6a 735f  ...X....deob_js_
+00002b10: 6765 7461 7474 7272 ab01 0000 5825 0000  getattrr....X%..
+00002b20: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00002b30: 6f62 6675 7363 6174 696f 6e2e 6a73 2e67  obfuscation.js.g
+00002b40: 6574 6174 7472 72ac 0100 0058 0e00 0000  etattrr....X....
+00002b50: 6465 6f62 5f6a 735f 7475 706c 6573 72ad  deob_js_tuplesr.
+00002b60: 0100 0058 2400 0000 7265 6669 6e65 7279  ...X$...refinery
+00002b70: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
+00002b80: 6f6e 2e6a 732e 7475 706c 6573 72ae 0100  on.js.tuplesr...
+00002b90: 0058 0800 0000 6465 6f62 5f70 7331 72af  .X....deob_ps1r.
+00002ba0: 0100 0058 2200 0000 7265 6669 6e65 7279  ...X"...refinery
+00002bb0: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
+00002bc0: 6f6e 2e70 7331 2e61 6c6c 72b0 0100 0058  on.ps1.allr....X
+00002bd0: 1100 0000 6465 6f62 5f70 7331 5f62 7261  ....deob_ps1_bra
+00002be0: 636b 6574 7372 b101 0000 5827 0000 0072  cketsr....X'...r
+00002bf0: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
+00002c00: 6675 7363 6174 696f 6e2e 7073 312e 6272  fuscation.ps1.br
+00002c10: 6163 6b65 7473 72b2 0100 0058 0e00 0000  acketsr....X....
+00002c20: 6465 6f62 5f70 7331 5f63 6173 6573 72b3  deob_ps1_casesr.
+00002c30: 0100 0058 2400 0000 7265 6669 6e65 7279  ...X$...refinery
+00002c40: 2e75 6e69 7473 2e6f 6266 7573 6361 7469  .units.obfuscati
+00002c50: 6f6e 2e70 7331 2e63 6173 6573 72b4 0100  on.ps1.casesr...
+00002c60: 0058 0f00 0000 6465 6f62 5f70 7331 5f63  .X....deob_ps1_c
+00002c70: 6f6e 6361 7472 b501 0000 5825 0000 0072  oncatr....X%...r
+00002c80: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
+00002c90: 6675 7363 6174 696f 6e2e 7073 312e 636f  fuscation.ps1.co
+00002ca0: 6e63 6174 72b6 0100 0058 0f00 0000 6465  ncatr....X....de
+00002cb0: 6f62 5f70 7331 5f65 7363 6170 6572 b701  ob_ps1_escaper..
+00002cc0: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
+00002cd0: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
+00002ce0: 6e2e 7073 312e 6573 6361 7065 72b8 0100  n.ps1.escaper...
+00002cf0: 0058 0f00 0000 6465 6f62 5f70 7331 5f66  .X....deob_ps1_f
+00002d00: 6f72 6d61 7472 b901 0000 5825 0000 0072  ormatr....X%...r
+00002d10: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
+00002d20: 6675 7363 6174 696f 6e2e 7073 312e 666f  fuscation.ps1.fo
+00002d30: 726d 6174 72ba 0100 0058 0f00 0000 6465  rmatr....X....de
+00002d40: 6f62 5f70 7331 5f69 6e76 6f6b 6572 bb01  ob_ps1_invoker..
+00002d50: 0000 5825 0000 0072 6566 696e 6572 792e  ..X%...refinery.
+00002d60: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
+00002d70: 6e2e 7073 312e 696e 766f 6b65 72bc 0100  n.ps1.invoker...
+00002d80: 0058 0f00 0000 6465 6f62 5f70 7331 5f73  .X....deob_ps1_s
+00002d90: 6563 7374 7272 bd01 0000 582b 0000 0072  ecstrr....X+...r
+00002da0: 6566 696e 6572 792e 756e 6974 732e 6f62  efinery.units.ob
+00002db0: 6675 7363 6174 696f 6e2e 7073 312e 7365  fuscation.ps1.se
+00002dc0: 6375 7265 7374 7269 6e67 72be 0100 0058  curestringr....X
+00002dd0: 1600 0000 6465 6f62 5f70 7331 5f73 7472  ....deob_ps1_str
+00002de0: 696e 6772 6570 6c61 6365 72bf 0100 0058  ingreplacer....X
+00002df0: 2c00 0000 7265 6669 6e65 7279 2e75 6e69  ,...refinery.uni
+00002e00: 7473 2e6f 6266 7573 6361 7469 6f6e 2e70  ts.obfuscation.p
+00002e10: 7331 2e73 7472 696e 6772 6570 6c61 6365  s1.stringreplace
+00002e20: 72c0 0100 0058 1100 0000 6465 6f62 5f70  r....X....deob_p
+00002e30: 7331 5f74 7970 6563 6173 7472 c101 0000  s1_typecastr....
+00002e40: 5827 0000 0072 6566 696e 6572 792e 756e  X'...refinery.un
+00002e50: 6974 732e 6f62 6675 7363 6174 696f 6e2e  its.obfuscation.
+00002e60: 7073 312e 7479 7065 6361 7374 72c2 0100  ps1.typecastr...
+00002e70: 0058 1000 0000 6465 6f62 5f70 7331 5f75  .X....deob_ps1_u
+00002e80: 6e63 7572 6c79 72c3 0100 0058 2600 0000  ncurlyr....X&...
+00002e90: 7265 6669 6e65 7279 2e75 6e69 7473 2e6f  refinery.units.o
+00002ea0: 6266 7573 6361 7469 6f6e 2e70 7331 2e75  bfuscation.ps1.u
+00002eb0: 6e63 7572 6c79 72c4 0100 0058 0800 0000  ncurlyr....X....
+00002ec0: 6465 6f62 5f76 6261 72c5 0100 0058 2200  deob_vbar....X".
+00002ed0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00002ee0: 2e6f 6266 7573 6361 7469 6f6e 2e76 6261  .obfuscation.vba
+00002ef0: 2e61 6c6c 72c6 0100 0058 1300 0000 6465  .allr....X....de
+00002f00: 6f62 5f76 6261 5f61 7269 7468 6d65 7469  ob_vba_arithmeti
+00002f10: 6372 c701 0000 5829 0000 0072 6566 696e  cr....X)...refin
+00002f20: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
+00002f30: 6174 696f 6e2e 7662 612e 6172 6974 686d  ation.vba.arithm
+00002f40: 6574 6963 72c8 0100 0058 1100 0000 6465  eticr....X....de
+00002f50: 6f62 5f76 6261 5f62 7261 636b 6574 7372  ob_vba_bracketsr
+00002f60: c901 0000 5827 0000 0072 6566 696e 6572  ....X'...refiner
+00002f70: 792e 756e 6974 732e 6f62 6675 7363 6174  y.units.obfuscat
+00002f80: 696f 6e2e 7662 612e 6272 6163 6b65 7473  ion.vba.brackets
+00002f90: 72ca 0100 0058 1600 0000 6465 6f62 5f76  r....X....deob_v
+00002fa0: 6261 5f63 6861 725f 6675 6e63 7469 6f6e  ba_char_function
+00002fb0: 72cb 0100 0058 2300 0000 7265 6669 6e65  r....X#...refine
+00002fc0: 7279 2e75 6e69 7473 2e6f 6266 7573 6361  ry.units.obfusca
+00002fd0: 7469 6f6e 2e76 6261 2e63 6861 7272 cc01  tion.vba.charr..
+00002fe0: 0000 5811 0000 0064 656f 625f 7662 615f  ..X....deob_vba_
+00002ff0: 636f 6d6d 656e 7473 72cd 0100 0058 2700  commentsr....X'.
+00003000: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+00003010: 2e6f 6266 7573 6361 7469 6f6e 2e76 6261  .obfuscation.vba
+00003020: 2e63 6f6d 6d65 6e74 7372 ce01 0000 580f  .commentsr....X.
+00003030: 0000 0064 656f 625f 7662 615f 636f 6e63  ...deob_vba_conc
+00003040: 6174 72cf 0100 0058 2500 0000 7265 6669  atr....X%...refi
+00003050: 6e65 7279 2e75 6e69 7473 2e6f 6266 7573  nery.units.obfus
+00003060: 6361 7469 6f6e 2e76 6261 2e63 6f6e 6361  cation.vba.conca
+00003070: 7472 d001 0000 5812 0000 0064 656f 625f  tr....X....deob_
+00003080: 7662 615f 636f 6e73 7461 6e74 7372 d101  vba_constantsr..
+00003090: 0000 5828 0000 0072 6566 696e 6572 792e  ..X(...refinery.
+000030a0: 756e 6974 732e 6f62 6675 7363 6174 696f  units.obfuscatio
+000030b0: 6e2e 7662 612e 636f 6e73 7461 6e74 7372  n.vba.constantsr
+000030c0: d201 0000 5818 0000 0064 656f 625f 7662  ....X....deob_vb
+000030d0: 615f 6475 6d6d 795f 7661 7269 6162 6c65  a_dummy_variable
+000030e0: 7372 d301 0000 5826 0000 0072 6566 696e  sr....X&...refin
+000030f0: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
+00003100: 6174 696f 6e2e 7662 612e 6475 6d6d 6965  ation.vba.dummie
+00003110: 7372 d401 0000 5816 0000 0064 656f 625f  sr....X....deob_
+00003120: 7662 615f 7374 7269 6e67 7265 706c 6163  vba_stringreplac
+00003130: 6572 d501 0000 582c 0000 0072 6566 696e  er....X,...refin
+00003140: 6572 792e 756e 6974 732e 6f62 6675 7363  ery.units.obfusc
+00003150: 6174 696f 6e2e 7662 612e 7374 7269 6e67  ation.vba.string
+00003160: 7265 706c 6163 6572 d601 0000 5816 0000  replacer....X...
+00003170: 0064 656f 625f 7662 615f 7374 7269 6e67  .deob_vba_string
+00003180: 7265 7665 7273 6572 d701 0000 582c 0000  reverser....X,..
+00003190: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+000031a0: 6f62 6675 7363 6174 696f 6e2e 7662 612e  obfuscation.vba.
+000031b0: 7374 7269 6e67 7265 7665 7273 6572 d801  stringreverser..
+000031c0: 0000 5815 0000 0064 656f 625f 7662 615f  ..X....deob_vba_
+000031d0: 6368 725f 6c69 7465 7261 6c73 72d9 0100  chr_literalsr...
+000031e0: 0058 2200 0000 7265 6669 6e65 7279 2e75  .X"...refinery.u
+000031f0: 6e69 7473 2e6f 6266 7573 6361 7469 6f6e  nits.obfuscation
+00003200: 2e76 6261 2e76 6261 72da 0100 0058 0500  .vba.vbar....X..
+00003210: 0000 6361 7276 6572 db01 0000 581c 0000  ..carver....X...
+00003220: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
+00003230: 7061 7474 6572 6e2e 6361 7276 6572 dc01  pattern.carver..
+00003240: 0000 5808 0000 0063 6172 7665 5f37 7a72  ..X....carve_7zr
+00003250: dd01 0000 581f 0000 0072 6566 696e 6572  ....X....refiner
+00003260: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
+00003270: 6361 7276 655f 377a 72de 0100 0058 0a00  carve_7zr....X..
+00003280: 0000 6361 7276 655f 6a73 6f6e 72df 0100  ..carve_jsonr...
+00003290: 0058 2100 0000 7265 6669 6e65 7279 2e75  .X!...refinery.u
 000032a0: 6e69 7473 2e70 6174 7465 726e 2e63 6172  nits.pattern.car
-000032b0: 7665 5f70 6572 e001 0000 5809 0000 0063  ve_per....X....c
-000032c0: 6172 7665 5f72 7466 72e1 0100 0058 2000  arve_rtfr....X .
-000032d0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000032e0: 2e70 6174 7465 726e 2e63 6172 7665 5f72  .pattern.carve_r
-000032f0: 7466 72e2 0100 0058 0900 0000 6361 7276  tfr....X....carv
-00003300: 655f 786d 6c72 e301 0000 5820 0000 0072  e_xmlr....X ...r
-00003310: 6566 696e 6572 792e 756e 6974 732e 7061  efinery.units.pa
-00003320: 7474 6572 6e2e 6361 7276 655f 786d 6c72  ttern.carve_xmlr
-00003330: e401 0000 5809 0000 0063 6172 7665 5f7a  ....X....carve_z
-00003340: 6970 72e5 0100 0058 2000 0000 7265 6669  ipr....X ...refi
+000032b0: 7665 5f6a 736f 6e72 e001 0000 5809 0000  ve_jsonr....X...
+000032c0: 0063 6172 7665 5f6c 6e6b 72e1 0100 0058  .carve_lnkr....X
+000032d0: 2000 0000 7265 6669 6e65 7279 2e75 6e69   ...refinery.uni
+000032e0: 7473 2e70 6174 7465 726e 2e63 6172 7665  ts.pattern.carve
+000032f0: 5f6c 6e6b 72e2 0100 0058 0800 0000 6361  _lnkr....X....ca
+00003300: 7276 655f 7065 72e3 0100 0058 1f00 0000  rve_per....X....
+00003310: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
+00003320: 6174 7465 726e 2e63 6172 7665 5f70 6572  attern.carve_per
+00003330: e401 0000 5809 0000 0063 6172 7665 5f72  ....X....carve_r
+00003340: 7466 72e5 0100 0058 2000 0000 7265 6669  tfr....X ...refi
 00003350: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
-00003360: 726e 2e63 6172 7665 5f7a 6970 72e6 0100  rn.carve_zipr...
-00003370: 0058 0600 0000 6465 6661 6e67 72e7 0100  .X....defangr...
-00003380: 0058 1d00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00003390: 6e69 7473 2e70 6174 7465 726e 2e64 6566  nits.pattern.def
-000033a0: 616e 6772 e801 0000 5809 0000 0064 6e73  angr....X....dns
-000033b0: 646f 6d61 696e 72e9 0100 0058 2000 0000  domainr....X ...
-000033c0: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
-000033d0: 6174 7465 726e 2e64 6e73 646f 6d61 696e  attern.dnsdomain
-000033e0: 72ea 0100 0058 0900 0000 6d69 6d65 776f  r....X....mimewo
-000033f0: 7264 7372 eb01 0000 5820 0000 0072 6566  rdsr....X ...ref
-00003400: 696e 6572 792e 756e 6974 732e 7061 7474  inery.units.patt
-00003410: 6572 6e2e 6d69 6d65 776f 7264 7372 ec01  ern.mimewordsr..
-00003420: 0000 5807 0000 0072 6573 706c 6974 72ed  ..X....resplitr.
-00003430: 0100 0058 1e00 0000 7265 6669 6e65 7279  ...X....refinery
-00003440: 2e75 6e69 7473 2e70 6174 7465 726e 2e72  .units.pattern.r
-00003450: 6573 706c 6974 72ee 0100 0058 0500 0000  esplitr....X....
-00003460: 7265 7375 6272 ef01 0000 581c 0000 0072  resubr....X....r
-00003470: 6566 696e 6572 792e 756e 6974 732e 7061  efinery.units.pa
-00003480: 7474 6572 6e2e 7265 7375 6272 f001 0000  ttern.resubr....
-00003490: 5803 0000 0072 6578 72f1 0100 0058 1a00  X....rexr....X..
-000034a0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-000034b0: 2e70 6174 7465 726e 2e72 6578 72f2 0100  .pattern.rexr...
-000034c0: 0058 0600 0000 7374 7275 6374 72f3 0100  .X....structr...
-000034d0: 0058 2400 0000 7265 6669 6e65 7279 2e75  .X$...refinery.u
-000034e0: 6e69 7473 2e70 6174 7465 726e 2e73 7472  nits.pattern.str
-000034f0: 7563 745f 7061 7273 6572 72f4 0100 0058  uct_parserr....X
-00003500: 0800 0000 7375 6266 696c 6573 72f5 0100  ....subfilesr...
-00003510: 0058 1f00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00003520: 6e69 7473 2e70 6174 7465 726e 2e73 7562  nits.pattern.sub
-00003530: 6669 6c65 7372 f601 0000 5809 0000 0075  filesr....X....u
-00003540: 726c 6775 6172 6473 72f7 0100 0058 2000  rlguardsr....X .
-00003550: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00003560: 2e70 6174 7465 726e 2e75 726c 6775 6172  .pattern.urlguar
-00003570: 6473 72f8 0100 0058 0300 0000 7874 7072  dsr....X....xtpr
-00003580: f901 0000 581a 0000 0072 6566 696e 6572  ....X....refiner
-00003590: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
-000035a0: 7874 7072 fa01 0000 5803 0000 0078 7477  xtpr....X....xtw
-000035b0: 72fb 0100 0058 1a00 0000 7265 6669 6e65  r....X....refine
-000035c0: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
-000035d0: 2e78 7477 72fc 0100 0058 0300 0000 6173  .xtwr....X....as
-000035e0: 6d72 fd01 0000 5818 0000 0072 6566 696e  mr....X....refin
-000035f0: 6572 792e 756e 6974 732e 7369 6e6b 732e  ery.units.sinks.
-00003600: 6173 6d72 fe01 0000 5804 0000 0064 756d  asmr....X....dum
-00003610: 7072 ff01 0000 5819 0000 0072 6566 696e  pr....X....refin
-00003620: 6572 792e 756e 6974 732e 7369 6e6b 732e  ery.units.sinks.
-00003630: 6475 6d70 7200 0200 0058 0500 0000 6965  dumpr....X....ie
-00003640: 6d61 7072 0102 0000 581a 0000 0072 6566  mapr....X....ref
-00003650: 696e 6572 792e 756e 6974 732e 7369 6e6b  inery.units.sink
-00003660: 732e 6965 6d61 7072 0202 0000 5804 0000  s.iemapr....X...
-00003670: 0070 6565 6b72 0302 0000 5819 0000 0072  .peekr....X....r
-00003680: 6566 696e 6572 792e 756e 6974 732e 7369  efinery.units.si
-00003690: 6e6b 732e 7065 656b 7204 0200 0058 0900  nks.peekr....X..
-000036a0: 0000 7070 6a73 6372 6970 7472 0502 0000  ..ppjscriptr....
-000036b0: 581e 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000036c0: 6974 732e 7369 6e6b 732e 7070 6a73 6372  its.sinks.ppjscr
-000036d0: 6970 7472 0602 0000 5806 0000 0070 706a  iptr....X....ppj
-000036e0: 736f 6e72 0702 0000 581b 0000 0072 6566  sonr....X....ref
-000036f0: 696e 6572 792e 756e 6974 732e 7369 6e6b  inery.units.sink
-00003700: 732e 7070 6a73 6f6e 7208 0200 0058 0500  s.ppjsonr....X..
-00003710: 0000 7070 786d 6c72 0902 0000 581a 0000  ..ppxmlr....X...
-00003720: 0072 6566 696e 6572 792e 756e 6974 732e  .refinery.units.
-00003730: 7369 6e6b 732e 7070 786d 6c72 0a02 0000  sinks.ppxmlr....
-00003740: 5803 0000 0063 6361 720b 0200 0058 1a00  X....ccar....X..
-00003750: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
-00003760: 2e73 7472 696e 6773 2e63 6361 720c 0200  .strings.ccar...
-00003770: 0058 0300 0000 6363 7072 0d02 0000 581a  .X....ccpr....X.
-00003780: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
-00003790: 732e 7374 7269 6e67 732e 6363 7072 0e02  s.strings.ccpr..
-000037a0: 0000 5804 0000 0063 666d 7472 0f02 0000  ..X....cfmtr....
-000037b0: 581b 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-000037c0: 6974 732e 7374 7269 6e67 732e 6366 6d74  its.strings.cfmt
-000037d0: 7210 0200 0058 0600 0000 636c 6f77 6572  r....X....clower
-000037e0: 7211 0200 0058 1d00 0000 7265 6669 6e65  r....X....refine
-000037f0: 7279 2e75 6e69 7473 2e73 7472 696e 6773  ry.units.strings
-00003800: 2e63 6c6f 7765 7272 1202 0000 5805 0000  .clowerr....X...
-00003810: 0063 7377 6170 7213 0200 0058 1c00 0000  .cswapr....X....
-00003820: 7265 6669 6e65 7279 2e75 6e69 7473 2e73  refinery.units.s
-00003830: 7472 696e 6773 2e63 7377 6170 7214 0200  trings.cswapr...
-00003840: 0058 0600 0000 6375 7070 6572 7215 0200  .X....cupperr...
-00003850: 0058 1d00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
-00003860: 6e69 7473 2e73 7472 696e 6773 2e63 7570  nits.strings.cup
-00003870: 7065 7272 1602 0000 5803 0000 0072 6570  perr....X....rep
-00003880: 7217 0200 0058 1a00 0000 7265 6669 6e65  r....X....refine
-00003890: 7279 2e75 6e69 7473 2e73 7472 696e 6773  ry.units.strings
-000038a0: 2e72 6570 7218 0200 0058 0400 0000 7265  .repr....X....re
-000038b0: 706c 7219 0200 0058 1b00 0000 7265 6669  plr....X....refi
-000038c0: 6e65 7279 2e75 6e69 7473 2e73 7472 696e  nery.units.strin
-000038d0: 6773 2e72 6570 6c72 1a02 0000 5804 0000  gs.replr....X...
-000038e0: 0073 6e69 7072 1b02 0000 581b 0000 0072  .snipr....X....r
-000038f0: 6566 696e 6572 792e 756e 6974 732e 7374  efinery.units.st
-00003900: 7269 6e67 732e 736e 6970 721c 0200 0058  rings.snipr....X
-00003910: 0700 0000 7374 7265 7463 6872 1d02 0000  ....stretchr....
-00003920: 581e 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
-00003930: 6974 732e 7374 7269 6e67 732e 7374 7265  its.strings.stre
-00003940: 7463 6872 1e02 0000 5807 0000 0074 6572  tchr....X....ter
-00003950: 6d66 6974 721f 0200 0058 1e00 0000 7265  mfitr....X....re
-00003960: 6669 6e65 7279 2e75 6e69 7473 2e73 7472  finery.units.str
-00003970: 696e 6773 2e74 6572 6d66 6974 7220 0200  ings.termfitr ..
-00003980: 0058 0400 0000 7472 696d 7221 0200 0058  .X....trimr!...X
-00003990: 1b00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
-000039a0: 7473 2e73 7472 696e 6773 2e74 7269 6d72  ts.strings.trimr
-000039b0: 2202 0000 752e                           "...u.
+00003360: 726e 2e63 6172 7665 5f72 7466 72e6 0100  rn.carve_rtfr...
+00003370: 0058 0900 0000 6361 7276 655f 786d 6c72  .X....carve_xmlr
+00003380: e701 0000 5820 0000 0072 6566 696e 6572  ....X ...refiner
+00003390: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
+000033a0: 6361 7276 655f 786d 6c72 e801 0000 5809  carve_xmlr....X.
+000033b0: 0000 0063 6172 7665 5f7a 6970 72e9 0100  ...carve_zipr...
+000033c0: 0058 2000 0000 7265 6669 6e65 7279 2e75  .X ...refinery.u
+000033d0: 6e69 7473 2e70 6174 7465 726e 2e63 6172  nits.pattern.car
+000033e0: 7665 5f7a 6970 72ea 0100 0058 0600 0000  ve_zipr....X....
+000033f0: 6465 6661 6e67 72eb 0100 0058 1d00 0000  defangr....X....
+00003400: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
+00003410: 6174 7465 726e 2e64 6566 616e 6772 ec01  attern.defangr..
+00003420: 0000 5809 0000 0064 6e73 646f 6d61 696e  ..X....dnsdomain
+00003430: 72ed 0100 0058 2000 0000 7265 6669 6e65  r....X ...refine
+00003440: 7279 2e75 6e69 7473 2e70 6174 7465 726e  ry.units.pattern
+00003450: 2e64 6e73 646f 6d61 696e 72ee 0100 0058  .dnsdomainr....X
+00003460: 0900 0000 6d69 6d65 776f 7264 7372 ef01  ....mimewordsr..
+00003470: 0000 5820 0000 0072 6566 696e 6572 792e  ..X ...refinery.
+00003480: 756e 6974 732e 7061 7474 6572 6e2e 6d69  units.pattern.mi
+00003490: 6d65 776f 7264 7372 f001 0000 5807 0000  mewordsr....X...
+000034a0: 0072 6573 706c 6974 72f1 0100 0058 1e00  .resplitr....X..
+000034b0: 0000 7265 6669 6e65 7279 2e75 6e69 7473  ..refinery.units
+000034c0: 2e70 6174 7465 726e 2e72 6573 706c 6974  .pattern.resplit
+000034d0: 72f2 0100 0058 0500 0000 7265 7375 6272  r....X....resubr
+000034e0: f301 0000 581c 0000 0072 6566 696e 6572  ....X....refiner
+000034f0: 792e 756e 6974 732e 7061 7474 6572 6e2e  y.units.pattern.
+00003500: 7265 7375 6272 f401 0000 5803 0000 0072  resubr....X....r
+00003510: 6578 72f5 0100 0058 1a00 0000 7265 6669  exr....X....refi
+00003520: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
+00003530: 726e 2e72 6578 72f6 0100 0058 0600 0000  rn.rexr....X....
+00003540: 7374 7275 6374 72f7 0100 0058 2400 0000  structr....X$...
+00003550: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
+00003560: 6174 7465 726e 2e73 7472 7563 745f 7061  attern.struct_pa
+00003570: 7273 6572 72f8 0100 0058 0800 0000 7375  rserr....X....su
+00003580: 6266 696c 6573 72f9 0100 0058 1f00 0000  bfilesr....X....
+00003590: 7265 6669 6e65 7279 2e75 6e69 7473 2e70  refinery.units.p
+000035a0: 6174 7465 726e 2e73 7562 6669 6c65 7372  attern.subfilesr
+000035b0: fa01 0000 5809 0000 0075 726c 6775 6172  ....X....urlguar
+000035c0: 6473 72fb 0100 0058 2000 0000 7265 6669  dsr....X ...refi
+000035d0: 6e65 7279 2e75 6e69 7473 2e70 6174 7465  nery.units.patte
+000035e0: 726e 2e75 726c 6775 6172 6473 72fc 0100  rn.urlguardsr...
+000035f0: 0058 0300 0000 7874 7072 fd01 0000 581a  .X....xtpr....X.
+00003600: 0000 0072 6566 696e 6572 792e 756e 6974  ...refinery.unit
+00003610: 732e 7061 7474 6572 6e2e 7874 7072 fe01  s.pattern.xtpr..
+00003620: 0000 5803 0000 0078 7477 72ff 0100 0058  ..X....xtwr....X
+00003630: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00003640: 7473 2e70 6174 7465 726e 2e78 7477 7200  ts.pattern.xtwr.
+00003650: 0200 0058 0300 0000 6173 6d72 0102 0000  ...X....asmr....
+00003660: 5818 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+00003670: 6974 732e 7369 6e6b 732e 6173 6d72 0202  its.sinks.asmr..
+00003680: 0000 5804 0000 0064 756d 7072 0302 0000  ..X....dumpr....
+00003690: 5819 0000 0072 6566 696e 6572 792e 756e  X....refinery.un
+000036a0: 6974 732e 7369 6e6b 732e 6475 6d70 7204  its.sinks.dumpr.
+000036b0: 0200 0058 0500 0000 6965 6d61 7072 0502  ...X....iemapr..
+000036c0: 0000 581a 0000 0072 6566 696e 6572 792e  ..X....refinery.
+000036d0: 756e 6974 732e 7369 6e6b 732e 6965 6d61  units.sinks.iema
+000036e0: 7072 0602 0000 5804 0000 0070 6565 6b72  pr....X....peekr
+000036f0: 0702 0000 5819 0000 0072 6566 696e 6572  ....X....refiner
+00003700: 792e 756e 6974 732e 7369 6e6b 732e 7065  y.units.sinks.pe
+00003710: 656b 7208 0200 0058 0900 0000 7070 6a73  ekr....X....ppjs
+00003720: 6372 6970 7472 0902 0000 581e 0000 0072  criptr....X....r
+00003730: 6566 696e 6572 792e 756e 6974 732e 7369  efinery.units.si
+00003740: 6e6b 732e 7070 6a73 6372 6970 7472 0a02  nks.ppjscriptr..
+00003750: 0000 5806 0000 0070 706a 736f 6e72 0b02  ..X....ppjsonr..
+00003760: 0000 581b 0000 0072 6566 696e 6572 792e  ..X....refinery.
+00003770: 756e 6974 732e 7369 6e6b 732e 7070 6a73  units.sinks.ppjs
+00003780: 6f6e 720c 0200 0058 0500 0000 7070 786d  onr....X....ppxm
+00003790: 6c72 0d02 0000 581a 0000 0072 6566 696e  lr....X....refin
+000037a0: 6572 792e 756e 6974 732e 7369 6e6b 732e  ery.units.sinks.
+000037b0: 7070 786d 6c72 0e02 0000 5803 0000 0063  ppxmlr....X....c
+000037c0: 6361 720f 0200 0058 1a00 0000 7265 6669  car....X....refi
+000037d0: 6e65 7279 2e75 6e69 7473 2e73 7472 696e  nery.units.strin
+000037e0: 6773 2e63 6361 7210 0200 0058 0300 0000  gs.ccar....X....
+000037f0: 6363 7072 1102 0000 581a 0000 0072 6566  ccpr....X....ref
+00003800: 696e 6572 792e 756e 6974 732e 7374 7269  inery.units.stri
+00003810: 6e67 732e 6363 7072 1202 0000 5804 0000  ngs.ccpr....X...
+00003820: 0063 666d 7472 1302 0000 581b 0000 0072  .cfmtr....X....r
+00003830: 6566 696e 6572 792e 756e 6974 732e 7374  efinery.units.st
+00003840: 7269 6e67 732e 6366 6d74 7214 0200 0058  rings.cfmtr....X
+00003850: 0600 0000 636c 6f77 6572 7215 0200 0058  ....clowerr....X
+00003860: 1d00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00003870: 7473 2e73 7472 696e 6773 2e63 6c6f 7765  ts.strings.clowe
+00003880: 7272 1602 0000 5805 0000 0063 7377 6170  rr....X....cswap
+00003890: 7217 0200 0058 1c00 0000 7265 6669 6e65  r....X....refine
+000038a0: 7279 2e75 6e69 7473 2e73 7472 696e 6773  ry.units.strings
+000038b0: 2e63 7377 6170 7218 0200 0058 0600 0000  .cswapr....X....
+000038c0: 6375 7070 6572 7219 0200 0058 1d00 0000  cupperr....X....
+000038d0: 7265 6669 6e65 7279 2e75 6e69 7473 2e73  refinery.units.s
+000038e0: 7472 696e 6773 2e63 7570 7065 7272 1a02  trings.cupperr..
+000038f0: 0000 5803 0000 0072 6570 721b 0200 0058  ..X....repr....X
+00003900: 1a00 0000 7265 6669 6e65 7279 2e75 6e69  ....refinery.uni
+00003910: 7473 2e73 7472 696e 6773 2e72 6570 721c  ts.strings.repr.
+00003920: 0200 0058 0400 0000 7265 706c 721d 0200  ...X....replr...
+00003930: 0058 1b00 0000 7265 6669 6e65 7279 2e75  .X....refinery.u
+00003940: 6e69 7473 2e73 7472 696e 6773 2e72 6570  nits.strings.rep
+00003950: 6c72 1e02 0000 5804 0000 0073 6e69 7072  lr....X....snipr
+00003960: 1f02 0000 581b 0000 0072 6566 696e 6572  ....X....refiner
+00003970: 792e 756e 6974 732e 7374 7269 6e67 732e  y.units.strings.
+00003980: 736e 6970 7220 0200 0058 0700 0000 7374  snipr ...X....st
+00003990: 7265 7463 6872 2102 0000 581e 0000 0072  retchr!...X....r
+000039a0: 6566 696e 6572 792e 756e 6974 732e 7374  efinery.units.st
+000039b0: 7269 6e67 732e 7374 7265 7463 6872 2202  rings.stretchr".
+000039c0: 0000 5807 0000 0074 6572 6d66 6974 7223  ..X....termfitr#
+000039d0: 0200 0058 1e00 0000 7265 6669 6e65 7279  ...X....refinery
+000039e0: 2e75 6e69 7473 2e73 7472 696e 6773 2e74  .units.strings.t
+000039f0: 6572 6d66 6974 7224 0200 0058 0400 0000  ermfitr$...X....
+00003a00: 7472 696d 7225 0200 0058 1b00 0000 7265  trimr%...X....re
+00003a10: 6669 6e65 7279 2e75 6e69 7473 2e73 7472  finery.units.str
+00003a20: 696e 6773 2e74 7269 6d72 2602 0000 752e  ings.trimr&...u.
```

### Comparing `binary-refinery-0.6.6/refinery/__init__.py` & `binary-refinery-0.6.7/refinery/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 1. `refinery.lib.frame`: framing syntax for working on lists of binary chunks
 2. `refinery.lib.argformats`: the multibin syntax for refinery arguments
 3. `refinery.lib.meta`: defining and using metadata variables within frames
 4. `refinery.units`: writing custom units, add command-line arguments, and how to use refinery
    units within Python code.
 """
-__version__ = '0.6.6'
+__version__ = '0.6.7'
 __distribution__ = 'binary-refinery'
 
 from typing import Dict, List, Optional, Type
 from importlib import resources
 from datetime import datetime
 
 import pickle
```

### Comparing `binary-refinery-0.6.6/refinery/data/rich.json` & `binary-refinery-0.6.7/refinery/data/rich.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984344894026975%*

 * *Differences: {"'ver'": "{'0001': {'ide': 'CVTPGD'}, '7DD9': OrderedDict([('ide', 'VS2022 v17.5.4 build "*

 * *          "32217')]), '7F12': OrderedDict([('ide', 'VS2022 v17.6.0 pre 5.0 build 32530')]), "*

 * *          "'7F0A': OrderedDict([('ide', 'VS2022 v17.6.0 pre 3.0 build 32522')])}"}*

```diff
@@ -274,15 +274,15 @@
     },
     "ver": {
         "0000": {
             "ide": "Visual Studio",
             "ver": ""
         },
         "0001": {
-            "ide": "CVTPGD (VS2019?)"
+            "ide": "CVTPGD"
         },
         "041F": {
             "ide": ".NET Framework",
             "ver": "4.6"
         },
         "042F": {
             "ide": "Visual Studio 2003",
@@ -2011,20 +2011,29 @@
         },
         "7DD7": {
             "ide": "VS2022 v17.5.0 build 32215"
         },
         "7DD8": {
             "ide": "VS2022 v17.5.3 build 32216"
         },
+        "7DD9": {
+            "ide": "VS2022 v17.5.4 build 32217"
+        },
         "7E43": {
             "ide": "VS2022 v17.6.0 pre 1.0 build 32323"
         },
         "7EF6": {
             "ide": "VS2022 v17.6.0 pre 2.0 build 32502"
         },
+        "7F0A": {
+            "ide": "VS2022 v17.6.0 pre 3.0 build 32522"
+        },
+        "7F12": {
+            "ide": "VS2022 v17.6.0 pre 5.0 build 32530"
+        },
         "9CB3": {
             "ide": "Visual Studio 2013",
             "ver": "12.10"
         },
         "9CB4": {
             "ide": "Visual Studio 2013",
             "ver": "12.10"
```

### Comparing `binary-refinery-0.6.6/refinery/explore.py` & `binary-refinery-0.6.7/refinery/explore.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/argformats.py` & `binary-refinery-0.6.7/refinery/lib/argformats.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/argparser.py` & `binary-refinery-0.6.7/refinery/lib/argparser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/chunks.py` & `binary-refinery-0.6.7/refinery/lib/chunks.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/crypto.py` & `binary-refinery-0.6.7/refinery/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/decompression.py` & `binary-refinery-0.6.7/refinery/lib/decompression.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/decorators.py` & `binary-refinery-0.6.7/refinery/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/deobfuscation.py` & `binary-refinery-0.6.7/refinery/lib/deobfuscation.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/dex.py` & `binary-refinery-0.6.7/refinery/lib/dex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/dotnet/deserialize.py` & `binary-refinery-0.6.7/refinery/lib/dotnet/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/dotnet/header.py` & `binary-refinery-0.6.7/refinery/lib/dotnet/header.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/dotnet/resources.py` & `binary-refinery-0.6.7/refinery/lib/dotnet/resources.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/dotnet/types.py` & `binary-refinery-0.6.7/refinery/lib/dotnet/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/environment.py` & `binary-refinery-0.6.7/refinery/lib/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,9 +154,10 @@
         else:
             return loglevel
 
 
 class environment:
     verbosity = EVLog('VERBOSITY')
     term_size = EVInt('TERM_SIZE')
+    disable_size_format = EVBool('DISABLE_SIZE_FORMAT')
     silence_ps1_warning = EVBool('SILENCE_PS1_WARNING')
     disable_ps1_bandaid = EVBool('DISABLE_PS1_BANDAID')
```

### Comparing `binary-refinery-0.6.6/refinery/lib/executable.py` & `binary-refinery-0.6.7/refinery/lib/executable.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/frame.py` & `binary-refinery-0.6.7/refinery/lib/frame.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/inline.py` & `binary-refinery-0.6.7/refinery/lib/inline.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/java.py` & `binary-refinery-0.6.7/refinery/lib/java.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/json.py` & `binary-refinery-0.6.7/refinery/lib/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/loader.py` & `binary-refinery-0.6.7/refinery/lib/loader.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/magic.py` & `binary-refinery-0.6.7/refinery/lib/magic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/meta.py` & `binary-refinery-0.6.7/refinery/lib/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 
 from io import StringIO
 from urllib.parse import quote_from_bytes, unquote_to_bytes
 from typing import Callable, Dict, Iterable, Optional, ByteString, Union, TYPE_CHECKING
 
 from refinery.lib.structures import MemoryFile
 from refinery.lib.tools import isbuffer, entropy, index_of_coincidence
+from refinery.lib.environment import environment
 
 
 if TYPE_CHECKING:
     from typing import Protocol
     from refinery.lib.frame import Chunk
 
     class _Derivation(Protocol):
@@ -318,33 +319,36 @@
     """
     The string representation of this int class is a a human-readable expression of size, using
     common units such as kB and MB.
     """
     width = 9
     align = True
 
-    def __repr__(self):
-        step = 1000.0
-        unit = None
-        result = self
-        for unit in [None, 'kB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB']:
-            if unit and result / step <= 0.1:
-                break
-            result /= step
-        if unit is None:
-            width = 3 if self.align else 1
-            return F'{result:{width}} BYTES'
-        else:
-            width = 6 if self.align else 1
-            comma = 3 if self.align else 1
-            return F'{result:0{width}.{comma}f} {unit}'
-
     def __str__(self):
         return str(int(self))
 
+    if environment.disable_size_format.value:
+        __repr__ = __str__
+    else:
+        def __repr__(self):
+            step = 1000.0
+            unit = None
+            result = self
+            for unit in [None, 'kB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB']:
+                if unit and result / step <= 0.1:
+                    break
+                result /= step
+            if unit is None:
+                width = 3 if self.align else 1
+                return F'{result:{width}} BYTES'
+            else:
+                width = 6 if self.align else 1
+                comma = 3 if self.align else 1
+                return F'{result:0{width}.{comma}f} {unit}'
+
 
 class TerseSizeInt(SizeInt):
     """
     Similar to `refinery.lib.meta.SizeInt`, but the representation does not pad with zeros to
     ensure having the same width for every input.
     """
     align = False
```

### Comparing `binary-refinery-0.6.6/refinery/lib/mime.py` & `binary-refinery-0.6.7/refinery/lib/mime.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/mscrypto.py` & `binary-refinery-0.6.7/refinery/lib/mscrypto.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/murmur.py` & `binary-refinery-0.6.7/refinery/lib/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/patterns/__init__.py` & `binary-refinery-0.6.7/refinery/lib/patterns/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,14 +183,19 @@
 
 _pattern_serrated_hostname = _pattern_serrated_socket + '?'
 _pattern_defanged_hostname = _pattern_defanged_socket + '?'
 
 
 _pattern_integer = '[-+]?(?:0[bB][01]+|0[xX][0-9a-fA-F]+|0[1-7][0-7]*|[1-9][0-9]*|0)(?=[uU]?[iI]\\d{1,2}|[LlHh]|[^a-zA-Z0-9]|$)'
 _pattern_float = R'[-+]?[0-9]*\.?[0-9]+(?:[eE][-+]?[0-9]+)?'
+_pattern_number = F'(?:(?:{_pattern_integer})|(?:{_pattern_float}))'
+_pattern_number = (
+    '[-+]?(?:0[bB][01]+|0[xX][0-9a-fA-F]+|0[1-7][0-7]*|(?:[1-9][0-9]*|0)(?P<fp1>\\.[0-9]*)?|(?P<fp2>\\.[0-9]+))'
+    '(?(fp1)(?:[eE][-+]?[0-9]+)?|(?(fp2)(?:[eE][-+]?[0-9]+)?|(?=[uU]?[iI]\\d{1,2}|[LlHh]|[^a-zA-Z0-9]|$)))'
+)
 _pattern_cmdstr = R'''(?:"(?:""|[^"])*"|'(?:''|[^'])*')'''
 _pattern_ps1str = R'''(?:@"\s*?[\r\n].*?[\r\n]"@|@'\s*?[\r\n].*?[\r\n]'@|"(?:`.|""|[^"])*"|'(?:''|[^'])*')'''
 _pattern_vbastr = R'''"(?:""|[^"])*"'''
 _pattern_vbaint = R'(?:&[bB][01]+|&[hH][0-9a-fA-F]+|&[oO][0-7]*|[-+]?(?:[1-9][0-9]*|0))(?=\b|$)'
 _pattern_string = R'''(?:"(?:[^"\\\r\n]|\\[^\r\n])*"|'(?:[^'\\\r\n]|\\[^\r\n])*')'''
 _pattern_string_multiline = R'''(?:"(?:[^"\\]|\\.)*"|'(?:[^'\\]|\\.)*')'''
 _pattern_urlenc_coarse = R'''(?:%[0-9a-fA-F]{2}|[0-9a-zA-Z\-\._~\?!$&=:\/#\[\]@'\(\)\*\+,;])+'''
@@ -278,14 +283,16 @@
     """
     An enumeration of patterns for certain formats.
     """
     integer = pattern(_pattern_integer)
     "Integer expressions"
     float = pattern(_pattern_float)
     "Floating point number expressions"
+    number = pattern(_pattern_number)
+    "Either an integer or a float"
     string = pattern(_pattern_string)
     "C syntax string literal"
     multiline_string = pattern(_pattern_string_multiline)
     "C syntax string literal that also allows line breaks"
     cmdstr = pattern(_pattern_cmdstr)
     "Windows command line escaped string literal"
     ps1str = pattern(_pattern_ps1str)
@@ -300,14 +307,16 @@
     "Any sequence of url-encoded characters, default char set"
     urlquote_coarse = pattern(_pattern_urlenc_coarse)
     "Any sequence of url-encoded characters, coarser variant with more characters allowed"
     urlquote_narrow = pattern(_pattern_urlenc_narrow)
     "A hex-encoded buffer using URL escape sequences"
     intarray = tokenize(_pattern_integer, sep=R'\s*[;,]\s*', bound='', unique_sep=True)
     "Sequences of integers, separated by commas or semicolons"
+    numarray = tokenize(_pattern_number, sep=R'\s*[;,]\s*', bound='', unique_sep=True)
+    "Sequences of numbers, separated by commas or semicolons"
     word = alphabet(R'\\w')
     "Sequences of word characters"
     letters = alphabet(R'[a-zA-Z]')
     "Sequences of alphabetic characters"
     wshenc = pattern(_pattern_wshenc)
     "Encoded Windows Scripting Host Scripts (JS/VBS)"
     alphanumeric = alphabet(R'[a-zA-Z0-9]')
@@ -344,33 +353,34 @@
 
     @classmethod
     def from_dashname(cls, key):
         return getattr(cls, key.replace('-', '_'))
 
 
 class wallets(PatternEnum):
+    # https://gist.github.com/etherx-dev/76559d9e6d916917a960e33ceea91481
     ADA = pattern("addr1[a-z0-9]+")
     ATOM = pattern("cosmos[-\\w\\.]{10,}")
     BCH = pattern("(bitcoincash:)?(q|p)[a-z0-9]{41}|(BITCOINCASH:)?(Q|P)[A-Z0-9]{41}")
-    BTC = pattern("[13][a-km-zA-HJ-NP-Z1-9]{25,34}")
+    BTC = pattern("(?:[13][a-km-zA-HJ-NP-Z1-9]{25,34}|bc1[a-z0-9]{25,39})")
     BTCP = pattern("5[HJK][1-9A-Za-z][^OIl]{48}")
     DASH = pattern("X[1-9A-HJ-NP-Za-km-z]{33}")
     DOGE = pattern("D{1}[5-9A-HJ-NP-U]{1}[1-9A-HJ-NP-Za-km-z]{32}")
     DOT = pattern("1[0-9a-zA-Z]{47}")
     ETH = pattern("0x[a-fA-F0-9]{40}")
     IOTA = pattern("iota[a-z0-9]{10,}")
     LSK = pattern("[0-9]{19}L")
     LTC = pattern("[LM3][a-km-zA-HJ-NP-Z1-9]{26,33}")
     NEO = pattern("N[0-9a-zA-Z]{33}")
     ONE = pattern("(?:bnb|one)1[a-z0-9]{38}")
     ONT = pattern("A[0-9a-zA-Z]{33}")
     RONIN = pattern("ronin:[a-fA-F0-9]{40}")
     TERRA = pattern("terra1[a-z0-9]{38}")
     XEM = pattern("N[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}-[A-Za-z0-9]{4,7}")
-    XLM = pattern("G[0-9A-Z]{40,60}")
+    XLM = pattern("G[A-D][A-Z2-7]{54}")
     XMR = pattern("4[0-9AB][1-9A-HJ-NP-Za-km-z]{90,120}")
     XRP = pattern("r[0-9a-zA-Z]{24,34}")
 
 
 class indicators(PatternEnum):
     """
     An enumeration of patterns for indicators.
```

### Comparing `binary-refinery-0.6.6/refinery/lib/patterns/tlds.py` & `binary-refinery-0.6.7/refinery/lib/patterns/tlds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/powershell.py` & `binary-refinery-0.6.7/refinery/lib/powershell.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/ripemd128.py` & `binary-refinery-0.6.7/refinery/lib/ripemd128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/serpent.py` & `binary-refinery-0.6.7/refinery/lib/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/structures.py` & `binary-refinery-0.6.7/refinery/lib/structures.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/suffixtree.py` & `binary-refinery-0.6.7/refinery/lib/suffixtree.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/thirdparty/acefile.py` & `binary-refinery-0.6.7/refinery/lib/thirdparty/acefile.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/thirdparty/batch_interpreter.py` & `binary-refinery-0.6.7/refinery/lib/thirdparty/batch_interpreter.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/thirdparty/pcode2code.py` & `binary-refinery-0.6.7/refinery/lib/thirdparty/pcode2code.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/thirdparty/xxhash.py` & `binary-refinery-0.6.7/refinery/lib/thirdparty/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/tools.py` & `binary-refinery-0.6.7/refinery/lib/tools.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/types.py` & `binary-refinery-0.6.7/refinery/lib/types.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/vfs.py` & `binary-refinery-0.6.7/refinery/lib/vfs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/lib/xml.py` & `binary-refinery-0.6.7/refinery/lib/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/__init__.py` & `binary-refinery-0.6.7/refinery/units/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/blockwise/__init__.py` & `binary-refinery-0.6.7/refinery/units/blockwise/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/blockwise/alu.py` & `binary-refinery-0.6.7/refinery/units/blockwise/alu.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/blockwise/bitrev.py` & `binary-refinery-0.6.7/refinery/units/blockwise/bitrev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/blockwise/byteswap.py` & `binary-refinery-0.6.7/refinery/units/blockwise/byteswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/blockwise/map.py` & `binary-refinery-0.6.7/refinery/units/blockwise/map.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/blockwise/rev.py` & `binary-refinery-0.6.7/refinery/units/blockwise/rev.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/blockwise/terminate.py` & `binary-refinery-0.6.7/refinery/units/blockwise/terminate.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/blockwise/xor.py` & `binary-refinery-0.6.7/refinery/units/blockwise/xor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/ap.py` & `binary-refinery-0.6.7/refinery/units/compression/ap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/blz.py` & `binary-refinery-0.6.7/refinery/units/compression/blz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/bz2.py` & `binary-refinery-0.6.7/refinery/units/compression/bz2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/decompress.py` & `binary-refinery-0.6.7/refinery/units/compression/decompress.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/jcalg.py` & `binary-refinery-0.6.7/refinery/units/compression/jcalg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/lz.py` & `binary-refinery-0.6.7/refinery/units/compression/lz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/lz4.py` & `binary-refinery-0.6.7/refinery/units/compression/lz4.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/lzf.py` & `binary-refinery-0.6.7/refinery/units/compression/lzf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/lzg.py` & `binary-refinery-0.6.7/refinery/units/compression/lzg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/lzip.py` & `binary-refinery-0.6.7/refinery/units/compression/lzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/lzjb.py` & `binary-refinery-0.6.7/refinery/units/compression/lzjb.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/lznt1.py` & `binary-refinery-0.6.7/refinery/units/compression/lznt1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/lzo.py` & `binary-refinery-0.6.7/refinery/units/compression/lzo.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/mscf.py` & `binary-refinery-0.6.7/refinery/units/compression/mscf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/qlz.py` & `binary-refinery-0.6.7/refinery/units/compression/qlz.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/szdd.py` & `binary-refinery-0.6.7/refinery/units/compression/szdd.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/compression/zl.py` & `binary-refinery-0.6.7/refinery/units/compression/zl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/__init__.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/camellia.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/camellia.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/chacha.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/chacha.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/gost.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/gost.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/hc128.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/hc128.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/isaac.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/isaac.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/rabbit.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/rabbit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/rc2.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/rc2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/rc4mod.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/rc4mod.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/rc5.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/rc5.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/rc6.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/rc6.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/rijndael.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/rijndael.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/rncrypt.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/rncrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/rot.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/rot.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/rsa.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/rsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/rsakey.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/rsakey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/salsa.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/salsa.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/seal.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/seal.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/secstr.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/secstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/serpent.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/serpent.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/tea.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/tea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/vigenere.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/vigenere.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/xtea.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/xtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/cipher/xxtea.py` & `binary-refinery-0.6.7/refinery/units/crypto/cipher/xxtea.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/hash/__init__.py` & `binary-refinery-0.6.7/refinery/units/crypto/hash/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/hash/checksums.py` & `binary-refinery-0.6.7/refinery/units/crypto/hash/checksums.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/hash/cryptographic.py` & `binary-refinery-0.6.7/refinery/units/crypto/hash/cryptographic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/hash/imphash.py` & `binary-refinery-0.6.7/refinery/units/crypto/hash/imphash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/hash/murmur.py` & `binary-refinery-0.6.7/refinery/units/crypto/hash/murmur.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/hash/xxhash.py` & `binary-refinery-0.6.7/refinery/units/crypto/hash/xxhash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/keyderive/CryptDeriveKey.py` & `binary-refinery-0.6.7/refinery/units/crypto/keyderive/CryptDeriveKey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/keyderive/DESDerive.py` & `binary-refinery-0.6.7/refinery/units/crypto/keyderive/DESDerive.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/keyderive/PasswordDeriveBytes.py` & `binary-refinery-0.6.7/refinery/units/crypto/keyderive/PasswordDeriveBytes.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/keyderive/__init__.py` & `binary-refinery-0.6.7/refinery/units/crypto/keyderive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/keyderive/kblob.py` & `binary-refinery-0.6.7/refinery/units/crypto/keyderive/kblob.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/keyderive/pbkdf1.py` & `binary-refinery-0.6.7/refinery/units/crypto/keyderive/pbkdf1.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/keyderive/pbkdf2.py` & `binary-refinery-0.6.7/refinery/units/crypto/keyderive/pbkdf2.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/crypto/keyderive/unixcrypt.py` & `binary-refinery-0.6.7/refinery/units/crypto/keyderive/unixcrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/atbash.py` & `binary-refinery-0.6.7/refinery/units/encoding/atbash.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/b32.py` & `binary-refinery-0.6.7/refinery/units/encoding/b32.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/b64.py` & `binary-refinery-0.6.7/refinery/units/encoding/b64.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/base.py` & `binary-refinery-0.6.7/refinery/units/encoding/base.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/esc.py` & `binary-refinery-0.6.7/refinery/units/encoding/esc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/hex.py` & `binary-refinery-0.6.7/refinery/units/encoding/hex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/netbios.py` & `binary-refinery-0.6.7/refinery/units/encoding/netbios.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/ps1str.py` & `binary-refinery-0.6.7/refinery/units/encoding/ps1str.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/recode.py` & `binary-refinery-0.6.7/refinery/units/encoding/recode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/url.py` & `binary-refinery-0.6.7/refinery/units/encoding/url.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/uuenc.py` & `binary-refinery-0.6.7/refinery/units/encoding/uuenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/encoding/wshenc.py` & `binary-refinery-0.6.7/refinery/units/encoding/wshenc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/__init__.py` & `binary-refinery-0.6.7/refinery/units/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/a3x.py` & `binary-refinery-0.6.7/refinery/units/formats/a3x.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/__init__.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xt.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xt.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     """
     Extract files from archives. The unit tries to identify the archive format and use the
     correct extractor.
     """
     def _handlers(self):
         from refinery.units.formats.office.xtone import xtone
         yield xtone
+        from refinery.units.formats.archive.xtgz import xtgz
+        yield xtgz
         from refinery.units.formats.email import xtmail
         yield xtmail
         from refinery.units.formats.pdf import xtpdf
         yield xtpdf
         from refinery.units.formats.archive.xtasar import xtasar
         yield xtasar
         from refinery.units.formats.office.xtrtf import xtrtf
```

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xt7z.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xt7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xtace.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xtace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xtasar.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xtasar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xtcab.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xtcab.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xtcpio.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xtcpio.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xtiso.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xtiso.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xtiss.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xtiss.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xtnode.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xtnode.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xtnsis.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xtnsis.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xtpyi.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xtpyi.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xttar.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xttar.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/archive/xtzip.py` & `binary-refinery-0.6.7/refinery/units/formats/archive/xtzip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/bat.py` & `binary-refinery-0.6.7/refinery/units/formats/bat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/csv.py` & `binary-refinery-0.6.7/refinery/units/formats/csv.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/deserialize_php.py` & `binary-refinery-0.6.7/refinery/units/formats/deserialize_php.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/email.py` & `binary-refinery-0.6.7/refinery/units/formats/email.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/evtx.py` & `binary-refinery-0.6.7/refinery/units/formats/evtx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/exe/vaddr.py` & `binary-refinery-0.6.7/refinery/units/formats/exe/vaddr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/exe/vmemref.py` & `binary-refinery-0.6.7/refinery/units/formats/exe/vmemref.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/exe/vsect.py` & `binary-refinery-0.6.7/refinery/units/formats/exe/vsect.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/exe/vsnip.py` & `binary-refinery-0.6.7/refinery/units/formats/exe/vsnip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/exe/vstack.py` & `binary-refinery-0.6.7/refinery/units/formats/exe/vstack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/hexload.py` & `binary-refinery-0.6.7/refinery/units/formats/hexload.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/html.py` & `binary-refinery-0.6.7/refinery/units/formats/html.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/httpresponse.py` & `binary-refinery-0.6.7/refinery/units/formats/httpresponse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/ifps.py` & `binary-refinery-0.6.7/refinery/units/formats/ifps.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/ifpsstr.py` & `binary-refinery-0.6.7/refinery/units/formats/ifpsstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/java/deserialize.py` & `binary-refinery-0.6.7/refinery/units/formats/java/deserialize.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/java/jvdasm.py` & `binary-refinery-0.6.7/refinery/units/formats/java/jvdasm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/json.py` & `binary-refinery-0.6.7/refinery/units/formats/json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/lnk.py` & `binary-refinery-0.6.7/refinery/units/formats/lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/msgpack.py` & `binary-refinery-0.6.7/refinery/units/formats/msgpack.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/msi.py` & `binary-refinery-0.6.7/refinery/units/formats/msi.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/office/doctxt.py` & `binary-refinery-0.6.7/refinery/units/formats/office/doctxt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/office/officecrypt.py` & `binary-refinery-0.6.7/refinery/units/formats/office/officecrypt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/office/vbapc.py` & `binary-refinery-0.6.7/refinery/units/formats/office/vbapc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/office/vbastr.py` & `binary-refinery-0.6.7/refinery/units/formats/office/vbastr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/office/xlmdeobf.py` & `binary-refinery-0.6.7/refinery/units/formats/office/xlmdeobf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/office/xlxtr.py` & `binary-refinery-0.6.7/refinery/units/formats/office/xlxtr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/office/xtdoc.py` & `binary-refinery-0.6.7/refinery/units/formats/office/xtdoc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/office/xtone.py` & `binary-refinery-0.6.7/refinery/units/formats/office/xtone.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/office/xtrtf.py` & `binary-refinery-0.6.7/refinery/units/formats/office/xtrtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/office/xtvba.py` & `binary-refinery-0.6.7/refinery/units/formats/office/xtvba.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pcap.py` & `binary-refinery-0.6.7/refinery/units/formats/pcap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pcap_http.py` & `binary-refinery-0.6.7/refinery/units/formats/pcap_http.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pdf.py` & `binary-refinery-0.6.7/refinery/units/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/__init__.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/__init__.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dncfx.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dncfx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnds.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnds.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnfields.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnfields.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnhdr.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnhdr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnmr.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnmr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnrc.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnrc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/dotnet/dnstr.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/dotnet/dnstr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/pemeta.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/pemeta.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/peoverlay.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/peoverlay.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/perc.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/perc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/pesig.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/pesig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pe/pestrip.py` & `binary-refinery-0.6.7/refinery/units/formats/pe/pestrip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pkcs7.py` & `binary-refinery-0.6.7/refinery/units/formats/pkcs7.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/pkcs7sig.py` & `binary-refinery-0.6.7/refinery/units/formats/pkcs7sig.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/stego.py` & `binary-refinery-0.6.7/refinery/units/formats/stego.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/tnetmtm.py` & `binary-refinery-0.6.7/refinery/units/formats/tnetmtm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/winreg.py` & `binary-refinery-0.6.7/refinery/units/formats/winreg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/formats/xml.py` & `binary-refinery-0.6.7/refinery/units/formats/xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/malware/n40.py` & `binary-refinery-0.6.7/refinery/units/malware/n40.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/__init__.py` & `binary-refinery-0.6.7/refinery/units/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/chop.py` & `binary-refinery-0.6.7/refinery/units/meta/chop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/cm.py` & `binary-refinery-0.6.7/refinery/units/meta/cm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/cull.py` & `binary-refinery-0.6.7/refinery/units/meta/cull.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/dedup.py` & `binary-refinery-0.6.7/refinery/units/meta/dedup.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/eat.py` & `binary-refinery-0.6.7/refinery/units/meta/eat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/ef.py` & `binary-refinery-0.6.7/refinery/units/meta/ef.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/emit.py` & `binary-refinery-0.6.7/refinery/units/meta/emit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/group.py` & `binary-refinery-0.6.7/refinery/units/meta/group.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/groupby.py` & `binary-refinery-0.6.7/refinery/units/meta/groupby.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/iff.py` & `binary-refinery-0.6.7/refinery/units/meta/iff.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/iffp.py` & `binary-refinery-0.6.7/refinery/units/meta/iffp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/iffs.py` & `binary-refinery-0.6.7/refinery/units/meta/iffs.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/iffx.py` & `binary-refinery-0.6.7/refinery/units/meta/iffx.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/max.py` & `binary-refinery-0.6.7/refinery/units/meta/max.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/min.py` & `binary-refinery-0.6.7/refinery/units/meta/min.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/mvc.py` & `binary-refinery-0.6.7/refinery/units/meta/mvc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/mvg.py` & `binary-refinery-0.6.7/refinery/units/meta/mvg.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/pad.py` & `binary-refinery-0.6.7/refinery/units/meta/pad.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/pick.py` & `binary-refinery-0.6.7/refinery/units/meta/pick.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/pop.py` & `binary-refinery-0.6.7/refinery/units/meta/pop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/push.py` & `binary-refinery-0.6.7/refinery/units/meta/push.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/put.py` & `binary-refinery-0.6.7/refinery/units/meta/put.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/queue.py` & `binary-refinery-0.6.7/refinery/units/meta/queue.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/reduce.py` & `binary-refinery-0.6.7/refinery/units/meta/reduce.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/scope.py` & `binary-refinery-0.6.7/refinery/units/meta/scope.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/sep.py` & `binary-refinery-0.6.7/refinery/units/meta/sep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/sorted.py` & `binary-refinery-0.6.7/refinery/units/meta/sorted.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/swap.py` & `binary-refinery-0.6.7/refinery/units/meta/swap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/transpose.py` & `binary-refinery-0.6.7/refinery/units/meta/transpose.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/meta/xfcc.py` & `binary-refinery-0.6.7/refinery/units/meta/xfcc.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/misc/autoxor.py` & `binary-refinery-0.6.7/refinery/units/misc/autoxor.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/misc/couple.py` & `binary-refinery-0.6.7/refinery/units/misc/couple.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/misc/datefix.py` & `binary-refinery-0.6.7/refinery/units/misc/datefix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/misc/drp.py` & `binary-refinery-0.6.7/refinery/units/misc/drp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/misc/nop.py` & `binary-refinery-0.6.7/refinery/units/misc/nop.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/misc/urlfix.py` & `binary-refinery-0.6.7/refinery/units/misc/urlfix.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/misc/xkey.py` & `binary-refinery-0.6.7/refinery/units/misc/xkey.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/__init__.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/js/arrays.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/js/arrays.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/js/getattr.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/js/getattr.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/js/tuples.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/js/tuples.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/__init__.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/all.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/brackets.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/cases.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/cases.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/concat.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/format.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/format.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/invoke.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/invoke.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/securestring.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/securestring.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/stringreplace.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/typecast.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/typecast.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/ps1/uncurly.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/ps1/uncurly.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/vba/all.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/vba/all.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/vba/arithmetic.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/vba/arithmetic.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/vba/brackets.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/vba/brackets.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/vba/char.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/vba/char.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/vba/concat.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/vba/concat.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/vba/constants.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/vba/constants.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/vba/dummies.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/vba/dummies.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/vba/stringreplace.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/vba/stringreplace.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/obfuscation/vba/stringreverse.py` & `binary-refinery-0.6.7/refinery/units/obfuscation/vba/stringreverse.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/__init__.py` & `binary-refinery-0.6.7/refinery/units/pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/carve.py` & `binary-refinery-0.6.7/refinery/units/pattern/carve.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/carve_7z.py` & `binary-refinery-0.6.7/refinery/units/pattern/carve_7z.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/carve_json.py` & `binary-refinery-0.6.7/refinery/units/pattern/carve_json.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/carve_lnk.py` & `binary-refinery-0.6.7/refinery/units/pattern/carve_lnk.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/carve_pe.py` & `binary-refinery-0.6.7/refinery/units/pattern/carve_pe.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/carve_rtf.py` & `binary-refinery-0.6.7/refinery/units/pattern/carve_rtf.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/carve_xml.py` & `binary-refinery-0.6.7/refinery/units/pattern/carve_xml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/carve_zip.py` & `binary-refinery-0.6.7/refinery/units/pattern/carve_zip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/defang.py` & `binary-refinery-0.6.7/refinery/units/pattern/defang.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/dnsdomain.py` & `binary-refinery-0.6.7/refinery/units/pattern/dnsdomain.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/mimewords.py` & `binary-refinery-0.6.7/refinery/units/pattern/mimewords.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/resplit.py` & `binary-refinery-0.6.7/refinery/units/pattern/resplit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/resub.py` & `binary-refinery-0.6.7/refinery/units/pattern/resub.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/rex.py` & `binary-refinery-0.6.7/refinery/units/pattern/rex.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/struct_parser.py` & `binary-refinery-0.6.7/refinery/units/pattern/struct_parser.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/subfiles.py` & `binary-refinery-0.6.7/refinery/units/pattern/subfiles.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/urlguards.py` & `binary-refinery-0.6.7/refinery/units/pattern/urlguards.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/xtp.py` & `binary-refinery-0.6.7/refinery/units/pattern/xtp.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/pattern/xtw.py` & `binary-refinery-0.6.7/refinery/units/pattern/xtw.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import re
+
 from refinery.units.pattern import PatternExtractor
 from refinery.units import RefineryCriticalException
 from refinery.lib.patterns import wallets
 
 
 class xtw(PatternExtractor):
     """
@@ -11,17 +15,18 @@
     This works similar to the `refinery.xtp` unit.
     """
 
     def __init__(self, stripspace=False, duplicates=False, longest=False, take=None):
         self.superinit(super(), **vars(), ascii=True, utf16=True)
 
     def process(self, data):
-        pattern = '|'.join(F'(?P<{p.name}>{p.value})' for p in wallets).encode('latin1')
+        pattern = '|'.join(FR'(?P<{p.name}>\b{p.value}\b)' for p in wallets)
+        pattern = FR'\b{pattern}\b'.encode('latin1')
 
-        def check(match):
+        def check(match: re.Match[bytes]):
             for name, value in match.groupdict().items():
                 if value is not None:
                     break
             else:
                 raise RefineryCriticalException('Received empty match.')
             return self.labelled(value, kind=name)
```

### Comparing `binary-refinery-0.6.6/refinery/units/sinks/__init__.py` & `binary-refinery-0.6.7/refinery/units/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/sinks/asm.py` & `binary-refinery-0.6.7/refinery/units/sinks/asm.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/sinks/dump.py` & `binary-refinery-0.6.7/refinery/units/sinks/dump.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/sinks/iemap.py` & `binary-refinery-0.6.7/refinery/units/sinks/iemap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/sinks/peek.py` & `binary-refinery-0.6.7/refinery/units/sinks/peek.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/sinks/ppjscript.py` & `binary-refinery-0.6.7/refinery/units/sinks/ppjscript.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/sinks/ppjson.py` & `binary-refinery-0.6.7/refinery/units/sinks/ppjson.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/sinks/ppxml.py` & `binary-refinery-0.6.7/refinery/units/sinks/ppxml.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/strings/cfmt.py` & `binary-refinery-0.6.7/refinery/units/strings/cfmt.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/strings/cswap.py` & `binary-refinery-0.6.7/refinery/units/strings/cswap.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/strings/rep.py` & `binary-refinery-0.6.7/refinery/units/strings/rep.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/strings/repl.py` & `binary-refinery-0.6.7/refinery/units/strings/repl.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/strings/snip.py` & `binary-refinery-0.6.7/refinery/units/strings/snip.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/strings/stretch.py` & `binary-refinery-0.6.7/refinery/units/strings/stretch.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/strings/termfit.py` & `binary-refinery-0.6.7/refinery/units/strings/termfit.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/refinery/units/strings/trim.py` & `binary-refinery-0.6.7/refinery/units/strings/trim.py`

 * *Files identical despite different names*

### Comparing `binary-refinery-0.6.6/setup.py` & `binary-refinery-0.6.7/setup.py`

 * *Files identical despite different names*

