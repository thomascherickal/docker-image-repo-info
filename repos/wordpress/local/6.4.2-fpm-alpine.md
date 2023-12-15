# `wordpress:6.4.2-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:ada068faa2207e3174f8851ff49af6c71588452a29c1ae75d9805509044d3acc`
- Created: `2023-12-06T20:31:30Z`
- Virtual Size: ~ 252.72 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-entrypoint.sh"]`
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

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.4.3-r2 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.4.3-r2 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.4.3-r2 installed size:
324 KiB

alpine-baselayout-3.4.3-r2 license:
GPL-2.0-only

```

### `apk` package: `alpine-baselayout-data`

```console
alpine-baselayout-data-3.4.3-r2 description:
Alpine base dir structure and init scripts

alpine-baselayout-data-3.4.3-r2 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-data-3.4.3-r2 installed size:
76 KiB

alpine-baselayout-data-3.4.3-r2 license:
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

### `apk` package: `apk-tools`

```console
apk-tools-2.14.0-r5 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.14.0-r5 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.14.0-r5 installed size:
304 KiB

apk-tools-2.14.0-r5 license:
GPL-2.0-only

```

### `apk` package: `argon2-libs`

```console
argon2-libs-20190702-r5 description:
The password hash Argon2, winner of PHC (libraries)

argon2-libs-20190702-r5 webpage:
https://github.com/P-H-C/phc-winner-argon2

argon2-libs-20190702-r5 installed size:
52 KiB

argon2-libs-20190702-r5 license:
Apache-2.0 OR CC0-1.0

```

### `apk` package: `avahi-libs`

```console
avahi-libs-0.8-r13 description:
Libraries for avahi run-time use

avahi-libs-0.8-r13 webpage:
https://www.avahi.org/

avahi-libs-0.8-r13 installed size:
120 KiB

avahi-libs-0.8-r13 license:
LGPL-2.1-or-later

```

### `apk` package: `bash`

```console
bash-5.2.21-r0 description:
The GNU Bourne Again shell

bash-5.2.21-r0 webpage:
https://www.gnu.org/software/bash/bash.html

bash-5.2.21-r0 installed size:
1364 KiB

bash-5.2.21-r0 license:
GPL-3.0-or-later

```

### `apk` package: `brotli-libs`

```console
brotli-libs-1.1.0-r1 description:
Generic lossless compressor (libraries)

brotli-libs-1.1.0-r1 webpage:
https://github.com/google/brotli

brotli-libs-1.1.0-r1 installed size:
932 KiB

brotli-libs-1.1.0-r1 license:
MIT

```

### `apk` package: `busybox`

```console
busybox-1.36.1-r15 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.36.1-r15 webpage:
https://busybox.net/

busybox-1.36.1-r15 installed size:
924 KiB

busybox-1.36.1-r15 license:
GPL-2.0-only

```

### `apk` package: `busybox-binsh`

```console
busybox-binsh-1.36.1-r15 description:
busybox ash /bin/sh

busybox-binsh-1.36.1-r15 webpage:
https://busybox.net/

busybox-binsh-1.36.1-r15 installed size:
8192 B

busybox-binsh-1.36.1-r15 license:
GPL-2.0-only

```

### `apk` package: `c-ares`

```console
c-ares-1.22.1-r0 description:
Asynchronous DNS/names resolver library

c-ares-1.22.1-r0 webpage:
https://c-ares.org/

c-ares-1.22.1-r0 installed size:
132 KiB

c-ares-1.22.1-r0 license:
MIT

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
curl-8.5.0-r0 description:
URL retrival utility and library

curl-8.5.0-r0 webpage:
https://curl.se/

curl-8.5.0-r0 installed size:
248 KiB

curl-8.5.0-r0 license:
curl

```

### `apk` package: `dbus-libs`

```console
dbus-libs-1.14.10-r0 description:
D-BUS access libraries

dbus-libs-1.14.10-r0 webpage:
https://www.freedesktop.org/Software/dbus

dbus-libs-1.14.10-r0 installed size:
288 KiB

dbus-libs-1.14.10-r0 license:
AFL-2.1 OR GPL-2.0-or-later

```

