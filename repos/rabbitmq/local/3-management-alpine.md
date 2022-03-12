# `rabbitmq:3.9.13-management-alpine`

## Docker Metadata

- Image ID: `sha256:07f08189cfa8060367b3a5c17ac112255483afe7d32d742ff522714e7b838504`
- Created: `2022-03-11T00:41:09.521989864Z`
- Virtual Size: ~ 180.35 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-entrypoint.sh"]`
- Command: `["rabbitmq-server"]`
- Environment:
  - `PATH=/opt/rabbitmq/sbin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `OPENSSL_VERSION=1.1.1m`
  - `OPENSSL_SOURCE_SHA256=f89199be8b23ca45fc7cb9f1d8d3ee67312318286ad030f5316aca6462db6c96`
  - `OPENSSL_PGP_KEY_IDS=0x8657ABB260F056B1E5190839D9C4D26D0E604491 0x5B2545DAB21995F4088CEFAA36CEE4DEB00CFE33 0xED230BEC4D4F2518B9D7DF41F0DB4D21C1D35231 0xC1F33DD8CE1D4CC613AF14DA9195C48241FBF7DD 0x7953AC1FBC3DC8B3B292393ED5E9E43F7DF9EE8C 0xE5E52560DD91C556DDBDA5D02064C53641C25E5D`
  - `OTP_VERSION=24.3`
  - `OTP_SOURCE_SHA256=ee8dd101af68ba175deec1844059ed287a22f7f46e72915631c965cc8be331f9`
  - `RABBITMQ_DATA_DIR=/var/lib/rabbitmq`
  - `RABBITMQ_VERSION=3.9.13`
  - `RABBITMQ_PGP_KEY_ID=0x0A9AF2115F4687BD29803A206B73A36E6026DFCA`
  - `RABBITMQ_HOME=/opt/rabbitmq`
  - `RABBITMQ_LOGS=-`
  - `HOME=/var/lib/rabbitmq`
  - `LANG=C.UTF-8`
  - `LANGUAGE=C.UTF-8`
  - `LC_ALL=C.UTF-8`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.2.0-r18 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.2.0-r18 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.2.0-r18 installed size:
404 KiB

alpine-baselayout-3.2.0-r18 license:
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
apk-tools-2.12.7-r3 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.12.7-r3 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.12.7-r3 installed size:
304 KiB

apk-tools-2.12.7-r3 license:
GPL-2.0-only

```

### `apk` package: `bash`

```console
bash-5.1.8-r0 description:
The GNU Bourne Again shell

bash-5.1.8-r0 webpage:
https://www.gnu.org/software/bash/bash.html

bash-5.1.8-r0 installed size:
1296 KiB

bash-5.1.8-r0 license:
GPL-3.0-or-later

```

### `apk` package: `busybox`

```console
busybox-1.34.1-r3 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.34.1-r3 webpage:
https://busybox.net/

busybox-1.34.1-r3 installed size:
924 KiB

busybox-1.34.1-r3 license:
GPL-2.0-only

```

### `apk` package: `ca-certificates-bundle`

```console
ca-certificates-bundle-20191127-r7 description:
Pre generated bundle of Mozilla certificates

ca-certificates-bundle-20191127-r7 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-bundle-20191127-r7 installed size:
228 KiB

ca-certificates-bundle-20191127-r7 license:
MPL-2.0 AND MIT

```

### `apk` package: `expat`

```console
expat-2.4.7-r0 description:
XML Parser library written in C

expat-2.4.7-r0 webpage:
http://www.libexpat.org/

expat-2.4.7-r0 installed size:
192 KiB

expat-2.4.7-r0 license:
MIT

```

### `apk` package: `gdbm`

```console
gdbm-1.22-r0 description:
GNU dbm is a set of database routines that use extensible hashing

gdbm-1.22-r0 webpage:
https://www.gnu.org/software/gdbm/

gdbm-1.22-r0 installed size:
88 KiB

gdbm-1.22-r0 license:
GPL-3.0-or-later

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
libcrypto1.1-1.1.1l-r7 description:
Crypto library from openssl

libcrypto1.1-1.1.1l-r7 webpage:
https://www.openssl.org/

libcrypto1.1-1.1.1l-r7 installed size:
2676 KiB

libcrypto1.1-1.1.1l-r7 license:
OpenSSL

```

### `apk` package: `libffi`

```console
libffi-3.4.2-r1 description:
portable, high level programming interface to various calling conventions.

libffi-3.4.2-r1 webpage:
https://sourceware.org/libffi/

libffi-3.4.2-r1 installed size:
60 KiB

libffi-3.4.2-r1 license:
MIT

```

### `apk` package: `libgcc`

```console
libgcc-10.3.1_git20211027-r0 description:
GNU C compiler runtime libraries

libgcc-10.3.1_git20211027-r0 webpage:
https://gcc.gnu.org

libgcc-10.3.1_git20211027-r0 installed size:
112 KiB

libgcc-10.3.1_git20211027-r0 license:
GPL-2.0-or-later LGPL-2.1-or-later

```

### `apk` package: `libintl`

