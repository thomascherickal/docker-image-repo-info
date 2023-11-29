# `nextcloud:27.1.4-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:b5c301ccef9ab72121b70b96de5288370746d6fb03452adc99e0b4476cbb8d7f`
- Created: `2023-11-28T18:41:29.485116326Z`
- Virtual Size: ~ 823.99 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/entrypoint.sh"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_LDFLAGS=-Wl,-O1 -pie`
  - `GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC`
  - `PHP_VERSION=8.2.13`
  - `PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc`
  - `PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b`
  - `PHP_MEMORY_LIMIT=512M`
  - `PHP_UPLOAD_LIMIT=512M`
  - `NEXTCLOUD_VERSION=27.1.4`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.4.3-r1 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.4.3-r1 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.4.3-r1 installed size:
324 KiB

alpine-baselayout-3.4.3-r1 license:
GPL-2.0-only

```

### `apk` package: `alpine-baselayout-data`

```console
alpine-baselayout-data-3.4.3-r1 description:
Alpine base dir structure and init scripts

alpine-baselayout-data-3.4.3-r1 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-data-3.4.3-r1 installed size:
76 KiB

alpine-baselayout-data-3.4.3-r1 license:
GPL-2.0-only

```

### `apk` package: `alpine-keys`

```console
alpine-keys-2.4-r1 description:
Public keys for Alpine Linux packages

alpine-keys-2.4-r1 webpage:
https://alpinelinux.org

alpine-keys-2.4-r1 installed size:
156 KiB

alpine-keys-2.4-r1 license:
MIT

```

### `apk` package: `aom-libs`

```console
aom-libs-3.6.1-r0 description:
Alliance for Open Media (AOM) AV1 codec SDK (libraries)

aom-libs-3.6.1-r0 webpage:
https://aomedia.org/

aom-libs-3.6.1-r0 installed size:
7252 KiB

aom-libs-3.6.1-r0 license:
BSD-2-Clause AND custom

```

### `apk` package: `apk-tools`

```console
apk-tools-2.14.0-r2 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.14.0-r2 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.14.0-r2 installed size:
304 KiB

apk-tools-2.14.0-r2 license:
GPL-2.0-only

```

### `apk` package: `argon2-libs`

```console
argon2-libs-20190702-r4 description:
The password hash Argon2, winner of PHC (libraries)

argon2-libs-20190702-r4 webpage:
https://github.com/P-H-C/phc-winner-argon2

argon2-libs-20190702-r4 installed size:
52 KiB

argon2-libs-20190702-r4 license:
Apache-2.0 OR CC0-1.0

```

### `apk` package: `avahi-libs`

```console
avahi-libs-0.8-r13 description:
Libraries for avahi run-time use

avahi-libs-0.8-r13 webpage:
https://www.avahi.org/

avahi-libs-0.8-r13 installed size:
124 KiB

avahi-libs-0.8-r13 license:
LGPL-2.1-or-later

```

### `apk` package: `brotli-libs`

```console
brotli-libs-1.0.9-r14 description:
Generic lossless compressor (libraries)

brotli-libs-1.0.9-r14 webpage:
https://github.com/google/brotli

brotli-libs-1.0.9-r14 installed size:
788 KiB

brotli-libs-1.0.9-r14 license:
MIT

```

### `apk` package: `busybox`

```console
busybox-1.36.1-r2 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.36.1-r2 webpage:
https://busybox.net/

busybox-1.36.1-r2 installed size:
924 KiB

busybox-1.36.1-r2 license:
GPL-2.0-only

```

### `apk` package: `busybox-binsh`

```console
busybox-binsh-1.36.1-r2 description:
busybox ash /bin/sh

busybox-binsh-1.36.1-r2 webpage:
https://busybox.net/

busybox-binsh-1.36.1-r2 installed size:
8192 B

busybox-binsh-1.36.1-r2 license:
GPL-2.0-only

```

### `apk` package: `ca-certificates`

```console
ca-certificates-20230506-r0 description:
Common CA certificates PEM files from Mozilla

ca-certificates-20230506-r0 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-20230506-r0 installed size:
688 KiB

ca-certificates-20230506-r0 license:
MPL-2.0 AND MIT

```

### `apk` package: `ca-certificates-bundle`

```console
ca-certificates-bundle-20230506-r0 description:
Pre generated bundle of Mozilla certificates

ca-certificates-bundle-20230506-r0 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-bundle-20230506-r0 installed size:
232 KiB

ca-certificates-bundle-20230506-r0 license:
MPL-2.0 AND MIT

```

### `apk` package: `cairo`

```console
cairo-1.17.8-r1 description:
A vector graphics library

cairo-1.17.8-r1 webpage:
https://cairographics.org/