### `apk` package: `fftw-double-libs`

```console
fftw-double-libs-3.3.10-r5 description:
Discrete Fourier transform (DFT) library

fftw-double-libs-3.3.10-r5 webpage:
http://www.fftw.org/

fftw-double-libs-3.3.10-r5 installed size:
2028 KiB

fftw-double-libs-3.3.10-r5 license:
GPL-2.0-or-later

```

### `apk` package: `fontconfig`

```console
fontconfig-2.14.2-r4 description:
Library for configuring and customizing font access

fontconfig-2.14.2-r4 webpage:
https://www.freedesktop.org/wiki/Software/fontconfig

fontconfig-2.14.2-r4 installed size:
708 KiB

fontconfig-2.14.2-r4 license:
MIT

```

### `apk` package: `freetype`

```console
freetype-2.13.2-r0 description:
TrueType font rendering library

freetype-2.13.2-r0 webpage:
https://www.freetype.org/

freetype-2.13.2-r0 installed size:
664 KiB

freetype-2.13.2-r0 license:
FTL OR GPL-2.0-or-later

```

### `apk` package: `ghostscript`

```console
ghostscript-10.02.1-r0 description:
Interpreter for the PostScript language and for PDF

ghostscript-10.02.1-r0 webpage:
https://ghostscript.com/

ghostscript-10.02.1-r0 installed size:
63 MiB

ghostscript-10.02.1-r0 license:
AGPL-3.0-or-later

```

### `apk` package: `gmp`

```console
gmp-6.3.0-r0 description:
free library for arbitrary precision arithmetic

gmp-6.3.0-r0 webpage:
https://gmplib.org/

gmp-6.3.0-r0 installed size:
432 KiB

gmp-6.3.0-r0 license:
LGPL-3.0-or-later OR GPL-2.0-or-later

```

### `apk` package: `gnu-libiconv-libs`

```console
gnu-libiconv-libs-1.17-r2 description:
GNU charset conversion library for libc which doesn't implement it (libraries)

gnu-libiconv-libs-1.17-r2 webpage:
https://www.gnu.org/software/libiconv

gnu-libiconv-libs-1.17-r2 installed size:
1064 KiB

gnu-libiconv-libs-1.17-r2 license:
LGPL-2.1-or-later

```

### `apk` package: `gnutls`

```console
gnutls-3.8.1-r0 description:
TLS protocol implementation

gnutls-3.8.1-r0 webpage:
https://www.gnutls.org/

gnutls-3.8.1-r0 installed size:
1852 KiB

gnutls-3.8.1-r0 license:
LGPL-2.1-or-later

```

### `apk` package: `icu-data-en`

```console
icu-data-en-74.1-r0 description:
Stripped down ICU data with only en_US/GB locale and no legacy charset converters

icu-data-en-74.1-r0 webpage:
https://icu.unicode.org/

icu-data-en-74.1-r0 installed size:
2756 KiB

icu-data-en-74.1-r0 license:
ICU

```

### `apk` package: `icu-libs`

```console
icu-libs-74.1-r0 description:
International Components for Unicode library (libraries)

icu-libs-74.1-r0 webpage:
https://icu.unicode.org/

icu-libs-74.1-r0 installed size:
4408 KiB

icu-libs-74.1-r0 license:
ICU

```

### `apk` package: `imagemagick`

```console
imagemagick-7.1.1.22-r0 description:
Collection of tools and libraries for many image formats

imagemagick-7.1.1.22-r0 webpage:
https://imagemagick.org/

imagemagick-7.1.1.22-r0 installed size:
4332 KiB

imagemagick-7.1.1.22-r0 license:
ImageMagick

```

### `apk` package: `imagemagick-jpeg`

