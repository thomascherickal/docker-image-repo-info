# `friendica:2023.09-dev-fpm-alpine`

## Docker Metadata

- Image ID: `sha256:79b851b3acf98d419375b1e2200e040d96f1578ebb4a27b042200380ff292203`
- Created: `2023-12-16T08:38:44.546452055Z`
- Virtual Size: ~ 129.24 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/entrypoint-dev.sh"]`
- Command: `["php-fpm"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c`
  - `PHP_INI_DIR=/usr/local/etc/php`
  - `PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64`
  - `PHP_LDFLAGS=-Wl,-O1 -pie`
  - `GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD`
  - `PHP_VERSION=8.1.26`
  - `PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz`
  - `PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc`
  - `PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f`
  - `GOSU_VERSION=1.14`
  - `PHP_MEMORY_LIMIT=512M`
  - `PHP_UPLOAD_LIMIT=512M`
  - `FRIENDICA_SYSLOG_FLAGS=39`
  - `FRIENDICA_VERSION=2023.09-dev`
  - `FRIENDICA_ADDONS=2023.09-dev`

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

### `apk` package: `gdbm`

```console
gdbm-1.23-r1 description:
GNU dbm is a set of database routines that use extensible hashing

gdbm-1.23-r1 webpage:
https://www.gnu.org/software/gdbm/

gdbm-1.23-r1 installed size:
84 KiB

gdbm-1.23-r1 license:
GPL-3.0-or-later

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

### `apk` package: `gnupg`

```console
gnupg-2.4.3-r1 description:
GNU Privacy Guard 2 - meta package for full GnuPG suite

gnupg-2.4.3-r1 webpage:
https://www.gnupg.org/

gnupg-2.4.3-r1 installed size:
4096 B

gnupg-2.4.3-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gnupg-dirmngr`

```console
gnupg-dirmngr-2.4.3-r1 description:
GNU Privacy Guard 2 - network certificate management service

gnupg-dirmngr-2.4.3-r1 webpage:
https://www.gnupg.org/

gnupg-dirmngr-2.4.3-r1 installed size:
656 KiB

gnupg-dirmngr-2.4.3-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gnupg-gpgconf`

```console
gnupg-gpgconf-2.4.3-r1 description:
GNU Privacy Guard 2 - core configuration utilities

gnupg-gpgconf-2.4.3-r1 webpage:
https://www.gnupg.org/

gnupg-gpgconf-2.4.3-r1 installed size:
248 KiB

gnupg-gpgconf-2.4.3-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gnupg-keyboxd`

```console
gnupg-keyboxd-2.4.3-r1 description:
GNU Privacy Guard 2 - keyboxd manager

gnupg-keyboxd-2.4.3-r1 webpage:
https://www.gnupg.org/

gnupg-keyboxd-2.4.3-r1 installed size:
232 KiB

gnupg-keyboxd-2.4.3-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gnupg-utils`

```console
gnupg-utils-2.4.3-r1 description:
GNU Privacy Guard 2 - utility programs

gnupg-utils-2.4.3-r1 webpage:
https://www.gnupg.org/

gnupg-utils-2.4.3-r1 installed size:
752 KiB

gnupg-utils-2.4.3-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gnupg-wks-client`

```console
gnupg-wks-client-2.4.3-r1 description:
GNU Privacy Guard 2 - Web Key Service client

gnupg-wks-client-2.4.3-r1 webpage:
https://www.gnupg.org/

gnupg-wks-client-2.4.3-r1 installed size:
184 KiB

gnupg-wks-client-2.4.3-r1 license:
GPL-3.0-or-later

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

### `apk` package: `gpg`

```console
gpg-2.4.3-r1 description:
GNU Privacy Guard 2 - public key operations only

gpg-2.4.3-r1 webpage:
https://www.gnupg.org/

gpg-2.4.3-r1 installed size:
932 KiB

gpg-2.4.3-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gpg-agent`

```console
gpg-agent-2.4.3-r1 description:
GNU Privacy Guard 2 - cryptographic agent

gpg-agent-2.4.3-r1 webpage:
https://www.gnupg.org/

gpg-agent-2.4.3-r1 installed size:
660 KiB

gpg-agent-2.4.3-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gpg-wks-server`

```console
gpg-wks-server-2.4.3-r1 description:
GNU Privacy Guard 2 - Web Key Service server

gpg-wks-server-2.4.3-r1 webpage:
https://www.gnupg.org/

gpg-wks-server-2.4.3-r1 installed size:
164 KiB

gpg-wks-server-2.4.3-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gpgsm`

```console
gpgsm-2.4.3-r1 description:
GNU Privacy Guard 2 - S/MIME version

gpgsm-2.4.3-r1 webpage:
https://www.gnupg.org/

gpgsm-2.4.3-r1 installed size:
484 KiB

gpgsm-2.4.3-r1 license:
GPL-3.0-or-later

```

### `apk` package: `gpgv`

