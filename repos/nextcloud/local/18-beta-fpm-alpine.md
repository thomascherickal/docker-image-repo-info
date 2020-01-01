# `nextcloud:18.0.0beta4-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:7315aacbf38b978d4b3ef0dbf698e9f5f10c87fa770dc92ad734bff232853103`
- Created: `2019-12-31T00:21:21.372016592Z`
- Virtual Size: ~ 370.99 Mb  
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
  - `GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D`
  - `PHP_VERSION=7.3.13`
  - `PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror`
  - `PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror`
  - `PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228`
  - `PHP_MD5=`
  - `NEXTCLOUD_VERSION=18.0.0beta4`

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

### `apk` package: `expat`

```console
expat-2.2.8-r0 description:
An XML Parser library written in C

expat-2.2.8-r0 webpage:
http://www.libexpat.org/

expat-2.2.8-r0 installed size:
184320

expat-2.2.8-r0 license:
MIT

```

### `apk` package: `fontconfig`

```console
fontconfig-2.13.1-r0 description:
Library for configuring and customizing font access

fontconfig-2.13.1-r0 webpage:
http://fontconfig.org

fontconfig-2.13.1-r0 installed size:
643072

fontconfig-2.13.1-r0 license:
GPL

```

### `apk` package: `freetype`

```console
freetype-2.10.0-r0 description:
TrueType font rendering library

freetype-2.10.0-r0 webpage:
https://www.freetype.org/

freetype-2.10.0-r0 installed size:
737280

freetype-2.10.0-r0 license:
FTL GPL-2.0-or-later

```

### `apk` package: `gmp`

```console
gmp-6.1.2-r1 description:
A free library for arbitrary precision arithmetic

gmp-6.1.2-r1 webpage:
https://gmplib.org/

gmp-6.1.2-r1 installed size:
421888

gmp-6.1.2-r1 license:
LGPL-3.0

```

### `apk` package: `icu-libs`

```console
icu-libs-64.2-r0 description:
International Components for Unicode library (libraries)

icu-libs-64.2-r0 webpage:
http://www.icu-project.org/

icu-libs-64.2-r0 installed size:
32145408

icu-libs-64.2-r0 license:
MIT ICU Unicode-TOU

```

### `apk` package: `imagemagick-libs`

```console
imagemagick-libs-7.0.8.68-r0 description:
Collection of tools and libraries for many image formats (libraries)

imagemagick-libs-7.0.8.68-r0 webpage:
https://www.imagemagick.org/

imagemagick-libs-7.0.8.68-r0 installed size:
3260416

imagemagick-libs-7.0.8.68-r0 license:
ImageMagick

```

### `apk` package: `lcms2`

```console
lcms2-2.9-r1 description:
Color Management Engine

lcms2-2.9-r1 webpage:
http://www.littlecms.com

lcms2-2.9-r1 installed size:
335872

lcms2-2.9-r1 license:
MIT

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

### `apk` package: `libbsd`

```console
libbsd-0.9.1-r0 description:
commonly-used BSD functions not implemented by all libcs

libbsd-0.9.1-r0 webpage:
https://libbsd.freedesktop.org/

libbsd-0.9.1-r0 installed size:
94208

libbsd-0.9.1-r0 license:
BSD

```

### `apk` package: `libbz2`

```console
libbz2-1.0.6-r7 description:
Shared library for bz2

libbz2-1.0.6-r7 webpage:
http://sources.redhat.com/bzip2

libbz2-1.0.6-r7 installed size:
73728

libbz2-1.0.6-r7 license:
BSD

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

### `apk` package: `libgcc`

```console
libgcc-8.3.0-r0 description:
GNU C compiler runtime libraries

libgcc-8.3.0-r0 webpage:
http://gcc.gnu.org

libgcc-8.3.0-r0 installed size:
90112

libgcc-8.3.0-r0 license:
GPL LGPL

```

### `apk` package: `libjpeg-turbo`

```console
libjpeg-turbo-2.0.3-r0 description:
Accelerated baseline JPEG compression and decompression library

libjpeg-turbo-2.0.3-r0 webpage:
https://libjpeg-turbo.org/

libjpeg-turbo-2.0.3-r0 installed size:
1343488

libjpeg-turbo-2.0.3-r0 license:
BSD-3-Clause IJG Zlib

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

### `apk` package: `libltdl`

```console
libltdl-2.4.6-r6 description:
Runtime libraries for GNU Libtool Dynamic Module Loader

libltdl-2.4.6-r6 webpage:
https://www.gnu.org/software/libtool

libltdl-2.4.6-r6 installed size:
53248

libltdl-2.4.6-r6 license:
LGPL-2.0+

```

### `apk` package: `libmemcached-libs`

```console
libmemcached-libs-1.0.18-r3 description:
Client library and command line tools for memcached server (libraries)

libmemcached-libs-1.0.18-r3 webpage:
http://libmemcached.org/

libmemcached-libs-1.0.18-r3 installed size:
335872

libmemcached-libs-1.0.18-r3 license:
BSD

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

### `apk` package: `libstdc++`

```console
libstdc++-8.3.0-r0 description:
GNU C++ standard runtime library

libstdc++-8.3.0-r0 webpage:
http://gcc.gnu.org

libstdc++-8.3.0-r0 installed size:
1392640

libstdc++-8.3.0-r0 license:
GPL LGPL

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

### `apk` package: `libuuid`

```console
libuuid-2.33.2-r0 description:
DCE compatible Universally Unique Identifier library

libuuid-2.33.2-r0 webpage:
https://git.kernel.org/cgit/utils/util-linux/util-linux.git

libuuid-2.33.2-r0 installed size:
40960

libuuid-2.33.2-r0 license:
GPL-2.0 GPL-2.0-or-later LGPL-2.0-or-later BSD Public-Domain

```

### `apk` package: `libwebp`

```console
libwebp-1.0.2-r0 description:
Libraries for working with WebP images

libwebp-1.0.2-r0 webpage:
https://developers.google.com/speed/webp

libwebp-1.0.2-r0 installed size:
581632

libwebp-1.0.2-r0 license:
BSD-3-Clause

```

### `apk` package: `libx11`

```console
libx11-1.6.8-r1 description:
X11 client-side library

libx11-1.6.8-r1 webpage:
http://xorg.freedesktop.org/

libx11-1.6.8-r1 installed size:
3391488

libx11-1.6.8-r1 license:
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
libxcb-1.13.1-r0 description:
X11 client-side library

libxcb-1.13.1-r0 webpage:
https://xcb.freedesktop.org

libxcb-1.13.1-r0 installed size:
1019904

libxcb-1.13.1-r0 license:
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
libxml2-2.9.9-r2 description:
XML parsing library, version 2

libxml2-2.9.9-r2 webpage:
http://www.xmlsoft.org/

libxml2-2.9.9-r2 installed size:
1216512

libxml2-2.9.9-r2 license:
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

### `apk` package: `popt`

```console
popt-1.16-r7 description:
A commandline option parser

popt-1.16-r7 webpage:
http://rpm5.org

popt-1.16-r7 installed size:
57344

popt-1.16-r7 license:
custom

```

### `apk` package: `rsync`

```console
rsync-3.1.3-r1 description:
A file transfer program to keep remote files in sync

rsync-3.1.3-r1 webpage:
https://rsync.samba.org/

rsync-3.1.3-r1 installed size:
446464

rsync-3.1.3-r1 license:
GPL-3.0

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