```console
imagemagick-jpeg-7.1.1.22-r0 description:
Collection of tools and libraries for many image formats (JPEG support modules)

imagemagick-jpeg-7.1.1.22-r0 webpage:
https://imagemagick.org/

imagemagick-jpeg-7.1.1.22-r0 installed size:
84 KiB

imagemagick-jpeg-7.1.1.22-r0 license:
ImageMagick

```

### `apk` package: `imagemagick-libs`

```console
imagemagick-libs-7.1.1.22-r0 description:
Collection of tools and libraries for many image formats (libraries)

imagemagick-libs-7.1.1.22-r0 webpage:
https://imagemagick.org/

imagemagick-libs-7.1.1.22-r0 installed size:
4152 KiB

imagemagick-libs-7.1.1.22-r0 license:
ImageMagick

```

### `apk` package: `imagemagick-pdf`

```console
imagemagick-pdf-7.1.1.22-r0 description:
Collection of tools and libraries for many image formats (PDF support modules)

imagemagick-pdf-7.1.1.22-r0 webpage:
https://imagemagick.org/

imagemagick-pdf-7.1.1.22-r0 installed size:
156 KiB

imagemagick-pdf-7.1.1.22-r0 license:
ImageMagick

```

### `apk` package: `imagemagick-tiff`

```console
imagemagick-tiff-7.1.1.22-r0 description:
Collection of tools and libraries for many image formats (TIFF support modules)

imagemagick-tiff-7.1.1.22-r0 webpage:
https://imagemagick.org/

imagemagick-tiff-7.1.1.22-r0 installed size:
144 KiB

imagemagick-tiff-7.1.1.22-r0 license:
ImageMagick

```

### `apk` package: `imagemagick-webp`

```console
imagemagick-webp-7.1.1.22-r0 description:
Collection of tools and libraries for many image formats (WebP support modules)

imagemagick-webp-7.1.1.22-r0 webpage:
https://imagemagick.org/

imagemagick-webp-7.1.1.22-r0 installed size:
56 KiB

imagemagick-webp-7.1.1.22-r0 license:
ImageMagick

```

### `apk` package: `jbig2dec`

```console
jbig2dec-0.20-r0 description:
JBIG2 image compression format decoder

jbig2dec-0.20-r0 webpage:
https://jbig2dec.com/

jbig2dec-0.20-r0 installed size:
148 KiB

jbig2dec-0.20-r0 license:
AGPL-3.0-or-later

```

### `apk` package: `lcms2`

```console
lcms2-2.15-r4 description:
Color Management Engine

lcms2-2.15-r4 webpage:
https://www.littlecms.com

lcms2-2.15-r4 installed size:
336 KiB

lcms2-2.15-r4 license:
MIT

```

### `apk` package: `libacl`

```console
libacl-2.3.1-r4 description:
Dynamic library for access control list support

libacl-2.3.1-r4 webpage:
https://savannah.nongnu.org/projects/acl

libacl-2.3.1-r4 installed size:
44 KiB

libacl-2.3.1-r4 license:
LGPL-2.1-or-later AND GPL-2.0-or-later

```

### `apk` package: `libbsd`

```console
libbsd-0.11.7-r3 description:
commonly-used BSD functions not implemented by all libcs

libbsd-0.11.7-r3 webpage:
https://libbsd.freedesktop.org/

libbsd-0.11.7-r3 installed size:
84 KiB

libbsd-0.11.7-r3 license:
BSD-3-Clause

```

### `apk` package: `libbz2`

```console
libbz2-1.0.8-r6 description:
Shared library for bz2

libbz2-1.0.8-r6 webpage:
https://sourceware.org/bzip2/

libbz2-1.0.8-r6 installed size:
88 KiB

libbz2-1.0.8-r6 license:
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
libcrypto3-3.1.4-r2 description:
Crypto library from openssl

libcrypto3-3.1.4-r2 webpage:
https://www.openssl.org/

libcrypto3-3.1.4-r2 installed size:
4500 KiB

libcrypto3-3.1.4-r2 license:
Apache-2.0

```

