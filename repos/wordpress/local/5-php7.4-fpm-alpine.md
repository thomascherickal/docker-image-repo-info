# `wordpress:5.3.2-php7.4-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:4c31dc22ad2f8b33a8aef69daa5f6286303680c5718b811412dca5d456a22db0`
- Created: `2020-01-18T06:05:14.731353031Z`
- Virtual Size: ~ 202.38 Mb  
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
  - `PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie`
  - `GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312`
  - `PHP_VERSION=7.4.1`
  - `PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror`
  - `PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror`
  - `PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762`
  - `PHP_MD5=`
  - `WORDPRESS_VERSION=5.3.2`
  - `WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b`

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

### `apk` package: `avahi-libs`

```console
avahi-libs-0.7-r4 description:
Libraries for avahi run-time use

avahi-libs-0.7-r4 webpage:
https://www.avahi.org/

avahi-libs-0.7-r4 installed size:
131072

avahi-libs-0.7-r4 license:
LGPL-2.0-or-later

```

### `apk` package: `bash`

```console
bash-5.0.11-r1 description:
The GNU Bourne Again shell

bash-5.0.11-r1 webpage:
https://www.gnu.org/software/bash/bash.html

bash-5.0.11-r1 installed size:
1200128

bash-5.0.11-r1 license:
GPL-3.0-or-later

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

### `apk` package: `cups-libs`

```console
cups-libs-2.2.12-r1 description:
CUPS libraries

cups-libs-2.2.12-r1 webpage:
https://www.cups.org/

cups-libs-2.2.12-r1 installed size:
569344

cups-libs-2.2.12-r1 license:
GPL-2.0-only

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

### `apk` package: `dbus-libs`

```console
dbus-libs-1.12.16-r2 description:
D-BUS access libraries

dbus-libs-1.12.16-r2 webpage:
https://www.freedesktop.org/Software/dbus

dbus-libs-1.12.16-r2 installed size:
307200

dbus-libs-1.12.16-r2 license:
AFL-2.1 OR GPL-2.0-or-later

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
freetype-2.10.1-r0 description:
TrueType font rendering library

freetype-2.10.1-r0 webpage:
https://www.freetype.org/

freetype-2.10.1-r0 installed size:
737280

freetype-2.10.1-r0 license:
FTL GPL-2.0-or-later

```

### `apk` package: `ghostscript`

```console
ghostscript-9.50-r0 description:
An interpreter for the PostScript language and for PDF

ghostscript-9.50-r0 webpage:
https://ghostscript.com/

ghostscript-9.50-r0 installed size:
50257920

ghostscript-9.50-r0 license:
AGPL-3.0-or-later

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

### `apk` package: `gnutls`

```console
gnutls-3.6.10-r0 description:
A TLS protocol implementation

gnutls-3.6.10-r0 webpage:
https://www.gnutls.org/

gnutls-3.6.10-r0 installed size:
1662976

gnutls-3.6.10-r0 license:
GPL-3.0-or-later

```

### `apk` package: `imagemagick-libs`

```console
imagemagick-libs-7.0.9.7-r0 description:
Collection of tools and libraries for many image formats (libraries)

imagemagick-libs-7.0.9.7-r0 webpage:
https://www.imagemagick.org/

imagemagick-libs-7.0.9.7-r0 installed size:
3260416

imagemagick-libs-7.0.9.7-r0 license:
ImageMagick

```

### `apk` package: `jbig2dec`

```console
jbig2dec-0.17-r0 description:
JBIG2 image compression format decoder

jbig2dec-0.17-r0 webpage:
https://jbig2dec.com/

jbig2dec-0.17-r0 installed size:
143360

jbig2dec-0.17-r0 license:
GPL-2.0-or-later

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

### `apk` package: `libffi`

```console
libffi-3.2.1-r6 description:
A portable, high level programming interface to various calling conventions.

libffi-3.2.1-r6 webpage:
http://sourceware.org/libffi

libffi-3.2.1-r6 installed size:
49152

libffi-3.2.1-r6 license:
MIT

```

