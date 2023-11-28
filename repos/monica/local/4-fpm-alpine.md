# `monica:4.0.0-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:7eb3a24d802cecd17c300d29d3321956a0c6797c35e86a0919acb1baa653871a`
- Created: `2023-11-28T01:48:44.827015192Z`
- Virtual Size: ~ 236.95 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/usr/local/bin/entrypoint.sh"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_LDFLAGS=-Wl,-O1 -pie`
  - `GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD`
  - `PHP_VERSION=8.1.26`
  - `PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc`
  - `PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f`
  - `PHP_OPCACHE_VALIDATE_TIMESTAMPS=0`
  - `PHP_OPCACHE_MAX_ACCELERATED_FILES=20000`
  - `PHP_OPCACHE_MEMORY_CONSUMPTION=192`
  - `PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10`
  - `PHP_MEMORY_LIMIT=512M`
  - `PHP_UPLOAD_LIMIT=512M`
  - `MONICA_VERSION=v4.0.0`
- Labels:
  - `org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org>`
  - `org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you.`
  - `org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e`
  - `org.opencontainers.image.source=https://github.com/monicahq/docker`
  - `org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager`
  - `org.opencontainers.image.url=https://monicahq.com`
  - `org.opencontainers.image.vendor=Monica`
  - `org.opencontainers.image.version=v4.0.0`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.4.3-r1 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.4.3-r1 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.4.3-r1 installed size:
324 KiB

alpine-baselayout-3.4.3-r1 license:
GPL-2.0-only

```

### `apk` package: `alpine-baselayout-data`

```console
alpine-baselayout-data-3.4.3-r1 description:
Alpine base dir structure and init scripts

alpine-baselayout-data-3.4.3-r1 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-data-3.4.3-r1 installed size:
76 KiB

alpine-baselayout-data-3.4.3-r1 license:
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
apk-tools-2.14.0-r2 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.14.0-r2 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.14.0-r2 installed size:
304 KiB

apk-tools-2.14.0-r2 license:
GPL-2.0-only

```

### `apk` package: `argon2-libs`

```console
argon2-libs-20190702-r4 description:
The password hash Argon2, winner of PHC (libraries)

argon2-libs-20190702-r4 webpage:
https://github.com/P-H-C/phc-winner-argon2

argon2-libs-20190702-r4 installed size:
52 KiB

argon2-libs-20190702-r4 license:
Apache-2.0 OR CC0-1.0

```

### `apk` package: `bash`

```console
bash-5.2.15-r5 description:
The GNU Bourne Again shell

bash-5.2.15-r5 webpage:
https://www.gnu.org/software/bash/bash.html

bash-5.2.15-r5 installed size:
1360 KiB

bash-5.2.15-r5 license:
GPL-3.0-or-later

```

### `apk` package: `brotli-libs`

```console
brotli-libs-1.0.9-r14 description:
Generic lossless compressor (libraries)

brotli-libs-1.0.9-r14 webpage:
https://github.com/google/brotli

brotli-libs-1.0.9-r14 installed size:
788 KiB

brotli-libs-1.0.9-r14 license:
MIT

```

### `apk` package: `busybox`

```console
busybox-1.36.1-r2 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.36.1-r2 webpage:
https://busybox.net/

busybox-1.36.1-r2 installed size:
924 KiB

busybox-1.36.1-r2 license:
GPL-2.0-only

```

### `apk` package: `busybox-binsh`

```console
busybox-binsh-1.36.1-r2 description:
busybox ash /bin/sh

busybox-binsh-1.36.1-r2 webpage:
https://busybox.net/

busybox-binsh-1.36.1-r2 installed size:
8192 B

busybox-binsh-1.36.1-r2 license:
GPL-2.0-only

```

### `apk` package: `ca-certificates`

```console
ca-certificates-20230506-r0 description:
Common CA certificates PEM files from Mozilla

ca-certificates-20230506-r0 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-20230506-r0 installed size:
688 KiB

ca-certificates-20230506-r0 license:
MPL-2.0 AND MIT

