# `matomo:3.13.3-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:bb4e82cc3a3b348dfb5f05581aa0a29f9ba57c936b564ce9cc9ae886437c2b60`
- Created: `2020-02-25T01:32:54.026859148Z`
- Virtual Size: ~ 145.04 Mb  
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
  - `PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie`
  - `GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312`
  - `PHP_VERSION=7.4.3`
  - `PHP_URL=https://www.php.net/get/php-7.4.3.tar.xz/from/this/mirror`
  - `PHP_ASC_URL=https://www.php.net/get/php-7.4.3.tar.xz.asc/from/this/mirror`
  - `PHP_SHA256=cf1f856d877c268124ded1ede40c9fb6142b125fdaafdc54f855120b8bc6982a`
  - `PHP_MD5=`
  - `MATOMO_VERSION=3.13.3`
- Labels:
  - `maintainer=pierre@piwik.org`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.2.0-r3 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.2.0-r3 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.2.0-r3 installed size:
413696

alpine-baselayout-3.2.0-r3 license:
GPL-2.0-only

```

### `apk` package: `alpine-keys`

```console
alpine-keys-2.1-r2 description:
Public keys for Alpine Linux packages

alpine-keys-2.1-r2 webpage:
https://alpinelinux.org

alpine-keys-2.1-r2 installed size:
98304

alpine-keys-2.1-r2 license:
MIT

```

### `apk` package: `apk-tools`

```console
apk-tools-2.10.4-r3 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.10.4-r3 webpage:
https://git.alpinelinux.org/cgit/apk-tools/

apk-tools-2.10.4-r3 installed size:
262144

apk-tools-2.10.4-r3 license:
GPL2

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

### `apk` package: `busybox`

```console
busybox-1.31.1-r9 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.31.1-r9 webpage:
https://busybox.net/

busybox-1.31.1-r9 installed size:
962560

busybox-1.31.1-r9 license:
GPL-2.0-only

```

### `apk` package: `ca-certificates`

```console
ca-certificates-20191127-r0 description:
Common CA certificates PEM files

ca-certificates-20191127-r0 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-20191127-r0 installed size:
741376

ca-certificates-20191127-r0 license:
MPL-2.0 GPL-2.0-or-later

```

### `apk` package: `ca-certificates-cacert`

```console
ca-certificates-cacert-20191127-r0 description:
Mozilla bundled certificates

ca-certificates-cacert-20191127-r0 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-cacert-20191127-r0 installed size:
245760

ca-certificates-cacert-20191127-r0 license:
MPL-2.0 GPL-2.0-or-later

```

### `apk` package: `curl`

```console
curl-7.67.0-r0 description:
URL retrival utility and library

curl-7.67.0-r0 webpage:
https://curl.haxx.se/

curl-7.67.0-r0 installed size:
225280

curl-7.67.0-r0 license:
MIT

```

### `apk` package: `db`

```console
db-5.3.28-r1 description:
The Berkeley DB embedded database system

db-5.3.28-r1 webpage:
https://www.oracle.com/technology/software/products/berkeley-db/index.html

db-5.3.28-r1 installed size:
1564672

db-5.3.28-r1 license:
custom

```

### `apk` package: `freetype`

```console
freetype-2.10.1-r0 description:
TrueType font rendering library

freetype-2.10.1-r0 webpage:
https://www.freetype.org/

freetype-2.10.1-r0 installed size:
737280

freetype-2.10.1-r0 license:
FTL GPL-2.0-or-later

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
libc-utils-0.7.2-r0 description:
Meta package to pull in correct libc

libc-utils-0.7.2-r0 webpage:
http://alpinelinux.org

libc-utils-0.7.2-r0 installed size:
4096

libc-utils-0.7.2-r0 license:
BSD

```

### `apk` package: `libcrypto1.1`

```console
libcrypto1.1-1.1.1d-r3 description:
Crypto library from openssl

libcrypto1.1-1.1.1d-r3 webpage:
https://www.openssl.org

libcrypto1.1-1.1.1d-r3 installed size:
2748416

libcrypto1.1-1.1.1d-r3 license:
OpenSSL

```