cairo-1.17.8-r1 installed size:
1040 KiB

cairo-1.17.8-r1 license:
LGPL-2.1-or-later OR MPL-1.1

```

### `apk` package: `cairo-gobject`

```console
cairo-gobject-1.17.8-r1 description:
A vector graphics library (gobject bindings)

cairo-gobject-1.17.8-r1 webpage:
https://cairographics.org/

cairo-gobject-1.17.8-r1 installed size:
44 KiB

cairo-gobject-1.17.8-r1 license:
LGPL-2.1-or-later OR MPL-1.1

```

### `apk` package: `cups-libs`

```console
cups-libs-2.4.7-r0 description:
CUPS libraries

cups-libs-2.4.7-r0 webpage:
https://github.com/OpenPrinting/cups/

cups-libs-2.4.7-r0 installed size:
576 KiB

cups-libs-2.4.7-r0 license:
Apache-2.0

```

### `apk` package: `curl`

```console
curl-8.4.0-r0 description:
URL retrival utility and library

curl-8.4.0-r0 webpage:
https://curl.se/

curl-8.4.0-r0 installed size:
248 KiB

curl-8.4.0-r0 license:
curl

```

### `apk` package: `dbus-libs`

```console
dbus-libs-1.14.8-r0 description:
D-BUS access libraries

dbus-libs-1.14.8-r0 webpage:
https://www.freedesktop.org/Software/dbus

dbus-libs-1.14.8-r0 installed size:
292 KiB

dbus-libs-1.14.8-r0 license:
AFL-2.1 OR GPL-2.0-or-later

```

### `apk` package: `fontconfig`

```console
fontconfig-2.14.2-r3 description:
Library for configuring and customizing font access

fontconfig-2.14.2-r3 webpage:
https://www.freedesktop.org/wiki/Software/fontconfig

fontconfig-2.14.2-r3 installed size:
712 KiB

fontconfig-2.14.2-r3 license:
MIT

```

### `apk` package: `freetype`

```console
freetype-2.13.0-r5 description:
TrueType font rendering library

freetype-2.13.0-r5 webpage:
https://www.freetype.org/

freetype-2.13.0-r5 installed size:
724 KiB

freetype-2.13.0-r5 license:
FTL OR GPL-2.0-or-later

```

### `apk` package: `fribidi`

```console
fribidi-1.0.13-r0 description:
Free Implementation of the Unicode Bidirectional Algorithm

fribidi-1.0.13-r0 webpage:
https://github.com/fribidi/fribidi

fribidi-1.0.13-r0 installed size:
156 KiB

fribidi-1.0.13-r0 license:
LGPL-2.1-or-later

```

### `apk` package: `gdbm`

```console
gdbm-1.23-r1 description:
GNU dbm is a set of database routines that use extensible hashing

gdbm-1.23-r1 webpage:
https://www.gnu.org/software/gdbm/

gdbm-1.23-r1 installed size:
88 KiB

gdbm-1.23-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gdk-pixbuf`

```console
gdk-pixbuf-2.42.10-r5 description:
GTK+ image loading library

gdk-pixbuf-2.42.10-r5 webpage:
https://wiki.gnome.org/Projects/GdkPixbuf

gdk-pixbuf-2.42.10-r5 installed size:
524 KiB

gdk-pixbuf-2.42.10-r5 license:
LGPL-2.1-or-later

```

### `apk` package: `ghostscript`

```console
ghostscript-10.02.0-r0 description:
An interpreter for the PostScript language and for PDF

ghostscript-10.02.0-r0 webpage:
https://ghostscript.com/

ghostscript-10.02.0-r0 installed size:
67 MiB

ghostscript-10.02.0-r0 license:
AGPL-3.0-or-later

```

### `apk` package: `glib`

```console
glib-2.76.4-r0 description:
Common C routines used by Gtk+ and other libs

glib-2.76.4-r0 webpage:
https://developer.gnome.org/glib/

glib-2.76.4-r0 installed size:
3824 KiB

glib-2.76.4-r0 license:
LGPL-2.1-or-later

```

### `apk` package: `gmp`

```console
gmp-6.2.1-r3 description:
free library for arbitrary precision arithmetic

gmp-6.2.1-r3 webpage:
https://gmplib.org/

gmp-6.2.1-r3 installed size:
420 KiB

gmp-6.2.1-r3 license:
LGPL-3.0-or-later OR GPL-2.0-or-later

```

### `apk` package: `gnu-libiconv-libs`

```console
gnu-libiconv-libs-1.17-r1 description:
GNU charset conversion library for libc which doesn't implement it (libraries)

gnu-libiconv-libs-1.17-r1 webpage:
https://www.gnu.org/software/libiconv

gnu-libiconv-libs-1.17-r1 installed size:
1064 KiB

