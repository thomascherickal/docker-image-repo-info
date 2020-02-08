# `fluentd:v1.9.1-1.0`

## Docker Metadata

- Image ID: `sha256:2d0f50ca7829aa85a5af485cba2c6f70f7ac4513909e032fa6595ef63c02d39b`
- Created: `2020-02-07T23:30:44.775206466Z`
- Virtual Size: ~ 44.87 Mb  
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
  - `Version=1.9.1`
  - `maintainer=Fluentd developers <fluentd@googlegroups.com>`

## `apk` (`.apk`-based packages)

### `apk` package: `alpine-baselayout`

```console
alpine-baselayout-3.1.0-r3 description:
Alpine base dir structure and init scripts

alpine-baselayout-3.1.0-r3 webpage:
https://git.alpinelinux.org/cgit/aports/tree/main/alpine-baselayout

alpine-baselayout-3.1.0-r3 installed size:
409600

alpine-baselayout-3.1.0-r3 license:
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
apk-tools-2.10.3-r1 description:
Alpine Package Keeper - package manager for alpine

apk-tools-2.10.3-r1 webpage:
https://git.alpinelinux.org/cgit/apk-tools/

apk-tools-2.10.3-r1 installed size:
262144

apk-tools-2.10.3-r1 license:
GPL2

```

### `apk` package: `busybox`

```console
busybox-1.29.3-r10 description:
Size optimized toolbox of many common UNIX utilities

busybox-1.29.3-r10 webpage:
http://busybox.net

busybox-1.29.3-r10 installed size:
905216

busybox-1.29.3-r10 license:
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
libcrypto1.1-1.1.1d-r2 description:
Crypto library from openssl

libcrypto1.1-1.1.1d-r2 webpage:
https://www.openssl.org

libcrypto1.1-1.1.1d-r2 installed size:
2748416

libcrypto1.1-1.1.1d-r2 license:
OpenSSL

```

### `apk` package: `libssl1.1`

```console
libssl1.1-1.1.1d-r2 description:
SSL shared libraries

libssl1.1-1.1.1d-r2 webpage:
https://www.openssl.org

libssl1.1-1.1.1d-r2 installed size:
536576

libssl1.1-1.1.1d-r2 license:
OpenSSL

```

### `apk` package: `libtls-standalone`

```console
libtls-standalone-2.7.4-r6 description:
libtls extricated from libressl sources

libtls-standalone-2.7.4-r6 webpage:
http://www.libressl.org/

libtls-standalone-2.7.4-r6 installed size:
110592

libtls-standalone-2.7.4-r6 license:
ISC

```

### `apk` package: `musl`

```console
musl-1.1.20-r5 description:
the musl c library (libc) implementation

musl-1.1.20-r5 webpage:
http://www.musl-libc.org/

musl-1.1.20-r5 installed size:
602112

musl-1.1.20-r5 license:
MIT

```

### `apk` package: `musl-utils`

```console
musl-utils-1.1.20-r5 description:
the musl c library (libc) implementation

musl-utils-1.1.20-r5 webpage:
http://www.musl-libc.org/

musl-utils-1.1.20-r5 installed size:
139264

musl-utils-1.1.20-r5 license:
MIT BSD GPL2+

```

### `apk` package: `ncurses-libs`

```console
ncurses-libs-6.1_p20190105-r0 description:
Ncurses libraries

ncurses-libs-6.1_p20190105-r0 webpage:
https://www.gnu.org/software/ncurses/

ncurses-libs-6.1_p20190105-r0 installed size:
499712

ncurses-libs-6.1_p20190105-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo`

```console
ncurses-terminfo-6.1_p20190105-r0 description:
Console display library (other terminfo files)

ncurses-terminfo-6.1_p20190105-r0 webpage:
https://www.gnu.org/software/ncurses/

ncurses-terminfo-6.1_p20190105-r0 installed size:
7274496

ncurses-terminfo-6.1_p20190105-r0 license:
MIT

```

### `apk` package: `ncurses-terminfo-base`

```console
ncurses-terminfo-base-6.1_p20190105-r0 description:
Descriptions of common terminals

ncurses-terminfo-base-6.1_p20190105-r0 webpage:
https://www.gnu.org/software/ncurses/

ncurses-terminfo-base-6.1_p20190105-r0 installed size:
94208

ncurses-terminfo-base-6.1_p20190105-r0 license:
MIT

```

### `apk` package: `readline`

```console
readline-7.0.003-r1 description:
GNU readline library

readline-7.0.003-r1 webpage:
https://tiswww.cwru.edu/php/chet/readline/rltop.html

readline-7.0.003-r1 installed size:
294912

readline-7.0.003-r1 license:
GPL

```

### `apk` package: `ruby`

```console
ruby-2.5.7-r0 description:
An object-oriented language for quick and easy programming

ruby-2.5.7-r0 webpage:
http://www.ruby-lang.org/en/

ruby-2.5.7-r0 installed size:
40960

ruby-2.5.7-r0 license:
Ruby BSD-2-Clause

```

### `apk` package: `ruby-etc`

```console
ruby-etc-2.5.7-r0 description:
Provides access to information typically stored in UNIX /etc directory

ruby-etc-2.5.7-r0 webpage:
http://www.ruby-lang.org/en/

ruby-etc-2.5.7-r0 installed size:
77824

ruby-etc-2.5.7-r0 license:
BSD-2-Clause

```

### `apk` package: `ruby-irb`

```console
ruby-irb-2.5.7-r0 description:
The Interactive Ruby

ruby-irb-2.5.7-r0 webpage:
http://www.ruby-lang.org/en/

ruby-irb-2.5.7-r0 installed size:
319488

ruby-irb-2.5.7-r0 license:
Ruby BSD-2-Clause

```

### `apk` package: `ruby-libs`

```console
ruby-libs-2.5.7-r0 description:
Libraries necessary to run Ruby

ruby-libs-2.5.7-r0 webpage:
http://www.ruby-lang.org/en/

ruby-libs-2.5.7-r0 installed size:
13094912

ruby-libs-2.5.7-r0 license:
Ruby BSD-2-Clause

```

### `apk` package: `ruby-webrick`

```console
ruby-webrick-2.5.7-r0 description:
HTTP server toolkit for Ruby

ruby-webrick-2.5.7-r0 webpage:
http://www.ruby-lang.org/en/

ruby-webrick-2.5.7-r0 installed size:
315392

ruby-webrick-2.5.7-r0 license:
BSD-2-Clause

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

### `apk` package: `ssl_client`

```console
ssl_client-1.29.3-r10 description:
EXternal ssl_client for busybox wget

ssl_client-1.29.3-r10 webpage:
http://busybox.net

ssl_client-1.29.3-r10 installed size:
28672

ssl_client-1.29.3-r10 license:
GPL-2.0

```

### `apk` package: `tini`

```console
tini-0.18.0-r0 description:
A tiny but valid init for containers

tini-0.18.0-r0 webpage:
https://github.com/krallin/tini

tini-0.18.0-r0 installed size:
36864

tini-0.18.0-r0 license:
MIT

```

### `apk` package: `yaml`

```console
yaml-0.2.1-r0 description:
YAML 1.1 parser and emitter written in C

yaml-0.2.1-r0 webpage:
http://pyyaml.org/wiki/LibYAML

yaml-0.2.1-r0 installed size:
126976

yaml-0.2.1-r0 license:
MIT

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
