# `joomla:4.0.6-php7.4-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:c6242a7ec8e4a0cb23b40390d91e650e0964f294f43d124feef1dc047a4001a3`
- Created: `2022-01-21T22:44:53.541042391Z`
- Virtual Size: ~ 199.65 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/entrypoint.sh"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_LDFLAGS=-Wl,-O1 -pie`
  - `GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312`
  - `PHP_VERSION=7.4.27`
  - `PHP_URL=https://www.php.net/distributions/php-7.4.27.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-7.4.27.tar.xz.asc`
  - `PHP_SHA256=3f8b937310f155822752229c2c2feb8cc2621e25a728e7b94d0d74c128c43d0c`
  - `JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1`
  - `JOOMLA_VERSION=4.0.6`
  - `JOOMLA_SHA512=a35f3181c594ef0c30e4f8ec122f32e2ebe1795ccd31f55656be0f214b1f6eed54ef7961aed0be772b2c4a6cc5d0e6454b9213f1ba8833dd52317c6d216d9fd8`
- Labels:
  - `maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.2.0-r18 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.2.0-r18 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.2.0-r18 installed size:
404 KiB

alpine-baselayout-3.2.0-r18 license:
GPL-2.0-only

```

### `apk` package: `alpine-keys`

```console
alpine-keys-2.4-r1 description:
Public keys for Alpine Linux packages

alpine-keys-2.4-r1 webpage:
https://alpinelinux.org

alpine-keys-2.4-r1 installed size:
156 KiB

alpine-keys-2.4-r1 license:
MIT

```

### `apk` package: `apk-tools`

```console
apk-tools-2.12.7-r3 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.12.7-r3 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.12.7-r3 installed size:
304 KiB

apk-tools-2.12.7-r3 license:
GPL-2.0-only

```

### `apk` package: `argon2-libs`

```console
argon2-libs-20190702-r1 description:
The password hash Argon2, winner of PHC (libraries)

argon2-libs-20190702-r1 webpage:
https://github.com/P-H-C/phc-winner-argon2

argon2-libs-20190702-r1 installed size:
52 KiB

argon2-libs-20190702-r1 license:
Apache-2.0 CC0-1.0

```

### `apk` package: `bash`

```console
bash-5.1.8-r0 description:
The GNU Bourne Again shell

bash-5.1.8-r0 webpage:
https://www.gnu.org/software/bash/bash.html

bash-5.1.8-r0 installed size:
1296 KiB

bash-5.1.8-r0 license:
GPL-3.0-or-later

```

### `apk` package: `brotli-libs`

```console
brotli-libs-1.0.9-r5 description:
Generic lossless compressor (libraries)

brotli-libs-1.0.9-r5 webpage:
https://github.com/google/brotli

brotli-libs-1.0.9-r5 installed size:
720 KiB

brotli-libs-1.0.9-r5 license:
MIT

```

### `apk` package: `busybox`

```console
busybox-1.34.1-r3 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.34.1-r3 webpage:
https://busybox.net/

busybox-1.34.1-r3 installed size:
924 KiB

busybox-1.34.1-r3 license:
GPL-2.0-only

```

### `apk` package: `ca-certificates`

```console
ca-certificates-20191127-r7 description:
Common CA certificates PEM files from Mozilla

ca-certificates-20191127-r7 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-20191127-r7 installed size:
676 KiB

ca-certificates-20191127-r7 license:
MPL-2.0 AND MIT

```

### `apk` package: `ca-certificates-bundle`

```console
ca-certificates-bundle-20191127-r7 description:
Pre generated bundle of Mozilla certificates

ca-certificates-bundle-20191127-r7 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-bundle-20191127-r7 installed size:
228 KiB

ca-certificates-bundle-20191127-r7 license:
MPL-2.0 AND MIT

```

### `apk` package: `curl`

```console
curl-7.80.0-r0 description:
URL retrival utility and library

curl-7.80.0-r0 webpage:
https://curl.se/

curl-7.80.0-r0 installed size:
248 KiB

curl-7.80.0-r0 license:
MIT

```

### `apk` package: `gdbm`

```console
gdbm-1.22-r0 description:
GNU dbm is a set of database routines that use extensible hashing

gdbm-1.22-r0 webpage:
https://www.gnu.org/software/gdbm/

gdbm-1.22-r0 installed size:
88 KiB

gdbm-1.22-r0 license:
GPL-3.0-or-later

```