gnu-libiconv-libs-1.17-r1 license:
LGPL-2.1-or-later

```

### `apk` package: `gnutls`

```console
gnutls-3.8.0-r2 description:
TLS protocol implementation

gnutls-3.8.0-r2 webpage:
https://www.gnutls.org/

gnutls-3.8.0-r2 installed size:
1848 KiB

gnutls-3.8.0-r2 license:
LGPL-2.1-or-later

```

### `apk` package: `graphite2`

```console
graphite2-1.3.14-r5 description:
reimplementation of the SIL Graphite text processing engine

graphite2-1.3.14-r5 webpage:
https://graphite.sil.org/

graphite2-1.3.14-r5 installed size:
136 KiB

graphite2-1.3.14-r5 license:
LGPL-2.1-or-later OR MPL-1.1

```

### `apk` package: `harfbuzz`

```console
harfbuzz-7.3.0-r0 description:
Text shaping library

harfbuzz-7.3.0-r0 webpage:
https://harfbuzz.github.io/

harfbuzz-7.3.0-r0 installed size:
1160 KiB

harfbuzz-7.3.0-r0 license:
MIT

```

### `apk` package: `icu-data-en`

```console
icu-data-en-73.2-r2 description:
Stripped down ICU data with only en_US/GB locale and no legacy charset converters

icu-data-en-73.2-r2 webpage:
https://icu.unicode.org/

icu-data-en-73.2-r2 installed size:
3016 KiB

icu-data-en-73.2-r2 license:
ICU

```

### `apk` package: `icu-libs`

```console
icu-libs-73.2-r2 description:
International Components for Unicode library (libraries)

icu-libs-73.2-r2 webpage:
https://icu.unicode.org/

icu-libs-73.2-r2 installed size:
4332 KiB

icu-libs-73.2-r2 license:
ICU

```

### `apk` package: `imagemagick`

```console
imagemagick-7.1.1.13-r1 description:
Collection of tools and libraries for many image formats

imagemagick-7.1.1.13-r1 webpage:
https://imagemagick.org/

imagemagick-7.1.1.13-r1 installed size:
4604 KiB

imagemagick-7.1.1.13-r1 license:
ImageMagick

```

### `apk` package: `imagemagick-libs`

```console
imagemagick-libs-7.1.1.13-r1 description:
Collection of tools and libraries for many image formats (libraries)

imagemagick-libs-7.1.1.13-r1 webpage:
https://imagemagick.org/

imagemagick-libs-7.1.1.13-r1 installed size:
3248 KiB

imagemagick-libs-7.1.1.13-r1 license:
ImageMagick

```

### `apk` package: `jbig2dec`

```console
jbig2dec-0.19-r3 description:
JBIG2 image compression format decoder

jbig2dec-0.19-r3 webpage:
https://jbig2dec.com/

jbig2dec-0.19-r3 installed size:
148 KiB

jbig2dec-0.19-r3 license:
AGPL-3.0-or-later

```

### `apk` package: `lcms2`

```console
lcms2-2.15-r2 description:
Color Management Engine

lcms2-2.15-r2 webpage:
https://www.littlecms.com

lcms2-2.15-r2 installed size:
336 KiB

lcms2-2.15-r2 license:
MIT

```

### `apk` package: `libacl`

```console
libacl-2.3.1-r3 description:
Dynamic library for access control list support

libacl-2.3.1-r3 webpage:
https://savannah.nongnu.org/projects/acl

libacl-2.3.1-r3 installed size:
44 KiB

libacl-2.3.1-r3 license:
LGPL-2.1-or-later AND GPL-2.0-or-later

```

### `apk` package: `libblkid`

```console
libblkid-2.38.1-r8 description:
Block device identification library from util-linux

libblkid-2.38.1-r8 webpage:
https://git.kernel.org/cgit/utils/util-linux/util-linux.git

libblkid-2.38.1-r8 installed size:
300 KiB

libblkid-2.38.1-r8 license:
LGPL-2.1-or-later

```

### `apk` package: `libbsd`

```console
libbsd-0.11.7-r1 description:
commonly-used BSD functions not implemented by all libcs

libbsd-0.11.7-r1 webpage:
https://libbsd.freedesktop.org/

libbsd-0.11.7-r1 installed size:
84 KiB

libbsd-0.11.7-r1 license:
BSD-3-Clause

```

### `apk` package: `libbz2`

```console
libbz2-1.0.8-r5 description:
Shared library for bz2

libbz2-1.0.8-r5 webpage:
https://sourceware.org/bzip2/

libbz2-1.0.8-r5 installed size:
88 KiB

libbz2-1.0.8-r5 license:
bzip2-1.0.6