### `apk` package: `libcurl`

```console
libcurl-8.5.0-r0 description:
The multiprotocol file transfer library

libcurl-8.5.0-r0 webpage:
https://curl.se/

libcurl-8.5.0-r0 installed size:
580 KiB

libcurl-8.5.0-r0 license:
curl

```

### `apk` package: `libexpat`

```console
libexpat-2.5.0-r2 description:
XML Parser library written in C (libraries)

libexpat-2.5.0-r2 webpage:
https://libexpat.github.io/

libexpat-2.5.0-r2 installed size:
144 KiB

libexpat-2.5.0-r2 license:
MIT

```

### `apk` package: `libffi`

```console
libffi-3.4.4-r3 description:
portable, high level programming interface to various calling conventions.

libffi-3.4.4-r3 webpage:
https://sourceware.org/libffi/

libffi-3.4.4-r3 installed size:
52 KiB

libffi-3.4.4-r3 license:
MIT

```

### `apk` package: `libgcc`

```console
libgcc-13.2.1_git20231014-r0 description:
GNU C compiler runtime libraries

libgcc-13.2.1_git20231014-r0 webpage:
https://gcc.gnu.org

libgcc-13.2.1_git20231014-r0 installed size:
152 KiB

libgcc-13.2.1_git20231014-r0 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `libgomp`

```console
libgomp-13.2.1_git20231014-r0 description:
GCC shared-memory parallel programming API library

libgomp-13.2.1_git20231014-r0 webpage:
https://gcc.gnu.org

libgomp-13.2.1_git20231014-r0 installed size:
324 KiB

libgomp-13.2.1_git20231014-r0 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `libidn2`

```console
libidn2-2.3.4-r4 description:
Encode/Decode library for internationalized domain names

libidn2-2.3.4-r4 webpage:
https://www.gnu.org/software/libidn#libidn2

libidn2-2.3.4-r4 installed size:
208 KiB

libidn2-2.3.4-r4 license:
GPL-2.0-or-later OR LGPL-3.0-or-later

```

### `apk` package: `libintl`

```console
libintl-0.22.3-r0 description:
GNU gettext runtime library

libintl-0.22.3-r0 webpage:
https://www.gnu.org/software/gettext/gettext.html

libintl-0.22.3-r0 installed size:
80 KiB

libintl-0.22.3-r0 license:
LGPL-2.1-or-later

```

### `apk` package: `libjpeg-turbo`

```console
libjpeg-turbo-3.0.1-r0 description:
Accelerated baseline JPEG compression and decompression library

libjpeg-turbo-3.0.1-r0 webpage:
https://libjpeg-turbo.org/

libjpeg-turbo-3.0.1-r0 installed size:
696 KiB

libjpeg-turbo-3.0.1-r0 license:
BSD-3-Clause AND IJG AND Zlib

```

### `apk` package: `libltdl`

```console
libltdl-2.4.7-r3 description:
Runtime libraries for GNU Libtool Dynamic Module Loader

libltdl-2.4.7-r3 webpage:
https://www.gnu.org/software/libtool

libltdl-2.4.7-r3 installed size:
52 KiB

libltdl-2.4.7-r3 license:
LGPL-2.0-or-later AND GPL-2.0-or-later

```

### `apk` package: `libmd`

```console
libmd-1.1.0-r0 description:
Message Digest functions from BSD systems

libmd-1.1.0-r0 webpage:
https://www.hadrons.org/software/libmd/

libmd-1.1.0-r0 installed size:
64 KiB

libmd-1.1.0-r0 license:
BSD-3-Clause AND BSD-2-Clause AND ISC AND Beerware AND Public Domain

```

### `apk` package: `libncursesw`

```console
libncursesw-6.4_p20231125-r0 description:
Console display library (libncursesw)

libncursesw-6.4_p20231125-r0 webpage:
https://invisible-island.net/ncurses/

libncursesw-6.4_p20231125-r0 installed size:
344 KiB

libncursesw-6.4_p20231125-r0 license:
X11

```