### `apk` package: `gmp`

```console
gmp-6.2.1-r0 description:
free library for arbitrary precision arithmetic

gmp-6.2.1-r0 webpage:
https://gmplib.org/

gmp-6.2.1-r0 installed size:
420 KiB

gmp-6.2.1-r0 license:
LGPL-3.0-or-later OR GPL-2.0-or-later

```

### `apk` package: `icu-libs`

```console
icu-libs-69.1-r1 description:
International Components for Unicode library (libraries)

icu-libs-69.1-r1 webpage:
https://icu.unicode.org/

icu-libs-69.1-r1 installed size:
31 MiB

icu-libs-69.1-r1 license:
MIT ICU Unicode-TOU

```

### `apk` package: `libacl`

```console
libacl-2.2.53-r0 description:
Dynamic library for access control list support

libacl-2.2.53-r0 webpage:
https://savannah.nongnu.org/projects/acl

libacl-2.2.53-r0 installed size:
44 KiB

libacl-2.2.53-r0 license:
LGPL-2.1-or-later AND GPL-2.0-or-later

```

### `apk` package: `libbz2`

```console
libbz2-1.0.8-r1 description:
Shared library for bz2

libbz2-1.0.8-r1 webpage:
http://sources.redhat.com/bzip2

libbz2-1.0.8-r1 installed size:
72 KiB

libbz2-1.0.8-r1 license:
bzip2-1.0.6

```

### `apk` package: `libc-utils`

```console
libc-utils-0.7.2-r3 description:
Meta package to pull in correct libc

libc-utils-0.7.2-r3 webpage:
https://alpinelinux.org

libc-utils-0.7.2-r3 installed size:
4096 B

libc-utils-0.7.2-r3 license:
BSD-2-Clause AND BSD-3-Clause

```

### `apk` package: `libcrypto1.1`

```console
libcrypto1.1-1.1.1l-r7 description:
Crypto library from openssl

libcrypto1.1-1.1.1l-r7 webpage:
https://www.openssl.org/

libcrypto1.1-1.1.1l-r7 installed size:
2676 KiB

libcrypto1.1-1.1.1l-r7 license:
OpenSSL

```

### `apk` package: `libcurl`

```console
libcurl-7.80.0-r0 description:
The multiprotocol file transfer library

libcurl-7.80.0-r0 webpage:
https://curl.se/

libcurl-7.80.0-r0 installed size:
504 KiB

libcurl-7.80.0-r0 license:
MIT

```

### `apk` package: `libgcc`

```console
libgcc-10.3.1_git20211027-r0 description:
GNU C compiler runtime libraries

libgcc-10.3.1_git20211027-r0 webpage:
https://gcc.gnu.org

libgcc-10.3.1_git20211027-r0 installed size:
112 KiB

libgcc-10.3.1_git20211027-r0 license:
GPL-2.0-or-later LGPL-2.1-or-later

```

### `apk` package: `libjpeg-turbo`

```console
libjpeg-turbo-2.1.2-r0 description:
Accelerated baseline JPEG compression and decompression library

libjpeg-turbo-2.1.2-r0 webpage:
https://libjpeg-turbo.org/

libjpeg-turbo-2.1.2-r0 installed size:
1140 KiB

libjpeg-turbo-2.1.2-r0 license:
BSD-3-Clause IJG Zlib

```

### `apk` package: `libldap`

```console
libldap-2.6.0-r0 description:
OpenLDAP libraries

libldap-2.6.0-r0 webpage:
https://www.openldap.org/

libldap-2.6.0-r0 installed size:
400 KiB

libldap-2.6.0-r0 license:
OLDAP-2.8

```

### `apk` package: `libmcrypt`

```console
libmcrypt-2.5.8-r9 description:
A library which provides a uniform interface to several symmetric encryption algorithms

libmcrypt-2.5.8-r9 webpage:
http://mcrypt.sourceforge.net/

libmcrypt-2.5.8-r9 installed size:
176 KiB

libmcrypt-2.5.8-r9 license:
LGPL-2.1-or-later

```

### `apk` package: `libmemcached-libs`