```

### `apk` package: `libc-utils`

```console
libc-utils-0.7.2-r5 description:
Meta package to pull in correct libc

libc-utils-0.7.2-r5 webpage:
https://alpinelinux.org

libc-utils-0.7.2-r5 installed size:
4096 B

libc-utils-0.7.2-r5 license:
BSD-2-Clause AND BSD-3-Clause

```

### `apk` package: `libcrypto3`

```console
libcrypto3-3.1.4-r1 description:
Crypto library from openssl

libcrypto3-3.1.4-r1 webpage:
https://www.openssl.org/

libcrypto3-3.1.4-r1 installed size:
4472 KiB

libcrypto3-3.1.4-r1 license:
Apache-2.0

```

### `apk` package: `libcurl`

```console
libcurl-8.4.0-r0 description:
The multiprotocol file transfer library

libcurl-8.4.0-r0 webpage:
https://curl.se/

libcurl-8.4.0-r0 installed size:
584 KiB

libcurl-8.4.0-r0 license:
curl

```

### `apk` package: `libde265`

```console
libde265-1.0.12-r0 description:
Open h.265 video codec implementation

libde265-1.0.12-r0 webpage:
https://github.com/strukturag/libde265

libde265-1.0.12-r0 installed size:
436 KiB

libde265-1.0.12-r0 license:
LGPL-3.0-or-later

```

### `apk` package: `libexpat`

```console
libexpat-2.5.0-r1 description:
XML Parser library written in C (libraries)

libexpat-2.5.0-r1 webpage:
https://libexpat.github.io/

libexpat-2.5.0-r1 installed size:
144 KiB

libexpat-2.5.0-r1 license:
MIT

```

### `apk` package: `libffi`

```console
libffi-3.4.4-r2 description:
portable, high level programming interface to various calling conventions.

libffi-3.4.4-r2 webpage:
https://sourceware.org/libffi/

libffi-3.4.4-r2 installed size:
52 KiB

libffi-3.4.4-r2 license:
MIT

```

### `apk` package: `libgcc`

```console
libgcc-12.2.1_git20220924-r10 description:
GNU C compiler runtime libraries

libgcc-12.2.1_git20220924-r10 webpage:
https://gcc.gnu.org

libgcc-12.2.1_git20220924-r10 installed size:
132 KiB

libgcc-12.2.1_git20220924-r10 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `libgomp`

```console
libgomp-12.2.1_git20220924-r10 description:
GCC shared-memory parallel programming API library

libgomp-12.2.1_git20220924-r10 webpage:
https://gcc.gnu.org

libgomp-12.2.1_git20220924-r10 installed size:
292 KiB

libgomp-12.2.1_git20220924-r10 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `libheif`

```console
libheif-1.16.2-r0 description:
ISO/IEC 23008-12:2017 HEIF file format decoder and encoder

libheif-1.16.2-r0 webpage:
https://www.libde265.org/

libheif-1.16.2-r0 installed size:
636 KiB

libheif-1.16.2-r0 license:
LGPL-3.0-or-later

```

### `apk` package: `libhwy`

```console
libhwy-1.0.4-r1 description:
Performance-portable, length-agnostic SIMD with runtime dispatch

libhwy-1.0.4-r1 webpage:
https://github.com/google/highway

libhwy-1.0.4-r1 installed size:
52 KiB

libhwy-1.0.4-r1 license:
Apache-2.0

```

### `apk` package: `libidn2`

```console
libidn2-2.3.4-r1 description:
Encode/Decode library for internationalized domain names

libidn2-2.3.4-r1 webpage:
https://www.gnu.org/software/libidn#libidn2

libidn2-2.3.4-r1 installed size:
208 KiB

libidn2-2.3.4-r1 license:
GPL-2.0-or-later AND LGPL-3.0-or-later

```

### `apk` package: `libintl`

```console
libintl-0.21.1-r7 description:
GNU gettext runtime library

libintl-0.21.1-r7 webpage:
https://www.gnu.org/software/gettext/gettext.html

libintl-0.21.1-r7 installed size:
56 KiB

libintl-0.21.1-r7 license:
LGPL-2.1-or-later

```

### `apk` package: `libjpeg-turbo`

```console
libjpeg-turbo-2.1.5.1-r3 description:
Accelerated baseline JPEG compression and decompression library

libjpeg-turbo-2.1.5.1-r3 webpage:
https://libjpeg-turbo.org/

libjpeg-turbo-2.1.5.1-r3 installed size:
1112 KiB

libjpeg-turbo-2.1.5.1-r3 license:
BSD-3-Clause AND IJG AND Zlib

```

### `apk` package: `libjxl`

```console
libjxl-0.8.2-r0 description:
JPEG XL image format reference implementation

