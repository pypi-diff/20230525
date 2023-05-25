# Comparing `tmp/tcod-9.2.5.tar.gz` & `tmp/tcod-9.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tcod-9.2.5.tar", last modified: Mon Mar  4 22:17:32 2019, max compression
+gzip compressed data, was "dist\tcod-9.3.0.tar", last modified: Sat Mar 16 00:17:31 2019, max compression
```

## Comparing `tcod-9.2.5.tar` & `tcod-9.3.0.tar`

### file list

```diff
@@ -1,435 +1,439 @@
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/
--rw-rw-rw-   0        0        0    14196 2019-03-04 22:16:05.000000 tcod-9.2.5/build_libtcod.py
--rw-rw-rw-   0        0        0    19224 2019-03-04 22:16:05.000000 tcod-9.2.5/CHANGELOG.rst
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:31.000000 tcod-9.2.5/dependencies/
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:31.000000 tcod-9.2.5/dependencies/fake_libc_include/
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/alloca.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/ar.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/argz.h
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:31.000000 tcod-9.2.5/dependencies/fake_libc_include/arpa/
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/arpa/inet.h
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:31.000000 tcod-9.2.5/dependencies/fake_libc_include/asm-generic/
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/asm-generic/int-ll64.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/assert.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/AvailabilityMacros.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx2intrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx5124fmapsintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx5124vnniwintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512bitalgintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512bwintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512cdintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512dqintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512erintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512fintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512ifmaintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512ifmavlintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512pfintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vbmi2intrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vbmi2vlintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vbmiintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vbmivlintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vlbwintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vldqintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vlintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vnniintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vnnivlintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vpopcntdqintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avx512vpopcntdqvlintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/avxintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/complex.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/ctype.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/dirent.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/dlfcn.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/emmintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/endian.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/envz.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/errno.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/fastmath.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/fcntl.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/features.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/fenv.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/float.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/getopt.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/grp.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/iconv.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/ieeefp.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/immintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/inttypes.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/iso646.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/langinfo.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/libgen.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/libintl.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/limits.h
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:31.000000 tcod-9.2.5/dependencies/fake_libc_include/linux/
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/linux/socket.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/linux/version.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/locale.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/malloc.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/math.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/mmintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/mm_malloc.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/netdb.h
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:31.000000 tcod-9.2.5/dependencies/fake_libc_include/netinet/
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/netinet/in.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/netinet/tcp.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/newlib.h
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:31.000000 tcod-9.2.5/dependencies/fake_libc_include/openssl/
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/openssl/err.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/openssl/evp.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/openssl/hmac.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/openssl/ssl.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/openssl/x509v3.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/paths.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/pmmintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/process.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/pthread.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/pwd.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/reent.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/regdef.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/regex.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sched.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/search.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/semaphore.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/setjmp.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/shaintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/signal.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/smmintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/stdarg.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/stdbool.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/stddef.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/stdint.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/stdio.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/stdlib.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/string.h
--rw-rw-rw-   0        0        0       19 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/strings.h
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:31.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/ioctl.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/mman.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/poll.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/resource.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/select.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/socket.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/stat.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/sysctl.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/time.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/types.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/uio.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/un.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/utsname.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/sys/wait.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/syslog.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/tar.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/TargetConditionals.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/termios.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/tgmath.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/time.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/tmmintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/unctrl.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/unistd.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/utime.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/utmp.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/wchar.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/wctype.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/wmmintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/x86intrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/xmmintrin.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/zlib.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/_ansi.h
--rw-rw-rw-   0        0        0      949 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/_fake_defines.h
--rw-rw-rw-   0        0        0     3649 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/_fake_typedefs.h
--rw-rw-rw-   0        0        0       55 2019-03-04 22:16:05.000000 tcod-9.2.5/dependencies/fake_libc_include/_syslist.h
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:31.000000 tcod-9.2.5/libtcod/
--rw-rw-rw-   0        0        0    46304 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/CHANGELOG.md
--rw-rw-rw-   0        0        0     2425 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/LIBTCOD-CREDITS.txt
--rw-rw-rw-   0        0        0     1626 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/LIBTCOD-LICENSE.txt
--rw-rw-rw-   0        0        0     5210 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/README.md
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:31.000000 tcod-9.2.5/libtcod/src/
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/libtcod/
--rw-rw-rw-   0        0        0     2233 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/bresenham.cpp
--rw-rw-rw-   0        0        0     3205 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/bresenham.h
--rw-rw-rw-   0        0        0     5419 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/bresenham.hpp
--rw-rw-rw-   0        0        0     6871 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/bresenham_c.c
--rw-rw-rw-   0        0        0     5942 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/bsp.cpp
--rw-rw-rw-   0        0        0     3635 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/bsp.h
--rw-rw-rw-   0        0        0    17873 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/bsp.hpp
--rw-rw-rw-   0        0        0     8141 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/bsp_c.c
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/libtcod/color/
--rw-rw-rw-   0        0        0     3022 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/color/canvas.cpp
--rw-rw-rw-   0        0        0     2147 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/color/canvas.h
--rw-rw-rw-   0        0        0     2379 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/color/color.h
--rw-rw-rw-   0        0        0    20135 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/color.cpp
--rw-rw-rw-   0        0        0    16268 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/color.h
--rw-rw-rw-   0        0        0    27085 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/color.hpp
--rw-rw-rw-   0        0        0    28212 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/color_c.c
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/libtcod/console/
--rw-rw-rw-   0        0        0     4230 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console/drawing.cpp
--rw-rw-rw-   0        0        0     4415 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console/drawing.h
--rw-rw-rw-   0        0        0    41411 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console/printing.cpp
--rw-rw-rw-   0        0        0     6375 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console/printing.h
--rw-rw-rw-   0        0        0    13426 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console/rexpaint.cpp
--rw-rw-rw-   0        0        0     2306 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console/rexpaint.h
--rw-rw-rw-   0        0        0    14278 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console.cpp
--rw-rw-rw-   0        0        0     6645 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console.h
--rw-rw-rw-   0        0        0    85862 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console.hpp
--rw-rw-rw-   0        0        0    54813 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console_c.cpp
--rw-rw-rw-   0        0        0     8436 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/console_types.h
--rw-rw-rw-   0        0        0     1863 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/deprecated.cpp
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/libtcod/engine/
--rw-rw-rw-   0        0        0     1647 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/engine/backend.cpp
--rw-rw-rw-   0        0        0     2408 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/engine/backend.h
--rw-rw-rw-   0        0        0     4841 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/engine/display.cpp
--rw-rw-rw-   0        0        0     5644 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/engine/display.h
--rw-rw-rw-   0        0        0     2662 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/engine/globals.cpp
--rw-rw-rw-   0        0        0     2988 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/engine/globals.h
--rw-rw-rw-   0        0        0     2858 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/fov.cpp
--rw-rw-rw-   0        0        0     3202 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/fov.h
--rw-rw-rw-   0        0        0    11766 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/fov.hpp
--rw-rw-rw-   0        0        0     7289 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/fov_c.c
--rw-rw-rw-   0        0        0     8212 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/fov_circular_raycasting.c
--rw-rw-rw-   0        0        0     6928 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/fov_diamond_raycasting.c
--rw-rw-rw-   0        0        0     8993 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/fov_permissive2.c
--rw-rw-rw-   0        0        0     3903 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/fov_recursive_shadowcasting.c
--rw-rw-rw-   0        0        0     9711 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/fov_restrictive.c
--rw-rw-rw-   0        0        0     2936 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/fov_types.h
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/libtcod/gui/
--rw-rw-rw-   0        0        0     3244 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/button.cpp
--rw-rw-rw-   0        0        0     2325 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/button.hpp
--rw-rw-rw-   0        0        0     2325 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/container.cpp
--rw-rw-rw-   0        0        0     2088 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/container.hpp
--rw-rw-rw-   0        0        0     3379 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/flatlist.cpp
--rw-rw-rw-   0        0        0     2386 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/flatlist.hpp
--rw-rw-rw-   0        0        0     2019 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/gui.hpp
--rw-rw-rw-   0        0        0     1905 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/gui_portability.hpp
--rw-rw-rw-   0        0        0     2139 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/hbox.cpp
--rw-rw-rw-   0        0        0     1839 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/hbox.hpp
--rw-rw-rw-   0        0        0     2063 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/image.cpp
--rw-rw-rw-   0        0        0     1997 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/image.hpp
--rw-rw-rw-   0        0        0     2107 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/label.cpp
--rw-rw-rw-   0        0        0     2020 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/label.hpp
--rw-rw-rw-   0        0        0     2301 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/radiobutton.cpp
--rw-rw-rw-   0        0        0     2488 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/radiobutton.hpp
--rw-rw-rw-   0        0        0     4012 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/slider.cpp
--rw-rw-rw-   0        0        0     2563 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/slider.hpp
--rw-rw-rw-   0        0        0     1897 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/statusbar.cpp
--rw-rw-rw-   0        0        0     1880 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/statusbar.hpp
--rw-rw-rw-   0        0        0     5109 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/textbox.cpp
--rw-rw-rw-   0        0        0     2449 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/textbox.hpp
--rw-rw-rw-   0        0        0     2297 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/togglebutton.cpp
--rw-rw-rw-   0        0        0     2327 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/togglebutton.hpp
--rw-rw-rw-   0        0        0     4044 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/toolbar.cpp
--rw-rw-rw-   0        0        0     2125 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/toolbar.hpp
--rw-rw-rw-   0        0        0     2076 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/vbox.cpp
--rw-rw-rw-   0        0        0     1915 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/vbox.hpp
--rw-rw-rw-   0        0        0     4389 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/widget.cpp
--rw-rw-rw-   0        0        0     3339 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/gui/widget.hpp
--rw-rw-rw-   0        0        0     6796 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/heightmap.cpp
--rw-rw-rw-   0        0        0     5254 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/heightmap.h
--rw-rw-rw-   0        0        0    25922 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/heightmap.hpp
--rw-rw-rw-   0        0        0    16884 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/heightmap_c.c
--rw-rw-rw-   0        0        0     4346 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/image.cpp
--rw-rw-rw-   0        0        0     4295 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/image.h
--rw-rw-rw-   0        0        0    20674 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/image.hpp
--rw-rw-rw-   0        0        0    30707 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/image_c.cpp
--rw-rw-rw-   0        0        0     3261 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/lex.cpp
--rw-rw-rw-   0        0        0     4241 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/lex.h
--rw-rw-rw-   0        0        0     3294 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/lex.hpp
--rw-rw-rw-   0        0        0    17556 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/lex_c.c
--rw-rw-rw-   0        0        0     2816 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/libtcod.h
--rw-rw-rw-   0        0        0     1647 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/libtcod.hpp
--rw-rw-rw-   0        0        0    20819 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/libtcod_int.h
--rw-rw-rw-   0        0        0     3215 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/list.h
--rw-rw-rw-   0        0        0    21887 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/list.hpp
--rw-rw-rw-   0        0        0     8600 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/list_c.c
--rw-rw-rw-   0        0        0     2426 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/mersenne.cpp
--rw-rw-rw-   0        0        0     3140 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/mersenne.h
--rw-rw-rw-   0        0        0    19955 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/mersenne.hpp
--rw-rw-rw-   0        0        0    18877 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/mersenne_c.c
--rw-rw-rw-   0        0        0     2198 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/mersenne_types.h
--rw-rw-rw-   0        0        0     1985 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/mouse.cpp
--rw-rw-rw-   0        0        0     2149 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/mouse.h
--rw-rw-rw-   0        0        0     3677 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/mouse.hpp
--rw-rw-rw-   0        0        0     2388 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/mouse_types.h
--rw-rw-rw-   0        0        0     2262 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/namegen.cpp
--rw-rw-rw-   0        0        0     2531 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/namegen.h
--rw-rw-rw-   0        0        0    16603 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/namegen.hpp
--rw-rw-rw-   0        0        0    24327 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/namegen_c.c
--rw-rw-rw-   0        0        0     3311 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/noise.cpp
--rw-rw-rw-   0        0        0     3295 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/noise.h
--rw-rw-rw-   0        0        0    15776 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/noise.hpp
--rw-rw-rw-   0        0        0    27033 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/noise_c.c
--rw-rw-rw-   0        0        0     1884 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/noise_defaults.h
--rw-rw-rw-   0        0        0     6287 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/parser.cpp
--rw-rw-rw-   0        0        0     7578 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/parser.h
--rw-rw-rw-   0        0        0    33242 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/parser.hpp
--rw-rw-rw-   0        0        0    31706 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/parser_c.c
--rw-rw-rw-   0        0        0     4447 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/path.cpp
--rw-rw-rw-   0        0        0     3817 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/path.h
--rw-rw-rw-   0        0        0    22352 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/path.hpp
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/libtcod/pathfinding/
--rw-rw-rw-   0        0        0     1645 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/pathfinding/astar.cpp
--rw-rw-rw-   0        0        0     1868 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/pathfinding/astar.h
--rw-rw-rw-   0        0        0     1648 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/pathfinding/dijkstra.cpp
--rw-rw-rw-   0        0        0     4607 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/pathfinding/dijkstra.h
--rw-rw-rw-   0        0        0     1647 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/pathfinding/generic.cpp
--rw-rw-rw-   0        0        0     6120 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/pathfinding/generic.h
--rw-rw-rw-   0        0        0    24611 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/path_c.c
--rw-rw-rw-   0        0        0     5808 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/portability.h
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/
--rw-rw-rw-   0        0        0     1496 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/console_2tris.glslf
--rw-rw-rw-   0        0        0      527 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/console_2tris.glslv
--rw-rw-rw-   0        0        0      273 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/console_grid.glslf
--rw-rw-rw-   0        0        0      527 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/console_grid.glslv
--rw-rw-rw-   0        0        0     3169 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_display.cpp
--rw-rw-rw-   0        0        0     2344 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_display.h
--rw-rw-rw-   0        0        0     2633 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_ext_.h
--rw-rw-rw-   0        0        0     6323 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_raii.cpp
--rw-rw-rw-   0        0        0     5360 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_raii.h
--rw-rw-rw-   0        0        0    13354 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_renderer.cpp
--rw-rw-rw-   0        0        0     2765 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_renderer.h
--rw-rw-rw-   0        0        0     9172 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/gl_alias.cpp
--rw-rw-rw-   0        0        0     2689 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/gl_alias.h
--rw-rw-rw-   0        0        0     1654 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/legacy_backend.cpp
--rw-rw-rw-   0        0        0     1867 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/legacy_backend.h
--rw-rw-rw-   0        0        0     9651 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_alias.cpp
--rw-rw-rw-   0        0        0     2890 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_alias.h
--rw-rw-rw-   0        0        0     5232 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_display.cpp
--rw-rw-rw-   0        0        0     3782 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_display.h
--rw-rw-rw-   0        0        0     6998 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_renderer.cpp
--rw-rw-rw-   0        0        0     2797 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_renderer.h
--rw-rw-rw-   0        0        0     6567 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sys.cpp
--rw-rw-rw-   0        0        0     7141 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sys.h
--rw-rw-rw-   0        0        0    25114 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sys.hpp
--rw-rw-rw-   0        0        0    14161 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sys_c.cpp
--rw-rw-rw-   0        0        0    22727 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sys_opengl_c.cpp
--rw-rw-rw-   0        0        0    19580 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sys_sdl2_c.cpp
--rw-rw-rw-   0        0        0    72570 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sys_sdl_c.cpp
--rw-rw-rw-   0        0        0     2662 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sys_sdl_img_bmp.cpp
--rw-rw-rw-   0        0        0     4272 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/sys_sdl_img_png.cpp
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/
--rw-rw-rw-   0        0        0     1728 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/observer.cpp
--rw-rw-rw-   0        0        0     3606 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/observer.h
--rw-rw-rw-   0        0        0     1644 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/tile.cpp
--rw-rw-rw-   0        0        0     2577 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/tile.h
--rw-rw-rw-   0        0        0     2060 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/tileset.cpp
--rw-rw-rw-   0        0        0     5115 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/tileset.h
--rw-rw-rw-   0        0        0     7467 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/tilesheet.cpp
--rw-rw-rw-   0        0        0     3041 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/tilesheet.h
--rw-rw-rw-   0        0        0     3649 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/truetype.cpp
--rw-rw-rw-   0        0        0      655 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tileset/truetype.h
--rw-rw-rw-   0        0        0     2020 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tree.h
--rw-rw-rw-   0        0        0     2061 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tree.hpp
--rw-rw-rw-   0        0        0     2006 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/tree_c.c
--rw-rw-rw-   0        0        0     2750 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/txtfield.cpp
--rw-rw-rw-   0        0        0     2732 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/txtfield.h
--rw-rw-rw-   0        0        0     2291 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/txtfield.hpp
--rw-rw-rw-   0        0        0    20680 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/txtfield_c.c
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/libtcod/utility/
--rw-rw-rw-   0        0        0     6080 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/utility/vector2.h
--rw-rw-rw-   0        0        0     2015 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/utility.h
--rw-rw-rw-   0        0        0     2111 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/version.h
--rw-rw-rw-   0        0        0    10960 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/wrappers.c
--rw-rw-rw-   0        0        0     6797 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/wrappers.h
--rw-rw-rw-   0        0        0     3658 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/zip.cpp
--rw-rw-rw-   0        0        0     3578 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/zip.h
--rw-rw-rw-   0        0        0    12280 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/zip.hpp
--rw-rw-rw-   0        0        0    11859 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod/zip_c.c
--rw-rw-rw-   0        0        0     4042 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod.cpp
--rw-rw-rw-   0        0        0     1655 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod.h
--rw-rw-rw-   0        0        0     1647 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod.hpp
--rw-rw-rw-   0        0        0     3274 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/libtcod_c.c
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/vendor/
--rw-rw-rw-   0        0        0    70416 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/glad.c
--rw-rw-rw-   0        0        0   127491 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/glad.h
--rw-rw-rw-   0        0        0    10037 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/khrplatform.h
--rw-rw-rw-   0        0        0   223161 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/lodepng.cpp
--rw-rw-rw-   0        0        0    82947 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/lodepng.h
--rw-rw-rw-   0        0        0      193 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/stb.c
--rw-rw-rw-   0        0        0    56319 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/stb_sprintf.h
--rw-rw-rw-   0        0        0   191762 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/stb_truetype.h
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/vendor/utf8proc/
--rw-rw-rw-   0        0        0    30127 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/utf8proc/utf8proc.c
--rw-rw-rw-   0        0        0    29484 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/utf8proc/utf8proc.h
--rw-rw-rw-   0        0        0  1614402 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/utf8proc/utf8proc_data.c
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/libtcod/src/vendor/zlib/
--rw-rw-rw-   0        0        0     5204 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/adler32.c
--rw-rw-rw-   0        0        0     2699 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/compress.c
--rw-rw-rw-   0        0        0    14053 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/crc32.c
--rw-rw-rw-   0        0        0    30562 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/crc32.h
--rw-rw-rw-   0        0        0    78889 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/deflate.c
--rw-rw-rw-   0        0        0    13150 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/deflate.h
--rw-rw-rw-   0        0        0      678 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/gzclose.c
--rw-rw-rw-   0        0        0     6819 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/gzguts.h
--rw-rw-rw-   0        0        0    16599 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/gzlib.c
--rw-rw-rw-   0        0        0    20428 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/gzread.c
--rw-rw-rw-   0        0        0    19253 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/gzwrite.c
--rw-rw-rw-   0        0        0    22715 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/infback.c
--rw-rw-rw-   0        0        0    12978 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/inffast.c
--rw-rw-rw-   0        0        0      427 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/inffast.h
--rw-rw-rw-   0        0        0     6332 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/inffixed.h
--rw-rw-rw-   0        0        0    54800 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/inflate.c
--rw-rw-rw-   0        0        0     6618 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/inflate.h
--rw-rw-rw-   0        0        0    12999 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/inftrees.c
--rw-rw-rw-   0        0        0     2928 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/inftrees.h
--rw-rw-rw-   0        0        0    43761 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/trees.c
--rw-rw-rw-   0        0        0     8472 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/trees.h
--rw-rw-rw-   0        0        0     2966 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/uncompr.c
--rw-rw-rw-   0        0        0    16298 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/zconf.h
--rw-rw-rw-   0        0        0    96239 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/zlib.h
--rw-rw-rw-   0        0        0     7304 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/zutil.c
--rw-rw-rw-   0        0        0     7127 2019-03-04 22:16:27.000000 tcod-9.2.5/libtcod/src/vendor/zlib/zutil.h
--rw-rw-rw-   0        0        0      196 2019-03-04 22:16:05.000000 tcod-9.2.5/libtcodpy.py
--rw-rw-rw-   0        0        0     1386 2019-03-04 22:16:05.000000 tcod-9.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0      337 2019-03-04 22:16:05.000000 tcod-9.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0    32152 2019-03-04 22:17:32.000000 tcod-9.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4879 2019-03-04 22:16:05.000000 tcod-9.2.5/README.rst
--rw-rw-rw-   0        0        0       71 2019-03-04 22:16:05.000000 tcod-9.2.5/requirements.txt
--rw-rw-rw-   0        0        0      248 2019-03-04 22:17:32.000000 tcod-9.2.5/setup.cfg
--rw-rw-rw-   0        0        0     4636 2019-03-04 22:16:05.000000 tcod-9.2.5/setup.py
--rw-rw-rw-   0        0        0      242 2019-03-04 22:16:05.000000 tcod-9.2.5/stdeb.cfg
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/tcod/
--rw-rw-rw-   0        0        0     8282 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/bsp.py
--rw-rw-rw-   0        0        0      881 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/cdef.h
--rw-rw-rw-   0        0        0      519 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/cffi.h
--rw-rw-rw-   0        0        0     4200 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/color.py
--rw-rw-rw-   0        0        0    36863 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/console.py
--rw-rw-rw-   0        0        0    21696 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/constants.py
--rw-rw-rw-   0        0        0    21459 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/event.py
--rw-rw-rw-   0        0        0    39424 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/event_constants.py
--rw-rw-rw-   0        0        0    10044 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/image.py
--rw-rw-rw-   0        0        0     1393 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/libtcod.py
--rw-rw-rw-   0        0        0   120335 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/libtcodpy.py
--rw-rw-rw-   0        0        0     4405 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/map.py
--rw-rw-rw-   0        0        0     2110 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/noise.c
--rw-rw-rw-   0        0        0     1012 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/noise.h
--rw-rw-rw-   0        0        0    10140 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/noise.py
--rw-rw-rw-   0        0        0     1544 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/path.cpp
--rw-rw-rw-   0        0        0     1539 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/path.h
--rw-rw-rw-   0        0        0    10153 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/path.py
--rw-rw-rw-   0        0        0      876 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/path2.py
--rw-rw-rw-   0        0        0        0 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/py.typed
--rw-rw-rw-   0        0        0      931 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/random.h
--rw-rw-rw-   0        0        0     4474 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/random.py
--rw-rw-rw-   0        0        0     2610 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/tcod.cpp
--rw-rw-rw-   0        0        0     1409 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/tcod.h
--rw-rw-rw-   0        0        0     4690 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/tcod.py
--rw-rw-rw-   0        0        0     7057 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/tdl.c
--rw-rw-rw-   0        0        0     2333 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/tdl.h
--rw-rw-rw-   0        0        0     1015 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/tileset.py
--rw-rw-rw-   0        0        0       23 2019-03-04 22:17:03.000000 tcod-9.2.5/tcod/version.py
--rw-rw-rw-   0        0        0      952 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/_internal.py
--rw-rw-rw-   0        0        0      899 2019-03-04 22:16:05.000000 tcod-9.2.5/tcod/__init__.py
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/tcod.egg-info/
--rw-rw-rw-   0        0        0        1 2019-03-04 22:17:31.000000 tcod-9.2.5/tcod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    32152 2019-03-04 22:17:31.000000 tcod-9.2.5/tcod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       30 2019-03-04 22:17:31.000000 tcod-9.2.5/tcod.egg-info/requires.txt
--rw-rw-rw-   0        0        0    14690 2019-03-04 22:17:31.000000 tcod-9.2.5/tcod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       19 2019-03-04 22:17:31.000000 tcod-9.2.5/tcod.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2019-03-04 22:17:32.000000 tcod-9.2.5/tdl/
--rw-rw-rw-   0        0        0    18298 2019-03-04 22:16:05.000000 tcod-9.2.5/tdl/event.py
--rw-rw-rw-   0        0        0    12296 2019-03-04 22:16:05.000000 tcod-9.2.5/tdl/map.py
--rw-rw-rw-   0        0        0     5915 2019-03-04 22:16:05.000000 tcod-9.2.5/tdl/noise.py
--rw-rw-rw-   0        0        0      943 2019-03-04 22:16:05.000000 tcod-9.2.5/tdl/style.py
--rw-rw-rw-   0        0        0     3150 2019-03-04 22:16:05.000000 tcod-9.2.5/tdl/terminal8x8.png
--rw-rw-rw-   0        0        0       29 2019-03-04 22:16:05.000000 tcod-9.2.5/tdl/version.py
--rw-rw-rw-   0        0        0    51651 2019-03-04 22:16:05.000000 tcod-9.2.5/tdl/__init__.py
--rw-rw-rw-   0        0        0      143 2019-03-04 22:16:05.000000 tcod-9.2.5/unittest.cfg
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/
+-rw-rw-rw-   0        0        0    14196 2019-03-16 00:16:40.000000 tcod-9.3.0/build_libtcod.py
+-rw-rw-rw-   0        0        0    20161 2019-03-16 00:16:40.000000 tcod-9.3.0/CHANGELOG.rst
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/dependencies/
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/dependencies/fake_libc_include/
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/alloca.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/ar.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/argz.h
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/dependencies/fake_libc_include/arpa/
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/arpa/inet.h
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/dependencies/fake_libc_include/asm-generic/
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/asm-generic/int-ll64.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/assert.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/AvailabilityMacros.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx2intrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx5124fmapsintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx5124vnniwintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512bitalgintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512bwintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512cdintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512dqintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512erintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512fintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512ifmaintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512ifmavlintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512pfintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vbmi2intrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vbmi2vlintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vbmiintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vbmivlintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vlbwintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vldqintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vlintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vnniintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vnnivlintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vpopcntdqintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avx512vpopcntdqvlintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/avxintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/complex.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/ctype.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/dirent.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/dlfcn.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/emmintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/endian.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/envz.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/errno.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/fastmath.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/fcntl.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/features.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/fenv.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/float.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/getopt.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/grp.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/iconv.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/ieeefp.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/immintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/inttypes.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/iso646.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/langinfo.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/libgen.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/libintl.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/limits.h
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/dependencies/fake_libc_include/linux/
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/linux/socket.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/linux/version.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/locale.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/malloc.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/math.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/mmintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/mm_malloc.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/netdb.h
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/dependencies/fake_libc_include/netinet/
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/netinet/in.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/netinet/tcp.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/newlib.h
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/dependencies/fake_libc_include/openssl/
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/openssl/err.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/openssl/evp.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/openssl/hmac.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/openssl/ssl.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/openssl/x509v3.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/paths.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/pmmintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/process.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/pthread.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/pwd.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/reent.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/regdef.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/regex.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sched.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/search.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/semaphore.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/setjmp.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/shaintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/signal.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/smmintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/stdarg.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/stdbool.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/stddef.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/stdint.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/stdio.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/stdlib.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/string.h
+-rw-rw-rw-   0        0        0       19 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/strings.h
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/ioctl.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/mman.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/poll.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/resource.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/select.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/socket.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/stat.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/sysctl.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/time.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/types.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/uio.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/un.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/utsname.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/sys/wait.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/syslog.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/tar.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/TargetConditionals.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/termios.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/tgmath.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/time.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/tmmintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/unctrl.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/unistd.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/utime.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/utmp.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/wchar.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/wctype.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/wmmintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/x86intrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/xmmintrin.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/zlib.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/_ansi.h
+-rw-rw-rw-   0        0        0      949 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/_fake_defines.h
+-rw-rw-rw-   0        0        0     3649 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/_fake_typedefs.h
+-rw-rw-rw-   0        0        0       55 2019-03-16 00:16:40.000000 tcod-9.3.0/dependencies/fake_libc_include/_syslist.h
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/
+-rw-rw-rw-   0        0        0    47227 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/CHANGELOG.md
+-rw-rw-rw-   0        0        0     2425 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/LIBTCOD-CREDITS.txt
+-rw-rw-rw-   0        0        0     1546 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/LICENSE.txt
+-rw-rw-rw-   0        0        0     5210 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/README.md
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/libtcod/
+-rw-rw-rw-   0        0        0     2241 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/bresenham.cpp
+-rw-rw-rw-   0        0        0     3213 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/bresenham.h
+-rw-rw-rw-   0        0        0     5427 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/bresenham.hpp
+-rw-rw-rw-   0        0        0     6879 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/bresenham_c.c
+-rw-rw-rw-   0        0        0     5950 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/bsp.cpp
+-rw-rw-rw-   0        0        0     3643 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/bsp.h
+-rw-rw-rw-   0        0        0    17881 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/bsp.hpp
+-rw-rw-rw-   0        0        0     8149 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/bsp_c.c
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/libtcod/color/
+-rw-rw-rw-   0        0        0     3030 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/color/canvas.cpp
+-rw-rw-rw-   0        0        0     2155 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/color/canvas.h
+-rw-rw-rw-   0        0        0     2387 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/color/color.h
+-rw-rw-rw-   0        0        0    20143 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/color.cpp
+-rw-rw-rw-   0        0        0    16276 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/color.h
+-rw-rw-rw-   0        0        0    27093 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/color.hpp
+-rw-rw-rw-   0        0        0    28220 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/color_c.c
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/libtcod/console/
+-rw-rw-rw-   0        0        0     4238 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console/drawing.cpp
+-rw-rw-rw-   0        0        0     4423 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console/drawing.h
+-rw-rw-rw-   0        0        0    41419 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console/printing.cpp
+-rw-rw-rw-   0        0        0     6383 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console/printing.h
+-rw-rw-rw-   0        0        0    13434 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console/rexpaint.cpp
+-rw-rw-rw-   0        0        0     2314 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console/rexpaint.h
+-rw-rw-rw-   0        0        0    14329 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console.cpp
+-rw-rw-rw-   0        0        0     6653 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console.h
+-rw-rw-rw-   0        0        0    85870 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console.hpp
+-rw-rw-rw-   0        0        0    54821 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console_c.cpp
+-rw-rw-rw-   0        0        0     8444 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/console_types.h
+-rw-rw-rw-   0        0        0     1871 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/deprecated.cpp
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/libtcod/engine/
+-rw-rw-rw-   0        0        0     1655 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/engine/backend.cpp
+-rw-rw-rw-   0        0        0     2416 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/engine/backend.h
+-rw-rw-rw-   0        0        0     6177 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/engine/display.cpp
+-rw-rw-rw-   0        0        0     7464 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/engine/display.h
+-rw-rw-rw-   0        0        0     2670 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/engine/globals.cpp
+-rw-rw-rw-   0        0        0     2996 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/engine/globals.h
+-rw-rw-rw-   0        0        0     2866 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/fov.cpp
+-rw-rw-rw-   0        0        0     3210 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/fov.h
+-rw-rw-rw-   0        0        0    11774 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/fov.hpp
+-rw-rw-rw-   0        0        0     7297 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/fov_c.c
+-rw-rw-rw-   0        0        0     8220 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/fov_circular_raycasting.c
+-rw-rw-rw-   0        0        0     6936 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/fov_diamond_raycasting.c
+-rw-rw-rw-   0        0        0     9001 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/fov_permissive2.c
+-rw-rw-rw-   0        0        0     3911 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/fov_recursive_shadowcasting.c
+-rw-rw-rw-   0        0        0     9719 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/fov_restrictive.c
+-rw-rw-rw-   0        0        0     2944 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/fov_types.h
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/libtcod/gui/
+-rw-rw-rw-   0        0        0     3252 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/button.cpp
+-rw-rw-rw-   0        0        0     2333 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/button.hpp
+-rw-rw-rw-   0        0        0     2333 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/container.cpp
+-rw-rw-rw-   0        0        0     2096 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/container.hpp
+-rw-rw-rw-   0        0        0     3387 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/flatlist.cpp
+-rw-rw-rw-   0        0        0     2394 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/flatlist.hpp
+-rw-rw-rw-   0        0        0     2027 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/gui.hpp
+-rw-rw-rw-   0        0        0     1913 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/gui_portability.hpp
+-rw-rw-rw-   0        0        0     2147 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/hbox.cpp
+-rw-rw-rw-   0        0        0     1847 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/hbox.hpp
+-rw-rw-rw-   0        0        0     2071 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/image.cpp
+-rw-rw-rw-   0        0        0     2005 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/image.hpp
+-rw-rw-rw-   0        0        0     2115 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/label.cpp
+-rw-rw-rw-   0        0        0     2028 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/label.hpp
+-rw-rw-rw-   0        0        0     2309 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/radiobutton.cpp
+-rw-rw-rw-   0        0        0     2496 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/radiobutton.hpp
+-rw-rw-rw-   0        0        0     4020 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/slider.cpp
+-rw-rw-rw-   0        0        0     2571 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/slider.hpp
+-rw-rw-rw-   0        0        0     1905 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/statusbar.cpp
+-rw-rw-rw-   0        0        0     1888 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/statusbar.hpp
+-rw-rw-rw-   0        0        0     5117 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/textbox.cpp
+-rw-rw-rw-   0        0        0     2457 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/textbox.hpp
+-rw-rw-rw-   0        0        0     2305 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/togglebutton.cpp
+-rw-rw-rw-   0        0        0     2335 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/togglebutton.hpp
+-rw-rw-rw-   0        0        0     4052 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/toolbar.cpp
+-rw-rw-rw-   0        0        0     2133 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/toolbar.hpp
+-rw-rw-rw-   0        0        0     2084 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/vbox.cpp
+-rw-rw-rw-   0        0        0     1923 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/vbox.hpp
+-rw-rw-rw-   0        0        0     4397 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/widget.cpp
+-rw-rw-rw-   0        0        0     3347 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/gui/widget.hpp
+-rw-rw-rw-   0        0        0     6804 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/heightmap.cpp
+-rw-rw-rw-   0        0        0     5262 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/heightmap.h
+-rw-rw-rw-   0        0        0    25930 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/heightmap.hpp
+-rw-rw-rw-   0        0        0    16892 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/heightmap_c.c
+-rw-rw-rw-   0        0        0     4354 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/image.cpp
+-rw-rw-rw-   0        0        0     4303 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/image.h
+-rw-rw-rw-   0        0        0    20682 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/image.hpp
+-rw-rw-rw-   0        0        0    30715 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/image_c.cpp
+-rw-rw-rw-   0        0        0     3269 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/lex.cpp
+-rw-rw-rw-   0        0        0     4249 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/lex.h
+-rw-rw-rw-   0        0        0     3302 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/lex.hpp
+-rw-rw-rw-   0        0        0    17564 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/lex_c.c
+-rw-rw-rw-   0        0        0     2849 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/libtcod.h
+-rw-rw-rw-   0        0        0     1655 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/libtcod.hpp
+-rw-rw-rw-   0        0        0    21245 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/libtcod_int.h
+-rw-rw-rw-   0        0        0     3223 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/list.h
+-rw-rw-rw-   0        0        0    21895 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/list.hpp
+-rw-rw-rw-   0        0        0     8608 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/list_c.c
+-rw-rw-rw-   0        0        0     2434 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/mersenne.cpp
+-rw-rw-rw-   0        0        0     3148 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/mersenne.h
+-rw-rw-rw-   0        0        0    19963 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/mersenne.hpp
+-rw-rw-rw-   0        0        0    18885 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/mersenne_c.c
+-rw-rw-rw-   0        0        0     2206 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/mersenne_types.h
+-rw-rw-rw-   0        0        0     1993 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/mouse.cpp
+-rw-rw-rw-   0        0        0     2157 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/mouse.h
+-rw-rw-rw-   0        0        0     3685 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/mouse.hpp
+-rw-rw-rw-   0        0        0     2396 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/mouse_types.h
+-rw-rw-rw-   0        0        0     2270 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/namegen.cpp
+-rw-rw-rw-   0        0        0     2539 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/namegen.h
+-rw-rw-rw-   0        0        0    16611 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/namegen.hpp
+-rw-rw-rw-   0        0        0    24335 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/namegen_c.c
+-rw-rw-rw-   0        0        0     3319 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/noise.cpp
+-rw-rw-rw-   0        0        0     3303 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/noise.h
+-rw-rw-rw-   0        0        0    15784 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/noise.hpp
+-rw-rw-rw-   0        0        0    27041 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/noise_c.c
+-rw-rw-rw-   0        0        0     1892 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/noise_defaults.h
+-rw-rw-rw-   0        0        0     6295 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/parser.cpp
+-rw-rw-rw-   0        0        0     7586 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/parser.h
+-rw-rw-rw-   0        0        0    33250 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/parser.hpp
+-rw-rw-rw-   0        0        0    31714 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/parser_c.c
+-rw-rw-rw-   0        0        0     4455 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/path.cpp
+-rw-rw-rw-   0        0        0     3825 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/path.h
+-rw-rw-rw-   0        0        0    22360 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/path.hpp
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/libtcod/pathfinding/
+-rw-rw-rw-   0        0        0     1653 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/pathfinding/astar.cpp
+-rw-rw-rw-   0        0        0     1876 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/pathfinding/astar.h
+-rw-rw-rw-   0        0        0     1656 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/pathfinding/dijkstra.cpp
+-rw-rw-rw-   0        0        0     4615 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/pathfinding/dijkstra.h
+-rw-rw-rw-   0        0        0     1655 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/pathfinding/generic.cpp
+-rw-rw-rw-   0        0        0     6128 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/pathfinding/generic.h
+-rw-rw-rw-   0        0        0    24619 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/path_c.c
+-rw-rw-rw-   0        0        0     5816 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/portability.h
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/
+-rw-rw-rw-   0        0        0     1496 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/console_2tris.glslf
+-rw-rw-rw-   0        0        0      527 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/console_2tris.glslv
+-rw-rw-rw-   0        0        0      273 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/console_grid.glslf
+-rw-rw-rw-   0        0        0      527 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/console_grid.glslv
+-rw-rw-rw-   0        0        0     2527 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/event.cpp
+-rw-rw-rw-   0        0        0     3266 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/event.h
+-rw-rw-rw-   0        0        0     3274 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_display.cpp
+-rw-rw-rw-   0        0        0     2408 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_display.h
+-rw-rw-rw-   0        0        0     2641 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_ext_.h
+-rw-rw-rw-   0        0        0     6331 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_raii.cpp
+-rw-rw-rw-   0        0        0     5368 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_raii.h
+-rw-rw-rw-   0        0        0    13362 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_renderer.cpp
+-rw-rw-rw-   0        0        0     2773 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_renderer.h
+-rw-rw-rw-   0        0        0     9180 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/gl_alias.cpp
+-rw-rw-rw-   0        0        0     2697 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/gl_alias.h
+-rw-rw-rw-   0        0        0     1662 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/legacy_backend.cpp
+-rw-rw-rw-   0        0        0     1875 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/legacy_backend.h
+-rw-rw-rw-   0        0        0     9659 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_alias.cpp
+-rw-rw-rw-   0        0        0     2898 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_alias.h
+-rw-rw-rw-   0        0        0     5887 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_display.cpp
+-rw-rw-rw-   0        0        0     4184 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_display.h
+-rw-rw-rw-   0        0        0     7006 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_renderer.cpp
+-rw-rw-rw-   0        0        0     2805 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_renderer.h
+-rw-rw-rw-   0        0        0     6575 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sys.cpp
+-rw-rw-rw-   0        0        0     7149 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sys.h
+-rw-rw-rw-   0        0        0    25122 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sys.hpp
+-rw-rw-rw-   0        0        0    14169 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sys_c.cpp
+-rw-rw-rw-   0        0        0    22735 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sys_opengl_c.cpp
+-rw-rw-rw-   0        0        0    19588 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sys_sdl2_c.cpp
+-rw-rw-rw-   0        0        0    72817 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sys_sdl_c.cpp
+-rw-rw-rw-   0        0        0     2670 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sys_sdl_img_bmp.cpp
+-rw-rw-rw-   0        0        0     4280 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/sys_sdl_img_png.cpp
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/
+-rw-rw-rw-   0        0        0     2332 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/fallback.cpp
+-rw-rw-rw-   0        0        0     2216 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/fallback.h
+-rw-rw-rw-   0        0        0     1736 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/observer.cpp
+-rw-rw-rw-   0        0        0     3614 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/observer.h
+-rw-rw-rw-   0        0        0     1652 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/tile.cpp
+-rw-rw-rw-   0        0        0     2585 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/tile.h
+-rw-rw-rw-   0        0        0     2068 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/tileset.cpp
+-rw-rw-rw-   0        0        0     5123 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/tileset.h
+-rw-rw-rw-   0        0        0     7475 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/tilesheet.cpp
+-rw-rw-rw-   0        0        0     3049 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/tilesheet.h
+-rw-rw-rw-   0        0        0     5300 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/truetype.cpp
+-rw-rw-rw-   0        0        0     2318 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tileset/truetype.h
+-rw-rw-rw-   0        0        0     2028 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tree.h
+-rw-rw-rw-   0        0        0     2069 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tree.hpp
+-rw-rw-rw-   0        0        0     2014 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/tree_c.c
+-rw-rw-rw-   0        0        0     2758 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/txtfield.cpp
+-rw-rw-rw-   0        0        0     2740 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/txtfield.h
+-rw-rw-rw-   0        0        0     2299 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/txtfield.hpp
+-rw-rw-rw-   0        0        0    20688 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/txtfield_c.c
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/libtcod/utility/
+-rw-rw-rw-   0        0        0     6088 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/utility/vector2.h
+-rw-rw-rw-   0        0        0     2023 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/utility.h
+-rw-rw-rw-   0        0        0     2119 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/version.h
+-rw-rw-rw-   0        0        0    10968 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/wrappers.c
+-rw-rw-rw-   0        0        0     6805 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/wrappers.h
+-rw-rw-rw-   0        0        0     3666 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/zip.cpp
+-rw-rw-rw-   0        0        0     3586 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/zip.h
+-rw-rw-rw-   0        0        0    12288 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/zip.hpp
+-rw-rw-rw-   0        0        0    11867 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod/zip_c.c
+-rw-rw-rw-   0        0        0     4124 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod.cpp
+-rw-rw-rw-   0        0        0     1663 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod.h
+-rw-rw-rw-   0        0        0     1655 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod.hpp
+-rw-rw-rw-   0        0        0     3282 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/libtcod_c.c
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/vendor/
+-rw-rw-rw-   0        0        0    70416 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/glad.c
+-rw-rw-rw-   0        0        0   127491 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/glad.h
+-rw-rw-rw-   0        0        0    10037 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/khrplatform.h
+-rw-rw-rw-   0        0        0   223161 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/lodepng.cpp
+-rw-rw-rw-   0        0        0    82947 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/lodepng.h
+-rw-rw-rw-   0        0        0      193 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/stb.c
+-rw-rw-rw-   0        0        0    56319 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/stb_sprintf.h
+-rw-rw-rw-   0        0        0   191762 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/stb_truetype.h
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/vendor/utf8proc/
+-rw-rw-rw-   0        0        0    30127 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/utf8proc/utf8proc.c
+-rw-rw-rw-   0        0        0    29484 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/utf8proc/utf8proc.h
+-rw-rw-rw-   0        0        0  1614402 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/utf8proc/utf8proc_data.c
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/libtcod/src/vendor/zlib/
+-rw-rw-rw-   0        0        0     5204 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/adler32.c
+-rw-rw-rw-   0        0        0     2699 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/compress.c
+-rw-rw-rw-   0        0        0    14053 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/crc32.c
+-rw-rw-rw-   0        0        0    30562 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/crc32.h
+-rw-rw-rw-   0        0        0    78889 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/deflate.c
+-rw-rw-rw-   0        0        0    13150 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/deflate.h
+-rw-rw-rw-   0        0        0      678 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/gzclose.c
+-rw-rw-rw-   0        0        0     6819 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/gzguts.h
+-rw-rw-rw-   0        0        0    16599 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/gzlib.c
+-rw-rw-rw-   0        0        0    20428 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/gzread.c
+-rw-rw-rw-   0        0        0    19253 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/gzwrite.c
+-rw-rw-rw-   0        0        0    22715 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/infback.c
+-rw-rw-rw-   0        0        0    12978 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/inffast.c
+-rw-rw-rw-   0        0        0      427 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/inffast.h
+-rw-rw-rw-   0        0        0     6332 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/inffixed.h
+-rw-rw-rw-   0        0        0    54800 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/inflate.c
+-rw-rw-rw-   0        0        0     6618 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/inflate.h
+-rw-rw-rw-   0        0        0    12999 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/inftrees.c
+-rw-rw-rw-   0        0        0     2928 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/inftrees.h
+-rw-rw-rw-   0        0        0    43761 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/trees.c
+-rw-rw-rw-   0        0        0     8472 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/trees.h
+-rw-rw-rw-   0        0        0     2966 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/uncompr.c
+-rw-rw-rw-   0        0        0    16298 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/zconf.h
+-rw-rw-rw-   0        0        0    96239 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/zlib.h
+-rw-rw-rw-   0        0        0     7304 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/zutil.c
+-rw-rw-rw-   0        0        0     7127 2019-03-16 00:16:50.000000 tcod-9.3.0/libtcod/src/vendor/zlib/zutil.h
+-rw-rw-rw-   0        0        0      196 2019-03-16 00:16:40.000000 tcod-9.3.0/libtcodpy.py
+-rw-rw-rw-   0        0        0     1386 2019-03-16 00:16:40.000000 tcod-9.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      337 2019-03-16 00:16:40.000000 tcod-9.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    32431 2019-03-16 00:17:31.000000 tcod-9.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4158 2019-03-16 00:16:40.000000 tcod-9.3.0/README.rst
+-rw-rw-rw-   0        0        0       71 2019-03-16 00:16:40.000000 tcod-9.3.0/requirements.txt
+-rw-rw-rw-   0        0        0      248 2019-03-16 00:17:31.000000 tcod-9.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     4739 2019-03-16 00:16:40.000000 tcod-9.3.0/setup.py
+-rw-rw-rw-   0        0        0      242 2019-03-16 00:16:40.000000 tcod-9.3.0/stdeb.cfg
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/tcod/
+-rw-rw-rw-   0        0        0     8282 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/bsp.py
+-rw-rw-rw-   0        0        0      881 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/cdef.h
+-rw-rw-rw-   0        0        0      519 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/cffi.h
+-rw-rw-rw-   0        0        0     4200 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/color.py
+-rw-rw-rw-   0        0        0    36926 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/console.py
+-rw-rw-rw-   0        0        0    21696 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/constants.py
+-rw-rw-rw-   0        0        0    23098 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/event.py
+-rw-rw-rw-   0        0        0    39424 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/event_constants.py
+-rw-rw-rw-   0        0        0    10044 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/image.py
+-rw-rw-rw-   0        0        0     2042 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/libtcod.py
+-rw-rw-rw-   0        0        0   125208 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/libtcodpy.py
+-rw-rw-rw-   0        0        0     6941 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/map.py
+-rw-rw-rw-   0        0        0     2110 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/noise.c
+-rw-rw-rw-   0        0        0     1012 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/noise.h
+-rw-rw-rw-   0        0        0    10140 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/noise.py
+-rw-rw-rw-   0        0        0     1544 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/path.cpp
+-rw-rw-rw-   0        0        0     1539 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/path.h
+-rw-rw-rw-   0        0        0    10153 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/path.py
+-rw-rw-rw-   0        0        0      876 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/path2.py
+-rw-rw-rw-   0        0        0        0 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/py.typed
+-rw-rw-rw-   0        0        0      931 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/random.h
+-rw-rw-rw-   0        0        0     4474 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/random.py
+-rw-rw-rw-   0        0        0     2610 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/tcod.cpp
+-rw-rw-rw-   0        0        0     1409 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/tcod.h
+-rw-rw-rw-   0        0        0     4690 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/tcod.py
+-rw-rw-rw-   0        0        0     7057 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/tdl.c
+-rw-rw-rw-   0        0        0     2333 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/tdl.h
+-rw-rw-rw-   0        0        0     1015 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/tileset.py
+-rw-rw-rw-   0        0        0       23 2019-03-16 00:17:11.000000 tcod-9.3.0/tcod/version.py
+-rw-rw-rw-   0        0        0     1442 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/_internal.py
+-rw-rw-rw-   0        0        0      899 2019-03-16 00:16:40.000000 tcod-9.3.0/tcod/__init__.py
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/tcod.egg-info/
+-rw-rw-rw-   0        0        0        1 2019-03-16 00:17:31.000000 tcod-9.3.0/tcod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    32431 2019-03-16 00:17:31.000000 tcod-9.3.0/tcod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2019-03-16 00:17:31.000000 tcod-9.3.0/tcod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0    14830 2019-03-16 00:17:31.000000 tcod-9.3.0/tcod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       19 2019-03-16 00:17:31.000000 tcod-9.3.0/tcod.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2019-03-16 00:17:31.000000 tcod-9.3.0/tdl/
+-rw-rw-rw-   0        0        0    18298 2019-03-16 00:16:40.000000 tcod-9.3.0/tdl/event.py
+-rw-rw-rw-   0        0        0    12296 2019-03-16 00:16:40.000000 tcod-9.3.0/tdl/map.py
+-rw-rw-rw-   0        0        0     5915 2019-03-16 00:16:40.000000 tcod-9.3.0/tdl/noise.py
+-rw-rw-rw-   0        0        0      943 2019-03-16 00:16:40.000000 tcod-9.3.0/tdl/style.py
+-rw-rw-rw-   0        0        0     3150 2019-03-16 00:16:40.000000 tcod-9.3.0/tdl/terminal8x8.png
+-rw-rw-rw-   0        0        0       29 2019-03-16 00:16:40.000000 tcod-9.3.0/tdl/version.py
+-rw-rw-rw-   0        0        0    51651 2019-03-16 00:16:40.000000 tcod-9.3.0/tdl/__init__.py
+-rw-rw-rw-   0        0        0      143 2019-03-16 00:16:40.000000 tcod-9.3.0/unittest.cfg
```

### Comparing `tcod-9.2.5/build_libtcod.py` & `tcod-9.3.0/build_libtcod.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/CHANGELOG.rst` & `tcod-9.3.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,43 @@
 ===========
  Changelog
 ===========
