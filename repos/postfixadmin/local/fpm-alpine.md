# `postfixadmin:3.2.2-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:fa1caabbf2d10eed5dd33efa17da6b6e37792393c7ff969f8949bbcd1293653f`
- Created: `2019-12-19T06:06:55.253309408Z`
- Virtual Size: ~ 88.23 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/usr/local/bin/docker-entrypoint.sh"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie`
  - `GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D`
  - `PHP_VERSION=7.3.13`
  - `PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror`
  - `PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror`
  - `PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228`
  - `PHP_MD5=`
  - `POSTFIXADMIN_VERSION=3.2.2`
  - `POSTFIXADMIN_SHA512=6c84cb215e69c52c26db0651e5d0d9d8bcb0a63b00d3c197f10fa1f0442a1fde44bb514fb476a1e68a21741d603febac67282961d01270e5969ee13d145121ee`
- Labels:
  - `maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.1.2-r0 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.1.2-r0 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.1.2-r0 installed size:
405504

alpine-baselayout-3.1.2-r0 license:
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
apk-tools-2.10.4-r2 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.10.4-r2 webpage:
https://git.alpinelinux.org/cgit/apk-tools/

apk-tools-2.10.4-r2 installed size:
262144

apk-tools-2.10.4-r2 license:
GPL2

```

### `apk` package: `argon2-libs`

```console
argon2-libs-20171227-r2 description:
The password hash Argon2, winner of PHC (libraries)

argon2-libs-20171227-r2 webpage:
https://github.com/P-H-C/phc-winner-argon2

argon2-libs-20171227-r2 installed size:
53248

argon2-libs-20171227-r2 license:
Apache-2.0 CC0-1.0

```

### `apk` package: `bash`

```console
bash-5.0.0-r0 description:
The GNU Bourne Again shell

bash-5.0.0-r0 webpage:
https://www.gnu.org/software/bash/bash.html

bash-5.0.0-r0 installed size:
1200128

bash-5.0.0-r0 license:
GPL-3.0-or-later

```

### `apk` package: `busybox`

```console
busybox-1.30.1-r2 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.30.1-r2 webpage:
https://busybox.net/

busybox-1.30.1-r2 installed size:
942080

busybox-1.30.1-r2 license:
GPL-2.0

```

### `apk` package: `ca-certificates`

```console
ca-certificates-20190108-r0 description:
Common CA certificates PEM files

ca-certificates-20190108-r0 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-20190108-r0 installed size:
737280

ca-certificates-20190108-r0 license:
MPL-2.0 GPL-2.0-or-later

```

### `apk` package: `ca-certificates-cacert`

```console
ca-certificates-cacert-20190108-r0 description:
Mozilla bundled certificates

ca-certificates-cacert-20190108-r0 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-cacert-20190108-r0 installed size:
245760

ca-certificates-cacert-20190108-r0 license:
MPL-2.0 GPL-2.0-or-later

```

### `apk` package: `coreutils`

```console
coreutils-8.31-r0 description:
The basic file, shell and text manipulation utilities

coreutils-8.31-r0 webpage:
https://www.gnu.org/software/coreutils/

coreutils-8.31-r0 installed size:
1122304

coreutils-8.31-r0 license:
GPL-3.0-or-later

```

### `apk` package: `curl`

```console
curl-7.66.0-r0 description:
URL retrival utility and library

curl-7.66.0-r0 webpage:
https://curl.haxx.se/

curl-7.66.0-r0 installed size:
225280

curl-7.66.0-r0 license:
MIT

```

### `apk` package: `db`

```console
db-5.3.28-r1 description:
The Berkeley DB embedded database system

db-5.3.28-r1 webpage:
https://www.oracle.com/technology/software/products/berkeley-db/index.html

db-5.3.28-r1 installed size:
1556480

db-5.3.28-r1 license:
custom

```

### `apk` package: `libacl`

```console
libacl-2.2.52-r6 description:
Dynamic library for access control list support

libacl-2.2.52-r6 webpage:
https://savannah.nongnu.org/projects/acl

libacl-2.2.52-r6 installed size:
53248

libacl-2.2.52-r6 license:
LGPL-2.1-or-later AND GPL-2.0-or-later

```

### `apk` package: `libattr`

```console
libattr-2.4.48-r0 description:
Utilities for managing filesystem extended attributes (libraries)

libattr-2.4.48-r0 webpage:
https://savannah.nongnu.org/projects/attr

libattr-2.4.48-r0 installed size:
32768

libattr-2.4.48-r0 license:
LGPL-2.1-or-later

```

### `apk` package: `libc-utils`

```console
libc-utils-0.7.1-r0 description:
Meta package to pull in correct libc

libc-utils-0.7.1-r0 webpage:
http://alpinelinux.org

libc-utils-0.7.1-r0 installed size:
4096

libc-utils-0.7.1-r0 license:
BSD

```

### `apk` package: `libcrypto1.1`

```console
libcrypto1.1-1.1.1d-r0 description:
Crypto library from openssl

libcrypto1.1-1.1.1d-r0 webpage:
https://www.openssl.org

libcrypto1.1-1.1.1d-r0 installed size:
2736128

libcrypto1.1-1.1.1d-r0 license:
OpenSSL

```

### `apk` package: `libcurl`

```console
libcurl-7.66.0-r0 description:
The multiprotocol file transfer library

libcurl-7.66.0-r0 webpage:
https://curl.haxx.se/

libcurl-7.66.0-r0 installed size:
454656

libcurl-7.66.0-r0 license:
MIT

```

### `apk` package: `libedit`