libjxl-0.8.2-r0 webpage:
https://github.com/libjxl/libjxl

libjxl-0.8.2-r0 installed size:
4148 KiB

libjxl-0.8.2-r0 license:
Apache-2.0

```

### `apk` package: `libldap`

```console
libldap-2.6.5-r0 description:
OpenLDAP libraries

libldap-2.6.5-r0 webpage:
https://www.openldap.org/

libldap-2.6.5-r0 installed size:
400 KiB

libldap-2.6.5-r0 license:
OLDAP-2.8

```

### `apk` package: `libltdl`

```console
libltdl-2.4.7-r2 description:
Runtime libraries for GNU Libtool Dynamic Module Loader

libltdl-2.4.7-r2 webpage:
https://www.gnu.org/software/libtool

libltdl-2.4.7-r2 installed size:
52 KiB

libltdl-2.4.7-r2 license:
LGPL-2.0-or-later AND GPL-2.0-or-later

```

### `apk` package: `libmd`

```console
libmd-1.0.4-r2 description:
Message Digest functions from BSD systems

libmd-1.0.4-r2 webpage:
https://www.hadrons.org/software/libmd/

libmd-1.0.4-r2 installed size:
56 KiB

libmd-1.0.4-r2 license:
BSD-3-Clause AND BSD-2-Clause AND ISC AND Beerware AND Public Domain

```

### `apk` package: `libmemcached-libs`

```console
libmemcached-libs-1.1.4-r1 description:
Client library and command line tools for memcached server (resurrected) (libraries)

libmemcached-libs-1.1.4-r1 webpage:
https://github.com/awesomized/libmemcached

libmemcached-libs-1.1.4-r1 installed size:
264 KiB

libmemcached-libs-1.1.4-r1 license:
BSD-3-Clause

```

### `apk` package: `libmount`

```console
libmount-2.38.1-r8 description:
Block device identification library from util-linux

libmount-2.38.1-r8 webpage:
https://git.kernel.org/cgit/utils/util-linux/util-linux.git

libmount-2.38.1-r8 installed size:
336 KiB

libmount-2.38.1-r8 license:
LGPL-2.1-or-later

```

### `apk` package: `libncursesw`

```console
libncursesw-6.4_p20230506-r0 description:
Console display library (libncursesw)

libncursesw-6.4_p20230506-r0 webpage:
https://invisible-island.net/ncurses/

libncursesw-6.4_p20230506-r0 installed size:
344 KiB

libncursesw-6.4_p20230506-r0 license:
X11

```

### `apk` package: `libpng`

```console
libpng-1.6.39-r3 description:
Portable Network Graphics library

libpng-1.6.39-r3 webpage:
http://www.libpng.org

libpng-1.6.39-r3 installed size:
204 KiB

libpng-1.6.39-r3 license:
Libpng

```

### `apk` package: `libpq`

```console
libpq-15.5-r0 description:
PostgreSQL client library

libpq-15.5-r0 webpage:
https://www.postgresql.org/

libpq-15.5-r0 installed size:
320 KiB

libpq-15.5-r0 license:
PostgreSQL

```

### `apk` package: `libraw`

```console
libraw-0.21.1-r1 description:
Library for reading RAW files obtained from digital photo cameras

libraw-0.21.1-r1 webpage:
https://www.libraw.org/

libraw-0.21.1-r1 installed size:
2400 KiB

libraw-0.21.1-r1 license:
CDDL-1.0 OR LGPL-2.1-only

```

### `apk` package: `librsvg`

```console
librsvg-2.56.3-r0 description:
SAX-based renderer for SVG files into a GdkPixbuf

librsvg-2.56.3-r0 webpage:
https://wiki.gnome.org/Projects/LibRsvg

librsvg-2.56.3-r0 installed size:
3488 KiB

librsvg-2.56.3-r0 license:
LGPL-2.1-or-later

```

### `apk` package: `libsasl`

```console
libsasl-2.1.28-r4 description:
Cyrus Simple Authentication and Security Layer (SASL) library

libsasl-2.1.28-r4 webpage:
https://www.cyrusimap.org/sasl/

libsasl-2.1.28-r4 installed size:
192 KiB

libsasl-2.1.28-r4 license:
custom

```

### `apk` package: `libsodium`

```console
libsodium-1.0.18-r3 description:
P(ortable|ackageable) NaCl-based crypto library

libsodium-1.0.18-r3 webpage:
https://github.com/jedisct1/libsodium

libsodium-1.0.18-r3 installed size:
336 KiB

libsodium-1.0.18-r3 license:
ISC

```

### `apk` package: `libssl3`

```console
libssl3-3.1.4-r1 description:
SSL shared libraries

libssl3-3.1.4-r1 webpage:
https://www.openssl.org/

