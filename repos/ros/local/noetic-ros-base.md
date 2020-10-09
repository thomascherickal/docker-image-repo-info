# `ros:noetic-ros-base`

## Docker Metadata

- Image ID: `sha256:3ca25dab881d3468ef6155113e4f91fbde961df564d0e4da60837ee105a544a8`
- Created: `2020-09-26T01:50:31.744866129Z`
- Virtual Size: ~ 1.18 Gb  
  (total size of all layers on-disk)
- Arch: `linux`/`amd64`
- Entrypoint: `["/ros_entrypoint.sh"]`
- Command: `["bash"]`
- Environment:
  - `PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin`
  - `LANG=C.UTF-8`
  - `LC_ALL=C.UTF-8`
  - `ROS_DISTRO=noetic`

## `dpkg` (`.deb`-based packages)

### `dpkg` source package: `acl=2.2.53-6`

Binary Packages:

- `libacl1:amd64=2.2.53-6`

Licenses: (parsed from: `/usr/share/doc/libacl1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris acl=2.2.53-6
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-6.dsc' acl_2.2.53-6.dsc 2336 SHA256:02dad794aa09133e557552d75568324ed3e84fb56e93626e67993cf54a97df34
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz' acl_2.2.53.orig.tar.gz 524300 SHA256:06be9865c6f418d851ff4494e12406568353b891ffe1f596b34693c387af26c7
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53.orig.tar.gz.asc' acl_2.2.53.orig.tar.gz.asc 833 SHA256:06849bece0b56a6a7269173abe101cff223bb9346d74027a3cd5ff80914abf4b
'http://archive.ubuntu.com/ubuntu/pool/main/a/acl/acl_2.2.53-6.debian.tar.xz' acl_2.2.53-6.debian.tar.xz 25108 SHA256:c80e6150d9b213e52f5e65ff78d4ee95a71b5a258c1f8b980365d20ed1753a5c
```

### `dpkg` source package: `adduser=3.118ubuntu2`

Binary Packages:

- `adduser=3.118ubuntu2`

Licenses: (parsed from: `/usr/share/doc/adduser/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris adduser=3.118ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu2.dsc' adduser_3.118ubuntu2.dsc 1131 SHA256:785f99d8c75c972cd42d3fab3afa07f97299bb1d70013fe5d295f045224774bb
'http://archive.ubuntu.com/ubuntu/pool/main/a/adduser/adduser_3.118ubuntu2.tar.xz' adduser_3.118ubuntu2.tar.xz 222364 SHA256:9429124c39c381b541005da6f0ae29831bd6533dd65c923e06ca2a7c310db382
```

### `dpkg` source package: `apr-util=1.6.1-4ubuntu2`

Binary Packages:

- `libaprutil1:amd64=1.6.1-4ubuntu2`
- `libaprutil1-dev=1.6.1-4ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libaprutil1/copyright`, `/usr/share/doc/libaprutil1-dev/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr-util=1.6.1-4ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-4ubuntu2.dsc' apr-util_1.6.1-4ubuntu2.dsc 2686 SHA256:bf8be458f58a6b1576d35bc78647bb0e990fc0d0c47ee7b51a5e2ecf3d378aac
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1.orig.tar.bz2' apr-util_1.6.1.orig.tar.bz2 428595 SHA256:d3e12f7b6ad12687572a3a39475545a072608f4ba03a6ce8a3778f607dd0035b
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr-util/apr-util_1.6.1-4ubuntu2.debian.tar.xz' apr-util_1.6.1-4ubuntu2.debian.tar.xz 213052 SHA256:2293c33f2e8d354aae7285e6037820d32305dcf4843093123c0683946ae35967
```

### `dpkg` source package: `apr=1.6.5-1ubuntu1`

Binary Packages:

- `libapr1:amd64=1.6.5-1ubuntu1`
- `libapr1-dev=1.6.5-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libapr1/copyright`, `/usr/share/doc/libapr1-dev/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris apr=1.6.5-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5-1ubuntu1.dsc' apr_1.6.5-1ubuntu1.dsc 2390 SHA256:9e9d5b1be5c9d17c4720d43096064da70a4cba1593f10c272328e16f8ed4c656
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5.orig.tar.bz2' apr_1.6.5.orig.tar.bz2 855393 SHA256:a67ca9fcf9c4ff59bce7f428a323c8b5e18667fdea7b0ebad47d194371b0a105
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5.orig.tar.bz2.asc' apr_1.6.5.orig.tar.bz2.asc 801 SHA256:9beff0bb06f4cbbb006176af93258d946d33b7fb54aac13a4c90cfba1cfd0c88
'http://archive.ubuntu.com/ubuntu/pool/main/a/apr/apr_1.6.5-1ubuntu1.debian.tar.xz' apr_1.6.5-1ubuntu1.debian.tar.xz 213596 SHA256:faca1bccb281c7d91bf0846ee908dd0be53b4482c0a1850e03397307682717d1
```

### `dpkg` source package: `apt=2.0.2ubuntu0.1`

Binary Packages:

- `apt=2.0.2ubuntu0.1`
- `libapt-pkg6.0:amd64=2.0.2ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/apt/copyright`, `/usr/share/doc/libapt-pkg6.0/copyright`)

- `GPL-2`
- `GPLv2+`

Source:

```console
$ apt-get source -qq --print-uris apt=2.0.2ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.0.2ubuntu0.1.dsc' apt_2.0.2ubuntu0.1.dsc 2542 SHA512:e990fd2133f79395fe56e93aefa6aa6459e85f9ac71f8d64119eec3c8028ddbc80581661b9744919f1d8154f7973bbb7b1c0bfd538f3ab5872ccf168ac96e13d
'http://archive.ubuntu.com/ubuntu/pool/main/a/apt/apt_2.0.2ubuntu0.1.tar.xz' apt_2.0.2ubuntu0.1.tar.xz 2169516 SHA512:dce019214bb737e09affe0e0ca7ff300a9d3d16aabce98fec3e5f3032d28610a3123122286b6f2b7286112ad86ff1cf5d35657085d27e9875315689375458beb
```

### `dpkg` source package: `attr=1:2.4.48-5`

Binary Packages:

- `libattr1:amd64=1:2.4.48-5`

Licenses: (parsed from: `/usr/share/doc/libattr1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2+`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris attr=1:2.4.48-5
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-5.dsc' attr_2.4.48-5.dsc 2433 SHA256:0b20a285b758083e2e202ffdd2930cef1bf84fee498791fc3e26b69a3bced01d
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz' attr_2.4.48.orig.tar.gz 467840 SHA256:5ead72b358ec709ed00bbf7a9eaef1654baad937c001c044fe8b74c57f5324e7
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48.orig.tar.gz.asc' attr_2.4.48.orig.tar.gz.asc 833 SHA256:5d23c2c83cc13d170f1c209f48d0efa1fc46d16487b790e9996c5206dcfe0395
'http://archive.ubuntu.com/ubuntu/pool/main/a/attr/attr_2.4.48-5.debian.tar.xz' attr_2.4.48-5.debian.tar.xz 25560 SHA256:02238253d324250dabdc0434f7de045d85df93458995a465ac434f2a3978a312
```

### `dpkg` source package: `audit=1:2.8.5-2ubuntu6`

Binary Packages:

- `libaudit-common=1:2.8.5-2ubuntu6`
- `libaudit1:amd64=1:2.8.5-2ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libaudit-common/copyright`, `/usr/share/doc/libaudit1/copyright`)

- `GPL-1`
- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris audit=1:2.8.5-2ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5-2ubuntu6.dsc' audit_2.8.5-2ubuntu6.dsc 2764 SHA256:b149fad8217d68a80299c1ef72539ee7d756146d692b7e51eade7341e60ac528
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5.orig.tar.gz' audit_2.8.5.orig.tar.gz 1140694 SHA256:0e5d4103646e00f8d1981e1cd2faea7a2ae28e854c31a803e907a383c5e2ecb7
'http://archive.ubuntu.com/ubuntu/pool/main/a/audit/audit_2.8.5-2ubuntu6.debian.tar.xz' audit_2.8.5-2ubuntu6.debian.tar.xz 18712 SHA256:d85ecf206bfe256a86e6d39602cd2744beda264a28e413f31c4da227e6542ea7
```

### `dpkg` source package: `autoconf=2.69-11.1`

Binary Packages:

- `autoconf=2.69-11.1`

Licenses: (parsed from: `/usr/share/doc/autoconf/copyright`)

- `GFDL-1.3`
- `GFDL-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `GPL-3`
- `GPL-3+`
- `GPL-3+ with Autoconf exception`
- `GPL-3+ with Texinfo exception`
- `MIT-X-Consortium`
- `no-modification`
- `other`
- `permissive`
- `permissive-long-disclaimer`
- `permissive-short-disclaimer`
- `permissive-without-disclaimer`
- `permissive-without-notices-or-disclaimer`

Source:

```console
$ apt-get source -qq --print-uris autoconf=2.69-11.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-11.1.dsc' autoconf_2.69-11.1.dsc 1735 SHA256:06ab6e617ed8d07eecbc29a1669cd748b7ce11ab457c186e7e8794fe02b231ba
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69.orig.tar.xz' autoconf_2.69.orig.tar.xz 1214744 SHA256:64ebcec9f8ac5b2487125a86a7760d2591ac9e1d3dbd59489633f9de62a57684
'http://archive.ubuntu.com/ubuntu/pool/main/a/autoconf/autoconf_2.69-11.1.debian.tar.xz' autoconf_2.69-11.1.debian.tar.xz 23488 SHA256:ff76de2fc2956773dc6f47301b66822ea3074a2e556dc2e761cb411342d2228b
```

### `dpkg` source package: `automake-1.16=1:1.16.1-4ubuntu6`

Binary Packages:

- `automake=1:1.16.1-4ubuntu6`

Licenses: (parsed from: `/usr/share/doc/automake/copyright`)

- `GFDL-1.3`
- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris automake-1.16=1:1.16.1-4ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.1-4ubuntu6.dsc' automake-1.16_1.16.1-4ubuntu6.dsc 1476 SHA256:03c69a65de46468cf20f0621330d137d21249aa7033a242b076aaff3ee0c7a33
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.1.orig.tar.xz' automake-1.16_1.16.1.orig.tar.xz 1534936 SHA256:5d05bb38a23fd3312b10aea93840feec685bdf4a41146e78882848165d3ae921
'http://archive.ubuntu.com/ubuntu/pool/main/a/automake-1.16/automake-1.16_1.16.1-4ubuntu6.debian.tar.xz' automake-1.16_1.16.1-4ubuntu6.debian.tar.xz 15348 SHA256:ed3474bddbe69ed00492113e3e2bbfc999373768e37f8a78555401c8abcbccca
```

### `dpkg` source package: `autotools-dev=20180224.1`

Binary Packages:

- `autotools-dev=20180224.1`

Licenses: (parsed from: `/usr/share/doc/autotools-dev/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris autotools-dev=20180224.1
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1.dsc' autotools-dev_20180224.1.dsc 1643 SHA256:795f558377bf6c90280c293b2711afc094cd1bf6ae486a395e1361ffd242cd2f
'http://archive.ubuntu.com/ubuntu/pool/main/a/autotools-dev/autotools-dev_20180224.1.tar.xz' autotools-dev_20180224.1.tar.xz 68256 SHA256:355a4d8461dfedebd2c5194603197712a10f71e20de73a35ab6e90b7acf3e837
```

### `dpkg` source package: `base-files=11ubuntu5.2`

Binary Packages:

- `base-files=11ubuntu5.2`

Licenses: (parsed from: `/usr/share/doc/base-files/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris base-files=11ubuntu5.2
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_11ubuntu5.2.dsc' base-files_11ubuntu5.2.dsc 1676 SHA512:8f10b639796469f1d8b9eff30fccf8418148b8a4d863771ce9f5936c4b33ff9e1d4adfd0a7140a5eff54096c31c0cb566996215b7985cbf591594cf9a0d23fd9
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-files/base-files_11ubuntu5.2.tar.xz' base-files_11ubuntu5.2.tar.xz 80528 SHA512:45aee06a5fb08562aff51fd1ceedbf9749535820754b9a64da989326b6c05c2e73b88d1cb3e03d078ce899a84b4c383cd19ad6a5be32573c936293bd5d2932cf
```

### `dpkg` source package: `base-passwd=3.5.47`

Binary Packages:

- `base-passwd=3.5.47`

Licenses: (parsed from: `/usr/share/doc/base-passwd/copyright`)

- `GPL-2`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris base-passwd=3.5.47
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.47.dsc' base-passwd_3.5.47.dsc 1757 SHA256:5a77a4cce51d1eb72e9d96d4083c641435c05888922c7bd3fa6b4395bf9afad3
'http://archive.ubuntu.com/ubuntu/pool/main/b/base-passwd/base-passwd_3.5.47.tar.xz' base-passwd_3.5.47.tar.xz 53024 SHA256:9810ae0216e96bf9fc7ca6163d47ef8ec7d1677f533451af5911d8202a490a23
```

### `dpkg` source package: `bash=5.0-6ubuntu1.1`

Binary Packages:

- `bash=5.0-6ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/bash/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris bash=5.0-6ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-6ubuntu1.1.dsc' bash_5.0-6ubuntu1.1.dsc 2418 SHA512:283e6fa78ac1a13e6e3a70efa6f67817871b12c1fe099475dfe6b87fd9f2926406446fabb72a66d8546ad320976761ffe68867a1e90bd6a5f97c07e851df9933
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0.orig.tar.xz' bash_5.0.orig.tar.xz 5554808 SHA512:f3a719997a8515bae7e84701afafc9b2cdd23c95d29533adb678000b08eba968450b93d5576c3cffbeccbdcd95b713db830e8efeda689258dcfe6f15f0c5dec4
'http://archive.ubuntu.com/ubuntu/pool/main/b/bash/bash_5.0-6ubuntu1.1.debian.tar.xz' bash_5.0-6ubuntu1.1.debian.tar.xz 74356 SHA512:450eacea5316075107da9951356021091dfc96889057769590ae8505fa851a99d2f48ce300281b8a448c87e9573cfa2f68a04369ee97955be204e73fa2fd6385
```

### `dpkg` source package: `binutils=2.34-6ubuntu1`

Binary Packages:

- `binutils=2.34-6ubuntu1`
- `binutils-common:amd64=2.34-6ubuntu1`
- `binutils-x86-64-linux-gnu=2.34-6ubuntu1`
- `libbinutils:amd64=2.34-6ubuntu1`
- `libctf-nobfd0:amd64=2.34-6ubuntu1`
- `libctf0:amd64=2.34-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/binutils/copyright`, `/usr/share/doc/binutils-common/copyright`, `/usr/share/doc/binutils-x86-64-linux-gnu/copyright`, `/usr/share/doc/libbinutils/copyright`, `/usr/share/doc/libctf-nobfd0/copyright`, `/usr/share/doc/libctf0/copyright`)

- `GFDL`
- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris binutils=2.34-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.34-6ubuntu1.dsc' binutils_2.34-6ubuntu1.dsc 8767 SHA256:ab7ef15972388dfc74e330893b195076f87cd55e3c9a58c8fa31406755fbd667
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.34.orig.tar.xz' binutils_2.34.orig.tar.xz 21637796 SHA256:f00b0e8803dc9bab1e2165bd568528135be734df3fabf8d0161828cd56028952
'http://archive.ubuntu.com/ubuntu/pool/main/b/binutils/binutils_2.34-6ubuntu1.debian.tar.xz' binutils_2.34-6ubuntu1.debian.tar.xz 155276 SHA256:a96049d0b8833f6b89105bc32fa4d9b79a157d8e753b27721741a0229d801034
```

### `dpkg` source package: `boost-defaults=1.71.0.0ubuntu2`

Binary Packages:

- `libboost-all-dev=1.71.0.0ubuntu2`
- `libboost-atomic-dev:amd64=1.71.0.0ubuntu2`
- `libboost-chrono-dev:amd64=1.71.0.0ubuntu2`
- `libboost-container-dev:amd64=1.71.0.0ubuntu2`
- `libboost-context-dev:amd64=1.71.0.0ubuntu2`
- `libboost-coroutine-dev:amd64=1.71.0.0ubuntu2`
- `libboost-date-time-dev:amd64=1.71.0.0ubuntu2`
- `libboost-dev:amd64=1.71.0.0ubuntu2`
- `libboost-exception-dev:amd64=1.71.0.0ubuntu2`
- `libboost-fiber-dev:amd64=1.71.0.0ubuntu2`
- `libboost-filesystem-dev:amd64=1.71.0.0ubuntu2`
- `libboost-graph-dev:amd64=1.71.0.0ubuntu2`
- `libboost-graph-parallel-dev=1.71.0.0ubuntu2`
- `libboost-iostreams-dev:amd64=1.71.0.0ubuntu2`
- `libboost-locale-dev:amd64=1.71.0.0ubuntu2`
- `libboost-log-dev=1.71.0.0ubuntu2`
- `libboost-math-dev:amd64=1.71.0.0ubuntu2`
- `libboost-mpi-dev=1.71.0.0ubuntu2`
- `libboost-mpi-python-dev=1.71.0.0ubuntu2`
- `libboost-numpy-dev=1.71.0.0ubuntu2`
- `libboost-program-options-dev:amd64=1.71.0.0ubuntu2`
- `libboost-python-dev=1.71.0.0ubuntu2`
- `libboost-random-dev:amd64=1.71.0.0ubuntu2`
- `libboost-regex-dev:amd64=1.71.0.0ubuntu2`
- `libboost-serialization-dev:amd64=1.71.0.0ubuntu2`
- `libboost-stacktrace-dev:amd64=1.71.0.0ubuntu2`
- `libboost-system-dev:amd64=1.71.0.0ubuntu2`
- `libboost-test-dev:amd64=1.71.0.0ubuntu2`
- `libboost-thread-dev:amd64=1.71.0.0ubuntu2`
- `libboost-timer-dev:amd64=1.71.0.0ubuntu2`
- `libboost-tools-dev=1.71.0.0ubuntu2`
- `libboost-type-erasure-dev:amd64=1.71.0.0ubuntu2`
- `libboost-wave-dev:amd64=1.71.0.0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libboost-all-dev/copyright`, `/usr/share/doc/libboost-atomic-dev/copyright`, `/usr/share/doc/libboost-chrono-dev/copyright`, `/usr/share/doc/libboost-container-dev/copyright`, `/usr/share/doc/libboost-context-dev/copyright`, `/usr/share/doc/libboost-coroutine-dev/copyright`, `/usr/share/doc/libboost-date-time-dev/copyright`, `/usr/share/doc/libboost-dev/copyright`, `/usr/share/doc/libboost-exception-dev/copyright`, `/usr/share/doc/libboost-fiber-dev/copyright`, `/usr/share/doc/libboost-filesystem-dev/copyright`, `/usr/share/doc/libboost-graph-dev/copyright`, `/usr/share/doc/libboost-graph-parallel-dev/copyright`, `/usr/share/doc/libboost-iostreams-dev/copyright`, `/usr/share/doc/libboost-locale-dev/copyright`, `/usr/share/doc/libboost-log-dev/copyright`, `/usr/share/doc/libboost-math-dev/copyright`, `/usr/share/doc/libboost-mpi-dev/copyright`, `/usr/share/doc/libboost-mpi-python-dev/copyright`, `/usr/share/doc/libboost-numpy-dev/copyright`, `/usr/share/doc/libboost-program-options-dev/copyright`, `/usr/share/doc/libboost-python-dev/copyright`, `/usr/share/doc/libboost-random-dev/copyright`, `/usr/share/doc/libboost-regex-dev/copyright`, `/usr/share/doc/libboost-serialization-dev/copyright`, `/usr/share/doc/libboost-stacktrace-dev/copyright`, `/usr/share/doc/libboost-system-dev/copyright`, `/usr/share/doc/libboost-test-dev/copyright`, `/usr/share/doc/libboost-thread-dev/copyright`, `/usr/share/doc/libboost-timer-dev/copyright`, `/usr/share/doc/libboost-tools-dev/copyright`, `/usr/share/doc/libboost-type-erasure-dev/copyright`, `/usr/share/doc/libboost-wave-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris boost-defaults=1.71.0.0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost-defaults/boost-defaults_1.71.0.0ubuntu2.dsc' boost-defaults_1.71.0.0ubuntu2.dsc 4789 SHA256:ac94fe30d32c9c15b944ec6407a2ee5e689ba6fff57bd2fe494a7f8d57fd771e
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost-defaults/boost-defaults_1.71.0.0ubuntu2.tar.xz' boost-defaults_1.71.0.0ubuntu2.tar.xz 11984 SHA256:0748142a99f3d3fac5d522f998137e08207d4856acd26b406ed1f495fc28fb0b
```

### `dpkg` source package: `boost1.71=1.71.0-6ubuntu6`

Binary Packages:

- `libboost-atomic1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-atomic1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-chrono1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-chrono1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-container1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-container1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-context1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-context1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-coroutine1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-coroutine1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-date-time1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-date-time1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-exception1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-fiber1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-fiber1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-filesystem1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-filesystem1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-graph-parallel1.71-dev=1.71.0-6ubuntu6`
- `libboost-graph-parallel1.71.0=1.71.0-6ubuntu6`
- `libboost-graph1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-graph1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-iostreams1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-iostreams1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-locale1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-locale1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-log1.71-dev=1.71.0-6ubuntu6`
- `libboost-log1.71.0=1.71.0-6ubuntu6`
- `libboost-math1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-math1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-mpi-python1.71-dev=1.71.0-6ubuntu6`
- `libboost-mpi-python1.71.0=1.71.0-6ubuntu6`
- `libboost-mpi1.71-dev=1.71.0-6ubuntu6`
- `libboost-mpi1.71.0=1.71.0-6ubuntu6`
- `libboost-numpy1.71-dev=1.71.0-6ubuntu6`
- `libboost-numpy1.71.0=1.71.0-6ubuntu6`
- `libboost-program-options1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-program-options1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-python1.71-dev=1.71.0-6ubuntu6`
- `libboost-python1.71.0=1.71.0-6ubuntu6`
- `libboost-random1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-random1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-regex1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-regex1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-serialization1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-serialization1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-stacktrace1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-stacktrace1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-system1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-system1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-test1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-test1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-thread1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-thread1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-timer1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-timer1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-type-erasure1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-type-erasure1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost-wave1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost-wave1.71.0:amd64=1.71.0-6ubuntu6`
- `libboost1.71-dev:amd64=1.71.0-6ubuntu6`
- `libboost1.71-tools-dev=1.71.0-6ubuntu6`

Licenses: (parsed from: `/usr/share/doc/libboost-atomic1.71-dev/copyright`, `/usr/share/doc/libboost-atomic1.71.0/copyright`, `/usr/share/doc/libboost-chrono1.71-dev/copyright`, `/usr/share/doc/libboost-chrono1.71.0/copyright`, `/usr/share/doc/libboost-container1.71-dev/copyright`, `/usr/share/doc/libboost-container1.71.0/copyright`, `/usr/share/doc/libboost-context1.71-dev/copyright`, `/usr/share/doc/libboost-context1.71.0/copyright`, `/usr/share/doc/libboost-coroutine1.71-dev/copyright`, `/usr/share/doc/libboost-coroutine1.71.0/copyright`, `/usr/share/doc/libboost-date-time1.71-dev/copyright`, `/usr/share/doc/libboost-date-time1.71.0/copyright`, `/usr/share/doc/libboost-exception1.71-dev/copyright`, `/usr/share/doc/libboost-fiber1.71-dev/copyright`, `/usr/share/doc/libboost-fiber1.71.0/copyright`, `/usr/share/doc/libboost-filesystem1.71-dev/copyright`, `/usr/share/doc/libboost-filesystem1.71.0/copyright`, `/usr/share/doc/libboost-graph-parallel1.71-dev/copyright`, `/usr/share/doc/libboost-graph-parallel1.71.0/copyright`, `/usr/share/doc/libboost-graph1.71-dev/copyright`, `/usr/share/doc/libboost-graph1.71.0/copyright`, `/usr/share/doc/libboost-iostreams1.71-dev/copyright`, `/usr/share/doc/libboost-iostreams1.71.0/copyright`, `/usr/share/doc/libboost-locale1.71-dev/copyright`, `/usr/share/doc/libboost-locale1.71.0/copyright`, `/usr/share/doc/libboost-log1.71-dev/copyright`, `/usr/share/doc/libboost-log1.71.0/copyright`, `/usr/share/doc/libboost-math1.71-dev/copyright`, `/usr/share/doc/libboost-math1.71.0/copyright`, `/usr/share/doc/libboost-mpi-python1.71-dev/copyright`, `/usr/share/doc/libboost-mpi-python1.71.0/copyright`, `/usr/share/doc/libboost-mpi1.71-dev/copyright`, `/usr/share/doc/libboost-mpi1.71.0/copyright`, `/usr/share/doc/libboost-numpy1.71-dev/copyright`, `/usr/share/doc/libboost-numpy1.71.0/copyright`, `/usr/share/doc/libboost-program-options1.71-dev/copyright`, `/usr/share/doc/libboost-program-options1.71.0/copyright`, `/usr/share/doc/libboost-python1.71-dev/copyright`, `/usr/share/doc/libboost-python1.71.0/copyright`, `/usr/share/doc/libboost-random1.71-dev/copyright`, `/usr/share/doc/libboost-random1.71.0/copyright`, `/usr/share/doc/libboost-regex1.71-dev/copyright`, `/usr/share/doc/libboost-regex1.71.0/copyright`, `/usr/share/doc/libboost-serialization1.71-dev/copyright`, `/usr/share/doc/libboost-serialization1.71.0/copyright`, `/usr/share/doc/libboost-stacktrace1.71-dev/copyright`, `/usr/share/doc/libboost-stacktrace1.71.0/copyright`, `/usr/share/doc/libboost-system1.71-dev/copyright`, `/usr/share/doc/libboost-system1.71.0/copyright`, `/usr/share/doc/libboost-test1.71-dev/copyright`, `/usr/share/doc/libboost-test1.71.0/copyright`, `/usr/share/doc/libboost-thread1.71-dev/copyright`, `/usr/share/doc/libboost-thread1.71.0/copyright`, `/usr/share/doc/libboost-timer1.71-dev/copyright`, `/usr/share/doc/libboost-timer1.71.0/copyright`, `/usr/share/doc/libboost-type-erasure1.71-dev/copyright`, `/usr/share/doc/libboost-type-erasure1.71.0/copyright`, `/usr/share/doc/libboost-wave1.71-dev/copyright`, `/usr/share/doc/libboost-wave1.71.0/copyright`, `/usr/share/doc/libboost1.71-dev/copyright`, `/usr/share/doc/libboost1.71-tools-dev/copyright`)

- `Apache-2.0`
- `BSD2`
- `BSD3_DEShaw`
- `BSD3_Google`
- `BSL-1.0`
- `Caramel`
- `CrystalClear`
- `HP`
- `Jam`
- `Kempf`
- `MIT`
- `NIST`
- `OldBoost1`
- `OldBoost2`
- `OldBoost3`
- `Python`
- `SGI`
- `Spencer`
- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris boost1.71=1.71.0-6ubuntu6
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.71/boost1.71_1.71.0-6ubuntu6.dsc' boost1.71_1.71.0-6ubuntu6.dsc 8517 SHA256:e05b5d8de7633e2bf353e9c75d999eafd93bdf47c993023d38f4e5ef5311557b
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.71/boost1.71_1.71.0.orig.tar.xz' boost1.71_1.71.0.orig.tar.xz 56601144 SHA256:e30fb3f666df75fc2ba23403ccbd8bcb0ee5595dc099412b4abde7a9fdde3918
'http://archive.ubuntu.com/ubuntu/pool/main/b/boost1.71/boost1.71_1.71.0-6ubuntu6.debian.tar.xz' boost1.71_1.71.0-6ubuntu6.debian.tar.xz 362348 SHA256:56031ade12bf8ca7c196f11f4afd5d2cc30ab840d2a1f1cec5e7ad87b68addeb
```

### `dpkg` source package: `brotli=1.0.7-6build1`

Binary Packages:

- `libbrotli1:amd64=1.0.7-6build1`

Licenses: (parsed from: `/usr/share/doc/libbrotli1/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris brotli=1.0.7-6build1
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7-6build1.dsc' brotli_1.0.7-6build1.dsc 2316 SHA256:6d46dbb44a7eb0442dc9743a803d6297809817c66a269a41e53009169a071257
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7.orig.tar.gz' brotli_1.0.7.orig.tar.gz 23827908 SHA256:4c61bfb0faca87219ea587326c467b95acb25555b53d1a421ffa3c8a9296ee2c
'http://archive.ubuntu.com/ubuntu/pool/main/b/brotli/brotli_1.0.7-6build1.debian.tar.xz' brotli_1.0.7-6build1.debian.tar.xz 4416 SHA256:7346c025427b3466252dc94d8a0d3e87692107a4d2ca49a382ac4de14e2957d5
```

### `dpkg` source package: `build-essential=12.8ubuntu1`

Binary Packages:

- `build-essential=12.8ubuntu1`

Licenses: (parsed from: `/usr/share/doc/build-essential/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris build-essential=12.8ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/b/build-essential/build-essential_12.8ubuntu1.dsc' build-essential_12.8ubuntu1.dsc 2246 SHA256:c01d45b98ba66df67e4426f1652986a640d56bbb9bb541ddd10a91efcc63e7a7
'http://archive.ubuntu.com/ubuntu/pool/main/b/build-essential/build-essential_12.8ubuntu1.tar.xz' build-essential_12.8ubuntu1.tar.xz 51104 SHA256:ba6afedc701c0fd6bc0210150a2733bc9ac479b3c47a508cc0da3c57acf06484
```

### `dpkg` source package: `bzip2=1.0.8-2`

Binary Packages:

- `bzip2=1.0.8-2`
- `libbz2-1.0:amd64=1.0.8-2`
- `libbz2-dev:amd64=1.0.8-2`

Licenses: (parsed from: `/usr/share/doc/bzip2/copyright`, `/usr/share/doc/libbz2-1.0/copyright`, `/usr/share/doc/libbz2-dev/copyright`)

- `BSD-variant`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris bzip2=1.0.8-2
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-2.dsc' bzip2_1.0.8-2.dsc 2180 SHA256:646cdcbb786a89a647cfafb280ef467143c06c445c4bf6fe69ec4a7882943064
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8.orig.tar.gz' bzip2_1.0.8.orig.tar.gz 810029 SHA256:ab5a03176ee106d3f0fa90e381da478ddae405918153cca248e682cd0c4a2269
'http://archive.ubuntu.com/ubuntu/pool/main/b/bzip2/bzip2_1.0.8-2.debian.tar.bz2' bzip2_1.0.8-2.debian.tar.bz2 26032 SHA256:237c8619bc9bc16f357b1077064a3e58aa1a230dadb4b9bb3bd8dc8f454afc0b
```

### `dpkg` source package: `ca-certificates=20190110ubuntu1.1`

Binary Packages:

- `ca-certificates=20190110ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/ca-certificates/copyright`)

- `GPL-2`
- `GPL-2+`
- `MPL-2.0`

Source:

```console
$ apt-get source -qq --print-uris ca-certificates=20190110ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110ubuntu1.1.dsc' ca-certificates_20190110ubuntu1.1.dsc 1921 SHA512:1457b40fa16171c622ce4164f79067a17031d1f2b77cede0000d9bda75dc9179173d3bac33dfd98ce454dbce71c8d8417a024d6569216d6fc451718468467bf9
'http://archive.ubuntu.com/ubuntu/pool/main/c/ca-certificates/ca-certificates_20190110ubuntu1.1.tar.xz' ca-certificates_20190110ubuntu1.1.tar.xz 243736 SHA512:1be3d0fd46bd4dbe5d6bb78391f2ee18ebb8283df1a513da80765bde63e770fe0eabb915375d81584c81f07fa71dc5529c3679069dae7d88bdb7fc0c864ced79
```

### `dpkg` source package: `cdebconf=0.251ubuntu1`

Binary Packages:

- `libdebconfclient0:amd64=0.251ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris cdebconf=0.251ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.251ubuntu1.dsc' cdebconf_0.251ubuntu1.dsc 2858 SHA256:0753b98ec773e743de19d393f444a8b88915ad75340cc58007eb7c309031121d
'http://archive.ubuntu.com/ubuntu/pool/main/c/cdebconf/cdebconf_0.251ubuntu1.tar.xz' cdebconf_0.251ubuntu1.tar.xz 276744 SHA256:d07848e52aecb70e82d8bafd082ecee3cccd7a8229b59527e07cc49023aa22d0
```

### `dpkg` source package: `cmake=3.16.3-1ubuntu1`

Binary Packages:

- `cmake=3.16.3-1ubuntu1`
- `cmake-data=3.16.3-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/cmake/copyright`, `/usr/share/doc/cmake-data/copyright`)

- `Apache-2.0`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause`
- `GPL-2`
- `GPL-2+with_exception`
- `GPL-3`
- `GPL-3+with_exception`
- `ISC`
- `MIT-like`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris cmake=3.16.3-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.16.3-1ubuntu1.dsc' cmake_3.16.3-1ubuntu1.dsc 3153 SHA256:d2838be8ee2aa92bb810722f87d3abe65e3f95ce5872f6e2e1789980574e4b89
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.16.3.orig.tar.gz' cmake_3.16.3.orig.tar.gz 9111826 SHA256:e54f16df9b53dac30fd626415833a6e75b0e47915393843da1825b096ee60668
'http://archive.ubuntu.com/ubuntu/pool/main/c/cmake/cmake_3.16.3-1ubuntu1.debian.tar.xz' cmake_3.16.3-1ubuntu1.debian.tar.xz 28936 SHA256:d071c791b5c7387846db25b78ddfdd8bdfa12dbd201d2a16b5c2387f9c971c04
```

### `dpkg` source package: `console-bridge=0.4.4+dfsg-1build1`

Binary Packages:

- `libconsole-bridge-dev:amd64=0.4.4+dfsg-1build1`
- `libconsole-bridge0.4:amd64=0.4.4+dfsg-1build1`

Licenses: (parsed from: `/usr/share/doc/libconsole-bridge-dev/copyright`, `/usr/share/doc/libconsole-bridge0.4/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris console-bridge=0.4.4+dfsg-1build1
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_0.4.4+dfsg-1build1.dsc' console-bridge_0.4.4+dfsg-1build1.dsc 2306 SHA256:fcdc1bde378e17db69a32bab6bb8f93161c8e1f58c0f47063f4a8dd2bec002b2
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_0.4.4+dfsg.orig.tar.xz' console-bridge_0.4.4+dfsg.orig.tar.xz 5688 SHA256:8fc6dacfeed0b67bb0fa96b8822b0f120961ff12830d1bee61f70cf5f3cbcb53
'http://archive.ubuntu.com/ubuntu/pool/universe/c/console-bridge/console-bridge_0.4.4+dfsg-1build1.debian.tar.xz' console-bridge_0.4.4+dfsg-1build1.debian.tar.xz 3744 SHA256:6033acc38324729d3cbff79210149ddc38be28ac2bfbcf703d352845314c49e3
```

### `dpkg` source package: `coreutils=8.30-3ubuntu2`

Binary Packages:

- `coreutils=8.30-3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/coreutils/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris coreutils=8.30-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.30-3ubuntu2.dsc' coreutils_8.30-3ubuntu2.dsc 2048 SHA256:f36fe0ac14978b240a750b79d2bbd737d6b1939296c3a287899933aa2a1906ea
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.30.orig.tar.xz' coreutils_8.30.orig.tar.xz 5359532 SHA256:e831b3a86091496cdba720411f9748de81507798f6130adeaef872d206e1b057
'http://archive.ubuntu.com/ubuntu/pool/main/c/coreutils/coreutils_8.30-3ubuntu2.debian.tar.xz' coreutils_8.30-3ubuntu2.debian.tar.xz 39636 SHA256:98204ef9d94e5c567880cd0245fdb7940eaf7592d6c6830c300ad117628b351f
```

### `dpkg` source package: `curl=7.68.0-1ubuntu2.2`

Binary Packages:

- `libcurl4:amd64=7.68.0-1ubuntu2.2`

Licenses: (parsed from: `/usr/share/doc/libcurl4/copyright`)

- `BSD-3-Clause`
- `BSD-4-Clause`
- `ISC`
- `curl`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris curl=7.68.0-1ubuntu2.2
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0-1ubuntu2.2.dsc' curl_7.68.0-1ubuntu2.2.dsc 2733 SHA512:19eb5cc831f04738cc18b31bd1f681af35229c90844e96b523f1f84e121d33195bff8258b085bd44bf8974f8cbaa1c88098cab0de5a00a836a9f0101f4817f98
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0.orig.tar.gz' curl_7.68.0.orig.tar.gz 4096350 SHA512:58b42c08b1cf4cb6e68f8e469d5b5f6298eebe286ba2677ad29e1a7eefd15b8609af54544f4c5a7dadebbd3b23bd77700830f2f60fbea7ae3f2f306e640010b0
'http://archive.ubuntu.com/ubuntu/pool/main/c/curl/curl_7.68.0-1ubuntu2.2.debian.tar.xz' curl_7.68.0-1ubuntu2.2.debian.tar.xz 34624 SHA512:8b6b58e88fc54cdc1fe77ab689d82df5164a1509424ff2813eba51018ad237cd2740c6f2a27b487f959371c9cb9bd2374d21aeea2cb145f226297e731d918a00
```

### `dpkg` source package: `cyrus-sasl2=2.1.27+dfsg-2`

Binary Packages:

- `libsasl2-2:amd64=2.1.27+dfsg-2`
- `libsasl2-modules-db:amd64=2.1.27+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/libsasl2-2/copyright`, `/usr/share/doc/libsasl2-modules-db/copyright`)

- `BSD-4-clause`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris cyrus-sasl2=2.1.27+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.dsc' cyrus-sasl2_2.1.27+dfsg-2.dsc 3393 SHA256:e7e09491a1c2589c9947164db091d0f9b21b7d122f128841b6eac1adfc51b6c2
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg.orig.tar.xz' cyrus-sasl2_2.1.27+dfsg.orig.tar.xz 2058596 SHA256:108b0c691c423837264f05abb559ea76c3dfdd91246555e8abe87c129a6e37cd
'http://archive.ubuntu.com/ubuntu/pool/main/c/cyrus-sasl2/cyrus-sasl2_2.1.27+dfsg-2.debian.tar.xz' cyrus-sasl2_2.1.27+dfsg-2.debian.tar.xz 99956 SHA256:ee894aeee645e842e39b434d5130e1bd15ea24b84c8eeeea3f5077511a87341a
```

### `dpkg` source package: `dash=0.5.10.2-6`

Binary Packages:

- `dash=0.5.10.2-6`

Licenses: (parsed from: `/usr/share/doc/dash/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris dash=0.5.10.2-6
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2-6.dsc' dash_0.5.10.2-6.dsc 1756 SHA256:d509a23ebdc4f107c911914590c1400e5a24383f35c5d6904e48d2afeff168ac
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2.orig.tar.gz' dash_0.5.10.2.orig.tar.gz 225196 SHA256:3c663919dc5c66ec991da14c7cf7e0be8ad00f3db73986a987c118862b5f6071
'http://archive.ubuntu.com/ubuntu/pool/main/d/dash/dash_0.5.10.2-6.debian.tar.xz' dash_0.5.10.2-6.debian.tar.xz 44232 SHA256:1448fbfc2541be52787da81ce03bb81ad6b1f380cba1b7e747abefdcd44f6c86
```

### `dpkg` source package: `db5.3=5.3.28+dfsg1-0.6ubuntu2`

Binary Packages:

- `libdb5.3:amd64=5.3.28+dfsg1-0.6ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris db5.3=5.3.28+dfsg1-0.6ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu2.dsc' db5.3_5.3.28+dfsg1-0.6ubuntu2.dsc 3245 SHA256:d879f4921a2f573132031d9371f0eb020005bdce48d6e12b436bf3515dda8663
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1.orig.tar.xz' db5.3_5.3.28+dfsg1.orig.tar.xz 19723860 SHA256:b19bf3dd8ce74b95a7b215be9a7c8489e8e8f18da60d64d6340a06e75f497749
'http://archive.ubuntu.com/ubuntu/pool/main/d/db5.3/db5.3_5.3.28+dfsg1-0.6ubuntu2.debian.tar.xz' db5.3_5.3.28+dfsg1-0.6ubuntu2.debian.tar.xz 30172 SHA256:e606e7827f077efc92afc6f0d43c921fab4577d619eab06fab23182aefab7506
```

### `dpkg` source package: `debconf=1.5.73`

Binary Packages:

- `debconf=1.5.73`

Licenses: (parsed from: `/usr/share/doc/debconf/copyright`)

- `BSD-2-clause`

Source:

```console
$ apt-get source -qq --print-uris debconf=1.5.73
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.73.dsc' debconf_1.5.73.dsc 2081 SHA256:cdd4c049414cd167a4a9479d883e205bf5cebb19fc4bb6f132000a56291eb670
'http://archive.ubuntu.com/ubuntu/pool/main/d/debconf/debconf_1.5.73.tar.xz' debconf_1.5.73.tar.xz 570780 SHA256:513895b2b77d9fb72542152390e7d4c67fe1e08de75fdad44d54ce1e7d83ecef
```

### `dpkg` source package: `debianutils=4.9.1`

Binary Packages:

- `debianutils=4.9.1`

Licenses: (parsed from: `/usr/share/doc/debianutils/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris debianutils=4.9.1
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.9.1.dsc' debianutils_4.9.1.dsc 1592 SHA256:d30866ea0352263fa7756010e8743ade350024b2fd491bc5befcbaa9a97626b7
'http://archive.ubuntu.com/ubuntu/pool/main/d/debianutils/debianutils_4.9.1.tar.xz' debianutils_4.9.1.tar.xz 157516 SHA256:af826685d9c56abfa873e84cd392539cd363cb0ba04a09d21187377e1b764091
```

### `dpkg` source package: `defusedxml=0.6.0-2`

Binary Packages:

- `python3-defusedxml=0.6.0-2`

Licenses: (parsed from: `/usr/share/doc/python3-defusedxml/copyright`)

- `Python`

Source:

```console
$ apt-get source -qq --print-uris defusedxml=0.6.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/d/defusedxml/defusedxml_0.6.0-2.dsc' defusedxml_0.6.0-2.dsc 2099 SHA256:ebc06e9f6417a6d72c51fcaa54aba7f038e28ab09610a7fc06da79c6ae8d9ecb
'http://archive.ubuntu.com/ubuntu/pool/main/d/defusedxml/defusedxml_0.6.0.orig.tar.gz' defusedxml_0.6.0.orig.tar.gz 62670 SHA256:f684034d135af4c6cbb949b8a4d2ed61634515257a67299e5f940fbaa34377f5
'http://archive.ubuntu.com/ubuntu/pool/main/d/defusedxml/defusedxml_0.6.0-2.debian.tar.xz' defusedxml_0.6.0-2.debian.tar.xz 8704 SHA256:b495ec628d01bc4fa502e60635786dfbf0a3103d9725db968337442f58a8718f
```

### `dpkg` source package: `diffutils=1:3.7-3`

Binary Packages:

- `diffutils=1:3.7-3`

Licenses: (parsed from: `/usr/share/doc/diffutils/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris diffutils=1:3.7-3
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7-3.dsc' diffutils_3.7-3.dsc 1453 SHA256:99dee94cec05454a65a9cb542bea1720dbd4c511d13f9784c9e3741e76a9b9ba
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7.orig.tar.xz' diffutils_3.7.orig.tar.xz 1448828 SHA256:b3a7a6221c3dc916085f0d205abf6b8e1ba443d4dd965118da364a1dc1cb3a26
'http://archive.ubuntu.com/ubuntu/pool/main/d/diffutils/diffutils_3.7-3.debian.tar.xz' diffutils_3.7-3.debian.tar.xz 11116 SHA256:a455228f12283b5f3c0165db4ab9b12071adc37fb9dd50dcb5e1b8851c524f1f
```

### `dpkg` source package: `distro-info-data=0.43ubuntu1.1`

Binary Packages:

- `distro-info-data=0.43ubuntu1.1`

Licenses: (parsed from: `/usr/share/doc/distro-info-data/copyright`)

- `ISC`

Source:

```console
$ apt-get source -qq --print-uris distro-info-data=0.43ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/d/distro-info-data/distro-info-data_0.43ubuntu1.1.dsc' distro-info-data_0.43ubuntu1.1.dsc 1738 SHA512:dd21380a71829f4dff4095dd2342054217bc19f5a77b672b8b9592268e047aebc9090a21e6c04c7f18d1b3481ab983f88217b56dadcc63929452431bafae192e
'http://archive.ubuntu.com/ubuntu/pool/main/d/distro-info-data/distro-info-data_0.43ubuntu1.1.tar.xz' distro-info-data_0.43ubuntu1.1.tar.xz 7476 SHA512:f317a6be32a4418b81c68d1c5c6b7c6408892a41a3808732c5f69da0e1050abdc6cac9c25d1badee6ba14944f820e0c703f63a9a4e05473c5b862f31376b8ba9
```

### `dpkg` source package: `dpkg=1.19.7ubuntu3`

Binary Packages:

- `dpkg=1.19.7ubuntu3`
- `dpkg-dev=1.19.7ubuntu3`
- `libdpkg-perl=1.19.7ubuntu3`

Licenses: (parsed from: `/usr/share/doc/dpkg/copyright`, `/usr/share/doc/dpkg-dev/copyright`, `/usr/share/doc/libdpkg-perl/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`
- `public-domain-md5`
- `public-domain-s-s-d`

Source:

```console
$ apt-get source -qq --print-uris dpkg=1.19.7ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.7ubuntu3.dsc' dpkg_1.19.7ubuntu3.dsc 2254 SHA256:462ecb9f8af5612f7fbc1181484d8376569f95bb0dc7b7c53891819a0434e81a
'http://archive.ubuntu.com/ubuntu/pool/main/d/dpkg/dpkg_1.19.7ubuntu3.tar.xz' dpkg_1.19.7ubuntu3.tar.xz 4731220 SHA256:598eba200da2e1b6097f11537c49e9ad7eb2292e148259bd76f9cd184f281853
```

### `dpkg` source package: `e2fsprogs=1.45.5-2ubuntu1`

Binary Packages:

- `e2fsprogs=1.45.5-2ubuntu1`
- `libcom-err2:amd64=1.45.5-2ubuntu1`
- `libext2fs2:amd64=1.45.5-2ubuntu1`
- `libss2:amd64=1.45.5-2ubuntu1`
- `logsave=1.45.5-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/e2fsprogs/copyright`, `/usr/share/doc/libcom-err2/copyright`, `/usr/share/doc/libext2fs2/copyright`, `/usr/share/doc/libss2/copyright`, `/usr/share/doc/logsave/copyright`)

- `GPL-2`
- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris e2fsprogs=1.45.5-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.5-2ubuntu1.dsc' e2fsprogs_1.45.5-2ubuntu1.dsc 3342 SHA256:a4d9f6948bd041523783a727854beff6b8c3786f96f70936e1d63b6cd9596b01
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.5.orig.tar.gz' e2fsprogs_1.45.5.orig.tar.gz 7938826 SHA256:91e72a2f6fee21b89624d8ece5a4b3751a17b28775d32cd048921050b4760ed9
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.5.orig.tar.gz.asc' e2fsprogs_1.45.5.orig.tar.gz.asc 488 SHA256:0f900698a89e3e1996cd86966e5ae0dc6f8d866e2cd8a0f4285c23e7ea696720
'http://archive.ubuntu.com/ubuntu/pool/main/e/e2fsprogs/e2fsprogs_1.45.5-2ubuntu1.debian.tar.xz' e2fsprogs_1.45.5-2ubuntu1.debian.tar.xz 81528 SHA256:bcf259dd0480b50996580a765fded85f89a0a6041f6c81cbbcce94f58944c51b
```

### `dpkg` source package: `empy=3.3.2-5.1`

Binary Packages:

- `python3-empy=3.3.2-5.1`

Licenses: (parsed from: `/usr/share/doc/python3-empy/copyright`)

- `GPL-2`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris empy=3.3.2-5.1
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.2-5.1.dsc' empy_3.3.2-5.1.dsc 2029 SHA256:529b5cbe61f295b7319e6f5209ac43447f505712c8a5956c9e3fe8c38a4f5de1
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.2.orig.tar.gz' empy_3.3.2.orig.tar.gz 138168 SHA256:99f016af2770c48ab57a65df7aae251360dc69a1514c15851458a71d4ddfea9c
'http://archive.ubuntu.com/ubuntu/pool/universe/e/empy/empy_3.3.2-5.1.debian.tar.xz' empy_3.3.2-5.1.debian.tar.xz 6896 SHA256:aa7d17e4f817d11418ca8669d5b366760853321701a14f5b686770a99cd192e8
```

### `dpkg` source package: `expat=2.2.9-1build1`

Binary Packages:

- `libexpat1:amd64=2.2.9-1build1`
- `libexpat1-dev:amd64=2.2.9-1build1`

Licenses: (parsed from: `/usr/share/doc/libexpat1/copyright`, `/usr/share/doc/libexpat1-dev/copyright`)

- `MIT`

Source:

```console
$ apt-get source -qq --print-uris expat=2.2.9-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1build1.dsc' expat_2.2.9-1build1.dsc 1998 SHA256:9f2d2e3bf2aec22907e3bf818fac7acc5f1e917821907bdea016f69a5cfe4da0
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9.orig.tar.gz' expat_2.2.9.orig.tar.gz 8273174 SHA256:c341ac8c79e021cc3392a6d76e138e62d1dd287592cb455148540331756a2208
'http://archive.ubuntu.com/ubuntu/pool/main/e/expat/expat_2.2.9-1build1.debian.tar.xz' expat_2.2.9-1build1.debian.tar.xz 10780 SHA256:400872937adfb41255914391a172237cfe317e57f129562ff2ec66773b2b5bbf
```

### `dpkg` source package: `findutils=4.7.0-1ubuntu1`

Binary Packages:

- `findutils=4.7.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/findutils/copyright`)

- `GFDL-1.3`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris findutils=4.7.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0-1ubuntu1.dsc' findutils_4.7.0-1ubuntu1.dsc 2446 SHA256:3d157948919082e66cb74e0f927efa3dd240d9fa9814973874d0fa77f3023ead
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz' findutils_4.7.0.orig.tar.xz 1895048 SHA256:c5fefbdf9858f7e4feb86f036e1247a54c79fc2d8e4b7064d5aaa1f47dfa789a
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0.orig.tar.xz.asc' findutils_4.7.0.orig.tar.xz.asc 488 SHA256:2f620e6d941e241fac52344a89149ab1ffeefb0fb9e42174e17a508d59a31d0f
'http://archive.ubuntu.com/ubuntu/pool/main/f/findutils/findutils_4.7.0-1ubuntu1.debian.tar.xz' findutils_4.7.0-1ubuntu1.debian.tar.xz 27700 SHA256:dfb2329fd141384c2d76409c2e99f164cc25954115529245d80d5d41e3167731
```

### `dpkg` source package: `gcc-10=10-20200411-0ubuntu1`

Binary Packages:

- `gcc-10-base:amd64=10-20200411-0ubuntu1`
- `libatomic1:amd64=10-20200411-0ubuntu1`
- `libcc1-0:amd64=10-20200411-0ubuntu1`
- `libgcc-s1:amd64=10-20200411-0ubuntu1`
- `libgfortran5:amd64=10-20200411-0ubuntu1`
- `libgomp1:amd64=10-20200411-0ubuntu1`
- `libitm1:amd64=10-20200411-0ubuntu1`
- `liblsan0:amd64=10-20200411-0ubuntu1`
- `libquadmath0:amd64=10-20200411-0ubuntu1`
- `libstdc++6:amd64=10-20200411-0ubuntu1`
- `libtsan0:amd64=10-20200411-0ubuntu1`
- `libubsan1:amd64=10-20200411-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/gcc-10-base/copyright`, `/usr/share/doc/libatomic1/copyright`, `/usr/share/doc/libcc1-0/copyright`, `/usr/share/doc/libgcc-s1/copyright`, `/usr/share/doc/libgfortran5/copyright`, `/usr/share/doc/libgomp1/copyright`, `/usr/share/doc/libitm1/copyright`, `/usr/share/doc/liblsan0/copyright`, `/usr/share/doc/libquadmath0/copyright`, `/usr/share/doc/libstdc++6/copyright`, `/usr/share/doc/libtsan0/copyright`, `/usr/share/doc/libubsan1/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-10=10-20200411-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-10/gcc-10_10-20200411-0ubuntu1.dsc' gcc-10_10-20200411-0ubuntu1.dsc 31097 SHA256:31e14253df2c6e84c158969c6832777a6d249a15af3e8887f96f7adcccb72217
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-10/gcc-10_10-20200411.orig.tar.gz' gcc-10_10-20200411.orig.tar.gz 90370841 SHA256:3370dce39f863735c44f1c5f002132a84d1c7de621d4ca81a24d6613034201a8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-10/gcc-10_10-20200411-0ubuntu1.debian.tar.xz' gcc-10_10-20200411-0ubuntu1.debian.tar.xz 557752 SHA256:b028f2e1e8f430f4c451222fba1caed9aea78e58c6b87970bd2dd119c29ac0fb
```

### `dpkg` source package: `gcc-7=7.5.0-6ubuntu2`

Binary Packages:

- `gcc-7-base:amd64=7.5.0-6ubuntu2`
- `libasan4:amd64=7.5.0-6ubuntu2`
- `libcilkrts5:amd64=7.5.0-6ubuntu2`
- `libgcc-7-dev:amd64=7.5.0-6ubuntu2`
- `libstdc++-7-dev:amd64=7.5.0-6ubuntu2`
- `libubsan0:amd64=7.5.0-6ubuntu2`

Licenses: (parsed from: `/usr/share/doc/gcc-7-base/copyright`, `/usr/share/doc/libasan4/copyright`, `/usr/share/doc/libcilkrts5/copyright`, `/usr/share/doc/libgcc-7-dev/copyright`, `/usr/share/doc/libstdc++-7-dev/copyright`, `/usr/share/doc/libubsan0/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-7=7.5.0-6ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gcc-7/gcc-7_7.5.0-6ubuntu2.dsc' gcc-7_7.5.0-6ubuntu2.dsc 23582 SHA256:9731b5f821081d7631af930323461759b9dbfe4a205b1c71af85fadd32cb4ef7
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gcc-7/gcc-7_7.5.0.orig.tar.gz' gcc-7_7.5.0.orig.tar.gz 73877115 SHA256:dd7f095be2cd6aa61bd914b5b8e78daccae741a816cf19357cd767bef24ec390
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gcc-7/gcc-7_7.5.0-6ubuntu2.diff.gz' gcc-7_7.5.0-6ubuntu2.diff.gz 574048 SHA256:4e223d4c81b95324adc14c7583c44de9c8bcf8358ade78851409b7dcf5e94678
```

### `dpkg` source package: `gcc-8=8.4.0-3ubuntu2`

Binary Packages:

- `cpp-8=8.4.0-3ubuntu2`
- `gcc-8=8.4.0-3ubuntu2`
- `gcc-8-base:amd64=8.4.0-3ubuntu2`
- `gfortran-8=8.4.0-3ubuntu2`
- `libgcc-8-dev:amd64=8.4.0-3ubuntu2`
- `libgfortran-8-dev:amd64=8.4.0-3ubuntu2`
- `libmpx2:amd64=8.4.0-3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/cpp-8/copyright`, `/usr/share/doc/gcc-8/copyright`, `/usr/share/doc/gcc-8-base/copyright`, `/usr/share/doc/gfortran-8/copyright`, `/usr/share/doc/libgcc-8-dev/copyright`, `/usr/share/doc/libgfortran-8-dev/copyright`, `/usr/share/doc/libmpx2/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-8=8.4.0-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gcc-8/gcc-8_8.4.0-3ubuntu2.dsc' gcc-8_8.4.0-3ubuntu2.dsc 21085 SHA256:8454ed1772ce33dfec1077cec9d0d3d8f9164bc463ff4ee0b41b590a18ddc6c8
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gcc-8/gcc-8_8.4.0.orig.tar.gz' gcc-8_8.4.0.orig.tar.gz 85278215 SHA256:eb917ceb079e90afe1e524dee295e2360c63b923c611ae231144385be37dde2a
'http://archive.ubuntu.com/ubuntu/pool/universe/g/gcc-8/gcc-8_8.4.0-3ubuntu2.diff.gz' gcc-8_8.4.0-3ubuntu2.diff.gz 518253 SHA256:650ab9597f51ba86a089161816454f61596a3a45e270e010d739c5a7d7d9c1d5
```

### `dpkg` source package: `gcc-9=9.3.0-10ubuntu2`

Binary Packages:

- `cpp-9=9.3.0-10ubuntu2`
- `g++-9=9.3.0-10ubuntu2`
- `gcc-9=9.3.0-10ubuntu2`
- `gcc-9-base:amd64=9.3.0-10ubuntu2`
- `libasan5:amd64=9.3.0-10ubuntu2`
- `libgcc-9-dev:amd64=9.3.0-10ubuntu2`
- `libstdc++-9-dev:amd64=9.3.0-10ubuntu2`

Licenses: (parsed from: `/usr/share/doc/cpp-9/copyright`, `/usr/share/doc/g++-9/copyright`, `/usr/share/doc/gcc-9/copyright`, `/usr/share/doc/gcc-9-base/copyright`, `/usr/share/doc/libasan5/copyright`, `/usr/share/doc/libgcc-9-dev/copyright`, `/usr/share/doc/libstdc++-9-dev/copyright`)

- `Artistic`
- `GFDL-1.2`
- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris gcc-9=9.3.0-10ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-9/gcc-9_9.3.0-10ubuntu2.dsc' gcc-9_9.3.0-10ubuntu2.dsc 24227 SHA256:1d22f7b0eb0d5d57faf213e9b19730486e6ce613afdcda5e233e67da193ed065
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-9/gcc-9_9.3.0.orig.tar.gz' gcc-9_9.3.0.orig.tar.gz 90490748 SHA256:e12a3369d34f49dd18f341dc3d101cc643129663a7b44312fddba595374e718f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-9/gcc-9_9.3.0-10ubuntu2.debian.tar.xz' gcc-9_9.3.0-10ubuntu2.debian.tar.xz 621440 SHA256:ea0575c3553d6b6767a1454f80d3752ddf2f217f96b9b416fa38fdcdffe1ffe3
```

### `dpkg` source package: `gcc-defaults=1.185.1ubuntu2`

Binary Packages:

- `cpp=4:9.3.0-1ubuntu2`
- `g++=4:9.3.0-1ubuntu2`
- `gcc=4:9.3.0-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/cpp/copyright`, `/usr/share/doc/g++/copyright`, `/usr/share/doc/gcc/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gcc-defaults=1.185.1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.185.1ubuntu2.dsc' gcc-defaults_1.185.1ubuntu2.dsc 16544 SHA256:32c0331bc75ecbc0d013b9e11401d1fc64cbd7b0198274cb25a183a27b5c407f
'http://archive.ubuntu.com/ubuntu/pool/main/g/gcc-defaults/gcc-defaults_1.185.1ubuntu2.tar.gz' gcc-defaults_1.185.1ubuntu2.tar.gz 58807 SHA256:342b5842c03073717bc98d6d9de7eb79027a1239735637743006933e5d44bb05
```

### `dpkg` source package: `gdbm=1.18.1-5`

Binary Packages:

- `libgdbm-compat4:amd64=1.18.1-5`
- `libgdbm6:amd64=1.18.1-5`

Licenses: (parsed from: `/usr/share/doc/libgdbm-compat4/copyright`, `/usr/share/doc/libgdbm6/copyright`)

- `GFDL-NIV-1.3+`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gdbm=1.18.1-5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1-5.dsc' gdbm_1.18.1-5.dsc 2635 SHA256:4c0c4498378c673c9d2d8dfb5b319a4830d2dd21e65faaaa8e0f09cb7f71606b
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz' gdbm_1.18.1.orig.tar.gz 941863 SHA256:86e613527e5dba544e73208f42b78b7c022d4fa5a6d5498bf18c8d6f745b91dc
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1.orig.tar.gz.asc' gdbm_1.18.1.orig.tar.gz.asc 412 SHA256:3254738e7689e44ac65e78a766806828b8282e6bb1c0e5bb6156a99e567889a5
'http://archive.ubuntu.com/ubuntu/pool/main/g/gdbm/gdbm_1.18.1-5.debian.tar.xz' gdbm_1.18.1-5.debian.tar.xz 16348 SHA256:3c1a0e05b40a97ee51ce77c736c72c37738ba31b2720111d3bc99175a2c3a3ed
```

### `dpkg` source package: `glib2.0=2.64.3-1~ubuntu20.04.1`

Binary Packages:

- `libglib2.0-0:amd64=2.64.3-1~ubuntu20.04.1`

Licenses: (parsed from: `/usr/share/doc/libglib2.0-0/copyright`)

- `Expat`
- `GPL-2+`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris glib2.0=2.64.3-1~ubuntu20.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.64.3-1~ubuntu20.04.1.dsc' glib2.0_2.64.3-1~ubuntu20.04.1.dsc 3256 SHA512:37318872e0a19da2664a945436647bbab52947e5eff00630cdd85828689bdabbac59ee06448698fa0f2ab5fd8270521167c0bf83557fee82bef80c6a3efe85ff
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.64.3.orig.tar.xz' glib2.0_2.64.3.orig.tar.xz 4778964 SHA512:a3828c37a50e86eb8791be53bd8af848d144e4580841ffab28f3b6eae5144f5cdf4a5d4b43130615b97488e700b274c2468fc7d561b3701a1fc686349501a1db
'http://archive.ubuntu.com/ubuntu/pool/main/g/glib2.0/glib2.0_2.64.3-1~ubuntu20.04.1.debian.tar.xz' glib2.0_2.64.3-1~ubuntu20.04.1.debian.tar.xz 91792 SHA512:b9cbb32bfb50e7136a0135b35770a16ba2b6366d5fc55c2bc9d3c3e7d69aafdb8debf5a7f679cc8fafdb0c278703f772855742bad702deceb847e04d4bb0a902
```

### `dpkg` source package: `glibc=2.31-0ubuntu9.1`

Binary Packages:

- `libc-bin=2.31-0ubuntu9.1`
- `libc-dev-bin=2.31-0ubuntu9.1`
- `libc6:amd64=2.31-0ubuntu9.1`
- `libc6-dev:amd64=2.31-0ubuntu9.1`

Licenses: (parsed from: `/usr/share/doc/libc-bin/copyright`, `/usr/share/doc/libc-dev-bin/copyright`, `/usr/share/doc/libc6/copyright`, `/usr/share/doc/libc6-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris glibc=2.31-0ubuntu9.1
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31-0ubuntu9.1.dsc' glibc_2.31-0ubuntu9.1.dsc 9456 SHA512:b3f10b8c8f421431c91f14efbc92fc165675d5cdb427629e67d5e19927de0f4024c736c9da1c5d4b7e2bd0aa01395b3e269aeccee161918311f2ea1c75815f1f
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31.orig.tar.xz' glibc_2.31.orig.tar.xz 17317924 SHA512:2ff56628fe935cacbdf1825534f15d45cb87a159cbdb2e6a981590eeb6174ed4b3ff7041519cdecbd4f624ac20b745e2dd9614c420dd3ea186b8f36bc4c2453c
'http://archive.ubuntu.com/ubuntu/pool/main/g/glibc/glibc_2.31-0ubuntu9.1.debian.tar.xz' glibc_2.31-0ubuntu9.1.debian.tar.xz 844816 SHA512:bca1857b031eda2d170256b97829c6b8a38493c66858a041e6f0143bf26c376c207e72d499ef1be07a83667419d55284407bae518511a702171eac58c6f31d62
```

### `dpkg` source package: `gmp=2:6.2.0+dfsg-4`

Binary Packages:

- `libgmp10:amd64=2:6.2.0+dfsg-4`

Licenses: (parsed from: `/usr/share/doc/libgmp10/copyright`)

- `GPL`
- `GPL-2`
- `GPL-3`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris gmp=2:6.2.0+dfsg-4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg-4.dsc' gmp_6.2.0+dfsg-4.dsc 2144 SHA256:4ca8c5bca982c78eb7679256a5d41b2c9363a6c3e3ee15ed765515bc328e9989
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg.orig.tar.xz' gmp_6.2.0+dfsg.orig.tar.xz 1842912 SHA256:5d7610449498a79aa62d4b9a8f6baaef91b8716726e1009e02b879962dff32ab
'http://archive.ubuntu.com/ubuntu/pool/main/g/gmp/gmp_6.2.0+dfsg-4.debian.tar.xz' gmp_6.2.0+dfsg-4.debian.tar.xz 21120 SHA256:a0772595583dbcf2147e8457602ccf4b524b18227d6804c4a74050df64ece912
```

### `dpkg` source package: `gnupg2=2.2.19-3ubuntu2`

Binary Packages:

- `dirmngr=2.2.19-3ubuntu2`
- `gnupg=2.2.19-3ubuntu2`
- `gnupg-l10n=2.2.19-3ubuntu2`
- `gnupg-utils=2.2.19-3ubuntu2`
- `gnupg2=2.2.19-3ubuntu2`
- `gpg=2.2.19-3ubuntu2`
- `gpg-agent=2.2.19-3ubuntu2`
- `gpg-wks-client=2.2.19-3ubuntu2`
- `gpg-wks-server=2.2.19-3ubuntu2`
- `gpgconf=2.2.19-3ubuntu2`
- `gpgsm=2.2.19-3ubuntu2`
- `gpgv=2.2.19-3ubuntu2`

Licenses: (parsed from: `/usr/share/doc/dirmngr/copyright`, `/usr/share/doc/gnupg/copyright`, `/usr/share/doc/gnupg-l10n/copyright`, `/usr/share/doc/gnupg-utils/copyright`, `/usr/share/doc/gnupg2/copyright`, `/usr/share/doc/gpg/copyright`, `/usr/share/doc/gpg-agent/copyright`, `/usr/share/doc/gpg-wks-client/copyright`, `/usr/share/doc/gpg-wks-server/copyright`, `/usr/share/doc/gpgconf/copyright`, `/usr/share/doc/gpgsm/copyright`, `/usr/share/doc/gpgv/copyright`)

- `BSD-3-clause`
- `CC0-1.0`
- `Expat`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `RFC-Reference`
- `TinySCHEME`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris gnupg2=2.2.19-3ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.19-3ubuntu2.dsc' gnupg2_2.2.19-3ubuntu2.dsc 3968 SHA256:f33406a797da145bfbb64a1e0bc42d904350b716408fc6c4d31ac3f7804c0244
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.19.orig.tar.bz2' gnupg2_2.2.19.orig.tar.bz2 6754972 SHA256:242554c0e06f3a83c420b052f750b65ead711cc3fddddb5e7274fcdbb4e9dec0
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.19.orig.tar.bz2.asc' gnupg2_2.2.19.orig.tar.bz2.asc 906 SHA256:9665fd179a29412115289bd18109629b855bf78adb6d262cfd4fb00ea09491d7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnupg2/gnupg2_2.2.19-3ubuntu2.debian.tar.xz' gnupg2_2.2.19-3ubuntu2.debian.tar.xz 65068 SHA256:fd2dc1a844dbce1b989e8c6f7d8199c950bd3c35c8aefa553dcc27f9cb977ac6
```

### `dpkg` source package: `gnutls28=3.6.13-2ubuntu1.3`

Binary Packages:

- `libgnutls30:amd64=3.6.13-2ubuntu1.3`

Licenses: (parsed from: `/usr/share/doc/libgnutls30/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`
- `CC0 license`
- `Expat`
- `GFDL-1.3`
- `GPL`
- `GPL-3`
- `GPLv3+`
- `LGPL`
- `LGPL-3`
- `LGPLv2.1+`
- `LGPLv3+_or_GPLv2+`
- `The main library is licensed under GNU Lesser`

Source:

```console
$ apt-get source -qq --print-uris gnutls28=3.6.13-2ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13-2ubuntu1.3.dsc' gnutls28_3.6.13-2ubuntu1.3.dsc 3594 SHA512:9a773f3bdf9048448a0ba8fbd9ab3d2883621df20f7bc62f7e298331d32be9c361ce4e9c3cfb702be543cb15c6743ada1a70dc28533beb736305a8e9f0d514c8
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13.orig.tar.xz' gnutls28_3.6.13.orig.tar.xz 5958956 SHA512:23581952cb72c9a34f378c002bb62413d5a1243b74b48ad8dc49eaea4020d33c550f8dc1dd374cf7fbfa4187b0ca1c5698c8a0430398268a8b8a863f8633305c
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13.orig.tar.xz.asc' gnutls28_3.6.13.orig.tar.xz.asc 667 SHA512:b343a8ace6a5c81c0c44b2cb65d8e83dfe5963c9bab04d9131fa8fd03cdf0c6f990d720af8767084e01bf5f7a7dbd0f048aefe68c3b6f1dc1ea1899d567a72f7
'http://archive.ubuntu.com/ubuntu/pool/main/g/gnutls28/gnutls28_3.6.13-2ubuntu1.3.debian.tar.xz' gnutls28_3.6.13-2ubuntu1.3.debian.tar.xz 64836 SHA512:b28fe3c01879a57fe15e39dd8bd23b236c0b7b2addfec1fbc2808034ea6e4d3feb0c365c46f7872fb604feb082116be6313fce008d7c3f4c4574e235404c6f1c
```

### `dpkg` source package: `googletest=1.10.0-2`

Binary Packages:

- `google-mock:amd64=1.10.0-2`
- `googletest=1.10.0-2`
- `libgtest-dev:amd64=1.10.0-2`

Licenses: (parsed from: `/usr/share/doc/google-mock/copyright`, `/usr/share/doc/googletest/copyright`, `/usr/share/doc/libgtest-dev/copyright`)

- `Apache`
- `BSD-C3`
- `GAP`

Source:

```console
$ apt-get source -qq --print-uris googletest=1.10.0-2
'http://archive.ubuntu.com/ubuntu/pool/universe/g/googletest/googletest_1.10.0-2.dsc' googletest_1.10.0-2.dsc 2195 SHA256:c7b1a205d6f704d54e8fb34b680a6c4e7f71f91af0ee8b29fa05adcec5c569d1
'http://archive.ubuntu.com/ubuntu/pool/universe/g/googletest/googletest_1.10.0.orig.tar.bz2' googletest_1.10.0.orig.tar.bz2 702821 SHA256:369d5e65753f0e86ed96dac25088488ff852332cbf1be1db58d062eecc4c32bf
'http://archive.ubuntu.com/ubuntu/pool/universe/g/googletest/googletest_1.10.0-2.debian.tar.xz' googletest_1.10.0-2.debian.tar.xz 10468 SHA256:af49f7e0195db575ca6bd907c09e2e85b78685dd3374e00bda53624f436bddb1
```

### `dpkg` source package: `gpgme1.0=1.13.1-7ubuntu2`

Binary Packages:

- `libgpgme-dev=1.13.1-7ubuntu2`
- `libgpgme11:amd64=1.13.1-7ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libgpgme-dev/copyright`, `/usr/share/doc/libgpgme11/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris gpgme1.0=1.13.1-7ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.13.1-7ubuntu2.dsc' gpgme1.0_1.13.1-7ubuntu2.dsc 2915 SHA256:cd281e669d7c382bb02ad86d432b24784c463fb6c8db15e7fd2099dce579325d
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.13.1.orig.tar.bz2' gpgme1.0_1.13.1.orig.tar.bz2 1759616 SHA256:c4e30b227682374c23cddc7fdb9324a99694d907e79242a25a4deeedb393be46
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.13.1.orig.tar.bz2.asc' gpgme1.0_1.13.1.orig.tar.bz2.asc 488 SHA256:2759362727500bc9ddee86c6383b63bee0e230bd6159e63ea3cb48dc1de0f303
'http://archive.ubuntu.com/ubuntu/pool/main/g/gpgme1.0/gpgme1.0_1.13.1-7ubuntu2.debian.tar.xz' gpgme1.0_1.13.1-7ubuntu2.debian.tar.xz 22236 SHA256:211f22649de0ab4099aae46bcadf7d29546c576fda23e9fb01daaa8548050d8f
```

### `dpkg` source package: `grep=3.4-1`

Binary Packages:

- `grep=3.4-1`

Licenses: (parsed from: `/usr/share/doc/grep/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris grep=3.4-1
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4-1.dsc' grep_3.4-1.dsc 1674 SHA256:785f527cede9631f075bdd6c7f35e65e6b82897d009682766cf35839a393277d
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4.orig.tar.xz' grep_3.4.orig.tar.xz 1555820 SHA256:58e6751c41a7c25bfc6e9363a41786cff3ba5709cf11d5ad903cf7cce31cc3fb
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4.orig.tar.xz.asc' grep_3.4.orig.tar.xz.asc 833 SHA256:4c1871ff6b79c5e5ce0a192272c171d06ec20762b4b258688b1ca2e47d94b23e
'http://archive.ubuntu.com/ubuntu/pool/main/g/grep/grep_3.4-1.debian.tar.xz' grep_3.4-1.debian.tar.xz 104364 SHA256:582d181804ce72fcfc4c6a9f13ea1dd73ad04c2723b5da346b69ee5cd24a7d08
```

### `dpkg` source package: `gzip=1.10-0ubuntu4`

Binary Packages:

- `gzip=1.10-0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/gzip/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris gzip=1.10-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-0ubuntu4.dsc' gzip_1.10-0ubuntu4.dsc 2134 SHA256:b1b05c873448fe2ae1029f55cfea8ae5139d0d88a66ed97768da911e833c9578
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10.orig.tar.gz' gzip_1.10.orig.tar.gz 1201421 SHA256:c91f74430bf7bc20402e1f657d0b252cb80aa66ba333a25704512af346633c68
'http://archive.ubuntu.com/ubuntu/pool/main/g/gzip/gzip_1.10-0ubuntu4.debian.tar.xz' gzip_1.10-0ubuntu4.debian.tar.xz 26592 SHA256:da4c6907f9769be8622349c1a5b81ba5d2ab03c82f1e116c2f3f1a9f00bb8055
```

### `dpkg` source package: `heimdal=7.7.0+dfsg-1ubuntu1`

Binary Packages:

- `libasn1-8-heimdal:amd64=7.7.0+dfsg-1ubuntu1`
- `libgssapi3-heimdal:amd64=7.7.0+dfsg-1ubuntu1`
- `libhcrypto4-heimdal:amd64=7.7.0+dfsg-1ubuntu1`
- `libheimbase1-heimdal:amd64=7.7.0+dfsg-1ubuntu1`
- `libheimntlm0-heimdal:amd64=7.7.0+dfsg-1ubuntu1`
- `libhx509-5-heimdal:amd64=7.7.0+dfsg-1ubuntu1`
- `libkrb5-26-heimdal:amd64=7.7.0+dfsg-1ubuntu1`
- `libroken18-heimdal:amd64=7.7.0+dfsg-1ubuntu1`
- `libwind0-heimdal:amd64=7.7.0+dfsg-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libasn1-8-heimdal/copyright`, `/usr/share/doc/libgssapi3-heimdal/copyright`, `/usr/share/doc/libhcrypto4-heimdal/copyright`, `/usr/share/doc/libheimbase1-heimdal/copyright`, `/usr/share/doc/libheimntlm0-heimdal/copyright`, `/usr/share/doc/libhx509-5-heimdal/copyright`, `/usr/share/doc/libkrb5-26-heimdal/copyright`, `/usr/share/doc/libroken18-heimdal/copyright`, `/usr/share/doc/libwind0-heimdal/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`
- `custom`
- `none`

Source:

```console
$ apt-get source -qq --print-uris heimdal=7.7.0+dfsg-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg-1ubuntu1.dsc' heimdal_7.7.0+dfsg-1ubuntu1.dsc 3633 SHA256:46b7873a11c8279f5efec50f16b5ed4abafa5a957224c3f624229f9d888e1ebe
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg.orig.tar.xz' heimdal_7.7.0+dfsg.orig.tar.xz 5945252 SHA256:6822c9547188b753b6325047fda9255744e4ebbbe02bb0dade78c261061fefac
'http://archive.ubuntu.com/ubuntu/pool/main/h/heimdal/heimdal_7.7.0+dfsg-1ubuntu1.debian.tar.xz' heimdal_7.7.0+dfsg-1ubuntu1.debian.tar.xz 128604 SHA256:0c0b4572de525c3c294bcdbde95ebfc3386461c47c2e8d1a86fe0d37da6bd479
```

### `dpkg` source package: `hostname=3.23`

Binary Packages:

- `hostname=3.23`

Licenses: (parsed from: `/usr/share/doc/hostname/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris hostname=3.23
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23.dsc' hostname_3.23.dsc 1402 SHA256:0694c083fad82da1fd33204557a30bfc745a689a64030ba360062daafe03ede0
'http://archive.ubuntu.com/ubuntu/pool/main/h/hostname/hostname_3.23.tar.gz' hostname_3.23.tar.gz 13672 SHA256:bc6d1954b22849869ff8b2a602e39f08b1702f686d4b58dd7927cdeb5b4876ef
```

### `dpkg` source package: `hwloc=2.1.0+dfsg-4`

Binary Packages:

- `libhwloc-dev:amd64=2.1.0+dfsg-4`
- `libhwloc-plugins:amd64=2.1.0+dfsg-4`
- `libhwloc15:amd64=2.1.0+dfsg-4`

Licenses: (parsed from: `/usr/share/doc/libhwloc-dev/copyright`, `/usr/share/doc/libhwloc-plugins/copyright`, `/usr/share/doc/libhwloc15/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris hwloc=2.1.0+dfsg-4
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hwloc/hwloc_2.1.0+dfsg-4.dsc' hwloc_2.1.0+dfsg-4.dsc 2758 SHA256:1334689b3a47dda17c203b8bc04cf4573dd80700b3b966361d1eec0ee4422c38
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hwloc/hwloc_2.1.0+dfsg.orig.tar.bz2' hwloc_2.1.0+dfsg.orig.tar.bz2 6010371 SHA256:ddaae849747431bf8bd0c8e7e0bf2e5bb0ce80f3641db8e84c460c8bb8319eb4
'http://archive.ubuntu.com/ubuntu/pool/universe/h/hwloc/hwloc_2.1.0+dfsg-4.debian.tar.xz' hwloc_2.1.0+dfsg-4.debian.tar.xz 12904 SHA256:5ce3ee7ab32628585261f8eb58840f23f55310f3e08819ed073a6b53816f9b78
```

### `dpkg` source package: `icu=66.1-2ubuntu2`

Binary Packages:

- `icu-devtools=66.1-2ubuntu2`
- `libicu-dev:amd64=66.1-2ubuntu2`
- `libicu66:amd64=66.1-2ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris icu=66.1-2ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_66.1-2ubuntu2.dsc' icu_66.1-2ubuntu2.dsc 2351 SHA256:a19b1f586160efd41dc7f9eec7babf5ce9d03b578aa59cd302f11c385e86d893
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_66.1.orig.tar.gz' icu_66.1.orig.tar.gz 24361305 SHA256:52a3f2209ab95559c1cf0a14f24338001f389615bf00e2585ef3dbc43ecf0a2e
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_66.1.orig.tar.gz.asc' icu_66.1.orig.tar.gz.asc 833 SHA256:08c81d86fb4ed07ce87434afdfdc39a4114ac494908cd4eebc734ba454a80f06
'http://archive.ubuntu.com/ubuntu/pool/main/i/icu/icu_66.1-2ubuntu2.debian.tar.xz' icu_66.1-2ubuntu2.debian.tar.xz 25500 SHA256:480775da69cad60a4dc1aa20097db1d87f5435406bafa3394394c8a546a514df
```

### `dpkg` source package: `infinipath-psm=3.3+20.604758e7-6`

Binary Packages:

- `libpsm-infinipath1=3.3+20.604758e7-6`

Licenses: (parsed from: `/usr/share/doc/libpsm-infinipath1/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris infinipath-psm=3.3+20.604758e7-6
'http://archive.ubuntu.com/ubuntu/pool/universe/i/infinipath-psm/infinipath-psm_3.3+20.604758e7-6.dsc' infinipath-psm_3.3+20.604758e7-6.dsc 2284 SHA256:6cc7c9ae03a29f8be84a2b59a8980cfeb80922b3322e8631372160efd46328b9
'http://archive.ubuntu.com/ubuntu/pool/universe/i/infinipath-psm/infinipath-psm_3.3+20.604758e7.orig.tar.xz' infinipath-psm_3.3+20.604758e7.orig.tar.xz 287112 SHA256:2fb37b3436866b7f6d7244edded875bf7ebc89e7a09a1f372ace548d0f90481d
'http://archive.ubuntu.com/ubuntu/pool/universe/i/infinipath-psm/infinipath-psm_3.3+20.604758e7-6.debian.tar.xz' infinipath-psm_3.3+20.604758e7-6.debian.tar.xz 9340 SHA256:e5464e1588270d3a0e540dcbb739434576cebb132bfbeb6d1c5301386f24e95f
```

### `dpkg` source package: `init-system-helpers=1.57`

Binary Packages:

- `init-system-helpers=1.57`

Licenses: (parsed from: `/usr/share/doc/init-system-helpers/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris init-system-helpers=1.57
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.57.dsc' init-system-helpers_1.57.dsc 1896 SHA256:88bb5af040c99f010b6d6947ff5c80ae4863ff787e0eeae91e99dcd15a10dbb8
'http://archive.ubuntu.com/ubuntu/pool/main/i/init-system-helpers/init-system-helpers_1.57.tar.xz' init-system-helpers_1.57.tar.xz 40460 SHA256:e9d83fd8756a42666fb5d19a8835813823295846659b4e58f138bb9b54e9f5dd
```

### `dpkg` source package: `isl=0.22.1-1`

Binary Packages:

- `libisl22:amd64=0.22.1-1`

Licenses: (parsed from: `/usr/share/doc/libisl22/copyright`)

- `BSD-2-clause`
- `LGPL-2`
- `LGPL-2.1+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris isl=0.22.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22.1-1.dsc' isl_0.22.1-1.dsc 1860 SHA256:9e9925317ef448cf679040edb6572a2874d497f758b613d9fc633bdafab197cb
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22.1.orig.tar.xz' isl_0.22.1.orig.tar.xz 1676948 SHA256:28658ce0f0bdb95b51fd2eb15df24211c53284f6ca2ac5e897acc3169e55b60f
'http://archive.ubuntu.com/ubuntu/pool/main/i/isl/isl_0.22.1-1.debian.tar.xz' isl_0.22.1-1.debian.tar.xz 25252 SHA256:bbeb62cfc95e51c25448e127c29fa8ac8009a6f471861de28f326bab2404a406
```

### `dpkg` source package: `keyutils=1.6-6ubuntu1`

Binary Packages:

- `libkeyutils1:amd64=1.6-6ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libkeyutils1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`

Source:

```console
$ apt-get source -qq --print-uris keyutils=1.6-6ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6-6ubuntu1.dsc' keyutils_1.6-6ubuntu1.dsc 2148 SHA256:76dfe0a0d9bb0a417d9c20c2f20b0beb9097dccd30c30a41375ef99cf0a710b6
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6.orig.tar.bz2' keyutils_1.6.orig.tar.bz2 93973 SHA256:d3aef20cec0005c0fa6b4be40079885567473185b1a57b629b030e67942c7115
'http://archive.ubuntu.com/ubuntu/pool/main/k/keyutils/keyutils_1.6-6ubuntu1.debian.tar.xz' keyutils_1.6-6ubuntu1.debian.tar.xz 13636 SHA256:a4ae24062e9d20a0e2092e4cb342b664c0211ba7efdfeb7bde5f8d209c9ad1db
```

### `dpkg` source package: `krb5=1.17-6ubuntu4`

Binary Packages:

- `libgssapi-krb5-2:amd64=1.17-6ubuntu4`
- `libk5crypto3:amd64=1.17-6ubuntu4`
- `libkrb5-3:amd64=1.17-6ubuntu4`
- `libkrb5support0:amd64=1.17-6ubuntu4`

Licenses: (parsed from: `/usr/share/doc/libgssapi-krb5-2/copyright`, `/usr/share/doc/libk5crypto3/copyright`, `/usr/share/doc/libkrb5-3/copyright`, `/usr/share/doc/libkrb5support0/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris krb5=1.17-6ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-6ubuntu4.dsc' krb5_1.17-6ubuntu4.dsc 3654 SHA256:e2e56f3faf968072ef89201a04e85cd59e003d123bd5a06e3a05f59a01c94301
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17.orig.tar.gz' krb5_1.17.orig.tar.gz 8761763 SHA256:5a6e2284a53de5702d3dc2be3b9339c963f9b5397d3fbbc53beb249380a781f5
'http://archive.ubuntu.com/ubuntu/pool/main/k/krb5/krb5_1.17-6ubuntu4.debian.tar.xz' krb5_1.17-6ubuntu4.debian.tar.xz 144560 SHA256:17d09fbe6a54de93fe2f21f1c384a55d0913862dec7ca96b2c0489266f3c16fd
```

### `dpkg` source package: `lapack=3.9.0-1build1`

Binary Packages:

- `libblas3:amd64=3.9.0-1build1`
- `liblapack3:amd64=3.9.0-1build1`

Licenses: (parsed from: `/usr/share/doc/libblas3/copyright`, `/usr/share/doc/liblapack3/copyright`)

- `BSD-3-clause`
- `BSD-3-clause-intel`

Source:

```console
$ apt-get source -qq --print-uris lapack=3.9.0-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.9.0-1build1.dsc' lapack_3.9.0-1build1.dsc 3413 SHA256:8657838da743a1f52b2cc08add3ce1f606cb8c2f6f6ef5321e1f21a927025952
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.9.0.orig.tar.gz' lapack_3.9.0.orig.tar.gz 7534567 SHA256:106087f1bb5f46afdfba7f569d0cbe23dacb9a07cd24733765a0e89dbe1ad573
'http://archive.ubuntu.com/ubuntu/pool/main/l/lapack/lapack_3.9.0-1build1.debian.tar.xz' lapack_3.9.0-1build1.debian.tar.xz 27380 SHA256:1a264e2cb403441463e8e8b6cf78dc8cf8a32dd9ba73a05767b9cac089bbb847
```

### `dpkg` source package: `libarchive=3.4.0-2ubuntu1`

Binary Packages:

- `libarchive13:amd64=3.4.0-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libarchive13/copyright`)

- `Apache-2.0`
- `BSD-1-clause-UCB`
- `BSD-124-clause-UCB`
- `BSD-2-clause`
- `BSD-3-clause-UCB`
- `BSD-4-clause-UCB`
- `Expat`
- `PD`

Source:

```console
$ apt-get source -qq --print-uris libarchive=3.4.0-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.4.0-2ubuntu1.dsc' libarchive_3.4.0-2ubuntu1.dsc 2530 SHA256:b622fcd254307c7d528102eb015a836786cd751fd0e5171cc49d46ef44883d61
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.4.0.orig.tar.gz' libarchive_3.4.0.orig.tar.gz 6908093 SHA256:8643d50ed40c759f5412a3af4e353cffbce4fdf3b5cf321cb72cacf06b2d825e
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.4.0.orig.tar.gz.asc' libarchive_3.4.0.orig.tar.gz.asc 833 SHA256:5aa9d657d9d2f2481a8dce1bab4c733cfc18657b451f6551d60f37cce4ca2f57
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libarchive/libarchive_3.4.0-2ubuntu1.debian.tar.xz' libarchive_3.4.0-2ubuntu1.debian.tar.xz 40444 SHA256:0754078b2183aee4f3cf88bdd3708f5c5ec983e0c1456643e88529be039d7e1b
```

### `dpkg` source package: `libassuan=2.5.3-7ubuntu2`

Binary Packages:

- `libassuan-dev=2.5.3-7ubuntu2`
- `libassuan0:amd64=2.5.3-7ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libassuan-dev/copyright`, `/usr/share/doc/libassuan0/copyright`)

- `GAP`
- `GAP~FSF`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with libtool exception`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libassuan=2.5.3-7ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7ubuntu2.dsc' libassuan_2.5.3-7ubuntu2.dsc 2647 SHA256:014fbd728fc1d0e954ade2a8d975539fc00d455261ca14a88d78b9e29625ee41
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2' libassuan_2.5.3.orig.tar.bz2 572348 SHA256:91bcb0403866b4e7c4bc1cc52ed4c364a9b5414b3994f718c70303f7f765e702
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3.orig.tar.bz2.asc' libassuan_2.5.3.orig.tar.bz2.asc 952 SHA256:53b16a6619a2690b4f22da645a1d0c14b5664825c87b165ca5bd0de32607888a
'http://archive.ubuntu.com/ubuntu/pool/main/liba/libassuan/libassuan_2.5.3-7ubuntu2.debian.tar.xz' libassuan_2.5.3-7ubuntu2.debian.tar.xz 13936 SHA256:586836fdfffdc58b4d47548d0f6e54593daa78098c6276a788d8b66c3616e233
```

### `dpkg` source package: `libbsd=0.10.0-1`

Binary Packages:

- `libbsd0:amd64=0.10.0-1`

Licenses: (parsed from: `/usr/share/doc/libbsd0/copyright`)

- `BSD-2-clause`
- `BSD-2-clause-NetBSD`
- `BSD-2-clause-author`
- `BSD-2-clause-verbatim`
- `BSD-3-clause`
- `BSD-3-clause-John-Birrell`
- `BSD-3-clause-Regents`
- `BSD-3-clause-author`
- `BSD-4-clause-Christopher-G-Demetriou`
- `BSD-4-clause-Niels-Provos`
- `BSD-5-clause-Peter-Wemm`
- `Beerware`
- `Expat`
- `ISC`
- `ISC-Original`
- `public-domain`
- `public-domain-Colin-Plumb`

Source:

```console
$ apt-get source -qq --print-uris libbsd=0.10.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0-1.dsc' libbsd_0.10.0-1.dsc 2197 SHA256:7c05e2c73658f64cbd4e1762b716cc7c4c1d68391191e82c7d266a351430edd6
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz' libbsd_0.10.0.orig.tar.xz 393576 SHA256:34b8adc726883d0e85b3118fa13605e179a62b31ba51f676136ecb2d0bc1a887
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0.orig.tar.xz.asc' libbsd_0.10.0.orig.tar.xz.asc 833 SHA256:4362f6d811ffc06659ac5cf777d8d01157bedfc28720b41fb485afb0a5acc0c7
'http://archive.ubuntu.com/ubuntu/pool/main/libb/libbsd/libbsd_0.10.0-1.debian.tar.xz' libbsd_0.10.0-1.debian.tar.xz 16660 SHA256:4cf37d6d5b72702b31b07384612e07173e94e081feef71fec206f86ab38f2411
```

### `dpkg` source package: `libcap-ng=0.7.9-2.1build1`

Binary Packages:

- `libcap-ng0:amd64=0.7.9-2.1build1`

Licenses: (parsed from: `/usr/share/doc/libcap-ng0/copyright`)

- `GPL-2`
- `GPL-3`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libcap-ng=0.7.9-2.1build1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.1build1.dsc' libcap-ng_0.7.9-2.1build1.dsc 2158 SHA256:6d74cf5c418659d70bce8e9a4bf6f0ef0210dbcadac15e0c4d4471c4671230a1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9.orig.tar.gz' libcap-ng_0.7.9.orig.tar.gz 449038 SHA256:4a1532bcf3731aade40936f6d6a586ed5a66ca4c7455e1338d1f6c3e09221328
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcap-ng/libcap-ng_0.7.9-2.1build1.debian.tar.xz' libcap-ng_0.7.9-2.1build1.debian.tar.xz 6256 SHA256:b73a0a36bb0c1c8144828552dedb7b3493f4a08b1c31a0f1d7046cf1682eac7d
```

### `dpkg` source package: `libcbor=0.6.0-0ubuntu1`

Binary Packages:

- `libcbor0.6:amd64=0.6.0-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libcbor0.6/copyright`)

- `Apache-2.0`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris libcbor=0.6.0-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0-0ubuntu1.dsc' libcbor_0.6.0-0ubuntu1.dsc 2115 SHA256:403caca4382a40d55caf3d88b792e45fa79a2f20746f422a3ba5cabb113444f6
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0.orig.tar.gz' libcbor_0.6.0.orig.tar.gz 262622 SHA256:ad97dfe6462a28956be38c924a5a557acf303d8454ca121e02150a5b87e03ee7
'http://archive.ubuntu.com/ubuntu/pool/main/libc/libcbor/libcbor_0.6.0-0ubuntu1.debian.tar.xz' libcbor_0.6.0-0ubuntu1.debian.tar.xz 5832 SHA256:719b8d56482b3ffc8adc05b16211d4b9bcce43ab877801801fd3927a9a8e66e1
```

### `dpkg` source package: `libedit=3.1-20191231-1`

Binary Packages:

- `libedit2:amd64=3.1-20191231-1`

Licenses: (parsed from: `/usr/share/doc/libedit2/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris libedit=3.1-20191231-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-1.dsc' libedit_3.1-20191231-1.dsc 2129 SHA256:1be31eebf9cf3b38a9e7c3c4d4b37f002e3f89df48f00dec32506cbe9337ae38
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231.orig.tar.gz' libedit_3.1-20191231.orig.tar.gz 516801 SHA256:dbb82cb7e116a5f8025d35ef5b4f7d4a3cdd0a3909a146a39112095a2d229071
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libedit/libedit_3.1-20191231-1.debian.tar.xz' libedit_3.1-20191231-1.debian.tar.xz 14168 SHA256:f815baa1932f9df5d4cdb316a85ebd3cc91441c4d83ba2c8454f342573ed0eab
```

### `dpkg` source package: `libevent=2.1.11-stable-1`

Binary Packages:

- `libevent-2.1-7:amd64=2.1.11-stable-1`
- `libevent-core-2.1-7:amd64=2.1.11-stable-1`
- `libevent-dev=2.1.11-stable-1`
- `libevent-extra-2.1-7:amd64=2.1.11-stable-1`
- `libevent-openssl-2.1-7:amd64=2.1.11-stable-1`
- `libevent-pthreads-2.1-7:amd64=2.1.11-stable-1`

Licenses: (parsed from: `/usr/share/doc/libevent-2.1-7/copyright`, `/usr/share/doc/libevent-core-2.1-7/copyright`, `/usr/share/doc/libevent-dev/copyright`, `/usr/share/doc/libevent-extra-2.1-7/copyright`, `/usr/share/doc/libevent-openssl-2.1-7/copyright`, `/usr/share/doc/libevent-pthreads-2.1-7/copyright`)

- `BSD-2-clause`
- `BSD-3-Clause~Kitware`
- `BSD-3-clause`
- `BSL`
- `Expat`
- `FSFUL`
- `FSFULLR`
- `FSFULLR-No-Warranty`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `ISC`
- `curl`

Source:

```console
$ apt-get source -qq --print-uris libevent=2.1.11-stable-1
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.11-stable-1.dsc' libevent_2.1.11-stable-1.dsc 2526 SHA256:b07a15f54f2ab403eed9aa648a1ea9bee05a5a5362570d334a76597e79a1d795
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.11-stable.orig.tar.gz' libevent_2.1.11-stable.orig.tar.gz 1082234 SHA256:a65bac6202ea8c5609fd5c7e480e6d25de467ea1917c08290c521752f147283d
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.11-stable.orig.tar.gz.asc' libevent_2.1.11-stable.orig.tar.gz.asc 488 SHA256:9add12a6852022f675e4388cb1ac0fdcd68c6c1bc6e5212fae78d3f1c00f2826
'http://archive.ubuntu.com/ubuntu/pool/main/libe/libevent/libevent_2.1.11-stable-1.debian.tar.xz' libevent_2.1.11-stable-1.debian.tar.xz 17264 SHA256:fae364ea17e708a73572dd8b0add7fcded427c9e2b2405679738459c6f02de8d
```

### `dpkg` source package: `libfabric=1.6.2-3`

Binary Packages:

- `libfabric1=1.6.2-3`

Licenses: (parsed from: `/usr/share/doc/libfabric1/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris libfabric=1.6.2-3
'http://archive.ubuntu.com/ubuntu/pool/universe/libf/libfabric/libfabric_1.6.2-3.dsc' libfabric_1.6.2-3.dsc 2213 SHA256:e4279de971618b3e358a81e3f003234fb129f10770fc4b6507b532ffed8a643c
'http://archive.ubuntu.com/ubuntu/pool/universe/libf/libfabric/libfabric_1.6.2.orig.tar.xz' libfabric_1.6.2.orig.tar.xz 1030072 SHA256:924f4ebfd5537c7aa8e59ac7d732712fdcfff6f3a5f42b598736fbf99466dc40
'http://archive.ubuntu.com/ubuntu/pool/universe/libf/libfabric/libfabric_1.6.2-3.debian.tar.xz' libfabric_1.6.2-3.debian.tar.xz 10124 SHA256:e448bb32ded1ca91fc4beb64e2c7bdf3a45d541e9d41aca87e86d426ed3db2dd
```

### `dpkg` source package: `libffi=3.3-4`

Binary Packages:

- `libffi7:amd64=3.3-4`

Licenses: (parsed from: `/usr/share/doc/libffi7/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libffi=3.3-4
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.3-4.dsc' libffi_3.3-4.dsc 1932 SHA256:4190ad8e7ae9167a0c67c5926bc3705acb191745cca93ef845dbc06fc097f380
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.3.orig.tar.gz' libffi_3.3.orig.tar.gz 1305466 SHA256:72fba7922703ddfa7a028d513ac15a85c8d54c8d67f55fa5a4802885dc652056
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libffi/libffi_3.3-4.debian.tar.xz' libffi_3.3-4.debian.tar.xz 9016 SHA256:0e8a6d9d87202d04d7646178479c3d365a845f9723da26625d533a169b378100
```

### `dpkg` source package: `libfido2=1.3.1-1ubuntu2`

Binary Packages:

- `libfido2-1:amd64=1.3.1-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libfido2-1/copyright`)

- `BSD-2-clause`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libfido2=1.3.1-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.3.1-1ubuntu2.dsc' libfido2_1.3.1-1ubuntu2.dsc 2315 SHA256:2ff6b7cc320b84461404fa3830dfb5b705f7920b431173479144c73b4b50a59c
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.3.1.orig.tar.gz' libfido2_1.3.1.orig.tar.gz 1512676 SHA256:ba35e22016b60c1e4be66dff3cd6a60c1fe4bfa0d91ec0b89ca9da25ebeaaf41
'http://archive.ubuntu.com/ubuntu/pool/main/libf/libfido2/libfido2_1.3.1-1ubuntu2.debian.tar.xz' libfido2_1.3.1-1ubuntu2.debian.tar.xz 73992 SHA256:678fed0bfe9ae7cdb1834caedfeb0d1c86a16c4476f679de017b39f2b356a2f8
```

### `dpkg` source package: `libgcrypt20=1.8.5-5ubuntu1`

Binary Packages:

- `libgcrypt20:amd64=1.8.5-5ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libgcrypt20/copyright`)

- `GPL-2`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libgcrypt20=1.8.5-5ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-5ubuntu1.dsc' libgcrypt20_1.8.5-5ubuntu1.dsc 2944 SHA256:d3f3f499949d51909b12eb09b30c3d2f8f999ecf9f8e9bb33516d6cf5cff978c
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2' libgcrypt20_1.8.5.orig.tar.bz2 2991291 SHA256:3b4a2a94cb637eff5bdebbcaf46f4d95c4f25206f459809339cdada0eb577ac3
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5.orig.tar.bz2.asc' libgcrypt20_1.8.5.orig.tar.bz2.asc 488 SHA256:4b24fda7847cd2b70ab19f4c38004a76bbdac46a1ddccff973ae88ba1296a22d
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgcrypt20/libgcrypt20_1.8.5-5ubuntu1.debian.tar.xz' libgcrypt20_1.8.5-5ubuntu1.debian.tar.xz 32788 SHA256:c69bfdd42f4470894e6e4be0b742fb61aea85e16432a47a8365991adcc3de712
```

### `dpkg` source package: `libgpg-error=1.37-1`

Binary Packages:

- `libgpg-error-dev=1.37-1`
- `libgpg-error0:amd64=1.37-1`

Licenses: (parsed from: `/usr/share/doc/libgpg-error-dev/copyright`, `/usr/share/doc/libgpg-error0/copyright`)

- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `g10-permissive`

Source:

```console
$ apt-get source -qq --print-uris libgpg-error=1.37-1
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.37-1.dsc' libgpg-error_1.37-1.dsc 2220 SHA256:e789ed6bf791c90e9ba28dc3923f54379862ca65bd286495942176dcfad5d8a7
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.37.orig.tar.bz2' libgpg-error_1.37.orig.tar.bz2 937282 SHA256:b32d6ff72a73cf79797f7f2d039e95e9c6f92f0c1450215410840ab62aea9763
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.37.orig.tar.bz2.asc' libgpg-error_1.37.orig.tar.bz2.asc 488 SHA256:394f0904c386f88e2b2db5042880a2a302cbc6e4ab902bacf3d338ded038066b
'http://archive.ubuntu.com/ubuntu/pool/main/libg/libgpg-error/libgpg-error_1.37-1.debian.tar.xz' libgpg-error_1.37-1.debian.tar.xz 17332 SHA256:09843b599726c1ab7b1fcd86ce617bd91d6378ff754c6da0b7e536ed1c3b6c16
```

### `dpkg` source package: `libidn2=2.2.0-2`

Binary Packages:

- `libidn2-0:amd64=2.2.0-2`

Licenses: (parsed from: `/usr/share/doc/libidn2-0/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `Unicode`

Source:

```console
$ apt-get source -qq --print-uris libidn2=2.2.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.2.0-2.dsc' libidn2_2.2.0-2.dsc 2436 SHA256:a5c5ece3748beaba9ce0a0b29cdab2fe9d861a965a7a96101a49f194acf759d6
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.2.0.orig.tar.gz' libidn2_2.2.0.orig.tar.gz 2110743 SHA256:fc734732b506d878753ec6606982bf7b936e868c25c30ddb0d83f7d7056381fe
'http://archive.ubuntu.com/ubuntu/pool/main/libi/libidn2/libidn2_2.2.0-2.debian.tar.xz' libidn2_2.2.0-2.debian.tar.xz 11184 SHA256:b38ce002d7eb1abbf2c870ac9570cd06a5087693f359b133defbf44b06f8784d
```

### `dpkg` source package: `libjsoncpp=1.7.4-3.1ubuntu2`

Binary Packages:

- `libjsoncpp1:amd64=1.7.4-3.1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libjsoncpp1/copyright`)

- `Expat_or_PublicDomain_or_DualExpatPD`
- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris libjsoncpp=1.7.4-3.1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.7.4-3.1ubuntu2.dsc' libjsoncpp_1.7.4-3.1ubuntu2.dsc 2292 SHA256:29b690adbc515bc430e11cec45d9da7142e53893495beffe678e6b73a8f74b3d
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.7.4.orig.tar.gz' libjsoncpp_1.7.4.orig.tar.gz 205752 SHA256:10dcd0677e80727e572a1e462193e51a5fde3e023b99e144b2ee1a469835f769
'http://archive.ubuntu.com/ubuntu/pool/main/libj/libjsoncpp/libjsoncpp_1.7.4-3.1ubuntu2.debian.tar.xz' libjsoncpp_1.7.4-3.1ubuntu2.debian.tar.xz 8388 SHA256:1c21094022e664a66a2feb45f22520c6a66ecc6e558534647cf4fa7a14cb770a
```

### `dpkg` source package: `libksba=1.3.5-2`

Binary Packages:

- `libksba8:amd64=1.3.5-2`

Licenses: (parsed from: `/usr/share/doc/libksba8/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris libksba=1.3.5-2
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5-2.dsc' libksba_1.3.5-2.dsc 2526 SHA256:4fd08fd129f97ab1df86c220b88b7b2c6e4e04aa90bfd3ae364d18022256bef8
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5.orig.tar.bz2' libksba_1.3.5.orig.tar.bz2 620649 SHA256:41444fd7a6ff73a79ad9728f985e71c9ba8cd3e5e53358e70d5f066d35c1a340
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5.orig.tar.bz2.asc' libksba_1.3.5.orig.tar.bz2.asc 287 SHA256:a954b03144ee882c838853da24fd7b6868b78df72a18c71079217d968698a76f
'http://archive.ubuntu.com/ubuntu/pool/main/libk/libksba/libksba_1.3.5-2.debian.tar.xz' libksba_1.3.5-2.debian.tar.xz 13852 SHA256:98c985bff973be1aecc702fa15887ff1e5b8de481d1dc3e99423a587754eaabd
```

### `dpkg` source package: `libnl3=3.4.0-1`

Binary Packages:

- `libnl-3-200:amd64=3.4.0-1`
- `libnl-3-dev:amd64=3.4.0-1`
- `libnl-route-3-200:amd64=3.4.0-1`
- `libnl-route-3-dev:amd64=3.4.0-1`

Licenses: (parsed from: `/usr/share/doc/libnl-3-200/copyright`, `/usr/share/doc/libnl-3-dev/copyright`, `/usr/share/doc/libnl-route-3-200/copyright`, `/usr/share/doc/libnl-route-3-dev/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libnl3=3.4.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnl3/libnl3_3.4.0-1.dsc' libnl3_3.4.0-1.dsc 2731 SHA256:737c5824e9e839210daa3f15704b13c405377c676c10f2650b2eec9f9dcb8c96
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnl3/libnl3_3.4.0.orig.tar.gz' libnl3_3.4.0.orig.tar.gz 933443 SHA256:b7287637ae71c6db6f89e1422c995f0407ff2fe50cecd61a312b6a9b0921f5bf
'http://archive.ubuntu.com/ubuntu/pool/main/libn/libnl3/libnl3_3.4.0-1.debian.tar.xz' libnl3_3.4.0-1.debian.tar.xz 25432 SHA256:c317f9c462e27f5c2086f8831223cce8b98801b30c91fd0a79f5e9e672803f92
```

### `dpkg` source package: `libpciaccess=0.16-0ubuntu1`

Binary Packages:

- `libpciaccess0:amd64=0.16-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libpciaccess0/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libpciaccess=0.16-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.16-0ubuntu1.dsc' libpciaccess_0.16-0ubuntu1.dsc 1554 SHA256:7a69bc588b31fddaced85ec551fa75b92a8654c1da090326fba0571ca74c9129
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.16.orig.tar.gz' libpciaccess_0.16.orig.tar.gz 470061 SHA256:84413553994aef0070cf420050aa5c0a51b1956b404920e21b81e96db6a61a27
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpciaccess/libpciaccess_0.16-0ubuntu1.diff.gz' libpciaccess_0.16-0ubuntu1.diff.gz 25561 SHA256:d5beb9c0d60fa77c3c9ec90d188bb14875d64e0be5644716d1e615caa93d9461
```

### `dpkg` source package: `libpsl=0.21.0-1ubuntu1`

Binary Packages:

- `libpsl5:amd64=0.21.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libpsl5/copyright`)

- `Chromium`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libpsl=0.21.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1ubuntu1.dsc' libpsl_0.21.0-1ubuntu1.dsc 2383 SHA256:38d6cf06b8ac1929efe109ac3d5f37ea6e89ea82f7a5125db4dc7a7b5f3faf94
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0.orig.tar.gz' libpsl_0.21.0.orig.tar.gz 8598583 SHA256:055aa87ec166c7afb985d0816c07ff440e1eb899881a318c51c69a0aeea8e279
'http://archive.ubuntu.com/ubuntu/pool/main/libp/libpsl/libpsl_0.21.0-1ubuntu1.debian.tar.xz' libpsl_0.21.0-1ubuntu1.debian.tar.xz 12476 SHA256:efd6c7ae8c244b582d6af943b5925d95a31a183abf695301f2fa49de9f694671
```

### `dpkg` source package: `libpsm2=11.2.86-1`

Binary Packages:

- `libpsm2-2=11.2.86-1`

Licenses: (parsed from: `/usr/share/doc/libpsm2-2/copyright`)

- `BSD-3-Clause/Intel`
- `BSD-3-Clause/TT`
- `BSD-3-Clause/zlib`
- `BSD-4-Clause/UC`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris libpsm2=11.2.86-1
'http://archive.ubuntu.com/ubuntu/pool/universe/libp/libpsm2/libpsm2_11.2.86-1.dsc' libpsm2_11.2.86-1.dsc 2119 SHA256:daed26a906cfdac62c13af7aa026bd86553fd93b2a9548a14b3be25808dc5641
'http://archive.ubuntu.com/ubuntu/pool/universe/libp/libpsm2/libpsm2_11.2.86.orig.tar.gz' libpsm2_11.2.86.orig.tar.gz 460705 SHA256:a5fb4412ddb5b12ab0e67bdd96fe7c010e0ffb2f332bdf4fe28c52bc31acf104
'http://archive.ubuntu.com/ubuntu/pool/universe/libp/libpsm2/libpsm2_11.2.86-1.debian.tar.xz' libpsm2_11.2.86-1.debian.tar.xz 7104 SHA256:69433ff0dd7fb7a299a6d14f5c57ff3f8dd1ec908293449cb8f0d91fffb96926
```

### `dpkg` source package: `libseccomp=2.4.3-1ubuntu3.20.04.3`

Binary Packages:

- `libseccomp2:amd64=2.4.3-1ubuntu3.20.04.3`

Licenses: (parsed from: `/usr/share/doc/libseccomp2/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libseccomp=2.4.3-1ubuntu3.20.04.3
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.20.04.3.dsc' libseccomp_2.4.3-1ubuntu3.20.04.3.dsc 2226 SHA512:7510d7ea834c48b67f3c40bb94b554029e5ea53e024808510da15550205cee369815a162f8697dd915fdd3d89c7afea60da89721d049769f51f2d4c5c9423feb
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3.orig.tar.gz' libseccomp_2.4.3.orig.tar.gz 598147 SHA512:7b7af2e98493243ffe1934fefff5723b24ae9b9bdc4bf039343ee8456c15acb0ea34e81ec292a41143848272aeca794ef92ad38fc3f42c77465170cb540479ef
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libseccomp/libseccomp_2.4.3-1ubuntu3.20.04.3.debian.tar.xz' libseccomp_2.4.3-1ubuntu3.20.04.3.debian.tar.xz 36444 SHA512:445b0bac2e39586aa99307fb558623bc8064fb4638ca650698344aab40d3a639c5a8f6c23384a36b9250eb8a682e06831315fc6d7910e768903b7cfac137ecbd
```

### `dpkg` source package: `libselinux=3.0-1build2`

Binary Packages:

- `libselinux1:amd64=3.0-1build2`

Licenses: (parsed from: `/usr/share/doc/libselinux1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libselinux=3.0-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.0-1build2.dsc' libselinux_3.0-1build2.dsc 2565 SHA256:9a8d6c354ed06350606c009d899d117e71fda20887792b2c25b38222d0190d93
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.0.orig.tar.gz' libselinux_3.0.orig.tar.gz 212096 SHA256:2ea2b30f671dae9d6b1391cbe8fb2ce5d36a3ee4fb1cd3c32f0d933c31b82433
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libselinux/libselinux_3.0-1build2.debian.tar.xz' libselinux_3.0-1build2.debian.tar.xz 23720 SHA256:ed85da0fe5561205c95f0f622562425dc7d8dd61ffd213a7fa914d778fe8da71
```

### `dpkg` source package: `libsemanage=3.0-1build2`

Binary Packages:

- `libsemanage-common=3.0-1build2`
- `libsemanage1:amd64=3.0-1build2`

Licenses: (parsed from: `/usr/share/doc/libsemanage-common/copyright`, `/usr/share/doc/libsemanage1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsemanage=3.0-1build2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.0-1build2.dsc' libsemanage_3.0-1build2.dsc 2678 SHA256:6231f4b00991657fafef2595eb571b2bcbe437de4ec9dc9929c0e69187db5f33
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.0.orig.tar.gz' libsemanage_3.0.orig.tar.gz 180745 SHA256:a497b0720d54eac427f1f3f618eed417e50ed8f4e47ed0f7a1d391bd416e84cf
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsemanage/libsemanage_3.0-1build2.debian.tar.xz' libsemanage_3.0-1build2.debian.tar.xz 17176 SHA256:38a646f91532c920c8c15a695c3585397ddbf032ecf49c52eb89d53c8eac48fb
```

### `dpkg` source package: `libsepol=3.0-1`

Binary Packages:

- `libsepol1:amd64=3.0-1`

Licenses: (parsed from: `/usr/share/doc/libsepol1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris libsepol=3.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.0-1.dsc' libsepol_3.0-1.dsc 1770 SHA256:0073de5844605d380dd56f6630678ad91459496dc768fa9eb4d8cc7f693f5c1a
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.0.orig.tar.gz' libsepol_3.0.orig.tar.gz 473864 SHA256:5b7ae1881909f1048b06f7a0c364c5c8a86ec12e0ec76e740fe9595a6033eb79
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsepol/libsepol_3.0-1.debian.tar.xz' libsepol_3.0-1.debian.tar.xz 14224 SHA256:a16b5bc3c041e016d01794d1a1b9826ed4426862622c05526e93607c325ec328
```

### `dpkg` source package: `libsigsegv=2.12-2`

Binary Packages:

- `libsigsegv2:amd64=2.12-2`

Licenses: (parsed from: `/usr/share/doc/libsigsegv2/copyright`)

- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `permissive-fsf`
- `permissive-other`

Source:

```console
$ apt-get source -qq --print-uris libsigsegv=2.12-2
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12-2.dsc' libsigsegv_2.12-2.dsc 2363 SHA256:b081b244de2f427345838f379405d8438c29db1fa746a4e270167ae7cb10c079
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz' libsigsegv_2.12.orig.tar.gz 451408 SHA256:3ae1af359eebaa4ffc5896a1aee3568c052c99879316a1ab57f8fe1789c390b6
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12.orig.tar.gz.asc' libsigsegv_2.12.orig.tar.gz.asc 2442 SHA256:1861a9a182bbb7a24a18f7e43fe0fa3eb6f6fd53780b30e01990677112694dfc
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsigsegv/libsigsegv_2.12-2.debian.tar.xz' libsigsegv_2.12-2.debian.tar.xz 8340 SHA256:73940fb346f7afd90c93a341164cd175349e0507de8b1c05b0834b598c372260
```

### `dpkg` source package: `libsodium=1.0.18-1`

Binary Packages:

- `libsodium23:amd64=1.0.18-1`

Licenses: (parsed from: `/usr/share/doc/libsodium23/copyright`)

- `BSD-2-clause`
- `CC0`
- `CC0-1.0`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libsodium=1.0.18-1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsodium/libsodium_1.0.18-1.dsc' libsodium_1.0.18-1.dsc 1913 SHA256:037b3ac05a50409cb462e2c21c7a67f983d193a22d2486f4ab3fdc793f5a731c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsodium/libsodium_1.0.18.orig.tar.gz' libsodium_1.0.18.orig.tar.gz 1619527 SHA256:d59323c6b712a1519a5daf710b68f5e7fde57040845ffec53850911f10a5d4f4
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libsodium/libsodium_1.0.18-1.debian.tar.xz' libsodium_1.0.18-1.debian.tar.xz 7440 SHA256:50863d8fc4f0a2a86f7b69745514455f0b9d74cf45906523c675ffe5b8db0377
```

### `dpkg` source package: `libssh=0.9.3-2ubuntu2.1`

Binary Packages:

- `libssh-4:amd64=0.9.3-2ubuntu2.1`

Licenses: (parsed from: `/usr/share/doc/libssh-4/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `LGPL-2.1`
- `LGPL-2.1+~OpenSSL`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris libssh=0.9.3-2ubuntu2.1
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.3-2ubuntu2.1.dsc' libssh_0.9.3-2ubuntu2.1.dsc 2538 SHA512:a0b51fd53355d282334d2ab1124de8c5995788160646d2a70a6d7027e0e2d49a82889ea9aa4a6d3ee0a7aaa7389370b49507bb24a6144578928417fafb47b29c
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.3.orig.tar.xz' libssh_0.9.3.orig.tar.xz 500068 SHA512:6e59718565daeca6d224426cc1095a112deff9af8e0b021917e04f08bb7409263c35724de95f591f38e26f0fb3bbbbc69b679b6775edc21dec158d241b076c6f
'http://archive.ubuntu.com/ubuntu/pool/main/libs/libssh/libssh_0.9.3-2ubuntu2.1.debian.tar.xz' libssh_0.9.3-2ubuntu2.1.debian.tar.xz 28488 SHA512:cecd6d2f385fa4c440aa03a7d864387bb1d5ca2f2e252103c295b1596b8b1336bfdefa2dd38ffaf7396423c9b7dafe005896177ded669a5790fd7320643d01b4
```

### `dpkg` source package: `libtasn1-6=4.16.0-2`

Binary Packages:

- `libtasn1-6:amd64=4.16.0-2`

Licenses: (parsed from: `/usr/share/doc/libtasn1-6/copyright`)

- `GFDL-1.3`
- `GPL-3`
- `LGPL`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris libtasn1-6=4.16.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0-2.dsc' libtasn1-6_4.16.0-2.dsc 2586 SHA256:fd4a387c71f95c3eceb1072a3f42c7021d73128027ea41a18d6efc6cbfdd764a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0.orig.tar.gz' libtasn1-6_4.16.0.orig.tar.gz 1812442 SHA256:0e0fb0903839117cb6e3b56e68222771bebf22ad7fc2295a0ed7d576e8d4329d
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0.orig.tar.gz.asc' libtasn1-6_4.16.0.orig.tar.gz.asc 488 SHA256:06c201e8c3b43c27465ed79294d4c4ec8dcd3e95e4a6176ecbf273229ee3e2d0
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtasn1-6/libtasn1-6_4.16.0-2.debian.tar.xz' libtasn1-6_4.16.0-2.debian.tar.xz 17740 SHA256:c1a89b0bac0fb7c83ebac4eafbca0475c24350ade6ccaef31266424725610624
```

### `dpkg` source package: `libtool=2.4.6-14`

Binary Packages:

- `libltdl-dev:amd64=2.4.6-14`
- `libltdl7:amd64=2.4.6-14`

Licenses: (parsed from: `/usr/share/doc/libltdl-dev/copyright`, `/usr/share/doc/libltdl7/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris libtool=2.4.6-14
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-14.dsc' libtool_2.4.6-14.dsc 2500 SHA256:939797b7ce62f69641d319e5d38e53b1608cee649355046eec74271e9fcfb9df
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz' libtool_2.4.6.orig.tar.xz 973080 SHA256:7c87a8c2c8c0fc9cd5019e402bed4292462d00a718a7cd5f11218153bf28b26f
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6.orig.tar.xz.asc' libtool_2.4.6.orig.tar.xz.asc 380 SHA256:ab68ebc45d60128a71fc36167cd29dcf3c3d6d639fd28663905ebaf3e2f43d6a
'http://archive.ubuntu.com/ubuntu/pool/main/libt/libtool/libtool_2.4.6-14.debian.tar.xz' libtool_2.4.6-14.debian.tar.xz 50832 SHA256:3ef693ea30def97a19fd94ffb2fa5421d5dc35cf7ad897a7161bd647eb4f2415
```

### `dpkg` source package: `libunistring=0.9.10-2`

Binary Packages:

- `libunistring2:amd64=0.9.10-2`

Licenses: (parsed from: `/usr/share/doc/libunistring2/copyright`)

- `FreeSoftware`
- `GFDL-1.2`
- `GFDL-1.2+`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with distribution exception`
- `GPL-3`
- `GPL-3+`
- `LGPL-3`
- `LGPL-3+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris libunistring=0.9.10-2
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-2.dsc' libunistring_0.9.10-2.dsc 2206 SHA256:c6faf64e2d978ec074ebf88264730121dfd03cc1639df94b5dc3eb05b1678532
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz' libunistring_0.9.10.orig.tar.xz 2051320 SHA256:eb8fb2c3e4b6e2d336608377050892b54c3c983b646c561836550863003c05d7
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10.orig.tar.xz.asc' libunistring_0.9.10.orig.tar.xz.asc 1310 SHA256:e1606f691034fa21b00e08269622743547c16d21cca6c8a64156b4774a49e78e
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libunistring/libunistring_0.9.10-2.debian.tar.xz' libunistring_0.9.10-2.debian.tar.xz 40708 SHA256:5e291a1a15549d12c64575c72868a8c94586715d35062b5efb48fe9a9d09924e
```

### `dpkg` source package: `libuv1=1.34.2-1ubuntu1`

Binary Packages:

- `libuv1:amd64=1.34.2-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libuv1/copyright`)

- `BSD-1-clause`
- `BSD-2-clause`
- `BSD-3-clause`
- `CC-BY-4.0`
- `Expat`
- `GPL-3`
- `GPL-3+`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris libuv1=1.34.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libuv1/libuv1_1.34.2-1ubuntu1.dsc' libuv1_1.34.2-1ubuntu1.dsc 2157 SHA256:543b13d8f0ee4b628f2259a1085bc701ea68c8789c205b0f54354c1266c3ce54
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libuv1/libuv1_1.34.2.orig.tar.gz' libuv1_1.34.2.orig.tar.gz 1245417 SHA256:8cfc368fc3eb2412a8972d3f0e600d9fb380ebc293c3b9403290ad00bab2ce3a
'http://archive.ubuntu.com/ubuntu/pool/main/libu/libuv1/libuv1_1.34.2-1ubuntu1.debian.tar.xz' libuv1_1.34.2-1ubuntu1.debian.tar.xz 21896 SHA256:c041a02b38d7dacb842808dec080fcbd95e5107fd425295e5e1714d5e7bb0496
```

### `dpkg` source package: `libx11=2:1.6.9-2ubuntu1.1`

Binary Packages:

- `libx11-6:amd64=2:1.6.9-2ubuntu1.1`
- `libx11-data=2:1.6.9-2ubuntu1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libx11=2:1.6.9-2ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.9-2ubuntu1.1.dsc' libx11_1.6.9-2ubuntu1.1.dsc 2671 SHA512:72c42a4f8ada92e23ce736a64bbb8a4c5ce9073a3402c1734def182cd567cc50036a7555ad065bf59716ca7a07401d35d5dd180b02a0bea6a0ec389a7f8718ef
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.9.orig.tar.gz' libx11_1.6.9.orig.tar.gz 2994329 SHA512:c79cf0924e920a2e8d2e9af45e73ed42b565dea79ac68d4c3889033738274694b29cedb62c057fec1aa7f7ad7dcf843334fccb43470bbae7922d42373c1c6045
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.9.orig.tar.gz.asc' libx11_1.6.9.orig.tar.gz.asc 659 SHA512:56e53d1481be4e12f89af2fbcd297a3612996f5ca1eae39d6fe336f9b52832ea430ac0568e556b9e57291562c56590086871c08ec7ac046f15af4211f680adee
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libx11/libx11_1.6.9-2ubuntu1.1.diff.gz' libx11_1.6.9-2ubuntu1.1.diff.gz 65340 SHA512:a50e3bb3f9927886cf9f5b074024def634487008b239952f96348befc69bd695c751a47e4405d95ffe11409659bafb3811a76a239ef364e48407a27fe607e445
```

### `dpkg` source package: `libxau=1:1.0.9-0ubuntu1`

Binary Packages:

- `libxau6:amd64=1:1.0.9-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxau=1:1.0.9-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-0ubuntu1.dsc' libxau_1.0.9-0ubuntu1.dsc 1563 SHA256:b59509d1f8f6c0e21b8bbd46ac1dffcd7a21a635ff3ce9c0acf68ba60fcb5e11
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9.orig.tar.gz' libxau_1.0.9.orig.tar.gz 394068 SHA256:1f123d8304b082ad63a9e89376400a3b1d4c29e67e3ea07b3f659cccca690eea
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxau/libxau_1.0.9-0ubuntu1.diff.gz' libxau_1.0.9-0ubuntu1.diff.gz 15142 SHA256:cf7e9d50c3b3b8dde3486ee6fcf9bb96585e2af32924e91c10c8612e48b5dce5
```

### `dpkg` source package: `libxcb=1.14-2`

Binary Packages:

- `libxcb1:amd64=1.14-2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcb=1.14-2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-2.dsc' libxcb_1.14-2.dsc 5344 SHA256:997dfadefa35a243a7160b62d628bb25e45439f61687459d581502905bcf1fb2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14.orig.tar.gz' libxcb_1.14.orig.tar.gz 640322 SHA256:2c7fcddd1da34d9b238c9caeda20d3bd7486456fc50b3cc6567185dbd5b0ad02
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcb/libxcb_1.14-2.diff.gz' libxcb_1.14-2.diff.gz 25716 SHA256:92d7e0a80c3c7f2a5b5afd0c0702183f1c483338d678d67d8d0e61fd8989ba85
```

### `dpkg` source package: `libxcrypt=1:4.4.10-10ubuntu4`

Binary Packages:

- `libcrypt-dev:amd64=1:4.4.10-10ubuntu4`
- `libcrypt1:amd64=1:4.4.10-10ubuntu4`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxcrypt=1:4.4.10-10ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.10-10ubuntu4.dsc' libxcrypt_4.4.10-10ubuntu4.dsc 2216 SHA256:457576b36eaa34dcf28b19e942908221d0618e9e4a2c0b9e11ba9693770756a2
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.10.orig.tar.xz' libxcrypt_4.4.10.orig.tar.xz 372652 SHA256:f790a8eac4e4af3124d2844a24a7afb3a972368e4dff63d701599c2f2d065fd3
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxcrypt/libxcrypt_4.4.10-10ubuntu4.debian.tar.xz' libxcrypt_4.4.10-10ubuntu4.debian.tar.xz 5760 SHA256:b2e665b5224911d24dbcbddfc61b7a27428c3ecb744f29ceea1b2984496f2ffa
```

### `dpkg` source package: `libxdmcp=1:1.1.3-0ubuntu1`

Binary Packages:

- `libxdmcp6:amd64=1:1.1.3-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxdmcp=1:1.1.3-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3-0ubuntu1.dsc' libxdmcp_1.1.3-0ubuntu1.dsc 1608 SHA256:3f98e3917b5de252eb517c55743bcc5682b43c9f70ead33231ac4318bbc816e1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3.orig.tar.gz' libxdmcp_1.1.3.orig.tar.gz 429668 SHA256:2ef9653d32e09d1bf1b837d0e0311024979653fe755ad3aaada8db1aa6ea180c
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxdmcp/libxdmcp_1.1.3-0ubuntu1.diff.gz' libxdmcp_1.1.3-0ubuntu1.diff.gz 18079 SHA256:3037a57202b724ecd7db70c21a601f58277c02ba89e7e5d999973e5baf6d05ca
```

### `dpkg` source package: `libxext=2:1.3.4-0ubuntu1`

Binary Packages:

- `libxext6:amd64=2:1.3.4-0ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris libxext=2:1.3.4-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-0ubuntu1.dsc' libxext_1.3.4-0ubuntu1.dsc 1727 SHA256:8319de2750f28c78e01267a5593776f10afd3f863d4820abe72dbf855a3a77ae
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4.orig.tar.gz' libxext_1.3.4.orig.tar.gz 494434 SHA256:8ef0789f282826661ff40a8eef22430378516ac580167da35cc948be9041aac1
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxext/libxext_1.3.4-0ubuntu1.diff.gz' libxext_1.3.4-0ubuntu1.diff.gz 20663 SHA256:87a4d23f1f9ff53f3a6cd7cc35252a1249dc63d274c566ea7e23b23585a86170
```

### `dpkg` source package: `libxml2=2.9.10+dfsg-5`

Binary Packages:

- `libxml2:amd64=2.9.10+dfsg-5`

Licenses: (parsed from: `/usr/share/doc/libxml2/copyright`)

- `ISC`
- `MIT-1`

Source:

```console
$ apt-get source -qq --print-uris libxml2=2.9.10+dfsg-5
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg-5.dsc' libxml2_2.9.10+dfsg-5.dsc 2982 SHA256:95f66df911ac4ff2b1d232b5f6613a968f91a55eb4554ed8aee65c4ae58ca42b
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg.orig.tar.xz' libxml2_2.9.10+dfsg.orig.tar.xz 2503560 SHA256:65ee7a2f5e100c64ddf7beb92297c9b2a30b994a76cd1fab67470cf22db6b7d0
'http://archive.ubuntu.com/ubuntu/pool/main/libx/libxml2/libxml2_2.9.10+dfsg-5.debian.tar.xz' libxml2_2.9.10+dfsg-5.debian.tar.xz 28736 SHA256:d2de33926b5f8093766050af3ad362a415f285c2339a675886f7b3aff3d220bf
```

### `dpkg` source package: `libyaml=0.2.2-1`

Binary Packages:

- `libyaml-0-2:amd64=0.2.2-1`

Licenses: (parsed from: `/usr/share/doc/libyaml-0-2/copyright`)

- `Expat`
- `permissive`

Source:

```console
$ apt-get source -qq --print-uris libyaml=0.2.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1.dsc' libyaml_0.2.2-1.dsc 1833 SHA256:b4baba985391f52409013a0c9303191e34aaa4c1c9200e4c01c4963df801db09
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2.orig.tar.gz' libyaml_0.2.2.orig.tar.gz 602509 SHA256:689ef3ebdecfa81f3789ccd2481acc81fc0f22f3f5c947eed95c4c0802e356b8
'http://archive.ubuntu.com/ubuntu/pool/main/liby/libyaml/libyaml_0.2.2-1.debian.tar.xz' libyaml_0.2.2-1.debian.tar.xz 4112 SHA256:186aad3e4bcd95891a8c59249c59f862f5f71601058fda0bf020a9e9e39320fe
```

### `dpkg` source package: `libzstd=1.4.4+dfsg-3`

Binary Packages:

- `libzstd1:amd64=1.4.4+dfsg-3`

Licenses: (parsed from: `/usr/share/doc/libzstd1/copyright`)

- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-2+`
- `zlib`

Source:

```console
$ apt-get source -qq --print-uris libzstd=1.4.4+dfsg-3
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.4+dfsg-3.dsc' libzstd_1.4.4+dfsg-3.dsc 2266 SHA256:f6e3cc2b022b9812daca4f427a00fc6e109e6e1e72e64d6a254add040853b110
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.4+dfsg.orig.tar.xz' libzstd_1.4.4+dfsg.orig.tar.xz 1357144 SHA256:be9f9bfd3f6816f21e1108869a9acad6efdc4882ed3f7a1f58ec752f67864890
'http://archive.ubuntu.com/ubuntu/pool/main/libz/libzstd/libzstd_1.4.4+dfsg-3.debian.tar.xz' libzstd_1.4.4+dfsg-3.debian.tar.xz 16068 SHA256:f7fec89f1fae04dfa551d124973167e09e84c864a25961aa20727cc91277b0e6
```

### `dpkg` source package: `linux=5.4.0-48.52`

Binary Packages:

- `linux-libc-dev:amd64=5.4.0-48.52`

Licenses: (parsed from: `/usr/share/doc/linux-libc-dev/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris linux=5.4.0-48.52
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.4.0-48.52.dsc' linux_5.4.0-48.52.dsc 6875 SHA512:235645735c8549f03b28b3d3306298a5fab55e44bc14c80bec89ed5d70ce786e78e1039d3c62b23abcd682149d583d396ef26cf9722a48fdd9f7db32de3b7e37
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.4.0.orig.tar.gz' linux_5.4.0.orig.tar.gz 170244619 SHA512:62b09a7231fd793973c5f59b16c4f6ffce621188b02a71915874b05e8e3f956fb6146d4a4fb1a4475bebe463949ca5a18da12842c3ce7c52e996e6bc4012a074
'http://archive.ubuntu.com/ubuntu/pool/main/l/linux/linux_5.4.0-48.52.diff.gz' linux_5.4.0-48.52.diff.gz 5335070 SHA512:937475b988ca5a48718cc4d3dfb50719569e97a5fb33f723c6e42e2f5fd4f9e97edb544a158b330107845a0bda0291ff988a7b4503dc6265a7ab4f5cfdbfd983
```

### `dpkg` source package: `lksctp-tools=1.0.18+dfsg-1`

Binary Packages:

- `libsctp-dev:amd64=1.0.18+dfsg-1`
- `libsctp1:amd64=1.0.18+dfsg-1`

Licenses: (parsed from: `/usr/share/doc/libsctp-dev/copyright`, `/usr/share/doc/libsctp1/copyright`)

- `BSD-3-clause`
- `GPL-2`
- `GPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris lksctp-tools=1.0.18+dfsg-1
'http://archive.ubuntu.com/ubuntu/pool/main/l/lksctp-tools/lksctp-tools_1.0.18+dfsg-1.dsc' lksctp-tools_1.0.18+dfsg-1.dsc 2017 SHA256:648c5a77722638056592fa9ba7bc99359ab70fcdf9f37c53e05d8cda96624705
'http://archive.ubuntu.com/ubuntu/pool/main/l/lksctp-tools/lksctp-tools_1.0.18+dfsg.orig.tar.gz' lksctp-tools_1.0.18+dfsg.orig.tar.gz 194751 SHA256:ac0f4e499281e1d190b5cc9c7e31570de4b82fade1c2754a21b2c8e215cb3cf5
'http://archive.ubuntu.com/ubuntu/pool/main/l/lksctp-tools/lksctp-tools_1.0.18+dfsg-1.debian.tar.xz' lksctp-tools_1.0.18+dfsg-1.debian.tar.xz 10488 SHA256:826130ee1a35bec5a0f73160328e4429f3a64e57a865c6e9b2286d2cc8ff2d30
```

### `dpkg` source package: `log4cxx=0.10.0-15ubuntu2`

Binary Packages:

- `liblog4cxx-dev:amd64=0.10.0-15ubuntu2`
- `liblog4cxx10v5:amd64=0.10.0-15ubuntu2`

Licenses: (parsed from: `/usr/share/doc/liblog4cxx-dev/copyright`, `/usr/share/doc/liblog4cxx10v5/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris log4cxx=0.10.0-15ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/universe/l/log4cxx/log4cxx_0.10.0-15ubuntu2.dsc' log4cxx_0.10.0-15ubuntu2.dsc 2167 SHA256:84a4258312dfa175547129e9f6e3fbee5f2940c14b5203a1ba81710bf79c03cb
'http://archive.ubuntu.com/ubuntu/pool/universe/l/log4cxx/log4cxx_0.10.0.orig.tar.gz' log4cxx_0.10.0.orig.tar.gz 1667425 SHA256:0de0396220a9566a580166e66b39674cb40efd2176f52ad2c65486c99c920c8c
'http://archive.ubuntu.com/ubuntu/pool/universe/l/log4cxx/log4cxx_0.10.0-15ubuntu2.debian.tar.xz' log4cxx_0.10.0-15ubuntu2.debian.tar.xz 16668 SHA256:427ea0f1c8dd86c9ba3ba371fd8e5794c4ef5c2c255b8f6b7516a3e97f50a019
```

### `dpkg` source package: `lsb=11.1.0ubuntu2`

Binary Packages:

- `lsb-base=11.1.0ubuntu2`
- `lsb-release=11.1.0ubuntu2`

Licenses: (parsed from: `/usr/share/doc/lsb-base/copyright`, `/usr/share/doc/lsb-release/copyright`)

- `BSD-3-clause`
- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris lsb=11.1.0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu2.dsc' lsb_11.1.0ubuntu2.dsc 2230 SHA256:983ff4ab1ab2b39af974e4b8f4373ab4028d0ee5a409e7cd40401fa8e6ecabde
'http://archive.ubuntu.com/ubuntu/pool/main/l/lsb/lsb_11.1.0ubuntu2.tar.xz' lsb_11.1.0ubuntu2.tar.xz 46024 SHA256:c6ab63b6702dc633988690aacde8ece3e460f8acd8f1af8e6a67ab2fe0798f41
```

### `dpkg` source package: `lz4=1.9.2-2`

Binary Packages:

- `liblz4-1:amd64=1.9.2-2`
- `liblz4-dev:amd64=1.9.2-2`

Licenses: (parsed from: `/usr/share/doc/liblz4-1/copyright`, `/usr/share/doc/liblz4-dev/copyright`)

- `BSD-2-clause`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris lz4=1.9.2-2
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2-2.dsc' lz4_1.9.2-2.dsc 1956 SHA256:103fa80edbf501cf6e6d9ee0ed3d75d6111cd06026b00aaccaa11fe5555b71a6
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2.orig.tar.gz' lz4_1.9.2.orig.tar.gz 305796 SHA256:658ba6191fa44c92280d4aa2c271b0f4fbc0e34d249578dd05e50e76d0e5efcc
'http://archive.ubuntu.com/ubuntu/pool/main/l/lz4/lz4_1.9.2-2.debian.tar.xz' lz4_1.9.2-2.debian.tar.xz 12712 SHA256:8970a0afc2f1633bbc8b7f55fa36ba711fb4d0c1811e591ad8f52d1d1968592c
```

### `dpkg` source package: `m4=1.4.18-4`

Binary Packages:

- `m4=1.4.18-4`

Licenses: (parsed from: `/usr/share/doc/m4/copyright`)

- `GFDL`
- `GPL`

Source:

```console
$ apt-get source -qq --print-uris m4=1.4.18-4
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-4.dsc' m4_1.4.18-4.dsc 1638 SHA256:11925f50e25f93d6b9a72336e7b9fd0de72a813d5d5f3204ecc3996f9ca3bbde
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz' m4_1.4.18.orig.tar.xz 1207688 SHA256:f2c1e86ca0a404ff281631bdc8377638992744b175afb806e25871a24a934e07
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18.orig.tar.xz.asc' m4_1.4.18.orig.tar.xz.asc 521 SHA256:a2a9fff657e65ff25a8f3734f484dbd3ede8f8290786af71626de367dcd74267
'http://archive.ubuntu.com/ubuntu/pool/main/m/m4/m4_1.4.18-4.debian.tar.xz' m4_1.4.18-4.debian.tar.xz 17240 SHA256:6543f074d5a3eed4ee7984f8a147c58e005c88254dfcf5bc3778c60b9ed07efd
```

### `dpkg` source package: `make-dfsg=4.2.1-1.2`

Binary Packages:

- `make=4.2.1-1.2`

Licenses: (parsed from: `/usr/share/doc/make/copyright`)

- `GPL-3`
- `GPL-3+`

Source:

```console
$ apt-get source -qq --print-uris make-dfsg=4.2.1-1.2
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.2.1-1.2.dsc' make-dfsg_4.2.1-1.2.dsc 2019 SHA256:0c8a2da5d51e03bf43e2929322d5a8406f08e5ee2d81a71ed6e5a8734f1b05cb
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.2.1.orig.tar.gz' make-dfsg_4.2.1.orig.tar.gz 1485018 SHA256:480405e8995796ea47cc54b281b7855280f0d815d296a1af1993eeeb72074e39
'http://archive.ubuntu.com/ubuntu/pool/main/m/make-dfsg/make-dfsg_4.2.1-1.2.diff.gz' make-dfsg_4.2.1-1.2.diff.gz 53108 SHA256:80e0b96cee381391a5d3322317075e23d8474c92c5fa4fecd334bc2e0920887b
```

### `dpkg` source package: `mawk=1.3.4.20200120-2`

Binary Packages:

- `mawk=1.3.4.20200120-2`

Licenses: (parsed from: `/usr/share/doc/mawk/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris mawk=1.3.4.20200120-2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-2.dsc' mawk_1.3.4.20200120-2.dsc 1915 SHA256:5069c46872ac74f5221250dfb88b31b1f2dbb8a2617c1e013f8f80cc34638c6d
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120.orig.tar.gz' mawk_1.3.4.20200120.orig.tar.gz 468855 SHA256:7fd4cd1e1fae9290fe089171181bbc6291dfd9bca939ca804f0ddb851c8b8237
'http://archive.ubuntu.com/ubuntu/pool/main/m/mawk/mawk_1.3.4.20200120-2.debian.tar.xz' mawk_1.3.4.20200120-2.debian.tar.xz 7504 SHA256:b772ed2f016b0286980c46cbc1f1f4ae62887ef2aa3dff6ef10cae638f923f26
```

### `dpkg` source package: `mime-support=3.64ubuntu1`

Binary Packages:

- `mime-support=3.64ubuntu1`

Licenses: (parsed from: `/usr/share/doc/mime-support/copyright`)

- `Bellcore`
- `ad-hoc`

Source:

```console
$ apt-get source -qq --print-uris mime-support=3.64ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.64ubuntu1.dsc' mime-support_3.64ubuntu1.dsc 1729 SHA256:669ba4f3fd7594f1c32731b5636b499f44f21c7667148f6f0d16043708743fdc
'http://archive.ubuntu.com/ubuntu/pool/main/m/mime-support/mime-support_3.64ubuntu1.tar.xz' mime-support_3.64ubuntu1.tar.xz 33980 SHA256:5007d2ebc25935bfca6d4bdac0efdfc089a38c1be49d19f0422559f666e4f2c4
```

### `dpkg` source package: `mpclib3=1.1.0-1`

Binary Packages:

- `libmpc3:amd64=1.1.0-1`

Licenses: (parsed from: `/usr/share/doc/libmpc3/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris mpclib3=1.1.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.1.0-1.dsc' mpclib3_1.1.0-1.dsc 1990 SHA256:bb57824015b735bf72399a53f8c6a241e6a8bd402753b0fdcdaa5b99d0aef790
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.1.0.orig.tar.gz' mpclib3_1.1.0.orig.tar.gz 701263 SHA256:6985c538143c1208dcb1ac42cedad6ff52e267b47e5f970183a3e75125b43c2e
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpclib3/mpclib3_1.1.0-1.diff.gz' mpclib3_1.1.0-1.diff.gz 3794 SHA256:84b10a4ae958b3015e136b75be5fee22961255d19be655f7d0adae8d4f3bc977
```

### `dpkg` source package: `mpdecimal=2.4.2-3`

Binary Packages:

- `libmpdec2:amd64=2.4.2-3`

Licenses: (parsed from: `/usr/share/doc/libmpdec2/copyright`)

- `BSD`
- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpdecimal=2.4.2-3
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-3.dsc' mpdecimal_2.4.2-3.dsc 1932 SHA256:4cdd04de9915af3c9d787f4922affc1993d76c25cd0715ffdd2658da37c86753
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2.orig.tar.gz' mpdecimal_2.4.2.orig.tar.gz 2271529 SHA256:83c628b90f009470981cf084c5418329c88b19835d8af3691b930afccb7d79c7
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpdecimal/mpdecimal_2.4.2-3.debian.tar.xz' mpdecimal_2.4.2-3.debian.tar.xz 6352 SHA256:1baf12776a911bc77f76e16aa7600d4ace21a27817f4a56373093065205a9292
```

### `dpkg` source package: `mpfr4=4.0.2-1`

Binary Packages:

- `libmpfr6:amd64=4.0.2-1`

Licenses: (parsed from: `/usr/share/doc/libmpfr6/copyright`)

- `GFDL-1.2`
- `LGPL-3`

Source:

```console
$ apt-get source -qq --print-uris mpfr4=4.0.2-1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.2-1.dsc' mpfr4_4.0.2-1.dsc 1972 SHA256:9021ec2462ed0e73ea1379266740473abf5f826be819226497729f6c6b02e672
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.2.orig.tar.xz' mpfr4_4.0.2.orig.tar.xz 1441996 SHA256:1d3be708604eae0e42d578ba93b390c2a145f17743a744d8f3f8c2ad5855a38a
'http://archive.ubuntu.com/ubuntu/pool/main/m/mpfr4/mpfr4_4.0.2-1.debian.tar.xz' mpfr4_4.0.2-1.debian.tar.xz 10544 SHA256:99c4d35654f33340f0efdec67142a34753157b20334cadad9018f5eab29738da
```

### `dpkg` source package: `mpi-defaults=1.13`

Binary Packages:

- `mpi-default-bin=1.13`
- `mpi-default-dev=1.13`

Licenses: (parsed from: `/usr/share/doc/mpi-default-bin/copyright`, `/usr/share/doc/mpi-default-dev/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mpi-defaults=1.13
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mpi-defaults/mpi-defaults_1.13.dsc' mpi-defaults_1.13.dsc 2676 SHA256:f560a94c82299f54dcef2d55b50267d7ab687a53caad97da057b298947941f5f
'http://archive.ubuntu.com/ubuntu/pool/universe/m/mpi-defaults/mpi-defaults_1.13.tar.xz' mpi-defaults_1.13.tar.xz 5316 SHA256:e5caa05970444c22fbe435f90b27e09c4753ad4205e4c94383084dadf07600b1
```

### `dpkg` source package: `mysql-8.0=8.0.21-0ubuntu0.20.04.4`

Binary Packages:

- `libmysqlclient-dev=8.0.21-0ubuntu0.20.04.4`
- `libmysqlclient21:amd64=8.0.21-0ubuntu0.20.04.4`

Licenses: (parsed from: `/usr/share/doc/libmysqlclient-dev/copyright`, `/usr/share/doc/libmysqlclient21/copyright`)

- `Artistic`
- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-like`
- `Boost-1.0`
- `GPL-2`
- `GPL-2+`
- `ISC`
- `LGPL`
- `LGPL-2`
- `public-domain`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris mysql-8.0=8.0.21-0ubuntu0.20.04.4
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.21-0ubuntu0.20.04.4.dsc' mysql-8.0_8.0.21-0ubuntu0.20.04.4.dsc 3434 SHA512:0ce6053ba5a25c4d358bada6c1e09954844406063780898f312d26088599fb2fc95eaeffc03c0efb44bddc34a070ef4f7c2361c9268d32db539fa4894acaa390
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.21.orig.tar.gz' mysql-8.0_8.0.21.orig.tar.gz 278292192 SHA512:18128edd7d9604ea69bd308f372d6663ef3629503969148e3a2117175c4ef625358b31b96e0e1b8d10a87037719e3cb61d5c71eee1e26ab0e0a1731977a2d7c1
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-8.0/mysql-8.0_8.0.21-0ubuntu0.20.04.4.debian.tar.xz' mysql-8.0_8.0.21-0ubuntu0.20.04.4.debian.tar.xz 159588 SHA512:64d1b2abcb9d1fc12e498cce181f36eab97fdeb3cef07d22f310616d7fff22fd63ee112583875c6c567644f8461645c452c06d9e13532f24023a913f2d66a0b1
```

### `dpkg` source package: `mysql-defaults=1.0.5ubuntu2`

Binary Packages:

- `default-libmysqlclient-dev:amd64=1.0.5ubuntu2`
- `mysql-common=5.8+1.0.5ubuntu2`

Licenses: (parsed from: `/usr/share/doc/default-libmysqlclient-dev/copyright`, `/usr/share/doc/mysql-common/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris mysql-defaults=1.0.5ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.5ubuntu2.dsc' mysql-defaults_1.0.5ubuntu2.dsc 2251 SHA256:788762eca77d2718a5ecc8e5fc49f90b32e81639a4a06169789e8f34fc35d379
'http://archive.ubuntu.com/ubuntu/pool/main/m/mysql-defaults/mysql-defaults_1.0.5ubuntu2.tar.xz' mysql-defaults_1.0.5ubuntu2.tar.xz 7168 SHA256:d1b17de186bf8afba5cfc0041ab3c3646dbbed653e72010e2222bb52396e54c0
```

### `dpkg` source package: `ncurses=6.2-0ubuntu2`

Binary Packages:

- `libncurses6:amd64=6.2-0ubuntu2`
- `libncursesw6:amd64=6.2-0ubuntu2`
- `libtinfo6:amd64=6.2-0ubuntu2`
- `ncurses-base=6.2-0ubuntu2`
- `ncurses-bin=6.2-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris ncurses=6.2-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2-0ubuntu2.dsc' ncurses_6.2-0ubuntu2.dsc 3831 SHA256:b580e8d50864a61bad0cedb17c8005ec6c24cd85d8ebbe472d1170552c8cd3bd
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2.orig.tar.gz' ncurses_6.2.orig.tar.gz 3425862 SHA256:30306e0c76e0f9f1f0de987cf1c82a5c21e1ce6568b9227f7da5b71cbea86c9d
'http://archive.ubuntu.com/ubuntu/pool/main/n/ncurses/ncurses_6.2-0ubuntu2.debian.tar.xz' ncurses_6.2-0ubuntu2.debian.tar.xz 61192 SHA256:3377d203f2ab08b119ed22ac420152f3c28872201e35b25e62dfe07641ed750a
```

### `dpkg` source package: `netifaces=0.10.4-1ubuntu4`

Binary Packages:

- `python3-netifaces=0.10.4-1ubuntu4`

Licenses: (parsed from: `/usr/share/doc/python3-netifaces/copyright`)

- `MIT-style`

Source:

```console
$ apt-get source -qq --print-uris netifaces=0.10.4-1ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.10.4-1ubuntu4.dsc' netifaces_0.10.4-1ubuntu4.dsc 2399 SHA256:dd7c2e32b8139501ba16aa17000358b0ed8f0c6b44d4f5ed0372a891a0320c25
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.10.4.orig.tar.gz' netifaces_0.10.4.orig.tar.gz 22969 SHA256:9656a169cb83da34d732b0eb72b39373d48774aee009a3d1272b7ea2ce109cde
'http://archive.ubuntu.com/ubuntu/pool/main/n/netifaces/netifaces_0.10.4-1ubuntu4.debian.tar.xz' netifaces_0.10.4-1ubuntu4.debian.tar.xz 8596 SHA256:dffdb241c6c83c52fa2a975fc6291d5b004e2ae0b71d2b9daaeb704e3552951b
```

### `dpkg` source package: `nettle=3.5.1+really3.5.1-2`

Binary Packages:

- `libhogweed5:amd64=3.5.1+really3.5.1-2`
- `libnettle7:amd64=3.5.1+really3.5.1-2`

Licenses: (parsed from: `/usr/share/doc/libhogweed5/copyright`, `/usr/share/doc/libnettle7/copyright`)

- `GAP`
- `GPL`
- `GPL-2`
- `GPL-2+`
- `GPL-2+ with Autoconf exception`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1+`
- `other`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nettle=3.5.1+really3.5.1-2
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1-2.dsc' nettle_3.5.1+really3.5.1-2.dsc 2375 SHA256:a64c789e3997a2bba012e0c136de9c11b1bc95cf03069c35d26b00582481eecf
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1.orig.tar.gz' nettle_3.5.1+really3.5.1.orig.tar.gz 1989593 SHA256:75cca1998761b02e16f2db56da52992aef622bf55a3b45ec538bc2eedadc9419
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1.orig.tar.gz.asc' nettle_3.5.1+really3.5.1.orig.tar.gz.asc 573 SHA256:557116e471c7c4556148866b5cec056d6de5f26d080e5930154018be6a9d893e
'http://archive.ubuntu.com/ubuntu/pool/main/n/nettle/nettle_3.5.1+really3.5.1-2.debian.tar.xz' nettle_3.5.1+really3.5.1-2.debian.tar.xz 20044 SHA256:7e816adb06d13913bcd350ca6cb777230b82508ca2d358a4062e5676bf335529
```

### `dpkg` source package: `nghttp2=1.40.0-1build1`

Binary Packages:

- `libnghttp2-14:amd64=1.40.0-1build1`

Licenses: (parsed from: `/usr/share/doc/libnghttp2-14/copyright`)

- `BSD-2-clause`
- `Expat`
- `GPL-3`
- `GPL-3+ with autoconf exception`
- `MIT`
- `SIL-OFL-1.1`
- `all-permissive`

Source:

```console
$ apt-get source -qq --print-uris nghttp2=1.40.0-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.40.0-1build1.dsc' nghttp2_1.40.0-1build1.dsc 2572 SHA256:2f945c4799485cae7ad8f0d1cf1720986bf13f6c65bab7582ef2ae51a48e3661
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.40.0.orig.tar.bz2' nghttp2_1.40.0.orig.tar.bz2 1937537 SHA256:82758e13727945f2408d0612762e4655180b039f058d5ff40d055fa1497bd94f
'http://archive.ubuntu.com/ubuntu/pool/main/n/nghttp2/nghttp2_1.40.0-1build1.debian.tar.xz' nghttp2_1.40.0-1build1.debian.tar.xz 12772 SHA256:d71772f726b343c803954c0bccf3150b736d0e1a7c82a03dc7560fc8bd3a0189
```

### `dpkg` source package: `nose=1.3.7-5`

Binary Packages:

- `python3-nose=1.3.7-5`

Licenses: (parsed from: `/usr/share/doc/python3-nose/copyright`)

- `Expat`
- `LGPL`
- `LGPL-2`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris nose=1.3.7-5
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose/nose_1.3.7-5.dsc' nose_1.3.7-5.dsc 2274 SHA256:7437bda7b3c68f7178007193771f68336bcffa0315bf0d9770611e6cd272a0b5
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose/nose_1.3.7.orig.tar.gz' nose_1.3.7.orig.tar.gz 280488 SHA256:f1bffef9cbc82628f6e7d7b40d7e255aefaa1adb6a1b1d26c69a8b79e6208a98
'http://archive.ubuntu.com/ubuntu/pool/universe/n/nose/nose_1.3.7-5.debian.tar.xz' nose_1.3.7-5.debian.tar.xz 13360 SHA256:975c22696f30a96f955be8cab2c70744d5dc78b8930a3cc4c77f588fcab27c5d
```

### `dpkg` source package: `npth=1.6-1`

Binary Packages:

- `libnpth0:amd64=1.6-1`

Licenses: (parsed from: `/usr/share/doc/libnpth0/copyright`)

- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris npth=1.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-1.dsc' npth_1.6-1.dsc 1925 SHA256:2c327ce494f702482e79ed620445cba303c4449dd0768fecee3ee7d5ade2544a
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6.orig.tar.bz2' npth_1.6.orig.tar.bz2 300486 SHA256:1393abd9adcf0762d34798dc34fdcf4d0d22a8410721e76f1e3afcd1daa4e2d1
'http://archive.ubuntu.com/ubuntu/pool/main/n/npth/npth_1.6-1.debian.tar.xz' npth_1.6-1.debian.tar.xz 10532 SHA256:d312d4a3cf1d082e2f2cf3ea752c41d34f7e120f77a941c6c1680e6093834353
```

### `dpkg` source package: `numactl=2.0.12-1`

Binary Packages:

- `libnuma-dev:amd64=2.0.12-1`
- `libnuma1:amd64=2.0.12-1`

Licenses: (parsed from: `/usr/share/doc/libnuma-dev/copyright`, `/usr/share/doc/libnuma1/copyright`)

- `GPL`
- `LGPL`

Source:

```console
$ apt-get source -qq --print-uris numactl=2.0.12-1
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.12-1.dsc' numactl_2.0.12-1.dsc 2033 SHA256:3b308b110de0728c5524b3135d871e55ebb6e4b93cdc583e93c4222219fe4d08
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.12.orig.tar.gz' numactl_2.0.12.orig.tar.gz 421425 SHA256:2e67513a62168de4777da20d89cdab66d75bcd3badc4256f6b190a8111cd93f8
'http://archive.ubuntu.com/ubuntu/pool/main/n/numactl/numactl_2.0.12-1.debian.tar.xz' numactl_2.0.12-1.debian.tar.xz 6756 SHA256:966724cac8f309b33959ae9922b3e5ab58ea821e2e802d96425e1eaada639a33
```

### `dpkg` source package: `numpy=1:1.17.4-5ubuntu3`

Binary Packages:

- `python3-numpy=1:1.17.4-5ubuntu3`

Licenses: (parsed from: `/usr/share/doc/python3-numpy/copyright`)

- `BSD-3-Clause`
- `MIT`
- `PSF`
- `Public-Domain`

Source:

```console
$ apt-get source -qq --print-uris numpy=1:1.17.4-5ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/main/n/numpy/numpy_1.17.4-5ubuntu3.dsc' numpy_1.17.4-5ubuntu3.dsc 2707 SHA256:7ebf0eba678c742c22defa4c8bf6976547f5ef67f0fe2877fa974a9fca87c071
'http://archive.ubuntu.com/ubuntu/pool/main/n/numpy/numpy_1.17.4.orig.tar.xz' numpy_1.17.4.orig.tar.xz 3519384 SHA256:71c77538fe4cc950da6dbce8f9b4e28b5660f1c91b5fe8b8718b18ee2cc5dc2f
'http://archive.ubuntu.com/ubuntu/pool/main/n/numpy/numpy_1.17.4-5ubuntu3.debian.tar.xz' numpy_1.17.4-5ubuntu3.debian.tar.xz 30332 SHA256:fca32aaf9e7786f4055e3f5102e23d5604da93e141066617ee4b9309c8927210
```

### `dpkg` source package: `nvidia-settings=440.82-0ubuntu0.20.04.1`

Binary Packages:

- `libxnvctrl0:amd64=440.82-0ubuntu0.20.04.1`

Licenses: (parsed from: `/usr/share/doc/libxnvctrl0/copyright`)

- `Expat`
- `Expat-NVIDIA`
- `Expat-Precision`
- `Expat-RedHat`
- `GPL-2`
- `other-MetroLink`
- `other-Metrolink`
- `other-XFree`

Source:

```console
$ apt-get source -qq --print-uris nvidia-settings=440.82-0ubuntu0.20.04.1
'http://archive.ubuntu.com/ubuntu/pool/main/n/nvidia-settings/nvidia-settings_440.82-0ubuntu0.20.04.1.dsc' nvidia-settings_440.82-0ubuntu0.20.04.1.dsc 2480 SHA512:f8fa55761479290eef387aef2484cadd2f681faa676f2f5e063f2b819f38782203fb7386acbd9cb4d13335e95a97bae7c08c2b12b643c1435e0f813eb079963c
'http://archive.ubuntu.com/ubuntu/pool/main/n/nvidia-settings/nvidia-settings_440.82.orig.tar.bz2' nvidia-settings_440.82.orig.tar.bz2 1128498 SHA512:8f9b546f65a1bd17f6336df9e62b0d1403581d3f60276793a536ff39bf67038def1c2738545b24b04eb465860f0cb97b5b9688d7dfb759fda567c05b1cc651ff
'http://archive.ubuntu.com/ubuntu/pool/main/n/nvidia-settings/nvidia-settings_440.82-0ubuntu0.20.04.1.debian.tar.xz' nvidia-settings_440.82-0ubuntu0.20.04.1.debian.tar.xz 23976 SHA512:a1770bfe6aaa3161396be1a95e64be178df6e41d645b337b1b4457fbdad425667758d5d7d5678e7eb04bb16088e53a362a4fe7dbc298a049984db4ab2a0df7bc
```

### `dpkg` source package: `ocl-icd=2.2.11-1ubuntu1`

Binary Packages:

- `ocl-icd-libopencl1:amd64=2.2.11-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/ocl-icd-libopencl1/copyright`)

- `BSD-2-Clause`

Source:

```console
$ apt-get source -qq --print-uris ocl-icd=2.2.11-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/o/ocl-icd/ocl-icd_2.2.11-1ubuntu1.dsc' ocl-icd_2.2.11-1ubuntu1.dsc 2101 SHA256:e786ea5edf5223f3ad32fa4b8d9a4455507b376e45342954ec5b36b21cb4904d
'http://archive.ubuntu.com/ubuntu/pool/main/o/ocl-icd/ocl-icd_2.2.11.orig.tar.gz' ocl-icd_2.2.11.orig.tar.gz 455800 SHA256:02fa41da98ae2807e92742196831d320e3fc2f4cb1118d0061d9f51dda867730
'http://archive.ubuntu.com/ubuntu/pool/main/o/ocl-icd/ocl-icd_2.2.11-1ubuntu1.debian.tar.xz' ocl-icd_2.2.11-1ubuntu1.debian.tar.xz 11204 SHA256:2baece01c46beada400992cfcbe5b0facb822bae07bda5d98f1a7ad4d474415c
```

### `dpkg` source package: `openldap=2.4.49+dfsg-2ubuntu1.3`

Binary Packages:

- `libldap-2.4-2:amd64=2.4.49+dfsg-2ubuntu1.3`
- `libldap-common=2.4.49+dfsg-2ubuntu1.3`
- `libldap2-dev:amd64=2.4.49+dfsg-2ubuntu1.3`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openldap=2.4.49+dfsg-2ubuntu1.3
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.49+dfsg-2ubuntu1.3.dsc' openldap_2.4.49+dfsg-2ubuntu1.3.dsc 3136 SHA512:9227ca59255b2127521e2fbc3a575f4bea4d8ca11c402a4d3cf4b2fe60630981d236b5edb48024b5dda5083acecd3afb7c582552699fa8032655af54b2d28eff
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.49+dfsg.orig.tar.gz' openldap_2.4.49+dfsg.orig.tar.gz 4844726 SHA512:c2096f6e37bae8e4d4dcc5cc8dad783996bc8677e7e62a06b9f55857f8950726ca3e3b0d8368563c8985123175f63625354ad5ac271db8b55d3ac62e8906d4c7
'http://archive.ubuntu.com/ubuntu/pool/main/o/openldap/openldap_2.4.49+dfsg-2ubuntu1.3.debian.tar.xz' openldap_2.4.49+dfsg-2ubuntu1.3.debian.tar.xz 182112 SHA512:15a048d1e5ddcc78f022a661da81d5ed01ffd9aa23379310938a8bac05d4d2b58fe3c47baa3e453fad2c6d4dafcee82766e98de2e7940473fac77deff8f946a5
```

### `dpkg` source package: `openmpi=4.0.3-0ubuntu1`

Binary Packages:

- `libopenmpi-dev:amd64=4.0.3-0ubuntu1`
- `libopenmpi3:amd64=4.0.3-0ubuntu1`
- `openmpi-bin=4.0.3-0ubuntu1`
- `openmpi-common=4.0.3-0ubuntu1`

Licenses: (parsed from: `/usr/share/doc/libopenmpi-dev/copyright`, `/usr/share/doc/libopenmpi3/copyright`, `/usr/share/doc/openmpi-bin/copyright`, `/usr/share/doc/openmpi-common/copyright`)

- `LGPL-2`

Source:

```console
$ apt-get source -qq --print-uris openmpi=4.0.3-0ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openmpi/openmpi_4.0.3-0ubuntu1.dsc' openmpi_4.0.3-0ubuntu1.dsc 2734 SHA256:a844e15b618c79b6affc72f7055860c93ac32554a53b03477712b25332c8639c
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openmpi/openmpi_4.0.3.orig.tar.xz' openmpi_4.0.3.orig.tar.xz 6591016 SHA256:1c28d029f4bd296a812d96fa9c959b02b8f5b528129bd49f5a7a209f11949122
'http://archive.ubuntu.com/ubuntu/pool/universe/o/openmpi/openmpi_4.0.3-0ubuntu1.debian.tar.xz' openmpi_4.0.3-0ubuntu1.debian.tar.xz 63360 SHA256:1ec55ff89ea12820c4349a0fd22638e71ece3003fae5f31902779dec9498a394
```

### `dpkg` source package: `openssh=1:8.2p1-4ubuntu0.1`

Binary Packages:

- `openssh-client=1:8.2p1-4ubuntu0.1`

Licenses: (parsed from: `/usr/share/doc/openssh-client/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Beer-ware`
- `Expat-with-advertising-restriction`
- `Mazieres-BSD-style`
- `OpenSSH`
- `Powell-BSD-style`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris openssh=1:8.2p1-4ubuntu0.1
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.2p1-4ubuntu0.1.dsc' openssh_8.2p1-4ubuntu0.1.dsc 3098 SHA512:0e51e026137b7e93d36167da66b8135e722f90cfc7d3a648336dab728f71e74988d1605bb73c788f1cf01161ceed7120a21a07c49e540c8ea16db853e496c51f
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.2p1.orig.tar.gz' openssh_8.2p1.orig.tar.gz 1701197 SHA512:c4db64e52a3a4c410de9de49f9cb104dd493b10250af3599b92457dd986277b3fd99a6f51cec94892fd1be5bd0369c5757262ea7805f0de464b245c3d34c120a
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssh/openssh_8.2p1-4ubuntu0.1.debian.tar.xz' openssh_8.2p1-4ubuntu0.1.debian.tar.xz 174784 SHA512:cca56b046669198489802c00d495b507f5a47b2f92b80f8e073eeae199bf2f5948078feefd2aaa9eeaec6ec93a8bebc7a68db6c0bc43bcb5325e43a9b4bc8ebe
```

### `dpkg` source package: `openssl=1.1.1f-1ubuntu2`

Binary Packages:

- `libssl-dev:amd64=1.1.1f-1ubuntu2`
- `libssl1.1:amd64=1.1.1f-1ubuntu2`
- `openssl=1.1.1f-1ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris openssl=1.1.1f-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f-1ubuntu2.dsc' openssl_1.1.1f-1ubuntu2.dsc 2705 SHA256:2704b83cc9f62d3ff30bff22a032b543620ade054da30c600fd0e2385c8d7c1b
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f.orig.tar.gz' openssl_1.1.1f.orig.tar.gz 9792828 SHA256:186c6bfe6ecfba7a5b48c47f8a1673d0f3b0e5ba2e25602dd23b629975da3f35
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f.orig.tar.gz.asc' openssl_1.1.1f.orig.tar.gz.asc 488 SHA256:e9c68097b05be8873e41bd33a9269378ca58e515fbaa30a512c315b602d41dda
'http://archive.ubuntu.com/ubuntu/pool/main/o/openssl/openssl_1.1.1f-1ubuntu2.debian.tar.xz' openssl_1.1.1f-1ubuntu2.debian.tar.xz 141644 SHA256:2a2709358bc19e4f8a1f23e25c8457c1d4c69a78d47aa4fc8dbda14545a8ec5e
```

### `dpkg` source package: `p11-kit=0.23.20-1build1`

Binary Packages:

- `libp11-kit0:amd64=0.23.20-1build1`

Licenses: (parsed from: `/usr/share/doc/libp11-kit0/copyright`)

- `BSD-3-Clause`
- `ISC`
- `ISC+IBM`
- `permissive-like-automake-output`
- `same-as-rest-of-p11kit`

Source:

```console
$ apt-get source -qq --print-uris p11-kit=0.23.20-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.20-1build1.dsc' p11-kit_0.23.20-1build1.dsc 2466 SHA256:25b3e4f00439457152fa958f1b54e0222fbb98585aa174308b6d6534b94445c3
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.20.orig.tar.xz' p11-kit_0.23.20.orig.tar.xz 822588 SHA256:14d86024c3dfd6b967d9bc0b4ec7b2973014fe7423481f4d230a1a63b8aa6104
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.20.orig.tar.xz.asc' p11-kit_0.23.20.orig.tar.xz.asc 854 SHA256:6429a15c3c071629add6712ed75916df90043d47250edb9235d89ee197f613b8
'http://archive.ubuntu.com/ubuntu/pool/main/p/p11-kit/p11-kit_0.23.20-1build1.debian.tar.xz' p11-kit_0.23.20-1build1.debian.tar.xz 22004 SHA256:c43279d68adc9f710ff438f7084316e1e3ca9918f7c653bf1cb932927c415960
```

### `dpkg` source package: `pam=1.3.1-5ubuntu4.1`

Binary Packages:

- `libpam-modules:amd64=1.3.1-5ubuntu4.1`
- `libpam-modules-bin=1.3.1-5ubuntu4.1`
- `libpam-runtime=1.3.1-5ubuntu4.1`
- `libpam0g:amd64=1.3.1-5ubuntu4.1`

Licenses: (parsed from: `/usr/share/doc/libpam-modules/copyright`, `/usr/share/doc/libpam-modules-bin/copyright`, `/usr/share/doc/libpam-runtime/copyright`, `/usr/share/doc/libpam0g/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pam=1.3.1-5ubuntu4.1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu4.1.dsc' pam_1.3.1-5ubuntu4.1.dsc 2707 SHA512:0fe1765785d9642b9dac56a5e0db8ebbbe2ce82d91cb92c8f050fe066d5c5e742a3562fab0a1f3618707052b2a813c08cb398fa6cf6900866286b3fdfe6e4214
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1.orig.tar.xz' pam_1.3.1.orig.tar.xz 912332 SHA512:6bc8e2a5b64686f0a23846221c5228c88418ba485b17c53b3a12f91262b5bb73566d6b6a5daa1f63bbae54310aee918b987e44a72ce809b4e7c668f0fadfe08e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pam/pam_1.3.1-5ubuntu4.1.debian.tar.xz' pam_1.3.1-5ubuntu4.1.debian.tar.xz 159852 SHA512:f43e7b4bfb1fe42d29099dc404e8b50a661acf8f53b3183ec3fdacc09946b7742a5b70387cde7728557199cb5914e39a330106176d406fcd51b79ecd7e479336
```

### `dpkg` source package: `paramiko=2.6.0-2`

Binary Packages:

- `python3-paramiko=2.6.0-2`

Licenses: (parsed from: `/usr/share/doc/python3-paramiko/copyright`)

- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris paramiko=2.6.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/paramiko/paramiko_2.6.0-2.dsc' paramiko_2.6.0-2.dsc 2340 SHA256:39621e677776d75e18912df8900617666c77b63d408a106437ccbb5edf37ff3c
'http://archive.ubuntu.com/ubuntu/pool/main/p/paramiko/paramiko_2.6.0.orig.tar.xz' paramiko_2.6.0.orig.tar.xz 678604 SHA256:b969d9c9590b6ef6f40520fef2fd11337cfa81a7b5101676f916d12c855f33d9
'http://archive.ubuntu.com/ubuntu/pool/main/p/paramiko/paramiko_2.6.0-2.debian.tar.xz' paramiko_2.6.0-2.debian.tar.xz 8108 SHA256:eb33e5575eb3aa1f01969cb0dcd8ff28494481c65bc950a771fa4a0ad63fe55c
```

### `dpkg` source package: `patch=2.7.6-6`

Binary Packages:

- `patch=2.7.6-6`

Licenses: (parsed from: `/usr/share/doc/patch/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris patch=2.7.6-6
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-6.dsc' patch_2.7.6-6.dsc 1699 SHA256:ad31c243b982ad8dede14f7b4dfe5bb798bb1dc6d4e28c51a797c3af58477c13
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6.orig.tar.xz' patch_2.7.6.orig.tar.xz 783756 SHA256:ac610bda97abe0d9f6b7c963255a11dcb196c25e337c61f94e4778d632f1d8fd
'http://archive.ubuntu.com/ubuntu/pool/main/p/patch/patch_2.7.6-6.debian.tar.xz' patch_2.7.6-6.debian.tar.xz 14464 SHA256:75ea94b265763b65005381f1eceeaf3351a70ec5c3243bc161d702776414db02
```

### `dpkg` source package: `pcre2=10.34-7`

Binary Packages:

- `libpcre2-8-0:amd64=10.34-7`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre2=10.34-7
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34-7.dsc' pcre2_10.34-7.dsc 2286 SHA256:c3e2bfd8fabf594238b3f17074dc8ac483aaf80a9f12dbfe927b80a74558732e
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34.orig.tar.gz' pcre2_10.34.orig.tar.gz 2271533 SHA256:da6aba7ba2509e918e41f4f744a59fa41a2425c59a298a232e7fe85691e00379
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre2/pcre2_10.34-7.diff.gz' pcre2_10.34-7.diff.gz 7068 SHA256:7d44ac1b171ef7f7051213a3a8505b28f3809ed3e2fb348567a29fdf5f2b5fdf
```

### `dpkg` source package: `pcre3=2:8.39-12build1`

Binary Packages:

- `libpcre16-3:amd64=2:8.39-12build1`
- `libpcre3:amd64=2:8.39-12build1`
- `libpcre3-dev:amd64=2:8.39-12build1`
- `libpcre32-3:amd64=2:8.39-12build1`
- `libpcrecpp0v5:amd64=2:8.39-12build1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pcre3=2:8.39-12build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-12build1.dsc' pcre3_8.39-12build1.dsc 2133 SHA256:e1dd0e352e5ba90aa89016dc3ad8b5990c1a8743c1550c613c7a9d9079a2da67
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39.orig.tar.bz2' pcre3_8.39.orig.tar.bz2 1560758 SHA256:b858099f82483031ee02092711689e7245586ada49e534a06e678b8ea9549e8b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pcre3/pcre3_8.39-12build1.debian.tar.gz' pcre3_8.39-12build1.debian.tar.gz 26478 SHA256:8f92c016f9200aad9a9028bbd96eded68394c756b09df76db2c0a54e8a1802c6
```

### `dpkg` source package: `perl=5.30.0-9build1`

Binary Packages:

- `libperl5.30:amd64=5.30.0-9build1`
- `perl=5.30.0-9build1`
- `perl-base=5.30.0-9build1`
- `perl-modules-5.30=5.30.0-9build1`

Licenses: (parsed from: `/usr/share/doc/libperl5.30/copyright`, `/usr/share/doc/perl/copyright`, `/usr/share/doc/perl-base/copyright`, `/usr/share/doc/perl-modules-5.30/copyright`)

- `Artistic`
- `Artistic,`
- `Artistic-2`
- `Artistic-dist`
- `BSD-3-clause`
- `BSD-3-clause-GENERIC`
- `BSD-3-clause-with-weird-numbering`
- `BSD-4-clause-POWERDOG`
- `BZIP`
- `CC0-1.0`
- `DONT-CHANGE-THE-GPL`
- `Expat`
- `GPL-1`
- `GPL-1+`
- `GPL-2`
- `GPL-2+`
- `GPL-3+-WITH-BISON-EXCEPTION`
- `HSIEH-BSD`
- `HSIEH-DERIVATIVE`
- `LGPL-2.1`
- `REGCOMP`
- `REGCOMP,`
- `RRA-KEEP-THIS-NOTICE`
- `SDBM-PUBLIC-DOMAIN`
- `TEXT-TABS`
- `Unicode`
- `ZLIB`

Source:

```console
$ apt-get source -qq --print-uris perl=5.30.0-9build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.0-9build1.dsc' perl_5.30.0-9build1.dsc 2896 SHA256:11a7a3cf75fe92fd8ea4469ff836c6372f7f17b20fad44d009495c9cf44480cd
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.0.orig-regen-configure.tar.gz' perl_5.30.0.orig-regen-configure.tar.gz 833235 SHA256:fc55a7309f9e2c404119b005774fc85a8488bad047aee611d17bbe2d608bf4de
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.0.orig.tar.xz' perl_5.30.0.orig.tar.xz 12419868 SHA256:ac501cad4af904d33370a9ea39dbb7a8ad4cb19bc7bc8a9c17d8dc3e81ef6306
'http://archive.ubuntu.com/ubuntu/pool/main/p/perl/perl_5.30.0-9build1.debian.tar.xz' perl_5.30.0-9build1.debian.tar.xz 161952 SHA256:74258880aa63b6248f9b2eba432dd08a8d72a9bbaeed40cd5070f73ca9d6ffeb
```

### `dpkg` source package: `pinentry=1.1.0-3build1`

Binary Packages:

- `pinentry-curses=1.1.0-3build1`

Licenses: (parsed from: `/usr/share/doc/pinentry-curses/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-3`
- `LGPL-3+`
- `X11`

Source:

```console
$ apt-get source -qq --print-uris pinentry=1.1.0-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-3build1.dsc' pinentry_1.1.0-3build1.dsc 2714 SHA256:69f7f343287886eebadb94177767d9aa74890d9f8420e3ab254803fcd21852bf
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0.orig.tar.bz2' pinentry_1.1.0.orig.tar.bz2 467702 SHA256:68076686fa724a290ea49cdf0d1c0c1500907d1b759a3bcbfbec0293e8f56570
'http://archive.ubuntu.com/ubuntu/pool/main/p/pinentry/pinentry_1.1.0-3build1.debian.tar.xz' pinentry_1.1.0-3build1.debian.tar.xz 17224 SHA256:2a11ee552389ba0499d6a9e1bfc38ee65a28bb97758832b982bbede68d2cb1b9
```

### `dpkg` source package: `pkg-config=0.29.1-0ubuntu4`

Binary Packages:

- `pkg-config=0.29.1-0ubuntu4`

Licenses: (parsed from: `/usr/share/doc/pkg-config/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris pkg-config=0.29.1-0ubuntu4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu4.dsc' pkg-config_0.29.1-0ubuntu4.dsc 1799 SHA256:d60186d733ce808c04a0afeb4b6790161f4ffc5bae6a26a566eab047a31ef2dc
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1.orig.tar.gz' pkg-config_0.29.1.orig.tar.gz 2013454 SHA256:beb43c9e064555469bd4390dcfd8030b1536e0aa103f08d7abf7ae8cac0cb001
'http://archive.ubuntu.com/ubuntu/pool/main/p/pkg-config/pkg-config_0.29.1-0ubuntu4.diff.gz' pkg-config_0.29.1-0ubuntu4.diff.gz 9373 SHA256:ac6d503134b8fbaca066aa3dea622c69a58e8845896ffd75066d14de27a41d58
```

### `dpkg` source package: `pmix=3.1.5-1`

Binary Packages:

- `libpmix2:amd64=3.1.5-1`

Licenses: (parsed from: `/usr/share/doc/libpmix2/copyright`)

- `GPL-2`
- `LGPL-2`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris pmix=3.1.5-1
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pmix/pmix_3.1.5-1.dsc' pmix_3.1.5-1.dsc 2167 SHA256:16790a9b6afcaa54d21f50ca8dcc8d181e75754e2d43565ee0a5d6d75b78e324
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pmix/pmix_3.1.5.orig.tar.xz' pmix_3.1.5.orig.tar.xz 665580 SHA256:af74f9bc175343ee6472848aedbe0b31b299645882b05a0bc8d354e8d403d91e
'http://archive.ubuntu.com/ubuntu/pool/universe/p/pmix/pmix_3.1.5-1.debian.tar.xz' pmix_3.1.5-1.debian.tar.xz 7656 SHA256:84150e848320f8d8c87f987f99f05ba19ec942d711385fff1f0e2ec6c9af9936
```

### `dpkg` source package: `poco=1.9.2-3ubuntu3`

Binary Packages:

- `libpoco-dev=1.9.2-3ubuntu3`
- `libpococrypto62:amd64=1.9.2-3ubuntu3`
- `libpocodata62:amd64=1.9.2-3ubuntu3`
- `libpocodatamysql62:amd64=1.9.2-3ubuntu3`
- `libpocodataodbc62:amd64=1.9.2-3ubuntu3`
- `libpocodatasqlite62:amd64=1.9.2-3ubuntu3`
- `libpocoencodings62:amd64=1.9.2-3ubuntu3`
- `libpocofoundation62:amd64=1.9.2-3ubuntu3`
- `libpocojson62:amd64=1.9.2-3ubuntu3`
- `libpocomongodb62:amd64=1.9.2-3ubuntu3`
- `libpoconet62:amd64=1.9.2-3ubuntu3`
- `libpoconetssl62:amd64=1.9.2-3ubuntu3`
- `libpocoredis62:amd64=1.9.2-3ubuntu3`
- `libpocoutil62:amd64=1.9.2-3ubuntu3`
- `libpocoxml62:amd64=1.9.2-3ubuntu3`
- `libpocozip62:amd64=1.9.2-3ubuntu3`

Licenses: (parsed from: `/usr/share/doc/libpoco-dev/copyright`, `/usr/share/doc/libpococrypto62/copyright`, `/usr/share/doc/libpocodata62/copyright`, `/usr/share/doc/libpocodatamysql62/copyright`, `/usr/share/doc/libpocodataodbc62/copyright`, `/usr/share/doc/libpocodatasqlite62/copyright`, `/usr/share/doc/libpocoencodings62/copyright`, `/usr/share/doc/libpocofoundation62/copyright`, `/usr/share/doc/libpocojson62/copyright`, `/usr/share/doc/libpocomongodb62/copyright`, `/usr/share/doc/libpoconet62/copyright`, `/usr/share/doc/libpoconetssl62/copyright`, `/usr/share/doc/libpocoredis62/copyright`, `/usr/share/doc/libpocoutil62/copyright`, `/usr/share/doc/libpocoxml62/copyright`, `/usr/share/doc/libpocozip62/copyright`)

- `BSD-3-clause`
- `BSL-1.0`
- `Expat`
- `MIT`
- `RSA-MD`
- `Zlib`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris poco=1.9.2-3ubuntu3
'http://archive.ubuntu.com/ubuntu/pool/universe/p/poco/poco_1.9.2-3ubuntu3.dsc' poco_1.9.2-3ubuntu3.dsc 3022 SHA256:0fd058a3c9b4d61036dc5d8d2dc8caa7bb630c2afbf8475fab97994522a73f37
'http://archive.ubuntu.com/ubuntu/pool/universe/p/poco/poco_1.9.2.orig.tar.bz2' poco_1.9.2.orig.tar.bz2 5327129 SHA256:74f117e2c6c0f2de1e4ffd6fc5b8053a7bc05d331e7a7c606d0fcc3917f827a4
'http://archive.ubuntu.com/ubuntu/pool/universe/p/poco/poco_1.9.2-3ubuntu3.debian.tar.xz' poco_1.9.2-3ubuntu3.debian.tar.xz 17572 SHA256:613bde63152c6892f51c13fdc6096dd803fc224da59a98e47bc93f0341c07a3b
```

### `dpkg` source package: `procps=2:3.3.16-1ubuntu2`

Binary Packages:

- `libprocps8:amd64=2:3.3.16-1ubuntu2`
- `procps=2:3.3.16-1ubuntu2`

Licenses: (parsed from: `/usr/share/doc/libprocps8/copyright`, `/usr/share/doc/procps/copyright`)

- `GPL-2`
- `GPL-2.0+`
- `LGPL-2`
- `LGPL-2.0+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris procps=2:3.3.16-1ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16-1ubuntu2.dsc' procps_3.3.16-1ubuntu2.dsc 2248 SHA256:1cd439a6bd527ab1d676fb6d0119cc825d4f7990b8b0f1daeaaad566925ab830
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16.orig.tar.xz' procps_3.3.16.orig.tar.xz 621892 SHA256:2919299e579d29be3501a802dfe77e6f23be228149d0396d83d0ffbe8fa7efbf
'http://archive.ubuntu.com/ubuntu/pool/main/p/procps/procps_3.3.16-1ubuntu2.debian.tar.xz' procps_3.3.16-1ubuntu2.debian.tar.xz 32916 SHA256:eb4d6806dbcf8ab69c4913c50d04f9d99e95f02dab82bda80140abd85d27d5b7
```

### `dpkg` source package: `pycryptodome=3.6.1-2build4`

Binary Packages:

- `python3-pycryptodome=3.6.1-2build4`

Licenses: (parsed from: `/usr/share/doc/python3-pycryptodome/copyright`)

- `BSD-2-clause`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris pycryptodome=3.6.1-2build4
'http://archive.ubuntu.com/ubuntu/pool/main/p/pycryptodome/pycryptodome_3.6.1-2build4.dsc' pycryptodome_3.6.1-2build4.dsc 2385 SHA256:8af50ee7bcc20e2c7ce46700f87f7f6c5f5d19964adb9b96179ce20197f0f355
'http://archive.ubuntu.com/ubuntu/pool/main/p/pycryptodome/pycryptodome_3.6.1.orig.tar.gz' pycryptodome_3.6.1.orig.tar.gz 7167199 SHA256:15013007e393d0cc0e69f4329a47c4c8597b7f3d02c12c03f805405542f70c71
'http://archive.ubuntu.com/ubuntu/pool/main/p/pycryptodome/pycryptodome_3.6.1-2build4.debian.tar.xz' pycryptodome_3.6.1-2build4.debian.tar.xz 10132 SHA256:8406b18b6889c652bc9a57e0527896848de96089e4718656a1535e64bdfb7ebb
```

### `dpkg` source package: `pyparsing=2.4.6-1`

Binary Packages:

- `python3-pyparsing=2.4.6-1`

Licenses: (parsed from: `/usr/share/doc/python3-pyparsing/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `Expat`
- `GPL-2`
- `GPL-3`
- `ellis-and-grant`
- `salvolainen`

Source:

```console
$ apt-get source -qq --print-uris pyparsing=2.4.6-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyparsing/pyparsing_2.4.6-1.dsc' pyparsing_2.4.6-1.dsc 2436 SHA256:53f7f9804c8d98bce52495ee7b744f5224eec54639fb2f6422a5d9ffec14eccd
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyparsing/pyparsing_2.4.6.orig.tar.gz' pyparsing_2.4.6.orig.tar.gz 649181 SHA256:4c830582a84fb022400b85429791bc551f1f4871c33f23e44f353119e92f969f
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyparsing/pyparsing_2.4.6-1.debian.tar.xz' pyparsing_2.4.6-1.debian.tar.xz 7748 SHA256:83ea6c57f8c1057b08e4c2e3b637017ec9f27da5c7216d75c6a0aa5dea242fba
```

### `dpkg` source package: `python-bcrypt=3.1.7-2ubuntu1`

Binary Packages:

- `python3-bcrypt=3.1.7-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/python3-bcrypt/copyright`)

- `Apache-2.0`
- `BSD-3-Clause`
- `BSD-4-Clause`
- `GPL-3`
- `GPL-3+`
- `ISC`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris python-bcrypt=3.1.7-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-bcrypt/python-bcrypt_3.1.7-2ubuntu1.dsc' python-bcrypt_3.1.7-2ubuntu1.dsc 2407 SHA256:06551ca9a8e09c69e153d8dcd2371426d0b1738d9a054f178d2e283be3109abb
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-bcrypt/python-bcrypt_3.1.7.orig.tar.xz' python-bcrypt_3.1.7.orig.tar.xz 34056 SHA256:9f2a25ec9e7df6dc448787df6a540b779e1f86445bf3c325043810bcc43a2d2b
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-bcrypt/python-bcrypt_3.1.7-2ubuntu1.debian.tar.xz' python-bcrypt_3.1.7-2ubuntu1.debian.tar.xz 14556 SHA256:12b3644b271f1e9c94a0dc538a92ea0d54262bd78c55c1db708beb5b62086500
```

### `dpkg` source package: `python-cffi=1.14.0-1build1`

Binary Packages:

- `python3-cffi-backend=1.14.0-1build1`

Licenses: (parsed from: `/usr/share/doc/python3-cffi-backend/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-cffi=1.14.0-1build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cffi/python-cffi_1.14.0-1build1.dsc' python-cffi_1.14.0-1build1.dsc 2919 SHA256:3ff41ebda23cbbc0e37c7fd324d8ba886a4371765732b365a3204d7fb53f9042
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cffi/python-cffi_1.14.0.orig.tar.gz' python-cffi_1.14.0.orig.tar.gz 463065 SHA256:2d384f4a127a15ba701207f7639d94106693b6cd64173d6c8988e2c25f3ac2b6
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cffi/python-cffi_1.14.0-1build1.debian.tar.xz' python-cffi_1.14.0-1build1.debian.tar.xz 6600 SHA256:1ad7f828cb4391776041edfba5182c2df03982401fc647dce43e73e24dfaa566
```

### `dpkg` source package: `python-cryptography=2.8-3`

Binary Packages:

- `python3-cryptography=2.8-3`

Licenses: (parsed from: `/usr/share/doc/python3-cryptography/copyright`)

- `Apache`
- `Apache-2.0`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris python-cryptography=2.8-3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cryptography/python-cryptography_2.8-3.dsc' python-cryptography_2.8-3.dsc 3517 SHA256:5606b9c1b44f97b5bf4c73a302a7b8fc2132ca4b832f8f0c653209dd32b4ae71
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cryptography/python-cryptography_2.8.orig.tar.gz' python-cryptography_2.8.orig.tar.gz 504516 SHA256:3cda1f0ed8747339bbdf71b9f38ca74c7b592f24f65cdb3ab3765e4b02871651
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-cryptography/python-cryptography_2.8-3.debian.tar.xz' python-cryptography_2.8-3.debian.tar.xz 11384 SHA256:52e7dded4e29db2272c047ce4ef46c56b816ae28e4cb4cfddadf160f6efcada0
```

### `dpkg` source package: `python-dateutil=2.7.3-3ubuntu1`

Binary Packages:

- `python3-dateutil=2.7.3-3ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python-dateutil=2.7.3-3ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.7.3-3ubuntu1.dsc' python-dateutil_2.7.3-3ubuntu1.dsc 2486 SHA256:7f2eb996853d7e06d2cffdf7f67f7893bb6ea351d3ee352596db70b855254c90
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.7.3.orig.tar.gz' python-dateutil_2.7.3.orig.tar.gz 302871 SHA256:e27001de32f627c22380a688bcc43ce83504a7bc5da472209b4c70f02829f0b8
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.7.3.orig.tar.gz.asc' python-dateutil_2.7.3.orig.tar.gz.asc 833 SHA256:95caabf7dc886ac18900896e0aa1b30f9cf1a44461fb780acffe130b37ee5047
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-dateutil/python-dateutil_2.7.3-3ubuntu1.debian.tar.xz' python-dateutil_2.7.3-3ubuntu1.debian.tar.xz 13988 SHA256:39ad4bfff2dc3167de320fd181e204ee19206807c6ad7c9a2642ef53398c8c48
```

### `dpkg` source package: `python-distro=1.4.0-1`

Binary Packages:

- `python3-distro=1.4.0-1`

Licenses: (parsed from: `/usr/share/doc/python3-distro/copyright`)

- `Apache-2.0`

Source:

```console
$ apt-get source -qq --print-uris python-distro=1.4.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-distro/python-distro_1.4.0-1.dsc' python-distro_1.4.0-1.dsc 2087 SHA256:6bbd33b1e8512e3a57de77242d6688ee9df6a1ed62b2aca545b608708d9e9064
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-distro/python-distro_1.4.0.orig.tar.gz' python-distro_1.4.0.orig.tar.gz 53719 SHA256:362dde65d846d23baee4b5c058c8586f219b5a54be1cf5fc6ff55c4578392f57
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-distro/python-distro_1.4.0-1.debian.tar.xz' python-distro_1.4.0-1.debian.tar.xz 2784 SHA256:ac87fa42e0a37aeec87a988982725ca3c567dd687e7bfbfd1cff86167066b891
```

### `dpkg` source package: `python-docutils=0.16+dfsg-2`

Binary Packages:

- `docutils-common=0.16+dfsg-2`
- `python3-docutils=0.16+dfsg-2`

Licenses: (parsed from: `/usr/share/doc/docutils-common/copyright`, `/usr/share/doc/python3-docutils/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `GPL-3`
- `GPL-3+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `Python-2.1.1`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris python-docutils=0.16+dfsg-2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.16+dfsg-2.dsc' python-docutils_0.16+dfsg-2.dsc 2526 SHA256:8b2368732cba4c0d1005a6c654a1ee752c55ea9f2ec96ebee9423774b08609c2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.16+dfsg.orig.tar.xz' python-docutils_0.16+dfsg.orig.tar.xz 1347300 SHA256:eee46a039937dd648a03a534647cdbb2370b288076e12d9e330a3fe8ef66781e
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-docutils/python-docutils_0.16+dfsg-2.debian.tar.xz' python-docutils_0.16+dfsg-2.debian.tar.xz 31004 SHA256:9dfaaf463e199f9568eee750e153f6e747a51a8ea642c5d668acf04e068c8699
```

### `dpkg` source package: `python-gnupg=0.4.5-2`

Binary Packages:

- `python3-gnupg=0.4.5-2`

Licenses: (parsed from: `/usr/share/doc/python3-gnupg/copyright`)

- `BSD-3-clause`
- `pycrypto`

Source:

```console
$ apt-get source -qq --print-uris python-gnupg=0.4.5-2
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-gnupg/python-gnupg_0.4.5-2.dsc' python-gnupg_0.4.5-2.dsc 2033 SHA256:3fe52d3aff364dfa5fb982deefb3065de552ac79a61ac79b836cccdaee92ccd4
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-gnupg/python-gnupg_0.4.5.orig.tar.gz' python-gnupg_0.4.5.orig.tar.gz 48792 SHA256:3353e59949cd2c15efbf1fca45e347d8a22f4bed0d93e9b89b2657bda19cec05
'http://archive.ubuntu.com/ubuntu/pool/universe/p/python-gnupg/python-gnupg_0.4.5-2.debian.tar.xz' python-gnupg_0.4.5-2.debian.tar.xz 7480 SHA256:1268d47768e7a2f5998dfd7f4e0a154ab1ee2ff2ede914b8c4d603fc48f7e4b3
```

### `dpkg` source package: `python-nacl=1.3.0-5`

Binary Packages:

- `python3-nacl=1.3.0-5`

Licenses: (parsed from: `/usr/share/doc/python3-nacl/copyright`)

- `Apache`
- `Apache-2.0`
- `Expat`
- `ISC`

Source:

```console
$ apt-get source -qq --print-uris python-nacl=1.3.0-5
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-nacl/python-nacl_1.3.0-5.dsc' python-nacl_1.3.0-5.dsc 2466 SHA256:010f8420812e280f3b32d65a2765b4d210d9426a75542ff2e2e516346d0e41c3
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-nacl/python-nacl_1.3.0.orig.tar.gz' python-nacl_1.3.0.orig.tar.gz 3351016 SHA256:0c6100edd16fefd1557da078c7a31e7b7d7a52ce39fdca2bec29d4f7b6e7600c
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-nacl/python-nacl_1.3.0-5.debian.tar.xz' python-nacl_1.3.0-5.debian.tar.xz 41116 SHA256:e7bd93414a20e972923a04d850cb1951a56f07eefd92389333a5b1254d61fcd4
```

### `dpkg` source package: `python-roman=2.0.0-3build1`

Binary Packages:

- `python3-roman=2.0.0-3build1`

Licenses: (parsed from: `/usr/share/doc/python3-roman/copyright`)

- `Python-2.1.1`
- `ZPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris python-roman=2.0.0-3build1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_2.0.0-3build1.dsc' python-roman_2.0.0-3build1.dsc 2181 SHA256:cefa55af9e933a8b3d83359de500e170197320a2cdb3b4edaa2f9a7334e4d46b
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_2.0.0.orig.tar.gz' python-roman_2.0.0.orig.tar.gz 4968 SHA256:98f2c0fb3cdcfba465d12c85b3b7139fc4cd2177f1325f1bacfe00878c8fa7b9
'http://archive.ubuntu.com/ubuntu/pool/main/p/python-roman/python-roman_2.0.0-3build1.debian.tar.xz' python-roman_2.0.0-3build1.debian.tar.xz 8680 SHA256:cf58cd8ac44d22da2aa0ad79957a4175b09552b4dd213c05fda34cde098584dc
```

### `dpkg` source package: `python3-catkin-pkg-modules=0.4.22-1`

Binary Packages:

- `python3-catkin-pkg-modules=0.4.22-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python3-catkin-pkg=0.4.22-100`

Binary Packages:

- `python3-catkin-pkg=0.4.22-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python3-defaults=3.8.2-0ubuntu2`

Binary Packages:

- `libpython3-dev:amd64=3.8.2-0ubuntu2`
- `libpython3-stdlib:amd64=3.8.2-0ubuntu2`
- `python3=3.8.2-0ubuntu2`
- `python3-dev=3.8.2-0ubuntu2`
- `python3-minimal=3.8.2-0ubuntu2`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-defaults=3.8.2-0ubuntu2
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.8.2-0ubuntu2.dsc' python3-defaults_3.8.2-0ubuntu2.dsc 2879 SHA256:3fa296ea2cd52738ebc44a1b83a8df500bf654356336d9bf057144171fe9ee7d
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-defaults/python3-defaults_3.8.2-0ubuntu2.tar.gz' python3-defaults_3.8.2-0ubuntu2.tar.gz 138226 SHA256:e4969a54306421ebfd195d0c064935db7c53f9f152d8abaae63da33819235e9a
```

### `dpkg` source package: `python3-rosdep-modules=0.19.0-1`

Binary Packages:

- `python3-rosdep-modules=0.19.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rosdep-modules=0.19.0-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rosdep-modules/python3-rosdep-modules_0.19.0-1.debian.tar.xz' python3-rosdep-modules_0.19.0-1.debian.tar.xz 2040 SHA512:99a49889a4e362334cf1b3f33e3029a184b98797ab49e4f532fb943ec08eff5dd48103f1b2a8d9d01f909b871938e10550b101369041505e093132076a968ee8
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rosdep-modules/python3-rosdep-modules_0.19.0-1.dsc' python3-rosdep-modules_0.19.0-1.dsc 960 SHA512:1bfbac504506c4d7b1c0a6ddfeda2f6de65e0eaeeddfbe2e7f81f3ee0309e8d9b5f0bc58d819e062ce88f73e0c74e30ab47ca2eb53b4c4ba292788bca4eaa645
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rosdep-modules/python3-rosdep-modules_0.19.0.orig.tar.gz' python3-rosdep-modules_0.19.0.orig.tar.gz 87969 SHA512:8cef879d00e1bc3d04a1138b9ceaa8fa734d84b3b8c2ac266a3406e85d26857a150b7547599fd27928c24dfe979e26adc61d2736d84b3cd5af0feccb5da21615
```

### `dpkg` source package: `python3-rosdep=0.19.0-1`

Binary Packages:

- `python3-rosdep=0.19.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rosdep=0.19.0-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rosdep/python3-rosdep_0.19.0-1.debian.tar.xz' python3-rosdep_0.19.0-1.debian.tar.xz 1988 SHA512:ea589d863f280b52f08ba88484a272cd933e1f9f0a31e21b9fc28d6140e248559b2b4a7b82b74e1f020b09c850a22a42b2f53281a2639a09ea36880da78b13f0
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rosdep/python3-rosdep_0.19.0-1.dsc' python3-rosdep_0.19.0-1.dsc 892 SHA512:fafaf765c61728e015ab5ce1e51b489e7d34340037f060d7f7e903438fbc86e04cf6daee10d89b385d7843536a47454797d714b49b5163522cecfd2bfe7c774b
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rosdep/python3-rosdep_0.19.0.orig.tar.gz' python3-rosdep_0.19.0.orig.tar.gz 31447 SHA512:7c19a0cbe56ecc7c4702bd1f8c0db365722764caf372bdf80c7a0bcd10100ca64967774d63c7591b5ba6abb8dbd585766b88dac6e021a15324b5b66b5c56bd6c
```

### `dpkg` source package: `python3-rosdistro-modules=0.8.2-1`

Binary Packages:

- `python3-rosdistro-modules=0.8.2-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python3-rosdistro=0.8.2-100`

Binary Packages:

- `python3-rosdistro=0.8.2-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `python3-rospkg-modules=1.2.8-1`

Binary Packages:

- `python3-rospkg-modules=1.2.8-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rospkg-modules=1.2.8-1
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rospkg-modules/python3-rospkg-modules_1.2.8-1.debian.tar.xz' python3-rospkg-modules_1.2.8-1.debian.tar.xz 1168 SHA512:b6a6d335cf727eead913a243d0ba00a14315e5893780e2f00561e54db432a0d89446180130336be7e5285b5c7b30ce146531cbfd60fb7f4289b56833279dc0e3
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rospkg-modules/python3-rospkg-modules_1.2.8-1.dsc' python3-rospkg-modules_1.2.8-1.dsc 940 SHA512:c947e02ec9c2bdd8935fa934480a6b8bf24c2448f05ae2587a15d34973e992f752d43b2f699dd8517d49258ce03b0b3bcd799d2138625e9ce463c37393f65610
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rospkg-modules/python3-rospkg-modules_1.2.8.orig.tar.gz' python3-rospkg-modules_1.2.8.orig.tar.gz 41375 SHA512:ec447afecdb934caff306c77b17c124fb20ba414f0a47537d859164c5c214c3864fe79c14a9d7685882ebd4121cfcc3d022eb222c1ec0c40be554480240c5db7
```

### `dpkg` source package: `python3-rospkg=1.2.8-100`

Binary Packages:

- `python3-rospkg=1.2.8-100`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-rospkg=1.2.8-100
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rospkg/python3-rospkg_1.2.8-100.debian.tar.xz' python3-rospkg_1.2.8-100.debian.tar.xz 1128 SHA512:96fef848978fe401812fb90bf6838d13c752b1407fbcc2e194252c65e16e1db8c8bc777a5e044a36996d2b547bf3cc18e588beab67a6d657b0d58c2508754037
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rospkg/python3-rospkg_1.2.8-100.dsc' python3-rospkg_1.2.8-100.dsc 876 SHA512:794e7c9418952ee16d70a98ae33b0119eb535a78404ca402b69476050916e90ff435907ae4008fcc637f46cb028762300a923034f7c33a1fac1e8669c49ae703
'http://packages.ros.org/ros/ubuntu/pool/main/p/python3-rospkg/python3-rospkg_1.2.8.orig.tar.gz' python3-rospkg_1.2.8.orig.tar.gz 17508 SHA512:e780ad435a35c87e521f46fcb0e1f4f483db07761c61b9c5a8704c0ccbdb755520ed92c9accc413d8f1717c0d4091b8588085d2612f29238d7a1e424e06a28ad
```

### `dpkg` source package: `python3-stdlib-extensions=3.8.2-1ubuntu1`

Binary Packages:

- `python3-distutils=3.8.2-1ubuntu1`
- `python3-lib2to3=3.8.2-1ubuntu1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris python3-stdlib-extensions=3.8.2-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.8.2-1ubuntu1.dsc' python3-stdlib-extensions_3.8.2-1ubuntu1.dsc 2477 SHA256:b02defe10e25b807a9ed121a94a6ca52653617cf045abf4624928c17a083d8d8
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.8.2.orig.tar.xz' python3-stdlib-extensions_3.8.2.orig.tar.xz 1058908 SHA256:15d0f5d9e33f0c274ac4f76db33811e68b43c4dea3071286fd1606a42bc08bd7
'http://archive.ubuntu.com/ubuntu/pool/main/p/python3-stdlib-extensions/python3-stdlib-extensions_3.8.2-1ubuntu1.debian.tar.xz' python3-stdlib-extensions_3.8.2-1ubuntu1.debian.tar.xz 17312 SHA256:87dbe56672ce938ade40e41a86d05313d714a6a2c9a8a5d9531974e1061b5f7d
```

### `dpkg` source package: `python3.8=3.8.2-1ubuntu1.2`

Binary Packages:

- `libpython3.8:amd64=3.8.2-1ubuntu1.2`
- `libpython3.8-dev:amd64=3.8.2-1ubuntu1.2`
- `libpython3.8-minimal:amd64=3.8.2-1ubuntu1.2`
- `libpython3.8-stdlib:amd64=3.8.2-1ubuntu1.2`
- `python3.8=3.8.2-1ubuntu1.2`
- `python3.8-dev=3.8.2-1ubuntu1.2`
- `python3.8-minimal=3.8.2-1ubuntu1.2`

Licenses: (parsed from: `/usr/share/doc/libpython3.8/copyright`, `/usr/share/doc/libpython3.8-dev/copyright`, `/usr/share/doc/libpython3.8-minimal/copyright`, `/usr/share/doc/libpython3.8-stdlib/copyright`, `/usr/share/doc/python3.8/copyright`, `/usr/share/doc/python3.8-dev/copyright`, `/usr/share/doc/python3.8-minimal/copyright`)

- `* Permission to use this software in any way is granted without`
- `By obtaining, using, and/or copying this software and/or its`
- `GPL-2`
- `Permission  is  hereby granted,  free  of charge,  to  any person`
- `Permission is hereby granted, free of charge, to any person obtaining`
- `Permission to use, copy, modify,`
- `Redistribution`
- `This software is provided 'as-is', without any express`
- `This software is provided as-is, without express`
- `binary forms, with`
- `distribute this software`
- `distribute this software and`
- `distribute this software for any`
- `implied`
- `its`
- `use in source`
- `without`

**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `pyyaml=5.3.1-1`

Binary Packages:

- `python3-yaml=5.3.1-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris pyyaml=5.3.1-1
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_5.3.1-1.dsc' pyyaml_5.3.1-1.dsc 2303 SHA256:1d3553551071695322b5f6b4e8236270a998186a8d1b1adba949e2467f47964b
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_5.3.1.orig.tar.gz' pyyaml_5.3.1.orig.tar.gz 269377 SHA256:b8eac752c5e14d3eca0e6dd9199cd627518cb5ec06add0de9d32baeee6fe645d
'http://archive.ubuntu.com/ubuntu/pool/main/p/pyyaml/pyyaml_5.3.1-1.debian.tar.xz' pyyaml_5.3.1-1.debian.tar.xz 7048 SHA256:d1489432534a5fda1f49cb3e134cdce9333f50a0edeea963bc9e3e63f2ae2aae
```

### `dpkg` source package: `rdma-core=28.0-1ubuntu1`

Binary Packages:

- `ibverbs-providers:amd64=28.0-1ubuntu1`
- `libibverbs-dev:amd64=28.0-1ubuntu1`
- `libibverbs1:amd64=28.0-1ubuntu1`
- `librdmacm1:amd64=28.0-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/ibverbs-providers/copyright`, `/usr/share/doc/libibverbs-dev/copyright`, `/usr/share/doc/libibverbs1/copyright`, `/usr/share/doc/librdmacm1/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-MIT`
- `CC0`
- `CPL-1.0`
- `GPL-2`
- `GPL-2+`
- `MIT`

Source:

```console
$ apt-get source -qq --print-uris rdma-core=28.0-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rdma-core/rdma-core_28.0-1ubuntu1.dsc' rdma-core_28.0-1ubuntu1.dsc 3316 SHA256:d189ccad9f79ff35d227802d4f91f97b5bc61625ec81557ab7f10dfe925dc17f
'http://archive.ubuntu.com/ubuntu/pool/main/r/rdma-core/rdma-core_28.0.orig.tar.gz' rdma-core_28.0.orig.tar.gz 1510050 SHA256:e8ae3a78f9908cdc9139e8f6a155cd0bb43a30d0e54f28a3c7a2df4af51b3f4d
'http://archive.ubuntu.com/ubuntu/pool/main/r/rdma-core/rdma-core_28.0-1ubuntu1.debian.tar.xz' rdma-core_28.0-1ubuntu1.debian.tar.xz 21944 SHA256:9dceabfcaf46267ccb29ec9204066a5995b6c2ca723e0613d5767d5d43f37e6e
```

### `dpkg` source package: `readline=8.0-4`

Binary Packages:

- `libreadline8:amd64=8.0-4`
- `readline-common=8.0-4`

Licenses: (parsed from: `/usr/share/doc/libreadline8/copyright`, `/usr/share/doc/readline-common/copyright`)

- `GFDL`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris readline=8.0-4
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0-4.dsc' readline_8.0-4.dsc 2434 SHA256:ac9c7bb7380fe740aef09f54becf482eb81032a33dc11f1a8f00e933c5f168f4
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0.orig.tar.gz' readline_8.0.orig.tar.gz 2975937 SHA256:e339f51971478d369f8a053a330a190781acb9864cf4c541060f12078948e461
'http://archive.ubuntu.com/ubuntu/pool/main/r/readline/readline_8.0-4.debian.tar.xz' readline_8.0-4.debian.tar.xz 30408 SHA256:60ed18dab6d6b7fc998a263d917f06d9cce6e1ccd19cd8bf4a9d33c5350cf8d6
```

### `dpkg` source package: `rhash=1.3.9-1`

Binary Packages:

- `librhash0:amd64=1.3.9-1`

Licenses: (parsed from: `/usr/share/doc/librhash0/copyright`)

- `0BSD`

Source:

```console
$ apt-get source -qq --print-uris rhash=1.3.9-1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.3.9-1.dsc' rhash_1.3.9-1.dsc 1990 SHA256:2c7d736fb4ddb0cec03e61b958921306cd8e0ba29ad2da4d9521739f25c7f053
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.3.9.orig.tar.gz' rhash_1.3.9.orig.tar.gz 403415 SHA256:42b1006f998adb189b1f316bf1a60e3171da047a85c4aaded2d0d26c1476c9f6
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.3.9.orig.tar.gz.asc' rhash_1.3.9.orig.tar.gz.asc 833 SHA256:db168ff736c3fc0983b705b8b95c63187ac79df554e11a47e5e719b242ff65d4
'http://archive.ubuntu.com/ubuntu/pool/main/r/rhash/rhash_1.3.9-1.debian.tar.xz' rhash_1.3.9-1.debian.tar.xz 9936 SHA256:64c6405e34a360297e9612564adb4af7fd0e2dc291f25df38252560c7ca1c11e
```

### `dpkg` source package: `ros-noetic-actionlib-msgs=1.13.0-1focal.20200812.170243`

Binary Packages:

- `ros-noetic-actionlib-msgs=1.13.0-1focal.20200812.170243`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-actionlib=1.13.2-1focal.20200826.180635`

Binary Packages:

- `ros-noetic-actionlib=1.13.2-1focal.20200826.180635`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-bond-core=1.8.6-1focal.20200901.145320`

Binary Packages:

- `ros-noetic-bond-core=1.8.6-1focal.20200901.145320`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-bond=1.8.6-1focal.20200901.144734`

Binary Packages:

- `ros-noetic-bond=1.8.6-1focal.20200901.144734`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-bondcpp=1.8.6-1focal.20200901.145108`

Binary Packages:

- `ros-noetic-bondcpp=1.8.6-1focal.20200901.145108`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-bondpy=1.8.6-1focal.20200901.145053`

Binary Packages:

- `ros-noetic-bondpy=1.8.6-1focal.20200901.145053`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-catkin=0.8.8-1focal.20200724.164751`

Binary Packages:

- `ros-noetic-catkin=0.8.8-1focal.20200724.164751`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-class-loader=0.5.0-1focal.20200724.165437`

Binary Packages:

- `ros-noetic-class-loader=0.5.0-1focal.20200724.165437`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-cmake-modules=0.5.0-1focal.20200724.165226`

Binary Packages:

- `ros-noetic-cmake-modules=0.5.0-1focal.20200724.165226`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-common-msgs=1.13.0-1focal.20200812.195732`

Binary Packages:

- `ros-noetic-common-msgs=1.13.0-1focal.20200812.195732`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-cpp-common=0.7.2-1focal.20200724.170504`

Binary Packages:

- `ros-noetic-cpp-common=0.7.2-1focal.20200724.170504`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-diagnostic-msgs=1.13.0-1focal.20200812.170346`

Binary Packages:

- `ros-noetic-diagnostic-msgs=1.13.0-1focal.20200812.170346`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-dynamic-reconfigure=1.7.1-1focal.20200901.144724`

Binary Packages:

- `ros-noetic-dynamic-reconfigure=1.7.1-1focal.20200901.144724`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-gencpp=0.6.5-1focal.20200724.170029`

Binary Packages:

- `ros-noetic-gencpp=0.6.5-1focal.20200724.170029`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-geneus=3.0.0-1focal.20200724.165941`

Binary Packages:

- `ros-noetic-geneus=3.0.0-1focal.20200724.165941`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-genlisp=0.4.18-1focal.20200724.165913`

Binary Packages:

- `ros-noetic-genlisp=0.4.18-1focal.20200724.165913`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-genmsg=0.5.16-1focal.20200724.165742`

Binary Packages:

- `ros-noetic-genmsg=0.5.16-1focal.20200724.165742`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-gennodejs=2.0.2-1focal.20200724.165923`

Binary Packages:

- `ros-noetic-gennodejs=2.0.2-1focal.20200724.165923`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-genpy=0.6.14-1focal.20200812.160957`

Binary Packages:

- `ros-noetic-genpy=0.6.14-1focal.20200812.160957`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-geometry-msgs=1.13.0-1focal.20200812.170527`

Binary Packages:

- `ros-noetic-geometry-msgs=1.13.0-1focal.20200812.170527`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-message-filters=1.15.8-1focal.20200812.185928`

Binary Packages:

- `ros-noetic-message-filters=1.15.8-1focal.20200812.185928`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-message-generation=0.4.1-1focal.20200812.162405`

Binary Packages:

- `ros-noetic-message-generation=0.4.1-1focal.20200812.162405`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-message-runtime=0.4.13-1focal.20200812.162259`

Binary Packages:

- `ros-noetic-message-runtime=0.4.13-1focal.20200812.162259`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-mk=1.15.6-1focal.20200812.172829`

Binary Packages:

- `ros-noetic-mk=1.15.6-1focal.20200812.172829`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-nav-msgs=1.13.0-1focal.20200812.172050`

Binary Packages:

- `ros-noetic-nav-msgs=1.13.0-1focal.20200812.172050`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-nodelet-core=1.10.0-1focal.20200901.160347`

Binary Packages:

- `ros-noetic-nodelet-core=1.10.0-1focal.20200901.160347`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-nodelet-topic-tools=1.10.0-1focal.20200901.152237`

Binary Packages:

- `ros-noetic-nodelet-topic-tools=1.10.0-1focal.20200901.152237`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-nodelet=1.10.0-1focal.20200901.151355`

Binary Packages:

- `ros-noetic-nodelet=1.10.0-1focal.20200901.151355`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-pluginlib=1.13.0-1focal.20200812.174323`

Binary Packages:

- `ros-noetic-pluginlib=1.13.0-1focal.20200812.174323`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-ros-base=1.5.0-1focal.20200901.160953`

Binary Packages:

- `ros-noetic-ros-base=1.5.0-1focal.20200901.160953`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-ros-comm=1.15.8-1focal.20200812.202746`

Binary Packages:

- `ros-noetic-ros-comm=1.15.8-1focal.20200812.202746`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-ros-core=1.5.0-1focal.20200812.204115`

Binary Packages:

- `ros-noetic-ros-core=1.5.0-1focal.20200812.204115`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-ros-environment=1.3.1-1focal.20200724.170728`

Binary Packages:

- `ros-noetic-ros-environment=1.3.1-1focal.20200724.170728`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-ros=1.15.6-1focal.20200812.173936`

Binary Packages:

- `ros-noetic-ros=1.15.6-1focal.20200812.173936`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosbag-migration-rule=1.0.1-1focal.20200724.170314`

Binary Packages:

- `ros-noetic-rosbag-migration-rule=1.0.1-1focal.20200724.170314`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosbag-storage=1.15.8-1focal.20200812.185350`

Binary Packages:

- `ros-noetic-rosbag-storage=1.15.8-1focal.20200812.185350`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosbag=1.15.8-1focal.20200812.191024`

Binary Packages:

- `ros-noetic-rosbag=1.15.8-1focal.20200812.191024`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosbash=1.15.6-1focal.20200724.171435`

Binary Packages:

- `ros-noetic-rosbash=1.15.6-1focal.20200724.171435`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosboost-cfg=1.15.6-1focal.20200724.170133`

Binary Packages:

- `ros-noetic-rosboost-cfg=1.15.6-1focal.20200724.170133`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosbuild=1.15.6-1focal.20200812.163643`

Binary Packages:

- `ros-noetic-rosbuild=1.15.6-1focal.20200812.163643`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosclean=1.15.6-1focal.20200724.164938`

Binary Packages:

- `ros-noetic-rosclean=1.15.6-1focal.20200724.164938`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosconsole-bridge=0.5.4-1focal.20200812.174333`

Binary Packages:

- `ros-noetic-rosconsole-bridge=0.5.4-1focal.20200812.174333`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosconsole=1.14.2-1focal.20200812.172838`

Binary Packages:

- `ros-noetic-rosconsole=1.14.2-1focal.20200812.172838`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roscpp-core=0.7.2-1focal.20200724.171512`

Binary Packages:

- `ros-noetic-roscpp-core=0.7.2-1focal.20200724.171512`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roscpp-serialization=0.7.2-1focal.20200724.171151`

Binary Packages:

- `ros-noetic-roscpp-serialization=0.7.2-1focal.20200724.171151`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roscpp-traits=0.7.2-1focal.20200724.170950`

Binary Packages:

- `ros-noetic-roscpp-traits=0.7.2-1focal.20200724.170950`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roscpp=1.15.8-1focal.20200812.174031`

Binary Packages:

- `ros-noetic-roscpp=1.15.8-1focal.20200812.174031`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roscreate=1.15.6-1focal.20200724.171702`

Binary Packages:

- `ros-noetic-roscreate=1.15.6-1focal.20200724.171702`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosgraph-msgs=1.11.3-1focal.20200812.171808`

Binary Packages:

- `ros-noetic-rosgraph-msgs=1.11.3-1focal.20200812.171808`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosgraph=1.15.8-1focal.20200724.164942`

Binary Packages:

- `ros-noetic-rosgraph=1.15.8-1focal.20200724.164942`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roslang=1.15.6-1focal.20200724.165900`

Binary Packages:

- `ros-noetic-roslang=1.15.6-1focal.20200724.165900`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roslaunch=1.15.8-1focal.20200812.181327`

Binary Packages:

- `ros-noetic-roslaunch=1.15.8-1focal.20200812.181327`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roslib=1.15.6-1focal.20200724.171431`

Binary Packages:

- `ros-noetic-roslib=1.15.6-1focal.20200724.171431`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roslisp=1.9.24-1focal.20200812.173107`

Binary Packages:

- `ros-noetic-roslisp=1.9.24-1focal.20200812.173107`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roslz4=1.15.8-1focal.20200724.172033`

Binary Packages:

- `ros-noetic-roslz4=1.15.8-1focal.20200724.172033`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosmake=1.15.6-1focal.20200724.165039`

Binary Packages:

- `ros-noetic-rosmake=1.15.6-1focal.20200724.165039`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosmaster=1.15.8-1focal.20200724.165053`

Binary Packages:

- `ros-noetic-rosmaster=1.15.8-1focal.20200724.165053`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosmsg=1.15.8-1focal.20200812.192620`

Binary Packages:

- `ros-noetic-rosmsg=1.15.8-1focal.20200812.192620`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosnode=1.15.8-1focal.20200812.195632`

Binary Packages:

- `ros-noetic-rosnode=1.15.8-1focal.20200812.195632`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosout=1.15.8-1focal.20200812.180004`

Binary Packages:

- `ros-noetic-rosout=1.15.8-1focal.20200812.180004`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rospack=2.6.2-1focal.20200724.171137`

Binary Packages:

- `ros-noetic-rospack=2.6.2-1focal.20200724.171137`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosparam=1.15.8-1focal.20200724.165530`

Binary Packages:

- `ros-noetic-rosparam=1.15.8-1focal.20200724.165530`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rospy=1.15.8-1focal.20200812.181338`

Binary Packages:

- `ros-noetic-rospy=1.15.8-1focal.20200812.181338`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosservice=1.15.8-1focal.20200812.194030`

Binary Packages:

- `ros-noetic-rosservice=1.15.8-1focal.20200812.194030`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rostest=1.15.8-1focal.20200812.183314`

Binary Packages:

- `ros-noetic-rostest=1.15.8-1focal.20200812.183314`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rostime=0.7.2-1focal.20200724.170727`

Binary Packages:

- `ros-noetic-rostime=0.7.2-1focal.20200724.170727`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rostopic=1.15.8-1focal.20200812.192658`

Binary Packages:

- `ros-noetic-rostopic=1.15.8-1focal.20200812.192658`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-rosunit=1.15.6-1focal.20200724.171710`

Binary Packages:

- `ros-noetic-rosunit=1.15.6-1focal.20200724.171710`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-roswtf=1.15.8-1focal.20200812.201106`

Binary Packages:

- `ros-noetic-roswtf=1.15.8-1focal.20200812.201106`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-sensor-msgs=1.13.0-1focal.20200812.192710`

Binary Packages:

- `ros-noetic-sensor-msgs=1.13.0-1focal.20200812.192710`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-shape-msgs=1.13.0-1focal.20200812.172454`

Binary Packages:

- `ros-noetic-shape-msgs=1.13.0-1focal.20200812.172454`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-smclib=1.8.6-1focal.20200901.144503`

Binary Packages:

- `ros-noetic-smclib=1.8.6-1focal.20200901.144503`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-std-msgs=0.5.13-1focal.20200812.163652`

Binary Packages:

- `ros-noetic-std-msgs=0.5.13-1focal.20200812.163652`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-std-srvs=1.11.3-1focal.20200812.163752`

Binary Packages:

- `ros-noetic-std-srvs=1.11.3-1focal.20200812.163752`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-stereo-msgs=1.13.0-1focal.20200812.194354`

Binary Packages:

- `ros-noetic-stereo-msgs=1.13.0-1focal.20200812.194354`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-topic-tools=1.15.8-1focal.20200812.185211`

Binary Packages:

- `ros-noetic-topic-tools=1.15.8-1focal.20200812.185211`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-trajectory-msgs=1.13.0-1focal.20200812.172518`

Binary Packages:

- `ros-noetic-trajectory-msgs=1.13.0-1focal.20200812.172518`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-visualization-msgs=1.13.0-1focal.20200812.172527`

Binary Packages:

- `ros-noetic-visualization-msgs=1.13.0-1focal.20200812.172527`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-noetic-xmlrpcpp=1.15.8-1focal.20200724.170935`

Binary Packages:

- `ros-noetic-xmlrpcpp=1.15.8-1focal.20200724.170935`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


**WARNING:** unable to find source (`apt-get source` failed or returned no results)!  
This is *usually* due to a new package version being released and the old version being removed.


### `dpkg` source package: `ros-rosinstall=0.7.8-4`

Binary Packages:

- `python3-rosinstall=0.7.8-4`

Licenses: (parsed from: `/usr/share/doc/python3-rosinstall/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris ros-rosinstall=0.7.8-4
'http://archive.ubuntu.com/ubuntu/pool/universe/r/ros-rosinstall/ros-rosinstall_0.7.8-4.dsc' ros-rosinstall_0.7.8-4.dsc 2272 SHA256:175559582ae999e96d337addfe50d1da734d2929de72885976c98616fc032486
'http://archive.ubuntu.com/ubuntu/pool/universe/r/ros-rosinstall/ros-rosinstall_0.7.8.orig.tar.gz' ros-rosinstall_0.7.8.orig.tar.gz 64864 SHA256:ce1266e63aaefccabb4b0aefc56f8cceb45d4e188a4ecad2f623cbb4a5b1843f
'http://archive.ubuntu.com/ubuntu/pool/universe/r/ros-rosinstall/ros-rosinstall_0.7.8-4.debian.tar.xz' ros-rosinstall_0.7.8-4.debian.tar.xz 5396 SHA256:b27ea6506f952767df7cdf174fecdb3116caf4f8902cdd7db014976937a8f3dc
```

### `dpkg` source package: `ros-vcstools=0.1.42-2`

Binary Packages:

- `python3-vcstools=0.1.42-2`

Licenses: (parsed from: `/usr/share/doc/python3-vcstools/copyright`)

- `BSD-3-clause`
- `Expat`

Source:

```console
$ apt-get source -qq --print-uris ros-vcstools=0.1.42-2
'http://archive.ubuntu.com/ubuntu/pool/universe/r/ros-vcstools/ros-vcstools_0.1.42-2.dsc' ros-vcstools_0.1.42-2.dsc 2250 SHA256:5b8d5c32cfe0dea157a9df3741abe6a71e5b481b1ceaf67d3183011a74fc90d9
'http://archive.ubuntu.com/ubuntu/pool/universe/r/ros-vcstools/ros-vcstools_0.1.42.orig.tar.gz' ros-vcstools_0.1.42.orig.tar.gz 65979 SHA256:3dccd4d3c82d3be6b0ba6a2def83af7e68ee495d108587ac66aa74720e5e9c97
'http://archive.ubuntu.com/ubuntu/pool/universe/r/ros-vcstools/ros-vcstools_0.1.42-2.debian.tar.xz' ros-vcstools_0.1.42-2.debian.tar.xz 4408 SHA256:8149158c31379770d87d371907eee3eba2cd1367a1828da0109408df5487bd87
```

### `dpkg` source package: `ros-wstool=0.1.18-2`

Binary Packages:

- `python3-wstool=0.1.18-2`

Licenses: (parsed from: `/usr/share/doc/python3-wstool/copyright`)

- `BSD-3-clause`

Source:

```console
$ apt-get source -qq --print-uris ros-wstool=0.1.18-2
'http://archive.ubuntu.com/ubuntu/pool/universe/r/ros-wstool/ros-wstool_0.1.18-2.dsc' ros-wstool_0.1.18-2.dsc 2206 SHA256:8d9f4a959214e512e083a13a672dc51d7078ea6baf35996ba20e9c26e45e67ca
'http://archive.ubuntu.com/ubuntu/pool/universe/r/ros-wstool/ros-wstool_0.1.18.orig.tar.gz' ros-wstool_0.1.18.orig.tar.gz 80595 SHA256:f04621acda755a45896db2d3a84131f96cf69905515997637b4568f3fad5c46e
'http://archive.ubuntu.com/ubuntu/pool/universe/r/ros-wstool/ros-wstool_0.1.18-2.debian.tar.xz' ros-wstool_0.1.18-2.debian.tar.xz 3300 SHA256:0db0a4ba0bf4f4f6d952136d9b792666be5534d037b7139aa857556a27a0697b
```

### `dpkg` source package: `rtmpdump=2.4+20151223.gitfa8646d.1-2build1`

Binary Packages:

- `librtmp1:amd64=2.4+20151223.gitfa8646d.1-2build1`

Licenses: (parsed from: `/usr/share/doc/librtmp1/copyright`)

- `GPL-2`
- `LGPL-2.1`

Source:

```console
$ apt-get source -qq --print-uris rtmpdump=2.4+20151223.gitfa8646d.1-2build1
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build1.dsc' rtmpdump_2.4+20151223.gitfa8646d.1-2build1.dsc 2439 SHA256:fd89213f2d41b00c212a411a945146c6b2e00fce1d1819a9ec380b0d91bd1077
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz' rtmpdump_2.4+20151223.gitfa8646d.1.orig.tar.gz 142213 SHA256:5c032f5c8cc2937eb55a81a94effdfed3b0a0304b6376147b86f951e225e3ab5
'http://archive.ubuntu.com/ubuntu/pool/main/r/rtmpdump/rtmpdump_2.4+20151223.gitfa8646d.1-2build1.debian.tar.xz' rtmpdump_2.4+20151223.gitfa8646d.1-2build1.debian.tar.xz 8216 SHA256:b256cc2aa96c9b99918052c4badfab0339ba95a852eab5ae37aa8b53c259efd2
```

### `dpkg` source package: `sbcl=2:2.0.1-3`

Binary Packages:

- `sbcl=2:2.0.1-3`

Licenses: (parsed from: `/usr/share/doc/sbcl/copyright`)

- `Apache-2.0`
- `BSD-3-clause`
- `Expat`
- `NTP`
- `NTP~disclaimer`
- `Unicode`
- `permissive-xerox`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sbcl=2:2.0.1-3
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sbcl/sbcl_2.0.1-3.dsc' sbcl_2.0.1-3.dsc 2302 SHA256:c7c0af62fe93e714970f3309fcb588947734224cdcb4d3b2e8859b9e0930ad77
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sbcl/sbcl_2.0.1.orig.tar.bz2' sbcl_2.0.1.orig.tar.bz2 6466983 SHA256:8450d60b7264a34158f8811d46dc6e74ff855bbd1227752572877e6604ce56e8
'http://archive.ubuntu.com/ubuntu/pool/universe/s/sbcl/sbcl_2.0.1-3.debian.tar.xz' sbcl_2.0.1-3.debian.tar.xz 74340 SHA256:4ce1590486545f367accafda50ab9a2ae19f19d2f80be3263dd26261ecff14a7
```

### `dpkg` source package: `sed=4.7-1`

Binary Packages:

- `sed=4.7-1`

Licenses: (parsed from: `/usr/share/doc/sed/copyright`)

- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris sed=4.7-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7-1.dsc' sed_4.7-1.dsc 1880 SHA256:dd0e8daed987929920f7729771f9c7a5b48d094923aaf686efd2ab19db776108
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7.orig.tar.xz' sed_4.7.orig.tar.xz 1298316 SHA256:2885768cd0a29ff8d58a6280a270ff161f6a3deb5690b2be6c49f46d4c67bd6a
'http://archive.ubuntu.com/ubuntu/pool/main/s/sed/sed_4.7-1.debian.tar.xz' sed_4.7-1.debian.tar.xz 59824 SHA256:a2ab8d50807fd2242f86d6c6257399e790445ab6f8932f7f487d34361b4fc483
```

### `dpkg` source package: `sensible-utils=0.0.12+nmu1`

Binary Packages:

- `sensible-utils=0.0.12+nmu1`

Licenses: (parsed from: `/usr/share/doc/sensible-utils/copyright`)

- `All-permissive`
- `GPL-2`
- `GPL-2+`
- `configure`
- `installsh`

Source:

```console
$ apt-get source -qq --print-uris sensible-utils=0.0.12+nmu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12+nmu1.dsc' sensible-utils_0.0.12+nmu1.dsc 1753 SHA256:68bcb3e542e29a8a0bf281d9145d0e4cd9def529af2ba0cfe0afee3c5af958bc
'http://archive.ubuntu.com/ubuntu/pool/main/s/sensible-utils/sensible-utils_0.0.12+nmu1.tar.xz' sensible-utils_0.0.12+nmu1.tar.xz 61988 SHA256:53c6606facf083adbbf0da04e6d774b31ff3f46c7ba36a82d3f182779f4c3f5b
```

### `dpkg` source package: `setuptools=45.2.0-1`

Binary Packages:

- `python3-pkg-resources=45.2.0-1`
- `python3-setuptools=45.2.0-1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris setuptools=45.2.0-1
'http://archive.ubuntu.com/ubuntu/pool/main/s/setuptools/setuptools_45.2.0-1.dsc' setuptools_45.2.0-1.dsc 2055 SHA256:67e6043f56584fddfec65174bf778cc31f335814155225064bd639c704f837d7
'http://archive.ubuntu.com/ubuntu/pool/main/s/setuptools/setuptools_45.2.0.orig.tar.xz' setuptools_45.2.0.orig.tar.xz 463920 SHA256:54b5b2244d9343374133e8a0d1378f843760885ddaca95458144b6b39cf698e9
'http://archive.ubuntu.com/ubuntu/pool/main/s/setuptools/setuptools_45.2.0-1.debian.tar.xz' setuptools_45.2.0-1.debian.tar.xz 14372 SHA256:c776ff57ecb4c2dfefdf2fb85509196836e402a6d7a0cd6f942939962e209c5c
```

### `dpkg` source package: `sgml-base=1.29.1`

Binary Packages:

- `sgml-base=1.29.1`

Licenses: (parsed from: `/usr/share/doc/sgml-base/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sgml-base=1.29.1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sgml-base/sgml-base_1.29.1.dsc' sgml-base_1.29.1.dsc 1526 SHA256:dc6bf6e060834d9534e38c3c322772d69ff3b32ceceb3739a7d4af84ce3cff8c
'http://archive.ubuntu.com/ubuntu/pool/main/s/sgml-base/sgml-base_1.29.1.tar.xz' sgml-base_1.29.1.tar.xz 12260 SHA256:3cac1ae8527c8ea0b699f2fb3891a0d44e49ece74d4e127f306e43cdb57bd78e
```

### `dpkg` source package: `shadow=1:4.8.1-1ubuntu5.20.04`

Binary Packages:

- `login=1:4.8.1-1ubuntu5.20.04`
- `passwd=1:4.8.1-1ubuntu5.20.04`

Licenses: (parsed from: `/usr/share/doc/login/copyright`, `/usr/share/doc/passwd/copyright`)

- `GPL-2`

Source:

```console
$ apt-get source -qq --print-uris shadow=1:4.8.1-1ubuntu5.20.04
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu5.20.04.dsc' shadow_4.8.1-1ubuntu5.20.04.dsc 1729 SHA512:fc557d6572f8732cc21f8bb69df08f6a289b3615e19f0374a4e4812b89e793e3f071c552a69c43cbb82e659ac735b3ad6d62d3205f3a12591037e3669430ea5d
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1.orig.tar.xz' shadow_4.8.1.orig.tar.xz 1611196 SHA512:780a983483d847ed3c91c82064a0fa902b6f4185225978241bc3bc03fcc3aa143975b46aee43151c6ba43efcfdb1819516b76ba7ad3d1d3c34fcc38ea42e917b
'http://archive.ubuntu.com/ubuntu/pool/main/s/shadow/shadow_4.8.1-1ubuntu5.20.04.debian.tar.xz' shadow_4.8.1-1ubuntu5.20.04.debian.tar.xz 85640 SHA512:237d007329c915889766807ad85c8954fe8cf81b8aa074cdc8eba46e6157cd9386dc53cd5054f13618af30af30033074e0881c2f3f43d5f7e86224b2a261791c
```

### `dpkg` source package: `six=1.14.0-2`

Binary Packages:

- `python3-six=1.14.0-2`

Licenses: (parsed from: `/usr/share/doc/python3-six/copyright`)

- `Expat`

Source:

```console
$ apt-get source -qq --print-uris six=1.14.0-2
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.14.0-2.dsc' six_1.14.0-2.dsc 2426 SHA256:1655e1f7246bd08332615eb3f6bb7769435724cd60e2ed0c0ce717e1ffd89416
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.14.0.orig.tar.gz' six_1.14.0.orig.tar.gz 33857 SHA256:236bdbdce46e6e6a3d61a337c0f8b763ca1e8717c03b369e87a7ec7ce1319c0a
'http://archive.ubuntu.com/ubuntu/pool/main/s/six/six_1.14.0-2.debian.tar.xz' six_1.14.0-2.debian.tar.xz 4368 SHA256:02a80f76758dde7a8b2f42cd05a20db56d956f4678a882f0aba905ee49847050
```

### `dpkg` source package: `sqlite3=3.31.1-4ubuntu0.2`

Binary Packages:

- `libsqlite3-0:amd64=3.31.1-4ubuntu0.2`
- `libsqlite3-dev:amd64=3.31.1-4ubuntu0.2`

Licenses: (parsed from: `/usr/share/doc/libsqlite3-0/copyright`, `/usr/share/doc/libsqlite3-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris sqlite3=3.31.1-4ubuntu0.2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1-4ubuntu0.2.dsc' sqlite3_3.31.1-4ubuntu0.2.dsc 2519 SHA512:d7adfe86e7996d2a45238bc3b782de6894a585bba1498b3747aacb15313160354bc072ab2e257a2a034ce44921bd07329b8a9172290428f753274b6d7b00326e
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1.orig-www.tar.xz' sqlite3_3.31.1.orig-www.tar.xz 5764424 SHA512:a47adacd46c673cfd674cb64fb54b054e69560aed8c8c429773f0eccdcdbce4be538397506eca8e2d169f4b46d0d47442b273e12d82f8c87e1aadf3ade458db6
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1.orig.tar.xz' sqlite3_3.31.1.orig.tar.xz 7108036 SHA512:67e1050efe2988fa3d0d7e4a87e147a8114c6ff9b6ca5307a068befb38e861930eaee0135048ff1abb1e6323b507cbc68a0aac3a8fe5f095d6fcea1547a7efaf
'http://archive.ubuntu.com/ubuntu/pool/main/s/sqlite3/sqlite3_3.31.1-4ubuntu0.2.debian.tar.xz' sqlite3_3.31.1-4ubuntu0.2.debian.tar.xz 33492 SHA512:87cc51bce108d6306d815683a1825b43a6e7a7d8dc2bade8ce34d3850b8a4437034b1383f5e60b8d9c4569e8ab5bb3eb28febda7745f4a9db01b5e1b0b11d5ae
```

### `dpkg` source package: `sudo=1.8.31-1ubuntu1.1`

Binary Packages:

- `sudo=1.8.31-1ubuntu1.1`

**WARNING:** unable to detect licenses! (package likely not compliant with DEP-5)  
If source is available (seen below), check the contents of `debian/copyright` within it.


Source:

```console
$ apt-get source -qq --print-uris sudo=1.8.31-1ubuntu1.1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.8.31-1ubuntu1.1.dsc' sudo_1.8.31-1ubuntu1.1.dsc 2088 SHA512:6d9b51976ed04b53fb4f9e7d00a8e10ab8cc8349c9d1c32bac6349ad3f91781c324ff05c66c9cf4bc6abf9586753f712fd98705fac33377fcc04dc8e338820f2
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.8.31.orig.tar.gz' sudo_1.8.31.orig.tar.gz 3350674 SHA512:b9e408a322938c7a712458e9012d8a5f648fba5b23a5057cf5d8372c7f931262595f1575c32c32b9cb1a04af670ff4611e7df48d197e5c4cc038d6b65439a28a
'http://archive.ubuntu.com/ubuntu/pool/main/s/sudo/sudo_1.8.31-1ubuntu1.1.debian.tar.xz' sudo_1.8.31-1ubuntu1.1.debian.tar.xz 32128 SHA512:fcf4bdc13466b158bf9700a6756dce29b1ce0820f6b0af4a5d669b2814444870a7668de4ef811d51f6324383af27e4dcb31f3af89ef1de5591dadb65efba039c
```

### `dpkg` source package: `systemd=245.4-4ubuntu3.2`

Binary Packages:

- `libsystemd0:amd64=245.4-4ubuntu3.2`
- `libudev1:amd64=245.4-4ubuntu3.2`

Licenses: (parsed from: `/usr/share/doc/libsystemd0/copyright`, `/usr/share/doc/libudev1/copyright`)

- `CC0-1.0`
- `Expat`
- `GPL-2`
- `GPL-2 with Linux-syscall-note exception`
- `GPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris systemd=245.4-4ubuntu3.2
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_245.4-4ubuntu3.2.dsc' systemd_245.4-4ubuntu3.2.dsc 5291 SHA512:d220f6dbe6b27f9a17a016ee952eef163be5e102b2436726f3b79a096ea3a2bd2d2c59d4bfd344bb9f5818ce9ab08a0ec08c05309b11547a98200ccfb2434b8e
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_245.4.orig.tar.gz' systemd_245.4.orig.tar.gz 9000780 SHA512:02036bb1ab05301a9d0dfdd4b9c9376e90134474482531e6e292122380be2f24f99177493dd3af6f8af1a8ed2599ee0996da91a3b1b7872bbfaf26a1c3e61b4c
'http://archive.ubuntu.com/ubuntu/pool/main/s/systemd/systemd_245.4-4ubuntu3.2.debian.tar.xz' systemd_245.4-4ubuntu3.2.debian.tar.xz 217140 SHA512:6e0561880e35bfb0e1943141465a8c23f0f029e4a02b0f6fb7c4a181d3f1a159c0afac1ed38f70f2b3044df874835ab31a2f619f3413d90f845d4ba90ad4ccd6
```

### `dpkg` source package: `sysvinit=2.96-2.1ubuntu1`

Binary Packages:

- `sysvinit-utils=2.96-2.1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/sysvinit-utils/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris sysvinit=2.96-2.1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-2.1ubuntu1.dsc' sysvinit_2.96-2.1ubuntu1.dsc 2751 SHA256:c8b5f2ef86c4c1b8bf6b8a48408a4aa0815b0cf416df51dc0a9b6b8134f7e42c
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz' sysvinit_2.96.orig.tar.xz 122164 SHA256:2a2e26b72aa235a23ab1c8471005f890309ce1196c83fbc9413c57b9ab62b587
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96.orig.tar.xz.asc' sysvinit_2.96.orig.tar.xz.asc 313 SHA256:dfc184b95da12c8c888c8ae6b0f26fe8a23b07fbcdd240f6600a8a78b9439fa0
'http://archive.ubuntu.com/ubuntu/pool/main/s/sysvinit/sysvinit_2.96-2.1ubuntu1.debian.tar.xz' sysvinit_2.96-2.1ubuntu1.debian.tar.xz 128840 SHA256:528041e261c90a957d9794bddb07217c89484d9c76a0279da508baec9684c4e6
```

### `dpkg` source package: `tar=1.30+dfsg-7`

Binary Packages:

- `tar=1.30+dfsg-7`

Licenses: (parsed from: `/usr/share/doc/tar/copyright`)

- `GPL-2`
- `GPL-3`

Source:

```console
$ apt-get source -qq --print-uris tar=1.30+dfsg-7
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg-7.dsc' tar_1.30+dfsg-7.dsc 1981 SHA256:5117afe47b5aab94c592d52c11c74dba146a11a7cdc22dbe067a4b5a5e895729
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg.orig.tar.xz' tar_1.30+dfsg.orig.tar.xz 1883220 SHA256:c02f3747ffe02017878303dde8b78e79cd220364c5e8048cf92320232e38912d
'http://archive.ubuntu.com/ubuntu/pool/main/t/tar/tar_1.30+dfsg-7.debian.tar.xz' tar_1.30+dfsg-7.debian.tar.xz 22168 SHA256:12763df7f214458a56edc4a4b27adb2cb2041d597d74212ba34736f02bb68cd3
```

### `dpkg` source package: `tinyxml2=7.0.0+dfsg-1build1`

Binary Packages:

- `libtinyxml2-6a:amd64=7.0.0+dfsg-1build1`
- `libtinyxml2-dev:amd64=7.0.0+dfsg-1build1`

Licenses: (parsed from: `/usr/share/doc/libtinyxml2-6a/copyright`, `/usr/share/doc/libtinyxml2-dev/copyright`)

- `GPL-2`
- `GPL-2+`
- `zlib/libpng`

Source:

```console
$ apt-get source -qq --print-uris tinyxml2=7.0.0+dfsg-1build1
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_7.0.0+dfsg-1build1.dsc' tinyxml2_7.0.0+dfsg-1build1.dsc 2053 SHA256:32a192cfb676070970b8718b40df4cf48208d4c8758a02acafa346df0de4e1bf
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_7.0.0+dfsg.orig.tar.gz' tinyxml2_7.0.0+dfsg.orig.tar.gz 359355 SHA256:1eceb87c311b5bf44b2b7351fa6ffda810605d7de402348157262543cf7185ef
'http://archive.ubuntu.com/ubuntu/pool/universe/t/tinyxml2/tinyxml2_7.0.0+dfsg-1build1.debian.tar.xz' tinyxml2_7.0.0+dfsg-1build1.debian.tar.xz 5832 SHA256:2544da0103456b5d9dd8e372cd6e4b0e74921ed878203c80d0319aa87d970f47
```

### `dpkg` source package: `tzdata=2020a-0ubuntu0.20.04`

Binary Packages:

- `tzdata=2020a-0ubuntu0.20.04`

Licenses: (parsed from: `/usr/share/doc/tzdata/copyright`)

- `ICU`

Source:

```console
$ apt-get source -qq --print-uris tzdata=2020a-0ubuntu0.20.04
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a-0ubuntu0.20.04.dsc' tzdata_2020a-0ubuntu0.20.04.dsc 2382 SHA512:71677b71676e7b751fa8f1c6b264922ff7d8c93032a8e30f24325d0ebfda47af10055fff8041cd7707e12e3bf7c6c781f3c1c5aca9b59205b8454df977f7d510
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz' tzdata_2020a.orig.tar.gz 397245 SHA512:2a2fc2e3ad8a6e4c574242296c847ad582c2c1d86add9c556e65c812d19b9528522e3c4dddb5239017091825d2acc5a2ccaf21dc41b900b6c300ef4264cc5a9d
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a.orig.tar.gz.asc' tzdata_2020a.orig.tar.gz.asc 833 SHA512:54c6539c4ed78f5ab8006f0a6ad99911a7002e742b185119bb3c77ba7c637777b2c7dce9867e16fd58088ad3f9d062d74c03f80e3225a599a3fc28581d87e366
'http://archive.ubuntu.com/ubuntu/pool/main/t/tzdata/tzdata_2020a-0ubuntu0.20.04.debian.tar.xz' tzdata_2020a-0ubuntu0.20.04.debian.tar.xz 164392 SHA512:e52770db0e044f219d8c56d366dcb4e9123beac8268d630017a1abde6f05cf84ef9091751c908545206c1b259cf75e0c50529a4e4d62c935645a6cc150f163bf
```

### `dpkg` source package: `ubuntu-keyring=2020.02.11.2`

Binary Packages:

- `ubuntu-keyring=2020.02.11.2`

Licenses: (parsed from: `/usr/share/doc/ubuntu-keyring/copyright`)

- `GPL`

Source:

```console
$ apt-get source -qq --print-uris ubuntu-keyring=2020.02.11.2
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2020.02.11.2.dsc' ubuntu-keyring_2020.02.11.2.dsc 1863 SHA256:f8544b69a2e982c3f588a588b306ae8f6eefea8194324680c0676244e251314f
'http://archive.ubuntu.com/ubuntu/pool/main/u/ubuntu-keyring/ubuntu-keyring_2020.02.11.2.tar.gz' ubuntu-keyring_2020.02.11.2.tar.gz 39180 SHA256:d2ee9deedb99f5a2b8bee2c0f9e85834638bfbc46d7a59edba7ce2bb6229bcec
```

### `dpkg` source package: `unixodbc=2.3.6-0.1build1`

Binary Packages:

- `libodbc1:amd64=2.3.6-0.1build1`

Licenses: (parsed from: `/usr/share/doc/libodbc1/copyright`)

- `GPL-2`
- `GPL-2+`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`

Source:

```console
$ apt-get source -qq --print-uris unixodbc=2.3.6-0.1build1
'http://archive.ubuntu.com/ubuntu/pool/main/u/unixodbc/unixodbc_2.3.6-0.1build1.dsc' unixodbc_2.3.6-0.1build1.dsc 2051 SHA256:5b1110505c41629471241b9ca35738b174a6db32db9d29d345bc7c3c507947f8
'http://archive.ubuntu.com/ubuntu/pool/main/u/unixodbc/unixodbc_2.3.6.orig.tar.gz' unixodbc_2.3.6.orig.tar.gz 2083106 SHA256:c7a1327a756653088f1f2c8566cd25689703eeb904728d1d971c9b31ed1a94db
'http://archive.ubuntu.com/ubuntu/pool/main/u/unixodbc/unixodbc_2.3.6-0.1build1.debian.tar.xz' unixodbc_2.3.6-0.1build1.debian.tar.xz 17988 SHA256:6b55abc12a3f22bf2836585d7ecdb9e82215661cab97af2a3c6c347632654c12
```

### `dpkg` source package: `util-linux=2.34-0.1ubuntu9.1`

Binary Packages:

- `bsdutils=1:2.34-0.1ubuntu9.1`
- `fdisk=2.34-0.1ubuntu9.1`
- `libblkid1:amd64=2.34-0.1ubuntu9.1`
- `libfdisk1:amd64=2.34-0.1ubuntu9.1`
- `libmount1:amd64=2.34-0.1ubuntu9.1`
- `libsmartcols1:amd64=2.34-0.1ubuntu9.1`
- `libuuid1:amd64=2.34-0.1ubuntu9.1`
- `mount=2.34-0.1ubuntu9.1`
- `util-linux=2.34-0.1ubuntu9.1`
- `uuid-dev:amd64=2.34-0.1ubuntu9.1`

Licenses: (parsed from: `/usr/share/doc/bsdutils/copyright`, `/usr/share/doc/fdisk/copyright`, `/usr/share/doc/libblkid1/copyright`, `/usr/share/doc/libfdisk1/copyright`, `/usr/share/doc/libmount1/copyright`, `/usr/share/doc/libsmartcols1/copyright`, `/usr/share/doc/libuuid1/copyright`, `/usr/share/doc/mount/copyright`, `/usr/share/doc/util-linux/copyright`, `/usr/share/doc/uuid-dev/copyright`)

- `BSD-2-clause`
- `BSD-3-clause`
- `BSD-4-clause`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `GPL-3+`
- `LGPL`
- `LGPL-2`
- `LGPL-2+`
- `LGPL-2.1`
- `LGPL-2.1+`
- `LGPL-3`
- `LGPL-3+`
- `MIT`
- `public-domain`

Source:

```console
$ apt-get source -qq --print-uris util-linux=2.34-0.1ubuntu9.1
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34-0.1ubuntu9.1.dsc' util-linux_2.34-0.1ubuntu9.1.dsc 4067 SHA512:cd98079e1a347852d84c0ebbfac643e7d7d66d7524a060a8bbb8df45153728dae957793b0cefacd4744fbbe4396efcd45e32beeaf8ab3afe347124373554ddbe
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34.orig.tar.xz' util-linux_2.34.orig.tar.xz 4974812 SHA512:2d0b76f63d32e7afb7acf61a83fabbfd58baa34ab78b3a331ce87f9c676a5fd71c56a493ded95039540d2c46b6048caaa38d7fb4491eb3d52d7b09dc54655cd7
'http://archive.ubuntu.com/ubuntu/pool/main/u/util-linux/util-linux_2.34-0.1ubuntu9.1.debian.tar.xz' util-linux_2.34-0.1ubuntu9.1.debian.tar.xz 91620 SHA512:b0ed129f1e7febe6a7370ef2becaca376b7bea478af084769f61c0b78cf4d3f5a0b5d8fe7c75017e74a8c4c6d22a37a2a9d7221c60822677220fa719d7f3b609
```

### `dpkg` source package: `xml-core=0.18+nmu1`

Binary Packages:

- `xml-core=0.18+nmu1`

Licenses: (parsed from: `/usr/share/doc/xml-core/copyright`)

- `GPL-2`
- `GPL-2+`

Source:

```console
$ apt-get source -qq --print-uris xml-core=0.18+nmu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xml-core/xml-core_0.18+nmu1.dsc' xml-core_0.18+nmu1.dsc 1632 SHA256:3b4bc034193f99750141611ae1c836c6b742c88ed0af1420051f3fcae30bf5ae
'http://archive.ubuntu.com/ubuntu/pool/main/x/xml-core/xml-core_0.18+nmu1.tar.xz' xml-core_0.18+nmu1.tar.xz 21312 SHA256:3e07592404b8ac38924fb650227cf5c9dcfc9933bd632eb4430635cd54898471
```

### `dpkg` source package: `xz-utils=5.2.4-1ubuntu1`

Binary Packages:

- `liblzma5:amd64=5.2.4-1ubuntu1`
- `xz-utils=5.2.4-1ubuntu1`

Licenses: (parsed from: `/usr/share/doc/liblzma5/copyright`, `/usr/share/doc/xz-utils/copyright`)

- `Autoconf`
- `GPL-2`
- `GPL-2+`
- `GPL-3`
- `LGPL-2`
- `LGPL-2.1`
- `LGPL-2.1+`
- `PD`
- `PD-debian`
- `config-h`
- `noderivs`
- `none`
- `permissive-fsf`
- `permissive-nowarranty`
- `probably-PD`

Source:

```console
$ apt-get source -qq --print-uris xz-utils=5.2.4-1ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1ubuntu1.dsc' xz-utils_5.2.4-1ubuntu1.dsc 2629 SHA512:09c0668c76bd1653460ae2207f2666785d6ec7bae424d168e2f5dc2c98d2c34b7f983963be27c39ac05df0ad76ccfe088b55a64a09319f26b785544d5c8ffb66
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz' xz-utils_5.2.4.orig.tar.xz 1053868 SHA512:00db7dd31a61541b1ce6946e0f21106f418dd1ac3f27cdb8682979cbc3bd777cd6dd1f04f9ba257a0a7e24041e15ca40d0dd5c130380dce62280af67a0beb97f
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4.orig.tar.xz.asc' xz-utils_5.2.4.orig.tar.xz.asc 879 SHA512:dbfce0556bc85545ce3566a01c25e4876f560409fc2d48f2dc382b10fbd2538c61d8f2c3667d86fc7313aec86c05e53926015000320f19615e97875adae42450
'http://archive.ubuntu.com/ubuntu/pool/main/x/xz-utils/xz-utils_5.2.4-1ubuntu1.debian.tar.xz' xz-utils_5.2.4-1ubuntu1.debian.tar.xz 135512 SHA512:9ec339da084b6aedd5d9dfafe879f7b90ae6dc473458dd8eda234e087f3aa80480b7b0792b54588d57e1b41a2c42f28ef87b8e6a8cd4bb51d43e2517f701724f
```

### `dpkg` source package: `zlib=1:1.2.11.dfsg-2ubuntu1`

Binary Packages:

- `zlib1g:amd64=1:1.2.11.dfsg-2ubuntu1`
- `zlib1g-dev:amd64=1:1.2.11.dfsg-2ubuntu1`

Licenses: (parsed from: `/usr/share/doc/zlib1g/copyright`, `/usr/share/doc/zlib1g-dev/copyright`)

- `Zlib`

Source:

```console
$ apt-get source -qq --print-uris zlib=1:1.2.11.dfsg-2ubuntu1
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu1.dsc' zlib_1.2.11.dfsg-2ubuntu1.dsc 2970 SHA256:2e56b0d54d841d974c96e6cc4361da7c75b1848cded85412cdb4b4bc7791233a
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg.orig.tar.gz' zlib_1.2.11.dfsg.orig.tar.gz 370248 SHA256:80c481411a4fe8463aeb8270149a0e80bb9eaf7da44132b6e16f2b5af01bc899
'http://archive.ubuntu.com/ubuntu/pool/main/z/zlib/zlib_1.2.11.dfsg-2ubuntu1.debian.tar.xz' zlib_1.2.11.dfsg-2ubuntu1.debian.tar.xz 49448 SHA256:11c13ba58bd033dbfd2c7408f4a4eaa02035e007dea79ae20f0db580eaa53c9c
```