```console
gpgv-2.4.3-r1 description:
GNU Privacy Guard 2 - signature verification only

gpgv-2.4.3-r1 webpage:
https://www.gnupg.org/

gpgv-2.4.3-r1 installed size:
436 KiB

gpgv-2.4.3-r1 license:
GPL-3.0-or-later

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

### `apk` package: `keyutils-libs`

```console
keyutils-libs-1.6.3-r3 description:
Key utilities library

keyutils-libs-1.6.3-r3 webpage:
https://people.redhat.com/~dhowells/keyutils/

keyutils-libs-1.6.3-r3 installed size:
32 KiB

keyutils-libs-1.6.3-r3 license:
GPL-2.0-or-later AND LGPL-2.0-or-later

```

### `apk` package: `krb5-conf`

```console
krb5-conf-1.0-r2 description:
Shared krb5.conf for both MIT krb5 and heimdal

krb5-conf-1.0-r2 webpage:
https://web.mit.edu/kerberos/www/

krb5-conf-1.0-r2 installed size:
12 KiB

krb5-conf-1.0-r2 license:
MIT

```

### `apk` package: `krb5-libs`

```console
krb5-libs-1.21.2-r0 description:
The shared libraries used by Kerberos 5

krb5-libs-1.21.2-r0 webpage:
https://web.mit.edu/kerberos/www/

krb5-libs-1.21.2-r0 installed size:
1824 KiB

krb5-libs-1.21.2-r0 license:
MIT

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

### `apk` package: `libassuan`

```console
libassuan-2.5.6-r1 description:
IPC library used by some GnuPG related software

libassuan-2.5.6-r1 webpage:
https://www.gnupg.org/software/libassuan/index.html

libassuan-2.5.6-r1 installed size:
84 KiB

libassuan-2.5.6-r1 license:
LGPL-2.1-or-later

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

### `apk` package: `libcom_err`

```console
libcom_err-1.47.0-r5 description:
Common error description library

libcom_err-1.47.0-r5 webpage:
https://e2fsprogs.sourceforge.net/

libcom_err-1.47.0-r5 installed size:
28 KiB

libcom_err-1.47.0-r5 license:
GPL-2.0-or-later AND LGPL-2.0-or-later AND BSD-3-Clause AND MIT

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

### `apk` package: `libgcrypt`

```console
libgcrypt-1.10.3-r0 description:
General purpose crypto library based on the code used in GnuPG

libgcrypt-1.10.3-r0 webpage:
https://www.gnupg.org/

libgcrypt-1.10.3-r0 installed size:
1172 KiB

libgcrypt-1.10.3-r0 license:
LGPL-2.1-or-later AND GPL-2.0-or-later

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

### `apk` package: `libgpg-error`

```console
libgpg-error-1.47-r2 description:
Support library for libgcrypt

libgpg-error-1.47-r2 webpage:
https://www.gnupg.org/

libgpg-error-1.47-r2 installed size:
176 KiB

libgpg-error-1.47-r2 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `libgsasl`

```console
libgsasl-2.2.0-r1 description:
An implementation of the Simple Authentication and Security Layer framework

libgsasl-2.2.0-r1 webpage:
https://josefsson.org/gsasl/

libgsasl-2.2.0-r1 installed size:
132 KiB

libgsasl-2.2.0-r1 license:
LGPL-2.0-or-later

```

### `apk` package: `libidn`

```console
libidn-1.41-r3 description:
Encode/Decode library for internationalized domain names

libidn-1.41-r3 webpage:
https://www.gnu.org/software/libidn

libidn-1.41-r3 installed size:
288 KiB

libidn-1.41-r3 license:
LGPL-2.1-or-later

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

### `apk` package: `libksba`

```console
libksba-1.6.5-r0 description:
Libksba is a CMS and X.509 access library

libksba-1.6.5-r0 webpage:
https://www.gnupg.org/software/libksba/index.html

libksba-1.6.5-r0 installed size:
216 KiB

libksba-1.6.5-r0 license:
LGPL-3.0-only AND GPL-2.0-only AND GPL-3.0-only

```

### `apk` package: `libldap`

```console
libldap-2.6.6-r1 description:
OpenLDAP libraries

libldap-2.6.6-r1 webpage:
https://www.openldap.org/

libldap-2.6.6-r1 installed size:
392 KiB

libldap-2.6.6-r1 license:
OLDAP-2.8

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

### `apk` package: `libmemcached-libs`

```console
libmemcached-libs-1.1.4-r1 description:
Client library and command line tools for memcached server (resurrected) (libraries)

libmemcached-libs-1.1.4-r1 webpage:
https://github.com/awesomized/libmemcached

libmemcached-libs-1.1.4-r1 installed size:
260 KiB

libmemcached-libs-1.1.4-r1 license:
BSD-3-Clause

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

### `apk` package: `libsasl`

```console
libsasl-2.1.28-r5 description:
Cyrus Simple Authentication and Security Layer (SASL) library

