# `wordpress:beta-5.8-beta2-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:42482018531a4c43658fa90fbc322af1afad51c0baab95b4615dafa23c2d7fb5`
- Created: `2021-06-15T22:22:34.708535372Z`
- Virtual Size: ~ 248.95 Mb  
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
  - `GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312`
  - `PHP_VERSION=7.4.20`
  - `PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc`
  - `PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335`

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

### `apk` package: `aom-libs`

```console
aom-libs-1.0.0-r1 description:
Alliance for Open Media (AOM) AV1 codec SDK (libraries)

aom-libs-1.0.0-r1 webpage:
https://aomedia.org/

aom-libs-1.0.0-r1 installed size:
3992 KiB

aom-libs-1.0.0-r1 license:
custom

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

### `apk` package: `cairo`

```console
cairo-1.16.0-r2 description:
A vector graphics library

cairo-1.16.0-r2 webpage:
https://cairographics.org/

cairo-1.16.0-r2 installed size:
1132 KiB

cairo-1.16.0-r2 license:
LGPL-2.0-or-later MPL-1.1

```

### `apk` package: `cairo-gobject`

```console
cairo-gobject-1.16.0-r2 description:
A vector graphics library (gobject bindings)

cairo-gobject-1.16.0-r2 webpage:
https://cairographics.org/

cairo-gobject-1.16.0-r2 installed size:
84 KiB

cairo-gobject-1.16.0-r2 license:
LGPL-2.0-or-later MPL-1.1

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

### `apk` package: `fribidi`

```console
fribidi-1.0.10-r0 description:
Free Implementation of the Unicode Bidirectional Algorithm

fribidi-1.0.10-r0 webpage:
https://github.com/fribidi/fribidi

fribidi-1.0.10-r0 installed size:
156 KiB

fribidi-1.0.10-r0 license:
LGPL-2.0-or-later

```

### `apk` package: `gdk-pixbuf`

```console
gdk-pixbuf-2.42.4-r0 description:
GTK+ image loading library

gdk-pixbuf-2.42.4-r0 webpage:
https://wiki.gnome.org/Projects/GdkPixbuf

gdk-pixbuf-2.42.4-r0 installed size:
560 KiB

gdk-pixbuf-2.42.4-r0 license:
LGPL-2.0-or-later

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

### `apk` package: `glib`

```console
glib-2.66.8-r0 description:
Common C routines used by Gtk+ and other libs

glib-2.66.8-r0 webpage:
https://developer.gnome.org/glib/

glib-2.66.8-r0 installed size:
3324 KiB

glib-2.66.8-r0 license:
LGPL-2.1-or-later

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

### `apk` package: `graphite2`

```console
graphite2-1.3.14-r0 description:
reimplementation of the SIL Graphite text processing engine

graphite2-1.3.14-r0 webpage:
https://graphite.sil.org/

graphite2-1.3.14-r0 installed size:
132 KiB

graphite2-1.3.14-r0 license:
LGPL-2.1-or-later OR MPL-1.1

```

### `apk` package: `harfbuzz`

```console
harfbuzz-2.7.4-r1 description:
Text shaping library

harfbuzz-2.7.4-r1 webpage:
https://freedesktop.org/wiki/Software/HarfBuzz

harfbuzz-2.7.4-r1 installed size:
1296 KiB

harfbuzz-2.7.4-r1 license:
MIT

```

### `apk` package: `imagemagick`

```console
imagemagick-7.0.11.13-r0 description:
Collection of tools and libraries for many image formats

imagemagick-7.0.11.13-r0 webpage:
https://www.imagemagick.org/

imagemagick-7.0.11.13-r0 installed size:
4560 KiB

imagemagick-7.0.11.13-r0 license:
ImageMagick

```

### `apk` package: `imagemagick-libs`

```console
imagemagick-libs-7.0.11.13-r0 description:
Collection of tools and libraries for many image formats (libraries)

imagemagick-libs-7.0.11.13-r0 webpage:
https://www.imagemagick.org/

imagemagick-libs-7.0.11.13-r0 installed size:
3252 KiB

imagemagick-libs-7.0.11.13-r0 license:
ImageMagick

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

### `apk` package: `libblkid`

```console
libblkid-2.36.1-r1 description:
Block device identification library from util-linux

libblkid-2.36.1-r1 webpage:
https://git.kernel.org/cgit/utils/util-linux/util-linux.git

libblkid-2.36.1-r1 installed size:
292 KiB

libblkid-2.36.1-r1 license:
GPL-3.0-or-later AND GPL-2.0-or-later AND GPL-2.0-only AND

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
libcurl-7.77.0-r0 description:
The multiprotocol file transfer library

libcurl-7.77.0-r0 webpage:
https://curl.se/

libcurl-7.77.0-r0 installed size:
500 KiB