```console
libintl-0.21-r0 description:
GNU gettext runtime library

libintl-0.21-r0 webpage:
https://www.gnu.org/software/gettext/gettext.html

libintl-0.21-r0 installed size:
56 KiB

libintl-0.21-r0 license:
LGPL-2.1-or-later

```

### `apk` package: `libproc`

```console
libproc-3.3.17-r0 description:
Library for monitoring system and processes

libproc-3.3.17-r0 webpage:
https://gitlab.com/procps-ng/procps

libproc-3.3.17-r0 installed size:
84 KiB

libproc-3.3.17-r0 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `libretls`

```console
libretls-3.3.4-r2 description:
port of libtls from libressl to openssl

libretls-3.3.4-r2 webpage:
https://git.causal.agency/libretls/

libretls-3.3.4-r2 installed size:
84 KiB

libretls-3.3.4-r2 license:
ISC AND (BSD-3-Clause OR MIT)

```

### `apk` package: `libssl1.1`

```console
libssl1.1-1.1.1l-r7 description:
SSL shared libraries

libssl1.1-1.1.1l-r7 webpage:
https://www.openssl.org/

libssl1.1-1.1.1l-r7 installed size:
528 KiB

libssl1.1-1.1.1l-r7 license:
OpenSSL

```

### `apk` package: `libstdc++`

```console
libstdc++-10.3.1_git20211027-r0 description:
GNU C++ standard runtime library

libstdc++-10.3.1_git20211027-r0 webpage:
https://gcc.gnu.org

libstdc++-10.3.1_git20211027-r0 installed size:
1664 KiB

libstdc++-10.3.1_git20211027-r0 license:
GPL-2.0-or-later LGPL-2.1-or-later

```

### `apk` package: `mpdecimal`

```console
mpdecimal-2.5.1-r1 description:
complete implementation of the General Decimal Arithmetic Specification

mpdecimal-2.5.1-r1 webpage:
https://www.bytereef.org/mpdecimal/index.html

mpdecimal-2.5.1-r1 installed size:
212 KiB

mpdecimal-2.5.1-r1 license:
BSD-2-Clause

```

### `apk` package: `musl`

```console
musl-1.2.2-r7 description:
the musl c library (libc) implementation

musl-1.2.2-r7 webpage:
https://musl.libc.org/

musl-1.2.2-r7 installed size:
608 KiB

musl-1.2.2-r7 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.2.2-r7 description:
the musl c library (libc) implementation

musl-utils-1.2.2-r7 webpage:
https://musl.libc.org/

musl-utils-1.2.2-r7 installed size:
140 KiB

musl-utils-1.2.2-r7 license:
MIT BSD GPL2+

```

### `apk` package: `ncurses-libs`

```console
ncurses-libs-6.3_p20211120-r0 description:
Ncurses libraries

ncurses-libs-6.3_p20211120-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-libs-6.3_p20211120-r0 installed size:
500 KiB

ncurses-libs-6.3_p20211120-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.3_p20211120-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.3_p20211120-r0 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-base-6.3_p20211120-r0 installed size:
216 KiB

ncurses-terminfo-base-6.3_p20211120-r0 license:
MIT

```

### `apk` package: `procps`

```console
procps-3.3.17-r0 description:
Utilities for monitoring your system and processes on your system

procps-3.3.17-r0 webpage:
https://gitlab.com/procps-ng/procps

procps-3.3.17-r0 installed size:
588 KiB

procps-3.3.17-r0 license:
GPL-2.0-or-later AND LGPL-2.1-or-later

```

### `apk` package: `python3`

```console
python3-3.9.7-r4 description:
A high-level scripting language

python3-3.9.7-r4 webpage:
https://www.python.org/

python3-3.9.7-r4 installed size:
45 MiB

python3-3.9.7-r4 license:
PSF-2.0

```

### `apk` package: `readline`

```console
readline-8.1.1-r0 description:
GNU readline library

readline-8.1.1-r0 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.1.1-r0 installed size:
308 KiB

readline-8.1.1-r0 license:
GPL-2.0-or-later

```

### `apk` package: `scanelf`

```console
scanelf-1.3.3-r0 description:
Scan ELF binaries for stuff

scanelf-1.3.3-r0 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.3.3-r0 installed size:
92 KiB

scanelf-1.3.3-r0 license:
GPL-2.0-only

```

### `apk` package: `sqlite-libs`

```console
sqlite-libs-3.36.0-r0 description:
Sqlite3 library

sqlite-libs-3.36.0-r0 webpage:
https://www.sqlite.org/

sqlite-libs-3.36.0-r0 installed size:
968 KiB

sqlite-libs-3.36.0-r0 license:
blessing

```

### `apk` package: `ssl_client`

```console
ssl_client-1.34.1-r3 description:
EXternal ssl_client for busybox wget

ssl_client-1.34.1-r3 webpage:
https://busybox.net/

ssl_client-1.34.1-r3 installed size:
28 KiB

ssl_client-1.34.1-r3 license:
GPL-2.0-only

```

### `apk` package: `su-exec`

```console
su-exec-0.2-r1 description:
switch user and group id, setgroups and exec

su-exec-0.2-r1 webpage:
https://github.com/ncopa/su-exec

su-exec-0.2-r1 installed size:
24 KiB

su-exec-0.2-r1 license:
MIT

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