-Changes relevant for users of the the tdl and tcod packages are documented
-here.
+Changes relevant to the users of python-tcod are documented here.
 
 This project adheres to `Semantic Versioning <https://semver.org/>`_ since
 v2.0.0
 
 Unreleased
 ------------------
 
+9.3.0 - 2019-03-15
+------------------
+Added
+ - The SDL2/OPENGL2 renderers can potentially use a fall-back font when none
+   are provided.
+ - New function `tcod.event.get_mouse_state`.
+ - New function `tcod.map.compute_fov` lets you get a visibility array directly
+   from a transparency array.
+Deprecated
+ - The following functions and classes have been deprecated.
+   - `tcod.Key`
+   - `tcod.Mouse`
+   - `tcod.mouse_get_status`
+   - `tcod.console_is_window_closed`
+   - `tcod.console_check_for_keypress`
+   - `tcod.console_wait_for_keypress`
+   - `tcod.console_delete`
+   - `tcod.sys_check_for_event`
+   - `tcod.sys_wait_for_event`
+ - The SDL, OPENGL, and GLSL renderers have been deprecated.
+ - Many libtcodpy functions have been marked with PendingDeprecationWarning's.
+Fixed
+ - To be more compatible with libtcodpy `tcod.console_init_root` will default
+   to the SDL render, but will raise warnings when an old renderer is used.
+
 9.2.5 - 2019-03-04
 ------------------
 Fixed
  - Fixed `tcod.namegen_generate_custom`.
 
 9.2.4 - 2019-03-02
 ------------------
@@ -27,50 +51,50 @@
    the future.
  - Methods and functionality preventing `tcod.Color` from behaving like a tuple
    have been deprecated.
 
 9.2.2 - 2019-02-26
 ------------------
 Fixed
-- `Console.print_box` wasn't setting the background color by default.
+ - `Console.print_box` wasn't setting the background color by default.
 
 9.2.1 - 2019-02-25
 ------------------
 Fixed
-- `tcod.sys_get_char_size` fixed on the new renderers.
+ - `tcod.sys_get_char_size` fixed on the new renderers.
 
 9.2.0 - 2019-02-24
 ------------------
 Added
-- New `tcod.console.get_height_rect` function, which can be used to get the
-  height of a print call without an existing console.
-- New `tcod.tileset` module, with a `set_truetype_font` function.
-Fixed
-- The new print methods now handle alignment according to how they were
-  documented.
-- `SDL2` and `OPENGL2` now support screenshots.
-- Windows and MacOS builds now restrict exported SDL2 symbols to only
-  SDL 2.0.5;  This will avoid hard to debug import errors when the wrong
-  version of SDL is dynamically linked.
-- The root console now starts with a white foreground.
+ - New `tcod.console.get_height_rect` function, which can be used to get the
+   height of a print call without an existing console.
+ - New `tcod.tileset` module, with a `set_truetype_font` function.
+Fixed
+ - The new print methods now handle alignment according to how they were
+   documented.
+ - `SDL2` and `OPENGL2` now support screenshots.
+ - Windows and MacOS builds now restrict exported SDL2 symbols to only
+   SDL 2.0.5;  This will avoid hard to debug import errors when the wrong
+   version of SDL is dynamically linked.
+ - The root console now starts with a white foreground.
 
 9.1.0 - 2019-02-23
 ------------------
 Added
-- Added the `tcod.random.MULTIPLY_WITH_CARRY` constant.
+ - Added the `tcod.random.MULTIPLY_WITH_CARRY` constant.
 Changed
-- The overhead for warnings has been reduced when running Python with the
-  optimize `-O` flag.
-- `tcod.random.Random` now provides a default algorithm.
+ - The overhead for warnings has been reduced when running Python with the
+   optimize `-O` flag.
+ - `tcod.random.Random` now provides a default algorithm.
 
 9.0.0 - 2019-02-17
 ------------------
 Changed
-- New console methods now default to an `fg` and `bg` of None instead of
-  white-on-black.
+ - New console methods now default to an `fg` and `bg` of None instead of
+   white-on-black.
 
 8.5.0 - 2019-02-15
 ------------------
 Added
  - `tcod.console.Console` now supports `str` and `repr`.
  - Added new Console methods which are independent from the console defaults.
  - You can now give an array when initializing a `tcod.console.Console`
