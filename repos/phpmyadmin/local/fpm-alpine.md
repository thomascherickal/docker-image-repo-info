# `phpmyadmin:5.1.1-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:1db219a4bd1871f3a3178b849fa53a8cdeb9f26734d378c34e8c0f4f63fe3ff5`
- Created: `2021-06-29T04:54:28.902975521Z`
- Virtual Size: ~ 146.06 Mb  
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
  - `PHP_VERSION=7.4.20`
  - `PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc`
  - `PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335`
  - `MAX_EXECUTION_TIME=600`
  - `MEMORY_LIMIT=512M`
  - `UPLOAD_LIMIT=2048K`
  - `VERSION=5.1.1`
  - `SHA256=1964d7190223c11e89fa1b7970c618e3a3bae2e859f5f60383f64c3848ef6921`
  - `URL=https://files.phpmyadmin.net/phpMyAdmin/5.1.1/phpMyAdmin-5.1.1-all-languages.tar.xz`
- Labels:
  - `org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net>`
  - `org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM.`
  - `org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme`
  - `org.opencontainers.image.licenses=GPL-2.0-only`
  - `org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git`
  - `org.opencontainers.image.title=Official phpMyAdmin Docker image`
  - `org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme`
  - `org.opencontainers.image.vendor=phpMyAdmin`
  - `org.opencontainers.image.version=5.1.1`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.2.0-r15 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.2.0-r15 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.2.0-r15 installed size:
404 KiB

alpine-baselayout-3.2.0-r15 license:
GPL-2.0-only

```

### `apk` package: `alpine-keys`

```console
alpine-keys-2.3-r1 description:
Public keys for Alpine Linux packages

alpine-keys-2.3-r1 webpage:
https://alpinelinux.org

alpine-keys-2.3-r1 installed size:
116 KiB

alpine-keys-2.3-r1 license:
MIT

```

### `apk` package: `apk-tools`

```console
apk-tools-2.12.5-r1 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.12.5-r1 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.12.5-r1 installed size:
304 KiB

apk-tools-2.12.5-r1 license:
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
bash-5.1.4-r0 description:
The GNU Bourne Again shell

bash-5.1.4-r0 webpage:
https://www.gnu.org/software/bash/bash.html

bash-5.1.4-r0 installed size:
1296 KiB

bash-5.1.4-r0 license:
GPL-3.0-or-later

```

### `apk` package: `brotli-libs`

```console
brotli-libs-1.0.9-r5 description:
Generic lossless compressor (libraries)

brotli-libs-1.0.9-r5 webpage:
https://github.com/google/brotli

brotli-libs-1.0.9-r5 installed size:
720 KiB

brotli-libs-1.0.9-r5 license:
MIT

```

### `apk` package: `busybox`

```console
busybox-1.33.1-r2 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.33.1-r2 webpage:
https://busybox.net/

busybox-1.33.1-r2 installed size:
928 KiB

busybox-1.33.1-r2 license:
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
curl-7.77.0-r1 description:
URL retrival utility and library

curl-7.77.0-r1 webpage:
https://curl.se/

curl-7.77.0-r1 installed size:
244 KiB

curl-7.77.0-r1 license:
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
libbsd-0.11.3-r0 description:
commonly-used BSD functions not implemented by all libcs

libbsd-0.11.3-r0 webpage:
https://libbsd.freedesktop.org/

libbsd-0.11.3-r0 installed size:
80 KiB

libbsd-0.11.3-r0 license:
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
libcurl-7.77.0-r1 description:
The multiprotocol file transfer library

libcurl-7.77.0-r1 webpage:
https://curl.se/

libcurl-7.77.0-r1 installed size:
500 KiB

libcurl-7.77.0-r1 license:
MIT

```

### `apk` package: `libedit`

```console
libedit-20210216.3.1-r0 description:
BSD line editing library

libedit-20210216.3.1-r0 webpage:
https://www.thrysoee.dk/editline

libedit-20210216.3.1-r0 installed size:
196 KiB

libedit-20210216.3.1-r0 license:
BSD-3-Clause

```

### `apk` package: `libice`

```console
libice-1.0.10-r0 description:
X11 Inter-Client Exchange library

libice-1.0.10-r0 webpage:
http://xorg.freedesktop.org/

libice-1.0.10-r0 installed size:
104 KiB

libice-1.0.10-r0 license:
X11

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

### `apk` package: `libmd`

```console
libmd-1.0.3-r0 description:
Message Digest functions from BSD systems

libmd-1.0.3-r0 webpage:
https://www.hadrons.org/software/libmd/

libmd-1.0.3-r0 installed size:
56 KiB

libmd-1.0.3-r0 license:
Public Domain

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

### `apk` package: `libretls`

```console
libretls-3.3.3-r0 description:
port of libtls from libressl to openssl

libretls-3.3.3-r0 webpage:
https://git.causal.agency/libretls/

libretls-3.3.3-r0 installed size:
84 KiB

libretls-3.3.3-r0 license:
ISC AND (BSD-3-Clause OR MIT)

```

### `apk` package: `libsm`

```console
libsm-1.2.3-r0 description:
X11 Session Management library

libsm-1.2.3-r0 webpage:
https://xorg.freedesktop.org/

