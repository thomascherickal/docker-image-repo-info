# `phpmyadmin:5.0.2-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:acaf66e70db555ca237719af1cf2fd4cc3ec55af2600ceb756062928395375c1`
- Created: `2020-08-27T00:23:29.442459626Z`
- Virtual Size: ~ 140.89 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/docker-entrypoint.sh"]`
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
  - `PHP_VERSION=7.4.9`
  - `PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc`
  - `PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b`
  - `PHP_MD5=`
  - `VERSION=5.0.2`
  - `SHA256=cbcc78d1499308d9329950fcba2ebaa84c559a934fe54efc027d459d8e4161c8`
  - `URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.2/phpMyAdmin-5.0.2-all-languages.tar.xz`
- Labels:
  - `org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net>`
  - `org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM.`
  - `org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme`
  - `org.opencontainers.image.licenses=GPL-2.0-only`
  - `org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git`
  - `org.opencontainers.image.title=Official phpMyAdmin Docker image`
  - `org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme`
  - `org.opencontainers.image.vendor=phpMyAdmin`
  - `org.opencontainers.image.version=5.0.2`

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
libcurl-7.69.1-r0 description:
The multiprotocol file transfer library

libcurl-7.69.1-r0 webpage:
https://curl.haxx.se/

libcurl-7.69.1-r0 installed size:
458752

libcurl-7.69.1-r0 license:
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

### `apk` package: `libice`

```console
libice-1.0.10-r0 description:
X11 Inter-Client Exchange library

libice-1.0.10-r0 webpage:
http://xorg.freedesktop.org/

libice-1.0.10-r0 installed size:
106496

libice-1.0.10-r0 license:
X11

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

### `apk` package: `libsm`

```console
libsm-1.2.3-r0 description:
X11 Session Management library

libsm-1.2.3-r0 webpage:
https://xorg.freedesktop.org/

libsm-1.2.3-r0 installed size:
49152

libsm-1.2.3-r0 license:
MIT

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

### `apk` package: `libwebp`

```console
libwebp-1.1.0-r0 description:
Libraries for working with WebP images

libwebp-1.1.0-r0 webpage:
https://developers.google.com/speed/webp

libwebp-1.1.0-r0 installed size:
589824

libwebp-1.1.0-r0 license:
BSD-3-Clause

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
libxml2-2.9.10-r4 description:
XML parsing library, version 2

libxml2-2.9.10-r4 webpage:
http://www.xmlsoft.org/

libxml2-2.9.10-r4 installed size:
1220608

libxml2-2.9.10-r4 license:
MIT

```

### `apk` package: `libxpm`

```console
libxpm-3.5.13-r0 description:
X11 pixmap library

libxpm-3.5.13-r0 webpage:
http://xorg.freedesktop.org/

libxpm-3.5.13-r0 installed size:
139264

libxpm-3.5.13-r0 license:
custom:BELL

```

### `apk` package: `libxt`

```console
libxt-1.2.0-r0 description:
X11 toolkit intrinsics library

libxt-1.2.0-r0 webpage:
http://xorg.freedesktop.org/

libxt-1.2.0-r0 installed size:
376832

libxt-1.2.0-r0 license:
custom

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

### `apk` package: `oniguruma`

```console
oniguruma-6.9.5-r1 description:
a regular expressions library

oniguruma-6.9.5-r1 webpage:
https://github.com/kkos/oniguruma

oniguruma-6.9.5-r1 installed size:
569344

oniguruma-6.9.5-r1 license:
BSD-2-Clause

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

### `apk` package: `tzdata`

```console
tzdata-2020a-r0 description:
Timezone data

tzdata-2020a-r0 webpage:
https://www.iana.org/time-zones

tzdata-2020a-r0 installed size:
3526656

tzdata-2020a-r0 license:
Public-Domain

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