### `apk` package: `libcurl`

```console
libcurl-7.67.0-r0 description:
The multiprotocol file transfer library

libcurl-7.67.0-r0 webpage:
https://curl.haxx.se/

libcurl-7.67.0-r0 installed size:
458752

libcurl-7.67.0-r0 license:
MIT

```

### `apk` package: `libedit`

```console
libedit-20191211.3.1-r0 description:
BSD line editing library

libedit-20191211.3.1-r0 webpage:
https://www.thrysoee.dk/editline

libedit-20191211.3.1-r0 installed size:
200704

libedit-20191211.3.1-r0 license:
BSD-3-Clause

```

### `apk` package: `libjpeg-turbo`

```console
libjpeg-turbo-2.0.4-r0 description:
Accelerated baseline JPEG compression and decompression library

libjpeg-turbo-2.0.4-r0 webpage:
https://libjpeg-turbo.org/

libjpeg-turbo-2.0.4-r0 installed size:
1355776

libjpeg-turbo-2.0.4-r0 license:
BSD-3-Clause IJG Zlib

```

### `apk` package: `libldap`

```console
libldap-2.4.48-r1 description:
OpenLDAP libraries

libldap-2.4.48-r1 webpage:
http://www.openldap.org/

libldap-2.4.48-r1 installed size:
626688

libldap-2.4.48-r1 license:
custom

```

### `apk` package: `libpng`

```console
libpng-1.6.37-r1 description:
Portable Network Graphics library

libpng-1.6.37-r1 webpage:
http://www.libpng.org

libpng-1.6.37-r1 installed size:
204800

libpng-1.6.37-r1 license:
Libpng

```

### `apk` package: `libsasl`

```console
libsasl-2.1.27-r5 description:
Cyrus Simple Authentication and Security Layer (SASL) library

libsasl-2.1.27-r5 webpage:
https://cyrusimap.org/

libsasl-2.1.27-r5 installed size:
180224

libsasl-2.1.27-r5 license:
custom

```

### `apk` package: `libsodium`

```console
libsodium-1.0.18-r0 description:
P(ortable|ackageable) NaCl-based crypto library

libsodium-1.0.18-r0 webpage:
https://github.com/jedisct1/libsodium

libsodium-1.0.18-r0 installed size:
344064

libsodium-1.0.18-r0 license:
ISC

```

### `apk` package: `libssl1.1`

```console
libssl1.1-1.1.1d-r3 description:
SSL shared libraries

libssl1.1-1.1.1d-r3 webpage:
https://www.openssl.org

libssl1.1-1.1.1d-r3 installed size:
536576

libssl1.1-1.1.1d-r3 license:
OpenSSL

```

### `apk` package: `libtls-standalone`

```console
libtls-standalone-2.9.1-r0 description:
libtls extricated from libressl sources

libtls-standalone-2.9.1-r0 webpage:
https://www.libressl.org/

libtls-standalone-2.9.1-r0 installed size:
110592

libtls-standalone-2.9.1-r0 license:
ISC

```

### `apk` package: `libxml2`

```console
libxml2-2.9.10-r2 description:
XML parsing library, version 2

libxml2-2.9.10-r2 webpage:
http://www.xmlsoft.org/

libxml2-2.9.10-r2 installed size:
1220608

libxml2-2.9.10-r2 license:
MIT

```

### `apk` package: `libzip`

```console
libzip-1.5.2-r0 description:
C library for manipulating zip archives

libzip-1.5.2-r0 webpage:
http://www.nih.at/libzip/index.html

libzip-1.5.2-r0 installed size:
122880

libzip-1.5.2-r0 license:
BSD-3-Clause

```

### `apk` package: `musl`