```

### Comparing `tcod-9.2.5/dependencies/fake_libc_include/_fake_defines.h` & `tcod-9.3.0/dependencies/fake_libc_include/_fake_defines.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/dependencies/fake_libc_include/_fake_typedefs.h` & `tcod-9.3.0/dependencies/fake_libc_include/_fake_typedefs.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/CHANGELOG.md` & `tcod-9.3.0/libtcod/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,42 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 
 This project attempts to adhere to [Semantic Versioning](http://semver.org/)
 since `1.7.0`.
 
 ## [Unreleased]
 ### Fixed
+- Fixed header declaration for `TCOD_sys_accumulate_console`.
+
+## [1.11.0] - 2019-03-15
+### Added
+- Added new functions which convert from SDL events to libtcod events:
+  - `TCOD_sys_process_key_event`
+  - `TCOD_sys_process_mouse_event`
+  - `tcod::sdl2::process_event`
+- Added a way to access libtcod's SDL variables.
+  - `TCOD_sys_get_sdl_window`
+  - `TCOD_sys_get_sdl_renderer`
+- Added `TCOD_sys_accumulate_console` which renders a console to the display
+  without automatically presenting it.
+- The new renderers can potentially use a fall-back font when none is provided.
+
+### Fixed
+- `TCOD_console_has_mouse_focus` and `TCOD_console_is_active` are now more
+  reliable with the newer renderers.
+
+## [1.10.8] - 2019-03-01
+### Deprecated
+- Updated libtcodpy deprecation warning with instructions on how to update to
+  python-tcod.
+
+## [1.10.7] - 2019-03-01
+### Changed
+- GCC releases now include debug symbols.
+### Fixed
 - `SDL2` and `OPENGL2` now support screenshots.
 - `TCOD_sys_get_char_size` fixed on the newer renderers.
 
 ## [1.10.6] - 2019-02-15
 ### Changed
 - Printing generates more compact layouts.
 ### Fixed
```

### Comparing `tcod-9.2.5/libtcod/LIBTCOD-CREDITS.txt` & `tcod-9.3.0/libtcod/LIBTCOD-CREDITS.txt`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/LIBTCOD-LICENSE.txt` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_display.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,57 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
+#ifndef LIBTCOD_SDL2_GL2_DISPLAY_H_
+#define LIBTCOD_SDL2_GL2_DISPLAY_H_
+
+#include "gl2_renderer.h"
+#include "sdl2_display.h"
+
+namespace tcod {
+namespace sdl2 {
+class OpenGL2Display: public WindowedDisplay {
+ public:
+  explicit OpenGL2Display(
+      std::shared_ptr<Tileset> tileset,
+      std::array<int, 2> window_size,
+      int window_flags,
+      const std::string& title);
+  virtual void set_tileset(std::shared_ptr<Tileset> tileset) override;
+  virtual void accumulate(const TCOD_Console*) override;
+  virtual void present(const TCOD_Console*) override;
+  virtual auto read_pixels() const -> Image override;
+ private:
+  std::shared_ptr<void> glcontext_;
+  OpenGL2Renderer tcod_renderer_;
+};
+} // namespace sdl2
+} // namespace tcod
+#endif //LIBTCOD_SDL2_GL2_DISPLAY_H_
```

### Comparing `tcod-9.2.5/libtcod/README.md` & `tcod-9.3.0/libtcod/README.md`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/libtcod/bresenham.cpp` & `tcod-9.3.0/libtcod/src/libtcod/bresenham.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "bresenham.hpp"
 
 // ********** bresenham line drawing **********
 void TCODLine::init(int xFrom, int yFrom, int xTo, int yTo) {
 	TCOD_line_init(xFrom,yFrom,xTo,yTo);
 }
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/bresenham.h` & `tcod-9.3.0/libtcod/src/libtcod/bresenham.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_BRESENHAM_H
 #define _TCOD_BRESENHAM_H
 
 #include "portability.h"
 
 #ifdef __cplusplus
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/bresenham.hpp` & `tcod-9.3.0/libtcod/src/libtcod/bresenham.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_BRESENHAM_HPP
 #define _TCOD_BRESENHAM_HPP
 
 #include "bresenham.h"
 
 class TCODLIB_API TCODLineListener {
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/bresenham_c.c` & `tcod-9.3.0/libtcod/src/libtcod/bresenham_c.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "bresenham.h"
 /**
  *  \file bresenham_c.c
  *  \brief bresenham line drawing
  */
 /* This static variable is deprecated since 1.6 */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/bsp.cpp` & `tcod-9.3.0/libtcod/src/libtcod/bsp.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "bsp.hpp"
 
 TCODBsp::TCODBsp(TCODBsp *father, bool left) {
 	if ( father->horizontal ) {
 		x=father->x;
 		w=father->w;
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/bsp.h` & `tcod-9.3.0/libtcod/src/libtcod/bsp.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_BSP_H
 #define _TCOD_BSP_H
 
 #include "portability.h"
 #include "mersenne_types.h"
 #include "tree.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/bsp.hpp` & `tcod-9.3.0/libtcod/src/libtcod/bsp.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_BSP_HPP
 #define _TCOD_BSP_HPP
 
 #include "bsp.h"
 #include "list.hpp"
 #include "mersenne.hpp"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/bsp_c.c` & `tcod-9.3.0/libtcod/src/libtcod/bsp_c.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "bsp.h"
 
 #include <stdlib.h>
 
 #include "list.h"
 #include "mersenne.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/color/canvas.cpp` & `tcod-9.3.0/libtcod/src/libtcod/color/canvas.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "canvas.h"
 
 #include <stdexcept>
 
 #include <sys/types.h>
 #include <sys/stat.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/color/canvas.h` & `tcod-9.3.0/libtcod/src/libtcod/color/canvas.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_COLOR_CANVAS_H_
 #define LIBTCOD_COLOR_CANVAS_H_
 #ifdef __cplusplus
 #include <string>
 #endif // __cplusplus
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/color/color.h` & `tcod-9.3.0/libtcod/src/libtcod/color/color.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_COLOR_COLOR_H_
 #define LIBTCOD_COLOR_COLOR_H_
 #include <stdint.h>
 
 #include "../color.h"
 #ifdef __cplusplus
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/color.cpp` & `tcod-9.3.0/libtcod/src/libtcod/color.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "color.hpp"
 
 #include "libtcod_int.h"
 
 // grey levels
 const TCODColor TCODColor::black(TCOD_BLACK);
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/color.h` & `tcod-9.3.0/libtcod/src/libtcod/color.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_COLOR_H
 #define _TCOD_COLOR_H
 
 #include "portability.h"
 
 #ifdef __cplusplus
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/color.hpp` & `tcod-9.3.0/libtcod/src/libtcod/color.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_COLOR_HPP
 #define _TCOD_COLOR_HPP
 
 #include <algorithm>
 
 #include "color.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/color_c.c` & `tcod-9.3.0/libtcod/src/libtcod/color_c.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "color.h"
 
 #include <math.h>
 
 #include "libtcod_int.h"
 #include "utility.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console/drawing.cpp` & `tcod-9.3.0/libtcod/src/libtcod/console/drawing.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "drawing.h"
 
 #include "../libtcod_int.h"
 #include "../console.h"
 namespace tcod {
 namespace console {
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console/drawing.h` & `tcod-9.3.0/libtcod/src/libtcod/console/drawing.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_CONSOLE_DRAWING_H_
 #define TCOD_CONSOLE_DRAWING_H_
 #include "../console_types.h"
 #include "../portability.h"
 /**
  *  Draw a rectangle onto a console.
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console/printing.cpp` & `tcod-9.3.0/libtcod/src/libtcod/console/printing.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "printing.h"
 
 #include <ctype.h>
 #ifndef NO_UNICODE
 #include <wchar.h>
 #include <wctype.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console/printing.h` & `tcod-9.3.0/libtcod/src/libtcod/console/printing.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_CONSOLE_PRINTING_H_
 #define TCOD_CONSOLE_PRINTING_H_
 
 #ifdef __cplusplus
 #include <array>
 #include <cstdbool>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console/rexpaint.cpp` & `tcod-9.3.0/libtcod/src/libtcod/console/rexpaint.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "rexpaint.h"
 
 #ifdef TCOD_CONSOLE_SUPPORT
 
 #include <limits.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console/rexpaint.h` & `tcod-9.3.0/libtcod/src/libtcod/console/rexpaint.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_CONSOLE_REXPAINT_H_
 #define TCOD_CONSOLE_REXPAINT_H_
 
 #include "../portability.h"
 #include "../console_types.h"
 #include "../list.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console.cpp` & `tcod-9.3.0/libtcod/src/libtcod/console.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,42 +1,47 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "console.hpp"
 
 #include <stdio.h>
 #include <stdarg.h>
 #include <string.h>
 
 #include "libtcod_int.h"
 #include "image.hpp"
+#include "engine/display.h"
 
 #ifdef TCOD_CONSOLE_SUPPORT
 
 TCODConsole* TCODConsole::root = new TCODConsole();
 
 TCODConsole::TCODConsole() {}
 TCODConsole::TCODConsole(int w, int h) {
@@ -138,15 +143,15 @@
 	TCOD_sys_set_window_title(title);
 }
 #endif
 
 void TCODConsole::initRoot(int w, int h, const char *title, bool fullscreen,
                            TCOD_renderer_t renderer)
 {
-  TCOD_console_init_root(w, h, title, fullscreen, renderer);
+  tcod::console::init_root(w, h, title ? title : "", fullscreen, renderer);
 }
 
 void TCODConsole::setFullscreen(bool fullscreen) {
 	TCOD_console_set_fullscreen(fullscreen);
 }
 
 bool TCODConsole::isFullscreen() {
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console.h` & `tcod-9.3.0/libtcod/src/libtcod/console.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_CONSOLE_H
 #define _TCOD_CONSOLE_H
 
 #include "portability.h"
 
 #ifdef TCOD_CONSOLE_SUPPORT
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console.hpp` & `tcod-9.3.0/libtcod/src/libtcod/console.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_CONSOLE_HPP
 #define _TCOD_CONSOLE_HPP
 
 #include <string>
 
 #include "console.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console_c.cpp` & `tcod-9.3.0/libtcod/src/libtcod/console_c.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "console.h"
 
 #include <stdio.h>
 #include <stdarg.h>
 #include <string.h>
 #include <stdlib.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/console_types.h` & `tcod-9.3.0/libtcod/src/libtcod/console_types.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_CONSOLE_TYPES_H
 #define _TCOD_CONSOLE_TYPES_H
 
 #include "portability.h"
 #include "color.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/deprecated.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/hbox.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,40 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "console.h"
-#include "console.hpp"
-
-void TCOD_console_set_keyboard_repeat(int, int) {}
-void TCOD_console_disable_keyboard_repeat() {}
-void TCODConsole::setKeyboardRepeat(int, int) {}
-void TCODConsole::disableKeyboardRepeat() {}
+#ifndef TCOD_GUI_HBOX_HPP
+#define TCOD_GUI_HBOX_HPP
+#include "vbox.hpp"
+class TCODLIB_GUI_API HBox : public VBox {
+public :
+	HBox(int x, int y, int padding);
+	void computeSize();
+};
+#endif /* TCOD_GUI_HBOX_HPP */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/engine/backend.cpp` & `tcod-9.3.0/libtcod/src/libtcod/tileset/fallback.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,57 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "backend.h"
+#include "fallback.h"
+
+#include <cstdlib>
+#include <string>
+
+#include "truetype.h"
+namespace tcod {
+namespace tileset {
+auto new_fallback_tileset(const std::array<int, 2>& tile_size)
+-> std::unique_ptr<Tileset>
+{
+#if defined(_WIN32) // Windows.
+  std::string font_path(std::getenv("SystemRoot"));
+  font_path += "\\Fonts\\LUCON.TTF";
+  return load_truetype(font_path, tile_size);
+#elif defined(__APPLE__) // MacOS.
+  return load_truetype("/System/Library/Fonts/SFCompactDisplay-Regular.otf",
+                       tile_size);
+#else // Linux?
+  return load_truetype(
+      "/usr/share/fonts/truetype/dejavu/DejaVuSansMono.ttf",
+      tile_size);
+#endif
+}
+} // namespace tileset
+} // namespace tcod
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/engine/backend.h` & `tcod-9.3.0/libtcod/src/libtcod/engine/backend.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_ENGINE_BACKEND_H_
 #define LIBTCOD_ENGINE_BACKEND_H_
 
 #ifdef __cplusplus
 #include <memory>
 #endif /* __cplusplus */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/engine/display.cpp` & `tcod-9.3.0/libtcod/src/libtcod/engine/display.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,61 +1,72 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "display.h"
 
 #include <cstring>
 #include <stdexcept>
 #include <string>
 
 #include <SDL.h>
 #include "globals.h"
 #include "../console.h"
 #include "../console.hpp"
 #include "../libtcod_int.h"
 #include "../sdl2/sdl2_display.h"
 #include "../sdl2/gl2_display.h"
+#include "../tileset/fallback.h"
 namespace tcod {
 /**
  *  Initialize the display using one of the new renderers.
  */
 template <class T>
 static void init_display(int w, int h, const std::string& title,
                          int fullscreen)
 {
   auto tileset = tcod::engine::get_tileset();
   if (!tileset) {
-    TCOD_fatal("A custom font is required to use the SDL2/OPENGL2 renderers.");
+    try { // Try to load a fall-back Tileset, but ignore failure.
+      tileset = tcod::tileset::new_fallback_tileset();
+      tcod::engine::set_tileset(tileset);
+    } catch (const std::runtime_error& e) {
+      throw std::runtime_error(
+          "Couldn't load a fallback font for the SDL2/OPENGL2 renderer.");
+    }
   }
-  auto display_size = std::make_pair(tileset->get_tile_width() * w,
-                                     tileset->get_tile_height() * h);
+  std::array<int, 2> display_size{tileset->get_tile_width() * w,
+                                  tileset->get_tile_height() * h};
   int display_flags = (SDL_WINDOW_RESIZABLE |
                        (fullscreen ? SDL_WINDOW_FULLSCREEN_DESKTOP : 0));
   tcod::engine::set_display(
       std::make_shared<T>(tileset, display_size, display_flags, title));
 }
 namespace console {
 void init_root(int w, int h, const std::string& title, bool fullscreen,
@@ -127,16 +138,54 @@
     return display->get_fullscreen() == 1;
   } else {
     return TCOD_ctx.fullscreen;
   }
 }
 bool TCOD_console_has_mouse_focus(void)
 {
+  auto display = tcod::engine::get_display();
+  if (display) {
+    auto window = display->get_sdl_window();
+    if (window) {
+      return (SDL_GetWindowFlags(window) & SDL_WINDOW_MOUSE_FOCUS) != 0;
+    }
+  }
   return TCOD_ctx.app_has_mouse_focus;
 }
 bool TCOD_console_is_active(void)
 {
+  auto display = tcod::engine::get_display();
+  if (display) {
+    auto window = display->get_sdl_window();
+    if (window) {
+      return (SDL_GetWindowFlags(window) & SDL_WINDOW_INPUT_FOCUS) != 0;
+    }
+  }
   return TCOD_ctx.app_is_active;
 }
 bool TCOD_console_is_window_closed(void) {
 	return TCOD_ctx.is_window_closed;
 }
+struct SDL_Window* TCOD_sys_get_sdl_window(void)
+{
+  auto display = tcod::engine::get_display();
+  if (display) {
+    return display->get_sdl_window();
+  }
+  return TCOD_sys_get_sdl_window_();
+}
+struct SDL_Renderer* TCOD_sys_get_sdl_renderer(void)
+{
+  auto display = tcod::engine::get_display();
+  if (display) {
+    return display->get_sdl_renderer();
+  }
+  return TCOD_sys_get_sdl_renderer_();
+}
+int TCOD_sys_accumulate_console(const TCOD_Console* console)
+{
+  console = tcod::console::validate_(console);
+  auto display = tcod::engine::get_display();
+  if (!console || !display) { return -1; }
+  display->accumulate(console);
+  return 0;
+}
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/engine/display.h` & `tcod-9.3.0/libtcod/src/libtcod/engine/display.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,101 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_ENGINE_DISPLAY_H_
 #define LIBTCOD_ENGINE_DISPLAY_H_
 
 #ifdef __cplusplus
+#include <array>
 #include <string>
-#include <utility>
 #endif // __cplusplus
 
 #include "../color/canvas.h"
 #include "../tileset/tileset.h"
 #include "../console_types.h"
 
+struct SDL_Window;
+struct SDL_Renderer;
 #ifdef __cplusplus
 namespace tcod {
 namespace engine {
 using tcod::image::Image;
 using tcod::tileset::Tileset;
 class Display {
  public:
   virtual ~Display() = default;
   virtual void set_tileset(std::shared_ptr<Tileset> tileset) = 0;
   virtual void set_title(const std::string& title) = 0;
   virtual std::string get_title() = 0;
   /**
    *  Set the fullscreen status if the display supports it.
    *
-   *  When it is suppered this can be used to switch between a window and
+   *  If it is supported this can be used to switch between a window and
    *  borderless fullscreen window.
    */
   virtual void set_fullscreen(bool fullscreen) = 0;
   /**
    *  Return true if the display is in fullscreen mode.
    *
    *  Returns a negative number if the display does not support fullscreen.
    */
   virtual int get_fullscreen() = 0;
+  /**
+   *  Render a console over this display.
+   */
+  virtual void accumulate(const TCOD_Console*) = 0;
+  /**
+   *  Render a console and present the display.
+   */
   virtual void present(const TCOD_Console*) = 0;
-  virtual auto pixel_to_tile(const std::pair<double, double>& xy)
-      -> std::pair<double, double> = 0;
+  virtual auto pixel_to_tile(const std::array<double, 2>& xy)
+      -> std::array<double, 2> = 0;
 
   virtual auto read_pixels() const -> Image = 0;
+  /**
+   *  Return the pointer to an SDL2 window, if this display uses SDL.
+   *
+   *  Could return nullptr.
+   */
+  virtual auto get_sdl_window() -> struct SDL_Window* = 0;
+  /**
+   *  Return the pointer to an SDL2 renderer, if this display uses SDL's
+   *  renderer.
+   *
+   *  Could return nullptr.
+   */
+  virtual auto get_sdl_renderer() -> struct SDL_Renderer* = 0;
 };
 /**
  *  Incomplete interface for subclasses which don't need an SDL2 window.
  */
 class TerminalDisplay: public Display {
  public:
   virtual void set_tileset(std::shared_ptr<Tileset>) override
@@ -88,19 +114,27 @@
   /**
    *  Return a negative error code.
    */
   virtual int get_fullscreen() override
   {
     return -1;
   }
-  virtual auto pixel_to_tile(const std::pair<double, double>& xy)
-      -> std::pair<double, double> override
+  virtual auto pixel_to_tile(const std::array<double, 2>& xy)
+      -> std::array<double, 2> override
   {
     return xy;
   }
+  virtual auto get_sdl_window() -> struct SDL_Window* override
+  {
+    return nullptr;
+  }
+  virtual auto get_sdl_renderer() -> struct SDL_Renderer* override
+  {
+    return nullptr;
+  }
 };
 } // namespace sdl2
 namespace console {
 TCODLIB_API void init_root(int w, int h, const std::string& title,
                            bool fullscreen, TCOD_renderer_t renderer);
 } // namespace console
 } // namespace tcod
@@ -160,10 +194,43 @@
  *  \endverbatim
  */
 TCODLIB_CAPI bool TCOD_console_is_active(void);
 /**
  *  Return true if the window is closing.
  */
 TCODLIB_CAPI bool TCOD_console_is_window_closed(void);
+/**
+ *  Return an SDL_Window pointer if one is in use, returns NULL otherwise.
+ *  \rst
+ *  .. versionadded:: 1.11
+ *  \endrst
+ */
+TCODLIB_CAPI struct SDL_Window* TCOD_sys_get_sdl_window(void);
+/**
+ *  Return an SDL_Renderer pointer if one is in use, returns NULL otherwise.
+ *  \rst
+ *  .. versionadded:: 1.11
+ *  \endrst
+ */
+TCODLIB_CAPI struct SDL_Renderer* TCOD_sys_get_sdl_renderer(void);
+/**
+ *  Render a console over the display.
+ *  \rst
+ *  `console` can be any size, the active render will try to scale it to fit
+ *  the screen.
+ *
+ *  The function will only work for the SDL2/OPENGL2 renderers.
+ *
+ *  Unlike :any:`TCOD_console_flush` this will not present the display.
+ *  You will need to do that manually, likely with the SDL API.
+ *
+ *  Returns 0 on success, or a negative number on a failure such as the
+ *  incorrect renderer being active.
+ *
+ *  .. versionadded:: 1.11
+ *
+ *  .. seealso::
+ *      :any:`TCOD_sys_get_sdl_window` :any:`TCOD_sys_get_sdl_renderer`
+ *  \endrst
+ */
+TCODLIB_CAPI int TCOD_sys_accumulate_console(const TCOD_Console* console);
 #endif // LIBTCOD_ENGINE_DISPLAY_H_
-
-
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/engine/globals.cpp` & `tcod-9.3.0/libtcod/src/libtcod/engine/globals.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "globals.h"
 
 #include <cstdlib>
 
 namespace tcod {
 namespace engine {
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/engine/globals.h` & `tcod-9.3.0/libtcod/src/libtcod/engine/globals.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_ENGINE_GLOBALS_H_
 #define LIBTCOD_ENGINE_GLOBALS_H_
 
 #ifdef __cplusplus
 #include <memory>
 #endif // __cplusplus
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/fov.cpp` & `tcod-9.3.0/libtcod/src/libtcod/fov.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "fov.hpp"
 
 TCODMap::TCODMap(int width,int height) {
 	data = TCOD_map_new(width,height);
 }
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/fov.h` & `tcod-9.3.0/libtcod/src/libtcod/fov.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_FOV_H
 #define _TCOD_FOV_H
 
 #include "portability.h"
 #include "fov_types.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/fov.hpp` & `tcod-9.3.0/libtcod/src/libtcod/fov.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_FOV_HPP
 #define _TCOD_FOV_HPP
 
 #include "fov.h"
 
 class TCODPath;
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/fov_c.c` & `tcod-9.3.0/libtcod/src/libtcod/fov_c.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "fov.h"
 
 #include <stdlib.h>
 #include <string.h>
 
 #include "libtcod_int.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/fov_circular_raycasting.c` & `tcod-9.3.0/libtcod/src/libtcod/fov_circular_raycasting.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "fov.h"
 
 #include <string.h>
 #include <math.h>
 #include <stdlib.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/fov_diamond_raycasting.c` & `tcod-9.3.0/libtcod/src/libtcod/fov_diamond_raycasting.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "fov.h"
 
 #include <stdlib.h>
 #include <string.h>
 
 #include "libtcod_int.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/fov_permissive2.c` & `tcod-9.3.0/libtcod/src/libtcod/fov_permissive2.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "fov.h"
 
 #include <stdlib.h>
 #include <string.h>
 #include <stdio.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/fov_recursive_shadowcasting.c` & `tcod-9.3.0/libtcod/src/libtcod/fov_recursive_shadowcasting.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "fov.h"
 
 #include <stdlib.h>
 #include <string.h>
 #include <math.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/fov_restrictive.c` & `tcod-9.3.0/libtcod/src/libtcod/fov_restrictive.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 /*
 * Mingos' Restrictive Precise Angle Shadowcasting (MRPAS) v1.2
 */
 #include "fov.h"
 
 #include <stdlib.h> /* for NULL in VS */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/fov_types.h` & `tcod-9.3.0/libtcod/src/libtcod/fov_types.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_FOV_TYPES_H_
 #define TCOD_FOV_TYPES_H_
 #include "portability.h"
 /**
  *  Private map cell struct.
  */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/button.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/button.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "button.hpp"
 
 #include <string.h>
 #include <algorithm>
 
 Button::Button(
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/button.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/button.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_GUI_BUTTON_HPP
 #define TCOD_GUI_BUTTON_HPP
 #include "widget.hpp"
 class TCODLIB_GUI_API Button : public Widget {
 public :
 	Button(const char *label, const char *tip, widget_callback_t cbk, void *userData=NULL);
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/container.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/container.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "container.hpp"
 
 Container::~Container() {
 	content.clearAndDelete();
 }
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/container.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/textbox.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,58 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef TCOD_GUI_CONTAINER_HPP
-#define TCOD_GUI_CONTAINER_HPP
+#ifndef TCOD_GUI_TEXTBOX_HPP
+#define TCOD_GUI_TEXTBOX_HPP
 #include "widget.hpp"
-class TCODLIB_GUI_API Container : public Widget {
+class TCODLIB_GUI_API TextBox : public Widget {
 public :
-	Container(int x, int y, int w, int h) : Widget(x,y,w,h) {}
-	virtual ~Container();
-	void addWidget(Widget *wid);
-	void removeWidget(Widget *wid);
-	void setVisible(bool val);
+	TextBox(int x,int y,int w, int maxw, const char *label, const char *value, const char *tip=NULL);
+	virtual ~TextBox();
 	void render();
-	void clear();
 	void update(const TCOD_key_t k);
+	void setText(const char *txt);
+	const char *getValue() { return txt; }
+	void setCallback(void (*cbk)(Widget *wid, char * val, void * data), void *data) { txtcbk=cbk; this->data=data; }
+	static void setBlinkingDelay(float delay) { blinkingDelay=delay; }
 protected :
-	TCODList<Widget *> content;
+	static float blinkingDelay;
+	char *label;
+	char *txt;
+	float blink;
+	int pos, offset;
+	int boxx,boxw,maxw;
+	bool insert;
+	void (*txtcbk)(Widget *wid, char * val, void *data);
+	void *data;
+
+	void onButtonClick();
 };
-#endif /* TCOD_GUI_CONTAINER_HPP */
+#endif /* TCOD_GUI_TEXTBOX_HPP */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/flatlist.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/flatlist.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "flatlist.hpp"
 
 #include <stdio.h>
 #include <math.h>
 
 FlatList::FlatList(int x,int y,int w, const char **list, const char *label, const char *tip)
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/flatlist.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/flatlist.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_GUI_FLATLIST_HPP
 #define TCOD_GUI_FLATLIST_HPP
 #include "textbox.hpp"
 class TCODLIB_GUI_API FlatList : public TextBox {
 public :
 	FlatList(int x,int y,int w, const char **list, const char *label, const char *tip=NULL);
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/gui.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/gui.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _GUI_HPP
 #define _GUI_HPP
 
 #include "../libtcod.hpp"
 
 #include "widget.hpp"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/gui_portability.hpp` & `tcod-9.3.0/libtcod/src/libtcod/tileset/truetype.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,60 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef TCOD_GUI_PORTABILITY_HPP
-#define TCOD_GUI_PORTABILITY_HPP
+#ifndef LIBTCOD_TILESET_TRUETYPE_H_
+#define LIBTCOD_TILESET_TRUETYPE_H_
+#ifdef __cplusplus
+#include <array>
+#include <memory>
+#endif // __cplusplus
+#include "tileset.h"
 
-#include "../portability.h"
-
-#ifdef TCOD_VISUAL_STUDIO
-#pragma warning(disable:4996)
-#pragma warning(disable:4251)
-#endif
-
-// DLL export
-#define TCODLIB_GUI_API TCODLIB_API
-
-#endif /* TCOD_GUI_PORTABILITY_HPP */
+#ifdef __cplusplus
+namespace tcod {
+namespace tileset {
+/**
+ *  Return a Tileset from a `.ttf` or `.otf` font file.
+ */
+auto load_truetype(
+    const std::string& path,
+    const std::array<int, 2>& tile_size)
+-> std::unique_ptr<Tileset>;
+} // namespace tileset
+} // namespace tcod
+#endif // __cplusplus
+/**
+ *  Set the global tileset from a TrueType font file.
+ */
+TCODLIB_CAPI int TCOD_tileset_load_truetype_(
+    const char* path,
+    int tile_width,
+    int tile_height);
+#endif // LIBTCOD_TILESET_TRUETYPE_H_
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/hbox.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/vbox.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,52 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "hbox.hpp"
-
-HBox::HBox(int x, int y, int padding) : VBox(x,y,padding) {
-}
+#include "vbox.hpp"
 
-void HBox::computeSize() {
-	int curx=x;
-	h=0;
+void VBox::computeSize() {
+	int cury=y;
+	w=0;
 	for (Widget **wid=content.begin(); wid != content.end(); wid ++ ) {
 		if ( (*wid)->isVisible() ) {
-			(*wid)->y=y;
-			(*wid)->x=curx;
+			(*wid)->x=x;
+			(*wid)->y=cury;
 			(*wid)->computeSize();
-			if ((*wid)->h > h) h=(*wid)->h;
-			curx+=(*wid)->w+padding;
+			if ((*wid)->w > w) w=(*wid)->w;
+			cury+=(*wid)->h+padding;
 		}
 	}
-	w=curx-x;
+	h=cury-y;
 	for (Widget **wid=content.begin(); wid != content.end(); wid ++ ) {
 		if ( (*wid)->isVisible() ) {
-			(*wid)->expand((*wid)->w,h);
+			(*wid)->expand(w,(*wid)->h);
 		}
 	}
 }
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/hbox.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/label.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,46 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef TCOD_GUI_HBOX_HPP
-#define TCOD_GUI_HBOX_HPP
-#include "vbox.hpp"
-class TCODLIB_GUI_API HBox : public VBox {
+#ifndef TCOD_GUI_LABEL_HPP
+#define TCOD_GUI_LABEL_HPP
+#include "widget.hpp"
+class TCODLIB_GUI_API Label : public Widget {
 public :
-	HBox(int x, int y, int padding);
+	Label(int x, int y, const char *label, const char *tip=NULL );
+	void render();
 	void computeSize();
+	void setValue(const char *label) { this->label=label; }
+protected :
+	const char *label;
+
+	void expand(int width, int height);
 };
-#endif /* TCOD_GUI_HBOX_HPP */
+#endif /* TCOD_GUI_LABEL_HPP */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/image.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/image.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "image.hpp"
 
 Image::Image(int x,int y,int w, int h, const char *tip) : Widget(x,y,w,h), back(TCODColor::black) {
 	if ( tip ) setTip(tip);
 }
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/image.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/vbox.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef TCOD_GUI_IMAGE_HPP
-#define TCOD_GUI_IMAGE_HPP
-#include "widget.hpp"
-class TCODLIB_GUI_API Image : public Widget {
+#ifndef TCOD_GUI_VBOX_HPP
+#define TCOD_GUI_VBOX_HPP
+#include "container.hpp"
+class TCODLIB_GUI_API VBox : public Container {
 public :
-	Image(int x,int y,int w, int h, const char *tip=NULL);
-	virtual ~Image();
-	void setBackgroundColor(const TCODColor col);
-	void render();
+	VBox(int x, int y, int padding) : Container(x,y,0,0),padding(padding) {}
+	void computeSize();
 protected :
-	void expand(int width, int height);
-
-	TCODColor back;
+	int padding;
 };
-#endif /* TCOD_GUI_IMAGE_HPP */
+#endif /* TCOD_GUI_VBOX_HPP */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/label.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/label.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "label.hpp"
 
 #include <algorithm>
 
 Label::Label(int x, int y, const char *label, const char *tip)
 : Widget(x, y, 0, 1)
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/label.hpp` & `tcod-9.3.0/libtcod/src/libtcod/txtfield.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,59 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef TCOD_GUI_LABEL_HPP
-#define TCOD_GUI_LABEL_HPP
-#include "widget.hpp"
-class TCODLIB_GUI_API Label : public Widget {
+#ifndef _TCOD_TEXT_HPP_
+#define _TCOD_TEXT_HPP_
+
+#include "color.hpp"
+#include "console.hpp"
+#include "txtfield.h"
+
+#ifdef TCOD_CONSOLE_SUPPORT
+
+class TCODLIB_API TCODText {
 public :
-	Label(int x, int y, const char *label, const char *tip=NULL );
-	void render();
-	void computeSize();
-	void setValue(const char *label) { this->label=label; }
+	TCODText(int x, int y, int w, int h, int max_chars);
+	TCODText(int w, int h, int max_chars);
+	~TCODText();
+	void setProperties(int cursor_char, int blink_interval, const char * prompt, int tab_size);
+	void setColors(TCODColor fore, TCODColor back, float back_transparency);
+	void setPos(int x, int y);
+	bool update(TCOD_key_t key);
+	void render(TCODConsole * con);
+	const char *getText();
+	void reset();
 protected :
-	const char *label;
-
-	void expand(int width, int height);
+	TCOD_text_t data;
 };
-#endif /* TCOD_GUI_LABEL_HPP */
+
+#endif /* TCOD_CONSOLE_SUPPORT */
+
+#endif
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/radiobutton.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/radiobutton.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "radiobutton.hpp"
 
 RadioButton *RadioButton::groupSelect[512];
 int RadioButton::defaultGroup=0;
 static bool init=false;
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/radiobutton.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/radiobutton.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_GUI_RADIOBUTTON_HPP
 #define TCOD_GUI_RADIOBUTTON_HPP
 #include "button.hpp"
 class TCODLIB_GUI_API RadioButton : public Button {
 public :
 	RadioButton(const char *label, const char *tip, widget_callback_t cbk, void *userData=NULL)
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/slider.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/slider.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "slider.hpp"
 
 #include <stdio.h>
 #include <string.h>
 #include <math.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/slider.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/slider.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_GUI_SLIDER_HPP
 #define TCOD_GUI_SLIDER_HPP
 #include "textbox.hpp"
 class TCODLIB_GUI_API Slider : public TextBox {
 public :
 	Slider(int x,int y,int w, float min, float max, const char *label, const char *tip=NULL);
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/statusbar.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/statusbar.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "statusbar.hpp"
 
 void StatusBar::render() {
 	con->setDefaultBackground(back);
 	con->rect(x,y,w,h,true,TCOD_BKGND_SET);
 	if ( focus && focus->tip ) {
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/statusbar.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/gui_portability.hpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,45 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef TCOD_GUI_STATUSBAR_HPP
-#define TCOD_GUI_STATUSBAR_HPP
-#include "widget.hpp"
-class TCODLIB_GUI_API StatusBar : public Widget {
-public :
-	StatusBar(int x,int y,int w, int h):Widget(x,y,w,h) {}
-	void render();
-};
-#endif /* TCOD_GUI_STATUSBAR_HPP */
+#ifndef TCOD_GUI_PORTABILITY_HPP
+#define TCOD_GUI_PORTABILITY_HPP
+
+#include "../portability.h"
+
+#ifdef TCOD_VISUAL_STUDIO
+#pragma warning(disable:4996)
+#pragma warning(disable:4251)
+#endif
+
+// DLL export
+#define TCODLIB_GUI_API TCODLIB_API
+
+#endif /* TCOD_GUI_PORTABILITY_HPP */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/textbox.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/textbox.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "textbox.hpp"
 
 #include <string.h>
 #include <stdio.h>
 
 float TextBox::blinkingDelay=0.5f;
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/textbox.hpp` & `tcod-9.3.0/libtcod/src/libtcod/namegen.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,64 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef TCOD_GUI_TEXTBOX_HPP
-#define TCOD_GUI_TEXTBOX_HPP
-#include "widget.hpp"
-class TCODLIB_GUI_API TextBox : public Widget {
-public :
-	TextBox(int x,int y,int w, int maxw, const char *label, const char *value, const char *tip=NULL);
-	virtual ~TextBox();
-	void render();
-	void update(const TCOD_key_t k);
-	void setText(const char *txt);
-	const char *getValue() { return txt; }
-	void setCallback(void (*cbk)(Widget *wid, char * val, void * data), void *data) { txtcbk=cbk; this->data=data; }
-	static void setBlinkingDelay(float delay) { blinkingDelay=delay; }
-protected :
-	static float blinkingDelay;
-	char *label;
-	char *txt;
-	float blink;
-	int pos, offset;
-	int boxx,boxw,maxw;
-	bool insert;
-	void (*txtcbk)(Widget *wid, char * val, void *data);
-	void *data;
+/*
+* Mingos' NameGen
+* This file was written by Dominik "Mingos" Marczuk.
+*/
+
+#ifndef _TCOD_NAMEGEN_H
+#define _TCOD_NAMEGEN_H
+
+#include "portability.h"
+#include "list.h"
+#include "mersenne.h"
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+/* the generator typedef */
+struct TCOD_NameGen;
+typedef struct TCOD_NameGen *TCOD_namegen_t;
 
-	void onButtonClick();
-};
-#endif /* TCOD_GUI_TEXTBOX_HPP */
+/* parse a file with syllable sets */
+TCODLIB_API void TCOD_namegen_parse (const char * filename, TCOD_random_t random);
+/* generate a name */
+TCODLIB_API char * TCOD_namegen_generate (char * name, bool allocate);
+/* generate a name using a custom generation rule */
+TCODLIB_API char * TCOD_namegen_generate_custom (char * name, char * rule, bool allocate);
+/* retrieve the list of all available syllable set names */
+TCODLIB_API TCOD_list_t TCOD_namegen_get_sets (void);
+/* delete a generator */
+TCODLIB_API void TCOD_namegen_destroy (void);
+#ifdef __cplusplus
+}
+#endif
+#endif
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/togglebutton.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/togglebutton.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "togglebutton.hpp"
 
 #include <string.h>
 
 void ToggleButton::render() {
 	con->setDefaultBackground(mouseIn ? backFocus : back);
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/togglebutton.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/togglebutton.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_GUI_TOGGLEBUTTON_HPP
 #define TCOD_GUI_TOGGLEBUTTON_HPP
 #include "button.hpp"
 class TCODLIB_GUI_API ToggleButton : public Button {
 public :
 	ToggleButton(const char *label, const char *tip, widget_callback_t cbk, void *userData=NULL)
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/toolbar.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/toolbar.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "toolbar.hpp"
 
 #include <string.h>
 #include <algorithm>
 
 class Separator : public Widget {
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/toolbar.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/statusbar.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef TCOD_GUI_TOOLBAR_HPP
-#define TCOD_GUI_TOOLBAR_HPP
-#include "container.hpp"
-class TCODLIB_GUI_API ToolBar : public Container {
+#ifndef TCOD_GUI_STATUSBAR_HPP
+#define TCOD_GUI_STATUSBAR_HPP
+#include "widget.hpp"
+class TCODLIB_GUI_API StatusBar : public Widget {
 public :
-	ToolBar(int x, int y, const char *name, const char *tip=NULL);
-	ToolBar(int x, int y, int w, const char *name, const char *tip=NULL);
-	~ToolBar();
+	StatusBar(int x,int y,int w, int h):Widget(x,y,w,h) {}
 	void render();
-	void setName(const char *name);
-	void addSeparator(const char *txt, const char *tip=NULL);
-	void computeSize();
-protected :
-	char *name;
-	int fixedWidth;
 };
-#endif /* TCOD_GUI_TOOLBAR_HPP */
+#endif /* TCOD_GUI_STATUSBAR_HPP */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/vbox.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/hbox.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,55 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "vbox.hpp"
+#include "hbox.hpp"
+
+HBox::HBox(int x, int y, int padding) : VBox(x,y,padding) {
+}
 
-void VBox::computeSize() {
-	int cury=y;
-	w=0;
+void HBox::computeSize() {
+	int curx=x;
+	h=0;
 	for (Widget **wid=content.begin(); wid != content.end(); wid ++ ) {
 		if ( (*wid)->isVisible() ) {
-			(*wid)->x=x;
-			(*wid)->y=cury;
+			(*wid)->y=y;
+			(*wid)->x=curx;
 			(*wid)->computeSize();
-			if ((*wid)->w > w) w=(*wid)->w;
-			cury+=(*wid)->h+padding;
+			if ((*wid)->h > h) h=(*wid)->h;
+			curx+=(*wid)->w+padding;
 		}
 	}
-	h=cury-y;
+	w=curx-x;
 	for (Widget **wid=content.begin(); wid != content.end(); wid ++ ) {
 		if ( (*wid)->isVisible() ) {
-			(*wid)->expand(w,(*wid)->h);
+			(*wid)->expand((*wid)->w,h);
 		}
 	}
 }
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/vbox.hpp` & `tcod-9.3.0/libtcod/LICENSE.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,30 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
- * All rights reserved.
- *
- * Redistribution and use in source and binary forms, with or without
- * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
- */
-#ifndef TCOD_GUI_VBOX_HPP
-#define TCOD_GUI_VBOX_HPP
-#include "container.hpp"
-class TCODLIB_GUI_API VBox : public Container {
-public :
-	VBox(int x, int y, int padding) : Container(x,y,0,0),padding(padding) {}
-	void computeSize();
-protected :
-	int padding;
-};
-#endif /* TCOD_GUI_VBOX_HPP */
+BSD 3-Clause License
+
+Copyright © 2008-2019, Jice and the libtcod contributors.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice,
+   this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/widget.cpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/widget.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "widget.hpp"
 
 #include <string.h>
 
 #include "../sys.hpp"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/gui/widget.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/widget.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_GUI_WIDGET_HPP
 #define TCOD_GUI_WIDGET_HPP
 #include "gui_portability.hpp"
 #include "../color.hpp"
 #include "../console.hpp"
 #include "../list.hpp"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/heightmap.cpp` & `tcod-9.3.0/libtcod/src/libtcod/heightmap.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "heightmap.hpp"
 
 #include <math.h>
 
 #include <cstring>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/heightmap.h` & `tcod-9.3.0/libtcod/src/libtcod/heightmap.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_HEIGHTMAP_H
 #define _TCOD_HEIGHTMAP_H
 
 #include "portability.h"
 #include "mersenne_types.h"
 #include "noise.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/heightmap.hpp` & `tcod-9.3.0/libtcod/src/libtcod/heightmap.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_HEIGHTMAP_HPP
 #define _TCOD_HEIGHTMAP_HPP
 
 #include "heightmap.h"
 #include "noise.hpp"
 /**
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/heightmap_c.c` & `tcod-9.3.0/libtcod/src/libtcod/heightmap_c.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "heightmap.h"
 
 #include <math.h>
 #include <stdlib.h>
 #include <string.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/image.cpp` & `tcod-9.3.0/libtcod/src/libtcod/image.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "image.hpp"
 
 #ifdef TCOD_IMAGE_SUPPORT
 
 TCODImage::TCODImage(const char *filename) : deleteData(true) {
   data = TCOD_image_load(filename);
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/image.h` & `tcod-9.3.0/libtcod/src/libtcod/image.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_IMAGE_H
 #define _TCOD_IMAGE_H
 
 #include "portability.h"
 #include "color.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/image.hpp` & `tcod-9.3.0/libtcod/src/libtcod/image.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_IMAGE_HPP
 #define _TCOD_IMAGE_HPP
 
 #include "color.hpp"
 
 #ifdef TCOD_IMAGE_SUPPORT
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/image_c.cpp` & `tcod-9.3.0/libtcod/src/libtcod/image_c.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "portability.h"
 #ifdef TCOD_IMAGE_SUPPORT
 #include "image.h"
 
 #include <stdlib.h>
 #include <stdarg.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/lex.cpp` & `tcod-9.3.0/libtcod/src/libtcod/lex.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "lex.hpp"
 
 #include <ctype.h>
 #include <string.h>
 #include <stdio.h>
 #include <stdlib.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/lex.h` & `tcod-9.3.0/libtcod/src/libtcod/lex.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 /*
  * This is a libtcod internal module.
  * Use at your own risks...
  */
 #ifndef _TCOD_LEX_H
 #define _TCOD_LEX_H
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/lex.hpp` & `tcod-9.3.0/libtcod/src/libtcod/lex.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 /*
  * This is a libtcod internal module.
  * Use at your own risks...
  */
 #ifndef _TCOD_LEX_HPP
 #define _TCOD_LEX_HPP
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/lex_c.c` & `tcod-9.3.0/libtcod/src/libtcod/lex_c.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "lex.h"
 
 #include <ctype.h>
 #include <string.h>
 #include <stdio.h>
 #include <stdlib.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/libtcod.h` & `tcod-9.3.0/libtcod/src/libtcod/libtcod.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _LIBTCOD_H
 #define _LIBTCOD_H
 
 #include "portability.h"
 #include "utility.h"
 #include "version.h"
@@ -56,14 +60,16 @@
 #include "console/printing.h"
 #include "console/rexpaint.h"
 
 #include "engine/backend.h"
 #include "engine/display.h"
 #include "engine/globals.h"
 
+#include "sdl2/event.h"
+
 #include "tileset/observer.h"
 #include "tileset/tileset.h"
 #include "tileset/tile.h"
 
 #ifdef __cplusplus
 #include "bresenham.hpp"
 #include "bsp.hpp"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/libtcod.hpp` & `tcod-9.3.0/libtcod/src/libtcod/mouse.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,52 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "libtcod.h"
+#include "mouse.hpp"
+
+#ifdef TCOD_CONSOLE_SUPPORT
+
+void TCODMouse::showCursor(bool visible) {
+	TCOD_mouse_show_cursor(visible);
+}
+
+bool TCODMouse::isCursorVisible() {
+	return TCOD_mouse_is_cursor_visible() != 0;
+}
+
+void TCODMouse::move(int x, int y) {
+	TCOD_mouse_move(x,y);
+}
+
+TCOD_mouse_t TCODMouse::getStatus() {
+	return TCOD_mouse_get_status();
+}
+
+#endif
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/libtcod_int.h` & `tcod-9.3.0/libtcod/src/libtcod/libtcod_int.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
  *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCODLIB_INT_H_
 #define TCODLIB_INT_H_
 #include <stdarg.h>
 #include <assert.h>
 #if defined(__ANDROID__)
 #include <android/log.h>
@@ -611,9 +615,21 @@
  *  Return true if the console is valid and the index is within it.
  */
 inline bool TCOD_console_is_index_valid_(const TCOD_Console* console,
                                          int x, int y)
 {
   return console && 0 <= x && x < console->w && 0 <= y && y < console->h;
 }
+TCOD_event_t TCOD_sys_handle_mouse_event(
+    const union SDL_Event* ev, TCOD_mouse_t* mouse);
+TCOD_event_t TCOD_sys_handle_key_event(
+    const union SDL_Event* ev, TCOD_key_t* key);
+/**
+ *  Private function, gets pointers of an old renderer.
+ */
+struct SDL_Window* TCOD_sys_get_sdl_window_(void);
+/**
+ *  Private function, gets pointers of an old renderer.
+ */
+struct SDL_Renderer* TCOD_sys_get_sdl_renderer_(void);
 #endif // __cplusplus
 #endif // TCODLIB_INT_H_
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/list.h` & `tcod-9.3.0/libtcod/src/libtcod/list.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_LIST_H
 #define _TCOD_LIST_H
 
 #include "portability.h"
 
 #ifdef __cplusplus
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/list.hpp` & `tcod-9.3.0/libtcod/src/libtcod/list.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_LIST_HPP
 #define _TCOD_LIST_HPP
 
 #include "list.h"
 
 #include <string.h> // memcpy
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/list_c.c` & `tcod-9.3.0/libtcod/src/libtcod/list_c.c`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "list.h"
 
 #include <stdlib.h> /* calloc */
 #include <string.h> /* NULL/memcpy */
 
 #include "utility.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/mersenne.cpp` & `tcod-9.3.0/libtcod/src/libtcod/mersenne.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "mersenne.hpp"
 
 #include <stdlib.h>
 
 #include "libtcod_int.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/mersenne.h` & `tcod-9.3.0/libtcod/src/libtcod/mersenne.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_RANDOM_H
 #define _TCOD_RANDOM_H
 
 #include "portability.h"
 #include "mersenne_types.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/mersenne.hpp` & `tcod-9.3.0/libtcod/src/libtcod/mersenne.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_RANDOM_HPP
 #define _TCOD_RANDOM_HPP
 
 #include "mersenne.h"
 /**
  @PageName random
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/mersenne_c.c` & `tcod-9.3.0/libtcod/src/libtcod/mersenne_c.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "mersenne.h"
 
 #include <time.h>
 #include <stdlib.h>
 #include <string.h>
 #include <math.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/mersenne_types.h` & `tcod-9.3.0/libtcod/src/libtcod/mersenne_types.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_RANDOM_TYPES_H
 #define _TCOD_RANDOM_TYPES_H
 struct TCOD_Random;
 typedef struct TCOD_Random *TCOD_random_t;
 
 /* dice roll */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/mouse.cpp` & `tcod-9.3.0/libtcod/src/libtcod/tileset/observer.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,36 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "mouse.hpp"
-
-#ifdef TCOD_CONSOLE_SUPPORT
-
-void TCODMouse::showCursor(bool visible) {
-	TCOD_mouse_show_cursor(visible);
-}
-
-bool TCODMouse::isCursorVisible() {
-	return TCOD_mouse_is_cursor_visible() != 0;
-}
-
-void TCODMouse::move(int x, int y) {
-	TCOD_mouse_move(x,y);
-}
-
-TCOD_mouse_t TCODMouse::getStatus() {
-	return TCOD_mouse_get_status();
-}
-
-#endif
+#include "observer.h"
+namespace tcod {
+namespace tileset {
+} // namespace tileset
+} // namespace tcod
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/mouse.h` & `tcod-9.3.0/libtcod/src/libtcod/mouse.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_MOUSE_H
 #define _TCOD_MOUSE_H
 
 #include "portability.h"
 
 #ifdef TCOD_CONSOLE_SUPPORT
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/mouse.hpp` & `tcod-9.3.0/libtcod/src/libtcod/mouse.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_MOUSE_HPP
 #define _TCOD_MOUSE_HPP
 
 #include "mouse.h"
 
 #ifdef TCOD_CONSOLE_SUPPORT
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/mouse_types.h` & `tcod-9.3.0/libtcod/src/libtcod/mouse_types.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_MOUSE_TYPES_H
 #define _TCOD_MOUSE_TYPES_H
 
 #include "portability.h"
 /* mouse data */
 typedef struct {
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/namegen.cpp` & `tcod-9.3.0/libtcod/src/libtcod/namegen.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 /*
 * Mingos' NameGen
 * This file was written by Dominik "Mingos" Marczuk.
 */
 #include "namegen.hpp"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/namegen.h` & `tcod-9.3.0/libtcod/src/libtcod/tileset/fallback.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,52 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-/*
-* Mingos' NameGen
-* This file was written by Dominik "Mingos" Marczuk.
-*/
-
-#ifndef _TCOD_NAMEGEN_H
-#define _TCOD_NAMEGEN_H
-
-#include "portability.h"
-#include "list.h"
-#include "mersenne.h"
-
+#ifndef LIBTCOD_TILESET_FALLBACK_H_
+#define LIBTCOD_TILESET_FALLBACK_H_
 #ifdef __cplusplus
-extern "C" {
-#endif
-/* the generator typedef */
-struct TCOD_NameGen;
-typedef struct TCOD_NameGen *TCOD_namegen_t;
-
-/* parse a file with syllable sets */
-TCODLIB_API void TCOD_namegen_parse (const char * filename, TCOD_random_t random);
-/* generate a name */
-TCODLIB_API char * TCOD_namegen_generate (char * name, bool allocate);
-/* generate a name using a custom generation rule */
-TCODLIB_API char * TCOD_namegen_generate_custom (char * name, char * rule, bool allocate);
-/* retrieve the list of all available syllable set names */
-TCODLIB_API TCOD_list_t TCOD_namegen_get_sets (void);
-/* delete a generator */
-TCODLIB_API void TCOD_namegen_destroy (void);
+#include <array>
+#include <memory>
+#endif // __cplusplus
+#include "tileset.h"
 #ifdef __cplusplus
-}
-#endif
-#endif
+namespace tcod {
+namespace tileset {
+/**
+ *  Try to return a fall-back Tileset, may return nullptr or throw an error.
+ *
+ *  Used when one is needed, but was not provided by the user.
+ */
+auto new_fallback_tileset(const std::array<int, 2>& tile_size = {12, 16})
+-> std::unique_ptr<Tileset>;
+} // namespace tileset
+} // namespace tcod
+#endif // __cplusplus
+#endif // LIBTCOD_TILESET_FALLBACK_H_
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/namegen.hpp` & `tcod-9.3.0/libtcod/src/libtcod/namegen.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 /*
 * Mingos' NameGen
 * This file was written by Dominik "Mingos" Marczuk.
 */
 
 #ifndef _TCOD_NAMEGEN_HPP
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/namegen_c.c` & `tcod-9.3.0/libtcod/src/libtcod/namegen_c.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 /*
 * Mingos' NameGen
 * This file was written by Dominik "Mingos" Marczuk.
 */
 #include "namegen.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/noise.cpp` & `tcod-9.3.0/libtcod/src/libtcod/noise.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "noise.hpp"
 
 #include <stdlib.h>
 TCODNoise::TCODNoise(int dimensions, TCOD_noise_type_t type) {
 	data = TCOD_noise_new(dimensions, TCOD_NOISE_DEFAULT_HURST, TCOD_NOISE_DEFAULT_LACUNARITY, TCODRandom::getInstance()->data);
 	TCOD_noise_set_type(data,type);
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/noise.h` & `tcod-9.3.0/libtcod/src/libtcod/noise.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_PERLIN_H
 #define _TCOD_PERLIN_H
 
 #include "portability.h"
 #include "mersenne_types.h"
 #include "noise_defaults.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/noise.hpp` & `tcod-9.3.0/libtcod/src/libtcod/noise.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_PERLIN_HPP
 #define _TCOD_PERLIN_HPP
 
 #include "mersenne.hpp"
 #include "noise.h"
 #include "noise_defaults.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/noise_c.c` & `tcod-9.3.0/libtcod/src/libtcod/noise_c.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "noise.h"
 
 #include <math.h>
 #include <stdlib.h>
 #include <string.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/noise_defaults.h` & `tcod-9.3.0/libtcod/src/libtcod/noise_defaults.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_NOISE_DEFAULTS
 #define _TCOD_NOISE_DEFAULTS
 
 #define TCOD_NOISE_MAX_OCTAVES			128
 #define TCOD_NOISE_MAX_DIMENSIONS		4
 #define TCOD_NOISE_DEFAULT_HURST        0.5f
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/parser.cpp` & `tcod-9.3.0/libtcod/src/libtcod/parser.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "parser.hpp"
 
 #include <stdlib.h>
 #include <string.h>
 #include <stdio.h>
 #include <stdarg.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/parser.h` & `tcod-9.3.0/libtcod/src/libtcod/parser.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_PARSER_H
 #define _TCOD_PARSER_H
 
 #include "portability.h"
 #include "color.h"
 #include "list.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/parser.hpp` & `tcod-9.3.0/libtcod/src/libtcod/parser.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_PARSER_HPP
 #define _TCOD_PARSER_HPP
 
 #include "color.hpp"
 #include "list.hpp"
 #include "parser.h"
```

#### html2text {}

```diff
@@ -1,37 +1,38 @@
-/* libtcod * Copyright Â© 2008-2019 Jice and the libtcod contributors. * All
-rights reserved. * * Redistribution and use in source and binary forms, with or
-without * modification, are permitted provided that the following conditions
-are met: * * Redistributions of source code must retain the above copyright *
-notice, this list of conditions and the following disclaimer. * *
-Redistributions in binary form must reproduce the above copyright * notice,
-this list of conditions and the following disclaimer in the * documentation
-and/or other materials provided with the distribution. * * The name of
-copyright holder nor the names of its contributors may not * be used to endorse
-or promote products derived from this software * without specific prior written
-permission. * * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND
-CONTRIBUTORS * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT
-NOT LIMITED * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
-PARTICULAR * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-* CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, *
-EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, *
-PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; *
-OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, *
-WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR *
-OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF *
-ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. */ #ifndef _TCOD_PARSER_HPP #define
-_TCOD_PARSER_HPP #include "color.hpp" #include "list.hpp" #include "parser.h" /
-** @PageName parser @PageTitle File parser @PageCategory Base toolkits
-@PageDesc This toolkit provides an easy way to parse complex text configuration
-files. It has two main advantages compared to a standard XML SAX parser: * The
-configuration file format is more human readable than XML * The parser knows
-some data types that it automatically converts to C variables (see Standard
-data_types) */ /** @PageName parser_format @PageFather parser @PageTitle The
-libtcod config file format @FuncTitle Comments @FuncDesc Your file can contain
-single line or multi-line comments :
+/* BSD 3-Clause License * * Copyright Â© 2008-2019, Jice and the libtcod
+contributors. * All rights reserved. * * Redistribution and use in source and
+binary forms, with or without * modification, are permitted provided that the
+following conditions are met: * * 1. Redistributions of source code must retain
+the above copyright notice, * this list of conditions and the following
+disclaimer. * * 2. Redistributions in binary form must reproduce the above
+copyright notice, * this list of conditions and the following disclaimer in the
+documentation * and/or other materials provided with the distribution. * * 3.
+Neither the name of the copyright holder nor the names of its * contributors
+may be used to endorse or promote products derived from * this software without
+specific prior written permission. * * THIS SOFTWARE IS PROVIDED BY THE
+COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" * AND ANY EXPRESS OR IMPLIED
+WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE * IMPLIED WARRANTIES OF
+MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE * ARE DISCLAIMED. IN NO
+EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE * LIABLE FOR ANY DIRECT,
+INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR * CONSEQUENTIAL DAMAGES
+(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF * SUBSTITUTE GOODS OR SERVICES;
+LOSS OF USE, DATA, OR PROFITS; OR BUSINESS * INTERRUPTION) HOWEVER CAUSED AND
+ON ANY THEORY OF LIABILITY, WHETHER IN * CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) * ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE * POSSIBILITY OF SUCH DAMAGE. */ #ifndef
+_TCOD_PARSER_HPP #define _TCOD_PARSER_HPP #include "color.hpp" #include
+"list.hpp" #include "parser.h" /** @PageName parser @PageTitle File parser
+@PageCategory Base toolkits @PageDesc This toolkit provides an easy way to
+parse complex text configuration files. It has two main advantages compared to
+a standard XML SAX parser: * The configuration file format is more human
+readable than XML * The parser knows some data types that it automatically
+converts to C variables (see Standard_data_types) */ /** @PageName
+parser_format @PageFather parser @PageTitle The libtcod config file format
+@FuncTitle Comments @FuncDesc Your file can contain single line or multi-line
+comments :
 // This is a single line comment
 /*
    This is a
    multi-line comment
 */
 Multi-line comments can be nested :
 /*
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/parser_c.c` & `tcod-9.3.0/libtcod/src/libtcod/parser_c.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "parser.h"
 
 #include <stdlib.h>
 #include <string.h>
 #include <stdio.h>
 #include <stdarg.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/path.cpp` & `tcod-9.3.0/libtcod/src/libtcod/path.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "path.hpp"
 
 
 TCODPath::TCODPath(const TCODMap *map, float diagonalCost) {
   data = TCOD_path_new_using_map(map->data, diagonalCost);
 }
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/path.h` & `tcod-9.3.0/libtcod/src/libtcod/path.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_PATH_H
 #define _TCOD_PATH_H
 
 #include "portability.h"
 #include "fov_types.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/path.hpp` & `tcod-9.3.0/libtcod/src/libtcod/path.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_PATH_HPP
 #define _TCOD_PATH_HPP
 
 #include "fov.hpp"
 #include "path.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/pathfinding/astar.cpp` & `tcod-9.3.0/libtcod/src/libtcod/tree_c.c`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,49 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "astar.h"
+#include "tree.h"
+
+#include <stdlib.h>
+
+TCOD_tree_t *TCOD_tree_new(void) {
+	return (TCOD_tree_t *)calloc(1,sizeof(TCOD_tree_t));
+}
+
+void TCOD_tree_add_son(TCOD_tree_t *node, TCOD_tree_t *son) {
+	TCOD_tree_t *lastson = node->sons;
+	son->father=node;
+	while ( lastson && lastson->next ) lastson=lastson->next;
+	if ( lastson ) {
+		lastson->next=son;
+	} else {
+		node->sons=son;
+	}
+}
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/pathfinding/astar.h` & `tcod-9.3.0/libtcod/src/libtcod/libtcod.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef LIBTCOD_PATHFINDING_ASTAR_H_
-#define LIBTCOD_PATHFINDING_ASTAR_H_
-#ifdef __cplusplus
-namespace tcod {
-namespace pathfinding {
-} // namespace pathfinding
-} // namespace tcod
-#endif // __cplusplus
-#endif // LIBTCOD_PATHFINDING_ASTAR_H_
+#include "libtcod.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/pathfinding/dijkstra.h` & `tcod-9.3.0/libtcod/src/libtcod/pathfinding/dijkstra.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_PATHFINDING_DIJKSTRA_H_
 #define LIBTCOD_PATHFINDING_DIJKSTRA_H_
 #ifdef __cplusplus
 #include <cstdbool>
 #include <cstddef>
 #include <algorithm>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/pathfinding/generic.h` & `tcod-9.3.0/libtcod/src/libtcod/pathfinding/generic.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_PATHFINDING_GENERIC_H_
 #define LIBTCOD_PATHFINDING_GENERIC_H_
 #ifdef __cplusplus
 #include <cstdbool>
 #include <cstddef>
 #include <algorithm>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/path_c.c` & `tcod-9.3.0/libtcod/src/libtcod/path_c.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "path.h"
 
 #include <stdlib.h>
 #include <stdio.h>
 #include <string.h>
 #include <math.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/portability.h` & `tcod-9.3.0/libtcod/src/libtcod/portability.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_PORTABILITY_H
 #define LIBTCOD_PORTABILITY_H
 /* uncomment to disable unicode support */
 /*#define NO_UNICODE */
 
 /* uncomment to disable opengl support */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/console_2tris.glslf` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/console_2tris.glslf`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/console_2tris.glslv` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/console_2tris.glslv`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/console_grid.glslv` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/console_grid.glslv`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_display.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_display.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,83 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "gl2_display.h"
 
 #include "gl2_ext_.h"
 #include <SDL.h>
 
 namespace tcod {
 namespace sdl2 {
 static std::shared_ptr<void> new_gl_context(OpenGL2Display& self)
 {
   std::shared_ptr<void> new_context(
-      SDL_GL_CreateContext(self.get_window()),
+      SDL_GL_CreateContext(self.get_sdl_window()),
       [](SDL_GLContext context){ SDL_GL_DeleteContext(context); });
   if (!new_context) { throw std::runtime_error(SDL_GetError()); }
   if(!gladLoadGLLoader(SDL_GL_GetProcAddress)) {
     throw std::runtime_error("Failed to invoke the GLAD loader.");
   }
   SDL_GL_SetSwapInterval(0);
   return new_context;
 }
 OpenGL2Display::OpenGL2Display(std::shared_ptr<Tileset> tileset,
-                         std::pair<int, int> window_size, int window_flags,
+                         std::array<int, 2> window_size, int window_flags,
                          const std::string& title)
 : WindowedDisplay(window_size, window_flags | SDL_WINDOW_OPENGL, title),
   glcontext_(new_gl_context(*this)),
   tcod_renderer_(tileset)
 {}
 void OpenGL2Display::set_tileset(std::shared_ptr<Tileset> tileset)
 {
   if (!tileset) {
     throw std::invalid_argument("tileset must not be nullptr.");
   }
   tcod_renderer_ = OpenGL2Renderer(tileset);
 }
-void OpenGL2Display::present(const TCOD_Console* console)
+void OpenGL2Display::accumulate(const TCOD_Console* console)
 {
   int window_size[2];
-  SDL_GL_GetDrawableSize(get_window(), &window_size[0], &window_size[1]);
+  SDL_GL_GetDrawableSize(get_sdl_window(), &window_size[0], &window_size[1]);
   glViewport(0,0,window_size[0],window_size[1]);
-
   tcod_renderer_.render(console);
-  SDL_GL_SwapWindow(get_window());
-
   update_pixel_to_tile_scale(console);
 }
+void OpenGL2Display::present(const TCOD_Console* console)
+{
+  accumulate(console);
+  SDL_GL_SwapWindow(get_sdl_window());
+}
 auto OpenGL2Display::read_pixels() const -> Image
 {
   return tcod_renderer_.read_pixels();
 }
 } // namespace sdl2
 } // namespace tcod
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_display.h` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_renderer.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,71 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef LIBTCOD_SDL2_GL2_DISPLAY_H_
-#define LIBTCOD_SDL2_GL2_DISPLAY_H_
-
-#include "gl2_renderer.h"
-#include "sdl2_display.h"
+#ifndef LIBTCOD_SDL2_GL2_RENDERER_H_
+#define LIBTCOD_SDL2_GL2_RENDERER_H_
+#ifdef __cplusplus
+#endif /* __cplusplus */
+#include <memory>
 
+#include "gl_alias.h"
+#include "gl2_raii.h"
+#include "../color/color.h"
+#include "../console_types.h"
+#include "../tileset/observer.h"
+#include "../tileset/tileset.h"
+#include "../utility/vector2.h"
+#ifdef __cplusplus
 namespace tcod {
 namespace sdl2 {
-class OpenGL2Display: public WindowedDisplay {
+using tcod::image::Image;
+using tcod::tileset::Tileset;
+class OpenGL2Renderer {
  public:
-  explicit OpenGL2Display(
-      std::shared_ptr<Tileset> tileset,
-      std::pair<int, int> window_size,
-      int window_flags,
-      const std::string& title);
-  virtual void set_tileset(std::shared_ptr<Tileset> tileset) override;
-  virtual void present(const TCOD_Console*) override;
-  virtual auto read_pixels() const -> Image override;
+  explicit OpenGL2Renderer(OpenGLTilesetAlias alias);
+  explicit OpenGL2Renderer(std::shared_ptr<Tileset> tileset)
+  : OpenGL2Renderer(OpenGLTilesetAlias(tileset))
+  {}
+  OpenGL2Renderer(const OpenGL2Renderer&) = delete;
+  OpenGL2Renderer& operator=(const OpenGL2Renderer&) = delete;
+  OpenGL2Renderer(OpenGL2Renderer&&) noexcept;
+  OpenGL2Renderer& operator=(OpenGL2Renderer&&) noexcept;
+  ~OpenGL2Renderer() noexcept;
+
+  void render(const TCOD_Console* console);
+  auto read_pixels() const -> Image;
  private:
-  std::shared_ptr<void> glcontext_;
-  OpenGL2Renderer tcod_renderer_;
+  class impl;
+  std::unique_ptr<impl> impl_;
 };
 } // namespace sdl2
 } // namespace tcod
-#endif //LIBTCOD_SDL2_GL2_DISPLAY_H_
+#endif // __cplusplus
+#endif // LIBTCOD_SDL2_GL2_RENDERER_H_
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_ext_.h` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_ext_.h`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_SDL2_GL2_EXT_H_
 #define LIBTCOD_SDL2_GL2_EXT_H_
 #include <stdexcept>
 
 #include "../../vendor/glad.h"
 namespace tcod {
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_raii.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_raii.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "gl2_raii.h"
 
 #include <array>
 #include <string>
 #include <utility>
 #include <vector>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_raii.h` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_raii.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_SDL2_GL2_RAII_H_
 #define LIBTCOD_SDL2_GL2_RAII_H_
 
 #include <cstddef>
 #include <cstdint>
 #include <string>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_renderer.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/gl2_renderer.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "gl2_renderer.h"
 
 #include <array>
 #include <string>
 #include <utility>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/gl2_renderer.h` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_renderer.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,75 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef LIBTCOD_SDL2_GL2_RENDERER_H_
-#define LIBTCOD_SDL2_GL2_RENDERER_H_
+#ifndef LIBTCOD_SDL2_SDL2_RENDERER_H_
+#define LIBTCOD_SDL2_SDL2_RENDERER_H_
 #ifdef __cplusplus
+#include <tuple>
 #endif /* __cplusplus */
-#include <memory>
 
-#include "gl_alias.h"
-#include "gl2_raii.h"
+#include "sdl2_alias.h"
 #include "../color/color.h"
 #include "../console_types.h"
 #include "../tileset/observer.h"
 #include "../tileset/tileset.h"
 #include "../utility/vector2.h"
 #ifdef __cplusplus
+struct SDL_Renderer;
+struct SDL_Texture;
 namespace tcod {
 namespace sdl2 {
 using tcod::image::Image;
 using tcod::tileset::Tileset;
-class OpenGL2Renderer {
+class SDL2Renderer {
  public:
-  explicit OpenGL2Renderer(OpenGLTilesetAlias alias);
-  explicit OpenGL2Renderer(std::shared_ptr<Tileset> tileset)
-  : OpenGL2Renderer(OpenGLTilesetAlias(tileset))
-  {}
-  OpenGL2Renderer(const OpenGL2Renderer&) = delete;
-  OpenGL2Renderer& operator=(const OpenGL2Renderer&) = delete;
-  OpenGL2Renderer(OpenGL2Renderer&&) noexcept;
-  OpenGL2Renderer& operator=(OpenGL2Renderer&&) noexcept;
-  ~OpenGL2Renderer() noexcept;
+  SDL2Renderer();
+  SDL2Renderer(struct SDL_Renderer* renderer, SDL2TilesetAlias alias);
+  SDL2Renderer(struct SDL_Renderer* renderer,
+               std::shared_ptr<Tileset> tileset);
 
-  void render(const TCOD_Console* console);
+  SDL2Renderer(const SDL2Renderer&) = delete;
+  SDL2Renderer& operator=(const SDL2Renderer&) = delete;
+  SDL2Renderer(SDL2Renderer&&) noexcept;
+  SDL2Renderer& operator=(SDL2Renderer&&) noexcept;
+
+  ~SDL2Renderer();
+
+  auto render(const TCOD_Console* console) -> struct SDL_Texture*;
   auto read_pixels() const -> Image;
+
  private:
   class impl;
   std::unique_ptr<impl> impl_;
 };
 } // namespace sdl2
 } // namespace tcod
-#endif // __cplusplus
-#endif // LIBTCOD_SDL2_GL2_RENDERER_H_
+#endif /* __cplusplus */
+#endif /* LIBTCOD_SDL2_SDL2_RENDERER_H_ */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/gl_alias.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/gl_alias.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "gl_alias.h"
 
 #include <map>
 #include <memory>
 #include <mutex>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/gl_alias.h` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/gl_alias.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_SDL2_GL_ALIAS_H_
 #define LIBTCOD_SDL2_GL_ALIAS_H_
 #include <cstdint>
 #include <array>
 #include <memory>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/legacy_backend.h` & `tcod-9.3.0/libtcod/src/libtcod/tree.hpp`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,57 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef LIBTCOD_SDL2_LEGACY_BACKEND_H_
-#define LIBTCOD_SDL2_LEGACY_BACKEND_H_
+#ifndef _TCOD_TREE_HPP
+#define _TCOD_TREE_HPP
+
+#include "tree.h"
+
+class TCODLIB_API TCODTree {
+public :
+	TCODTree *next;
+	TCODTree *father;
+	TCODTree *sons;
+
+	TCODTree() : next(NULL),father(NULL),sons(NULL){}
+	void addSon(TCODTree *data) {
+		data->father=this;
+		TCODTree *lastson = sons;
+		while ( lastson && lastson->next ) lastson=lastson->next;
+		if ( lastson ) {
+			lastson->next=data;
+		} else {
+			sons=data;
+		}
+	}
+
+};
 
-#ifdef __cplusplus
-namespace tcod {
-namespace sdl2 {
-} // namespace sdl2
-} // namespace tcod
-#endif /* __cplusplus */
-#endif /* LIBTCOD_SDL2_LEGACY_BACKEND_H_ */
+#endif
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_alias.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_alias.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "sdl2_alias.h"
 
 #include <map>
 #include <memory>
 #include <mutex>
 #include <stdexcept>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_alias.h` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_alias.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_SDL2_SDL2_ALIAS_H_
 #define LIBTCOD_SDL2_SDL2_ALIAS_H_
 #include <memory>
 
 #include "../console.h"
 #include "../tileset/observer.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_display.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_display.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,88 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "sdl2_display.h"
 
 #include <cstdint>
 #include <stdexcept>
 
 #include "../console.h"
 #include "../libtcod_int.h"
 
 #include <SDL.h>
 
 namespace tcod {
 namespace sdl2 {
-WindowedDisplay::WindowedDisplay(std::pair<int, int> window_size,
-                                 int window_flags, const std::string& title)
+/**
+ *  Initialize a return a new SDL2 window.
+ *
+ *  If the SDL_WINDOW_OPENGL flag is set then it will create an OpenGL 2.0
+ *  context.
+ */
+static auto init_sdl2_window(
+    const std::array<int, 2>& window_size,
+    int window_flags,
+    const std::string& title)
+-> std::shared_ptr<struct SDL_Window>
 {
-  int width = window_size.first;
-  int height = window_size.second;
+  int width = window_size.at(0);
+  int height = window_size.at(1);
   if (width < 0 || height < 0) {
     throw std::invalid_argument("width and height must be non-negative.");
   }
   if (SDL_Init(SDL_INIT_VIDEO | SDL_INIT_EVENTS | SDL_INIT_TIMER)) {
     throw std::runtime_error(SDL_GetError());
   }
   SDL_GL_SetAttribute(SDL_GL_CONTEXT_PROFILE_MASK, SDL_GL_CONTEXT_PROFILE_CORE);
   SDL_GL_SetAttribute(SDL_GL_CONTEXT_MAJOR_VERSION, 2);
   SDL_GL_SetAttribute(SDL_GL_CONTEXT_MINOR_VERSION, 0);
-  window_ = std::shared_ptr<SDL_Window>(
+  auto window = std::shared_ptr<SDL_Window>(
       SDL_CreateWindow(
           title.c_str(), SDL_WINDOWPOS_UNDEFINED, SDL_WINDOWPOS_UNDEFINED,
           width, height, window_flags),
-      [](SDL_Window* window){ SDL_DestroyWindow(window); });
-  if (!window_) { throw std::runtime_error(SDL_GetError()); }
-}
+      [](SDL_Window* window_ptr){ SDL_DestroyWindow(window_ptr); });
+  if (!window) { throw std::runtime_error(SDL_GetError()); }
+  return window;
+}
+WindowedDisplay::WindowedDisplay(std::shared_ptr<struct SDL_Window> window)
+: window_(window)
+{}
+WindowedDisplay::WindowedDisplay(const std::array<int, 2>& window_size,
+                                 int window_flags, const std::string& title)
+: WindowedDisplay(init_sdl2_window(window_size, window_flags, title))
+{}
 void WindowedDisplay::set_title(const std::string& title)
 {
   if (!window_) { throw std::logic_error("Unresolved class invariant."); }
   SDL_SetWindowTitle(window_.get(), title.c_str());
 }
 std::string WindowedDisplay::get_title()
 {
@@ -89,43 +110,50 @@
     static_cast<double>(TCOD_console_get_width(console))
     / static_cast<double>(width),
     static_cast<double>(TCOD_console_get_height(console))
     / static_cast<double>(height),
   };
 }
 
-SDL2Display::SDL2Display(std::shared_ptr<Tileset> tileset,
-                         std::pair<int, int> window_size, int window_flags,
-                         const std::string& title)
+SDL2Display::SDL2Display(
+    std::shared_ptr<Tileset> tileset,
+    const std::array<int, 2>& window_size,
+    int window_flags,
+    const std::string& title)
 : WindowedDisplay(window_size, window_flags, title)
 {
   // Configure SDL2 renderer.
   renderer_ = std::shared_ptr<SDL_Renderer>(
-      SDL_CreateRenderer(get_window(), -1, SDL_RENDERER_TARGETTEXTURE),
+      SDL_CreateRenderer(get_sdl_window(), -1, SDL_RENDERER_TARGETTEXTURE),
       [](SDL_Renderer* renderer){ SDL_DestroyRenderer(renderer); });
   if (!renderer_) { throw std::runtime_error(SDL_GetError()); }
   // Configure libtcod renderer.
   set_tileset(tileset);
 }
 void SDL2Display::set_tileset(std::shared_ptr<Tileset> tileset)
 {
   if (!renderer_) { throw std::logic_error("Unresolved class invariant."); }
   if (!tileset) {
     throw std::invalid_argument("tileset must not be nullptr.");
   }
   tcod_renderer_ = SDL2Renderer(renderer_.get(), tileset);
 }
-void SDL2Display::present(const TCOD_Console* console)
+void SDL2Display::accumulate(const TCOD_Console* console)
 {
   if (!renderer_) { throw std::logic_error("Unresolved class invariant."); }
   SDL_Texture* backbuffer = tcod_renderer_.render(console);
   SDL_RenderClear(renderer_.get());
   SDL_RenderCopy(renderer_.get(), backbuffer, nullptr, nullptr);
-  SDL_RenderPresent(renderer_.get());
   update_pixel_to_tile_scale(console);
 }
+void SDL2Display::present(const TCOD_Console* console)
+{
+  if (!renderer_) { throw std::logic_error("Unresolved class invariant."); }
+  accumulate(console);
+  SDL_RenderPresent(renderer_.get());
+}
 auto SDL2Display::read_pixels() const -> Image
 {
   return tcod_renderer_.read_pixels();
 }
 } // namespace sdl2
 } // namespace tcod
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_display.h` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_display.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_SDL2_SDL2_DISPLAY_H_
 #define LIBTCOD_SDL2_SDL2_DISPLAY_H_
 
 #ifdef __cplusplus
+#include <array>
 #include <memory>
 #include <string>
-#include <utility>
 #endif // __cplusplus
 
 #include "sdl2_renderer.h"
 #include "../engine/display.h"
 
 struct SDL_Window;
 struct SDL_Renderer;
@@ -44,57 +48,70 @@
 namespace sdl2 {
 using tcod::image::Image;
 /**
  *  Incomplete interface for subclasses expecting an SDL2 window.
  */
 class WindowedDisplay: public engine::Display {
  public:
-  WindowedDisplay(std::pair<int, int> window_size, int window_flags,
+  explicit WindowedDisplay(std::shared_ptr<struct SDL_Window> window);
+  WindowedDisplay(const std::array<int, 2>& window_size, int window_flags,
                   const std::string& title);
   virtual void set_title(const std::string& title) override;
   virtual std::string get_title() override;
   virtual void set_fullscreen(bool fullscreen) override;
   virtual int get_fullscreen() override;
-  SDL_Window* get_window() { return window_.get(); }
   /**
    *  Return the tile coordinate of the last console given to present.
    */
-  virtual auto pixel_to_tile(const std::pair<double, double>& xy)
-      -> std::pair<double, double> override
+  virtual auto pixel_to_tile(const std::array<double, 2>& xy)
+      -> std::array<double, 2> override
   {
     return {
-        xy.first * pixel_to_tile_scale.first,
-        xy.second * pixel_to_tile_scale.second,
+        std::get<0>(xy) * std::get<0>(pixel_to_tile_scale),
+        std::get<1>(xy) * std::get<1>(pixel_to_tile_scale),
     };
   }
+  virtual auto get_sdl_window() -> struct SDL_Window* override
+  {
+    return window_.get();
+  }
+  virtual auto get_sdl_renderer() -> struct SDL_Renderer* override
+  {
+    return nullptr;
+  }
  protected:
   /**
    *  Update the scale using a console/tileset and the current window size.
    */
   void update_pixel_to_tile_scale(const TCOD_Console* console);
  private:
   std::shared_ptr<SDL_Window> window_;
   /**
    *  Scale used to convert from pixel coordinate to tile coordinate.
    */
-  std::pair<double, double> pixel_to_tile_scale = {1.0, 1.0};
+  std::array<double, 2> pixel_to_tile_scale = {1.0, 1.0};
 };
 /**
  *  Display interface using a basic SDL2 renderer.
  */
 class SDL2Display: public WindowedDisplay {
  public:
   SDL2Display(
       std::shared_ptr<Tileset> tileset,
-      std::pair<int, int> window_size,
+      const std::array<int, 2>& window_size,
       int window_flags,
       const std::string& title);
   virtual void set_tileset(std::shared_ptr<Tileset> tileset) override;
+  virtual void accumulate(const TCOD_Console*) override;
   virtual void present(const TCOD_Console*) override;
   virtual auto read_pixels() const -> Image override;
+  virtual auto get_sdl_renderer() -> struct SDL_Renderer* override
+  {
+    return renderer_.get();
+  }
  private:
   std::shared_ptr<SDL_Renderer> renderer_;
   SDL2Renderer tcod_renderer_;
 };
 } // namespace sdl2
 } // namespace tcod
 #endif // __cplusplus
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_renderer.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sdl2/sdl2_renderer.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "sdl2_renderer.h"
 
 #include <map>
 
 #include <SDL.h>
 namespace tcod {
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sdl2/sdl2_renderer.h` & `tcod-9.3.0/libtcod/src/libtcod/tileset/tilesheet.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,89 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef LIBTCOD_SDL2_SDL2_RENDERER_H_
-#define LIBTCOD_SDL2_SDL2_RENDERER_H_
+#ifndef LIBTCOD_TILESET_TILESHEET_H_
+#define LIBTCOD_TILESET_TILESHEET_H_
 #ifdef __cplusplus
-#include <tuple>
-#endif /* __cplusplus */
+#include <memory>
+#include <string>
+#include <utility>
+#endif // __cplusplus
 
-#include "sdl2_alias.h"
-#include "../color/color.h"
-#include "../console_types.h"
-#include "../tileset/observer.h"
-#include "../tileset/tileset.h"
-#include "../utility/vector2.h"
+#include "../color/canvas.h"
+#include "tile.h"
 #ifdef __cplusplus
-struct SDL_Renderer;
-struct SDL_Texture;
 namespace tcod {
-namespace sdl2 {
-using tcod::image::Image;
-using tcod::tileset::Tileset;
-class SDL2Renderer {
+namespace tileset {
+using image::Image;
+/**
+ *  The layout of tiles on a tile-sheet.
+ */
+struct TilesheetLayout {
+  int tile_width;
+  int tile_height;
+  int columns;
+  int rows;
+};
+class Tilesheet {
  public:
-  SDL2Renderer();
-  SDL2Renderer(struct SDL_Renderer* renderer, SDL2TilesetAlias alias);
-  SDL2Renderer(struct SDL_Renderer* renderer,
-               std::shared_ptr<Tileset> tileset);
-
-  SDL2Renderer(const SDL2Renderer&) = delete;
-  SDL2Renderer& operator=(const SDL2Renderer&) = delete;
-  SDL2Renderer(SDL2Renderer&&) noexcept;
-  SDL2Renderer& operator=(SDL2Renderer&&) noexcept;
-
-  ~SDL2Renderer();
-
-  auto render(const TCOD_Console* console) -> struct SDL_Texture*;
-  auto read_pixels() const -> Image;
-
+  Tilesheet();
+  explicit Tilesheet(const Image& canvas, const TilesheetLayout& layout);
+  explicit Tilesheet(const Image& canvas, const std::pair<int, int>& layout);
+  Tilesheet(Tilesheet&&) noexcept;
+  Tilesheet& operator=(Tilesheet&&) noexcept;
+  Tilesheet(const Tilesheet&);
+  Tilesheet& operator=(const Tilesheet&);
+  ~Tilesheet() noexcept;
+  /**
+   *  Return the tile at `x` and `y`.
+   */
+  Image get_tile(int x, int y) const;
+  /**
+   *  Return the tile at `n`.
+   */
+  Image get_tile(int n) const;
+  int get_tile_width() const noexcept;
+  int get_tile_height() const noexcept;
+  int get_columns() const noexcept;
+  int get_rows() const noexcept;
+  int count() const noexcept;
  private:
   class impl;
   std::unique_ptr<impl> impl_;
 };
-} // namespace sdl2
+/**
+ *  Load a Tilesheet from an image file.
+ */
+Tilesheet LoadTilesheet(const std::string &filename);
+} // namespace tileset
 } // namespace tcod
-#endif /* __cplusplus */
-#endif /* LIBTCOD_SDL2_SDL2_RENDERER_H_ */
+#endif // __cplusplus
+#endif /* LIBTCOD_TILESET_TILESHEET_H_ */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sys.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sys.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "sys.hpp"
 
 #include <stdio.h>
 #include <stdarg.h>
 
 #ifdef TCOD_OSUTIL_SUPPORT
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sys.h` & `tcod-9.3.0/libtcod/src/libtcod/sys.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_SYS_H
 #define _TCOD_SYS_H
 
 #include "portability.h"
 #include "list.h"
 #include "image.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sys.hpp` & `tcod-9.3.0/libtcod/src/libtcod/sys.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_SYS_HPP
 #define _TCOD_SYS_HPP
 
 #include "image.hpp"
 #include "mouse.hpp"
 #include "sys.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sys_c.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sys_c.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "sys.h"
 
 #include <ctype.h>
 #include <stdlib.h>
 #include <stdio.h>
 #include <stdarg.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sys_opengl_c.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sys_opengl_c.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 /*
  * This renderer is mostly copied and pasted from Antagonist's SkyFire GLSL roguelike engine
  */
 #ifndef TCOD_BARE
 #include "sys.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sys_sdl2_c.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sys_sdl2_c.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_BARE
 #include "sys.h"
 
 #include <stdio.h>
 #include <string.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sys_sdl_c.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sys_sdl_c.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
  *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_BARE
 #include "mouse.h"
 #include "sys.h"
 
 #include <array>
 #include <string.h>
@@ -1244,17 +1248,17 @@
  *  Convert a pixel coordinate to a tile coordinate using global state.
  */
 void TCOD_sys_pixel_to_tile(double* x, double* y)
 {
   if (!x || !y) { return; }
   auto display = tcod::engine::get_display();
   if (display) {
-    std::pair<double, double> xy = display->pixel_to_tile({*x, *y});
-    *x = xy.first;
-    *y = xy.second;
+    std::array<double, 2> xy = display->pixel_to_tile({*x, *y});
+    *x = std::get<0>(xy);
+    *y = std::get<1>(xy);
   } else {
     *x = (*x - TCOD_ctx.fullscreen_offsetx) / TCOD_ctx.font_width;
     *y = (*y - TCOD_ctx.fullscreen_offsety) / TCOD_ctx.font_height;
   }
 }
 /**
  *  Parse the coordinates and motion of an SDL event into a libtcod mouse
@@ -1281,21 +1285,26 @@
       mouse.y = ev.button.y;
       mouse.dx = mouse.dy = 0;
       break;
     default: return;
   }
   auto display = tcod::engine::get_display();
   if (display) {
-    std::pair<int, int> cell_xy = display->pixel_to_tile({mouse.x, mouse.y});
-    std::pair<int, int> prev_cell_xy = display->pixel_to_tile(
-        {mouse.x - mouse.dx, mouse.y - mouse.dy});
-    mouse.cx = cell_xy.first;
-    mouse.cy = cell_xy.second;
-    mouse.dcx = cell_xy.first - prev_cell_xy.first;
-    mouse.dcy = cell_xy.second - prev_cell_xy.second;
+    auto to_tile = [&](double x, double y) -> std::array<int, 2> {
+      std::array<double, 2> result(display->pixel_to_tile({x, y}));
+      return {static_cast<int>(result.at(0)), static_cast<int>(result.at(1))};
+    };
+    std::array<int, 2> cell_xy(to_tile(mouse.x, mouse.y));
+    std::array<int, 2> prev_cell_xy(
+        to_tile(mouse.x - mouse.dx, mouse.y - mouse.dy)
+    );
+    mouse.cx = cell_xy.at(0);
+    mouse.cy = cell_xy.at(1);
+    mouse.dcx = cell_xy.at(0) - prev_cell_xy.at(0);
+    mouse.dcy = cell_xy.at(1) - prev_cell_xy.at(1);
   } else {
     mouse.x -= TCOD_ctx.fullscreen_offsetx;
     mouse.y -= TCOD_ctx.fullscreen_offsety;
     mouse.cx = mouse.x / TCOD_ctx.font_width;
     mouse.cy = mouse.y / TCOD_ctx.font_height;
     int prev_cx = (mouse.x - mouse.dx) / TCOD_ctx.font_width;
     int prev_cy = (mouse.y - mouse.dy) / TCOD_ctx.font_height;
@@ -1304,16 +1313,17 @@
   }
 }
 /**
  *  Parse an SDL_Event into `mouse` and return the relevant TCOD_event_t.
  *
  *  Returns 0 if the event wasn't mouse related.
  */
-static TCOD_event_t TCOD_sys_handle_mouse_event(const SDL_Event *ev,
-                                                TCOD_mouse_t *mouse) {
+TCOD_event_t TCOD_sys_handle_mouse_event(
+    const SDL_Event* ev, TCOD_mouse_t* mouse)
+{
   if (!ev || !mouse) { return TCOD_EVENT_NONE; }
   sdl_parse_mouse_(*ev, *mouse);
   switch(ev->type) {
     case SDL_MOUSEMOTION:
       return TCOD_EVENT_MOUSE_MOVE;
     case SDL_MOUSEWHEEL:
       return TCOD_EVENT_MOUSE_PRESS;
@@ -1346,16 +1356,16 @@
   }
 }
 /**
  *  Parse an SDL_Event into `key` and return the relevant TCOD_event_t.
  *
  *  Returns 0 if the event wasn't keyboard related.
  */
-static TCOD_event_t TCOD_sys_handle_key_event(const SDL_Event *ev,
-                                              TCOD_key_t *key) {
+TCOD_event_t TCOD_sys_handle_key_event(const SDL_Event* ev, TCOD_key_t* key)
+{
   if (!ev || !key) { return TCOD_EVENT_NONE; }
   switch(ev->type) {
     case SDL_KEYDOWN:
       *key = TCOD_sys_SDLtoTCOD(ev, TCOD_KEY_PRESSED);
       return TCOD_EVENT_KEY_PRESS;
     case SDL_KEYUP:
       *key = TCOD_sys_SDLtoTCOD(ev, TCOD_KEY_RELEASED);
@@ -1952,8 +1962,16 @@
  */
 int TCOD_get_tileid_for_charcode_(int charcode) {
   if (charcode >= 0 && charcode < TCOD_ctx.max_font_chars) {
     return TCOD_ctx.ascii_to_tcod[charcode];
   }
   return 0;
 }
+struct SDL_Window* TCOD_sys_get_sdl_window_(void)
+{
+  return window;
+}
+struct SDL_Renderer* TCOD_sys_get_sdl_renderer_(void)
+{
+  return renderer;
+}
 #endif /* TCOD_BARE */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sys_sdl_img_bmp.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sys_sdl_img_bmp.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_BARE
 #include "sys.h"
 
 #include <SDL.h>
 
 #include "libtcod_int.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/sys_sdl_img_png.cpp` & `tcod-9.3.0/libtcod/src/libtcod/sys_sdl_img_png.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef TCOD_BARE
 #include "sys.h"
 
 #if !defined (__HAIKU__) && !defined (__ANDROID__)
 #include <stdlib.h>
 #include <stdio.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/tileset/observer.cpp` & `tcod-9.3.0/libtcod/src/libtcod/tileset/tileset.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,52 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
+#include "tileset.h"
+
+#include <memory>
+#include <string>
+
 #include "observer.h"
+#include "tilesheet.h"
+#include "../libtcod_int.h"
+
 namespace tcod {
 namespace tileset {
+extern "C" {
+Tileset* TCOD_tileset_new(int tile_width, int tile_height) {
+  return new Tileset(tile_width, tile_height);
+}
+void TCOD_tileset_delete(Tileset* tileset) {
+  if (tileset) { delete tileset; }
+}
+} // extern "C"
 } // namespace tileset
 } // namespace tcod
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/tileset/observer.h` & `tcod-9.3.0/libtcod/src/libtcod/tileset/observer.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_TILESET_OBSERVER_H_
 #define LIBTCOD_TILESET_OBSERVER_H_
 #include "../portability.h"
 
 #ifdef __cplusplus
 #include <algorithm>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/tileset/tile.cpp` & `tcod-9.3.0/libtcod/src/libtcod/tree.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,51 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "tile.h"
+#ifndef _TCOD_TREE_H
+#define _TCOD_TREE_H
+
+#include "portability.h"
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+typedef struct _TCOD_tree_t {
+	struct _TCOD_tree_t *next;
+	struct _TCOD_tree_t *father;
+	struct _TCOD_tree_t *sons;
+} TCOD_tree_t;
+
+TCODLIB_API TCOD_tree_t *TCOD_tree_new(void);
+TCODLIB_API void TCOD_tree_add_son(TCOD_tree_t *node, TCOD_tree_t *son);
+#ifdef __cplusplus
+}
+#endif
+#endif
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/tileset/tile.h` & `tcod-9.3.0/libtcod/src/libtcod/tileset/tile.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_TILESET_TILE_H_
 #define LIBTCOD_TILESET_TILE_H_
 #include <stdint.h>
 #ifdef __cplusplus
 #include <algorithm>
 #include <vector>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/tileset/tileset.cpp` & `tcod-9.3.0/libtcod/src/libtcod/pathfinding/generic.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,32 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "tileset.h"
-
-#include <memory>
-#include <string>
-
-#include "observer.h"
-#include "tilesheet.h"
-#include "../libtcod_int.h"
-
-namespace tcod {
-namespace tileset {
-extern "C" {
-Tileset* TCOD_tileset_new(int tile_width, int tile_height) {
-  return new Tileset(tile_width, tile_height);
-}
-void TCOD_tileset_delete(Tileset* tileset) {
-  if (tileset) { delete tileset; }
-}
-} // extern "C"
-} // namespace tileset
-} // namespace tcod
+#include "generic.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/tileset/tileset.h` & `tcod-9.3.0/libtcod/src/libtcod/tileset/tileset.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_TILESET_TILESET_H_
 #define LIBTCOD_TILESET_TILESET_H_
 #ifdef __cplusplus
 #include <algorithm>
 #include <memory>
 #include <utility>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/tileset/tilesheet.cpp` & `tcod-9.3.0/libtcod/src/libtcod/tileset/tilesheet.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "tilesheet.h"
 
 #include "../../vendor/lodepng.h"
 #include "../color/canvas.h"
 namespace tcod {
 namespace tileset {
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/tree.hpp` & `tcod-9.3.0/libtcod/src/libtcod/gui/container.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,48 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#ifndef _TCOD_TREE_HPP
-#define _TCOD_TREE_HPP
-
-#include "tree.h"
-
-class TCODLIB_API TCODTree {
+#ifndef TCOD_GUI_CONTAINER_HPP
+#define TCOD_GUI_CONTAINER_HPP
+#include "widget.hpp"
+class TCODLIB_GUI_API Container : public Widget {
 public :
-	TCODTree *next;
-	TCODTree *father;
-	TCODTree *sons;
-
-	TCODTree() : next(NULL),father(NULL),sons(NULL){}
-	void addSon(TCODTree *data) {
-		data->father=this;
-		TCODTree *lastson = sons;
-		while ( lastson && lastson->next ) lastson=lastson->next;
-		if ( lastson ) {
-			lastson->next=data;
-		} else {
-			sons=data;
-		}
-	}
-
+	Container(int x, int y, int w, int h) : Widget(x,y,w,h) {}
+	virtual ~Container();
+	void addWidget(Widget *wid);
+	void removeWidget(Widget *wid);
+	void setVisible(bool val);
+	void render();
+	void clear();
+	void update(const TCOD_key_t k);
+protected :
+	TCODList<Widget *> content;
 };
-
-#endif
+#endif /* TCOD_GUI_CONTAINER_HPP */
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/tree_c.c` & `tcod-9.3.0/libtcod/src/libtcod.hpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,32 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "tree.h"
-
-#include <stdlib.h>
-
-TCOD_tree_t *TCOD_tree_new(void) {
-	return (TCOD_tree_t *)calloc(1,sizeof(TCOD_tree_t));
-}
-
-void TCOD_tree_add_son(TCOD_tree_t *node, TCOD_tree_t *son) {
-	TCOD_tree_t *lastson = node->sons;
-	son->father=node;
-	while ( lastson && lastson->next ) lastson=lastson->next;
-	if ( lastson ) {
-		lastson->next=son;
-	} else {
-		node->sons=son;
-	}
-}
+#include "libtcod.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/txtfield.cpp` & `tcod-9.3.0/libtcod/src/libtcod/txtfield.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "txtfield.hpp"
 
 #ifdef TCOD_CONSOLE_SUPPORT
 
 TCODText::TCODText(int x, int y, int w, int h, int max_chars){
 	data=TCOD_text_init(x,y,w,h,max_chars);
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/txtfield.h` & `tcod-9.3.0/libtcod/src/libtcod/txtfield.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_TEXT_H_
 #define _TCOD_TEXT_H_
 
 #include "portability.h"
 
 #ifdef TCOD_CONSOLE_SUPPORT
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/txtfield_c.c` & `tcod-9.3.0/libtcod/src/libtcod/txtfield_c.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "txtfield.h"
 
 #ifdef TCOD_CONSOLE_SUPPORT
 
 #include <stdlib.h>
 #include <string.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/utility/vector2.h` & `tcod-9.3.0/libtcod/src/libtcod/utility/vector2.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_UTILITY_VECTOR2_H_
 #define LIBTCOD_UTILITY_VECTOR2_H_
 #ifdef __cplusplus
 #include <algorithm>
 #include <cstddef>
 #include <initializer_list>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/utility.h` & `tcod-9.3.0/libtcod/src/libtcod/utility.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_UTILITY_H
 #define LIBTCOD_UTILITY_H
 /******************************************
  utility macros
  ******************************************/
 #define MAX(a,b) (((a)>(b))?(a):(b))
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/version.h` & `tcod-9.3.0/libtcod/src/libtcod/version.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,46 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef LIBTCOD_VERSION_H
 #define LIBTCOD_VERSION_H
 
 #define TCOD_MAJOR_VERSION  1
-#define TCOD_MINOR_VERSION  10
-#define TCOD_PATCHLEVEL     6
+#define TCOD_MINOR_VERSION  11
+#define TCOD_PATCHLEVEL     0
 
-#define TCOD_STRVERSION "1.10.6"
+#define TCOD_STRVERSION "1.11.0"
 
 #define TCOD_HEXVERSION (0x010000 * TCOD_MAJOR_VERSION \
                          + 0x0100 * TCOD_MINOR_VERSION \
                            + 0x01 * TCOD_PATCHLEVEL)
 #define TCOD_TECHVERSION (TCOD_HEXVERSION * 0x100)
 
 #define TCOD_STRVERSIONNAME "libtcod " TCOD_STRVERSION
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/wrappers.c` & `tcod-9.3.0/libtcod/src/libtcod/wrappers.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "wrappers.h"
 
 #include <math.h>
 #include <string.h>
 
 #include "console.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/wrappers.h` & `tcod-9.3.0/libtcod/src/libtcod/wrappers.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef WRAPPERS_H
 #define WRAPPERS_H
 
 #include "portability.h"
 #include "console_types.h"
 #include "image.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/zip.cpp` & `tcod-9.3.0/libtcod/src/libtcod/zip.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "zip.hpp"
 
 TCODZip::TCODZip() {
 	data=TCOD_zip_new();
 }
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/zip.h` & `tcod-9.3.0/libtcod/src/libtcod/zip.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_ZIP_H
 #define _TCOD_ZIP_H
 
 #include "portability.h"
 #include "color.h"
 #include "console_types.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/zip.hpp` & `tcod-9.3.0/libtcod/src/libtcod/zip.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #ifndef _TCOD_ZIP_HPP
 #define _TCOD_ZIP_HPP
 
 #include "color.hpp"
 #include "console.hpp"
 #include "image.hpp"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod/zip_c.c` & `tcod-9.3.0/libtcod/src/libtcod/zip_c.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 #include "zip.h"
 
 #include <stdlib.h>
 #include <string.h>
 #include <zlib.h>
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod.cpp` & `tcod-9.3.0/libtcod/src/libtcod.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 /** \file libtcod.cpp
  *
  *  To statically link a C++ program with libtcod you'll need to follow
  *  the directions for compiling `libtcod_c.c` and then add `libtcod.cpp` to
  *  your source files.
  */
@@ -64,22 +68,24 @@
 #include "libtcod/console/rexpaint.cpp"
 #include "libtcod/engine/backend.cpp"
 #include "libtcod/engine/display.cpp"
 #include "libtcod/engine/globals.cpp"
 #include "libtcod/pathfinding/astar.cpp"
 #include "libtcod/pathfinding/generic.cpp"
 #include "libtcod/pathfinding/dijkstra.cpp"
+#include "libtcod/sdl2/event.cpp"
 #include "libtcod/sdl2/gl_alias.cpp"
 #include "libtcod/sdl2/gl2_display.cpp"
 #include "libtcod/sdl2/gl2_raii.cpp"
 #include "libtcod/sdl2/gl2_renderer.cpp"
 #include "libtcod/sdl2/legacy_backend.cpp"
 #include "libtcod/sdl2/sdl2_alias.cpp"
 #include "libtcod/sdl2/sdl2_display.cpp"
 #include "libtcod/sdl2/sdl2_renderer.cpp"
+#include "libtcod/tileset/fallback.cpp"
 #include "libtcod/tileset/observer.cpp"
 #include "libtcod/tileset/tile.cpp"
 #include "libtcod/tileset/tileset.cpp"
 #include "libtcod/tileset/tilesheet.cpp"
 #include "libtcod/tileset/truetype.cpp"
 
 #include "libtcod/gui/button.cpp"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod.h` & `tcod-9.3.0/LICENSE.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
- * All rights reserved.
- *
- * Redistribution and use in source and binary forms, with or without
- * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
- */
-#include "libtcod/libtcod.h"
+BSD 2-Clause License
+
+Copyright (c) 2009-2019, Kyle Stewart and the python-tcod contributors.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod.hpp` & `tcod-9.3.0/libtcod/src/libtcod/pathfinding/astar.cpp`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,32 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
-#include "libtcod.h"
+#include "astar.h"
```

### Comparing `tcod-9.2.5/libtcod/src/libtcod_c.c` & `tcod-9.3.0/libtcod/src/libtcod_c.c`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-/* libtcod
- * Copyright © 2008-2019 Jice and the libtcod contributors.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
  * All rights reserved.
  *
  * Redistribution and use in source and binary forms, with or without
  * modification, are permitted provided that the following conditions are met:
- *     * Redistributions of source code must retain the above copyright
- *       notice, this list of conditions and the following disclaimer.
- *     * Redistributions in binary form must reproduce the above copyright
- *       notice, this list of conditions and the following disclaimer in the
- *       documentation and/or other materials provided with the distribution.
- *     * The name of copyright holder nor the names of its contributors may not
- *       be used to endorse or promote products derived from this software
- *       without specific prior written permission.
- *
- * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
- * ``AS IS'' AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
- * TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
- * CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
- * EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
- * PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
- * OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
- * WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
- * OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
- * ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
  */
 /** \file libtcod_c.c
  *
  *  To statically link a C/C++ program with libtcod:
  *
  *  * Add `libtcod_c.c` and `libtcod.cpp` to your list of source files to
  *    compile.
```

### Comparing `tcod-9.2.5/libtcod/src/vendor/glad.c` & `tcod-9.3.0/libtcod/src/vendor/glad.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/glad.h` & `tcod-9.3.0/libtcod/src/vendor/glad.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/khrplatform.h` & `tcod-9.3.0/libtcod/src/vendor/khrplatform.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/lodepng.cpp` & `tcod-9.3.0/libtcod/src/vendor/lodepng.cpp`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/lodepng.h` & `tcod-9.3.0/libtcod/src/vendor/lodepng.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/stb_sprintf.h` & `tcod-9.3.0/libtcod/src/vendor/stb_sprintf.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/stb_truetype.h` & `tcod-9.3.0/libtcod/src/vendor/stb_truetype.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/utf8proc/utf8proc.c` & `tcod-9.3.0/libtcod/src/vendor/utf8proc/utf8proc.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/utf8proc/utf8proc.h` & `tcod-9.3.0/libtcod/src/vendor/utf8proc/utf8proc.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/utf8proc/utf8proc_data.c` & `tcod-9.3.0/libtcod/src/vendor/utf8proc/utf8proc_data.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/adler32.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/adler32.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/compress.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/compress.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/crc32.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/crc32.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/crc32.h` & `tcod-9.3.0/libtcod/src/vendor/zlib/crc32.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/deflate.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/deflate.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/deflate.h` & `tcod-9.3.0/libtcod/src/vendor/zlib/deflate.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/gzclose.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/gzclose.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/gzguts.h` & `tcod-9.3.0/libtcod/src/vendor/zlib/gzguts.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/gzlib.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/gzlib.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/gzread.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/gzread.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/gzwrite.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/gzwrite.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/infback.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/infback.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/inffast.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/inffast.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/inffixed.h` & `tcod-9.3.0/libtcod/src/vendor/zlib/inffixed.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/inflate.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/inflate.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/inflate.h` & `tcod-9.3.0/libtcod/src/vendor/zlib/inflate.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/inftrees.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/inftrees.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/inftrees.h` & `tcod-9.3.0/libtcod/src/vendor/zlib/inftrees.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/trees.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/trees.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/trees.h` & `tcod-9.3.0/libtcod/src/vendor/zlib/trees.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/uncompr.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/uncompr.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/zconf.h` & `tcod-9.3.0/libtcod/src/vendor/zlib/zconf.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/zlib.h` & `tcod-9.3.0/libtcod/src/vendor/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/zutil.c` & `tcod-9.3.0/libtcod/src/vendor/zlib/zutil.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/libtcod/src/vendor/zlib/zutil.h` & `tcod-9.3.0/libtcod/src/vendor/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/LICENSE.txt` & `tcod-9.3.0/libtcod/src/libtcod/tileset/tile.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-BSD 2-Clause License
-
-Copyright (c) 2009-2019, Kyle Stewart and the python-tcod contributors.
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+/* BSD 3-Clause License
+ *
+ * Copyright © 2008-2019, Jice and the libtcod contributors.
+ * All rights reserved.
+ *
+ * Redistribution and use in source and binary forms, with or without
+ * modification, are permitted provided that the following conditions are met:
+ *
+ * 1. Redistributions of source code must retain the above copyright notice,
+ *    this list of conditions and the following disclaimer.
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright notice,
+ *    this list of conditions and the following disclaimer in the documentation
+ *    and/or other materials provided with the distribution.
+ *
+ * 3. Neither the name of the copyright holder nor the names of its
+ *    contributors may be used to endorse or promote products derived from
+ *    this software without specific prior written permission.
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+ * AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
+ * LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
+ * CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
+ * SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+ * INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+ * CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+ * POSSIBILITY OF SUCH DAMAGE.
+ */
+#include "tile.h"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tcod-9.2.5/PKG-INFO` & `tcod-9.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tcod
-Version: 9.2.5
+Version: 9.3.0
 Summary: Pythonic cffi port of libtcod.
 Home-page: https://github.com/libtcod/python-tcod
 Author: Kyle Stewart
 Author-email: 4B796C65+tdl@gmail.com
 License: Simplified BSD License
 Description: .. contents::
            :backlinks: top
@@ -36,43 +36,26 @@
         If you had code that runs on libtcodpy then you can use this library as a
         drop-in replacement.  This installs a libtcodpy module so you'll only need to
         delete the libtcodpy/ folder that's usually bundled in an older libtcodpy
         project.
         
         Guides and Tutorials for libtcodpy should work with the tcod module.
         
-        The latest documentation can be found
-        `here <https://python-tcod.readthedocs.io/en/latest/>`_.
+        The latest documentation can be found here:
+        https://python-tcod.readthedocs.io/en/latest/
         
         ==============
          Installation
         ==============
-        The recommended way to install is by using pip.  Older versions of pip will
-        have issues installing tcod, so make sure it's up-to-date.
+        Detailed installation instructions are here:
+        https://python-tcod.readthedocs.io/en/latest/installation.html
         
-        Windows / MacOS
-        ---------------
-        To install using pip, use the following command::
-        
-            > python -m pip install tcod
-        
-        If you get the error "ImportError: DLL load failed: The specified module could
-        not be found." when trying to import tcod/tdl then you may need the latest
-        `Microsoft Visual C runtime
-        <https://support.microsoft.com/en-ca/help/2977003/the-latest-supported-visual-c-downloads>`_.
-        
-        Linux
-        -----
-        On Linux python-tcod will need to be built from source.
-        Assuming you have Python, pip, and apt-get, then you'll run these commands to
-        install python-tcod and its dependencies to your user environment::
-        
-            $ sudo apt-get install gcc python-dev python3-dev libsdl2-dev libffi-dev libomp5
-            $ pip2 install tcod
-            $ pip3 install tcod
+        For the most part it's just::
+        
+            pip3 install tcod
         
         ==============
          Requirements
         ==============
         * Python 3.5+
         * Windows, Linux, or MacOS X 10.9+.
         * On Windows, requires the Visual C++ runtime 2015 or later.
@@ -137,21 +120,45 @@
         .. |Pyup| image:: https://pyup.io/repos/github/libtcod/python-tcod/shield.svg
             :target: https://pyup.io/repos/github/libtcod/python-tcod/
             :alt: Updates
         
         ===========
          Changelog
         ===========
-        Changes relevant for users of the the tdl and tcod packages are documented
-        here.
+        Changes relevant to the users of python-tcod are documented here.
         
         This project adheres to `Semantic Versioning <https://semver.org/>`_ since
         v2.0.0
         
         
+        9.3.0 - 2019-03-15
+        ------------------
+        Added
+         - The SDL2/OPENGL2 renderers can potentially use a fall-back font when none
+           are provided.
+         - New function `tcod.event.get_mouse_state`.
+         - New function `tcod.map.compute_fov` lets you get a visibility array directly
+           from a transparency array.
+        Deprecated
+         - The following functions and classes have been deprecated.
+           - `tcod.Key`
+           - `tcod.Mouse`
+           - `tcod.mouse_get_status`
+           - `tcod.console_is_window_closed`
+           - `tcod.console_check_for_keypress`
+           - `tcod.console_wait_for_keypress`
+           - `tcod.console_delete`
+           - `tcod.sys_check_for_event`
+           - `tcod.sys_wait_for_event`
+         - The SDL, OPENGL, and GLSL renderers have been deprecated.
+         - Many libtcodpy functions have been marked with PendingDeprecationWarning's.
+        Fixed
+         - To be more compatible with libtcodpy `tcod.console_init_root` will default
+           to the SDL render, but will raise warnings when an old renderer is used.
+        
         9.2.5 - 2019-03-04
         ------------------
         Fixed
          - Fixed `tcod.namegen_generate_custom`.
         
         9.2.4 - 2019-03-02
         ------------------
@@ -165,50 +172,50 @@
            the future.
          - Methods and functionality preventing `tcod.Color` from behaving like a tuple
            have been deprecated.
         
         9.2.2 - 2019-02-26
         ------------------
         Fixed
-        - `Console.print_box` wasn't setting the background color by default.
+         - `Console.print_box` wasn't setting the background color by default.
         
         9.2.1 - 2019-02-25
         ------------------
         Fixed
-        - `tcod.sys_get_char_size` fixed on the new renderers.
+         - `tcod.sys_get_char_size` fixed on the new renderers.
         
         9.2.0 - 2019-02-24
         ------------------
         Added
-        - New `tcod.console.get_height_rect` function, which can be used to get the
-          height of a print call without an existing console.
-        - New `tcod.tileset` module, with a `set_truetype_font` function.
-        Fixed
-        - The new print methods now handle alignment according to how they were
-          documented.
-        - `SDL2` and `OPENGL2` now support screenshots.
-        - Windows and MacOS builds now restrict exported SDL2 symbols to only
-          SDL 2.0.5;  This will avoid hard to debug import errors when the wrong
-          version of SDL is dynamically linked.
-        - The root console now starts with a white foreground.
+         - New `tcod.console.get_height_rect` function, which can be used to get the
+           height of a print call without an existing console.
+         - New `tcod.tileset` module, with a `set_truetype_font` function.
+        Fixed
+         - The new print methods now handle alignment according to how they were
+           documented.
+         - `SDL2` and `OPENGL2` now support screenshots.
+         - Windows and MacOS builds now restrict exported SDL2 symbols to only
+           SDL 2.0.5;  This will avoid hard to debug import errors when the wrong
+           version of SDL is dynamically linked.
+         - The root console now starts with a white foreground.
         
         9.1.0 - 2019-02-23
         ------------------
         Added
-        - Added the `tcod.random.MULTIPLY_WITH_CARRY` constant.
+         - Added the `tcod.random.MULTIPLY_WITH_CARRY` constant.
         Changed
-        - The overhead for warnings has been reduced when running Python with the
-          optimize `-O` flag.
-        - `tcod.random.Random` now provides a default algorithm.
+         - The overhead for warnings has been reduced when running Python with the
+           optimize `-O` flag.
+         - `tcod.random.Random` now provides a default algorithm.
         
         9.0.0 - 2019-02-17
         ------------------
         Changed
-        - New console methods now default to an `fg` and `bg` of None instead of
-          white-on-black.
+         - New console methods now default to an `fg` and `bg` of None instead of
+           white-on-black.
         
         8.5.0 - 2019-02-15
         ------------------
         Added
          - `tcod.console.Console` now supports `str` and `repr`.
          - Added new Console methods which are independent from the console defaults.
          - You can now give an array when initializing a `tcod.console.Console`
```

### Comparing `tcod-9.2.5/README.rst` & `tcod-9.3.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -28,43 +28,26 @@
 If you had code that runs on libtcodpy then you can use this library as a
 drop-in replacement.  This installs a libtcodpy module so you'll only need to
 delete the libtcodpy/ folder that's usually bundled in an older libtcodpy
 project.
 
 Guides and Tutorials for libtcodpy should work with the tcod module.
 
-The latest documentation can be found
-`here <https://python-tcod.readthedocs.io/en/latest/>`_.
+The latest documentation can be found here:
+https://python-tcod.readthedocs.io/en/latest/
 
 ==============
  Installation
 ==============
-The recommended way to install is by using pip.  Older versions of pip will
-have issues installing tcod, so make sure it's up-to-date.
+Detailed installation instructions are here:
+https://python-tcod.readthedocs.io/en/latest/installation.html
 
-Windows / MacOS
----------------
-To install using pip, use the following command::
-
-    > python -m pip install tcod
-
-If you get the error "ImportError: DLL load failed: The specified module could
-not be found." when trying to import tcod/tdl then you may need the latest
-`Microsoft Visual C runtime
-<https://support.microsoft.com/en-ca/help/2977003/the-latest-supported-visual-c-downloads>`_.
-
-Linux
------
-On Linux python-tcod will need to be built from source.
-Assuming you have Python, pip, and apt-get, then you'll run these commands to
-install python-tcod and its dependencies to your user environment::
-
-    $ sudo apt-get install gcc python-dev python3-dev libsdl2-dev libffi-dev libomp5
-    $ pip2 install tcod
-    $ pip3 install tcod
+For the most part it's just::
+
+    pip3 install tcod
 
 ==============
  Requirements
 ==============
 * Python 3.5+
 * Windows, Linux, or MacOS X 10.9+.
 * On Windows, requires the Visual C++ runtime 2015 or later.
```

### Comparing `tcod-9.2.5/setup.py` & `tcod-9.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -83,16 +83,19 @@
         changelog = f.read()
         changelog = changelog.replace("\nUnreleased\n------------------", "")
     return "\n".join([readme, changelog])
 
 
 if sys.version_info < (3, 5):
     error = """
-    python-tcod supports Python 3.5 and above.
-    The last version supporting Python 2.7/3.4 was 'tcod==6.0.7'
+    This version of python-tcod only supports Python 3.5 and above.
+    The last version supporting Python 2.7/3.4 was 'tcod==6.0.7'.
+
+    The end-of-life for Python 2 is the year 2020.
+    https://pythonclock.org/
 
     Python {py} detected.
     """.format(
         py=".".join([str(v) for v in sys.version_info[:3]])
     )
 
     print(error)
```

### Comparing `tcod-9.2.5/tcod/bsp.py` & `tcod-9.3.0/tcod/bsp.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/cdef.h` & `tcod-9.3.0/tcod/cdef.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/cffi.h` & `tcod-9.3.0/tcod/cffi.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/color.py` & `tcod-9.3.0/tcod/color.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/console.py` & `tcod-9.3.0/tcod/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
                 |xxxxxxxxxxxxxxxxxxxx|
                 |                    >
 
             .. versionadded:: 8.5
     """
 
     DTYPE = [("ch", np.intc), ("fg", "(3,)u1"), ("bg", "(3,)u1")]  # type: Any
+    _DTYPE_RGB = np.dtype("(3,)u1")  # type: Any
 
     def __init__(
         self,
         width: int,
         height: int,
         order: str = "C",
         buffer: Optional[np.array] = None,
@@ -106,16 +107,16 @@
             if self._order == "F":
                 buffer = buffer.transpose()
             self._ch = np.ascontiguousarray(buffer["ch"], np.intc)
             self._fg = np.ascontiguousarray(buffer["fg"], "u1")
             self._bg = np.ascontiguousarray(buffer["bg"], "u1")
         else:
             self._ch = np.ndarray((height, width), dtype=np.intc)
-            self._fg = np.ndarray((height, width), dtype="(3,)u1")
-            self._bg = np.ndarray((height, width), dtype="(3,)u1")
+            self._fg = np.ndarray((height, width), dtype=self._DTYPE_RGB)
+            self._bg = np.ndarray((height, width), dtype=self._DTYPE_RGB)
 
         # libtcod uses the root console for defaults.
         default_bg_blend = 0
         default_alignment = 0
         if lib.TCOD_ctx.root != ffi.NULL:
             default_bg_blend = lib.TCOD_ctx.root.bkgnd_flag
             default_alignment = lib.TCOD_ctx.root.alignment
```

### Comparing `tcod-9.2.5/tcod/constants.py` & `tcod-9.3.0/tcod/constants.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/event.py` & `tcod-9.3.0/tcod/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,54 @@
     pass
 
 
 class KeyUp(KeyboardEvent):
     pass
 
 
-class MouseMotion(Event):
+class MouseState(Event):
+    """
+    Attributes:
+        type (str): Always "MOUSESTATE".
+        pixel (Point): The pixel coordinates of the mouse.
+        tile (Point): The integer tile coordinates of the mouse on the screen.
+        state (int): A bitmask of which mouse buttons are currently held.
+
+            Will be a combination of the following names:
+
+            * tcod.event.BUTTON_LMASK
+            * tcod.event.BUTTON_MMASK
+            * tcod.event.BUTTON_RMASK
+            * tcod.event.BUTTON_X1MASK
+            * tcod.event.BUTTON_X2MASK
+
+    .. addedversion:: 9.3
+    """
+
+    def __init__(
+        self,
+        pixel: Tuple[int, int] = (0, 0),
+        tile: Tuple[int, int] = (0, 0),
+        state: int = 0,
+    ):
+        super().__init__()
+        self.pixel = Point(*pixel)
+        self.tile = Point(*tile)
+        self.state = state
+
+    def __repr__(self) -> str:
+        return ("tcod.event.%s(pixel=%r, tile=%r, state=%s)") % (
+            self.__class__.__name__,
+            self.pixel,
+            self.tile,
+            _describe_bitmask(self.state, _REVERSE_BUTTON_MASK_TABLE),
+        )
+
+
+class MouseMotion(MouseState):
     """
     Attributes:
         type (str): Always "MOUSEMOTION".
         pixel (Point): The pixel coordinates of the mouse.
         pixel_motion (Point): The pixel delta.
         tile (Point): The integer tile coordinates of the mouse on the screen.
         tile_motion (Point): The integer tile delta.
@@ -204,20 +243,17 @@
         self,
         pixel: Tuple[int, int] = (0, 0),
         pixel_motion: Tuple[int, int] = (0, 0),
         tile: Tuple[int, int] = (0, 0),
         tile_motion: Tuple[int, int] = (0, 0),
         state: int = 0,
     ):
-        super().__init__()
-        self.pixel = Point(*pixel)
+        super().__init__(pixel, tile, state)
         self.pixel_motion = Point(*pixel_motion)
-        self.tile = Point(*tile)
         self.tile_motion = Point(*tile_motion)
-        self.state = state
 
     @classmethod
     def from_sdl_event(cls, sdl_event: Any) -> "MouseMotion":
         motion = sdl_event.motion
 
         pixel = motion.x, motion.y
         pixel_motion = motion.xrel, motion.yrel
@@ -241,15 +277,15 @@
             self.pixel_motion,
             self.tile,
             self.tile_motion,
             _describe_bitmask(self.state, _REVERSE_BUTTON_MASK_TABLE),
         )
 
 
