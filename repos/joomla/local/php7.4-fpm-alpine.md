# `joomla:3.9.24-php7.4-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:26228f2da6fcd0aeb2b78fe590ae276acbd8864f0ed93f74526010d0e68cd643`
- Created: `2021-02-18T07:32:35.171700553Z`
- Virtual Size: ~ 136.23 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/entrypoint.sh"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_LDFLAGS=-Wl,-O1 -pie`
  - `GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312`
  - `PHP_VERSION=7.4.15`
  - `PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc`
  - `PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8`
  - `JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1`
  - `JOOMLA_VERSION=3.9.24`
  - `JOOMLA_SHA512=0c34ea3334c613c3ae30f7ce60a808643a136920e108dcaad278d77cf3036a0ace92e30fb31f8ae9addcf6fc954655339d7abe9bc3de0b7f7032bf6429300888`
- Labels:
  - `maintainer=Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.2.0-r8 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.2.0-r8 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.2.0-r8 installed size:
409600

alpine-baselayout-3.2.0-r8 license:
GPL-2.0-only

```

### `apk` package: `alpine-keys`

```console
alpine-keys-2.2-r0 description:
Public keys for Alpine Linux packages

alpine-keys-2.2-r0 webpage:
https://alpinelinux.org

alpine-keys-2.2-r0 installed size:
106496

alpine-keys-2.2-r0 license:
MIT

```

### `apk` package: `apk-tools`

```console
apk-tools-2.12.1-r0 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.12.1-r0 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.12.1-r0 installed size:
311296

apk-tools-2.12.1-r0 license:
GPL-2.0-only

```

### `apk` package: `argon2-libs`

```console
argon2-libs-20190702-r1 description:
The password hash Argon2, winner of PHC (libraries)

argon2-libs-20190702-r1 webpage:
https://github.com/P-H-C/phc-winner-argon2

argon2-libs-20190702-r1 installed size:
53248

argon2-libs-20190702-r1 license:
Apache-2.0 CC0-1.0

```

### `apk` package: `bash`

```console
bash-5.1.0-r0 description:
The GNU Bourne Again shell

bash-5.1.0-r0 webpage:
https://www.gnu.org/software/bash/bash.html

bash-5.1.0-r0 installed size:
1327104

bash-5.1.0-r0 license:
GPL-3.0-or-later

```

### `apk` package: `brotli-libs`

```console
brotli-libs-1.0.9-r3 description:
Generic lossless compressor (libraries)

brotli-libs-1.0.9-r3 webpage:
https://github.com/google/brotli

brotli-libs-1.0.9-r3 installed size:
737280

brotli-libs-1.0.9-r3 license:
MIT

```

### `apk` package: `busybox`

```console
busybox-1.32.1-r3 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.32.1-r3 webpage:
https://busybox.net/

busybox-1.32.1-r3 installed size:
946176

busybox-1.32.1-r3 license:
GPL-2.0-only

```

### `apk` package: `ca-certificates`

```console
ca-certificates-20191127-r5 description:
Common CA certificates PEM files from Mozilla

ca-certificates-20191127-r5 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-20191127-r5 installed size:
688128

ca-certificates-20191127-r5 license:
MPL-2.0 AND MIT

```

### `apk` package: `ca-certificates-bundle`

```console
ca-certificates-bundle-20191127-r5 description:
Pre generated bundle of Mozilla certificates

ca-certificates-bundle-20191127-r5 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-bundle-20191127-r5 installed size:
233472

ca-certificates-bundle-20191127-r5 license:
MPL-2.0 AND MIT

```

### `apk` package: `curl`

```console
curl-7.74.0-r0 description:
URL retrival utility and library

curl-7.74.0-r0 webpage:
https://curl.haxx.se/

curl-7.74.0-r0 installed size:
245760

curl-7.74.0-r0 license:
MIT

```

### `apk` package: `gdbm`

```console
gdbm-1.19-r0 description:
GNU dbm is a set of database routines that use extensible hashing

gdbm-1.19-r0 webpage:
https://www.gnu.org/software/gdbm/

gdbm-1.19-r0 installed size:
229376

gdbm-1.19-r0 license:
GPL-3.0-or-later

```

### `apk` package: `gmp`

```console
gmp-6.2.1-r0 description:
free library for arbitrary precision arithmetic

gmp-6.2.1-r0 webpage:
https://gmplib.org/

gmp-6.2.1-r0 installed size:
425984

gmp-6.2.1-r0 license:
LGPL-3.0-or-later OR GPL-2.0-or-later

```

### `apk` package: `libacl`

