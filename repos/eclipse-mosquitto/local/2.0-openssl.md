# `eclipse-mosquitto:2.0.18-openssl`

## Docker Metadata

- Image ID: `sha256:f0d4d2aca50d4de5a7c4cfac4d4874f867ada0ad7b2c70c0c01357df272fd991`
- Created: `2023-10-21T00:15:37.356119146Z`
- Virtual Size: ~ 9.51 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/docker-entrypoint.sh"]`
- Command: `["/usr/sbin/mosquitto","-c","/mosquitto/config/mosquitto.conf"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `VERSION=2.0.18`
  - `DOWNLOAD_SHA256=d665fe7d0032881b1371a47f34169ee4edab67903b2cd2b4c083822823f4448a`
  - `GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7`
  - `LWS_VERSION=4.2.1`
  - `LWS_SHA256=842da21f73ccba2be59e680de10a8cce7928313048750eb6ad73b6fa50763c51`
- Labels:
  - `description=Eclipse Mosquitto MQTT Broker`
  - `maintainer=Roger Light <roger@atchoo.org>`

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

### `apk` package: `cjson`

```console
cjson-1.7.15-r4 description:
Lighweight JSON parser in C

cjson-1.7.15-r4 webpage:
https://github.com/DaveGamble/cJSON

cjson-1.7.15-r4 installed size:
44 KiB

cjson-1.7.15-r4 license:
MIT

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
libcrypto3-3.1.3-r0 description:
Crypto library from openssl

libcrypto3-3.1.3-r0 webpage:
https://www.openssl.org/

libcrypto3-3.1.3-r0 installed size:
4468 KiB

libcrypto3-3.1.3-r0 license:
Apache-2.0

```

### `apk` package: `libssl3`

```console
libssl3-3.1.3-r0 description:
SSL shared libraries

libssl3-3.1.3-r0 webpage:
https://www.openssl.org/

libssl3-3.1.3-r0 installed size:
552 KiB

libssl3-3.1.3-r0 license:
Apache-2.0

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
