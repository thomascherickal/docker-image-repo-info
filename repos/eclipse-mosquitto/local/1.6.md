# `eclipse-mosquitto:1.6.9`

## Docker Metadata

- Image ID: `sha256:e2f58db07ce196428b91294a323d35c75dc477505296b9bc97093dd2ac36ebd9`
- Created: `2020-03-03T23:19:47.379119758Z`
- Virtual Size: ~ 5.60 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/docker-entrypoint.sh"]`
- Command: `["/usr/sbin/mosquitto","-c","/mosquitto/config/mosquitto.conf"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `VERSION=1.6.9`
  - `DOWNLOAD_SHA256=412979b2db0a0020bd02fa64f0a0de9e7000b84462586e32b67f29bb1f6c1685`
  - `GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7`
  - `LWS_VERSION=2.4.2`
- Labels:
  - `description=Eclipse Mosquitto MQTT Broker`
  - `maintainer=Roger Light <roger@atchoo.org>`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.1.0-r0 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.1.0-r0 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.1.0-r0 installed size:
397312

alpine-baselayout-3.1.0-r0 license:
GPL-2.0

```

### `apk` package: `alpine-keys`

```console
alpine-keys-2.1-r1 description:
Public keys for Alpine Linux packages

alpine-keys-2.1-r1 webpage:
http://alpinelinux.org

alpine-keys-2.1-r1 installed size:
98304

alpine-keys-2.1-r1 license:
MIT

```

### `apk` package: `apk-tools`

```console
apk-tools-2.10.1-r0 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.10.1-r0 webpage:
https://git.alpinelinux.org/cgit/apk-tools/

apk-tools-2.10.1-r0 installed size:
262144

apk-tools-2.10.1-r0 license:
GPL2

```

### `apk` package: `busybox`

```console
busybox-1.28.4-r3 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.28.4-r3 webpage:
http://busybox.net

busybox-1.28.4-r3 installed size:
905216

busybox-1.28.4-r3 license:
GPL-2.0

```

### `apk` package: `ca-certificates`

```console
ca-certificates-20190108-r0 description:
Common CA certificates PEM files

ca-certificates-20190108-r0 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-20190108-r0 installed size:
733184

ca-certificates-20190108-r0 license:
MPL-2.0 GPL-2.0-or-later

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

### `apk` package: `libressl2.7-libcrypto`

```console
libressl2.7-libcrypto-2.7.5-r0 description:
libressl libcrypto library

libressl2.7-libcrypto-2.7.5-r0 webpage:
https://www.libressl.org/

libressl2.7-libcrypto-2.7.5-r0 installed size:
2125824

libressl2.7-libcrypto-2.7.5-r0 license:
custom

```

### `apk` package: `libressl2.7-libssl`

```console
libressl2.7-libssl-2.7.5-r0 description:
libressl libssl library

libressl2.7-libssl-2.7.5-r0 webpage:
https://www.libressl.org/

libressl2.7-libssl-2.7.5-r0 installed size:
327680

libressl2.7-libssl-2.7.5-r0 license:
custom

```

### `apk` package: `libressl2.7-libtls`

```console
libressl2.7-libtls-2.7.5-r0 description:
libressl libtls library

libressl2.7-libtls-2.7.5-r0 webpage:
https://www.libressl.org/

libressl2.7-libtls-2.7.5-r0 installed size:
77824

libressl2.7-libtls-2.7.5-r0 license:
custom

```

### `apk` package: `musl`

```console
musl-1.1.19-r11 description:
the musl c library (libc) implementation

musl-1.1.19-r11 webpage:
http://www.musl-libc.org/

musl-1.1.19-r11 installed size:
602112

musl-1.1.19-r11 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.1.19-r11 description:
the musl c library (libc) implementation

musl-utils-1.1.19-r11 webpage:
http://www.musl-libc.org/

musl-utils-1.1.19-r11 installed size:
122880

musl-utils-1.1.19-r11 license:
MIT BSD GPL2+

```

### `apk` package: `scanelf`

```console
scanelf-1.2.3-r0 description:
Scan ELF binaries for stuff

scanelf-1.2.3-r0 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.2.3-r0 installed size:
94208

scanelf-1.2.3-r0 license:
GPL-2.0

```

### `apk` package: `ssl_client`

```console
ssl_client-1.28.4-r3 description:
EXternal ssl_client for busybox wget

ssl_client-1.28.4-r3 webpage:
http://busybox.net

ssl_client-1.28.4-r3 installed size:
24576

ssl_client-1.28.4-r3 license:
GPL-2.0

```

### `apk` package: `zlib`

```console
zlib-1.2.11-r1 description:
A compression/decompression Library

zlib-1.2.11-r1 webpage:
http://zlib.net

zlib-1.2.11-r1 installed size:
102400

zlib-1.2.11-r1 license:
zlib

```