-class MouseButtonEvent(Event):
+class MouseButtonEvent(MouseState):
     """
     Attributes:
         type (str): Will be "MOUSEBUTTONDOWN" or "MOUSEBUTTONUP",
                     depending on the event.
         pixel (Point): The pixel coordinates of the mouse.
         tile (Point): The integer tile coordinates of the mouse on the screen.
         button (int): Which mouse button.
@@ -265,18 +301,23 @@
 
     def __init__(
         self,
         pixel: Tuple[int, int] = (0, 0),
         tile: Tuple[int, int] = (0, 0),
         button: int = 0,
     ):
-        super().__init__()
-        self.pixel = Point(*pixel)
-        self.tile = Point(*tile)
-        self.button = button
+        super().__init__(pixel, tile, button)
+
+    @property
+    def button(self) -> int:
+        return self.state
+
+    @button.setter
+    def button(self, value: int) -> None:
+        self.state = value
 
     @classmethod
     def from_sdl_event(cls, sdl_event: Any) -> Any:
         button = sdl_event.button
         pixel = button.x, button.y
         subtile = _pixel_to_tile(*pixel)
         tile = int(subtile[0]), int(subtile[1])
@@ -290,30 +331,31 @@
             self.pixel,
             self.tile,
             _REVERSE_BUTTON_TABLE[self.button],
         )
 
 
 class MouseButtonDown(MouseButtonEvent):
-    pass
+    """Same as MouseButtonEvent but with ``type="MouseButtonDown"``."""
 
 
 class MouseButtonUp(MouseButtonEvent):
-    pass
+    """Same as MouseButtonEvent but with ``type="MouseButtonUp"``."""
 
 
 class MouseWheel(Event):
     """
     Attributes:
         type (str): Always "MOUSEWHEEL".
         x (int): Horizontal scrolling. A positive value means scrolling right.
         y (int): Vertical scrolling. A positive value means scrolling away from
                  the user.
         flipped (bool): If True then the values of `x` and `y` are the opposite
