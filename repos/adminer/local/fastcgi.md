# `adminer:4.8.1-fastcgi`

## Docker Metadata

- Image ID: `sha256:c0f42d5c2fff321cfa172109e25111844d4855f85d29d1cbaf3a0e083c404eed`
- Created: `2021-06-01T23:19:30.038179083Z`
- Virtual Size: ~ 89.86 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
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
  - `PHP_VERSION=7.4.19`
  - `PHP_URL=https://www.php.net/distributions/php-7.4.19.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-7.4.19.tar.xz.asc`
  - `PHP_SHA256=6c17172c4a411ccb694d9752de899bb63c72a0a3ebe5089116bc13658a1467b2`
  - `ADMINER_VERSION=4.8.1`
  - `ADMINER_DOWNLOAD_SHA256=2fd7e6d8f987b243ab1839249551f62adce19704c47d3d0c8dd9e57ea5b9c6b3`
  - `ADMINER_SRC_DOWNLOAD_SHA256=ef832414296d11eed33e9d85fff3fb316c63f13f05fceb4a961cbe4cb2ae8712`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.2.0-r8 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.2.0-r8 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.2.0-r8 installed size:
400 KiB

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
104 KiB

alpine-keys-2.2-r0 license:
MIT

```

### `apk` package: `apk-tools`

```console
apk-tools-2.12.5-r0 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.12.5-r0 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.12.5-r0 installed size:
304 KiB

apk-tools-2.12.5-r0 license:
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

### `apk` package: `brotli-libs`

```console
brotli-libs-1.0.9-r3 description:
Generic lossless compressor (libraries)

brotli-libs-1.0.9-r3 webpage:
https://github.com/google/brotli

brotli-libs-1.0.9-r3 installed size:
720 KiB

brotli-libs-1.0.9-r3 license:
MIT

```

### `apk` package: `busybox`

```console
busybox-1.32.1-r6 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.32.1-r6 webpage:
https://busybox.net/

busybox-1.32.1-r6 installed size:
924 KiB

busybox-1.32.1-r6 license:
GPL-2.0-only

```

### `apk` package: `ca-certificates`

```console
ca-certificates-20191127-r5 description:
Common CA certificates PEM files from Mozilla

ca-certificates-20191127-r5 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-20191127-r5 installed size:
672 KiB

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
228 KiB

ca-certificates-bundle-20191127-r5 license:
MPL-2.0 AND MIT

```

### `apk` package: `curl`

```console
curl-7.76.1-r0 description:
URL retrival utility and library

curl-7.76.1-r0 webpage:
https://curl.se/

curl-7.76.1-r0 installed size:
244 KiB

curl-7.76.1-r0 license:
MIT

```

### `apk` package: `freetds`

```console
freetds-1.2.18-r0 description:
Tabular Datastream Library

freetds-1.2.18-r0 webpage:
https://www.freetds.org/

freetds-1.2.18-r0 installed size:
1840 KiB

freetds-1.2.18-r0 license:
GPL-2.0-or-later OR LGPL-2.0-or-later

```

### `apk` package: `gdbm`

```console
gdbm-1.19-r0 description:
GNU dbm is a set of database routines that use extensible hashing

gdbm-1.19-r0 webpage:
https://www.gnu.org/software/gdbm/

gdbm-1.19-r0 installed size:
224 KiB

gdbm-1.19-r0 license:
GPL-3.0-or-later

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
libcrypto1.1-1.1.1k-r0 description:
Crypto library from openssl

libcrypto1.1-1.1.1k-r0 webpage:
https://www.openssl.org/

libcrypto1.1-1.1.1k-r0 installed size:
2704 KiB

libcrypto1.1-1.1.1k-r0 license:
OpenSSL

```

### `apk` package: `libcurl`