### `apk` package: `libpng`

```console
libpng-1.6.40-r0 description:
Portable Network Graphics library

libpng-1.6.40-r0 webpage:
http://www.libpng.org

libpng-1.6.40-r0 installed size:
200 KiB

libpng-1.6.40-r0 license:
Libpng

```

### `apk` package: `libsharpyuv`

```console
libsharpyuv-1.3.2-r0 description:
Libraries for working with WebP images (libsharpyuv library)

libsharpyuv-1.3.2-r0 webpage:
https://developers.google.com/speed/webp

libsharpyuv-1.3.2-r0 installed size:
36 KiB

libsharpyuv-1.3.2-r0 license:
BSD-3-Clause

```

### `apk` package: `libsodium`

```console
libsodium-1.0.19-r0 description:
P(ortable|ackageable) NaCl-based crypto library

libsodium-1.0.19-r0 webpage:
https://github.com/jedisct1/libsodium

libsodium-1.0.19-r0 installed size:
348 KiB

libsodium-1.0.19-r0 license:
ISC

```

### `apk` package: `libssl3`

```console
libssl3-3.1.4-r2 description:
SSL shared libraries

libssl3-3.1.4-r2 webpage:
https://www.openssl.org/

libssl3-3.1.4-r2 installed size:
548 KiB

libssl3-3.1.4-r2 license:
Apache-2.0

```

### `apk` package: `libstdc++`

```console
libstdc++-13.2.1_git20231014-r0 description:
GNU C++ standard runtime library

libstdc++-13.2.1_git20231014-r0 webpage:
https://gcc.gnu.org

libstdc++-13.2.1_git20231014-r0 installed size:
2652 KiB

libstdc++-13.2.1_git20231014-r0 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `libtasn1`

```console
libtasn1-4.19.0-r2 description:
The ASN.1 library used in GNUTLS

libtasn1-4.19.0-r2 webpage:
https://www.gnu.org/software/gnutls/

libtasn1-4.19.0-r2 installed size:
80 KiB

libtasn1-4.19.0-r2 license:
LGPL-2.1-or-later

```

### `apk` package: `libunistring`

```console
libunistring-1.1-r2 description:
Library for manipulating Unicode strings and C strings

libunistring-1.1-r2 webpage:
https://www.gnu.org/software/libunistring/

libunistring-1.1-r2 installed size:
1664 KiB

libunistring-1.1-r2 license:
GPL-2.0-or-later OR LGPL-3.0-or-later

```

### `apk` package: `libwebp`

```console
libwebp-1.3.2-r0 description:
Libraries for working with WebP images

libwebp-1.3.2-r0 webpage:
https://developers.google.com/speed/webp

libwebp-1.3.2-r0 installed size:
468 KiB

libwebp-1.3.2-r0 license:
BSD-3-Clause

```

### `apk` package: `libwebpdemux`

```console
libwebpdemux-1.3.2-r0 description:
Libraries for working with WebP images (libwebpdemux library)

libwebpdemux-1.3.2-r0 webpage:
https://developers.google.com/speed/webp

libwebpdemux-1.3.2-r0 installed size:
32 KiB

libwebpdemux-1.3.2-r0 license:
BSD-3-Clause

```

### `apk` package: `libwebpmux`

```console
libwebpmux-1.3.2-r0 description:
Libraries for working with WebP images (libwebpmux library)

libwebpmux-1.3.2-r0 webpage:
https://developers.google.com/speed/webp

libwebpmux-1.3.2-r0 installed size:
60 KiB

libwebpmux-1.3.2-r0 license:
BSD-3-Clause

```

### `apk` package: `libx11`

```console
libx11-1.8.7-r0 description:
X11 client-side library

libx11-1.8.7-r0 webpage:
https://xorg.freedesktop.org/

libx11-1.8.7-r0 installed size:
3084 KiB

libx11-1.8.7-r0 license:
X11

```

### `apk` package: `libxau`

```console
libxau-1.0.11-r3 description:
X11 authorisation library