libcurl-7.77.0-r0 license:
MIT

```

### `apk` package: `libde265`

```console
libde265-1.0.4-r0 description:
Open h.265 video codec implementation

libde265-1.0.4-r0 webpage:
https://github.com/strukturag/libde265

libde265-1.0.4-r0 installed size:
808 KiB

libde265-1.0.4-r0 license:
LGPL-3.0-or-later

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

### `apk` package: `libheif`

```console
libheif-1.9.1-r0 description:
ISO/IEC 23008-12:2017 HEIF file format decoder and encoder

libheif-1.9.1-r0 webpage:
https://www.libde265.org/

libheif-1.9.1-r0 installed size:
576 KiB

libheif-1.9.1-r0 license:
LGPL-3.0-or-later

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

### `apk` package: `libmount`

```console
libmount-2.36.1-r1 description:
Block device identification library from util-linux

libmount-2.36.1-r1 webpage:
https://git.kernel.org/cgit/utils/util-linux/util-linux.git

libmount-2.36.1-r1 installed size:
328 KiB

libmount-2.36.1-r1 license:
GPL-3.0-or-later AND GPL-2.0-or-later AND GPL-2.0-only AND

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

### `apk` package: `librsvg`

```console
librsvg-2.50.4-r0 description:
SAX-based renderer for SVG files into a GdkPixbuf

librsvg-2.50.4-r0 webpage:
https://wiki.gnome.org/Projects/LibRsvg

librsvg-2.50.4-r0 installed size:
10 MiB

librsvg-2.50.4-r0 license:
LGPL-2.1-or-later

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

### `apk` package: `libwebp`

```console
libwebp-1.1.0-r0 description:
Libraries for working with WebP images

libwebp-1.1.0-r0 webpage:
https://developers.google.com/speed/webp

libwebp-1.1.0-r0 installed size:
576 KiB

libwebp-1.1.0-r0 license:
BSD-3-Clause

```

### `apk` package: `libx11`

```console
libx11-1.7.1-r0 description:
X11 client-side library

libx11-1.7.1-r0 webpage:
http://xorg.freedesktop.org/

libx11-1.7.1-r0 installed size:
3240 KiB

libx11-1.7.1-r0 license:
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

### `apk` package: `libxft`

```console
libxft-2.3.3-r0 description:
FreeType-based font drawing library for X

libxft-2.3.3-r0 webpage:
http://xorg.freedesktop.org/

libxft-2.3.3-r0 installed size:
92 KiB

libxft-2.3.3-r0 license:
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

### `apk` package: `libxrender`

```console
libxrender-0.9.10-r3 description:
X Rendering Extension client library

libxrender-0.9.10-r3 webpage:
http://xorg.freedesktop.org/

libxrender-0.9.10-r3 installed size:
56 KiB

libxrender-0.9.10-r3 license:
custom

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

### `apk` package: `pango`

```console
pango-1.48.2-r0 description:
library for layout and rendering of text

pango-1.48.2-r0 webpage:
https://www.pango.org/

pango-1.48.2-r0 installed size:
588 KiB

pango-1.48.2-r0 license:
LGPL-2.1-or-later

```

### `apk` package: `pcre`

```console
pcre-8.44-r0 description:
Perl-compatible regular expression library

pcre-8.44-r0 webpage:
http://pcre.sourceforge.net

pcre-8.44-r0 installed size:
392 KiB

pcre-8.44-r0 license:
BSD-3-Clause

```

### `apk` package: `pixman`

```console
pixman-0.40.0-r2 description:
Low-level pixel manipulation library

pixman-0.40.0-r2 webpage:
https://gitlab.freedesktop.org/pixman

pixman-0.40.0-r2 installed size:
608 KiB

pixman-0.40.0-r2 license:
MIT

```

### `apk` package: `pkgconf`

```console
pkgconf-1.7.3-r0 description:
development framework configuration tools

pkgconf-1.7.3-r0 webpage:
https://git.sr.ht/~kaniini/pkgconf

pkgconf-1.7.3-r0 installed size:
140 KiB

pkgconf-1.7.3-r0 license:
ISC

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

### `apk` package: `shared-mime-info`

```console
shared-mime-info-2.0-r0 description:
Freedesktop.org Shared MIME Info

shared-mime-info-2.0-r0 webpage:
http://freedesktop.org/Software/shared-mime-info

shared-mime-info-2.0-r0 installed size:
2392 KiB

shared-mime-info-2.0-r0 license:
GPL-2.0-or-later

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

### `apk` package: `x265-libs`

```console
x265-libs-3.4-r0 description:
Open Source H265/HEVC video encoder (libraries)

x265-libs-3.4-r0 webpage:
http://x265.org

x265-libs-3.4-r0 installed size:
4524 KiB

x265-libs-3.4-r0 license:
GPL-2.0-or-later

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