```

### `apk` package: `ca-certificates-bundle`

```console
ca-certificates-bundle-20230506-r0 description:
Pre generated bundle of Mozilla certificates

ca-certificates-bundle-20230506-r0 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-bundle-20230506-r0 installed size:
232 KiB

ca-certificates-bundle-20230506-r0 license:
MPL-2.0 AND MIT

```

### `apk` package: `coreutils`

```console
coreutils-9.3-r1 description:
The basic file, shell and text manipulation utilities

coreutils-9.3-r1 webpage:
https://www.gnu.org/software/coreutils/

coreutils-9.3-r1 installed size:
1092 KiB

coreutils-9.3-r1 license:
GPL-3.0-or-later

```

### `apk` package: `curl`

```console
curl-8.4.0-r0 description:
URL retrival utility and library

curl-8.4.0-r0 webpage:
https://curl.se/

curl-8.4.0-r0 installed size:
248 KiB

curl-8.4.0-r0 license:
curl

```

### `apk` package: `freetype`

```console
freetype-2.13.0-r5 description:
TrueType font rendering library

freetype-2.13.0-r5 webpage:
https://www.freetype.org/

freetype-2.13.0-r5 installed size:
724 KiB

freetype-2.13.0-r5 license:
FTL OR GPL-2.0-or-later

```

### `apk` package: `gdbm`

```console
gdbm-1.23-r1 description:
GNU dbm is a set of database routines that use extensible hashing

gdbm-1.23-r1 webpage:
https://www.gnu.org/software/gdbm/

gdbm-1.23-r1 installed size:
88 KiB

gdbm-1.23-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gmp`

```console
gmp-6.2.1-r3 description:
free library for arbitrary precision arithmetic

gmp-6.2.1-r3 webpage:
https://gmplib.org/

gmp-6.2.1-r3 installed size:
420 KiB

gmp-6.2.1-r3 license:
LGPL-3.0-or-later OR GPL-2.0-or-later

```

### `apk` package: `gnu-libiconv-libs`

```console
gnu-libiconv-libs-1.17-r1 description:
GNU charset conversion library for libc which doesn't implement it (libraries)

gnu-libiconv-libs-1.17-r1 webpage:
https://www.gnu.org/software/libiconv

gnu-libiconv-libs-1.17-r1 installed size:
1064 KiB

gnu-libiconv-libs-1.17-r1 license:
LGPL-2.1-or-later

```

### `apk` package: `icu-data-en`

```console
icu-data-en-73.2-r2 description:
Stripped down ICU data with only en_US/GB locale and no legacy charset converters

icu-data-en-73.2-r2 webpage:
https://icu.unicode.org/

icu-data-en-73.2-r2 installed size:
3016 KiB

icu-data-en-73.2-r2 license:
ICU

```

### `apk` package: `icu-libs`

```console
icu-libs-73.2-r2 description:
International Components for Unicode library (libraries)

icu-libs-73.2-r2 webpage:
https://icu.unicode.org/

icu-libs-73.2-r2 installed size:
4332 KiB

icu-libs-73.2-r2 license:
ICU

```

### `apk` package: `libacl`

```console
libacl-2.3.1-r3 description:
Dynamic library for access control list support

libacl-2.3.1-r3 webpage:
https://savannah.nongnu.org/projects/acl

libacl-2.3.1-r3 installed size:
44 KiB

libacl-2.3.1-r3 license:
LGPL-2.1-or-later AND GPL-2.0-or-later

```

### `apk` package: `libattr`

```console
libattr-2.5.1-r4 description:
utilities for managing filesystem extended attributes (libraries)

libattr-2.5.1-r4 webpage:
https://savannah.nongnu.org/projects/attr

libattr-2.5.1-r4 installed size:
32 KiB

libattr-2.5.1-r4 license:
LGPL-2.1-or-later

```

### `apk` package: `libbz2`

```console
libbz2-1.0.8-r5 description:
Shared library for bz2

libbz2-1.0.8-r5 webpage:
https://sourceware.org/bzip2/