libxau-1.0.11-r3 webpage:
https://xorg.freedesktop.org/

libxau-1.0.11-r3 installed size:
28 KiB

libxau-1.0.11-r3 license:
MIT

```

### `apk` package: `libxcb`

```console
libxcb-1.16-r0 description:
X11 client-side library

libxcb-1.16-r0 webpage:
https://xcb.freedesktop.org

libxcb-1.16-r0 installed size:
1012 KiB

libxcb-1.16-r0 license:
MIT

```

### `apk` package: `libxdmcp`

```console
libxdmcp-1.1.4-r3 description:
X11 Display Manager Control Protocol library

libxdmcp-1.1.4-r3 webpage:
https://xorg.freedesktop.org/

libxdmcp-1.1.4-r3 installed size:
40 KiB

libxdmcp-1.1.4-r3 license:
MIT

```

### `apk` package: `libxext`

```console
libxext-1.3.5-r3 description:
X11 miscellaneous extensions library

libxext-1.3.5-r3 webpage:
https://xorg.freedesktop.org/

libxext-1.3.5-r3 installed size:
80 KiB

libxext-1.3.5-r3 license:
MIT

```

### `apk` package: `libxml2`

```console
libxml2-2.11.6-r0 description:
XML parsing library, version 2

libxml2-2.11.6-r0 webpage:
https://gitlab.gnome.org/GNOME/libxml2

libxml2-2.11.6-r0 installed size:
1092 KiB

libxml2-2.11.6-r0 license:
MIT

```

### `apk` package: `libzip`

```console
libzip-1.10.1-r0 description:
C library for manipulating zip archives

libzip-1.10.1-r0 webpage:
https://libzip.org/

libzip-1.10.1-r0 installed size:
112 KiB

libzip-1.10.1-r0 license:
BSD-3-Clause

```

### `apk` package: `musl`

```console
musl-1.2.4_git20230717-r4 description:
the musl c library (libc) implementation

musl-1.2.4_git20230717-r4 webpage:
https://musl.libc.org/

musl-1.2.4_git20230717-r4 installed size:
652 KiB

musl-1.2.4_git20230717-r4 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.2.4_git20230717-r4 description:
the musl c library (libc) implementation

musl-utils-1.2.4_git20230717-r4 webpage:
https://musl.libc.org/

musl-utils-1.2.4_git20230717-r4 installed size:
128 KiB

musl-utils-1.2.4_git20230717-r4 license:
MIT AND BSD-2-Clause AND GPL-2.0-or-later

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.4_p20231125-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.4_p20231125-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-base-6.4_p20231125-r0 installed size:
212 KiB

ncurses-terminfo-base-6.4_p20231125-r0 license:
X11

```

### `apk` package: `nettle`

```console
nettle-3.9.1-r0 description:
Low-level cryptographic library

nettle-3.9.1-r0 webpage:
https://www.lysator.liu.se/~nisse/nettle/

nettle-3.9.1-r0 installed size:
592 KiB

nettle-3.9.1-r0 license:
GPL-2.0-or-later OR LGPL-3.0-or-later

```

### `apk` package: `nghttp2-libs`

```console
nghttp2-libs-1.58.0-r0 description:
HTTP/2 C client, server and proxy (libraries)

nghttp2-libs-1.58.0-r0 webpage:
https://nghttp2.org

nghttp2-libs-1.58.0-r0 installed size:
152 KiB

nghttp2-libs-1.58.0-r0 license:
MIT

```

### `apk` package: `oniguruma`

```console
oniguruma-6.9.9-r0 description:
a regular expressions library

oniguruma-6.9.9-r0 webpage:
https://github.com/kkos/oniguruma

oniguruma-6.9.9-r0 installed size:
552 KiB

oniguruma-6.9.9-r0 license:
BSD-2-Clause

```

### `apk` package: `openssl`

```console
openssl-3.1.4-r2 description:
Toolkit for Transport Layer Security (TLS)

