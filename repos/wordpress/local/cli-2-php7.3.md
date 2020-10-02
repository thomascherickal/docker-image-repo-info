# `wordpress:cli-2.4.0-php7.3`

## Docker Metadata

- Image ID: `sha256:c62f0aebd05895ab4fab2d60270e53987f9519b2fd63884910f8e5c97070e499`
- Created: `2020-10-02T04:54:55.275337555Z`
- Virtual Size: ~ 132.29 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-entrypoint.sh"]`
- Command: `["wp","shell"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_LDFLAGS=-Wl,-O1 -pie`
  - `GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D`
  - `PHP_VERSION=7.3.23`
  - `PHP_URL=https://www.php.net/distributions/php-7.3.23.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-7.3.23.tar.xz.asc`
  - `PHP_SHA256=2bdd36176f318f451fb3942bf1e935aabb3c2786cac41a9080f084ad6390e034`
  - `PHP_MD5=`
  - `WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06`
  - `WORDPRESS_CLI_VERSION=2.4.0`
  - `WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.2.0-r6 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.2.0-r6 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.2.0-r6 installed size:
409600

alpine-baselayout-3.2.0-r6 license:
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
apk-tools-2.10.5-r1 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.10.5-r1 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.10.5-r1 installed size:
262144

apk-tools-2.10.5-r1 license:
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
bash-5.0.17-r0 description:
The GNU Bourne Again shell

bash-5.0.17-r0 webpage:
https://www.gnu.org/software/bash/bash.html

bash-5.0.17-r0 installed size:
1200128

bash-5.0.17-r0 license:
GPL-3.0-or-later

```

### `apk` package: `brotli-libs`

```console
brotli-libs-1.0.7-r5 description:
Generic lossless compressor (libraries)

brotli-libs-1.0.7-r5 webpage:
https://github.com/google/brotli

brotli-libs-1.0.7-r5 installed size:
712704

brotli-libs-1.0.7-r5 license:
MIT

```

### `apk` package: `busybox`

```console
busybox-1.31.1-r16 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.31.1-r16 webpage:
https://busybox.net/

busybox-1.31.1-r16 installed size:
962560

busybox-1.31.1-r16 license:
GPL-2.0-only

```

### `apk` package: `ca-certificates`

```console
ca-certificates-20191127-r3 description:
Common CA certificates PEM files from Mozilla

ca-certificates-20191127-r3 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-20191127-r3 installed size:
688128

ca-certificates-20191127-r3 license:
MPL-2.0 GPL-2.0-or-later

```

### `apk` package: `ca-certificates-bundle`

```console
ca-certificates-bundle-20191127-r2 description:
Pre generated bundle of Mozilla certificates

ca-certificates-bundle-20191127-r2 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-bundle-20191127-r2 installed size:
233472

ca-certificates-bundle-20191127-r2 license:
MPL-2.0 GPL-2.0-or-later

```

### `apk` package: `curl`

```console
curl-7.69.1-r0 description:
URL retrival utility and library

curl-7.69.1-r0 webpage:
https://curl.haxx.se/

curl-7.69.1-r0 installed size:
229376

curl-7.69.1-r0 license:
MIT

```

### `apk` package: `expat`

```console
expat-2.2.9-r1 description:
An XML Parser library written in C

expat-2.2.9-r1 webpage:
http://www.libexpat.org/

expat-2.2.9-r1 installed size:
188416

expat-2.2.9-r1 license:
MIT

```

### `apk` package: `fontconfig`

```console
fontconfig-2.13.1-r2 description:
Library for configuring and customizing font access

fontconfig-2.13.1-r2 webpage:
https://www.freedesktop.org/wiki/Software/fontconfig

fontconfig-2.13.1-r2 installed size:
647168

fontconfig-2.13.1-r2 license:
MIT

```

### `apk` package: `freetype`

```console
freetype-2.10.2-r0 description:
TrueType font rendering library

freetype-2.10.2-r0 webpage:
https://www.freetype.org/

freetype-2.10.2-r0 installed size:
749568

freetype-2.10.2-r0 license:
FTL GPL-2.0-or-later

```

### `apk` package: `imagemagick-libs`

```console
imagemagick-libs-7.0.10.25-r0 description:
Collection of tools and libraries for many image formats (libraries)

imagemagick-libs-7.0.10.25-r0 webpage:
https://www.imagemagick.org/

imagemagick-libs-7.0.10.25-r0 installed size:
3293184

imagemagick-libs-7.0.10.25-r0 license:
ImageMagick

```

### `apk` package: `lcms2`

```console
lcms2-2.9-r1 description:
Color Management Engine

lcms2-2.9-r1 webpage:
http://www.littlecms.com

lcms2-2.9-r1 installed size:
339968

lcms2-2.9-r1 license:
MIT

```

### `apk` package: `less`