```console
libcurl-7.76.1-r0 description:
The multiprotocol file transfer library

libcurl-7.76.1-r0 webpage:
https://curl.se/

libcurl-7.76.1-r0 installed size:
488 KiB

libcurl-7.76.1-r0 license:
MIT

```

### `apk` package: `libedit`

```console
libedit-20191231.3.1-r1 description:
BSD line editing library

libedit-20191231.3.1-r1 webpage:
https://www.thrysoee.dk/editline

libedit-20191231.3.1-r1 installed size:
196 KiB

libedit-20191231.3.1-r1 license:
BSD-3-Clause

```

### `apk` package: `libldap`

```console
libldap-2.4.57-r1 description:
OpenLDAP libraries

libldap-2.4.57-r1 webpage:
https://www.openldap.org/

libldap-2.4.57-r1 installed size:
616 KiB

libldap-2.4.57-r1 license:
custom

```

### `apk` package: `libpq`

```console
libpq-13.2-r0 description:
PostgreSQL libraries

libpq-13.2-r0 webpage:
https://www.postgresql.org/

libpq-13.2-r0 installed size:
328 KiB

libpq-13.2-r0 license:
PostgreSQL

```

### `apk` package: `libsasl`

```console
libsasl-2.1.27-r10 description:
Cyrus Simple Authentication and Security Layer (SASL) library

libsasl-2.1.27-r10 webpage:
https://www.cyrusimap.org/sasl/

libsasl-2.1.27-r10 installed size:
192 KiB

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
340 KiB

libsodium-1.0.18-r0 license:
ISC

```

### `apk` package: `libssl1.1`

```console
libssl1.1-1.1.1k-r0 description:
SSL shared libraries

libssl1.1-1.1.1k-r0 webpage:
https://www.openssl.org/

libssl1.1-1.1.1k-r0 installed size:
528 KiB

libssl1.1-1.1.1k-r0 license:
OpenSSL

```

### `apk` package: `libtls-standalone`

```console
libtls-standalone-2.9.1-r1 description:
libtls extricated from libressl sources

libtls-standalone-2.9.1-r1 webpage:
https://www.libressl.org/

libtls-standalone-2.9.1-r1 installed size:
108 KiB

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
1196 KiB

libxml2-2.9.10-r6 license:
MIT

```

### `apk` package: `musl`

```console
musl-1.2.2-r0 description:
the musl c library (libc) implementation

musl-1.2.2-r0 webpage:
https://musl.libc.org/

musl-1.2.2-r0 installed size:
608 KiB

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
140 KiB

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
496 KiB

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
216 KiB

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
168 KiB

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
556 KiB

oniguruma-6.9.6-r0 license:
BSD-2-Clause

```

### `apk` package: `openssl`

```console
openssl-1.1.1k-r0 description:
Toolkit for Transport Layer Security (TLS)

openssl-1.1.1k-r0 webpage:
https://www.openssl.org/

openssl-1.1.1k-r0 installed size:
660 KiB

openssl-1.1.1k-r0 license:
OpenSSL

```

### `apk` package: `readline`

```console
readline-8.1.0-r0 description:
GNU readline library

readline-8.1.0-r0 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.1.0-r0 installed size:
308 KiB

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
92 KiB

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
948 KiB

sqlite-libs-3.34.1-r0 license:
Public-Domain

```

### `apk` package: `ssl_client`

```console
ssl_client-1.32.1-r6 description:
EXternal ssl_client for busybox wget

ssl_client-1.32.1-r6 webpage:
https://busybox.net/

ssl_client-1.32.1-r6 installed size:
28 KiB

ssl_client-1.32.1-r6 license:
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

### `apk` package: `unixodbc`

```console
unixodbc-2.3.9-r1 description:
ODBC is an open specification to access Data Sources

unixodbc-2.3.9-r1 webpage:
http://www.unixodbc.org/

unixodbc-2.3.9-r1 installed size:
700 KiB

unixodbc-2.3.9-r1 license:
LGPL-2.0-or-later

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
