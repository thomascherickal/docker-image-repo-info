# `wordpress:5.3.2-php7.2-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:028223050414ee033d909713a9b8e620bc8d65550aa157e4b4353496fb78c91a`
- Created: `2019-12-20T01:50:25.818619206Z`
- Virtual Size: ~ 195.22 Mb  
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
  - `GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F`
  - `PHP_VERSION=7.2.26`
  - `PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror`
  - `PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror`
  - `PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d`
  - `PHP_MD5=`
  - `WORDPRESS_VERSION=5.3.2`
  - `WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b`

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

### `apk` package: `avahi-libs`

```console
avahi-libs-0.7-r2 description:
Libraries for avahi run-time use

avahi-libs-0.7-r2 webpage:
https://www.avahi.org/

avahi-libs-0.7-r2 installed size:
131072

avahi-libs-0.7-r2 license:
LGPL-2.0-or-later

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

### `apk` package: `cups-libs`

```console
cups-libs-2.2.12-r0 description:
CUPS libraries

cups-libs-2.2.12-r0 webpage:
https://www.cups.org/

cups-libs-2.2.12-r0 installed size:
565248

cups-libs-2.2.12-r0 license:
GPL-2.0-only

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

### `apk` package: `dbus-libs`

```console
dbus-libs-1.12.16-r0 description:
D-BUS access libraries

dbus-libs-1.12.16-r0 webpage:
https://www.freedesktop.org/Software/dbus

dbus-libs-1.12.16-r0 installed size:
303104

dbus-libs-1.12.16-r0 license:
AFL-2.1 OR GPL-2.0-or-later

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

### `apk` package: `ghostscript`

```console
ghostscript-9.27-r5 description:
An interpreter for the PostScript language and for PDF

ghostscript-9.27-r5 webpage:
https://ghostscript.com/

ghostscript-9.27-r5 installed size:
50642944

ghostscript-9.27-r5 license:
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
gnutls-3.6.8-r0 description:
A TLS protocol implementation

gnutls-3.6.8-r0 webpage:
https://www.gnutls.org/

gnutls-3.6.8-r0 installed size:
1581056

gnutls-3.6.8-r0 license:
GPL-3.0-or-later

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

### `apk` package: `jbig2dec`

```console
jbig2dec-0.16-r0 description:
JBIG2 image compression format decoder

jbig2dec-0.16-r0 webpage:
https://www.ghostscript.com/jbig2dec.html

jbig2dec-0.16-r0 installed size:
143360

jbig2dec-0.16-r0 license:
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
libintl-0.19.8.1-r4 description:
GNU gettext runtime library

libintl-0.19.8.1-r4 webpage:
https://www.gnu.org/software/gettext/gettext.html

libintl-0.19.8.1-r4 installed size:
73728

libintl-0.19.8.1-r4 license:
LGPL-2.1+

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
libssl1.1-1.1.1d-r0 description:
SSL shared libraries

libssl1.1-1.1.1d-r0 webpage:
https://www.openssl.org

libssl1.1-1.1.1d-r0 installed size:
532480

libssl1.1-1.1.1d-r0 license:
OpenSSL

```

### `apk` package: `libtasn1`

```console
libtasn1-4.14-r0 description:
The ASN.1 library used in GNUTLS

libtasn1-4.14-r0 webpage:
https://www.gnu.org/software/gnutls/

libtasn1-4.14-r0 installed size:
135168

libtasn1-4.14-r0 license:
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
1536000

libunistring-0.9.10-r0 license:
GPL-2.0+ OR LGPL-3.0+

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

### `apk` package: `nettle`

```console
nettle-3.4.1-r1 description:
A low-level cryptographic library

nettle-3.4.1-r1 webpage:
http://www.lysator.liu.se/~nisse/nettle/

nettle-3.4.1-r1 installed size:
450560

nettle-3.4.1-r1 license:
LGPL-2.0-or-later

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

### `apk` package: `p11-kit`

```console
p11-kit-0.23.16.1-r0 description:
Library for loading and sharing PKCS#11 modules

p11-kit-0.23.16.1-r0 webpage:
https://p11-glue.freedesktop.org/

p11-kit-0.23.16.1-r0 installed size:
1232896

p11-kit-0.23.16.1-r0 license:
BSD

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

### `apk` package: `sed`

```console
sed-4.7-r0 description:
GNU stream editor

sed-4.7-r0 webpage:
https://www.gnu.org/software/sed

sed-4.7-r0 installed size:
159744

sed-4.7-r0 license:
GPL-3.0+

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

### `apk` package: `tiff`

```console
tiff-4.0.10-r3 description:
Provides support for the Tag Image File Format or TIFF

tiff-4.0.10-r3 webpage:
http://www.libtiff.org

tiff-4.0.10-r3 installed size:
442368

tiff-4.0.10-r3 license:
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
zlib-1.2.11-r1 description:
A compression/decompression Library

zlib-1.2.11-r1 webpage:
http://zlib.net

zlib-1.2.11-r1 installed size:
110592

zlib-1.2.11-r1 license:
zlib

```