```console
less-551-r0 description:
File pager

less-551-r0 webpage:
http://www.greenwoodsoftware.com/less/

less-551-r0 installed size:
200704

less-551-r0 license:
GPL

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

### `apk` package: `libbsd`

```console
libbsd-0.10.0-r0 description:
commonly-used BSD functions not implemented by all libcs

libbsd-0.10.0-r0 webpage:
https://libbsd.freedesktop.org/

libbsd-0.10.0-r0 installed size:
94208

libbsd-0.10.0-r0 license:
BSD

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
libcrypto1.1-1.1.1g-r0 description:
Crypto library from openssl

libcrypto1.1-1.1.1g-r0 webpage:
https://www.openssl.org/

libcrypto1.1-1.1.1g-r0 installed size:
2760704

libcrypto1.1-1.1.1g-r0 license:
OpenSSL

```

### `apk` package: `libcurl`

```console
libcurl-7.69.1-r1 description:
The multiprotocol file transfer library

libcurl-7.69.1-r1 webpage:
https://curl.haxx.se/

libcurl-7.69.1-r1 installed size:
458752

libcurl-7.69.1-r1 license:
MIT

```

### `apk` package: `libedit`

```console
libedit-20191231.3.1-r0 description:
BSD line editing library

libedit-20191231.3.1-r0 webpage:
https://www.thrysoee.dk/editline

libedit-20191231.3.1-r0 installed size:
200704

libedit-20191231.3.1-r0 license:
BSD-3-Clause

```

### `apk` package: `libgcc`

```console
libgcc-9.3.0-r2 description:
GNU C compiler runtime libraries

libgcc-9.3.0-r2 webpage:
https://gcc.gnu.org

libgcc-9.3.0-r2 installed size:
90112

libgcc-9.3.0-r2 license:
GPL-2.0-or-later LGPL-2.1-or-later

```

### `apk` package: `libjpeg-turbo`

```console
libjpeg-turbo-2.0.5-r0 description:
Accelerated baseline JPEG compression and decompression library

libjpeg-turbo-2.0.5-r0 webpage:
https://libjpeg-turbo.org/

libjpeg-turbo-2.0.5-r0 installed size:
1056768

libjpeg-turbo-2.0.5-r0 license:
BSD-3-Clause IJG Zlib

```

### `apk` package: `libltdl`

```console
libltdl-2.4.6-r7 description:
Runtime libraries for GNU Libtool Dynamic Module Loader

libltdl-2.4.6-r7 webpage:
https://www.gnu.org/software/libtool

libltdl-2.4.6-r7 installed size:
53248

libltdl-2.4.6-r7 license:
LGPL-2.0+

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
libssl1.1-1.1.1g-r0 description:
SSL shared libraries

libssl1.1-1.1.1g-r0 webpage:
https://www.openssl.org/

libssl1.1-1.1.1g-r0 installed size:
540672

libssl1.1-1.1.1g-r0 license:
OpenSSL

```

### `apk` package: `libstdc++`

```console
libstdc++-9.3.0-r2 description:
GNU C++ standard runtime library

libstdc++-9.3.0-r2 webpage:
https://gcc.gnu.org

libstdc++-9.3.0-r2 installed size:
1671168

libstdc++-9.3.0-r2 license:
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

### `apk` package: `libuuid`

```console
libuuid-2.35.2-r0 description:
DCE compatible Universally Unique Identifier library

libuuid-2.35.2-r0 webpage:
https://git.kernel.org/cgit/utils/util-linux/util-linux.git

libuuid-2.35.2-r0 installed size:
40960

libuuid-2.35.2-r0 license:
GPL-2.0 GPL-2.0-or-later LGPL-2.0-or-later BSD Public-Domain

```

### `apk` package: `libx11`

```console
libx11-1.6.12-r0 description:
X11 client-side library

libx11-1.6.12-r0 webpage:
http://xorg.freedesktop.org/

libx11-1.6.12-r0 installed size:
3391488

libx11-1.6.12-r0 license:
custom:XFREE86

```

### `apk` package: `libxau`

```console
libxau-1.0.9-r0 description:
X11 authorisation library

libxau-1.0.9-r0 webpage:
http://xorg.freedesktop.org/

libxau-1.0.9-r0 installed size:
28672

libxau-1.0.9-r0 license:
MIT

```

### `apk` package: `libxcb`

```console
libxcb-1.14-r1 description:
X11 client-side library

libxcb-1.14-r1 webpage:
https://xcb.freedesktop.org

libxcb-1.14-r1 installed size:
1019904

libxcb-1.14-r1 license:
MIT

```

### `apk` package: `libxdmcp`

```console
libxdmcp-1.1.3-r0 description:
X11 Display Manager Control Protocol library

libxdmcp-1.1.3-r0 webpage:
http://xorg.freedesktop.org/

libxdmcp-1.1.3-r0 installed size:
40960

libxdmcp-1.1.3-r0 license:
MIT

```