```console
libedit-20190324.3.1-r0 description:
BSD line editing library

libedit-20190324.3.1-r0 webpage:
https://www.thrysoee.dk/editline

libedit-20190324.3.1-r0 installed size:
200704

libedit-20190324.3.1-r0 license:
BSD-3-Clause

```

### `apk` package: `libldap`

```console
libldap-2.4.48-r0 description:
OpenLDAP libraries

libldap-2.4.48-r0 webpage:
http://www.openldap.org/

libldap-2.4.48-r0 installed size:
626688

libldap-2.4.48-r0 license:
custom

```

### `apk` package: `libpq`

```console
libpq-11.6-r0 description:
PostgreSQL libraries

libpq-11.6-r0 webpage:
https://www.postgresql.org/

libpq-11.6-r0 installed size:
315392

libpq-11.6-r0 license:
PostgreSQL

```

### `apk` package: `libsasl`

```console
libsasl-2.1.27-r3 description:
Cyrus Simple Authentication and Security Layer (SASL) library

libsasl-2.1.27-r3 webpage:
https://cyrusimap.org/

libsasl-2.1.27-r3 installed size:
180224

libsasl-2.1.27-r3 license:
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
libssl1.1-1.1.1d-r0 description:
SSL shared libraries

libssl1.1-1.1.1d-r0 webpage:
https://www.openssl.org

libssl1.1-1.1.1d-r0 installed size:
532480

libssl1.1-1.1.1d-r0 license:
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
libxml2-2.9.9-r2 description:
XML parsing library, version 2

libxml2-2.9.9-r2 webpage:
http://www.xmlsoft.org/

libxml2-2.9.9-r2 installed size:
1216512

libxml2-2.9.9-r2 license:
MIT

```

### `apk` package: `musl`

```console
musl-1.1.22-r3 description:
the musl c library (libc) implementation

musl-1.1.22-r3 webpage:
http://www.musl-libc.org/

musl-1.1.22-r3 installed size:
598016

musl-1.1.22-r3 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.1.22-r3 description:
the musl c library (libc) implementation

musl-utils-1.1.22-r3 webpage:
http://www.musl-libc.org/

musl-utils-1.1.22-r3 installed size:
147456

musl-utils-1.1.22-r3 license:
MIT BSD GPL2+

```

### `apk` package: `ncurses-libs`

```console
ncurses-libs-6.1_p20190518-r0 description:
Ncurses libraries

ncurses-libs-6.1_p20190518-r0 webpage:
https://www.gnu.org/software/ncurses/

ncurses-libs-6.1_p20190518-r0 installed size:
503808

ncurses-libs-6.1_p20190518-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo`

```console
ncurses-terminfo-6.1_p20190518-r0 description:
Console display library (other terminfo files)

ncurses-terminfo-6.1_p20190518-r0 webpage:
https://www.gnu.org/software/ncurses/

ncurses-terminfo-6.1_p20190518-r0 installed size:
7307264

ncurses-terminfo-6.1_p20190518-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.1_p20190518-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.1_p20190518-r0 webpage:
https://www.gnu.org/software/ncurses/

ncurses-terminfo-base-6.1_p20190518-r0 installed size:
94208

ncurses-terminfo-base-6.1_p20190518-r0 license:
MIT

```

### `apk` package: `nghttp2-libs`

```console
nghttp2-libs-1.39.2-r0 description:
Experimental HTTP/2 client, server and proxy (libraries)

nghttp2-libs-1.39.2-r0 webpage:
https://nghttp2.org

nghttp2-libs-1.39.2-r0 installed size:
155648

nghttp2-libs-1.39.2-r0 license:
MIT

```

### `apk` package: `openssl`

```console
openssl-1.1.1d-r0 description:
Toolkit for Transport Layer Security (TLS)

openssl-1.1.1d-r0 webpage:
https://www.openssl.org

openssl-1.1.1d-r0 installed size:
679936

openssl-1.1.1d-r0 license:
OpenSSL

```

### `apk` package: `readline`

```console
readline-8.0.0-r0 description:
GNU readline library

readline-8.0.0-r0 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.0.0-r0 installed size:
299008

readline-8.0.0-r0 license:
GPL

```

### `apk` package: `scanelf`

```console
scanelf-1.2.3-r0 description:
Scan ELF binaries for stuff

scanelf-1.2.3-r0 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.2.3-r0 installed size:
98304

scanelf-1.2.3-r0 license:
GPL-2.0

```

### `apk` package: `sqlite-libs`

```console
sqlite-libs-3.28.0-r2 description:
Sqlite3 library

sqlite-libs-3.28.0-r2 webpage:
https://www.sqlite.org/

sqlite-libs-3.28.0-r2 installed size:
925696

sqlite-libs-3.28.0-r2 license:
Public-Domain

```

### `apk` package: `ssl_client`

```console
ssl_client-1.30.1-r2 description:
EXternal ssl_client for busybox wget

ssl_client-1.30.1-r2 webpage:
https://busybox.net/

ssl_client-1.30.1-r2 installed size:
28672

ssl_client-1.30.1-r2 license:
GPL-2.0

```

### `apk` package: `tar`

```console
tar-1.32-r0 description:
Utility used to store, backup, and transport files

tar-1.32-r0 webpage:
https://www.gnu.org

tar-1.32-r0 installed size:
491520

tar-1.32-r0 license:
GPL

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
zlib-1.2.11-r1 description:
A compression/decompression Library

zlib-1.2.11-r1 webpage:
http://zlib.net

zlib-1.2.11-r1 installed size:
110592

zlib-1.2.11-r1 license:
zlib

```
