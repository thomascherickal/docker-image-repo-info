# `fluentd:v1.16.0-1.0`

## Docker Metadata

- Image ID: `sha256:d619c23c9ae269bd4d905563b3b29e8cf52f3b43a98e608ae7f3bc9f3813a07d`
- Created: `2023-06-14T22:34:24.376942755Z`
- Virtual Size: ~ 58.91 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["tini","--","/bin/entrypoint.sh"]`
- Command: `["fluentd"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `FLUENTD_CONF=fluent.conf`
  - `LD_PRELOAD=`
- Labels:
  - `Description=Fluentd docker image`
  - `Vendor=Fluent Organization`
  - `Version=1.16.0`
  - `maintainer=Fluentd developers <fluentd@googlegroups.com>`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.4.0-r0 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.4.0-r0 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.4.0-r0 installed size:
324 KiB

alpine-baselayout-3.4.0-r0 license:
GPL-2.0-only

```

### `apk` package: `alpine-baselayout-data`

```console
alpine-baselayout-data-3.4.0-r0 description:
Alpine base dir structure and init scripts

alpine-baselayout-data-3.4.0-r0 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-data-3.4.0-r0 installed size:
76 KiB

alpine-baselayout-data-3.4.0-r0 license:
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
apk-tools-2.12.10-r1 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.12.10-r1 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.12.10-r1 installed size:
300 KiB

apk-tools-2.12.10-r1 license:
GPL-2.0-only

```

### `apk` package: `busybox`

```console
busybox-1.35.0-r29 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.35.0-r29 webpage:
https://busybox.net/

busybox-1.35.0-r29 installed size:
940 KiB

busybox-1.35.0-r29 license:
GPL-2.0-only

```

### `apk` package: `busybox-binsh`

```console
busybox-binsh-1.35.0-r29 description:
busybox ash /bin/sh

busybox-binsh-1.35.0-r29 webpage:
https://busybox.net/

busybox-binsh-1.35.0-r29 installed size:
8192 B

busybox-binsh-1.35.0-r29 license:
GPL-2.0-only

```

### `apk` package: `ca-certificates`

```console
ca-certificates-20230506-r0 description:
Common CA certificates PEM files from Mozilla

ca-certificates-20230506-r0 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-20230506-r0 installed size:
692 KiB

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

### `apk` package: `gmp`

```console
gmp-6.2.1-r2 description:
free library for arbitrary precision arithmetic

gmp-6.2.1-r2 webpage:
https://gmplib.org/

gmp-6.2.1-r2 installed size:
420 KiB

gmp-6.2.1-r2 license:
LGPL-3.0-or-later OR GPL-2.0-or-later

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

### `apk` package: `libcrypto3`

```console
libcrypto3-3.0.9-r1 description:
Crypto library from openssl

libcrypto3-3.0.9-r1 webpage:
https://www.openssl.org/

libcrypto3-3.0.9-r1 installed size:
4108 KiB

libcrypto3-3.0.9-r1 license:
Apache-2.0

```

### `apk` package: `libffi`

```console
libffi-3.4.4-r0 description:
portable, high level programming interface to various calling conventions.

libffi-3.4.4-r0 webpage:
https://sourceware.org/libffi/

libffi-3.4.4-r0 installed size:
52 KiB

libffi-3.4.4-r0 license:
MIT

```

### `apk` package: `libssl3`

```console
libssl3-3.0.9-r1 description:
SSL shared libraries

libssl3-3.0.9-r1 webpage:
https://www.openssl.org/

libssl3-3.0.9-r1 installed size:
608 KiB

libssl3-3.0.9-r1 license:
Apache-2.0

```

### `apk` package: `libucontext`

```console
libucontext-1.2-r0 description:
ucontext function implementations

libucontext-1.2-r0 webpage:
https://github.com/kaniini/libucontext

libucontext-1.2-r0 installed size:
40 KiB

libucontext-1.2-r0 license:
ISC

```

### `apk` package: `musl`

```console
musl-1.2.3-r5 description:
the musl c library (libc) implementation

musl-1.2.3-r5 webpage:
https://musl.libc.org/

musl-1.2.3-r5 installed size:
620 KiB

musl-1.2.3-r5 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.2.3-r5 description:
the musl c library (libc) implementation

musl-utils-1.2.3-r5 webpage:
https://musl.libc.org/

musl-utils-1.2.3-r5 installed size:
132 KiB

musl-utils-1.2.3-r5 license:
MIT AND BSD-2-Clause AND GPL-2.0-or-later

```

### `apk` package: `ncurses-libs`

```console
ncurses-libs-6.3_p20221119-r1 description:
Ncurses libraries

ncurses-libs-6.3_p20221119-r1 webpage:
https://invisible-island.net/ncurses/

ncurses-libs-6.3_p20221119-r1 installed size:
500 KiB

ncurses-libs-6.3_p20221119-r1 license:
MIT

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.3_p20221119-r1 description:
Descriptions of common terminals

ncurses-terminfo-base-6.3_p20221119-r1 webpage:
https://invisible-island.net/ncurses/

ncurses-terminfo-base-6.3_p20221119-r1 installed size:
216 KiB

ncurses-terminfo-base-6.3_p20221119-r1 license:
MIT

```

### `apk` package: `readline`

```console
readline-8.2.0-r0 description:
GNU readline library

readline-8.2.0-r0 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-8.2.0-r0 installed size:
308 KiB

readline-8.2.0-r0 license:
GPL-2.0-or-later

```

### `apk` package: `ruby`

```console
ruby-3.1.4-r0 description:
An object-oriented language for quick and easy programming

ruby-3.1.4-r0 webpage:
https://www.ruby-lang.org/

ruby-3.1.4-r0 installed size:
44 KiB

ruby-3.1.4-r0 license:
Ruby AND BSD-2-Clause AND MIT

```

### `apk` package: `ruby-libs`

```console
ruby-libs-3.1.4-r0 description:
Libraries necessary to run Ruby

ruby-libs-3.1.4-r0 webpage:
https://www.ruby-lang.org/

ruby-libs-3.1.4-r0 installed size:
15 MiB

ruby-libs-3.1.4-r0 license:
Ruby AND BSD-2-Clause AND MIT

```

### `apk` package: `ruby-webrick`

```console
ruby-webrick-1.7.0-r1 description:
HTTP server toolkit for Ruby

ruby-webrick-1.7.0-r1 webpage:
https://github.com/ruby/webrick

ruby-webrick-1.7.0-r1 installed size:
328 KiB

ruby-webrick-1.7.0-r1 license:
BSD-2-Clause

```

### `apk` package: `scanelf`

```console
scanelf-1.3.5-r1 description:
Scan ELF binaries for stuff

scanelf-1.3.5-r1 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.3.5-r1 installed size:
96 KiB

scanelf-1.3.5-r1 license:
GPL-2.0-only

```

### `apk` package: `ssl_client`

```console
ssl_client-1.35.0-r29 description:
EXternal ssl_client for busybox wget

ssl_client-1.35.0-r29 webpage:
https://busybox.net/

ssl_client-1.35.0-r29 installed size:
28 KiB

ssl_client-1.35.0-r29 license:
GPL-2.0-only

```

### `apk` package: `tini`

```console
tini-0.19.0-r1 description:
A tiny but valid init for containers

tini-0.19.0-r1 webpage:
https://github.com/krallin/tini

tini-0.19.0-r1 installed size:
36 KiB

tini-0.19.0-r1 license:
MIT

```

### `apk` package: `yaml`

```console
yaml-0.2.5-r0 description:
YAML 1.1 parser and emitter written in C

yaml-0.2.5-r0 webpage:
https://pyyaml.org/wiki/LibYAML

yaml-0.2.5-r0 installed size:
120 KiB

yaml-0.2.5-r0 license:
MIT

```

### `apk` package: `zlib`

```console
zlib-1.2.13-r0 description:
A compression/decompression Library

zlib-1.2.13-r0 webpage:
https://zlib.net/

zlib-1.2.13-r0 installed size:
108 KiB

zlib-1.2.13-r0 license:
Zlib

```