libbz2-1.0.8-r5 installed size:
88 KiB

libbz2-1.0.8-r5 license:
bzip2-1.0.6

```

### `apk` package: `libc-utils`

```console
libc-utils-0.7.2-r5 description:
Meta package to pull in correct libc

libc-utils-0.7.2-r5 webpage:
https://alpinelinux.org

libc-utils-0.7.2-r5 installed size:
4096 B

libc-utils-0.7.2-r5 license:
BSD-2-Clause AND BSD-3-Clause

```

### `apk` package: `libcrypto3`

```console
libcrypto3-3.1.4-r1 description:
Crypto library from openssl

libcrypto3-3.1.4-r1 webpage:
https://www.openssl.org/

libcrypto3-3.1.4-r1 installed size:
4472 KiB

libcrypto3-3.1.4-r1 license:
Apache-2.0

```

### `apk` package: `libcurl`

```console
libcurl-8.4.0-r0 description:
The multiprotocol file transfer library

libcurl-8.4.0-r0 webpage:
https://curl.se/

libcurl-8.4.0-r0 installed size:
584 KiB

libcurl-8.4.0-r0 license:
curl

```

### `apk` package: `libgcc`

```console
libgcc-12.2.1_git20220924-r10 description:
GNU C compiler runtime libraries

libgcc-12.2.1_git20220924-r10 webpage:
https://gcc.gnu.org

libgcc-12.2.1_git20220924-r10 installed size:
132 KiB

libgcc-12.2.1_git20220924-r10 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `libidn2`

```console
libidn2-2.3.4-r1 description:
Encode/Decode library for internationalized domain names

libidn2-2.3.4-r1 webpage:
https://www.gnu.org/software/libidn#libidn2

libidn2-2.3.4-r1 installed size:
208 KiB

libidn2-2.3.4-r1 license:
GPL-2.0-or-later AND LGPL-3.0-or-later

```

### `apk` package: `libjpeg-turbo`

```console
libjpeg-turbo-2.1.5.1-r3 description:
Accelerated baseline JPEG compression and decompression library

libjpeg-turbo-2.1.5.1-r3 webpage:
https://libjpeg-turbo.org/

libjpeg-turbo-2.1.5.1-r3 installed size:
1112 KiB

libjpeg-turbo-2.1.5.1-r3 license:
BSD-3-Clause AND IJG AND Zlib

```

### `apk` package: `libmemcached-libs`

```console
libmemcached-libs-1.1.4-r1 description:
Client library and command line tools for memcached server (resurrected) (libraries)

libmemcached-libs-1.1.4-r1 webpage:
https://github.com/awesomized/libmemcached

libmemcached-libs-1.1.4-r1 installed size:
264 KiB

libmemcached-libs-1.1.4-r1 license:
BSD-3-Clause

```

### `apk` package: `libncursesw`

```console
libncursesw-6.4_p20230506-r0 description:
Console display library (libncursesw)

libncursesw-6.4_p20230506-r0 webpage:
https://invisible-island.net/ncurses/

libncursesw-6.4_p20230506-r0 installed size:
344 KiB

libncursesw-6.4_p20230506-r0 license:
X11

```

### `apk` package: `libpng`

```console
libpng-1.6.39-r3 description:
Portable Network Graphics library

libpng-1.6.39-r3 webpage:
http://www.libpng.org

libpng-1.6.39-r3 installed size:
204 KiB

libpng-1.6.39-r3 license:
Libpng

```

### `apk` package: `libpq`

```console
libpq-15.5-r0 description:
PostgreSQL client library

libpq-15.5-r0 webpage:
https://www.postgresql.org/

libpq-15.5-r0 installed size:
320 KiB

libpq-15.5-r0 license:
PostgreSQL

```

### `apk` package: `libsasl`

```console
libsasl-2.1.28-r4 description:
Cyrus Simple Authentication and Security Layer (SASL) library

libsasl-2.1.28-r4 webpage:
https://www.cyrusimap.org/sasl/

libsasl-2.1.28-r4 installed size:
192 KiB

libsasl-2.1.28-r4 license:
custom

```

