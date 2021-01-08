# `express-gateway:1.x`

## Docker Metadata

- Image ID: `sha256:ad08c791a2a01fadaaa242d81f83d8a28b872316cc8e4568c290536874399d28`
- Created: `2021-01-05T18:08:48.110955984Z`
- Virtual Size: ~ 124.40 Mb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["docker-entrypoint.sh"]`
- Command: `["node","-e","require('express-gateway')().run();"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `NODE_VERSION=10.23.1`
  - `YARN_VERSION=1.22.5`
  - `NODE_ENV=production`
  - `NODE_PATH=/usr/local/share/.config/yarn/global/node_modules/`
  - `EG_CONFIG_DIR=/var/lib/eg`
  - `CHOKIDAR_USEPOLLING=true`
- Labels:
  - `maintainer=Vincenzo Chianese, vincenzo@express-gateway.io`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.2.0-r3 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.2.0-r3 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.2.0-r3 installed size:
413696

alpine-baselayout-3.2.0-r3 license:
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
apk-tools-2.10.5-r0 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.10.5-r0 webpage:
https://git.alpinelinux.org/cgit/apk-tools/

apk-tools-2.10.5-r0 installed size:
262144

apk-tools-2.10.5-r0 license:
GPL2

```

### `apk` package: `busybox`

```console
busybox-1.31.1-r9 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.31.1-r9 webpage:
https://busybox.net/

busybox-1.31.1-r9 installed size:
962560

busybox-1.31.1-r9 license:
GPL-2.0-only

```

### `apk` package: `ca-certificates-cacert`

```console
ca-certificates-cacert-20191127-r2 description:
Mozilla bundled certificates

ca-certificates-cacert-20191127-r2 webpage:
https://www.mozilla.org/en-US/about/governance/policies/security-group/certs/

ca-certificates-cacert-20191127-r2 installed size:
245760

ca-certificates-cacert-20191127-r2 license:
MPL-2.0 GPL-2.0-or-later

```

### `apk` package: `libc-utils`

```console
libc-utils-0.7.2-r0 description:
Meta package to pull in correct libc

libc-utils-0.7.2-r0 webpage:
http://alpinelinux.org

libc-utils-0.7.2-r0 installed size:
4096

libc-utils-0.7.2-r0 license:
BSD

```

### `apk` package: `libcrypto1.1`

```console
libcrypto1.1-1.1.1i-r0 description:
Crypto library from openssl

libcrypto1.1-1.1.1i-r0 webpage:
https://www.openssl.org

libcrypto1.1-1.1.1i-r0 installed size:
2764800

libcrypto1.1-1.1.1i-r0 license:
OpenSSL

```

### `apk` package: `libgcc`

```console
libgcc-9.3.0-r0 description:
GNU C compiler runtime libraries

libgcc-9.3.0-r0 webpage:
http://gcc.gnu.org

libgcc-9.3.0-r0 installed size:
90112

libgcc-9.3.0-r0 license:
GPL LGPL

```

### `apk` package: `libssl1.1`

```console
libssl1.1-1.1.1i-r0 description:
SSL shared libraries

libssl1.1-1.1.1i-r0 webpage:
https://www.openssl.org

libssl1.1-1.1.1i-r0 installed size:
540672

libssl1.1-1.1.1i-r0 license:
OpenSSL

```

### `apk` package: `libstdc++`

```console
libstdc++-9.3.0-r0 description:
GNU C++ standard runtime library

libstdc++-9.3.0-r0 webpage:
http://gcc.gnu.org

libstdc++-9.3.0-r0 installed size:
1671168

libstdc++-9.3.0-r0 license:
GPL LGPL

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

### `apk` package: `musl`

```console
musl-1.1.24-r3 description:
the musl c library (libc) implementation

musl-1.1.24-r3 webpage:
https://musl.libc.org/

musl-1.1.24-r3 installed size:
614400

musl-1.1.24-r3 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.1.24-r3 description:
the musl c library (libc) implementation

musl-utils-1.1.24-r3 webpage:
https://musl.libc.org/

musl-utils-1.1.24-r3 installed size:
151552

musl-utils-1.1.24-r3 license:
MIT BSD GPL2+

```

### `apk` package: `scanelf`

```console
scanelf-1.2.4-r0 description:
Scan ELF binaries for stuff

scanelf-1.2.4-r0 webpage:
https://wiki.gentoo.org/wiki/Hardened/PaX_Utilities

scanelf-1.2.4-r0 installed size:
94208

scanelf-1.2.4-r0 license:
GPL-2.0-only

```

### `apk` package: `ssl_client`

```console
ssl_client-1.31.1-r9 description:
EXternal ssl_client for busybox wget

ssl_client-1.31.1-r9 webpage:
https://busybox.net/

ssl_client-1.31.1-r9 installed size:
28672

ssl_client-1.31.1-r9 license:
GPL-2.0-only

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
