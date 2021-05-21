# `wordpress:5.7.2-php8.0-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:e9f68a9673aab9154b9f8347725480c2f9b26ce98be1a2d969e309fd920d6019`
- Created: `2021-05-19T23:45:34.270917142Z`
- Virtual Size: ~ 199.27 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-entrypoint.sh"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_LDFLAGS=-Wl,-O1 -pie`
  - `GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F`
  - `PHP_VERSION=8.0.6`
  - `PHP_URL=https://www.php.net/distributions/php-8.0.6.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-8.0.6.tar.xz.asc`
  - `PHP_SHA256=e9871d3b6c391fe9e89f86f6334852dcc10eeaaa8d5565beb8436e7f0cf30e20`

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

### `apk` package: `avahi-libs`

```console
avahi-libs-0.8-r2 description:
Libraries for avahi run-time use

avahi-libs-0.8-r2 webpage:
https://www.avahi.org/

avahi-libs-0.8-r2 installed size:
128 KiB

avahi-libs-0.8-r2 license:
LGPL-2.0-or-later

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

### `apk` package: `cups-libs`

```console
cups-libs-2.3.3-r1 description:
CUPS libraries

cups-libs-2.3.3-r1 webpage:
https://www.cups.org/

cups-libs-2.3.3-r1 installed size:
564 KiB

cups-libs-2.3.3-r1 license:
GPL-2.0-only

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

### `apk` package: `dbus-libs`

```console
dbus-libs-1.12.20-r1 description:
D-BUS access libraries

dbus-libs-1.12.20-r1 webpage:
https://www.freedesktop.org/Software/dbus

dbus-libs-1.12.20-r1 installed size:
304 KiB

dbus-libs-1.12.20-r1 license:
AFL-2.1 OR GPL-2.0-or-later

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

### `apk` package: `ghostscript`

```console
ghostscript-9.53.3-r0 description:
An interpreter for the PostScript language and for PDF

ghostscript-9.53.3-r0 webpage:
https://ghostscript.com/

ghostscript-9.53.3-r0 installed size:
48 MiB

ghostscript-9.53.3-r0 license:
AGPL-3.0-or-later

```

### `apk` package: `gmp`

```console
gmp-6.2.1-r0 description:
free library for arbitrary precision arithmetic

gmp-6.2.1-r0 webpage:
https://gmplib.org/

gmp-6.2.1-r0 installed size:
416 KiB

gmp-6.2.1-r0 license:
LGPL-3.0-or-later OR GPL-2.0-or-later

```

### `apk` package: `gnutls`

```console
gnutls-3.7.1-r0 description:
TLS protocol implementation

gnutls-3.7.1-r0 webpage:
https://www.gnutls.org/

gnutls-3.7.1-r0 installed size:
1848 KiB

gnutls-3.7.1-r0 license:
LGPL-2.1-or-later

```

### `apk` package: `jbig2dec`

```console
jbig2dec-0.19-r0 description:
JBIG2 image compression format decoder

jbig2dec-0.19-r0 webpage:
https://jbig2dec.com/

jbig2dec-0.19-r0 installed size:
148 KiB

jbig2dec-0.19-r0 license:
GPL-2.0-or-later

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

### `apk` package: `libffi`

```console
libffi-3.3-r2 description:
A portable, high level programming interface to various calling conventions.

libffi-3.3-r2 webpage:
https://sourceware.org/libffi

libffi-3.3-r2 installed size:
52 KiB

libffi-3.3-r2 license:
MIT

```

### `apk` package: `libintl`

```console
libintl-0.20.2-r2 description:
GNU gettext runtime library

libintl-0.20.2-r2 webpage:
https://www.gnu.org/software/gettext/gettext.html

libintl-0.20.2-r2 installed size:
56 KiB

libintl-0.20.2-r2 license:
LGPL-2.1-or-later

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

### `apk` package: `libtasn1`

```console
libtasn1-4.16.0-r1 description:
The ASN.1 library used in GNUTLS

libtasn1-4.16.0-r1 webpage:
https://www.gnu.org/software/gnutls/

libtasn1-4.16.0-r1 installed size:
88 KiB

libtasn1-4.16.0-r1 license:
LGPL-2.1-or-later

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

### `apk` package: `libunistring`

```console
libunistring-0.9.10-r0 description:
Library for manipulating Unicode strings and C strings

libunistring-0.9.10-r0 webpage:
https://www.gnu.org/software/libunistring/

libunistring-0.9.10-r0 installed size:
1504 KiB

libunistring-0.9.10-r0 license:
GPL-2.0+ OR LGPL-3.0+

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

### `apk` package: `nettle`

```console
nettle-3.7.2-r0 description:
A low-level cryptographic library

nettle-3.7.2-r0 webpage:
https://www.lysator.liu.se/~nisse/nettle/

nettle-3.7.2-r0 installed size:
564 KiB

nettle-3.7.2-r0 license:
LGPL-2.0-or-later

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

### `apk` package: `p11-kit`

```console
p11-kit-0.23.22-r0 description:
Library for loading and sharing PKCS#11 modules

p11-kit-0.23.22-r0 webpage:
https://p11-glue.freedesktop.org/

p11-kit-0.23.22-r0 installed size:
1200 KiB

p11-kit-0.23.22-r0 license:
BSD-3-Clause

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

### `apk` package: `sed`

```console
sed-4.8-r0 description:
GNU stream editor

sed-4.8-r0 webpage:
https://www.gnu.org/software/sed

sed-4.8-r0 installed size:
160 KiB

sed-4.8-r0 license:
GPL-3.0-or-later

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

### `apk` package: `tiff`

```console
tiff-4.2.0-r0 description:
Provides support for the Tag Image File Format or TIFF

tiff-4.2.0-r0 webpage:
https://gitlab.com/libtiff/libtiff

tiff-4.2.0-r0 installed size:
452 KiB

tiff-4.2.0-r0 license:
libtiff

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