-                        of their usual values.
+                        of their usual values.  This depends on the settings of
+                        the Operating System.
     """
 
     def __init__(self, x: int, y: int, flipped: bool = False):
         super().__init__()
         self.x = x
         self.y = y
         self.flipped = flipped
@@ -662,14 +704,25 @@
     def ev_windowtakefocus(self, event: WindowEvent) -> None:
         pass
 
     def ev_windowhittest(self, event: WindowEvent) -> None:
         pass
 
 
+def get_mouse_state() -> MouseState:
+    """Return the current state of the mouse.
+
+    .. addedversion:: 9.3
+    """
+    xy = tcod.ffi.new("int[2]")
+    buttons = tcod.lib.SDL_GetMouseState(xy, xy + 1)
+    x, y = _pixel_to_tile(*xy)
+    return MouseState((xy[0], xy[1]), (int(x), int(y)), buttons)
+
+
 __all__ = [
     "Point",
     "BUTTON_LEFT",
     "BUTTON_MIDDLE",
     "BUTTON_RIGHT",
     "BUTTON_X1",
     "BUTTON_X2",
```

### Comparing `tcod-9.2.5/tcod/event_constants.py` & `tcod-9.3.0/tcod/event_constants.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/image.py` & `tcod-9.3.0/tcod/image.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/libtcodpy.py` & `tcod-9.3.0/tcod/libtcodpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     FONT_LAYOUT_ASCII_INCOL,
     FOV_RESTRICTIVE,
     FOV_PERMISSIVE_0,
     NOISE_DEFAULT,
     KEY_RELEASED,
 )
 
-from tcod._internal import deprecate
+from tcod._internal import deprecate, pending_deprecate
 
 from tcod.tcod import _int, _unpack_char_p
 from tcod.tcod import _bytes, _unicode, _fmt
 from tcod.tcod import _CDataWrapper
 from tcod.tcod import _PropagateException
 from tcod.tcod import _console
 
@@ -356,14 +356,17 @@
         lalt (bool): True when left alt is held.
         lctrl (bool): True when left control is held.
         lmeta (bool): True when left meta key is held.
         ralt (bool): True when right alt is held.
         rctrl (bool): True when right control is held.
         rmeta (bool): True when right meta key is held.
         shift (bool): True when any shift is held.
+
+    .. deprecated:: 9.3
+        Use events from the :any:`tcod.event` module instead.
     """
 
     _BOOL_ATTRIBUTES = (
         "lalt",
         "lctrl",
         "lmeta",
         "ralt",
@@ -464,14 +467,17 @@
         rbutton (bool): Right button status.
         mbutton (bool): Middle button status.
         lbutton_pressed (bool): Left button pressed event.
         rbutton_pressed (bool): Right button pressed event.
         mbutton_pressed (bool): Middle button pressed event.
         wheel_up (bool): Wheel up event.
         wheel_down (bool): Wheel down event.
+
+    .. deprecated:: 9.3
+        Use events from the :any:`tcod.event` module instead.
     """
 
     def __init__(
         self,
         x: int = 0,
         y: int = 0,
         dx: int = 0,
@@ -748,14 +754,15 @@
     This function exists for backwards compatibility.
 
     .. deprecated:: 2.0
        BSP deletion is automatic.
     """
 
 
+@pending_deprecate()
 def color_lerp(
     c1: Tuple[int, int, int], c2: Tuple[int, int, int], a: float
 ) -> Color:
     """Return the linear interpolation between two colors.
 
     ``a`` is the interpolation value, with 0 returing ``c1``,
     1 returning ``c2``, and 0.5 returing a color halfway between both.
@@ -769,14 +776,15 @@
 
     Returns:
         Color: The interpolated Color.
     """
     return Color._new_from_cdata(lib.TCOD_color_lerp(c1, c2, a))
 
 
+@pending_deprecate()
 def color_set_hsv(c: Color, h: float, s: float, v: float) -> None:
     """Set a color using: hue, saturation, and value parameters.
 
     Does not return a new Color.  ``c`` is modified inplace.
 
     Args:
         c (Union[Color, List[Any]]): A Color instance, or a list of any kind.
@@ -785,14 +793,15 @@
         v (float): Value, from 0 to 1.
     """
     new_color = ffi.new("TCOD_color_t*")
     lib.TCOD_color_set_HSV(new_color, h, s, v)
     c[:] = new_color.r, new_color.g, new_color.b
 
 
+@pending_deprecate()
 def color_get_hsv(c: Tuple[int, int, int]) -> Tuple[float, float, float]:
     """Return the (hue, saturation, value) of a color.
 
     Args:
         c (Union[Tuple[int, int, int], Sequence[int]]):
             An (r, g, b) sequence or Color instance.
 
@@ -801,14 +810,15 @@
             A tuple with (hue, saturation, value) values, from 0 to 1.
     """
     hsv = ffi.new("float [3]")
     lib.TCOD_color_get_HSV(c, hsv, hsv + 1, hsv + 2)
     return hsv[0], hsv[1], hsv[2]
 
 
+@pending_deprecate()
 def color_scale_HSV(c: Color, scoef: float, vcoef: float) -> None:
     """Scale a color's saturation and value.
 
     Does not return a new Color.  ``c`` is modified inplace.
 
     Args:
         c (Union[Color, List[int]]): A Color instance, or an [r, g, b] list.
@@ -819,14 +829,15 @@
     """
     color_p = ffi.new("TCOD_color_t*")
     color_p.r, color_p.g, color_p.b = c.r, c.g, c.b
     lib.TCOD_color_scale_HSV(color_p, scoef, vcoef)
     c[:] = color_p.r, color_p.g, color_p.b
 
 
+@pending_deprecate()
 def color_gen_map(
     colors: Iterable[Tuple[int, int, int]], indexes: Iterable[int]
 ) -> List[Color]:
     """Return a smoothly defined scale of colors.
 
     If ``indexes`` is [0, 3, 9] for example, the first color from ``colors``
     will be returned at 0, the 2nd will be at 3, and the 3rd will be at 9.
@@ -863,24 +874,33 @@
     """Set up the primary display and return the root console.
 
     `w` and `h` are the columns and rows of the new window (in tiles.)
 
     `title` is an optional string to display on the windows title bar.
 
     `fullscreen` determines if the window will start in fullscreen.  Fullscreen
-    mode is unreliable unless the renderer is set to `RENDERER_SDL2` or
-    `RENDERER_OPENGL2`.
+    mode is unreliable unless the renderer is set to `tcod.RENDERER_SDL2` or
+    `tcod.RENDERER_OPENGL2`.
 
-    `renderer` is the rendering back-end that libtcod will use.  Options are:
-
-    * `tcod.RENDERER_SDL`
-    * `tcod.RENDERER_OPENGL`
-    * `tcod.RENDERER_GLSL`
-    * `tcod.RENDERER_SDL2`
-    * `tcod.RENDERER_OPENGL2`
+    `renderer` is the rendering back-end that libtcod will use.
+    If you don't know which to pick, then use `tcod.RENDERER_SDL2`.
+    Options are:
+
+    * `tcod.RENDERER_SDL`:
+      A deprecated software/SDL2 renderer.
+    * `tcod.RENDERER_OPENGL`:
+      A deprecated SDL2/OpenGL1 renderer.
+    * `tcod.RENDERER_GLSL`:
+      A deprecated SDL2/OpenGL2 renderer.
+    * `tcod.RENDERER_SDL2`:
+      The recommended SDL2 renderer.  Rendering is decided by SDL2 and can be
+      changed by using an SDL2 hint.
+    * `tcod.RENDERER_OPENGL2`:
+      An SDL2/OPENGL2 renderer.  Usually faster than regular SDL2.
+      Requires OpenGL 2.0 Core.
 
     `order` will affect how the array attributes of the returned root console
     are indexed.  `order='C'` is the default, but `order='F'` is recommended.
 
     .. versionchanged:: 4.3
         Added `order` parameter.
         `title` parameter is now optional.
@@ -889,15 +909,30 @@
         The default `renderer` is now automatic instead of always being
         `RENDERER_SDL`.
     """
     if title is None:
         # Use the scripts filename as the title.
         title = os.path.basename(sys.argv[0])
     if renderer is None:
-        renderer = tcod.constants.RENDERER_SDL2
+        warnings.warn(
+            "A renderer should be given, see the online documentation.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+        renderer = tcod.constants.RENDERER_SDL
+    elif renderer in (
+        tcod.constants.RENDERER_SDL,
+        tcod.constants.RENDERER_OPENGL,
+        tcod.constants.RENDERER_GLSL,
+    ):
+        warnings.warn(
+            "The SDL, OPENGL, and GLSL renderers are deprecated.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
     lib.TCOD_console_init_root(w, h, _bytes(title), fullscreen, renderer)
     console = tcod.console.Console._get_root(order)
     console.clear()
     return console
 
 
 def console_set_custom_font(
@@ -964,14 +999,15 @@
 
     .. deprecated:: 2.0
         Use `Console.height` instead.
     """
     return int(lib.TCOD_console_get_height(_console(con)))
 
 
+@pending_deprecate()
 def console_map_ascii_code_to_font(
     asciiCode: int, fontCharX: int, fontCharY: int
 ) -> None:
     """Set a character code to new coordinates on the tile-set.
 
     `asciiCode` must be within the bounds created during the initialization of
     the loaded tile-set.  For example, you can't use 255 here unless you have a
@@ -985,14 +1021,15 @@
                          0 is the topmost tile.
     """
     lib.TCOD_console_map_ascii_code_to_font(
         _int(asciiCode), fontCharX, fontCharY
     )
 
 
+@pending_deprecate()
 def console_map_ascii_codes_to_font(
     firstAsciiCode: int, nbCodes: int, fontCharX: int, fontCharY: int
 ) -> None:
     """Remap a contiguous set of codes to a contiguous set of tiles.
 
     Both the tile-set and character codes must be contiguous to use this
     function.  If this is not the case you may want to use
@@ -1008,14 +1045,15 @@
 
     """
     lib.TCOD_console_map_ascii_codes_to_font(
         _int(firstAsciiCode), nbCodes, fontCharX, fontCharY
     )
 
 
+@pending_deprecate()
 def console_map_string_to_font(s: str, fontCharX: int, fontCharY: int) -> None:
     """Remap a string of codes to a contiguous set of tiles.
 
     Args:
         s (AnyStr): A string of character codes to map to new values.
                     The null character `'\\x00'` will prematurely end this
                     function.
@@ -1042,38 +1080,46 @@
     Args:
         fullscreen (bool): Use True to change to fullscreen.
                            Use False to change to windowed.
     """
     lib.TCOD_console_set_fullscreen(fullscreen)
 
 
+@deprecate('Use the tcod.event module to check for "QUIT" type events.')
 def console_is_window_closed() -> bool:
-    """Returns True if the window has received and exit event."""
+    """Returns True if the window has received and exit event.
+
+    .. deprecated:: 9.3
+        Use the :any:`tcod.event` module to check for "QUIT" type events.
+    """
     return bool(lib.TCOD_console_is_window_closed())
 
 
+@pending_deprecate()
 def console_has_mouse_focus() -> bool:
     """Return True if the window has mouse focus."""
     return bool(lib.TCOD_console_has_mouse_focus())
 
 
+@pending_deprecate()
 def console_is_active() -> bool:
     """Return True if the window has keyboard focus."""
     return bool(lib.TCOD_console_is_active())
 
 
 def console_set_window_title(title: str) -> None:
     """Change the current title bar string.
 
     Args:
         title (AnyStr): A string to change the title bar to.
     """
     lib.TCOD_console_set_window_title(_bytes(title))
 
 
+@pending_deprecate()
 def console_credits() -> None:
     lib.TCOD_console_credits()
 
 
 def console_credits_reset() -> None:
     lib.TCOD_console_credits_reset()
 
@@ -1135,14 +1181,15 @@
 
     .. deprecated:: 8.5
         Call the :any:`Console.clear` method instead.
     """
     lib.TCOD_console_clear(_console(con))
 
 
+@pending_deprecate()
 def console_put_char(
     con: tcod.console.Console,
     x: int,
     y: int,
     c: Union[int, str],
     flag: int = BKGND_DEFAULT,
 ) -> None:
@@ -1154,14 +1201,15 @@
         y (int): Character y position from the top.
         c (Union[int, AnyStr]): Character to draw, can be an integer or string.
         flag (int): Blending mode to use, defaults to BKGND_DEFAULT.
     """
     lib.TCOD_console_put_char(_console(con), x, y, _int(c), flag)
 
 
+@pending_deprecate()
 def console_put_char_ex(
     con: tcod.console.Console,
     x: int,
     y: int,
     c: Union[int, str],
     fore: Tuple[int, int, int],
     back: Tuple[int, int, int],
@@ -1177,14 +1225,15 @@
             An (r, g, b) sequence or Color instance.
         back (Union[Tuple[int, int, int], Sequence[int]]):
             An (r, g, b) sequence or Color instance.
     """
     lib.TCOD_console_put_char_ex(_console(con), x, y, _int(c), fore, back)
 
 
+@pending_deprecate()
 def console_set_char_background(
     con: tcod.console.Console,
     x: int,
     y: int,
     col: Tuple[int, int, int],
     flag: int = BKGND_SET,
 ) -> None:
@@ -1485,14 +1534,15 @@
     .. deprecated:: 8.5
         Use :any:`Console.print_frame` instead.
     """
     fmt = _fmt(fmt) if fmt else ffi.NULL
     lib.TCOD_console_printf_frame(_console(con), x, y, w, h, clear, flag, fmt)
 
 
+@pending_deprecate()
 def console_set_color_control(
     con: int, fore: Tuple[int, int, int], back: Tuple[int, int, int]
 ) -> None:
     """Configure :any:`color controls`.
 
     Args:
         con (int): :any:`Color control` constant to modify.
@@ -1565,48 +1615,61 @@
     .. deprecated:: 8.4
         Array access performs significantly faster than using this function.
         See :any:`Console.ch`.
     """
     return lib.TCOD_console_get_char(_console(con), x, y)  # type: ignore
 
 
+@pending_deprecate()
 def console_set_fade(fade: int, fadingColor: Tuple[int, int, int]) -> None:
     lib.TCOD_console_set_fade(fade, fadingColor)
 
 
+@pending_deprecate()
 def console_get_fade() -> int:
     return int(lib.TCOD_console_get_fade())
 
 
+@pending_deprecate()
 def console_get_fading_color() -> Color:
     return Color._new_from_cdata(lib.TCOD_console_get_fading_color())
 
 
 # handling keyboard input
+@deprecate("Use the tcod.event.wait function to wait for events.")
 def console_wait_for_keypress(flush: bool) -> Key:
     """Block until the user presses a key, then returns a new Key.
 
     Args:
         flush bool: If True then the event queue is cleared before waiting
                     for the next event.
 
     Returns:
         Key: A new Key instance.
+
+    .. deprecated:: 9.3
+        Use the :any:`tcod.event.wait` function to wait for events.
     """
     key = Key()
     lib.TCOD_console_wait_for_keypress_wrapper(key.key_p, flush)
     return key
 
 
+@deprecate("Use the tcod.event.get function to check for events.")
 def console_check_for_keypress(flags: int = KEY_RELEASED) -> Key:
+    """
+    .. deprecated:: 9.3
+        Use the :any:`tcod.event.get` function to check for events.
+    """
     key = Key()
     lib.TCOD_console_check_for_keypress_wrapper(key.key_p, flags)
     return key
 
 
+@pending_deprecate()
 def console_is_key_pressed(key: int) -> bool:
     return bool(lib.TCOD_console_is_key_pressed(key))
 
 
 # using offscreen consoles
 @deprecate("Create a console using `tcod.console.Console(...)` instead.")
 def console_new(w: int, h: int) -> tcod.console.Console:
@@ -1678,18 +1741,38 @@
 def console_delete(con: tcod.console.Console) -> None:
     """Closes the window if `con` is the root console.
 
     libtcod objects are automatically garbage collected once they go out of
     scope.
 
     This function exists for backwards compatibility.
+
+    .. deprecated:: 9.3
+        This function is not needed for normal :any:`tcod.console.Console`'s.
+        The root console should be used in a with statement instead to ensure
+        that it closes.
     """
     con = _console(con)
     if con == ffi.NULL:
         lib.TCOD_console_delete(con)
+        warnings.warn(
+            "Instead of this call you should use a with statement to ensure"
+            " the root console closes, for example:"
+            "\n    with tcod.console_init_root(...) as root_console:"
+            "\n        ...",
+            DeprecationWarning,
+            stacklevel=2,
+        )
+    else:
+        warnings.warn(
+            "You no longer need to make this call, "
+            "Console's are deleted when they go out of scope.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
 
 
 @deprecate("Assign to the console.fg array instead.")
 def console_fill_foreground(
     con: tcod.console.Console,
     r: Sequence[int],
     g: Sequence[int],
@@ -1787,35 +1870,39 @@
     else:
         # otherwise convert using the ffi module
         carr = ffi.new("int[]", arr)
 
     lib.TCOD_console_fill_char(_console(con), carr)
 
 
+@pending_deprecate()
 def console_load_asc(con: tcod.console.Console, filename: str) -> bool:
     """Update a console from a non-delimited ASCII `.asc` file."""
     return bool(
         lib.TCOD_console_load_asc(_console(con), filename.encode("utf-8"))
     )
 
 
+@pending_deprecate()
 def console_save_asc(con: tcod.console.Console, filename: str) -> bool:
     """Save a console to a non-delimited ASCII `.asc` file."""
     return bool(
         lib.TCOD_console_save_asc(_console(con), filename.encode("utf-8"))
     )
 
 
+@pending_deprecate()
 def console_load_apf(con: tcod.console.Console, filename: str) -> bool:
     """Update a console from an ASCII Paint `.apf` file."""
     return bool(
         lib.TCOD_console_load_apf(_console(con), filename.encode("utf-8"))
     )
 
 
+@pending_deprecate()
 def console_save_apf(con: tcod.console.Console, filename: str) -> bool:
     """Save a console to an ASCII Paint `.apf` file."""
     return bool(
         lib.TCOD_console_save_apf(_console(con), filename.encode("utf-8"))
     )
 
 
@@ -1878,14 +1965,15 @@
                 tcod_list, filename.encode("utf-8"), compress_level
             )
         )
     finally:
         lib.TCOD_list_delete(tcod_list)
 
 
+@pending_deprecate()
 def path_new_using_map(
     m: tcod.map.Map, dcost: float = 1.41
 ) -> tcod.path.AStar:
     """Return a new AStar using the given Map.
 
     Args:
         m (Map): A Map instance.
@@ -1893,14 +1981,15 @@
                        Can be set to 0 to disable diagonal movement.
     Returns:
         AStar: A new AStar instance.
     """
     return tcod.path.AStar(m, dcost)
 
 
+@pending_deprecate()
 def path_new_using_function(
     w: int,
     h: int,
     func: Callable[[int, int, int, int, Any], float],
     userData: Any = 0,
     dcost: float = 1.41,
 ) -> tcod.path.AStar:
@@ -1917,14 +2006,15 @@
         AStar: A new AStar instance.
     """
     return tcod.path.AStar(
         tcod.path._EdgeCostFunc((func, userData), (w, h)), dcost
     )
 
 
+@pending_deprecate()
 def path_compute(
     p: tcod.path.AStar, ox: int, oy: int, dx: int, dy: int
 ) -> bool:
     """Find a path from (ox, oy) to (dx, dy).  Return True if path is found.
 
     Args:
         p (AStar): An AStar instance.
@@ -1934,14 +2024,15 @@
         dy (int): Destination y position.
     Returns:
         bool: True if a valid path was found.  Otherwise False.
     """
     return bool(lib.TCOD_path_compute(p._path_c, ox, oy, dx, dy))
 
 
+@pending_deprecate()
 def path_get_origin(p: tcod.path.AStar) -> Tuple[int, int]:
     """Get the current origin position.
 
     This point moves when :any:`path_walk` returns the next x,y step.
 
     Args:
         p (AStar): An AStar instance.
@@ -1950,74 +2041,80 @@
     """
     x = ffi.new("int *")
     y = ffi.new("int *")
     lib.TCOD_path_get_origin(p._path_c, x, y)
     return x[0], y[0]
 
 
+@pending_deprecate()
 def path_get_destination(p: tcod.path.AStar) -> Tuple[int, int]:
     """Get the current destination position.
 
     Args:
         p (AStar): An AStar instance.
     Returns:
         Tuple[int, int]: An (x, y) point.
     """
     x = ffi.new("int *")
     y = ffi.new("int *")
     lib.TCOD_path_get_destination(p._path_c, x, y)
     return x[0], y[0]
 
 
+@pending_deprecate()
 def path_size(p: tcod.path.AStar) -> int:
     """Return the current length of the computed path.
 
     Args:
         p (AStar): An AStar instance.
     Returns:
         int: Length of the path.
     """
     return int(lib.TCOD_path_size(p._path_c))
 
 
+@pending_deprecate()
 def path_reverse(p: tcod.path.AStar) -> None:
     """Reverse the direction of a path.
 
     This effectively swaps the origin and destination points.
 
     Args:
         p (AStar): An AStar instance.
     """
     lib.TCOD_path_reverse(p._path_c)
 
 
+@pending_deprecate()
 def path_get(p: tcod.path.AStar, idx: int) -> Tuple[int, int]:
     """Get a point on a path.
 
     Args:
         p (AStar): An AStar instance.
         idx (int): Should be in range: 0 <= inx < :any:`path_size`
     """
     x = ffi.new("int *")
     y = ffi.new("int *")
     lib.TCOD_path_get(p._path_c, idx, x, y)
     return x[0], y[0]
 
 
+@pending_deprecate()
 def path_is_empty(p: tcod.path.AStar) -> bool:
     """Return True if a path is empty.
 
     Args:
         p (AStar): An AStar instance.
     Returns:
         bool: True if a path is empty.  Otherwise False.
     """
     return bool(lib.TCOD_path_is_empty(p._path_c))
 
 
+@pending_deprecate()
 def path_walk(
     p: tcod.path.AStar, recompute: bool
 ) -> Union[Tuple[int, int], Tuple[None, None]]:
     """Return the next (x, y) point in a path, or (None, None) if it's empty.
 
     When ``recompute`` is True and a previously valid path reaches a point
     where it is now blocked, a new path will automatically be found.
@@ -2040,61 +2137,71 @@
 def path_delete(p: tcod.path.AStar) -> None:
     """Does nothing. libtcod objects are managed by Python's garbage collector.
 
     This function exists for backwards compatibility with libtcodpy.
     """
 
 
+@pending_deprecate()
 def dijkstra_new(m: tcod.map.Map, dcost: float = 1.41) -> tcod.path.Dijkstra:
     return tcod.path.Dijkstra(m, dcost)
 
 
+@pending_deprecate()
 def dijkstra_new_using_function(
     w: int,
     h: int,
     func: Callable[[int, int, int, int, Any], float],
     userData: Any = 0,
     dcost: float = 1.41,
 ) -> tcod.path.Dijkstra:
     return tcod.path.Dijkstra(
         tcod.path._EdgeCostFunc((func, userData), (w, h)), dcost
     )
 
 
+@pending_deprecate()
 def dijkstra_compute(p: tcod.path.Dijkstra, ox: int, oy: int) -> None:
     lib.TCOD_dijkstra_compute(p._path_c, ox, oy)
 
 
+@pending_deprecate()
 def dijkstra_path_set(p: tcod.path.Dijkstra, x: int, y: int) -> bool:
     return bool(lib.TCOD_dijkstra_path_set(p._path_c, x, y))
 
 
+@pending_deprecate()
 def dijkstra_get_distance(p: tcod.path.Dijkstra, x: int, y: int) -> int:
     return int(lib.TCOD_dijkstra_get_distance(p._path_c, x, y))
 
 
+@pending_deprecate()
 def dijkstra_size(p: tcod.path.Dijkstra) -> int:
     return int(lib.TCOD_dijkstra_size(p._path_c))
 
 
+@pending_deprecate()
 def dijkstra_reverse(p: tcod.path.Dijkstra) -> None:
     lib.TCOD_dijkstra_reverse(p._path_c)
 
 
+@pending_deprecate()
 def dijkstra_get(p: tcod.path.Dijkstra, idx: int) -> Tuple[int, int]:
     x = ffi.new("int *")
     y = ffi.new("int *")
     lib.TCOD_dijkstra_get(p._path_c, idx, x, y)
     return x[0], y[0]
 
 
+@pending_deprecate()
 def dijkstra_is_empty(p: tcod.path.Dijkstra) -> bool:
     return bool(lib.TCOD_dijkstra_is_empty(p._path_c))
 
 
+@pending_deprecate()
 def dijkstra_path_walk(
     p: tcod.path.Dijkstra
 ) -> Union[Tuple[int, int], Tuple[None, None]]:
     x = ffi.new("int *")
     y = ffi.new("int *")
     if lib.TCOD_dijkstra_path_walk(p._path_c, x, y):
         return x[0], y[0]
@@ -2121,14 +2228,15 @@
     if array.dtype != np.float32:
         raise ValueError("array dtype must be float32, not %r" % array.dtype)
     width, height = array.shape
     pointer = ffi.cast("float *", array.ctypes.data)
     return ffi.new("TCOD_heightmap_t *", (width, height, pointer))
 
 
+@pending_deprecate()
 def heightmap_new(w: int, h: int, order: str = "C") -> np.ndarray:
     """Return a new numpy.ndarray formatted for use with heightmap functions.
 
     `w` and `h` are the width and height of the array.
 
     `order` is given to the new NumPy array, it can be 'C' or 'F'.
 
@@ -2147,14 +2255,15 @@
         return np.zeros((h, w), np.float32, order="C")
     elif order == "F":
         return np.zeros((w, h), np.float32, order="F")
     else:
         raise ValueError("Invalid order parameter, should be 'C' or 'F'.")
 
 
+@deprecate("Assign to heightmaps as a NumPy array instead.")
 def heightmap_set_value(hm: np.ndarray, x: int, y: int, value: float) -> None:
     """Set the value of a point on a heightmap.
 
     .. deprecated:: 2.0
         `hm` is a NumPy array, so values should be assigned to it directly.
     """
     if hm.flags["C_CONTIGUOUS"]:
@@ -2242,26 +2351,28 @@
 
     .. deprecated:: 2.0
         Do ``hm2[:] = hm1[:]`` instead.
     """
     hm2[:] = hm1[:]
 
 
+@pending_deprecate()
 def heightmap_normalize(
     hm: np.ndarray, mi: float = 0.0, ma: float = 1.0
 ) -> None:
     """Normalize heightmap values between ``mi`` and ``ma``.
 
     Args:
         mi (float): The lowest value after normalization.
         ma (float): The highest value after normalization.
     """
     lib.TCOD_heightmap_normalize(_heightmap_cdata(hm), mi, ma)
 
 
+@pending_deprecate()
 def heightmap_lerp_hm(
     hm1: np.ndarray, hm2: np.ndarray, hm3: np.ndarray, coef: float
 ) -> None:
     """Perform linear interpolation between two heightmaps storing the result
     in ``hm3``.
 
     This is the same as doing ``hm3[:] = hm1[:] + (hm2[:] - hm1[:]) * coef``
@@ -2311,14 +2422,15 @@
     .. deprecated:: 2.0
         Do ``hm3[:] = hm1[:] * hm2[:]`` instead.
         Alternatively you can do ``HeightMap(hm1.array[:] * hm2.array[:])``.
     """
     hm3[:] = hm1[:] * hm2[:]
 
 
+@pending_deprecate()
 def heightmap_add_hill(
     hm: np.ndarray, x: float, y: float, radius: float, height: float
 ) -> None:
     """Add a hill (a half spheroid) at given position.
 
     If height == radius or -radius, the hill is a half-sphere.
 
@@ -2328,14 +2440,15 @@
         y (float): The y position at the center of the new hill.
         radius (float): The size of the new hill.
         height (float): The height or depth of the new hill.
     """
     lib.TCOD_heightmap_add_hill(_heightmap_cdata(hm), x, y, radius, height)
 
 
+@pending_deprecate()
 def heightmap_dig_hill(
     hm: np.ndarray, x: float, y: float, radius: float, height: float
 ) -> None:
     """
 
     This function takes the highest value (if height > 0) or the lowest
     (if height < 0) between the map and the hill.
@@ -2349,14 +2462,15 @@
         y (float): The y position at the center of the new carving.
         radius (float): The size of the carving.
         height (float): The height or depth of the hill to dig out.
     """
     lib.TCOD_heightmap_dig_hill(_heightmap_cdata(hm), x, y, radius, height)
 
 
+@pending_deprecate()
 def heightmap_rain_erosion(
     hm: np.ndarray,
     nbDrops: int,
     erosionCoef: float,
     sedimentationCoef: float,
     rnd: Optional[tcod.random.Random] = None,
 ) -> None:
@@ -2377,14 +2491,15 @@
         nbDrops,
         erosionCoef,
         sedimentationCoef,
         rnd.random_c if rnd else ffi.NULL,
     )
 
 
+@pending_deprecate()
 def heightmap_kernel_transform(
     hm: np.ndarray,
     kernelsize: int,
     dx: Sequence[int],
     dy: Sequence[int],
     weight: Sequence[float],
     minLevel: float,
@@ -2435,14 +2550,15 @@
     cdy = ffi.new("int[]", dy)
     cweight = ffi.new("float[]", weight)
     lib.TCOD_heightmap_kernel_transform(
         _heightmap_cdata(hm), kernelsize, cdx, cdy, cweight, minLevel, maxLevel
     )
 
 
+@pending_deprecate()
 def heightmap_add_voronoi(
     hm: np.ndarray,
     nbPoints: Any,
     nbCoef: int,
     coef: Sequence[float],
     rnd: Optional[tcod.random.Random] = None,
 ) -> None:
@@ -2557,14 +2673,15 @@
         addy,
         octaves,
         delta,
         scale,
     )
 
 
+@pending_deprecate()
 def heightmap_dig_bezier(
     hm: np.ndarray,
     px: Tuple[int, int, int, int],
     py: Tuple[int, int, int, int],
     startRadius: float,
     startDepth: float,
     endRadius: float,
@@ -2616,14 +2733,15 @@
             stacklevel=2,
         )
         return hm[x, y]  # type: ignore
     else:
         raise ValueError("This array is not contiguous.")
 
 
+@pending_deprecate()
 def heightmap_get_interpolated_value(
     hm: np.ndarray, x: float, y: float
 ) -> float:
     """Return the interpolated height at non integer coordinates.
 
     Args:
         hm (numpy.ndarray): A numpy.ndarray formatted for heightmap functions.
@@ -2634,28 +2752,30 @@
         float: The value at ``x``, ``y``.
     """
     return float(
         lib.TCOD_heightmap_get_interpolated_value(_heightmap_cdata(hm), x, y)
     )
 
 
+@pending_deprecate()
 def heightmap_get_slope(hm: np.ndarray, x: int, y: int) -> float:
     """Return the slope between 0 and (pi / 2) at given coordinates.
 
     Args:
         hm (numpy.ndarray): A numpy.ndarray formatted for heightmap functions.
         x (int): The x coordinate.
         y (int): The y coordinate.
 
     Returns:
         float: The steepness at ``x``, ``y``.  From 0 to (pi / 2)
     """
     return float(lib.TCOD_heightmap_get_slope(_heightmap_cdata(hm), x, y))
 
 
+@pending_deprecate()
 def heightmap_get_normal(
     hm: np.ndarray, x: float, y: float, waterLevel: float
 ) -> Tuple[float, float, float]:
     """Return the map normal at given coordinates.
 
     Args:
         hm (numpy.ndarray): A numpy.ndarray formatted for heightmap functions.
@@ -2686,14 +2806,15 @@
     .. deprecated:: 8.1
         Can be replaced by an equivalent NumPy function such as:
         ``numpy.count_nonzero((mi <= hm) & (hm < ma))``
     """
     return int(lib.TCOD_heightmap_count_cells(_heightmap_cdata(hm), mi, ma))
 
 
+@pending_deprecate()
 def heightmap_has_land_on_border(hm: np.ndarray, waterlevel: float) -> bool:
     """Returns True if the map edges are below ``waterlevel``, otherwise False.
 
     Args:
         hm (numpy.ndarray): A numpy.ndarray formatted for heightmap functions.
         waterLevel (float): The water level to use.
 
@@ -2731,69 +2852,81 @@
     This function exists for backwards compatibility with libtcodpy.
 
     .. deprecated:: 2.0
         libtcod-cffi deletes heightmaps automatically.
     """
 
 
+@pending_deprecate()
 def image_new(width: int, height: int) -> tcod.image.Image:
     return tcod.image.Image(width, height)
 
 
+@pending_deprecate()
 def image_clear(image: tcod.image.Image, col: Tuple[int, int, int]) -> None:
     image.clear(col)
 
 
+@pending_deprecate()
 def image_invert(image: tcod.image.Image) -> None:
     image.invert()
 
 
+@pending_deprecate()
 def image_hflip(image: tcod.image.Image) -> None:
     image.hflip()
 
 
+@pending_deprecate()
 def image_rotate90(image: tcod.image.Image, num: int = 1) -> None:
     image.rotate90(num)
 
 
+@pending_deprecate()
 def image_vflip(image: tcod.image.Image) -> None:
     image.vflip()
 
 
+@pending_deprecate()
 def image_scale(image: tcod.image.Image, neww: int, newh: int) -> None:
     image.scale(neww, newh)
 
 
+@pending_deprecate()
 def image_set_key_color(
     image: tcod.image.Image, col: Tuple[int, int, int]
 ) -> None:
     image.set_key_color(col)
 
 
+@pending_deprecate()
 def image_get_alpha(image: tcod.image.Image, x: int, y: int) -> int:
     return image.get_alpha(x, y)
 
 
+@pending_deprecate()
 def image_is_pixel_transparent(
     image: tcod.image.Image, x: int, y: int
 ) -> bool:
     return bool(lib.TCOD_image_is_pixel_transparent(image.image_c, x, y))
 
 
+@pending_deprecate()
 def image_load(filename: str) -> tcod.image.Image:
     """Load an image file into an Image instance and return it.
 
     Args:
         filename (AnyStr): Path to a .bmp or .png image file.
     """
     return tcod.image.Image._from_cdata(
         ffi.gc(lib.TCOD_image_load(_bytes(filename)), lib.TCOD_image_delete)
     )
 
 
+@pending_deprecate()
 def image_from_console(console: tcod.console.Console) -> tcod.image.Image:
     """Return an Image with a Consoles pixel data.
 
     This effectively takes a screen-shot of the Console.
 
     Args:
         console (Console): Any Console instance.
@@ -2802,80 +2935,89 @@
         ffi.gc(
             lib.TCOD_image_from_console(_console(console)),
             lib.TCOD_image_delete,
         )
     )
 
 
+@pending_deprecate()
 def image_refresh_console(
     image: tcod.image.Image, console: tcod.console.Console
 ) -> None:
     image.refresh_console(console)
 
 
+@pending_deprecate()
 def image_get_size(image: tcod.image.Image) -> Tuple[int, int]:
     return image.width, image.height
 
 
+@pending_deprecate()
 def image_get_pixel(
     image: tcod.image.Image, x: int, y: int
 ) -> Tuple[int, int, int]:
     return image.get_pixel(x, y)
 
 
+@pending_deprecate()
 def image_get_mipmap_pixel(
     image: tcod.image.Image, x0: float, y0: float, x1: float, y1: float
 ) -> Tuple[int, int, int]:
     return image.get_mipmap_pixel(x0, y0, x1, y1)
 
 
+@pending_deprecate()
 def image_put_pixel(
     image: tcod.image.Image, x: int, y: int, col: Tuple[int, int, int]
 ) -> None:
     image.put_pixel(x, y, col)
 
 
+@pending_deprecate()
 def image_blit(
     image: tcod.image.Image,
     console: tcod.console.Console,
     x: float,
     y: float,
     bkgnd_flag: int,
     scalex: float,
     scaley: float,
     angle: float,
 ) -> None:
     image.blit(console, x, y, bkgnd_flag, scalex, scaley, angle)
 
 
+@pending_deprecate()
 def image_blit_rect(
     image: tcod.image.Image,
     console: tcod.console.Console,
     x: int,
     y: int,
     w: int,
     h: int,
     bkgnd_flag: int,
 ) -> None:
     image.blit_rect(console, x, y, w, h, bkgnd_flag)
 
 
+@pending_deprecate()
 def image_blit_2x(
     image: tcod.image.Image,
     console: tcod.console.Console,
     dx: int,
     dy: int,
     sx: int = 0,
     sy: int = 0,
     w: int = -1,
     h: int = -1,
 ) -> None:
     image.blit_2x(console, dx, dy, sx, sy, w, h)
 
 
+@pending_deprecate()
 def image_save(image: tcod.image.Image, filename: str) -> None:
     image.save_as(filename)
 
 
 @deprecate("libtcod objects are deleted automatically.")
 def image_delete(image: tcod.image.Image) -> None:
     """Does nothing. libtcod objects are managed by Python's garbage collector.
@@ -3146,65 +3288,75 @@
 
     .. deprecated:: 4.5
         Check the :any:`tcod.map.Map.height` attribute instead.
     """
     return map.height
 
 
+@pending_deprecate()
 def mouse_show_cursor(visible: bool) -> None:
     """Change the visibility of the mouse cursor."""
     lib.TCOD_mouse_show_cursor(visible)
 
 
+@pending_deprecate()
 def mouse_is_cursor_visible() -> bool:
     """Return True if the mouse cursor is visible."""
     return bool(lib.TCOD_mouse_is_cursor_visible())
 
 
+@pending_deprecate()
 def mouse_move(x: int, y: int) -> None:
     lib.TCOD_mouse_move(x, y)
 
 
+@deprecate("Use tcod.event.get_mouse_state() instead.")
 def mouse_get_status() -> Mouse:
     return Mouse(lib.TCOD_mouse_get_status())
 
 
+@pending_deprecate()
 def namegen_parse(
     filename: str, random: Optional[tcod.random.Random] = None
 ) -> None:
     lib.TCOD_namegen_parse(_bytes(filename), random or ffi.NULL)
 
 
+@pending_deprecate()
 def namegen_generate(name: str) -> str:
     return _unpack_char_p(lib.TCOD_namegen_generate(_bytes(name), False))
 
 
+@pending_deprecate()
 def namegen_generate_custom(name: str, rule: str) -> str:
     return _unpack_char_p(
         lib.TCOD_namegen_generate_custom(_bytes(name), _bytes(rule), False)
     )
 
 
+@pending_deprecate()
 def namegen_get_sets() -> List[str]:
     sets = lib.TCOD_namegen_get_sets()
     try:
         lst = []
         while not lib.TCOD_list_is_empty(sets):
             lst.append(
                 _unpack_char_p(ffi.cast("char *", lib.TCOD_list_pop(sets)))
             )
     finally:
         lib.TCOD_list_delete(sets)
     return lst
 
 
+@pending_deprecate()
 def namegen_destroy() -> None:
     lib.TCOD_namegen_destroy()
 
 
+@pending_deprecate()
 def noise_new(
     dim: int,
     h: float = NOISE_DEFAULT_HURST,
     l: float = NOISE_DEFAULT_LACUNARITY,  # noqa: E741
     random: Optional[tcod.random.Random] = None,
 ) -> tcod.noise.Noise:
     """Return a new Noise instance.
@@ -3217,23 +3369,25 @@
 
     Returns:
         Noise: The new Noise instance.
     """
     return tcod.noise.Noise(dim, hurst=h, lacunarity=l, seed=random)
 
 
+@pending_deprecate()
 def noise_set_type(n: tcod.noise.Noise, typ: int) -> None:
     """Set a Noise objects default noise algorithm.
 
     Args:
         typ (int): Any NOISE_* constant.
     """
     n.algorithm = typ
 
 
+@pending_deprecate()
 def noise_get(
     n: tcod.noise.Noise, f: Sequence[float], typ: int = NOISE_DEFAULT
 ) -> float:
     """Return the noise value sampled from the ``f`` coordinate.
 
     ``f`` should be a tuple or list with a length matching
     :any:`Noise.dimensions`.
@@ -3247,14 +3401,15 @@
 
     Returns:
         float: The sampled noise value.
     """
     return float(lib.TCOD_noise_get_ex(n.noise_c, ffi.new("float[4]", f), typ))
 
 
+@pending_deprecate()
 def noise_get_fbm(
     n: tcod.noise.Noise,
     f: Sequence[float],
     oc: float,
     typ: int = NOISE_DEFAULT,
 ) -> float:
     """Return the fractal Brownian motion sampled from the ``f`` coordinate.
@@ -3269,14 +3424,15 @@
         float: The sampled noise value.
     """
     return float(
         lib.TCOD_noise_get_fbm_ex(n.noise_c, ffi.new("float[4]", f), oc, typ)
     )
 
 
+@pending_deprecate()
 def noise_get_turbulence(
     n: tcod.noise.Noise,
     f: Sequence[float],
     oc: float,
     typ: int = NOISE_DEFAULT,
 ) -> float:
     """Return the turbulence noise sampled from the ``f`` coordinate.
@@ -3471,37 +3627,40 @@
 DISTRIBUTION_LINEAR = 0
 DISTRIBUTION_GAUSSIAN = 1
 DISTRIBUTION_GAUSSIAN_RANGE = 2
 DISTRIBUTION_GAUSSIAN_INVERSE = 3
 DISTRIBUTION_GAUSSIAN_RANGE_INVERSE = 4
 
 
+@pending_deprecate()
 def random_get_instance() -> tcod.random.Random:
     """Return the default Random instance.
 
     Returns:
         Random: A Random instance using the default random number generator.
     """
     return tcod.random.Random._new_from_cdata(
         ffi.cast("mersenne_data_t*", lib.TCOD_random_get_instance())
     )
 
 
+@pending_deprecate()
 def random_new(algo: int = RNG_CMWC) -> tcod.random.Random:
     """Return a new Random instance.  Using ``algo``.
 
     Args:
         algo (int): The random number algorithm to use.
 
     Returns:
         Random: A new Random instance using the given algorithm.
     """
     return tcod.random.Random(algo)
 
 
+@pending_deprecate()
 def random_new_from_seed(
     seed: Hashable, algo: int = RNG_CMWC
 ) -> tcod.random.Random:
     """Return a new Random instance.  Using the given ``seed`` and ``algo``.
 
     Args:
         seed (Hashable): The RNG seed.  Should be a 32-bit integer, but any
@@ -3510,50 +3669,53 @@
 
     Returns:
         Random: A new Random instance using the given algorithm.
     """
     return tcod.random.Random(algo, seed)
 
 
+@pending_deprecate()
 def random_set_distribution(
     rnd: Optional[tcod.random.Random], dist: int
 ) -> None:
     """Change the distribution mode of a random number generator.
 
     Args:
         rnd (Optional[Random]): A Random instance, or None to use the default.
         dist (int): The distribution mode to use.  Should be DISTRIBUTION_*.
     """
     lib.TCOD_random_set_distribution(rnd.random_c if rnd else ffi.NULL, dist)
 
 
+@pending_deprecate()
 def random_get_int(rnd: Optional[tcod.random.Random], mi: int, ma: int) -> int:
     """Return a random integer in the range: ``mi`` <= n <= ``ma``.
 
-    The result is affacted by calls to :any:`random_set_distribution`.
+    The result is affected by calls to :any:`random_set_distribution`.
 
     Args:
         rnd (Optional[Random]): A Random instance, or None to use the default.
         low (int): The lower bound of the random range, inclusive.
         high (int): The upper bound of the random range, inclusive.
 
     Returns:
         int: A random integer in the range ``mi`` <= n <= ``ma``.
     """
     return int(
         lib.TCOD_random_get_int(rnd.random_c if rnd else ffi.NULL, mi, ma)
     )
 
 
+@pending_deprecate()
 def random_get_float(
     rnd: Optional[tcod.random.Random], mi: float, ma: float
 ) -> float:
     """Return a random float in the range: ``mi`` <= n <= ``ma``.
 
-    The result is affacted by calls to :any:`random_set_distribution`.
+    The result is affected by calls to :any:`random_set_distribution`.
 
     Args:
         rnd (Optional[Random]): A Random instance, or None to use the default.
         low (float): The lower bound of the random range, inclusive.
         high (float): The upper bound of the random range, inclusive.
 
     Returns:
@@ -3576,14 +3738,15 @@
         Both funtions return a double precision float.
     """
     return float(
         lib.TCOD_random_get_double(rnd.random_c if rnd else ffi.NULL, mi, ma)
     )
 
 
+@pending_deprecate()
 def random_get_int_mean(
     rnd: Optional[tcod.random.Random], mi: int, ma: int, mean: int
 ) -> int:
     """Return a random weighted integer in the range: ``mi`` <= n <= ``ma``.
 
     The result is affacted by calls to :any:`random_set_distribution`.
 
@@ -3599,14 +3762,15 @@
     return int(
         lib.TCOD_random_get_int_mean(
             rnd.random_c if rnd else ffi.NULL, mi, ma, mean
         )
     )
 
 
+@pending_deprecate()
 def random_get_float_mean(
     rnd: Optional[tcod.random.Random], mi: float, ma: float, mean: float
 ) -> float:
     """Return a random weighted float in the range: ``mi`` <= n <= ``ma``.
 
     The result is affacted by calls to :any:`random_set_distribution`.
 
@@ -3839,14 +4003,15 @@
     """
     lib.TCOD_sys_save_screenshot(
         _bytes(name) if name is not None else ffi.NULL
     )
 
 
 # custom fullscreen resolution
+@pending_deprecate()
 def sys_force_fullscreen_resolution(width: int, height: int) -> None:
     """Force a specific resolution in fullscreen.
 
     Will use the smallest available resolution so that:
 
     * resolution width >= width and
       resolution width >= root console width * font char width
@@ -3881,14 +4046,15 @@
     w = ffi.new("int *")
     h = ffi.new("int *")
     lib.TCOD_sys_get_char_size(w, h)
     return w[0], h[0]
 
 
 # update font bitmap
+@pending_deprecate()
 def sys_update_char(
     asciiCode: int,
     fontx: int,
     fonty: int,
     img: tcod.image.Image,
     x: int,
     y: int,
@@ -3907,14 +4073,15 @@
         img (Image): An image containing the new character bitmap.
         x (int): Left pixel of the character in the image.
         y (int): Top pixel of the character in the image.
     """
     lib.TCOD_sys_update_char(_int(asciiCode), fontx, fonty, img, x, y)
 
 
+@pending_deprecate()
 def sys_register_SDL_renderer(callback: Callable[[Any], None]) -> None:
     """Register a custom randering function with libtcod.
 
     Note:
         This callback will only be called by the SDL renderer.
 
     The callack will receive a :any:`CData <ffi-cdata>` void* to an
@@ -3931,33 +4098,38 @@
         @ffi.def_extern(onerror=propagate)  # type: ignore
         def _pycall_sdl_hook(sdl_surface: Any) -> None:
             callback(sdl_surface)
 
         lib.TCOD_sys_register_SDL_renderer(lib._pycall_sdl_hook)
 
 
+@deprecate("Use tcod.event.get to check for events.")
 def sys_check_for_event(
     mask: int, k: Optional[Key], m: Optional[Mouse]
 ) -> int:
     """Check for and return an event.
 
     Args:
         mask (int): :any:`Event types` to wait for.
         k (Optional[Key]): A tcod.Key instance which might be updated with
                            an event.  Can be None.
         m (Optional[Mouse]): A tcod.Mouse instance which might be updated
                              with an event.  Can be None.
+
+    .. deprecated:: 9.3
+        Use the :any:`tcod.event.get` function to check for events.
     """
     return int(
         lib.TCOD_sys_check_for_event(
             mask, k.key_p if k else ffi.NULL, m.mouse_p if m else ffi.NULL
         )
     )
 
 
+@deprecate("Use tcod.event.wait to wait for events.")
 def sys_wait_for_event(
     mask: int, k: Optional[Key], m: Optional[Mouse], flush: bool
 ) -> int:
     """Wait for an event then return.
 
     If flush is True then the buffer will be cleared before waiting. Otherwise
     each available event will be returned in the order they're recieved.
@@ -3965,14 +4137,17 @@
     Args:
         mask (int): :any:`Event types` to wait for.
         k (Optional[Key]): A tcod.Key instance which might be updated with
                            an event.  Can be None.
         m (Optional[Mouse]): A tcod.Mouse instance which might be updated
                              with an event.  Can be None.
         flush (bool): Clear the event buffer before waiting.
+
+    .. deprecated:: 9.3
+        Use the :any:`tcod.event.wait` function to wait for events.
     """
     return int(
         lib.TCOD_sys_wait_for_event(
             mask,
             k.key_p if k else ffi.NULL,
             m.mouse_p if m else ffi.NULL,
             flush,
```

### Comparing `tcod-9.2.5/tcod/map.py` & `tcod-9.3.0/tcod/map.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,9 @@
 """libtcod map attributes and field-of-view functions.
 
-Example::
-
-    >>> import tcod.map
-    >>> m = tcod.map.Map(width=3, height=4)
-    >>> m.walkable
-    array([[False, False, False],
-           [False, False, False],
-           [False, False, False],
-           [False, False, False]]...)
-
-    # Like the rest of the tcod modules, all arrays here are
-    # in row-major order and are addressed with [y,x]
-    >>> m.transparent[:] = True # Sets all to True.
-    >>> m.transparent[1:3,0] = False # Sets (1, 0) and (2, 0) to False.
-    >>> m.transparent
-    array([[ True,  True,  True],
-           [False,  True,  True],
-           [False,  True,  True],
-           [ True,  True,  True]]...)
-
-    >>> m.compute_fov(0, 0)
-    >>> m.fov
-    array([[ True,  True,  True],
-           [ True,  True,  True],
-           [False,  True,  True],
-           [False, False,  True]]...)
-    >>> m.fov[3,1]
-    False
 
 """
 from typing import Any
 
 import numpy as np
 
 from tcod.libtcod import lib, ffi
@@ -56,14 +28,42 @@
     Attributes:
         width (int): Read only width of this Map.
         height (int): Read only height of this Map.
         transparent: A boolean array of transparent cells.
         walkable: A boolean array of walkable cells.
         fov: A boolean array of the cells lit by :any:'compute_fov'.
 
+    Example::
+
+        >>> import tcod.map
+        >>> m = tcod.map.Map(width=3, height=4)
+        >>> m.walkable
+        array([[False, False, False],
+               [False, False, False],
+               [False, False, False],
+               [False, False, False]]...)
+
+        # Like the rest of the tcod modules, all arrays here are
+        # in row-major order and are addressed with [y,x]
+        >>> m.transparent[:] = True  # Sets all to True.
+        >>> m.transparent[1:3,0] = False  # Sets (1, 0) and (2, 0) to False.
+        >>> m.transparent
+        array([[ True,  True,  True],
+               [False,  True,  True],
+               [False,  True,  True],
+               [ True,  True,  True]]...)
+
+        >>> m.compute_fov(0, 0)
+        >>> m.fov
+        array([[ True,  True,  True],
+               [ True,  True,  True],
+               [False,  True,  True],
+               [False, False,  True]]...)
+        >>> m.fov[3,1]
+        False
     """
 
     def __init__(self, width: int, height: int, order: str = "C"):
         self.width = width
         self.height = height
         self._order = tcod._internal.verify_order(order)
 
@@ -110,14 +110,17 @@
             x (int): Point of view, x-coordinate.
             y (int): Point of view, y-coordinate.
             radius (int): Maximum view distance from the point of view.
 
                 A value of `0` will give an infinite distance.
             light_walls (bool): Light up walls, or only the floor.
             algorithm (int): Defaults to tcod.FOV_RESTRICTIVE
+
+        If you already have transparency in a NumPy array then you could use
+        :any:`tcod.map_compute_fov` instead.
         """
         lib.TCOD_map_compute_fov(
             self.map_c, x, y, radius, light_walls, algorithm
         )
 
     def __setstate__(self, state: Any) -> None:
         if "_Map__buffer" not in state:  # deprecated
@@ -135,7 +138,72 @@
         self.__dict__.update(state)
         self.map_c = self.__as_cdata()
 
     def __getstate__(self) -> Any:
         state = self.__dict__.copy()
         del state["map_c"]
         return state
+
+
+def compute_fov(
+    transparency: np.array,
+    x: int,
+    y: int,
+    radius: int = 0,
+    light_walls: bool = True,
+    algorithm: int = tcod.constants.FOV_RESTRICTIVE,
+) -> np.array:
+    """Return the visible area of a field-of-view computation.
+
+    `transparency` is a 2 dimensional array where all non-zero values are
+    considered transparent.  The returned array will match the shape of this
+    array.
+
+    `x` and `y` are the 1st and 2nd coordinates of the origin point.  Areas
+    are visible when they can be seen from this point-of-view.
+
+    `radius` is the maximum view distance from `x`/`y`.  If this is zero then
+    the maximum distance is used.
+
+    If `light_walls` is True then visible obstacles will be returned, otherwise
+    only transparent areas will be.
+
+    `algorithm` is the field-of-view algorithm to run.  The default value is
+    `tcod.FOV_RESTRICTIVE`.
+    The options are:
+
+    * `tcod.FOV_BASIC`:
+      Simple ray-cast implementation.
+    * `tcod.FOV_DIAMOND`
+    * `tcod.FOV_SHADOW`:
+      Recursive shadow caster.
+    * `tcod.FOV_PERMISSIVE(n)`:
+      `n` starts at 0 (most restrictive) and goes up to 8 (most permissive.)
+    * `tcod.FOV_RESTRICTIVE`
+
+    .. versionadded:: 9.3
+
+    Example::
+
+        >>> explored = np.zeros((3, 5), dtype=bool, order="F")
+        >>> transparency = np.ones((3, 5), dtype=bool, order="F")
+        >>> transparency[:2, 2] = False
+        >>> transparency  # Transparent area.
+        array([[ True,  True, False,  True,  True],
+               [ True,  True, False,  True,  True],
+               [ True,  True,  True,  True,  True]]...)
+        >>> visible = tcod.map.compute_fov(transparency, 0, 0)
+        >>> visible  # Visible area.
+        array([[ True,  True,  True, False, False],
+               [ True,  True,  True, False, False],
+               [ True,  True,  True,  True, False]]...)
+        >>> explored |= visible  # Keep track of an explored area.
+    """
+    if len(transparency.shape) != 2:
+        raise TypeError(
+            "transparency must be an array of 2 dimensions"
+            " (shape is %r)" % transparency.shape
+        )
+    map_ = Map(transparency.shape[1], transparency.shape[0])
+    map_.transparent[...] = transparency
+    map_.compute_fov(x, y, radius, light_walls, algorithm)
+    return map_.fov
```

### Comparing `tcod-9.2.5/tcod/noise.c` & `tcod-9.3.0/tcod/noise.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/noise.h` & `tcod-9.3.0/tcod/noise.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/noise.py` & `tcod-9.3.0/tcod/noise.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/path.cpp` & `tcod-9.3.0/tcod/path.cpp`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/path.h` & `tcod-9.3.0/tcod/path.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/path.py` & `tcod-9.3.0/tcod/path.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/path2.py` & `tcod-9.3.0/tcod/path2.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/random.h` & `tcod-9.3.0/tcod/random.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/random.py` & `tcod-9.3.0/tcod/random.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/tcod.cpp` & `tcod-9.3.0/tcod/tcod.cpp`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/tcod.h` & `tcod-9.3.0/tcod/tcod.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/tcod.py` & `tcod-9.3.0/tcod/tcod.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/tdl.c` & `tcod-9.3.0/tcod/tdl.c`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/tdl.h` & `tcod-9.3.0/tcod/tdl.h`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/tileset.py` & `tcod-9.3.0/tcod/tileset.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod/__init__.py` & `tcod-9.3.0/tcod/__init__.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tcod.egg-info/PKG-INFO` & `tcod-9.3.0/tcod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tcod
-Version: 9.2.5
+Version: 9.3.0
 Summary: Pythonic cffi port of libtcod.
 Home-page: https://github.com/libtcod/python-tcod
 Author: Kyle Stewart
 Author-email: 4B796C65+tdl@gmail.com
 License: Simplified BSD License
 Description: .. contents::
            :backlinks: top
@@ -36,43 +36,26 @@
         If you had code that runs on libtcodpy then you can use this library as a
         drop-in replacement.  This installs a libtcodpy module so you'll only need to
         delete the libtcodpy/ folder that's usually bundled in an older libtcodpy
         project.
         
         Guides and Tutorials for libtcodpy should work with the tcod module.
         
-        The latest documentation can be found
-        `here <https://python-tcod.readthedocs.io/en/latest/>`_.
+        The latest documentation can be found here:
+        https://python-tcod.readthedocs.io/en/latest/
         
         ==============
          Installation
         ==============
-        The recommended way to install is by using pip.  Older versions of pip will
-        have issues installing tcod, so make sure it's up-to-date.
+        Detailed installation instructions are here:
+        https://python-tcod.readthedocs.io/en/latest/installation.html
         
-        Windows / MacOS
-        ---------------
-        To install using pip, use the following command::
-        
-            > python -m pip install tcod
-        
-        If you get the error "ImportError: DLL load failed: The specified module could
-        not be found." when trying to import tcod/tdl then you may need the latest
-        `Microsoft Visual C runtime
-        <https://support.microsoft.com/en-ca/help/2977003/the-latest-supported-visual-c-downloads>`_.
-        
-        Linux
-        -----
-        On Linux python-tcod will need to be built from source.
-        Assuming you have Python, pip, and apt-get, then you'll run these commands to
-        install python-tcod and its dependencies to your user environment::
-        
-            $ sudo apt-get install gcc python-dev python3-dev libsdl2-dev libffi-dev libomp5
-            $ pip2 install tcod
-            $ pip3 install tcod
+        For the most part it's just::
+        
+            pip3 install tcod
         
         ==============
          Requirements
         ==============
         * Python 3.5+
         * Windows, Linux, or MacOS X 10.9+.
         * On Windows, requires the Visual C++ runtime 2015 or later.
@@ -137,21 +120,45 @@
         .. |Pyup| image:: https://pyup.io/repos/github/libtcod/python-tcod/shield.svg
             :target: https://pyup.io/repos/github/libtcod/python-tcod/
             :alt: Updates
         
         ===========
          Changelog
         ===========
-        Changes relevant for users of the the tdl and tcod packages are documented
-        here.
+        Changes relevant to the users of python-tcod are documented here.
         
         This project adheres to `Semantic Versioning <https://semver.org/>`_ since
         v2.0.0
         
         
+        9.3.0 - 2019-03-15
+        ------------------
+        Added
+         - The SDL2/OPENGL2 renderers can potentially use a fall-back font when none
+           are provided.
+         - New function `tcod.event.get_mouse_state`.
+         - New function `tcod.map.compute_fov` lets you get a visibility array directly
+           from a transparency array.
+        Deprecated
+         - The following functions and classes have been deprecated.
+           - `tcod.Key`
+           - `tcod.Mouse`
+           - `tcod.mouse_get_status`
+           - `tcod.console_is_window_closed`
+           - `tcod.console_check_for_keypress`
+           - `tcod.console_wait_for_keypress`
+           - `tcod.console_delete`
+           - `tcod.sys_check_for_event`
+           - `tcod.sys_wait_for_event`
+         - The SDL, OPENGL, and GLSL renderers have been deprecated.
+         - Many libtcodpy functions have been marked with PendingDeprecationWarning's.
+        Fixed
+         - To be more compatible with libtcodpy `tcod.console_init_root` will default
+           to the SDL render, but will raise warnings when an old renderer is used.
+        
         9.2.5 - 2019-03-04
         ------------------
         Fixed
          - Fixed `tcod.namegen_generate_custom`.
         
         9.2.4 - 2019-03-02
         ------------------
@@ -165,50 +172,50 @@
            the future.
          - Methods and functionality preventing `tcod.Color` from behaving like a tuple
            have been deprecated.
         
         9.2.2 - 2019-02-26
         ------------------
         Fixed
-        - `Console.print_box` wasn't setting the background color by default.
+         - `Console.print_box` wasn't setting the background color by default.
         
         9.2.1 - 2019-02-25
         ------------------
         Fixed
-        - `tcod.sys_get_char_size` fixed on the new renderers.
+         - `tcod.sys_get_char_size` fixed on the new renderers.
         
         9.2.0 - 2019-02-24
         ------------------
         Added
-        - New `tcod.console.get_height_rect` function, which can be used to get the
-          height of a print call without an existing console.
-        - New `tcod.tileset` module, with a `set_truetype_font` function.
-        Fixed
-        - The new print methods now handle alignment according to how they were
-          documented.
-        - `SDL2` and `OPENGL2` now support screenshots.
-        - Windows and MacOS builds now restrict exported SDL2 symbols to only
-          SDL 2.0.5;  This will avoid hard to debug import errors when the wrong
-          version of SDL is dynamically linked.
-        - The root console now starts with a white foreground.
+         - New `tcod.console.get_height_rect` function, which can be used to get the
+           height of a print call without an existing console.
+         - New `tcod.tileset` module, with a `set_truetype_font` function.
+        Fixed
+         - The new print methods now handle alignment according to how they were
+           documented.
+         - `SDL2` and `OPENGL2` now support screenshots.
+         - Windows and MacOS builds now restrict exported SDL2 symbols to only
+           SDL 2.0.5;  This will avoid hard to debug import errors when the wrong
+           version of SDL is dynamically linked.
+         - The root console now starts with a white foreground.
         
         9.1.0 - 2019-02-23
         ------------------
         Added
-        - Added the `tcod.random.MULTIPLY_WITH_CARRY` constant.
+         - Added the `tcod.random.MULTIPLY_WITH_CARRY` constant.
         Changed
-        - The overhead for warnings has been reduced when running Python with the
-          optimize `-O` flag.
-        - `tcod.random.Random` now provides a default algorithm.
+         - The overhead for warnings has been reduced when running Python with the
+           optimize `-O` flag.
+         - `tcod.random.Random` now provides a default algorithm.
         
         9.0.0 - 2019-02-17
         ------------------
         Changed
-        - New console methods now default to an `fg` and `bg` of None instead of
-          white-on-black.
+         - New console methods now default to an `fg` and `bg` of None instead of
+           white-on-black.
         
         8.5.0 - 2019-02-15
         ------------------
         Added
          - `tcod.console.Console` now supports `str` and `repr`.
          - Added new Console methods which are independent from the console defaults.
          - You can now give an array when initializing a `tcod.console.Console`
```

### Comparing `tcod-9.2.5/tcod.egg-info/SOURCES.txt` & `tcod-9.3.0/tcod.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 dependencies/fake_libc_include/sys/types.h
 dependencies/fake_libc_include/sys/uio.h
 dependencies/fake_libc_include/sys/un.h
 dependencies/fake_libc_include/sys/utsname.h
 dependencies/fake_libc_include/sys/wait.h
 libtcod/CHANGELOG.md
 libtcod/LIBTCOD-CREDITS.txt
-libtcod/LIBTCOD-LICENSE.txt
+libtcod/LICENSE.txt
 libtcod/README.md
 libtcod/src/libtcod.cpp
 libtcod/src/libtcod_c.c
 libtcod/src/vendor/glad.c
 libtcod/src/vendor/lodepng.cpp
 libtcod/src/vendor/utf8proc/utf8proc.c
 libtcod/src/vendor/zlib/adler32.c
@@ -314,14 +314,16 @@
 libtcod/src/libtcod/pathfinding/dijkstra.h
 libtcod/src/libtcod/pathfinding/generic.cpp
 libtcod/src/libtcod/pathfinding/generic.h
 libtcod/src/libtcod/sdl2/console_2tris.glslf
 libtcod/src/libtcod/sdl2/console_2tris.glslv
 libtcod/src/libtcod/sdl2/console_grid.glslf
 libtcod/src/libtcod/sdl2/console_grid.glslv
+libtcod/src/libtcod/sdl2/event.cpp
+libtcod/src/libtcod/sdl2/event.h
 libtcod/src/libtcod/sdl2/gl2_display.cpp
 libtcod/src/libtcod/sdl2/gl2_display.h
 libtcod/src/libtcod/sdl2/gl2_ext_.h
 libtcod/src/libtcod/sdl2/gl2_raii.cpp
 libtcod/src/libtcod/sdl2/gl2_raii.h
 libtcod/src/libtcod/sdl2/gl2_renderer.cpp
 libtcod/src/libtcod/sdl2/gl2_renderer.h
@@ -331,14 +333,16 @@
 libtcod/src/libtcod/sdl2/legacy_backend.h
 libtcod/src/libtcod/sdl2/sdl2_alias.cpp
 libtcod/src/libtcod/sdl2/sdl2_alias.h
 libtcod/src/libtcod/sdl2/sdl2_display.cpp
 libtcod/src/libtcod/sdl2/sdl2_display.h
 libtcod/src/libtcod/sdl2/sdl2_renderer.cpp
 libtcod/src/libtcod/sdl2/sdl2_renderer.h
+libtcod/src/libtcod/tileset/fallback.cpp
+libtcod/src/libtcod/tileset/fallback.h
 libtcod/src/libtcod/tileset/observer.cpp
 libtcod/src/libtcod/tileset/observer.h
 libtcod/src/libtcod/tileset/tile.cpp
 libtcod/src/libtcod/tileset/tile.h
 libtcod/src/libtcod/tileset/tileset.cpp
 libtcod/src/libtcod/tileset/tileset.h
 libtcod/src/libtcod/tileset/tilesheet.cpp
```

### Comparing `tcod-9.2.5/tdl/event.py` & `tcod-9.3.0/tdl/event.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tdl/map.py` & `tcod-9.3.0/tdl/map.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tdl/noise.py` & `tcod-9.3.0/tdl/noise.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tdl/style.py` & `tcod-9.3.0/tdl/style.py`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tdl/terminal8x8.png` & `tcod-9.3.0/tdl/terminal8x8.png`

 * *Files identical despite different names*

### Comparing `tcod-9.2.5/tdl/__init__.py` & `tcod-9.3.0/tdl/__init__.py`

 * *Files identical despite different names*

