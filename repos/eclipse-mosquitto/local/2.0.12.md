# `eclipse-mosquitto:2.0.12`

## Docker Metadata

- Image ID: `sha256:a45972533f35be06249f61a9f698f3a490b1436172dbf938ab0ec0034a67f8b7`
- Created: `2021-09-02T17:24:00.831621833Z`
- Virtual Size: ~ 11.81 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/docker-entrypoint.sh"]`
- Command: `["/usr/sbin/mosquitto","-c","/mosquitto/config/mosquitto.conf"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `VERSION=2.0.12`
  - `DOWNLOAD_SHA256=31cf0065cb431d6f4e57a5f4d56663e839c9d177362eff89582d7cfde191c933`
  - `GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7`
  - `LWS_VERSION=4.2.1`
  - `LWS_SHA256=842da21f73ccba2be59e680de10a8cce7928313048750eb6ad73b6fa50763c51`
- Labels:
  - `description=Eclipse Mosquitto MQTT Broker`
  - `maintainer=Roger Light <roger@atchoo.org>`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.2.0-r16 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.2.0-r16 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.2.0-r16 installed size:
404 KiB

alpine-baselayout-3.2.0-r16 license:
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
apk-tools-2.12.7-r0 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.12.7-r0 webpage:
https://gitlab.alpinelinux.org/alpine/apk-tools

apk-tools-2.12.7-r0 installed size:
304 KiB

apk-tools-2.12.7-r0 license:
GPL-2.0-only

```

### `apk` package: `busybox`

```console
busybox-1.33.1-r3 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.33.1-r3 webpage:
https://busybox.net/

busybox-1.33.1-r3 installed size:
928 KiB

busybox-1.33.1-r3 license:
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

### `apk` package: `cjson`

```console
cjson-1.7.14-r1 description:
Lighweight JSON parser in C

cjson-1.7.14-r1 webpage:
https://github.com/DaveGamble/cJSON

cjson-1.7.14-r1 installed size:
44 KiB

cjson-1.7.14-r1 license:
MIT

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
libcrypto1.1-1.1.1l-r0 description:
Crypto library from openssl

libcrypto1.1-1.1.1l-r0 webpage:
https://www.openssl.org/

libcrypto1.1-1.1.1l-r0 installed size:
2704 KiB

libcrypto1.1-1.1.1l-r0 license:
OpenSSL

```

### `apk` package: `libressl`

```console
libressl-3.3.3-r0 description:
Version of the TLS/crypto stack forked from OpenSSL

libressl-3.3.3-r0 webpage:
https://www.libressl.org/

libressl-3.3.3-r0 installed size:
552 KiB

libressl-3.3.3-r0 license:
custom

```

### `apk` package: `libressl3.3-libcrypto`

```console
libressl3.3-libcrypto-3.3.3-r0 description:
libressl libcrypto library

libressl3.3-libcrypto-3.3.3-r0 webpage:
https://www.libressl.org/

libressl3.3-libcrypto-3.3.3-r0 installed size:
1844 KiB

libressl3.3-libcrypto-3.3.3-r0 license:
custom

```

### `apk` package: `libressl3.3-libssl`

```console
libressl3.3-libssl-3.3.3-r0 description:
libressl libssl library

libressl3.3-libssl-3.3.3-r0 webpage:
https://www.libressl.org/

libressl3.3-libssl-3.3.3-r0 installed size:
364 KiB

libressl3.3-libssl-3.3.3-r0 license:
custom

```

### `apk` package: `libressl3.3-libtls`

```console
libressl3.3-libtls-3.3.3-r0 description:
libressl libtls library

libressl3.3-libtls-3.3.3-r0 webpage:
https://www.libressl.org/

libressl3.3-libtls-3.3.3-r0 installed size:
1872 KiB

libressl3.3-libtls-3.3.3-r0 license:
custom

```

### `apk` package: `libretls`

```console
libretls-3.3.3p1-r2 description:
port of libtls from libressl to openssl

libretls-3.3.3p1-r2 webpage:
https://git.causal.agency/libretls/

libretls-3.3.3p1-r2 installed size:
84 KiB

libretls-3.3.3p1-r2 license:
ISC AND (BSD-3-Clause OR MIT)

```

### `apk` package: `libssl1.1`

```console
libssl1.1-1.1.1l-r0 description:
SSL shared libraries

libssl1.1-1.1.1l-r0 webpage:
https://www.openssl.org/

libssl1.1-1.1.1l-r0 installed size:
528 KiB

libssl1.1-1.1.1l-r0 license:
OpenSSL

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

### `apk` package: `ssl_client`

```console
ssl_client-1.33.1-r3 description:
EXternal ssl_client for busybox wget

ssl_client-1.33.1-r3 webpage:
https://busybox.net/

ssl_client-1.33.1-r3 installed size:
28 KiB

ssl_client-1.33.1-r3 license:
GPL-2.0-only

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