libssl3-3.1.4-r1 installed size:
552 KiB

libssl3-3.1.4-r1 license:
Apache-2.0

```

### `apk` package: `libstdc++`

```console
libstdc++-12.2.1_git20220924-r10 description:
GNU C++ standard runtime library

libstdc++-12.2.1_git20220924-r10 webpage:
https://gcc.gnu.org

libstdc++-12.2.1_git20220924-r10 installed size:
2356 KiB

libstdc++-12.2.1_git20220924-r10 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `libtasn1`

```console
libtasn1-4.19.0-r1 description:
The ASN.1 library used in GNUTLS

libtasn1-4.19.0-r1 webpage:
https://www.gnu.org/software/gnutls/

libtasn1-4.19.0-r1 installed size:
80 KiB

libtasn1-4.19.0-r1 license:
LGPL-2.1-or-later

```

### `apk` package: `libunistring`

```console
libunistring-1.1-r1 description:
Library for manipulating Unicode strings and C strings

libunistring-1.1-r1 webpage:
https://www.gnu.org/software/libunistring/

libunistring-1.1-r1 installed size:
1696 KiB

libunistring-1.1-r1 license:
GPL-2.0-or-later OR LGPL-3.0-or-later

```

### `apk` package: `libwebp`

```console
libwebp-1.3.2-r0 description:
Libraries for working with WebP images

libwebp-1.3.2-r0 webpage:
https://developers.google.com/speed/webp

libwebp-1.3.2-r0 installed size:
596 KiB

libwebp-1.3.2-r0 license:
BSD-3-Clause

```

### `apk` package: `libx11`

```console
libx11-1.8.7-r0 description:
X11 client-side library

libx11-1.8.7-r0 webpage:
https://xorg.freedesktop.org/

libx11-1.8.7-r0 installed size:
3092 KiB

libx11-1.8.7-r0 license:
X11

```

### `apk` package: `libxau`

```console
libxau-1.0.11-r2 description:
X11 authorisation library

libxau-1.0.11-r2 webpage:
https://xorg.freedesktop.org/

libxau-1.0.11-r2 installed size:
28 KiB

libxau-1.0.11-r2 license:
MIT

```

### `apk` package: `libxcb`

```console
libxcb-1.15-r1 description:
X11 client-side library

libxcb-1.15-r1 webpage:
https://xcb.freedesktop.org

libxcb-1.15-r1 installed size:
980 KiB

libxcb-1.15-r1 license:
MIT

```

### `apk` package: `libxdmcp`

```console
libxdmcp-1.1.4-r2 description:
X11 Display Manager Control Protocol library

libxdmcp-1.1.4-r2 webpage:
https://xorg.freedesktop.org/

libxdmcp-1.1.4-r2 installed size:
40 KiB

libxdmcp-1.1.4-r2 license:
MIT

```

### `apk` package: `libxext`

```console
libxext-1.3.5-r2 description:
X11 miscellaneous extensions library

libxext-1.3.5-r2 webpage:
https://xorg.freedesktop.org/

libxext-1.3.5-r2 installed size:
80 KiB

libxext-1.3.5-r2 license:
MIT

```

### `apk` package: `libxft`

```console
libxft-2.3.8-r1 description:
FreeType-based font drawing library for X

libxft-2.3.8-r1 webpage:
https://xorg.freedesktop.org/

libxft-2.3.8-r1 installed size:
96 KiB

libxft-2.3.8-r1 license:
MIT

```

### `apk` package: `libxml2`

```console
libxml2-2.11.6-r0 description:
XML parsing library, version 2

libxml2-2.11.6-r0 webpage:
http://www.xmlsoft.org/

libxml2-2.11.6-r0 installed size:
1108 KiB

libxml2-2.11.6-r0 license:
MIT

```

### `apk` package: `libxrender`

```console
libxrender-0.9.11-r3 description:
X Rendering Extension client library

libxrender-0.9.11-r3 webpage:
https://xorg.freedesktop.org/

libxrender-0.9.11-r3 installed size:
56 KiB

libxrender-0.9.11-r3 license:
MIT

```

### `apk` package: `libxxhash`

```console
libxxhash-0.8.2-r0 description:
Extremely fast non-cryptographic hash algorithm (libraries)

libxxhash-0.8.2-r0 webpage:
https://cyan4973.github.io/xxHash/

libxxhash-0.8.2-r0 installed size:
44 KiB

libxxhash-0.8.2-r0 license:
BSD-2-Clause

```

### `apk` package: `libzip`

```console
libzip-1.9.2-r2 description:
C library for manipulating zip archives

libzip-1.9.2-r2 webpage:
https://libzip.org/

libzip-1.9.2-r2 installed size:
112 KiB

libzip-1.9.2-r2 license:
BSD-3-Clause

```