```console
libacl-2.2.53-r0 description:
Dynamic library for access control list support

libacl-2.2.53-r0 webpage:
https://savannah.nongnu.org/projects/acl

libacl-2.2.53-r0 installed size:
45056

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
73728

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
4096

libc-utils-0.7.2-r3 license:
BSD-2-Clause AND BSD-3-Clause

```

### `apk` package: `libcrypto1.1`

```console
libcrypto1.1-1.1.1j-r0 description:
Crypto library from openssl

libcrypto1.1-1.1.1j-r0 webpage:
https://www.openssl.org/

libcrypto1.1-1.1.1j-r0 installed size:
2768896

libcrypto1.1-1.1.1j-r0 license:
OpenSSL

```

### `apk` package: `libcurl`

```console
libcurl-7.74.0-r0 description:
The multiprotocol file transfer library

libcurl-7.74.0-r0 webpage:
https://curl.haxx.se/

libcurl-7.74.0-r0 installed size:
495616

libcurl-7.74.0-r0 license:
MIT

```

### `apk` package: `libedit`

```console
libedit-20191231.3.1-r1 description:
BSD line editing library

libedit-20191231.3.1-r1 webpage:
https://www.thrysoee.dk/editline

libedit-20191231.3.1-r1 installed size:
200704

libedit-20191231.3.1-r1 license:
BSD-3-Clause

```

### `apk` package: `libgcc`

```console
libgcc-10.2.1_pre1-r3 description:
GNU C compiler runtime libraries

libgcc-10.2.1_pre1-r3 webpage:
https://gcc.gnu.org

libgcc-10.2.1_pre1-r3 installed size:
114688

libgcc-10.2.1_pre1-r3 license:
GPL-2.0-or-later LGPL-2.1-or-later

```

### `apk` package: `libjpeg-turbo`

```console
libjpeg-turbo-2.0.6-r0 description:
Accelerated baseline JPEG compression and decompression library

libjpeg-turbo-2.0.6-r0 webpage:
https://libjpeg-turbo.org/

libjpeg-turbo-2.0.6-r0 installed size:
1056768

libjpeg-turbo-2.0.6-r0 license:
BSD-3-Clause IJG Zlib

```

### `apk` package: `libldap`

```console
libldap-2.4.57-r0 description:
OpenLDAP libraries

libldap-2.4.57-r0 webpage:
https://www.openldap.org/

libldap-2.4.57-r0 installed size:
630784

libldap-2.4.57-r0 license:
custom

```

### `apk` package: `libmcrypt`

```console
libmcrypt-2.5.8-r9 description:
A library which provides a uniform interface to several symmetric encryption algorithms

libmcrypt-2.5.8-r9 webpage:
http://mcrypt.sourceforge.net/

libmcrypt-2.5.8-r9 installed size:
180224

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
335872

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
208896

libpng-1.6.37-r1 license:
Libpng

```

### `apk` package: `libpq`

```console
libpq-13.1-r2 description:
PostgreSQL libraries

libpq-13.1-r2 webpage:
https://www.postgresql.org/

libpq-13.1-r2 installed size:
335872

libpq-13.1-r2 license:
PostgreSQL

```

### `apk` package: `libsasl`

```console
libsasl-2.1.27-r10 description:
Cyrus Simple Authentication and Security Layer (SASL) library

libsasl-2.1.27-r10 webpage:
https://www.cyrusimap.org/sasl/

libsasl-2.1.27-r10 installed size:
196608

libsasl-2.1.27-r10 license:
custom

```

### `apk` package: `libsodium`

```console
libsodium-1.0.18-r0 description:
P(ortable|ackageable) NaCl-based crypto library

libsodium-1.0.18-r0 webpage:
https://github.com/jedisct1/libsodium

libsodium-1.0.18-r0 installed size:
348160

libsodium-1.0.18-r0 license:
ISC

```

### `apk` package: `libssl1.1`

```console
libssl1.1-1.1.1j-r0 description:
SSL shared libraries

libssl1.1-1.1.1j-r0 webpage:
https://www.openssl.org/

libssl1.1-1.1.1j-r0 installed size:
540672

libssl1.1-1.1.1j-r0 license:
OpenSSL

```

### `apk` package: `libstdc++`

```console
libstdc++-10.2.1_pre1-r3 description:
GNU C++ standard runtime library

libstdc++-10.2.1_pre1-r3 webpage:
https://gcc.gnu.org

libstdc++-10.2.1_pre1-r3 installed size:
1708032

libstdc++-10.2.1_pre1-r3 license:
GPL-2.0-or-later LGPL-2.1-or-later

```

### `apk` package: `libtls-standalone`