libsm-1.2.3-r0 installed size:
48 KiB

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

### `apk` package: `libuuid`

```console
libuuid-2.37-r0 description:
DCE compatible Universally Unique Identifier library

libuuid-2.37-r0 webpage:
https://git.kernel.org/cgit/utils/util-linux/util-linux.git

libuuid-2.37-r0 installed size:
40 KiB

libuuid-2.37-r0 license:
GPL-3.0-or-later AND GPL-2.0-or-later AND GPL-2.0-only AND

```

### `apk` package: `libwebp`

```console
libwebp-1.2.0-r2 description:
Libraries for working with WebP images

libwebp-1.2.0-r2 webpage:
https://developers.google.com/speed/webp

libwebp-1.2.0-r2 installed size:
580 KiB

libwebp-1.2.0-r2 license:
BSD-3-Clause

```

### `apk` package: `libx11`

```console
libx11-1.7.2-r0 description:
X11 client-side library

libx11-1.7.2-r0 webpage:
http://xorg.freedesktop.org/

libx11-1.7.2-r0 installed size:
3240 KiB

libx11-1.7.2-r0 license:
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
libxcb-1.14-r2 description:
X11 client-side library

libxcb-1.14-r2 webpage:
https://xcb.freedesktop.org

libxcb-1.14-r2 installed size:
996 KiB

libxcb-1.14-r2 license:
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
libxml2-2.9.12-r1 description:
XML parsing library, version 2

libxml2-2.9.12-r1 webpage:
http://www.xmlsoft.org/

libxml2-2.9.12-r1 installed size:
1200 KiB

libxml2-2.9.12-r1 license:
MIT

```

### `apk` package: `libxpm`

```console
libxpm-3.5.13-r0 description:
X11 pixmap library

libxpm-3.5.13-r0 webpage:
http://xorg.freedesktop.org/

libxpm-3.5.13-r0 installed size:
136 KiB

libxpm-3.5.13-r0 license:
custom:BELL

```

### `apk` package: `libxt`

```console
libxt-1.2.1-r0 description:
X11 toolkit intrinsics library

libxt-1.2.1-r0 webpage:
http://xorg.freedesktop.org/

libxt-1.2.1-r0 installed size:
372 KiB

libxt-1.2.1-r0 license:
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
musl-1.2.2-r3 description:
the musl c library (libc) implementation

musl-1.2.2-r3 webpage:
https://musl.libc.org/

musl-1.2.2-r3 installed size:
608 KiB

musl-1.2.2-r3 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.2.2-r3 description:
the musl c library (libc) implementation

musl-utils-1.2.2-r3 webpage:
https://musl.libc.org/

musl-utils-1.2.2-r3 installed size:
144 KiB

musl-utils-1.2.2-r3 license:
MIT BSD GPL2+

```

### `apk` package: `ncurses-libs`

```console
ncurses-libs-6.2_p20210612-r0 description:
Ncurses libraries

ncurses-libs-6.2_p20210612-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-libs-6.2_p20210612-r0 installed size:
500 KiB

ncurses-libs-6.2_p20210612-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.2_p20210612-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.2_p20210612-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-base-6.2_p20210612-r0 installed size:
216 KiB

ncurses-terminfo-base-6.2_p20210612-r0 license:
MIT

```

### `apk` package: `nghttp2-libs`

```console
nghttp2-libs-1.43.0-r0 description:
Experimental HTTP/2 client, server and proxy (libraries)

nghttp2-libs-1.43.0-r0 webpage:
https://nghttp2.org

nghttp2-libs-1.43.0-r0 installed size:
168 KiB

nghttp2-libs-1.43.0-r0 license:
MIT

```

### `apk` package: `oniguruma`

```console
oniguruma-6.9.7.1-r0 description:
a regular expressions library

oniguruma-6.9.7.1-r0 webpage:
https://github.com/kkos/oniguruma

oniguruma-6.9.7.1-r0 installed size:
560 KiB

oniguruma-6.9.7.1-r0 license:
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
scanelf-1.3.2-r0 description:
Scan ELF binaries for stuff

scanelf-1.3.2-r0 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.3.2-r0 installed size:
92 KiB

scanelf-1.3.2-r0 license:
GPL-2.0-only

```

### `apk` package: `sqlite-libs`

```console
sqlite-libs-3.35.5-r0 description:
Sqlite3 library

sqlite-libs-3.35.5-r0 webpage:
https://www.sqlite.org/

sqlite-libs-3.35.5-r0 installed size:
964 KiB

sqlite-libs-3.35.5-r0 license:
Public-Domain

```

### `apk` package: `ssl_client`

```console
ssl_client-1.33.1-r2 description:
EXternal ssl_client for busybox wget

ssl_client-1.33.1-r2 webpage:
https://busybox.net/

ssl_client-1.33.1-r2 installed size:
28 KiB

ssl_client-1.33.1-r2 license:
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

### `apk` package: `tzdata`

```console
tzdata-2021a-r0 description:
Timezone data

tzdata-2021a-r0 webpage:
https://www.iana.org/time-zones

tzdata-2021a-r0 installed size:
3436 KiB

tzdata-2021a-r0 license:
Public-Domain

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