### `apk` package: `libxext`

```console
libxext-1.3.4-r0 description:
X11 miscellaneous extensions library

libxext-1.3.4-r0 webpage:
http://xorg.freedesktop.org/

libxext-1.3.4-r0 installed size:
86016

libxext-1.3.4-r0 license:
MIT

```

### `apk` package: `libxml2`

```console
libxml2-2.9.10-r5 description:
XML parsing library, version 2

libxml2-2.9.10-r5 webpage:
http://www.xmlsoft.org/

libxml2-2.9.10-r5 installed size:
1220608

libxml2-2.9.10-r5 license:
MIT

```

### `apk` package: `libzip`

```console
libzip-1.6.1-r1 description:
C library for manipulating zip archives

libzip-1.6.1-r1 webpage:
http://www.nih.at/libzip/index.html

libzip-1.6.1-r1 installed size:
106496

libzip-1.6.1-r1 license:
BSD-3-Clause

```

### `apk` package: `mariadb-client`

```console
mariadb-client-10.4.13-r0 description:
Client for the MariaDB database

mariadb-client-10.4.13-r0 webpage:
https://www.mariadb.org/

mariadb-client-10.4.13-r0 installed size:
29753344

mariadb-client-10.4.13-r0 license:
GPL-2.0-or-later

```

### `apk` package: `mariadb-common`

```console
mariadb-common-10.4.13-r0 description:
MariaDB common files for both server and client

mariadb-common-10.4.13-r0 webpage:
https://www.mariadb.org/

mariadb-common-10.4.13-r0 installed size:
2265088

mariadb-common-10.4.13-r0 license:
GPL-2.0-or-later

```

### `apk` package: `musl`

```console
musl-1.1.24-r9 description:
the musl c library (libc) implementation

musl-1.1.24-r9 webpage:
https://musl.libc.org/

musl-1.1.24-r9 installed size:
614400

musl-1.1.24-r9 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.1.24-r8 description:
the musl c library (libc) implementation

musl-utils-1.1.24-r8 webpage:
https://musl.libc.org/

musl-utils-1.1.24-r8 installed size:
151552

musl-utils-1.1.24-r8 license:
MIT BSD GPL2+

```

### `apk` package: `mysql-client`

```console
mysql-client-10.4.13-r0 description:
Dummy package for mysql-client migration

mysql-client-10.4.13-r0 webpage:
https://www.mariadb.org/

mysql-client-10.4.13-r0 installed size:
4096

mysql-client-10.4.13-r0 license:
GPL-2.0-or-later

```

### `apk` package: `ncurses-libs`

```console
ncurses-libs-6.2_p20200523-r0 description:
Ncurses libraries

ncurses-libs-6.2_p20200523-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-libs-6.2_p20200523-r0 installed size:
507904

ncurses-libs-6.2_p20200523-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.2_p20200523-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.2_p20200523-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-base-6.2_p20200523-r0 installed size:
217088

ncurses-terminfo-base-6.2_p20200523-r0 license:
MIT

```

### `apk` package: `nghttp2-libs`

```console
nghttp2-libs-1.41.0-r0 description:
Experimental HTTP/2 client, server and proxy (libraries)

nghttp2-libs-1.41.0-r0 webpage:
https://nghttp2.org

nghttp2-libs-1.41.0-r0 installed size:
159744

nghttp2-libs-1.41.0-r0 license:
MIT

```

### `apk` package: `openssl`

```console
openssl-1.1.1g-r0 description:
Toolkit for Transport Layer Security (TLS)

openssl-1.1.1g-r0 webpage:
https://www.openssl.org/

openssl-1.1.1g-r0 installed size:
675840

openssl-1.1.1g-r0 license:
OpenSSL

```

### `apk` package: `readline`

```console
readline-8.0.4-r0 description:
GNU readline library

readline-8.0.4-r0 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.0.4-r0 installed size:
299008

readline-8.0.4-r0 license:
GPL-2.0-or-later

```

### `apk` package: `scanelf`

```console
scanelf-1.2.6-r0 description:
Scan ELF binaries for stuff

scanelf-1.2.6-r0 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.2.6-r0 installed size:
94208

scanelf-1.2.6-r0 license:
GPL-2.0-only

```

### `apk` package: `sqlite-libs`

```console
sqlite-libs-3.32.1-r0 description:
Sqlite3 library

sqlite-libs-3.32.1-r0 webpage:
https://www.sqlite.org/

sqlite-libs-3.32.1-r0 installed size:
962560

sqlite-libs-3.32.1-r0 license:
Public-Domain

```

### `apk` package: `ssl_client`

```console
ssl_client-1.31.1-r16 description:
EXternal ssl_client for busybox wget

ssl_client-1.31.1-r16 webpage:
https://busybox.net/

ssl_client-1.31.1-r16 installed size:
28672

ssl_client-1.31.1-r16 license:
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