### `apk` package: `lz4-libs`

```console
lz4-libs-1.9.4-r4 description:
LZ4 is lossless compression algorithm with fast decoder @ multiple GB/s per core. (libraries)

lz4-libs-1.9.4-r4 webpage:
https://github.com/lz4/lz4

lz4-libs-1.9.4-r4 installed size:
144 KiB

lz4-libs-1.9.4-r4 license:
BSD-2-Clause AND GPL-2.0-only

```

### `apk` package: `musl`

```console
musl-1.2.4-r2 description:
the musl c library (libc) implementation

musl-1.2.4-r2 webpage:
https://musl.libc.org/

musl-1.2.4-r2 installed size:
620 KiB

musl-1.2.4-r2 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.2.4-r1 description:
the musl c library (libc) implementation

musl-utils-1.2.4-r1 webpage:
https://musl.libc.org/

musl-utils-1.2.4-r1 installed size:
132 KiB

musl-utils-1.2.4-r1 license:
MIT AND BSD-2-Clause AND GPL-2.0-or-later

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.4_p20230506-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.4_p20230506-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-base-6.4_p20230506-r0 installed size:
216 KiB

ncurses-terminfo-base-6.4_p20230506-r0 license:
X11

```

### `apk` package: `nettle`

```console
nettle-3.8.1-r2 description:
A low-level cryptographic library

nettle-3.8.1-r2 webpage:
https://www.lysator.liu.se/~nisse/nettle/

nettle-3.8.1-r2 installed size:
580 KiB

nettle-3.8.1-r2 license:
GPL-2.0-or-later OR LGPL-3.0-or-later

```

### `apk` package: `nghttp2-libs`

```console
nghttp2-libs-1.57.0-r0 description:
Experimental HTTP/2 client, server and proxy (libraries)

nghttp2-libs-1.57.0-r0 webpage:
https://nghttp2.org

nghttp2-libs-1.57.0-r0 installed size:
152 KiB

nghttp2-libs-1.57.0-r0 license:
MIT

```

### `apk` package: `numactl`

```console
numactl-2.0.16-r4 description:
Simple NUMA policy support

numactl-2.0.16-r4 webpage:
https://github.com/numactl/numactl

numactl-2.0.16-r4 installed size:
60 KiB

numactl-2.0.16-r4 license:
LGPL-2.1-only

```

### `apk` package: `oniguruma`

```console
oniguruma-6.9.8-r1 description:
a regular expressions library

oniguruma-6.9.8-r1 webpage:
https://github.com/kkos/oniguruma

oniguruma-6.9.8-r1 installed size:
544 KiB

oniguruma-6.9.8-r1 license:
BSD-2-Clause

```

### `apk` package: `openssl`

```console
openssl-3.1.4-r1 description:
Toolkit for Transport Layer Security (TLS)

openssl-3.1.4-r1 webpage:
https://www.openssl.org/

openssl-3.1.4-r1 installed size:
752 KiB

openssl-3.1.4-r1 license:
Apache-2.0

```

### `apk` package: `p11-kit`

```console
p11-kit-0.24.1-r2 description:
Library for loading and sharing PKCS#11 modules

p11-kit-0.24.1-r2 webpage:
https://p11-glue.freedesktop.org/

p11-kit-0.24.1-r2 installed size:
1012 KiB

p11-kit-0.24.1-r2 license:
BSD-3-Clause

```

### `apk` package: `pango`

```console
pango-1.50.14-r1 description:
library for layout and rendering of text

pango-1.50.14-r1 webpage:
https://www.pango.org/

pango-1.50.14-r1 installed size:
640 KiB

pango-1.50.14-r1 license:
LGPL-2.1-or-later

```

### `apk` package: `pcre2`

```console
pcre2-10.42-r1 description:
Perl-compatible regular expression library

pcre2-10.42-r1 webpage:
https://pcre.org/

pcre2-10.42-r1 installed size:
676 KiB

pcre2-10.42-r1 license:
BSD-3-Clause

```

### `apk` package: `pixman`

```console
pixman-0.42.2-r1 description:
Low-level pixel manipulation library

pixman-0.42.2-r1 webpage:
https://gitlab.freedesktop.org/pixman

pixman-0.42.2-r1 installed size:
584 KiB

pixman-0.42.2-r1 license:
MIT

```

### `apk` package: `pkgconf`

```console
pkgconf-1.9.5-r0 description:
development framework configuration tools

pkgconf-1.9.5-r0 webpage:
https://gitea.treehouse.systems/ariadne/pkgconf

pkgconf-1.9.5-r0 installed size:
164 KiB

pkgconf-1.9.5-r0 license:
ISC

```

### `apk` package: `popt`