```console
libmemcached-libs-1.0.18-r4 description:
Client library and command line tools for memcached server (libraries)

libmemcached-libs-1.0.18-r4 webpage:
https://libmemcached.org/libMemcached.html

libmemcached-libs-1.0.18-r4 installed size:
328 KiB

libmemcached-libs-1.0.18-r4 license:
BSD-3-Clause

```

### `apk` package: `libpng`

```console
libpng-1.6.37-r1 description:
Portable Network Graphics library

libpng-1.6.37-r1 webpage:
http://www.libpng.org

libpng-1.6.37-r1 installed size:
204 KiB

libpng-1.6.37-r1 license:
Libpng

```

### `apk` package: `libpq`

```console
libpq-14.1-r4 description:
PostgreSQL client library

libpq-14.1-r4 webpage:
https://www.postgresql.org/

libpq-14.1-r4 installed size:
328 KiB

libpq-14.1-r4 license:
PostgreSQL

```

### `apk` package: `libretls`

```console
libretls-3.3.4-r2 description:
port of libtls from libressl to openssl

libretls-3.3.4-r2 webpage:
https://git.causal.agency/libretls/

libretls-3.3.4-r2 installed size:
84 KiB

libretls-3.3.4-r2 license:
ISC AND (BSD-3-Clause OR MIT)

```

### `apk` package: `libsasl`

```console
libsasl-2.1.27-r14 description:
Cyrus Simple Authentication and Security Layer (SASL) library

libsasl-2.1.27-r14 webpage:
https://www.cyrusimap.org/sasl/

libsasl-2.1.27-r14 installed size:
192 KiB

libsasl-2.1.27-r14 license:
custom

```

### `apk` package: `libsodium`

```console
libsodium-1.0.18-r0 description:
P(ortable|ackageable) NaCl-based crypto library

libsodium-1.0.18-r0 webpage:
https://github.com/jedisct1/libsodium

libsodium-1.0.18-r0 installed size:
340 KiB

libsodium-1.0.18-r0 license:
ISC

```

### `apk` package: `libssl1.1`

```console
libssl1.1-1.1.1l-r7 description:
SSL shared libraries

libssl1.1-1.1.1l-r7 webpage:
https://www.openssl.org/

libssl1.1-1.1.1l-r7 installed size:
528 KiB

libssl1.1-1.1.1l-r7 license:
OpenSSL

```

### `apk` package: `libstdc++`

```console
libstdc++-10.3.1_git20211027-r0 description:
GNU C++ standard runtime library

libstdc++-10.3.1_git20211027-r0 webpage:
https://gcc.gnu.org

libstdc++-10.3.1_git20211027-r0 installed size:
1664 KiB

libstdc++-10.3.1_git20211027-r0 license:
GPL-2.0-or-later LGPL-2.1-or-later

```

### `apk` package: `libxml2`

```console
libxml2-2.9.12-r2 description:
XML parsing library, version 2

libxml2-2.9.12-r2 webpage:
http://www.xmlsoft.org/

libxml2-2.9.12-r2 installed size:
1200 KiB

libxml2-2.9.12-r2 license:
MIT

```

### `apk` package: `libzip`

```console
libzip-1.8.0-r1 description:
C library for manipulating zip archives

libzip-1.8.0-r1 webpage:
https://libzip.org/

libzip-1.8.0-r1 installed size:
116 KiB

libzip-1.8.0-r1 license:
BSD-3-Clause

```

### `apk` package: `musl`

```console
musl-1.2.2-r7 description:
the musl c library (libc) implementation

musl-1.2.2-r7 webpage:
https://musl.libc.org/

musl-1.2.2-r7 installed size:
608 KiB

musl-1.2.2-r7 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.2.2-r7 description:
the musl c library (libc) implementation

musl-utils-1.2.2-r7 webpage:
https://musl.libc.org/

musl-utils-1.2.2-r7 installed size:
140 KiB

musl-utils-1.2.2-r7 license:
MIT BSD GPL2+

```

### `apk` package: `ncurses-libs`

```console
ncurses-libs-6.3_p20211120-r0 description:
Ncurses libraries

ncurses-libs-6.3_p20211120-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-libs-6.3_p20211120-r0 installed size:
500 KiB

ncurses-libs-6.3_p20211120-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.3_p20211120-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.3_p20211120-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-base-6.3_p20211120-r0 installed size:
216 KiB

ncurses-terminfo-base-6.3_p20211120-r0 license:
MIT

```