openssl-3.1.4-r2 webpage:
https://www.openssl.org/

openssl-3.1.4-r2 installed size:
732 KiB

openssl-3.1.4-r2 license:
Apache-2.0

```

### `apk` package: `p11-kit`

```console
p11-kit-0.25.3-r0 description:
Library for loading and sharing PKCS#11 modules

p11-kit-0.25.3-r0 webpage:
https://p11-glue.freedesktop.org/

p11-kit-0.25.3-r0 installed size:
1400 KiB

p11-kit-0.25.3-r0 license:
BSD-3-Clause

```

### `apk` package: `readline`

```console
readline-8.2.1-r2 description:
GNU readline library

readline-8.2.1-r2 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.2.1-r2 installed size:
296 KiB

readline-8.2.1-r2 license:
GPL-2.0-or-later

```

### `apk` package: `scanelf`

```console
scanelf-1.3.7-r2 description:
Scan ELF binaries for stuff

scanelf-1.3.7-r2 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.3.7-r2 installed size:
80 KiB

scanelf-1.3.7-r2 license:
GPL-2.0-only

```

### `apk` package: `sqlite-libs`

```console
sqlite-libs-3.44.2-r0 description:
C library that implements an SQL database engine (libraries)

sqlite-libs-3.44.2-r0 webpage:
https://www.sqlite.org/

sqlite-libs-3.44.2-r0 installed size:
1412 KiB

sqlite-libs-3.44.2-r0 license:
blessing

```

### `apk` package: `ssl_client`

```console
ssl_client-1.36.1-r15 description:
EXternal ssl_client for busybox wget

ssl_client-1.36.1-r15 webpage:
https://busybox.net/

ssl_client-1.36.1-r15 installed size:
28 KiB

ssl_client-1.36.1-r15 license:
GPL-2.0-only

```

### `apk` package: `tar`

```console
tar-1.35-r2 description:
Utility used to store, backup, and transport files

tar-1.35-r2 webpage:
https://www.gnu.org/software/tar/

tar-1.35-r2 installed size:
428 KiB

tar-1.35-r2 license:
GPL-3.0-or-later

```

### `apk` package: `tiff`

```console
tiff-4.6.0-r0 description:
Provides support for the Tag Image File Format or TIFF

tiff-4.6.0-r0 webpage:
https://gitlab.com/libtiff/libtiff

tiff-4.6.0-r0 installed size:
456 KiB

tiff-4.6.0-r0 license:
libtiff

```

### `apk` package: `xz`

```console
xz-5.4.5-r0 description:
Library and CLI tools for XZ and LZMA compressed files

xz-5.4.5-r0 webpage:
https://tukaani.org/xz

xz-5.4.5-r0 installed size:
172 KiB

xz-5.4.5-r0 license:
GPL-2.0-or-later AND Public-Domain AND LGPL-2.1-or-later

```

### `apk` package: `xz-libs`

```console
xz-libs-5.4.5-r0 description:
Library and CLI tools for XZ and LZMA compressed files (libraries)

xz-libs-5.4.5-r0 webpage:
https://tukaani.org/xz

xz-libs-5.4.5-r0 installed size:
232 KiB

xz-libs-5.4.5-r0 license:
GPL-2.0-or-later AND Public-Domain AND LGPL-2.1-or-later

```

### `apk` package: `zlib`

```console
zlib-1.3-r2 description:
A compression/decompression Library

zlib-1.3-r2 webpage:
https://zlib.net/

zlib-1.3-r2 installed size:
108 KiB

zlib-1.3-r2 license:
Zlib

```

### `apk` package: `zstd-libs`

```console
zstd-libs-1.5.5-r8 description:
Zstandard - Fast real-time compression algorithm (libraries)

zstd-libs-1.5.5-r8 webpage:
https://www.zstd.net/

zstd-libs-1.5.5-r8 installed size:
712 KiB

zstd-libs-1.5.5-r8 license:
BSD-3-Clause OR GPL-2.0-or-later

```