```console
popt-1.19-r2 description:
commandline option parser

popt-1.19-r2 webpage:
https://github.com/rpm-software-management/popt

popt-1.19-r2 installed size:
56 KiB

popt-1.19-r2 license:
MIT

```

### `apk` package: `readline`

```console
readline-8.2.1-r1 description:
GNU readline library

readline-8.2.1-r1 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.2.1-r1 installed size:
300 KiB

readline-8.2.1-r1 license:
GPL-2.0-or-later

```

### `apk` package: `rsync`

```console
rsync-3.2.7-r4 description:
A file transfer program to keep remote files in sync

rsync-3.2.7-r4 webpage:
https://rsync.samba.org/

rsync-3.2.7-r4 installed size:
412 KiB

rsync-3.2.7-r4 license:
GPL-3.0-or-later

```

### `apk` package: `scanelf`

```console
scanelf-1.3.7-r1 description:
Scan ELF binaries for stuff

scanelf-1.3.7-r1 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.3.7-r1 installed size:
88 KiB

scanelf-1.3.7-r1 license:
GPL-2.0-only

```

### `apk` package: `shared-mime-info`

```console
shared-mime-info-2.2-r5 description:
Freedesktop.org Shared MIME Info

shared-mime-info-2.2-r5 webpage:
https://freedesktop.org/Software/shared-mime-info

shared-mime-info-2.2-r5 installed size:
2452 KiB

shared-mime-info-2.2-r5 license:
GPL-2.0-or-later

```

### `apk` package: `sqlite-libs`

```console
sqlite-libs-3.41.2-r2 description:
C library that implements an SQL database engine (libraries)

sqlite-libs-3.41.2-r2 webpage:
https://www.sqlite.org/

sqlite-libs-3.41.2-r2 installed size:
976 KiB

sqlite-libs-3.41.2-r2 license:
blessing

```

### `apk` package: `ssl_client`

```console
ssl_client-1.36.1-r2 description:
EXternal ssl_client for busybox wget

ssl_client-1.36.1-r2 webpage:
https://busybox.net/

ssl_client-1.36.1-r2 installed size:
28 KiB

ssl_client-1.36.1-r2 license:
GPL-2.0-only

```

### `apk` package: `tar`

```console
tar-1.34-r3 description:
Utility used to store, backup, and transport files

tar-1.34-r3 webpage:
https://www.gnu.org/software/tar/

tar-1.34-r3 installed size:
468 KiB

tar-1.34-r3 license:
GPL-3.0-or-later

```

### `apk` package: `tiff`

```console
tiff-4.5.1-r0 description:
Provides support for the Tag Image File Format or TIFF

tiff-4.5.1-r0 webpage:
https://gitlab.com/libtiff/libtiff

tiff-4.5.1-r0 installed size:
448 KiB

tiff-4.5.1-r0 license:
libtiff

```

### `apk` package: `x265-libs`

```console
x265-libs-3.5-r4 description:
Open Source H265/HEVC video encoder (libraries)

x265-libs-3.5-r4 webpage:
https://www.videolan.org/developers/x265.html

x265-libs-3.5-r4 installed size:
18 MiB

x265-libs-3.5-r4 license:
GPL-2.0-or-later

```

### `apk` package: `xz`

```console
xz-5.4.3-r0 description:
Library and CLI tools for XZ and LZMA compressed files

xz-5.4.3-r0 webpage:
https://tukaani.org/xz

xz-5.4.3-r0 installed size:
172 KiB

xz-5.4.3-r0 license:
GPL-2.0-or-later AND Public-Domain AND LGPL-2.1-or-later

```

### `apk` package: `xz-libs`

```console
xz-libs-5.4.3-r0 description:
Library and CLI tools for XZ and LZMA compressed files (libraries)

xz-libs-5.4.3-r0 webpage:
https://tukaani.org/xz

xz-libs-5.4.3-r0 installed size:
232 KiB

xz-libs-5.4.3-r0 license:
GPL-2.0-or-later AND Public-Domain AND LGPL-2.1-or-later

```

### `apk` package: `zlib`

```console
zlib-1.2.13-r1 description:
A compression/decompression Library

zlib-1.2.13-r1 webpage:
https://zlib.net/

zlib-1.2.13-r1 installed size:
108 KiB

zlib-1.2.13-r1 license:
Zlib

```

### `apk` package: `zstd-libs`

```console
zstd-libs-1.5.5-r4 description:
Zstandard - Fast real-time compression algorithm (libraries)

zstd-libs-1.5.5-r4 webpage:
https://www.zstd.net/

zstd-libs-1.5.5-r4 installed size:
736 KiB

zstd-libs-1.5.5-r4 license:
BSD-3-Clause GPL-2.0-or-later

```