```console
libtls-standalone-2.9.1-r1 description:
libtls extricated from libressl sources

libtls-standalone-2.9.1-r1 webpage:
https://www.libressl.org/

libtls-standalone-2.9.1-r1 installed size:
110592

libtls-standalone-2.9.1-r1 license:
ISC

```

### `apk` package: `libxml2`

```console
libxml2-2.9.10-r6 description:
XML parsing library, version 2

libxml2-2.9.10-r6 webpage:
http://www.xmlsoft.org/

libxml2-2.9.10-r6 installed size:
1224704

libxml2-2.9.10-r6 license:
MIT

```

### `apk` package: `libzip`

```console
libzip-1.7.3-r2 description:
C library for manipulating zip archives

libzip-1.7.3-r2 webpage:
http://www.nih.at/libzip/index.html

libzip-1.7.3-r2 installed size:
110592

libzip-1.7.3-r2 license:
BSD-3-Clause

```

### `apk` package: `musl`

```console
musl-1.2.2-r0 description:
the musl c library (libc) implementation

musl-1.2.2-r0 webpage:
https://musl.libc.org/

musl-1.2.2-r0 installed size:
622592

musl-1.2.2-r0 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.2.2-r0 description:
the musl c library (libc) implementation

musl-utils-1.2.2-r0 webpage:
https://musl.libc.org/

musl-utils-1.2.2-r0 installed size:
143360

musl-utils-1.2.2-r0 license:
MIT BSD GPL2+

```

### `apk` package: `ncurses-libs`

```console
ncurses-libs-6.2_p20210109-r0 description:
Ncurses libraries

ncurses-libs-6.2_p20210109-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-libs-6.2_p20210109-r0 installed size:
507904

ncurses-libs-6.2_p20210109-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.2_p20210109-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.2_p20210109-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-base-6.2_p20210109-r0 installed size:
221184

ncurses-terminfo-base-6.2_p20210109-r0 license:
MIT

```

### `apk` package: `nghttp2-libs`

```console
nghttp2-libs-1.42.0-r1 description:
Experimental HTTP/2 client, server and proxy (libraries)

nghttp2-libs-1.42.0-r1 webpage:
https://nghttp2.org

nghttp2-libs-1.42.0-r1 installed size:
172032

nghttp2-libs-1.42.0-r1 license:
MIT

```

### `apk` package: `oniguruma`

```console
oniguruma-6.9.6-r0 description:
a regular expressions library

oniguruma-6.9.6-r0 webpage:
https://github.com/kkos/oniguruma

oniguruma-6.9.6-r0 installed size:
569344

oniguruma-6.9.6-r0 license:
BSD-2-Clause

```

### `apk` package: `openssl`

```console
openssl-1.1.1j-r0 description:
Toolkit for Transport Layer Security (TLS)

openssl-1.1.1j-r0 webpage:
https://www.openssl.org/

openssl-1.1.1j-r0 installed size:
675840

openssl-1.1.1j-r0 license:
OpenSSL

```

### `apk` package: `readline`

```console
readline-8.1.0-r0 description:
GNU readline library

readline-8.1.0-r0 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.1.0-r0 installed size:
315392

readline-8.1.0-r0 license:
GPL-2.0-or-later

```

### `apk` package: `scanelf`

```console
scanelf-1.2.8-r0 description:
Scan ELF binaries for stuff

scanelf-1.2.8-r0 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.2.8-r0 installed size:
94208

scanelf-1.2.8-r0 license:
GPL-2.0-only

```

### `apk` package: `sqlite-libs`

```console
sqlite-libs-3.34.1-r0 description:
Sqlite3 library

sqlite-libs-3.34.1-r0 webpage:
https://www.sqlite.org/

sqlite-libs-3.34.1-r0 installed size:
970752

sqlite-libs-3.34.1-r0 license:
Public-Domain

```

### `apk` package: `ssl_client`

```console
ssl_client-1.32.1-r3 description:
EXternal ssl_client for busybox wget

ssl_client-1.32.1-r3 webpage:
https://busybox.net/

ssl_client-1.32.1-r3 installed size:
28672

ssl_client-1.32.1-r3 license:
GPL-2.0-only

```

### `apk` package: `tar`

```console
tar-1.33-r1 description:
Utility used to store, backup, and transport files

tar-1.33-r1 webpage:
https://www.gnu.org/software/tar/

tar-1.33-r1 installed size:
499712

tar-1.33-r1 license:
GPL-3.0-or-later

```

### `apk` package: `xz`

```console
xz-5.2.5-r0 description:
Library and CLI tools for XZ and LZMA compressed files

xz-5.2.5-r0 webpage:
https://tukaani.org/xz

xz-5.2.5-r0 installed size:
163840

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
151552

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
110592

zlib-1.2.11-r3 license:
Zlib

```