### `apk` package: `libintl`

```console
libintl-0.20.1-r2 description:
GNU gettext runtime library

libintl-0.20.1-r2 webpage:
https://www.gnu.org/software/gettext/gettext.html

libintl-0.20.1-r2 installed size:
57344

libintl-0.20.1-r2 license:
LGPL-2.1-or-later

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
libssl1.1-1.1.1d-r3 description:
SSL shared libraries

libssl1.1-1.1.1d-r3 webpage:
https://www.openssl.org

libssl1.1-1.1.1d-r3 installed size:
536576

libssl1.1-1.1.1d-r3 license:
OpenSSL

```

### `apk` package: `libtasn1`

```console
libtasn1-4.15.0-r0 description:
The ASN.1 library used in GNUTLS

libtasn1-4.15.0-r0 webpage:
https://www.gnu.org/software/gnutls/

libtasn1-4.15.0-r0 installed size:
151552

libtasn1-4.15.0-r0 license:
GPL-3.0 LGPL

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

### `apk` package: `libunistring`

```console
libunistring-0.9.10-r0 description:
Library for manipulating Unicode strings and C strings

libunistring-0.9.10-r0 webpage:
https://www.gnu.org/software/libunistring/

libunistring-0.9.10-r0 installed size:
1540096

libunistring-0.9.10-r0 license:
GPL-2.0+ OR LGPL-3.0+

```

### `apk` package: `libuuid`

```console
libuuid-2.34-r1 description:
DCE compatible Universally Unique Identifier library

libuuid-2.34-r1 webpage:
https://git.kernel.org/cgit/utils/util-linux/util-linux.git

libuuid-2.34-r1 installed size:
40960

libuuid-2.34-r1 license:
GPL-2.0 GPL-2.0-or-later LGPL-2.0-or-later BSD Public-Domain

```

### `apk` package: `libx11`

```console
libx11-1.6.9-r0 description:
X11 client-side library

libx11-1.6.9-r0 webpage:
http://xorg.freedesktop.org/

libx11-1.6.9-r0 installed size:
3391488

libx11-1.6.9-r0 license:
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
libxml2-2.9.10-r1 description:
XML parsing library, version 2

libxml2-2.9.10-r1 webpage:
http://www.xmlsoft.org/

libxml2-2.9.10-r1 installed size:
1220608

libxml2-2.9.10-r1 license:
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

### `apk` package: `nettle`

```console
nettle-3.5.1-r0 description:
A low-level cryptographic library

nettle-3.5.1-r0 webpage:
https://www.lysator.liu.se/~nisse/nettle/

nettle-3.5.1-r0 installed size:
462848

nettle-3.5.1-r0 license:
LGPL-2.0-or-later

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

### `apk` package: `p11-kit`

```console
p11-kit-0.23.18.1-r0 description:
Library for loading and sharing PKCS#11 modules

p11-kit-0.23.18.1-r0 webpage:
https://p11-glue.freedesktop.org/

p11-kit-0.23.18.1-r0 installed size:
1245184

p11-kit-0.23.18.1-r0 license:
BSD-3-Clause

```

### `apk` package: `readline`

```console
readline-8.0.1-r0 description:
GNU readline library

readline-8.0.1-r0 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.0.1-r0 installed size:
299008

readline-8.0.1-r0 license:
GPL-2.0-or-later

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

### `apk` package: `sed`

```console
sed-4.7-r0 description:
GNU stream editor

sed-4.7-r0 webpage:
https://www.gnu.org/software/sed

sed-4.7-r0 installed size:
163840

sed-4.7-r0 license:
GPL-3.0+

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

### `apk` package: `tiff`

```console
tiff-4.1.0-r0 description:
Provides support for the Tag Image File Format or TIFF

tiff-4.1.0-r0 webpage:
http://www.libtiff.org

tiff-4.1.0-r0 installed size:
450560

tiff-4.1.0-r0 license:
libtiff

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