### `apk` package: `nghttp2-libs`

```console
nghttp2-libs-1.46.0-r0 description:
Experimental HTTP/2 client, server and proxy (libraries)

nghttp2-libs-1.46.0-r0 webpage:
https://nghttp2.org

nghttp2-libs-1.46.0-r0 installed size:
156 KiB

nghttp2-libs-1.46.0-r0 license:
MIT

```

### `apk` package: `oniguruma`

```console
oniguruma-6.9.7.1-r0 description:
a regular expressions library

oniguruma-6.9.7.1-r0 webpage:
https://github.com/kkos/oniguruma

oniguruma-6.9.7.1-r0 installed size:
560 KiB

oniguruma-6.9.7.1-r0 license:
BSD-2-Clause

```

### `apk` package: `openssl`

```console
openssl-1.1.1l-r7 description:
toolkit for transport layer security (TLS) - version 1.1

openssl-1.1.1l-r7 webpage:
https://www.openssl.org/

openssl-1.1.1l-r7 installed size:
660 KiB

openssl-1.1.1l-r7 license:
OpenSSL

```

### `apk` package: `readline`

```console
readline-8.1.1-r0 description:
GNU readline library

readline-8.1.1-r0 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.1.1-r0 installed size:
308 KiB

readline-8.1.1-r0 license:
GPL-2.0-or-later

```

### `apk` package: `scanelf`

```console
scanelf-1.3.3-r0 description:
Scan ELF binaries for stuff

scanelf-1.3.3-r0 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.3.3-r0 installed size:
92 KiB

scanelf-1.3.3-r0 license:
GPL-2.0-only

```

### `apk` package: `sqlite-libs`

```console
sqlite-libs-3.36.0-r0 description:
Sqlite3 library

sqlite-libs-3.36.0-r0 webpage:
https://www.sqlite.org/

sqlite-libs-3.36.0-r0 installed size:
968 KiB

sqlite-libs-3.36.0-r0 license:
blessing

```

### `apk` package: `ssl_client`

```console
ssl_client-1.34.1-r3 description:
EXternal ssl_client for busybox wget

ssl_client-1.34.1-r3 webpage:
https://busybox.net/

ssl_client-1.34.1-r3 installed size:
28 KiB

ssl_client-1.34.1-r3 license:
GPL-2.0-only

```

### `apk` package: `tar`

```console
tar-1.34-r0 description:
Utility used to store, backup, and transport files

tar-1.34-r0 webpage:
https://www.gnu.org/software/tar/

tar-1.34-r0 installed size:
488 KiB

tar-1.34-r0 license:
GPL-3.0-or-later

```

### `apk` package: `xz`

```console
xz-5.2.5-r0 description:
Library and CLI tools for XZ and LZMA compressed files

xz-5.2.5-r0 webpage:
https://tukaani.org/xz

xz-5.2.5-r0 installed size:
160 KiB

xz-5.2.5-r0 license:
GPL-2.0-or-later AND Public-Domain AND LGPL-2.1-or-later

```

### `apk` package: `xz-libs`

```console
xz-libs-5.2.5-r0 description:
Library and CLI tools for XZ and LZMA compressed files (libraries)

xz-libs-5.2.5-r0 webpage:
https://tukaani.org/xz

xz-libs-5.2.5-r0 installed size:
148 KiB

xz-libs-5.2.5-r0 license:
GPL-2.0-or-later AND Public-Domain AND LGPL-2.1-or-later

```

### `apk` package: `zlib`

```console
zlib-1.2.11-r3 description:
A compression/decompression Library

zlib-1.2.11-r3 webpage:
https://zlib.net/

zlib-1.2.11-r3 installed size:
108 KiB

zlib-1.2.11-r3 license:
Zlib

```

### `apk` package: `zstd-libs`

```console
zstd-libs-1.5.0-r0 description:
Zstandard - Fast real-time compression algorithm (libraries)

zstd-libs-1.5.0-r0 webpage:
https://www.zstd.net/

zstd-libs-1.5.0-r0 installed size:
1088 KiB

zstd-libs-1.5.0-r0 license:
BSD-3-Clause GPL-2.0-or-later

```