```console
musl-1.1.24-r0 description:
the musl c library (libc) implementation

musl-1.1.24-r0 webpage:
http://www.musl-libc.org/

musl-1.1.24-r0 installed size:
610304

musl-1.1.24-r0 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.1.24-r0 description:
the musl c library (libc) implementation

musl-utils-1.1.24-r0 webpage:
http://www.musl-libc.org/

musl-utils-1.1.24-r0 installed size:
147456

musl-utils-1.1.24-r0 license:
MIT BSD GPL2+

```

### `apk` package: `ncurses-libs`

```console
ncurses-libs-6.1_p20191130-r0 description:
Ncurses libraries

ncurses-libs-6.1_p20191130-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-libs-6.1_p20191130-r0 installed size:
507904

ncurses-libs-6.1_p20191130-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo`

```console
ncurses-terminfo-6.1_p20191130-r0 description:
Console display library (other terminfo files)

ncurses-terminfo-6.1_p20191130-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-6.1_p20191130-r0 installed size:
7348224

ncurses-terminfo-6.1_p20191130-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.1_p20191130-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.1_p20191130-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-base-6.1_p20191130-r0 installed size:
94208

ncurses-terminfo-base-6.1_p20191130-r0 license:
MIT

```

### `apk` package: `nghttp2-libs`

```console
nghttp2-libs-1.40.0-r0 description:
Experimental HTTP/2 client, server and proxy (libraries)

nghttp2-libs-1.40.0-r0 webpage:
https://nghttp2.org

nghttp2-libs-1.40.0-r0 installed size:
159744

nghttp2-libs-1.40.0-r0 license:
MIT

```

### `apk` package: `oniguruma`

```console
oniguruma-6.9.4-r0 description:
a regular expressions library

oniguruma-6.9.4-r0 webpage:
https://github.com/kkos/oniguruma

oniguruma-6.9.4-r0 installed size:
561152

oniguruma-6.9.4-r0 license:
BSD-2-Clause

```

### `apk` package: `openssl`

```console
openssl-1.1.1d-r3 description:
Toolkit for Transport Layer Security (TLS)

openssl-1.1.1d-r3 webpage:
https://www.openssl.org

openssl-1.1.1d-r3 installed size:
675840

openssl-1.1.1d-r3 license:
OpenSSL

```

### `apk` package: `scanelf`

```console
scanelf-1.2.4-r0 description:
Scan ELF binaries for stuff

scanelf-1.2.4-r0 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.2.4-r0 installed size:
94208

scanelf-1.2.4-r0 license:
GPL-2.0-only

```

### `apk` package: `sqlite-libs`

```console
sqlite-libs-3.30.1-r1 description:
Sqlite3 library

sqlite-libs-3.30.1-r1 webpage:
https://www.sqlite.org/

sqlite-libs-3.30.1-r1 installed size:
937984

sqlite-libs-3.30.1-r1 license:
Public-Domain

```

### `apk` package: `ssl_client`

```console
ssl_client-1.31.1-r9 description:
EXternal ssl_client for busybox wget

ssl_client-1.31.1-r9 webpage:
https://busybox.net/

ssl_client-1.31.1-r9 installed size:
28672

ssl_client-1.31.1-r9 license:
GPL-2.0-only

```

### `apk` package: `tar`

```console
tar-1.32-r1 description:
Utility used to store, backup, and transport files

tar-1.32-r1 webpage:
https://www.gnu.org/software/tar/

tar-1.32-r1 installed size:
499712

tar-1.32-r1 license:
GPL-3.0-or-later

```

### `apk` package: `xz`

```console
xz-5.2.4-r0 description:
Library and CLI tools for XZ and LZMA compressed files

xz-5.2.4-r0 webpage:
https://tukaani.org/xz

xz-5.2.4-r0 installed size:
163840

xz-5.2.4-r0 license:
GPL-2.0-or-later Public-Domain

```

### `apk` package: `xz-libs`

```console
xz-libs-5.2.4-r0 description:
Library and CLI tools for XZ and LZMA compressed files (libraries)

xz-libs-5.2.4-r0 webpage:
https://tukaani.org/xz

xz-libs-5.2.4-r0 installed size:
151552

xz-libs-5.2.4-r0 license:
GPL-2.0-or-later Public-Domain

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