### `apk` package: `libsodium`

```console
libsodium-1.0.18-r3 description:
P(ortable|ackageable) NaCl-based crypto library

libsodium-1.0.18-r3 webpage:
https://github.com/jedisct1/libsodium

libsodium-1.0.18-r3 installed size:
336 KiB

libsodium-1.0.18-r3 license:
ISC

```

### `apk` package: `libssl3`

```console
libssl3-3.1.4-r1 description:
SSL shared libraries

libssl3-3.1.4-r1 webpage:
https://www.openssl.org/

libssl3-3.1.4-r1 installed size:
552 KiB

libssl3-3.1.4-r1 license:
Apache-2.0

```

### `apk` package: `libstdc++`

```console
libstdc++-12.2.1_git20220924-r10 description:
GNU C++ standard runtime library

libstdc++-12.2.1_git20220924-r10 webpage:
https://gcc.gnu.org

libstdc++-12.2.1_git20220924-r10 installed size:
2356 KiB

libstdc++-12.2.1_git20220924-r10 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `libunistring`

```console
libunistring-1.1-r1 description:
Library for manipulating Unicode strings and C strings

libunistring-1.1-r1 webpage:
https://www.gnu.org/software/libunistring/

libunistring-1.1-r1 installed size:
1696 KiB

libunistring-1.1-r1 license:
GPL-2.0-or-later OR LGPL-3.0-or-later

```

### `apk` package: `libwebp`

```console
libwebp-1.3.2-r0 description:
Libraries for working with WebP images

libwebp-1.3.2-r0 webpage:
https://developers.google.com/speed/webp

libwebp-1.3.2-r0 installed size:
596 KiB

libwebp-1.3.2-r0 license:
BSD-3-Clause

```

### `apk` package: `libxml2`

```console
libxml2-2.11.6-r0 description:
XML parsing library, version 2

libxml2-2.11.6-r0 webpage:
http://www.xmlsoft.org/

libxml2-2.11.6-r0 installed size:
1108 KiB

libxml2-2.11.6-r0 license:
MIT

```

### `apk` package: `libzip`

```console
libzip-1.9.2-r2 description:
C library for manipulating zip archives

libzip-1.9.2-r2 webpage:
https://libzip.org/

libzip-1.9.2-r2 installed size:
112 KiB

libzip-1.9.2-r2 license:
BSD-3-Clause

```

### `apk` package: `musl`

```console
musl-1.2.4-r2 description:
the musl c library (libc) implementation

musl-1.2.4-r2 webpage:
https://musl.libc.org/

musl-1.2.4-r2 installed size:
620 KiB

musl-1.2.4-r2 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.2.4-r1 description:
the musl c library (libc) implementation

musl-utils-1.2.4-r1 webpage:
https://musl.libc.org/

musl-utils-1.2.4-r1 installed size:
132 KiB

musl-utils-1.2.4-r1 license:
MIT AND BSD-2-Clause AND GPL-2.0-or-later

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.4_p20230506-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.4_p20230506-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-base-6.4_p20230506-r0 installed size:
216 KiB

ncurses-terminfo-base-6.4_p20230506-r0 license:
X11

```

### `apk` package: `nghttp2-libs`

```console
nghttp2-libs-1.57.0-r0 description:
Experimental HTTP/2 client, server and proxy (libraries)

nghttp2-libs-1.57.0-r0 webpage:
https://nghttp2.org

nghttp2-libs-1.57.0-r0 installed size:
152 KiB

nghttp2-libs-1.57.0-r0 license:
MIT

```

### `apk` package: `oniguruma`

```console
oniguruma-6.9.8-r1 description:
a regular expressions library

oniguruma-6.9.8-r1 webpage:
https://github.com/kkos/oniguruma

oniguruma-6.9.8-r1 installed size:
544 KiB

oniguruma-6.9.8-r1 license:
BSD-2-Clause

```

### `apk` package: `openssl`

```console
openssl-3.1.4-r1 description:
Toolkit for Transport Layer Security (TLS)