libsasl-2.1.28-r5 webpage:
https://www.cyrusimap.org/sasl/

libsasl-2.1.28-r5 installed size:
192 KiB

libsasl-2.1.28-r5 license:
custom

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

### `apk` package: `libverto`

```console
libverto-0.3.2-r2 description:
Main loop abstraction library

libverto-0.3.2-r2 webpage:
https://github.com/latchset/libverto

libverto-0.3.2-r2 installed size:
36 KiB

libverto-0.3.2-r2 license:
MIT

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

### `apk` package: `libxxhash`

```console
libxxhash-0.8.2-r2 description:
Extremely fast non-cryptographic hash algorithm (libraries)

libxxhash-0.8.2-r2 webpage:
https://cyan4973.github.io/xxHash/

libxxhash-0.8.2-r2 installed size:
80 KiB

libxxhash-0.8.2-r2 license:
BSD-2-Clause

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

### `apk` package: `linux-pam`

```console
linux-pam-1.5.3-r7 description:
Linux PAM (Pluggable Authentication Modules for Linux)

linux-pam-1.5.3-r7 webpage:
https://www.kernel.org/pub/linux/libs/pam

linux-pam-1.5.3-r7 installed size:
1036 KiB

linux-pam-1.5.3-r7 license:
BSD-3-Clause

```

### `apk` package: `lz4-libs`

```console
lz4-libs-1.9.4-r5 description:
LZ4 is lossless compression algorithm with fast decoder @ multiple GB/s per core. (libraries)

lz4-libs-1.9.4-r5 webpage:
https://github.com/lz4/lz4

lz4-libs-1.9.4-r5 installed size:
144 KiB

lz4-libs-1.9.4-r5 license:
BSD-2-Clause AND GPL-2.0-only

```

### `apk` package: `msmtp`

```console
msmtp-1.8.25-r0 description:
SMTP client with a sendmail compatible interface

msmtp-1.8.25-r0 webpage:
https://marlam.de/msmtp/

msmtp-1.8.25-r0 installed size:
156 KiB

msmtp-1.8.25-r0 license:
GPL-3.0-or-later

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

### `apk` package: `npth`

```console
npth-1.6-r4 description:
The New GNU Portable Threads library

npth-1.6-r4 webpage:
https://gnupg.org/related_software/npth/

npth-1.6-r4 installed size:
32 KiB

npth-1.6-r4 license:
LGPL-2.0-or-later

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

### `apk` package: `pinentry`

```console
pinentry-1.2.1-r1 description:
Collection of simple PIN or passphrase entry dialogs which utilize the Assuan protocol

pinentry-1.2.1-r1 webpage:
https://www.gnupg.org/aegypten2/

pinentry-1.2.1-r1 installed size:
72 KiB

pinentry-1.2.1-r1 license:
GPL-2.0-or-later

```

### `apk` package: `popt`

```console
popt-1.19-r3 description:
commandline option parser

popt-1.19-r3 webpage:
https://github.com/rpm-software-management/popt

popt-1.19-r3 installed size:
56 KiB

popt-1.19-r3 license:
MIT

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

### `apk` package: `rsync`

```console
rsync-3.2.7-r4 description:
A file transfer program to keep remote files in sync

rsync-3.2.7-r4 webpage:
https://rsync.samba.org/

rsync-3.2.7-r4 installed size:
408 KiB

rsync-3.2.7-r4 license:
GPL-3.0-or-later

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

### `apk` package: `shadow`

```console
shadow-4.14.2-r0 description:
PAM-using login and passwd utilities (usermod, useradd, ...)

shadow-4.14.2-r0 webpage:
https://github.com/shadow-maint/shadow

shadow-4.14.2-r0 installed size:
1356 KiB

shadow-4.14.2-r0 license:
BSD-3-Clause

```

### `apk` package: `skalibs`

```console
skalibs-2.14.0.1-r0 description:
Set of general-purpose C programming libraries for skarnet.org software.

skalibs-2.14.0.1-r0 webpage:
https://skarnet.org/software/skalibs/

skalibs-2.14.0.1-r0 installed size:
192 KiB

skalibs-2.14.0.1-r0 license:
ISC

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

### `apk` package: `tini`

```console
tini-0.19.0-r2 description:
A tiny but valid init for containers

tini-0.19.0-r2 webpage:
https://github.com/krallin/tini

tini-0.19.0-r2 installed size:
36 KiB

tini-0.19.0-r2 license:
MIT

```

### `apk` package: `utmps-libs`

```console
utmps-libs-0.1.2.2-r0 description:
A secure utmp/wtmp implementation (libraries)

utmps-libs-0.1.2.2-r0 webpage:
https://skarnet.org/software/utmps/

utmps-libs-0.1.2.2-r0 installed size:
24 KiB

utmps-libs-0.1.2.2-r0 license:
ISC

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
