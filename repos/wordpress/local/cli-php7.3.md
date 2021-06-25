# `wordpress:cli-2.5.0-php7.3`

## Docker Metadata

- Image ID: `sha256:cbf708c55e059372188831f20e5a45ab88679b6b7d905f460339a24f2e72c7fe`
- Created: `2021-06-24T07:10:58.115297165Z`
- Virtual Size: ~ 130.27 Mb  
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
  - `PHP_VERSION=7.3.28`
  - `PHP_URL=https://www.php.net/distributions/php-7.3.28.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-7.3.28.tar.xz.asc`
  - `PHP_SHA256=a2a84dbec8c1eee3f46c5f249eaaa2ecb3f9e7a6f5d0604d2df44ff8d4904dbe`
  - `WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06`
  - `WORDPRESS_CLI_VERSION=2.5.0`
  - `WORDPRESS_CLI_SHA512=08dd9035fda1d529807380d5b757839e2809e289eb1a698fe33e7e21a1431d3f77c551c2b2db5adc55083d5075ea4137407994111890f765e790a97e6d9ca7af`

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

### `apk` package: `bash`

```console
bash-5.1.0-r0 description:
The GNU Bourne Again shell

bash-5.1.0-r0 webpage:
https://www.gnu.org/software/bash/bash.html

bash-5.1.0-r0 installed size:
1296 KiB

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

### `apk` package: `expat`

```console
expat-2.2.10-r1 description:
XML Parser library written in C

expat-2.2.10-r1 webpage:
http://www.libexpat.org/

expat-2.2.10-r1 installed size:
184 KiB

expat-2.2.10-r1 license:
MIT

```

### `apk` package: `fontconfig`

```console
fontconfig-2.13.1-r3 description:
Library for configuring and customizing font access

fontconfig-2.13.1-r3 webpage:
https://www.freedesktop.org/wiki/Software/fontconfig

fontconfig-2.13.1-r3 installed size:
632 KiB

fontconfig-2.13.1-r3 license:
MIT

```

### `apk` package: `freetype`

```console
freetype-2.10.4-r1 description:
TrueType font rendering library

freetype-2.10.4-r1 webpage:
https://www.freetype.org/

freetype-2.10.4-r1 installed size:
728 KiB

freetype-2.10.4-r1 license:
FTL GPL-2.0-or-later

```

### `apk` package: `imagemagick-libs`

```console
imagemagick-libs-7.0.10.57-r0 description:
Collection of tools and libraries for many image formats (libraries)

imagemagick-libs-7.0.10.57-r0 webpage:
https://www.imagemagick.org/

imagemagick-libs-7.0.10.57-r0 installed size:
3244 KiB

imagemagick-libs-7.0.10.57-r0 license:
ImageMagick

```

### `apk` package: `lcms2`

```console
lcms2-2.11-r0 description:
Color Management Engine

lcms2-2.11-r0 webpage:
http://www.littlecms.com

lcms2-2.11-r0 installed size:
332 KiB

lcms2-2.11-r0 license:
MIT GPL-3.0-only

```

### `apk` package: `less`

```console
less-563-r0 description:
File pager

less-563-r0 webpage:
http://www.greenwoodsoftware.com/less/

less-563-r0 installed size:
196 KiB

less-563-r0 license:
GPL-3.0-or-later OR BSD-2-Clause

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

### `apk` package: `libbsd`

```console
libbsd-0.10.0-r0 description:
commonly-used BSD functions not implemented by all libcs

libbsd-0.10.0-r0 webpage:
https://libbsd.freedesktop.org/

libbsd-0.10.0-r0 installed size:
92 KiB

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

### `apk` package: `libgcc`

```console
libgcc-10.2.1_pre1-r3 description:
GNU C compiler runtime libraries

libgcc-10.2.1_pre1-r3 webpage:
https://gcc.gnu.org

libgcc-10.2.1_pre1-r3 installed size:
112 KiB

libgcc-10.2.1_pre1-r3 license:
GPL-2.0-or-later LGPL-2.1-or-later

```

### `apk` package: `libjpeg-turbo`

```console
libjpeg-turbo-2.1.0-r0 description:
Accelerated baseline JPEG compression and decompression library

libjpeg-turbo-2.1.0-r0 webpage:
https://libjpeg-turbo.org/

libjpeg-turbo-2.1.0-r0 installed size:
1076 KiB

libjpeg-turbo-2.1.0-r0 license:
BSD-3-Clause IJG Zlib

```

### `apk` package: `libltdl`

```console
libltdl-2.4.6-r7 description:
Runtime libraries for GNU Libtool Dynamic Module Loader

libltdl-2.4.6-r7 webpage:
https://www.gnu.org/software/libtool

libltdl-2.4.6-r7 installed size:
52 KiB

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
204 KiB

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

### `apk` package: `libstdc++`

```console
libstdc++-10.2.1_pre1-r3 description:
GNU C++ standard runtime library

libstdc++-10.2.1_pre1-r3 webpage:
https://gcc.gnu.org

libstdc++-10.2.1_pre1-r3 installed size:
1668 KiB

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
108 KiB

libtls-standalone-2.9.1-r1 license:
ISC

```

### `apk` package: `libuuid`

```console
libuuid-2.36.1-r1 description:
DCE compatible Universally Unique Identifier library

libuuid-2.36.1-r1 webpage:
https://git.kernel.org/cgit/utils/util-linux/util-linux.git

libuuid-2.36.1-r1 installed size:
40 KiB

libuuid-2.36.1-r1 license:
GPL-3.0-or-later AND GPL-2.0-or-later AND GPL-2.0-only AND

```

### `apk` package: `libx11`

```console
libx11-1.7.0-r0 description:
X11 client-side library

libx11-1.7.0-r0 webpage:
http://xorg.freedesktop.org/

libx11-1.7.0-r0 installed size:
3240 KiB

libx11-1.7.0-r0 license:
custom:XFREE86

```

### `apk` package: `libxau`

```console
libxau-1.0.9-r0 description:
X11 authorisation library

libxau-1.0.9-r0 webpage:
http://xorg.freedesktop.org/

libxau-1.0.9-r0 installed size:
28 KiB

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
996 KiB

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
40 KiB

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
84 KiB

libxext-1.3.4-r0 license:
MIT

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

### `apk` package: `libzip`

```console
libzip-1.7.3-r2 description:
C library for manipulating zip archives

libzip-1.7.3-r2 webpage:
http://www.nih.at/libzip/index.html

libzip-1.7.3-r2 installed size:
108 KiB

libzip-1.7.3-r2 license:
BSD-3-Clause

```

### `apk` package: `mariadb-client`

```console
mariadb-client-10.5.9-r0 description:
Client for the MariaDB database

mariadb-client-10.5.9-r0 webpage:
https://www.mariadb.org/

mariadb-client-10.5.9-r0 installed size:
28 MiB

mariadb-client-10.5.9-r0 license:
GPL-2.0-or-later

```

### `apk` package: `mariadb-common`

```console
mariadb-common-10.5.9-r0 description:
MariaDB common files for both server and client

mariadb-common-10.5.9-r0 webpage:
https://www.mariadb.org/

mariadb-common-10.5.9-r0 installed size:
2240 KiB

mariadb-common-10.5.9-r0 license:
GPL-2.0-or-later

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

### `apk` package: `mysql-client`

```console
mysql-client-10.5.9-r0 description:
Dummy package for mysql-client migration

mysql-client-10.5.9-r0 webpage:
https://www.mariadb.org/

mysql-client-10.5.9-r0 installed size:
4096 B

mysql-client-10.5.9-r0 license:
GPL-2.0-or-later

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