openssl-3.1.4-r1 webpage:
https://www.openssl.org/

openssl-3.1.4-r1 installed size:
752 KiB

openssl-3.1.4-r1 license:
Apache-2.0

```

### `apk` package: `readline`

```console
readline-8.2.1-r1 description:
GNU readline library

readline-8.2.1-r1 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.2.1-r1 installed size:
300 KiB

readline-8.2.1-r1 license:
GPL-2.0-or-later

```

### `apk` package: `scanelf`

```console
scanelf-1.3.7-r1 description:
Scan ELF binaries for stuff

scanelf-1.3.7-r1 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.3.7-r1 installed size:
88 KiB

scanelf-1.3.7-r1 license:
GPL-2.0-only

```

### `apk` package: `skalibs`

```console
skalibs-2.13.1.1-r1 description:
Set of general-purpose C programming libraries for skarnet.org software.

skalibs-2.13.1.1-r1 webpage:
https://skarnet.org/software/skalibs/

skalibs-2.13.1.1-r1 installed size:
196 KiB

skalibs-2.13.1.1-r1 license:
ISC

```

### `apk` package: `sqlite-libs`

```console
sqlite-libs-3.41.2-r2 description:
C library that implements an SQL database engine (libraries)

sqlite-libs-3.41.2-r2 webpage:
https://www.sqlite.org/

sqlite-libs-3.41.2-r2 installed size:
976 KiB

sqlite-libs-3.41.2-r2 license:
blessing

```

### `apk` package: `ssl_client`

```console
ssl_client-1.36.1-r2 description:
EXternal ssl_client for busybox wget

ssl_client-1.36.1-r2 webpage:
https://busybox.net/

ssl_client-1.36.1-r2 installed size:
28 KiB

ssl_client-1.36.1-r2 license:
GPL-2.0-only

```

### `apk` package: `tar`

```console
tar-1.34-r3 description:
Utility used to store, backup, and transport files

tar-1.34-r3 webpage:
https://www.gnu.org/software/tar/

tar-1.34-r3 installed size:
468 KiB

tar-1.34-r3 license:
GPL-3.0-or-later

```

### `apk` package: `utmps-libs`

```console
utmps-libs-0.1.2.1-r1 description:
A secure utmp/wtmp implementation (libraries)

utmps-libs-0.1.2.1-r1 webpage:
https://skarnet.org/software/utmps/

utmps-libs-0.1.2.1-r1 installed size:
24 KiB

utmps-libs-0.1.2.1-r1 license:
ISC

```

### `apk` package: `xz`

```console
xz-5.4.3-r0 description:
Library and CLI tools for XZ and LZMA compressed files

xz-5.4.3-r0 webpage:
https://tukaani.org/xz

xz-5.4.3-r0 installed size:
172 KiB

xz-5.4.3-r0 license:
GPL-2.0-or-later AND Public-Domain AND LGPL-2.1-or-later

```

### `apk` package: `xz-libs`

```console
xz-libs-5.4.3-r0 description:
Library and CLI tools for XZ and LZMA compressed files (libraries)

xz-libs-5.4.3-r0 webpage:
https://tukaani.org/xz

xz-libs-5.4.3-r0 installed size:
232 KiB

xz-libs-5.4.3-r0 license:
GPL-2.0-or-later AND Public-Domain AND LGPL-2.1-or-later

```

### `apk` package: `zlib`

```console
zlib-1.2.13-r1 description:
A compression/decompression Library

zlib-1.2.13-r1 webpage:
https://zlib.net/

zlib-1.2.13-r1 installed size:
108 KiB

zlib-1.2.13-r1 license:
Zlib

```

### `apk` package: `zstd-libs`

```console
zstd-libs-1.5.5-r4 description:
Zstandard - Fast real-time compression algorithm (libraries)

zstd-libs-1.5.5-r4 webpage:
https://www.zstd.net/

zstd-libs-1.5.5-r4 installed size:
736 KiB

zstd-libs-1.5.5-r4 license:
BSD-3-Clause GPL-2.0-or-later

```
